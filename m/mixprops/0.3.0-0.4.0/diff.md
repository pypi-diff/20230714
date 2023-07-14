# Comparing `tmp/mixprops-0.3.0.tar.gz` & `tmp/mixprops-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixprops-0.3.0.tar", max compression
+gzip compressed data, was "mixprops-0.4.0.tar", max compression
```

## Comparing `mixprops-0.3.0.tar` & `mixprops-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1064 2023-07-13 13:14:06.181738 mixprops-0.3.0/LICENSE
--rw-r--r--   0        0        0     2016 2023-07-13 13:14:06.181738 mixprops-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/__init__.py
--rw-r--r--   0        0        0     1549 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/cli.py
--rw-r--r--   0        0        0      205 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/constants.py
--rw-r--r--   0        0        0     9650 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/data/species_T_1000_6000.csv
--rw-r--r--   0        0        0     9140 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/data/species_T_200_1000.csv
--rw-r--r--   0        0        0      974 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/database.py
--rw-r--r--   0        0        0     4579 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/mixture.py
--rw-r--r--   0        0        0     1530 2023-07-13 13:14:24.209764 mixprops-0.3.0/mixprops/reference_conditions.py
--rw-r--r--   0        0        0     2399 2023-07-13 13:14:06.181738 mixprops-0.3.0/mixprops/species.py
--rw-r--r--   0        0        0      585 2023-07-13 13:14:06.181738 mixprops-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 mixprops-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 12:34:29.231803 mixprops-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2596 2023-07-14 12:34:29.231803 mixprops-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/__init__.py
+-rw-r--r--   0        0        0     1566 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/cli.py
+-rw-r--r--   0        0        0      228 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/constants.py
+-rw-r--r--   0        0        0     9650 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/data/species_T_1000_6000.csv
+-rw-r--r--   0        0        0     9140 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/data/species_T_200_1000.csv
+-rw-r--r--   0        0        0      974 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/database.py
+-rw-r--r--   0        0        0     4557 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/mixture.py
+-rw-r--r--   0        0        0      609 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/settings.py
+-rw-r--r--   0        0        0     2191 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/species.py
+-rw-r--r--   0        0        0     1340 2023-07-14 12:34:49.027946 mixprops-0.4.0/mixprops/state.py
+-rw-r--r--   0        0        0      320 2023-07-14 12:34:29.231803 mixprops-0.4.0/mixprops/units.py
+-rw-r--r--   0        0        0      630 2023-07-14 12:34:29.231803 mixprops-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 mixprops-0.4.0/PKG-INFO
```

### Comparing `mixprops-0.3.0/LICENSE` & `mixprops-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mixprops-0.3.0/mixprops/cli.py` & `mixprops-0.4.0/mixprops/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 import argparse
 
 import pandas as pd
 
 from mixprops.mixture import Mixture
-from mixprops.reference_conditions import ReferenceConditions
+from mixprops.settings import get_settings
+from mixprops.state import State
+
+settings = get_settings()
 
 
 def cli():
     parser = argparse.ArgumentParser(description="Mixture properties calculator.")
+    parser.add_argument("--units", type=str, required=False, help="System units")
     parser.add_argument(
-        "-rc",
-        "--conditions",
-        type=str,
-        required=True,
-        help="Reference conditions values.",
+        "--pressure-unit", type=str, required=False, help="Pressure unit"
     )
     parser.add_argument(
-        "-u", "--units", type=str, required=True, help="Reference conditions units."
+        "--state",
+        type=str,
+        required=True,
+        help="Mixture state",
     )
-    parser.add_argument("-s", "--species", type=str, required=True, help="Species.")
+    parser.add_argument("--species", type=str, required=True, help="Species")
     parser.add_argument(
-        "-sc",
         "--composition",
         type=str,
         required=True,
         help="Molar composition as fractions.",
     )
     args = parser.parse_args()
 
