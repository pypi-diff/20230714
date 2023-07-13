# Comparing `tmp/population_trend-5.2.0.tar.gz` & `tmp/population_trend-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-5.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-5.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-5.2.0.tar` & `population_trend-5.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1037 2023-07-07 21:37:02.983211 population_trend-5.2.0/README.md
--rw-r--r--   0        0        0      251 2023-07-07 21:37:02.983211 population_trend-5.2.0/population_trend/__init__.py
--rw-r--r--   0        0        0     7273 2023-07-07 21:37:02.983211 population_trend-5.2.0/population_trend/calculate_growth_rates.py
--rw-r--r--   0        0        0     2542 2023-07-07 21:37:02.983211 population_trend-5.2.0/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-07 21:37:02.983211 population_trend-5.2.0/population_trend/filter_data.py
--rw-r--r--   0        0        0     6056 2023-07-07 21:37:02.983211 population_trend-5.2.0/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-07 21:37:02.983211 population_trend-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 population_trend-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0      246 2023-07-13 22:03:10.707444 population_trend-5.3.0/README.md
+-rw-r--r--   0        0        0      251 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/__init__.py
+-rw-r--r--   0        0        0     7767 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/calculate_growth_rates.py
+-rw-r--r--   0        0        0     2603 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     6056 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-13 22:03:10.707444 population_trend-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 population_trend-5.3.0/PKG-INFO
```

### Comparing `population_trend-5.2.0/population_trend/calculate_growth_rates.py` & `population_trend-5.3.0/population_trend/calculate_growth_rates.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from bootstrapping_tools import (
-    lambda_calculator,
-    power_law,
     bootstrap_from_time_series,
-    get_bootstrap_deltas,
-    generate_latex_interval_string,
+    calculate_intervals_from_p_values_and_alpha,
     calculate_p_values,
+    generate_latex_interval_string,
+    get_bootstrap_deltas,
+    lambda_calculator,
+    power_law,
 )
 from matplotlib.ticker import MaxNLocator
 
 import json
 import matplotlib.pyplot as plt
 import numpy as np
 
@@ -76,42 +77,52 @@
     else:
         porcentaje_cambio = calculate_porcentual_diff(
             model.iloc[-1], cantidad_nidos["Maxima_cantidad_nidos"].iloc[0]
         )
     return porcentaje_cambio
 
 
-class Bootstrap_from_time_series_parameterizer:
-    def __init__(self, blocks_length=3, N=2000, column_name="Maxima_cantidad_nidos"):
+class Bootstrap_from_time_series_parametrizer:
+    def __init__(self, blocks_length=3, N=2000, column_name="Maxima_cantidad_nidos", alpha=0.05):
         self.parameters = dict(
             dataframe=None,
             column_name=column_name,
             N=N,
             return_distribution=True,
             blocks_length=blocks_length,
+            alpha=alpha,
         )
 
     def set_data(self, data):
         self.parameters["dataframe"] = data
 
 
 Bootstrap = dict(
-    default=Bootstrap_from_time_series_parameterizer(),
-    testing=Bootstrap_from_time_series_parameterizer(blocks_length=2, N=100),
+    default=Bootstrap_from_time_series_parametrizer(),
+    testing=Bootstrap_from_time_series_parametrizer(blocks_length=2, N=100),
 )
 
 
 class Bootstrap_from_time_series:
     def __init__(self, bootstrap_parametrizer):
         self.parameters = bootstrap_parametrizer.parameters
-        self.lambdas_distribution, self.intervals = self._calculate_distribution_and_interval()
+        self.lambdas_distribution, _ = self._calculate_distribution_and_interval()
         self.season_series = self.parameters["dataframe"]["Temporada"]
         self.data_series = self.parameters["dataframe"][self.parameters["column_name"]]
+        self.intervals = self.intervals_from_p_values_and_alpha()
         self.lambdas = [interval[0] for interval in self.intervals]
 
+    def intervals_from_p_values_and_alpha(self):
+        p_value_mayor, p_value_menor = calculate_p_values(self.lambdas_distribution)
+        p_values = (p_value_mayor, p_value_menor)
+        intervals = calculate_intervals_from_p_values_and_alpha(
+            self.lambdas_distribution, p_values, self.parameters["alpha"]
+        )
+        return intervals
+
     def get_distribution(self):
         return self.lambdas_distribution
 
     def _calculate_distribution_and_interval(self):
         lambdas_distribution, intervals = bootstrap_from_time_series(**self.parameters)
         return lambdas_distribution, intervals
 
@@ -163,15 +174,15 @@
             "lambda_latex_interval": self.get_lambda_interval_latex_string(),
             "bootstrap_distribution": self.get_intermediate_lambdas(),
         }
         with open(output_path, "w") as file:
             json.dump(json_dict, file)
 
 
-def calculate_growth_rates_table(bootstrap: Bootstrap_from_time_series_parameterizer):
+def calculate_growth_rates_table(bootstrap: Bootstrap_from_time_series_parametrizer):
     bootstraper = Bootstrap_from_time_series(bootstrap)
     df = bootstrap.parameters["dataframe"]
     model = bootstraper.xxfit_population_model()
     inferior_limit, central, superior_limit = bootstraper.get_inferior_central_and_superior_limit()
     lambda_latex_string = bootstraper.get_lambda_interval_latex_string()
     bootstrap_distribution = bootstraper.get_distribution()
     lambdas_distribution = [interval[0] for interval in bootstrap_distribution]
```

### Comparing `population_trend-5.2.0/population_trend/cli.py` & `population_trend-5.3.0/population_trend/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from population_trend.filter_data import filter_by_species_and_island
 from population_trend.population_growth_model import (
     Population_Trend_Model,
     Plotter_Population_Trend_Model,
 )
 from population_trend.calculate_growth_rates import (
-    Bootstrap_from_time_series_parameterizer,
+    Bootstrap_from_time_series_parametrizer,
     Bootstrap_from_time_series,
 )
 import pandas as pd
 import typer
 import json
 
 app = typer.Typer(help="Write filtered burrows data by species and island")
@@ -16,19 +16,23 @@
 
 @app.command(help="Write json with bootstrap intervals")
 def write_bootstrap_intervals_json(
     data_path: str = "data/processed/gumu_guadalupe_burrows.csv",
     blocks_length: int = 3,
     bootstrap_number: int = 2000,
     variable_of_interest: str = "Maxima_cantidad_nidos",
+    alpha: float = 0.05,
     output_path: str = "reports/non-tabular/gumu_guadalupe_boostrap_intervals.json",
 ):
     data = pd.read_csv(data_path)
-    parametrizer = Bootstrap_from_time_series_parameterizer(
-        blocks_length=blocks_length, N=bootstrap_number, column_name=variable_of_interest
+    parametrizer = Bootstrap_from_time_series_parametrizer(
+        blocks_length=blocks_length,
+        N=bootstrap_number,
+        column_name=variable_of_interest,
+        alpha=alpha,
     )
     parametrizer.set_data(data)
     bootstrap = Bootstrap_from_time_series(parametrizer)
     bootstrap.save_intervals(output_path)
 
 
 @app.command(help="Write csv with ouput-path")
```

### Comparing `population_trend-5.2.0/population_trend/population_growth_model.py` & `population_trend-5.3.0/population_trend/population_growth_model.py`

 * *Files identical despite different names*

