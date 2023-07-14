# Comparing `tmp/generation_models-0.2.3.tar.gz` & `tmp/generation_models-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generation_models-0.2.3.tar", max compression
+gzip compressed data, was "generation_models-0.2.4.tar", max compression
```

## Comparing `generation_models-0.2.3.tar` & `generation_models-0.2.4.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0    37936 2023-06-24 00:20:25.625866 generation_models-0.2.3/generation_models.py
--rw-r--r--   0        0        0      656 2023-06-24 00:20:25.628234 generation_models-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.3/setup.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-07-11 20:35:07.150247 generation_models-0.2.4/generation_models/.gitignore
+-rw-r--r--   0        0        0       47 2023-07-11 20:35:07.150247 generation_models-0.2.4/generation_models/__init__.py
+-rw-r--r--   0        0        0    39916 2023-07-14 17:54:43.208495 generation_models-0.2.4/generation_models/generation_models.py
+-rw-r--r--   0        0        0      653 2023-07-14 17:56:35.969091 generation_models-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 generation_models-0.2.4/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.4/PKG-INFO
```

### Comparing `generation_models-0.2.3/generation_models.py` & `generation_models-0.2.4/generation_models/generation_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,17 +205,37 @@
         return len(self.rtm[0])
 
 
 class MarketBase(BaseModel):
     """_"""
 
     energy_prices: t.Union[DARTPrices, t.List[float], DARTPriceScenarios]
-    reserve_markets: t.Optional[ReserveMarkets]
+    reserve_markets: t.Optional[ReserveMarkets] = None
     time_interval_mins: t.Optional[int] = 60
-    load_peak_reduction: t.Optional[LoadPeakReduction]
+    load_peak_reduction: t.Optional[LoadPeakReduction] = None
+    dam_award: t.Optional[t.List[float]] = None
+
+    @root_validator(skip_on_failure=True)
+    def validate_dam_award(cls, values):
+        if values["dam_award"] is not None:
+            assert isinstance(
+                values["energy_prices"], (DARTPrices, DARTPriceScenarios)
+            ), "When providing a dam_award, separate DAM and RTM prices are required."
+            if isinstance(values["energy_prices"], DARTPriceScenarios):
+                rtm_prices = values["energy_prices"].rtm[0]
+            else:
+                rtm_prices = values["energy_prices"].rtm
+            _check_time_interval(
+                sub_hourly=rtm_prices,
+                hourly=values["dam_award"],
+                time_interval_mins=values["time_interval_mins"],
+                subhourly_str="rtm prices",
+                hourly_str="dam awards",
+            )
+        return values
 
     @root_validator(skip_on_failure=True)
     def check_time_interval(cls, values):
         if isinstance(values["energy_prices"], DARTPrices):
             _check_time_interval(
                 values["energy_prices"].rtm,
                 values["energy_prices"].dam,
@@ -228,15 +248,20 @@
     @root_validator(skip_on_failure=True)
     def check_length(cls, values):
         if values["reserve_markets"]:
             if isinstance(values["energy_prices"], DARTPriceScenarios):
                 dam_prices = values["energy_prices"].dam[0]
             else:
                 dam_prices = values["energy_prices"].dam
-            _check_lengths({"dam prices": dam_prices, "reserve market data": values["reserve_markets"]})
+            _check_lengths(
+                {
+                    "dam prices": dam_prices,
+                    "reserve market data": values["reserve_markets"],
+                }
+            )
 
         if values["load_peak_reduction"]:
             _check_lengths(
                 {"rtm prices": values["energy_prices"].rtm, "peak reduction data": values["load_peak_reduction"]}
             )
         return values
 
@@ -858,38 +883,45 @@
             "DART": MarketConfig(da=BidOfferStrategy.quantity_only, rt=BidOfferStrategy.quantity_only),
         }[self]
 
 
 class BidOfferStrategy(str, Enum):
     quantity_only = "quantity-only"
     price_quantity = "price-quantity"
+    awarded = "awarded"
 
 
 class MarketConfig(BaseModel):
     """_"""
 
     da: t.Optional[BidOfferStrategy]
     rt: t.Optional[BidOfferStrategy]
 
     @validator("rt")
     def valid_rt_configs(cls, v):
-        if v == "price-quantity":
-            raise ValueError("rt price-quantity not yet implemented")
+        if v not in {BidOfferStrategy.quantity_only, None}:
+            raise ValueError("only quantity-only supported for RTM")
         return v
 
     @property
     def independent_dam(self) -> bool:
         return self.da is not None and self.rt is not None
 
     @property
     def value(self) -> str:
         """For symmetry with EnergyStrategy"""
         return json.dumps({"DAM": self.da.value, "RTM": self.rt.value})
 
 
+default_market_config = MarketConfig(
+    da=BidOfferStrategy.quantity_only,
+    rt=None,
+)
+
+
 class Solver(str, Enum):
     HiGHS = "HiGHS"
     GLPK = "GLPK"
     HiGHS_GLPK = "HiGHS-GLPK"
     GLPK_HiGHS = "GLPK-HiGHS"
 
 
