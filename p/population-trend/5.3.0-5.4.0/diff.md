# Comparing `tmp/population_trend-5.3.0.tar.gz` & `tmp/population_trend-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "population_trend-5.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "population_trend-5.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `population_trend-5.3.0.tar` & `population_trend-5.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      246 2023-07-13 22:03:10.707444 population_trend-5.3.0/README.md
--rw-r--r--   0        0        0      251 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/__init__.py
--rw-r--r--   0        0        0     7767 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/calculate_growth_rates.py
--rw-r--r--   0        0        0     2603 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/cli.py
--rw-r--r--   0        0        0      403 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/filter_data.py
--rw-r--r--   0        0        0     6056 2023-07-13 22:03:10.707444 population_trend-5.3.0/population_trend/population_growth_model.py
--rw-r--r--   0        0        0      495 2023-07-13 22:03:10.707444 population_trend-5.3.0/pyproject.toml
--rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 population_trend-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0      246 2023-07-14 20:05:38.787905 population_trend-5.4.0/README.md
+-rw-r--r--   0        0        0      251 2023-07-14 20:05:38.787905 population_trend-5.4.0/population_trend/__init__.py
+-rw-r--r--   0        0        0     8025 2023-07-14 20:05:38.787905 population_trend-5.4.0/population_trend/calculate_growth_rates.py
+-rw-r--r--   0        0        0     2603 2023-07-14 20:05:38.787905 population_trend-5.4.0/population_trend/cli.py
+-rw-r--r--   0        0        0      403 2023-07-14 20:05:38.787905 population_trend-5.4.0/population_trend/filter_data.py
+-rw-r--r--   0        0        0     6069 2023-07-14 20:05:38.787905 population_trend-5.4.0/population_trend/population_growth_model.py
+-rw-r--r--   0        0        0      495 2023-07-14 20:05:38.787905 population_trend-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0      713 1970-01-01 00:00:00.000000 population_trend-5.4.0/PKG-INFO
```

### Comparing `population_trend-5.3.0/population_trend/calculate_growth_rates.py` & `population_trend-5.4.0/population_trend/calculate_growth_rates.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,44 +101,49 @@
     testing=Bootstrap_from_time_series_parametrizer(blocks_length=2, N=100),
 )
 
 
 class Bootstrap_from_time_series:
     def __init__(self, bootstrap_parametrizer):
         self.parameters = bootstrap_parametrizer.parameters
-        self.lambdas_distribution, _ = self._calculate_distribution_and_interval()
+        self.lambdas_n0_distribution, _ = self._calculate_distribution_and_interval()
         self.season_series = self.parameters["dataframe"]["Temporada"]
         self.data_series = self.parameters["dataframe"][self.parameters["column_name"]]
         self.intervals = self.intervals_from_p_values_and_alpha()
-        self.lambdas = [interval[0] for interval in self.intervals]
+        self.interval_lambdas = [interval[0] for interval in self.intervals]
 
     def intervals_from_p_values_and_alpha(self):
-        p_value_mayor, p_value_menor = calculate_p_values(self.lambdas_distribution)
-        p_values = (p_value_mayor, p_value_menor)
+        p_values = self.get_p_values()
         intervals = calculate_intervals_from_p_values_and_alpha(
-            self.lambdas_distribution, p_values, self.parameters["alpha"]
+            self.lambdas_n0_distribution, p_values, self.parameters["alpha"]
         )
         return intervals
 
+    def get_p_values(self):
+        lambdas = [lambdas_n0[0] for lambdas_n0 in self.lambdas_n0_distribution]
+        p_value_mayor, p_value_menor = calculate_p_values(lambdas)
+        p_values = (p_value_mayor, p_value_menor)
+        return p_values
+
     def get_distribution(self):
-        return self.lambdas_distribution
+        return self.lambdas_n0_distribution
 
     def _calculate_distribution_and_interval(self):
-        lambdas_distribution, intervals = bootstrap_from_time_series(**self.parameters)
-        return lambdas_distribution, intervals
+        lambdas_n0_distribution, intervals = bootstrap_from_time_series(**self.parameters)
+        return lambdas_n0_distribution, intervals
 
     def get_inferior_central_and_superior_limit(self):
         inferior_limit, central, superior_limit = get_bootstrap_deltas(
-            self.lambdas, **{"decimals": 2}
+            self.interval_lambdas, **{"decimals": 2}
         )
         return inferior_limit, central, superior_limit
 
     def get_lambda_interval_latex_string(self):
         lambda_latex_string = generate_latex_interval_string(
-            self.lambdas, deltas=False, **{"decimals": 2}
+            self.interval_lambdas, deltas=False, **{"decimals": 2}
         )
         return lambda_latex_string
 
     def generate_season_interval(self):
         return "({}-{})".format(
             self.season_series.min(axis=0),
             self.season_series.max(axis=0),
@@ -160,23 +165,24 @@
             parameters[1],
         )
         return model
 
     def get_intermediate_lambdas(self):
         return [
             lambda_n0
-            for lambda_n0 in self.lambdas_distribution
+            for lambda_n0 in self.lambdas_n0_distribution
             if (lambda_n0[0] > self.intervals[0][0]) and (lambda_n0[0] < self.intervals[2][0])
         ]
 
     def save_intervals(self, output_path):
         json_dict = {
             "intervals": list(self.intervals),
             "lambda_latex_interval": self.get_lambda_interval_latex_string(),
-            "bootstrap_distribution": self.get_intermediate_lambdas(),
+            "p-values": self.get_p_values(),
+            "bootstrap_intermediate_distribution": self.get_intermediate_lambdas(),
         }
         with open(output_path, "w") as file:
             json.dump(json_dict, file)
 
 
 def calculate_growth_rates_table(bootstrap: Bootstrap_from_time_series_parametrizer):
     bootstraper = Bootstrap_from_time_series(bootstrap)
```

### Comparing `population_trend-5.3.0/population_trend/cli.py` & `population_trend-5.4.0/population_trend/cli.py`

 * *Files identical despite different names*

### Comparing `population_trend-5.3.0/population_trend/population_growth_model.py` & `population_trend-5.4.0/population_trend/population_growth_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(self, fit_data, json_parameters, interest_variable):
         self.intervals = json_parameters["intervals"]
         self.model_domain = calculate_model_domain(fit_data)
         self.interest_variable = interest_variable
         self.initial_population = lambda_calculator(
             fit_data["Temporada"], fit_data[self.interest_variable]
         )
-        self.bootstrap_distribution = json_parameters["bootstrap_distribution"]
+        self.bootstrap_distribution = json_parameters["bootstrap_intermediate_distribution"]
 
     def intern_model(self, i):
         return power_law(
             self.model_domain, self.bootstrap_distribution[i][0], self.bootstrap_distribution[i][1]
         )
 
     @property
```

### Comparing `population_trend-5.3.0/PKG-INFO` & `population_trend-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: population_trend
-Version: 5.3.0
+Version: 5.4.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/population_trend
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: population_trend Version: 5.3.0 Summary: A template
+Metadata-Version: 2.1 Name: population_trend Version: 5.4.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/population_trend Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 bootstrapping-tools==3.0.0 Requires-Dist: geci-plots Requires-Dist: typer
 [https://www.islas.org.mx/img/logo.svg] # Population trend Este repo lo usamos
 en lambdas y cormorant. Tiene la clase para graficas
```