-    conditions = args.conditions.split(",")
-    units = args.units.split(",")
-
-    ref_conditions = ReferenceConditions(
-        absolute_pressure_unit=units[0],
-        temperature_unit=units[1],
-        absolute_pressure=float(conditions[0]),
-        temperature=float(conditions[1]),
+    if args.units:
+        settings.units = args.units
+    if args.pressure_unit:
+        settings.pressure_unit = args.pressure_unit
+
+    state = args.state.split(",")
+
+    state = State(
+        settings=settings,
+        pressure=float(state[0]),
+        temperature=float(state[1]),
     )
 
     species = args.species.split(",")
     composition = [float(mf) for mf in args.composition.split(",")]
 
     if len(species) != len(composition):
         raise ValueError("Species and fractions should be of the same length")
 
-    mixture = Mixture(
-        species=list(zip(species, composition)), reference_conditions=ref_conditions
-    )
+    mixture = Mixture(species=list(zip(species, composition)), state=state)
 
     df = pd.DataFrame.from_dict([mixture.model_dump()])
 
     print("")
     print(df.T.rename(columns={0: "Value"}))
     print("")
```

### Comparing `mixprops-0.3.0/mixprops/data/species_T_1000_6000.csv` & `mixprops-0.4.0/mixprops/data/species_T_1000_6000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.3.0/mixprops/data/species_T_200_1000.csv` & `mixprops-0.4.0/mixprops/data/species_T_200_1000.csv`

 * *Files identical despite different names*

### Comparing `mixprops-0.3.0/mixprops/database.py` & `mixprops-0.4.0/mixprops/database.py`

 * *Files identical despite different names*

### Comparing `mixprops-0.3.0/mixprops/mixture.py` & `mixprops-0.4.0/mixprops/mixture.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,77 +2,79 @@
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel, ConfigDict, Field, computed_field
 
 from mixprops.constants import R_U
 from mixprops.database import Database
-from mixprops.reference_conditions import ReferenceConditions
 from mixprops.species import MixtureSpecies
+from mixprops.state import State
+
+
+def is_valid_composition(number: float, total: float) -> bool:
+    return 0 <= number <= total
 
 
 class Mixture(BaseModel):
     species: List[Tuple[str, float]] = Field(repr=False, exclude=True)
-    reference_conditions: ReferenceConditions = Field(repr=False, exclude=True)
+    state: State = Field(repr=False, exclude=True)
     df: pd.DataFrame = Field(repr=False, exclude=True)
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def __init__(
         self,
         species: List[Tuple[str, float]],
-        reference_conditions: ReferenceConditions,
+        state: State,
     ):
+        total = 1.0
         composition = [spec[1] for spec in species]
 
-        if abs(sum(composition) - 1.0) > 1e-6:
-            raise ValueError(
-                "Invalid species composition, mole fractions should sum to 1"
-            )
+        if not all(is_valid_composition(value, total) for value in composition):
+            raise ValueError("Invalid species composition, expecting fraction format")
+
+        if abs(sum(composition) - total) > 1e-6:
+            raise ValueError(f"Invalid species composition, they should sum to {total}")
 
         db: Database = Database.from_file(
             file="species_T_200_1000.csv"
-            if reference_conditions.temperature <= 1000
+            if state.temperature <= 1000
             else "species_T_1000_6000.csv"
         )
         relevant_species: List[MixtureSpecies] = []
 
         for spec in species:
             relevant_spec = db.find_species(name=spec[0])
             relevant_species.append(
                 MixtureSpecies(
                     species=relevant_spec,
                     mole_fraction=spec[1],
-                    reference_conditions=reference_conditions,
+                    state=state,
                 )
             )
 
         temp_df = pd.DataFrame.from_records(
             data=[spec.model_dump() for spec in relevant_species]
         )
         species_df = pd.json_normalize(temp_df.species)
-        temp_df.drop(columns=["species", "reference_conditions"], inplace=True)
+        temp_df.drop(columns=["species", "state"], inplace=True)
         df = pd.concat([temp_df, species_df], axis=1)
         df["mass_fraction"] = df.mass / df.mass.sum()
         df["mass_ovr_mole_weight"] = df.mass_fraction / df.molecular_weight
-        super().__init__(
-            species=species, reference_conditions=reference_conditions, df=df
-        )
+        super().__init__(species=species, state=state, df=df)
 
     @computed_field
     @property
     def molecular_weight(self) -> np.float64:
         return self.df.mole_fraction @ self.df.molecular_weight
 
     @computed_field
     @property
     def density(self) -> np.float64:
-        return (self.reference_conditions.absolute_pressure) / (
-            R_U
-            * (self.reference_conditions.temperature)
-            * self.df.mass_ovr_mole_weight.sum()
+        return (self.state.pressure) / (
+            R_U * (self.state.temperature) * self.df.mass_ovr_mole_weight.sum()
         )
 
     @computed_field
     @property
     def specific_heat_capacity(self) -> np.float64:
         return self.df.mass_fraction @ self.df.heat_capacity
 
@@ -126,10 +128,10 @@
     @computed_field
     @property
     def speed_of_sound(self) -> np.float64:
         return np.sqrt(
             (
                 self.adiabatic_index
                 * (R_U / self.molecular_weight)
-                * (self.reference_conditions.temperature)
+                * (self.state.temperature)
             )
         )
```

### Comparing `mixprops-0.3.0/pyproject.toml` & `mixprops-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "mixprops"
-version = "0.3.0"
+version = "0.4.0"
 description = "Mixture properties calculator"
 authors = ["Oliver Aarnikoivu <oliveraarnikoivu@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["mixprops/data/*.csv"]
 
 [tool.poetry.scripts]
 mixprops = "mixprops.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 pydantic = "^2.0.2"
 pandas = "^2.0.3"
+pydantic-settings = "^2.0.1"
+pyyaml = "^6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 pre-commit = "^3.3.3"
```

### Comparing `mixprops-0.3.0/PKG-INFO` & `mixprops-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: mixprops
-Version: 0.3.0
+Version: 0.4.0
 Summary: Mixture properties calculator
 License: MIT
 Author: Oliver Aarnikoivu
 Author-email: oliveraarnikoivu@icloud.com
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 # mixprops
 
 [![CI](https://github.com/oaarnikoivu/mixprops/workflows/CI/badge.svg)](https://github.com/oaarnikoivu/mixprops/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/mixprops)](https://pypi.org/project/mixprops/)
 [![versions](https://img.shields.io/pypi/pyversions/mixprops.svg)](https://github.com/oaarnikoivu/mixprops)
@@ -25,68 +27,85 @@
 Mixture properties calculator.
 
 ## Installation
 
 ### Python
 
 ```bash
-pip install mixprops
+pip install mixprops --upgrade
 ```
 
-### CLI
+## Configuration
 
-Follow instructions from [pipx](https://github.com/pypa/pipx) to install `pipx`.
+Using a `settings.yaml` configuration file, you can specify the units system used for computation.
 
-```bash
-pipx install git+https://github.com/oaarnikoivu/mixprops.git
+### Available units systems:
+
+- `SI` - International System of Units
+- `SIC` - International System of Units with temperature in degrees Celsius (DEFAULT)
+- `IS` - Imperial Unit System (currently this only assumes a temperature in degrees Fahrenheit)
+
+You may also overwrite the default Pressure unit of Pascal:
+
+- `Pa` - Pascal
+- `kPa` - Kilopascal
+- `Mpa` - Megapascal
+- `bar` - bar
+
+### Example
+
+```yaml
+units: "SI" # International System of Units
+pressure_unit: "kPa" # Kilopascal
 ```
 
-## Usage
+## Properties
 
-### Python
+- `molecular_weight` - Molecular weight (g/mol)
+- `density` - Density (kg/m3)
+- `specific_heat_capacity` - Specific heat capacity (J/kg-K)
+- `viscosity` - Viscosity (kg/m-s)
+- `conductivity` - Thermal conductivity (W/m-K)
+- `speed_of_sound` - Speed of sound (m/s)
+- `adiabatic_index` - Adiabatic index
+
+## Supported species
+
+For the supported species, see the `.csv` files in the `mixprops/data` directory.
+
+## Examples
 
 ```python
 from mixprops.mixture import Mixture
-from mixprops.reference_conditions import ReferenceConditions
+from mixprops.state import State
 
 mixture = Mixture(
     species=[("O2", 0.21), ("N2", 0.79)],
-    reference_conditions=ReferenceConditions(
-        absolute_pressure_unit="Pa",
-        absolute_pressure=101325,
-        temperature_unit="C",
-        temperature=25
-    ))
+    state=State(pressure=101325, temperature=25))
 
 print(mixture.specific_heat_capacity)
-# 1011.338752
+# 1011.3387518918726
 ```
 
 ### CLI
 
+Follow instructions from [pipx](https://github.com/pypa/pipx) to install `pipx`.
+
 ```bash
-mixprops \
-    -rc 101325,25 \
-    -u Pa,C \
-    -s O2,N2 \
-    -sc 0.21,0.79
+pipx install git+https://github.com/oaarnikoivu/mixprops.git
 ```
 
-- rc = Reference conditions -> Absolute pressure,temperature
-- u = Reference condition units -> Pressure unit,temperature unit
-- s = Comma separated list of species by name or species -> O2,N2 or Oxygen,Nitrogen
-- sc = Species molar composition as comma separated mole fractions -> 0.21,0.79
-
-### Properties
-
-- `molecular_weight` - Molecular weight (g/mol)
-- `density` - Density (kg/m3)
-- `specific_heat_capacity` - Specific heat capacity (J/kg-K)
-- `viscosity` - Viscosity (kg/m-s)
-- `conductivity` - Thermal conductivity (W/m-K)
-- `speed_of_sound` - Speed of sound (m/s)
-- `adiabatic_index` - Adiabatic index
-
-### Supported species
+```bash
+mixprops \
+    --units SIC \
+    --pressure-unit Pa \
+    --state 101325,25 \
+    --species O2,N2 \
+    --composition 0.21,0.79
+```
 
-For the supported species, see the `.csv` files in the `mixprops/data` directory.
+- `--units` = Units system -> Optional, defaults to `SIC`
+- `--pressure-unit` = Pressure unit -> Optional, defaults to `Pa`
+- `--state` = Mixture state -> Absolute pressure,temperature
+- `--species` = Comma separated list of species by name or species -> O2,N2 or Oxygen,Nitrogen
+- `--composition` = Species molar composition as comma separated mole fractions -> 0.21,0.79
```