@@ -906,40 +938,44 @@
     energy_strategy: t.Optional[t.Union[EnergyStrategy, MarketConfig]]
     dart: t.Optional[bool]
     uncertain_soe: bool = True
     dam_annual_cycle_limit: float = None
     no_virtual_trades: bool = False
     initial_soe: float = 0.0
     duration_requirement_on_discharge: bool = True  # True for ERCOT
+    no_stop_offers: bool = False  # just for comparing to competitors
     solver: t.Optional[Solver] = None
     solver_config: SolverConfig = SolverConfig()
 
     @root_validator(skip_on_failure=True)
-    def check_dam_annual_cycle_limit(cls, values):
-        if values["dam_annual_cycle_limit"] is not None and not (values["dart"] or values["energy_strategy"] == "DART"):
-            raise AssertionError("dart must be `true` if dam_annual_cycle_limit is set")
+    def coerce_strategy_to_market_config(cls, values):
+        assert not (values["dart"] is not None and values["energy_strategy"] is not None), (
+            "Only one of `dart` or `energy_strategy` may be provided. `dart` is deprecated; use `energy_strategy`"
+            " instead."
+        )
+        strategy = values["energy_strategy"]
+        if strategy is None:
+            strategy = EnergyStrategy.dart if values["dart"] else EnergyStrategy.da
+            values["dart"] = None
+        if isinstance(strategy, EnergyStrategy):
+            values["energy_strategy"] = strategy.to_market_config()
+
+        if not values["energy_strategy"].independent_dam:
+            if values["dam_annual_cycle_limit"] is not None:
+                raise ValueError("Must model separate dam and rtm markets if dam_annual_cycle_limit is set")
+            if values["no_virtual_trades"]:
+                raise ValueError("Must model separate dam and rtm markets if no_virtual_trades is set to True")
         return values
 
     @root_validator(skip_on_failure=True)
     def check_solver_config(cls, values):
         if values["solver_config"].solver_specific and (values["solver"] not in {"HiGHS", "GLPK"}):
             raise ValueError("solver_specific options may only be passed when using HiGHS or GLPK solver")
         return values
 
-    @root_validator(skip_on_failure=True)
-    def support_deprecated_dart(cls, values):
-        assert not (values["dart"] is not None and values["energy_strategy"] is not None), (
-            "Only one of `dart` or `energy_strategy` may be provided. `dart` is deprecated; use `energy_strategy`"
-            " instead."
-        )
-        if values["energy_strategy"] is None:
-            values["energy_strategy"] = EnergyStrategy.dart if values["dart"] else EnergyStrategy.da
-            values["dart"] = None
-        return values
-
 
 class MultiStorageInputs(StorageSolverOptions):
     """_"""
 
     batteries: t.List[BatteryParams]
 
     @validator("batteries")
@@ -1038,14 +1074,20 @@
         assert ("reg_up" in (values["reserve_markets"].up or dict())) and (
             "reg_down" in (values["reserve_markets"].down or dict())
         ), "when storage_inputs.symmetric_reg is True, both reg_up and reg_down reg markets must be provided"
 
     return values
 
 
+def _check_dam_award_against_config(values):
+    assert (values["dam_award"] is not None) == (
+        values["storage_inputs"].energy_strategy.da == BidOfferStrategy.awarded
+    ), "DAM award must be provided if and only if the DAM strategy is 'awarded'"
+
+
 @optional_discriminators(["pv_inputs"])
 class PVStorageModel(ImportExportLimitMixin, MarketBase):
     """_"""
 
     project_type: t.Optional[t.Literal["hybrid"]] = "hybrid"
     storage_inputs: MultiStorageInputs
     storage_coupling: StorageCoupling
@@ -1058,14 +1100,19 @@
         return self.pv_inputs.project_term
 
     @property
     def project_term_units(self) -> TermUnits:
         return self.pv_inputs.project_term_units
 
     @root_validator(skip_on_failure=True)
+    def check_dam_award_against_config(cls, values):
+        _check_dam_award_against_config(values)
+        return values
+
+    @root_validator(skip_on_failure=True)
     def check_time_intervals(cls, values):
         assert (
             values["time_interval_mins"] <= values["pv_inputs"].time_interval_mins
         ), "price time_interval_mins must less than or equal to pv time_interval_mins"
         return values
 
     @root_validator(skip_on_failure=True)
@@ -1104,14 +1151,19 @@
 
     project_type: t.Optional[t.Literal["storage"]] = "storage"
     storage_inputs: MultiStorageInputs
     downstream_system: t.Optional[DownstreamSystem]
     ambient_temp: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
+    def check_dam_award_against_config(cls, values):
+        _check_dam_award_against_config(values)
+        return values
+
+    @root_validator(skip_on_failure=True)
     def check_ambient_temp_length(cls, values):
         if values["ambient_temp"]:
             price_str, price = _get_price_str_and_price(values)
             _check_lengths({price_str: price, "ambient_temp": values["ambient_temp"]})
         return values
 
     @root_validator(skip_on_failure=True)
```

### Comparing `generation_models-0.2.3/pyproject.toml` & `generation_models-0.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "generation-models"
-version = "0.2.3"
+version = "0.2.4"
 description = "generation API data model"
 authors = ["battery_al <allenlawrence94@gmail.com>"]
-packages = [{include = "generation_models.py"}]
+packages = [{include = "generation_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

