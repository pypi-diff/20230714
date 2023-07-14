# Comparing `tmp/AutoCarver-5.0.2.tar.gz` & `tmp/AutoCarver-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.2.tar", last modified: Fri Jul 14 00:02:19 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.3.tar", last modified: Fri Jul 14 20:32:07 2023, max compression
```

## Comparing `AutoCarver-5.0.2.tar` & `AutoCarver-5.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.708739 AutoCarver-5.0.2/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39408 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26042 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.393093 AutoCarver-5.0.3/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.393093 AutoCarver-5.0.3/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41746 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.393093 AutoCarver-5.0.3/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 20:32:07.000000 AutoCarver-5.0.3/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:32:07.397094 AutoCarver-5.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-14 20:31:53.000000 AutoCarver-5.0.3/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.2/AutoCarver/auto_carver.py` & `AutoCarver-5.0.3/AutoCarver/auto_carver.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,24 +179,23 @@
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
             output_dtype=output_dtype,
             str_nan=str_nan,
+            str_default = str_default,
             dropna=dropna,
             copy=copy,
+            verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
-        self.dropna = dropna  # whether or not to group NaNs with other modalities
-        self.verbose = verbose
-        self.str_default = str_default
         self.min_carved_freq = min_carved_freq
         self.min_group_size = 1
         measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
         assert (
             sort_by in measures
         ), f"""Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
         self.sort_by = sort_by
@@ -273,15 +272,15 @@
             quantitative_features=self.quantitative_features,
             qualitative_features=self.qualitative_features,
             min_freq=self.min_freq,
             ordinal_features=self.ordinal_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             str_default=self.str_default,
-            copy=False,
+            copy=True,  # copying anyways, otherwise no discretization from start to finish
             verbose=self.verbose,
         )
         x_copy = discretizer.fit_transform(x_copy, y)
         if x_test_copy is not None:
             x_test_copy = discretizer.transform(x_test_copy, y_test)
         self.input_dtypes.update(discretizer.input_dtypes)  # saving data types
 
@@ -305,15 +304,15 @@
         # computing crosstabs for each feature on train/test
         xtabs = get_xtabs(self.features, x_copy, y, labels_orders)
         xtabs_test = get_xtabs(self.features, x_test_copy, y_test, labels_orders)
 
         # optimal butcketization/carving of each feature
         for n, feature in enumerate(self.features):
             if self.verbose:  # verbose if requested
-                print(f"\n---\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})")
+                print(f"\n------\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})\n---")
 
             # getting xtabs on train/test
             xtab = xtabs[feature]
             xtab_test = xtabs_test[feature]
             if self.verbose:  # verbose if requested
                 print(xtab)
 
@@ -323,26 +322,28 @@
             # getting best combination
             best_combination = self.get_best_combination(order, xtab, xtab_test=xtab_test)
 
             # checking that a suitable combination has been found
             if best_combination is not None:
                 order, xtab, xtab_test = best_combination
                 if self.verbose:  # verbose if requested
-                    print(xtab)
+                    print(xtab)  # TODO get the good labels
 
                 # updating label_orders
                 labels_orders.update({feature: order})
             
             # no suitable combination has been found -> removing feature
             else:
                 print(f"No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features.")
                 self.remove_feature(feature)
                 if feature in labels_orders:
                     labels_orders.pop(feature)
 
+            if self.verbose:  # verbose if requested
+                print("------\n")
 
         # converting potential labels into there respective values (quantiles)
         self.values_orders.update(
             convert_to_values(
                 features=self.features,
                 quantitative_features=self.quantitative_features,
                 values_orders=self.values_orders,
```

### Comparing `AutoCarver-5.0.2/AutoCarver/converters.py` & `AutoCarver-5.0.3/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.2/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.3/AutoCarver/discretizers/discretizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,21 +114,21 @@
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
             output_dtype='str',
             str_nan=str_nan,
+            str_default = str_default,
             copy=copy,
+            verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
-        self.str_default = str_default
-        self.verbose = verbose
     
     def remove_feature(self, feature: str) -> None:
         """Removes a feature from the Discretizer
 
         Parameters
         ----------
         feature : str
@@ -145,64 +145,71 @@
         Parameters
         ----------
         X : DataFrame
             _description_
         y : Series
             _description_
         """
+        # Checking for binary target and copying X 
+        x_copy = self.prepare_data(X, y)
+
         # [Qualitative features] Grouping qualitative features
         if len(self.qualitative_features) > 0:
             if self.verbose:  # verbose if requested
-                print("\n---\n[Discretizer] Fit Qualitative Features")
+                print("------\n[Discretizer] Fit Qualitative Features\n---")
 
             # grouping qualitative features
-            discretizer = QualitativeDiscretizer(
+            qualitative_discretizer = QualitativeDiscretizer(
                 qualitative_features=self.qualitative_features,
                 ordinal_features=self.ordinal_features,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 input_dtypes=self.input_dtypes,
                 str_nan=self.str_nan,
                 str_default=self.str_default,
-                copy=self.copy,
+                copy=False,  # always False as x_copy is already a copy (if requested)
                 verbose=self.verbose,
             )
-            discretizer.fit(X, y)
+            qualitative_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
-            self.values_orders.update(discretizer.values_orders)
+            self.values_orders.update(qualitative_discretizer.values_orders)
 
             # removing dropped features
             for feature in self.qualitative_features:
-                if feature not in discretizer.values_orders:
+                if feature not in qualitative_discretizer.values_orders:
                     self.remove_feature(feature)
+            if self.verbose:  # verbose if requested
+                print("------\n")
 
         # [Quantitative features] Grouping quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
-                print("\n---\n[Discretizer] Fit Quantitative Features")
+                print("------\n[Discretizer] Fit Quantitative Features\n---")
 
             # grouping quantitative features
-            discretizer = QuantitativeDiscretizer(
+            quantitative_discretizer = QuantitativeDiscretizer(
                 quantitative_features=self.quantitative_features,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 input_dtypes=self.input_dtypes,
                 str_nan=self.str_nan,
                 verbose=self.verbose,
             )
-            discretizer.fit(X, y)
+            quantitative_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
-            self.values_orders.update(discretizer.values_orders)
+            self.values_orders.update(quantitative_discretizer.values_orders)
 
             # removing dropped features
             for feature in self.quantitative_features:
-                if feature not in discretizer.values_orders:
+                if feature not in quantitative_discretizer.values_orders:
                     self.remove_feature(feature)
+            if self.verbose:  # verbose if requested
+                print("------\n")
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
 
 
@@ -277,25 +284,25 @@
         self.features = list(set(qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
         self.ordinal_features = list(set(ordinal_features))
 
         # class specific attributes
         self.min_freq = min_freq
-        self.str_default = str_default
-        self.verbose = verbose
 
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
             output_dtype='str',
             str_nan=str_nan,
+            str_default = str_default,
             copy=copy,
+            verbose=verbose,
         )
 
         # non-ordinal qualitative features
         self.non_ordinal_features = [
             feature for feature in self.qualitative_features if feature not in self.ordinal_features
         ]
 
@@ -338,25 +345,25 @@
             if self.verbose:
                 unexpected_dtypes = [typ for dtyp in dtypes[not_object] for typ in dtyp if typ != str]
                 print(
                     f"""Non-string features: {str(features_to_convert)}. Trying to convert them using type_discretizers.StringDiscretizer, otherwise convert them manually. Unexpected data types: {str(list(unexpected_dtypes))}."""
                 )
 
             # converting specified features into qualitative features
-            stringer = StringDiscretizer(features=features_to_convert, values_orders=self.values_orders)
-            x_copy = stringer.fit_transform(x_copy)
+            string_discretizer = StringDiscretizer(features=features_to_convert, values_orders=self.values_orders, verbose=self.verbose)
+            x_copy = string_discretizer.fit_transform(x_copy)
 
             # updating values_orders accordingly
-            self.values_orders.update(stringer.values_orders)
+            self.values_orders.update(string_discretizer.values_orders)
 
         # all known values for features
         known_values = {feature: values.values() for feature, values in self.values_orders.items()}
 
         # checking that all unique values in X are in values_orders
-        check_new_values(x_copy, self.ordinal_features, known_values)
+        check_new_values(x_copy, self.ordinal_features, known_values, self.str_nan, self.str_default)
 
         return x_copy
     
     def remove_feature(self, feature: str) -> None:
         """Removes a feature from the Discretizer
 
         Parameters
@@ -384,44 +391,46 @@
         Returns
         -------
         _type_
             _description_
         """
 
         # checking data before bucketization
-        Xc = self.prepare_data(X, y)
+        x_copy = self.prepare_data(X, y)
 
         # [Qualitative ordinal features] Grouping rare values into closest common one
         if len(self.ordinal_features) > 0:
-            discretizer = OrdinalDiscretizer(
+            ordinal_discretizer = OrdinalDiscretizer(
                 features=self.ordinal_features,
                 values_orders=self.values_orders,
                 min_freq=self.min_freq,
                 verbose=self.verbose,
                 str_nan=self.str_nan,
+                copy=False,
             )
-            discretizer.fit(Xc, y)
+            ordinal_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
-            self.values_orders.update(discretizer.values_orders)
+            self.values_orders.update(ordinal_discretizer.values_orders)
 
         # [Qualitative non-ordinal features] Grouping rare values into str_default '__OTHER__'
         if len(self.non_ordinal_features) > 0:
-            discretizer = DefaultDiscretizer(
-                self.non_ordinal_features,
+            default_discretizer = DefaultDiscretizer(
+                features=self.non_ordinal_features,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 str_nan=self.str_nan,
                 str_default=self.str_default,
                 verbose=self.verbose,
+                copy=False,
             )
-            discretizer.fit(Xc, y)
+            default_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
-            self.values_orders.update(discretizer.values_orders)
+            self.values_orders.update(default_discretizer.values_orders)
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
 
 
@@ -452,14 +461,15 @@
         quantitative_features: list[str],
         min_freq: float,
         *,
         values_orders: dict[str, GroupedList] = None,
         input_dtypes: Union[str, dict[str, str]] = "float",
         str_nan: str = "__NAN__",
         verbose: bool = False,
+        copy: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
         features : list[str]
             _description_
@@ -483,20 +493,20 @@
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=quantitative_features,
             values_orders=values_orders,
             input_dtypes=input_dtypes,
             output_dtype='str',
             str_nan=str_nan,
-            copy=True,
+            copy=copy,
+            verbose=verbose,
         )
 
         # class specific attributes
         self.min_freq = min_freq
-        self.verbose = verbose
 
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Checking data for bucketization"""
         # checking for binary target and copying X
         x_copy = super().prepare_data(X, y)
 
         # checking for quantitative columns
@@ -509,51 +519,53 @@
     def fit(self, X: DataFrame, y: Series) -> None:
         """Learning TRAIN distribution"""
 
         # checking data before bucketization
         x_copy = self.prepare_data(X, y)
 
         # [Quantitative features] Grouping values into quantiles
-        discretizer = QuantileDiscretizer(
+        quantile_discretizer = QuantileDiscretizer(
             self.features,
             min_freq=self.min_freq,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
-            copy=False,
+            copy=True,  # needs to be True so that it does not transform x_copy
+            verbose = self.verbose,
         )
-        x_copy = discretizer.fit_transform(x_copy, y)
+        x_copy = quantile_discretizer.fit_transform(x_copy, y)
 
         # storing orders of grouped features
-        self.values_orders.update(discretizer.values_orders)
+        self.values_orders.update(quantile_discretizer.values_orders)
 
         # [Quantitative features] Grouping rare quantiles into closest common one
-        #  -> can exist because of overrepresented values (values more frequent than 1/q)
+        #  -> can exist because of overrepresented values (values more frequent than min_freq)
         # searching for features with rare quantiles: computing min frequency per feature
         frequencies = x_copy[self.features].apply(
             min_value_counts, values_orders=self.values_orders, axis=0
         )
 
         # minimal frequency of a quantile
         q_min_freq = self.min_freq / 2
 
         # identifying features that have rare modalities
         has_rare = list(frequencies[frequencies <= q_min_freq].index)
 
         # Grouping rare modalities
         if len(has_rare) > 0:
-            discretizer = OrdinalDiscretizer(
+            ordinal_discretizer = OrdinalDiscretizer(
                 has_rare,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 str_nan=self.str_nan,
+                copy=False,
                 verbose=self.verbose,
                 input_dtypes=self.input_dtypes,
             )
-            discretizer.fit(x_copy, y)
+            ordinal_discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
-            self.values_orders.update(discretizer.values_orders)
+            self.values_orders.update(ordinal_discretizer.values_orders)
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
```

### Comparing `AutoCarver-5.0.2/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.3/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base tools to build simple buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
 from typing import Any, Dict, List, Union
 
 from json import dumps
-from numpy import array, inf, isfinite, nan, ndarray, select, sort
+from numpy import array, inf, isfinite, nan, ndarray, select, sort, floating, integer
 from pandas import DataFrame, Series, isna, notna, unique
 from sklearn.base import BaseEstimator, TransformerMixin
 
 
 def nan_unique(x: Series) -> list[Any]:
     """Unique non-NaN values.
 
@@ -55,15 +55,15 @@
     if isinstance(applied, DataFrame):
         converted = applied.to_dict(orient="list")
 
     return converted
 
 
 # TODO: remove known_values
-def check_new_values(X: DataFrame, features: list[str], known_values: dict[str, list[Any]]) -> None:
+def check_new_values(X: DataFrame, features: list[str], known_values: dict[str, list[Any]], str_nan: str, str_default: str) -> None:
     """Checks for new, unexpected values, in X
 
     Parameters
     ----------
     X : DataFrame
         New DataFrame (at transform time)
     features : list[str]
@@ -78,14 +78,16 @@
         result_type="expand",
     )
     uniques = applied_to_dict_list(uniques)
 
     # checking for unexpected values for each feature
     for feature in features:
         unexpected = [val for val in uniques[feature] if val not in known_values[feature]]
+        assert str_nan not in unexpected, "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_nan`. "
+        assert str_default not in unexpected, "It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_default`. "
         assert (
             len(unexpected) == 0
         ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was not provided. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
 
 
 def check_missing_values(
     X: DataFrame, features: list[str], known_values: dict[str, list[Any]]
@@ -116,34 +118,42 @@
             len(unexpected) == 0
         ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was provided but there are not matching value in provided X. You should check 'values_orders['{feature}']' for unwanted values."
 
 
 class GroupedList(list):
     """An ordered list that's extended with a dict."""
 
-    def __init__(self, iterable: Any = ()) -> None:
-        """An ordered list that historizes its elements' merges.
+    def __init__(self, iterable: Union[ndarray, dict, list, tuple] = (), order: list[Any] = None, content: dict[str, list[Any]] = None) -> None:
+        """An ordered list that historizes its elements' content.
 
         Parameters
         ----------
-        iterable : Any, optional
-            list, dict or GroupedList, by default ()
+        iterable : Union[ndarray, dict, list, tuple], optional
+            List-like or GroupedList, by default ()
+        order : list[Any], optional
+            Used when loading .json, ordering of values, by default None
+        content : dict[str, list[Any]], optional
+            Used when loading .json, (learned) content per value, by default None
         """
 
+        # initiating iterable from order and content # TODO: move list to an attribute?
+        if order is not None and content is not None:
+            iterable = {group: content[group] for group in order}
+
         # case -1: iterable is an array
         if isinstance(iterable, ndarray):
             iterable = list(iterable)
 
-        # case 0: iterable is the contained dict
+        # case 0: iterable is the content dict
         if isinstance(iterable, dict):
             # storing ordered keys of the dict
             keys = list(iterable)
 
-            # storing the values contained per key
-            self.contained = dict(iterable.items())
+            # storing the values content per key
+            self.content = dict(iterable.items())
 
             # checking that all values are only present once
             all_values = [val for _, values in iterable.items() for val in values]
             assert len(list(set(all_values))) == len(
                 all_values
             ), "A value is present in several keys (groups)"
 
@@ -156,56 +166,56 @@
                     for iter_key, values in iterable.items()
                     for val in values
                     if key != iter_key
                 ]
                 if key not in all_values:
                     # checking that key is missing from its values
                     if key not in iterable[key]:
-                        self.contained.update({key: self.contained[key] + [key]})
+                        self.content.update({key: self.content[key] + [key]})
                 # the key already is in another key (and its values are empty)
                 # the key as already been grouped
                 else:
-                    self.contained.pop(key)
+                    self.content.pop(key)
                     keys.remove(key)
 
             # initiating the list with those keys
             super().__init__(keys)
 
         # case 1: copying a GroupedList
-        elif hasattr(iterable, "contained"):
+        elif hasattr(iterable, "content"):
             # initiating the list with the provided list of keys
             super().__init__(iterable)
 
             # copying values associated to keys
-            self.contained = dict(iterable.contained.items())
+            self.content = dict(iterable.content.items())
 
         # case 2: initiating GroupedList from a list
         elif isinstance(iterable, list):
             # initiating the list with the provided list of keys
             super().__init__(iterable)
 
             # initiating the values with the provided list of keys
-            self.contained = {v: [v] for v in iterable}
+            self.content = {v: [v] for v in iterable}
 
     def get(self, key: Any) -> list[Any]:
-        """List of values contained in key
+        """List of values content in key
 
         Parameters
         ----------
         key : Any
             Group.
 
         Returns
         -------
         list[Any]
-            Values contained in key
+            Values content in key
         """
 
         # default to fing an element
-        found = self.contained.get(key)
+        found = self.content.get(key)
 
         return found
 
     def group(self, discarded: Any, kept: Any) -> None:
         """Groups the discarded value with the kept value
 
         Parameters
@@ -218,20 +228,20 @@
 
         # checking that those values are distinct
         if not is_equal(discarded, kept):
             # checking that those values exist in the list
             assert discarded in self, f"{discarded} not in list"
             assert kept in self, f"{kept} not in list"
 
-            # accessing values contained in each value
-            contained_discarded = self.contained.get(discarded)
-            contained_kept = self.contained.get(kept)
+            # accessing values content in each value
+            content_discarded = self.content.get(discarded)
+            content_kept = self.content.get(kept)
 
-            # updating contained dict
-            self.contained.update({kept: contained_discarded + contained_kept, discarded: []})
+            # updating content dict
+            self.content.update({kept: content_discarded + content_kept, discarded: []})
 
             # removing discarded from the list
             self.remove(discarded)
 
     def group_list(self, to_discard: list[Any], to_keep: Any) -> None:
         """Groups elements to_discard into values to_keep
 
@@ -252,30 +262,30 @@
         Parameters
         ----------
         new_value : Any
             New key to be added.
         """
 
         self += [new_value]
-        self.contained.update({new_value: [new_value]})
+        self.content.update({new_value: [new_value]})
 
-    def update(self, new_value: Dict[Any, list[Any]]) -> None:
+    def update(self, new_value: Dict[Any, list[Any]]) -> None:  # TODO: not working as expected
         """Updates the GroupedList via a dict
 
         Parameters
         ----------
         new_value : Dict[Any, list[Any]]
-            Dict of key, values to updated `contained` dict
+            Dict of key, values to updated `content` dict
         """
 
         # adding keys to the order if they are new values
         self += [key for key, _ in new_value.items() if key not in self]
 
-        # updating contained according to new_value
-        self.contained.update(new_value)
+        # updating content according to new_value
+        self.content.update(new_value)
 
     def sort(self):
         """Sorts the values of the list and dict (if any, NaNs are last).
 
         Returns
         -------
         GroupedList
@@ -313,29 +323,29 @@
         assert all(
             o in self for o in ordering
         ), f"Unknown values in ordering: {str([v for v in ordering if v not in self])}"
         assert all(
             s in ordering for s in self
         ), f"Missing value from ordering: {str([v for v in self if v not in ordering])}"
 
-        # ordering the contained
+        # ordering the content
         sorted = GroupedList({k: self.get(k) for k in ordering})
 
         return sorted
 
     def remove(self, value: Any) -> None:
         """Removes a value from the GroupedList
 
         Parameters
         ----------
         value : Any
             value to be removed
         """
         super().remove(value)
-        self.contained.pop(value)
+        self.content.pop(value)
 
     def pop(self, idx: int) -> None:
         """Pop a value from the GroupedList by index
 
         Parameters
         ----------
         idx : int
@@ -356,38 +366,38 @@
         -------
         Any
             Corresponding key (group)
         """
 
         found = [
             key
-            for key, values in self.contained.items()
+            for key, values in self.content.items()
             if any(is_equal(value, elt) for elt in values)
         ]
 
         if any(found):
             return found[0]
 
         return value
 
     def values(self) -> list[Any]:
-        """All values contained in all groups
+        """All values content in all groups
 
         Returns
         -------
         list[Any]
             List of all values in the GroupedList
         """
 
-        known = [value for values in self.contained.values() for value in values]
+        known = [value for values in self.content.values() for value in values]
 
         return known
 
     def contains(self, value: Any) -> bool:
-        """Checks if a value is contained in any group, also matches NaNs.
+        """Checks if a value is content in any group, also matches NaNs.
 
         Parameters
         ----------
         value : Any
             Value to search for
 
         Returns
@@ -447,16 +457,18 @@
         self,
         features: list[str],
         *,
         values_orders: dict[str, GroupedList] = None,
         input_dtypes: Union[str, dict[str, str]] = 'str',
         output_dtype: str = 'str',
         str_nan: str = None,
+        str_default: str = None,
         dropna: bool = True,
-        copy: bool = False,
+        copy: bool = True,
+        verbose: bool = True,
     ) -> None:
         """Initiates a Discretizer by dict of GroupedList
 
         Parameters
         ----------
         features : list[str]
             List of column names to be discretized
@@ -491,30 +503,41 @@
 
         # string value of numpy.nan
         self.str_nan = str_nan
 
         # whether or not to reinstate numpy nan after bucketization
         self.dropna = dropna
 
+        # string value of rare values
+        self.str_default = str_default
+
+        # whether to print info
+        self.verbose = verbose
+
         # identifying qualitative features by there type
         self.qualitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "str"
         ]
 
         # identifying quantitative features by there type
         self.quantitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "float"
         ]
 
         # for each feature, getting label associated to each value
         self.labels_per_values: dict[str, dict[Any, Any]]= {}  # will be initiated during fit
 
-    def get_labels_per_values(self) -> dict[str, dict[Any, Any]]:
+    def get_labels_per_values(self, output_dtype: str) -> dict[str, dict[Any, Any]]:
         """Creates a dict that contains, for each feature, for each value, the associated label
 
+        Parameters
+        ----------
+        output_dtype : str
+            Whether or not to convert the output to float.
+
         Returns
         -------
         dict[str, dict[Any, Any]]
             Dict of labels per values per feature
         """
         # initiating dict of labels per values per feature
         labels_per_values: dict[str, dict[Any, Any]] = {}
@@ -527,16 +550,20 @@
             # case 0: quantitative feature -> labels per quantile (removes str_nan)
             if feature in self.quantitative_features:
                 labels = get_labels(values, self.str_nan)
             # case 1: qualitative feature -> by default, labels are values
             else:
                 labels = [value for value in values if value != self.str_nan]  # (removing str_nan)
             
-            # case 2: requested float output -> converting to integers
-            if self.output_dtype == 'float':
+            # add NaNs if there are any
+            if self.str_nan in values:
+                labels += [self.str_nan]
+                
+            # requested float output (AutoCarver) -> converting to integers
+            if output_dtype == 'float':
                 labels = [n for n, _ in enumerate(labels)]
 
             # building label per value
             label_per_value: dict[Any, Any] = {}
             for group_of_values, label in zip(values, labels):
                 for value in values.get(group_of_values):
                     label_per_value.update({value: label})
@@ -608,22 +635,22 @@
             Model target, by default None
         """
         # checking that all features to discretize are in values_orders
         missing_features = [feature for feature in self.features if feature not in self.values_orders]
         assert len(missing_features) == 0, f"Missing values_orders for following features {str(missing_features)}."
 
         # for each feature, getting label associated to each value
-        self.labels_per_values = self.get_labels_per_values()
+        self.labels_per_values = self.get_labels_per_values(self.output_dtype)
 
         return self
 
     def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
-        the `GroupedList.contained` dict.
+        the `GroupedList.content` dict.
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after `features` attribute
         y : Series, optional
             Model target, by default None
@@ -637,30 +664,37 @@
         # copying dataframes
         x_copy = X
         if self.copy:
             x_copy = X.copy()
 
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
+            if self.verbose:  # verbose if requested
+                print(f" - [GroupedListDiscretizer] Transform Quantitative {str(self.quantitative_features)}")
             x_copy = self.transform_quantitative(x_copy, y)
 
         # transforming qualitative features
         if len(self.qualitative_features) > 0:
+            if self.verbose:  # verbose if requested
+                print(f" - [GroupedListDiscretizer] Transform Qualitative {str(self.qualitative_features)}")
             x_copy = self.transform_qualitative(x_copy, y)
         
         # reinstating nans
         if not self.dropna:
-            x_copy[self.features] = x_copy[self.features].replace(self.str_nan, nan)
+            for feature in self.features:
+                label_per_value = self.labels_per_values[feature]
+                if self.str_nan in label_per_value:  # checking for nans in the feature
+                    x_copy[feature] = x_copy[feature].replace(label_per_value[self.str_nan], nan)
 
         return x_copy
 
     def transform_quantitative(self, X: DataFrame, y: Series) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
-        the `GroupedList.contained` dict.
+        the `GroupedList.content` dict.
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after `values_orders` keys
         y : Series, optional
             Model target, by default None
@@ -687,38 +721,34 @@
                      feature_values.contains(self.str_nan)
                 ), f"Unexpected value! Missing values found for feature '{feature}' at transform step but not during fit. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
                 nan_value = feature_values.get_group(self.str_nan)
                 # checking that nans have been grouped to a quantile otherwise they are left as numpy.nan (for comparison purposes)
                 if nan_value != self.str_nan:
                     X.loc[nans, feature] = nan_value
 
-            # removing nans from quantiles and labels (can not mix str and floats for comparison purposes)
-            if self.str_nan in feature_values:  # filtering out nans if any
-                feature_values = [value for value in feature_values if value != self.str_nan]
-
             # list of masks of values to replace with there respective group
-            values_to_group = [X[feature] <= quantile for quantile in feature_values]
+            values_to_group = [X[feature] <= value for value in feature_values if value != self.str_nan]
 
             # corressponding group for each value
-            group_labels = [[self.labels_per_values[feature][value]] * x_len for value in feature_values]
+            group_labels = [[self.labels_per_values[feature][value]] * x_len for value in feature_values if value != self.str_nan]
 
             # checking for values to group
             if len(values_to_group) > 0:
                 X[feature] = select(values_to_group, group_labels, default=X[feature])
 
             # converting nans to there value
             if any(nans):
                 X.loc[nans, feature] = self.labels_per_values[feature].get(nan_value, self.str_nan)
 
         return X
 
     def transform_qualitative(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
-        the `GroupedList.contained` dict.
+        the `GroupedList.content` dict.
 
         Parameters
         ----------
         X : DataFrame
             Contains columns named after `values_orders` keys
         y : Series, optional
             Model target, by default None
@@ -729,93 +759,87 @@
             _description_
         """
         # filling up nans with specified value
         if self.str_nan:
             X[self.qualitative_features] = X[self.qualitative_features].fillna(self.str_nan)
 
         # checking that all unique values in X are in values_orders
-        check_new_values(X, self.qualitative_features, {feature: values.values() for feature, values in self.values_orders.items()})
+        check_new_values(X, self.qualitative_features, {feature: values.values() for feature, values in self.values_orders.items()}, self.str_nan, self.str_default)
 
         # replacing values for there corresponding label
         X = X.replace({feature: label_per_value for feature, label_per_value in self.labels_per_values.items() if feature in self.qualitative_features})           
 
         return X
     
     def to_json(self) ->  str:
         """Converts the GroupedListDiscretizer's values_orders to .json
 
         Returns
         -------
         str
             _description_
         """
-        # extracting contained dictionnaries
+        # extracting content dictionnaries
         content = {
             "features": self.features,
-            "values_ordres": self.values_orders,  # TODO: adapt maybe init GroupedList with {"values": values, "contained": values.contained} ?
+            "values_ordres": self.values_orders,  # TODO: adapt maybe init GroupedList with {"values": values, "content": values.content} ?
             "input_dtypes": self.input_dtypes,
             "output_dtype": self.output_dtype,
             "str_nan": self.str_nan,
             "copy": self.copy,
         }
-        # contained_orders = {feature: {"values": values, "contained": values.contained} for feature, values in self.values_orders.items()}
+        # content_orders = {feature: {"values": values, "content": values.content} for feature, values in self.values_orders.items()}
         # dumping as json
         return dumps(content)
     
     def summary(self) -> DataFrame:
         """Summarizes the data bucketization
 
         Returns
         -------
         DataFrame
             A summary of feature's values
         """
-        # getting quantitative labels
-        if any(self.quantitative_features):
-            print("converting to labels\n\n")
-            labels_orders = convert_to_labels(
-                self.features, self.quantitative_features, self.values_orders, self.str_nan, dropna=False
-            )
+        # raw label per value with output_dtype 'str'
+        raw_labels_per_values = self.get_labels_per_values(output_dtype='str')
+
         # initiating summaries
         summaries: list[dict[str, Any]] = []
         for feature in self.features:
-            init_summary = {'feature': feature}  # initiating feature summary
-            
-            # case 0: quantitative features
-            if feature in self.quantitative_features:
-                init_summary.update({'data_type': 'quantitative'})
-                # feature's modalities
-                modalities = labels_orders[feature]
-                # values included in each modality
-                contained = modalities.contained
-                
-                # adding nans
-                if self.values_orders[feature].contains(self.str_nan):
-                    nan_group = self.values_orders[feature].get_group(self.str_nan)
-                    contained.update({nan_group: contained[nan_group] + [self.str_nan]})
-
+            # adding each value/label 
+            for value, label in self.labels_per_values[feature].items():
+                # initiating feature summary (default value/label)
+                feature_summary = {'feature': feature, 'dtype': self.input_dtypes[feature], 'label': label, 'content': value}
+
+                # case 0: qualitative feature -> not adding floats and integers str_default
+                if feature in self.qualitative_features:
+                    if not isinstance(value, floating):  # checking for floats
+                        if not isinstance(value, integer):  # checking for ints
+                            if value != self.str_default:  # checking for str_default
+                                summaries += [feature_summary]
+
+                # case 1: quantitative feature -> take the raw label per value
+                elif feature in self.quantitative_features:
+                    feature_summary.update({'content': raw_labels_per_values[feature][value]})
+                    summaries += [feature_summary]
 
-            # case 1: quantitative features
-            else:
-                init_summary.update({'data_type': 'qualitative'})
-                # feature's modalities
-                modalities = self.values_orders[feature]
-                # values included in each modality
-                contained = modalities.contained
-            
-            # adding all modalities and there content
-            for modality in modalities:
-                modality_summary = {k: v for k, v in init_summary.items()}
-                modality_summary.update({"modality": modality, "values": contained[modality]})
-
-                # case 2: when the output_dtype == 'float'
-                #if self.output_dtype == 'float':
-                #    modality_summary.update({"modality": self.output_dtype[feature][modality]})
-
-                summaries += [modality_summary]
+        # adding nans for quantitative features (when nan has been grouped)
+        for feature in self.quantitative_features:
+            # initiating feature summary (no value/label)
+            feature_summary = {'feature': feature, 'dtype': self.input_dtypes[feature]}
+            # if there are nans -> if already added it will be dropped afterwards (unique content)
+            if self.str_nan in raw_labels_per_values[feature]:
+                nan_group = self.values_orders[feature].get_group(self.str_nan)
+                feature_summary.update({'label': self.labels_per_values[feature][nan_group], 'content': self.str_nan})
+                summaries += [feature_summary]
+
+        # aggregating unique values per label
+        summaries = DataFrame(summaries).groupby(['feature', 'dtype', 'label'])['content'].apply(lambda u: list(unique(u)))
+        # sorting and seting index
+        summaries = summaries.reset_index().sort_values(['dtype', 'feature']).set_index(['feature', 'dtype'])
 
         return summaries
 
 
 def convert_to_labels(
     features: list[str],
     quantitative_features: list[str],
@@ -873,15 +897,15 @@
 
     # updating feature orders (that keeps NaNs and quantiles)
     for feature in features:
         # initial complete ordering with NAN and quantiles
         order = values_orders[feature]
 
         # checking for grouped modalities
-        groups_to_discard = label_orders[feature].contained
+        groups_to_discard = label_orders[feature].content
 
         # grouping the raw quantile values
         for kept_value, group_to_discard in groups_to_discard.items():
             # for qualitative features grouping as is
             # for quantitative features getting quantile per alias
             if feature in quantitative_features:
                 # getting raw quantiles to be grouped
```

### Comparing `AutoCarver-5.0.2/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.3/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,20 @@
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=features,
             values_orders=values_orders,
             input_dtypes='str',
             output_dtype='str',
             str_nan=str_nan,
+            str_default = str_default,
             copy=copy,
+            verbose=verbose,
         )
         
         self.min_freq = min_freq
-        self.str_default = str_default
-        self.verbose = verbose
 
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Called during fit step
 
         Parameters
         ----------
         X : DataFrame
@@ -92,15 +92,15 @@
         # checks and initilizes values_orders
         for feature in self.features:
             # initiating features missing from values_orders
             if feature not in self.values_orders:
                 self.values_orders.update({feature: GroupedList(nan_unique(x_copy[feature]))})
 
         # checking that all unique values in X are in values_orders
-        check_new_values(x_copy, self.features, self.values_orders)
+        check_new_values(x_copy, self.features, self.values_orders, self.str_nan, self.str_default)  # TODO problem here
         # checking that all unique values in values_orders are in X
         check_missing_values(x_copy, self.features, self.values_orders)
 
         # adding NANS
         for feature in self.features:
             if any(x_copy[feature].isna()):
                 self.values_orders[feature].append(self.str_nan)
@@ -120,15 +120,15 @@
         y : Series
             _description_
         """
         # copying dataframe and checking data before bucketization
         x_copy = self.prepare_data(X, y)
         
         if self.verbose:  # verbose if requested
-            print(f" - [DefaultDiscretizer] Fit {', '.join(self.features)}")
+            print(f" - [DefaultDiscretizer] Fit {str(self.features)}")
 
         # computing frequencies of each modality
         frequencies = x_copy.apply(value_counts, normalize=True, axis=0)
 
         for feature in self.features:
             # sorting orders based on target rates
             order = self.values_orders[feature]
@@ -168,29 +168,159 @@
             # sorting order updating values_orders
             self.values_orders.update({feature: order.sort_by(new_order)})
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
+    
 
-class BaseQualitativeDiscretizer(GroupedListDiscretizer):
-    """TODO: to implement to mutualize prepare_data and remove_feature across qualitative discretizers"""
+class OrdinalDiscretizer(GroupedListDiscretizer):
+    """Discretizes ordered qualitative features into groups more frequent than min_freq.
+    NaNs are left untouched.
+
+    Modality is choosen amongst the preceding and following values in the provided order.
+    The choosen modality is:
+    - the closest in target rate
+    - or the one with the lowest frequency
+    """
 
     def __init__(
         self,
-        features: List[str],
-        values_orders: Dict[str, GroupedList],
+        features: list[str],
+        values_orders: dict[str, GroupedList],
+        min_freq: float,
         *,
+        str_nan: str = "__NAN__",
+        input_dtypes: Union[str, dict[str, str]] = "str",
         copy: bool = False,
-        input_dtypes: Union[str, Dict[str, str]] = None,
-        str_nan: str = None,
-        verbose: bool = False
-    ) -> None:
-        super().__init__(features, values_orders, copy=copy, input_dtypes=input_dtypes, str_nan=str_nan, verbose=verbose)
+        verbose: bool = False,
+    ):
+        """Initializes a OrdinalDiscretizer
+
+        Parameters
+        ----------
+        features : List[str]
+            List of column names to be discretized
+        values_orders : Dict[str, Any]
+            Dict of column names (keys) and modalities' associated order (values)
+        min_freq : float
+            Minimum frequency per modality. Less frequent modalities are grouped in the closest value of the order.
+        str_nan : str, optional
+            _description_, by default None
+        input_dtypes : Union[str, Dict[str, str]], optional
+            String of type to be considered for all features or
+            Dict of column names and associated types:
+            - if 'float' uses transform_quantitative
+            - if 'str' uses transform_qualitative,
+            default 'str'
+        copy : bool, optional
+            _description_, by default False
+        verbose : bool, optional
+            _description_, by default False
+        """
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=features,
+            values_orders=values_orders,
+            input_dtypes=input_dtypes,
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+            verbose=verbose,
+        )
+
+        # class specific attributes
+        self.min_freq = min_freq
+
+    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
+        """Called during fit step
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series
+            _description_
+
+        Returns
+        -------
+        DataFrame
+            _description_
+        """
+        # checking for binary target and copying X
+        x_copy = super().prepare_data(X, y)
+        # adding NANS
+        for feature in self.features:
+            if any(x_copy[feature].isna()):
+                values = self.values_orders[feature]
+                if not values.contains(self.str_nan):
+                    values.append(self.str_nan)
+                    self.values_orders.update({feature: values})
+
+        # removing NaNs if any already imputed -> grouping only non-nan values
+        if self.str_nan:
+            x_copy = x_copy.replace(self.str_nan, nan)
+
+        return x_copy
+
+    def fit(self, X: DataFrame, y: Series) -> None:
+        """Learns common modalities on the training set
+
+        Parameters
+        ----------
+        X : DataFrame
+            Training set that contains columns named after `values_orders` keys.
+        y : Series
+            Model target.
+        """
+        if self.verbose:  # verbose if requested
+            print(f" - [OrdinalDiscretizer] Fit {str(self.features)}")
+
+        # checking values orders
+        x_copy = self.prepare_data(X, y)
+
+        # getting label per value
+        labels_per_values = self.get_labels_per_values(output_dtype='str')
+
+        # converting potential quantiles into there labels
+        known_orders = convert_to_labels(
+            features=self.features,
+            quantitative_features=self.quantitative_features,
+            values_orders=self.values_orders,
+            str_nan=self.str_nan,
+            dropna=True,
+        )
+
+        # grouping rare modalities for each feature
+        common_modalities = x_copy[self.features].apply(
+            find_common_modalities,
+            y=y,
+            min_freq=self.min_freq,
+            values_orders=known_orders,
+            axis=0,
+            result_type="reduce",
+        )
+
+        # converting potential labels into there respective values (quantiles)
+        self.values_orders.update(
+            convert_to_values(
+                features=self.features,
+                quantitative_features=self.quantitative_features,
+                values_orders=self.values_orders,
+                label_orders=common_modalities,
+                str_nan=self.str_nan,
+            )
+        )
+
+        # discretizing features based on each feature's values_order
+        super().fit(x_copy, y)
+
+        return self
+
 
 class ChainedDiscretizer(GroupedListDiscretizer):
     """Chained Discretization based on a list of GroupedList."""
 
     def __init__(
         self,
         features: list[str],
@@ -229,14 +359,15 @@
         super().__init__(
             features=features,
             values_orders=values_orders,
             input_dtypes='str',
             output_dtype='str',
             str_nan=str_nan,
             copy=copy,
+            verbose=verbose,
         )
 
         self.min_freq = min_freq
 
         self.chained_orders = [GroupedList(values) for values in chained_orders]
 
         # parameters to handle missing/unknown values
@@ -244,15 +375,15 @@
 
         # known_values: all ordered values describe in each level of the chained_orders
         # starting off with first level 
         known_values = self.chained_orders[0].values()
         # adding each level
         for next_level in self.chained_orders[1:]:
             # highest value per group of the level
-            highest_ranking_value = {group: [value for value in values if value!=group][-1] for group, values in next_level.contained.items()}
+            highest_ranking_value = {group: [value for value in values if value!=group][-1] for group, values in next_level.content.items()}
             
             # adding next_level group to the order
             for group, highest_value in highest_ranking_value.items():
                 highest_index = known_values.index(highest_value)
                 known_values = known_values[:highest_index + 1] + [group] + known_values[highest_index + 1:]
         self.known_values = known_values
 
@@ -325,15 +456,15 @@
             # updating values_orders accordingly
             self.values_orders.update(stringer.values_orders)
 
         # all known values for features
         known_values = {feature: values.values() for feature, values in self.values_orders.items()}
 
         # checking that all unique values in X are in values_orders
-        check_new_values(x_copy, self.features, known_values)
+        check_new_values(x_copy, self.features, known_values, self.str_nan, self.str_default)
 
         # filling nans
         x_copy = x_copy.fillna(self.str_nan)
 
         return x_copy
     
     def fit(self, X: DataFrame, y: Series = None) -> None:
@@ -351,17 +482,17 @@
         _type_
             _description_
         """
         # filling nans
         x_copy = self.prepare_data(X, y)
 
         # iterating over each feature
-        for n, feature in enumerate(self.features):
-            if self.verbose:  # verbose if requested
-                print(f" - [ChainedDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
+        if self.verbose:  # verbose if requested
+            print(f" - [ChainedDiscretizer] Fit {str(self.features)}")
+        for feature in self.features:
 
             # computing frequencies of each modality
             frequencies = x_copy[feature].value_counts(normalize=True)
             values, frequencies = frequencies.index, frequencies.values
 
             # adding NaNs to the order if any
             order = self.values_orders[feature]
@@ -412,158 +543,14 @@
                 frequencies = x_copy[feature].value_counts(normalize=True)
                 values, frequencies = frequencies.index, frequencies.values
 
         super().fit(X, y)
 
         return self
 
-
-class OrdinalDiscretizer(GroupedListDiscretizer):
-    """Discretizes ordered qualitative features into groups more frequent than min_freq.
-    NaNs are left untouched.
-
-    Modality is choosen amongst the preceding and following values in the provided order.
-    The choosen modality is:
-    - the closest in target rate
-    - or the one with the lowest frequency
-    """
-
-    def __init__(
-        self,
-        features: list[str],
-        values_orders: dict[str, GroupedList],
-        min_freq: float,
-        *,
-        str_nan: str = "__NAN__",
-        input_dtypes: Union[str, dict[str, str]] = "str",
-        copy: bool = False,
-        verbose: bool = False,
-    ):
-        """Initializes a OrdinalDiscretizer
-
-        Parameters
-        ----------
-        features : List[str]
-            List of column names to be discretized
-        values_orders : Dict[str, Any]
-            Dict of column names (keys) and modalities' associated order (values)
-        min_freq : float
-            Minimum frequency per modality. Less frequent modalities are grouped in the closest value of the order.
-        str_nan : str, optional
-            _description_, by default None
-        input_dtypes : Union[str, Dict[str, str]], optional
-            String of type to be considered for all features or
-            Dict of column names and associated types:
-            - if 'float' uses transform_quantitative
-            - if 'str' uses transform_qualitative,
-            default 'str'
-        copy : bool, optional
-            _description_, by default False
-        verbose : bool, optional
-            _description_, by default False
-        """
-        # Initiating GroupedListDiscretizer
-        super().__init__(
-            features=features,
-            values_orders=values_orders,
-            input_dtypes=input_dtypes,
-            output_dtype='str',
-            str_nan=str_nan,
-            copy=copy,
-        )
-
-        self.min_freq = min_freq
-        self.verbose = verbose
-
-    def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
-        """Called during fit step
-
-        Parameters
-        ----------
-        X : DataFrame
-            _description_
-        y : Series
-            _description_
-
-        Returns
-        -------
-        DataFrame
-            _description_
-        """
-        # adding NANS
-        for feature in self.features:
-            if any(X[feature].isna()):
-                self.values_orders[feature].append(self.str_nan)
-
-        # removing NaNs if any already imputed
-        x_copy = X
-        if self.str_nan:
-            x_copy = x_copy.replace(self.str_nan, nan)
-
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (
-            1 in y_values
-        ), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-
-        return x_copy
-
-    def fit(self, X: DataFrame, y: Series) -> None:
-        """Learns common modalities on the training set
-
-        Parameters
-        ----------
-        X : DataFrame
-            Training set that contains columns named after `values_orders` keys.
-        y : Series
-            Model target.
-        """
-        if self.verbose:  # verbose if requested
-            print(f" - [OrdinalDiscretizer] Fit {', '.join(self.features)}")
-
-        # checking values orders
-        x_copy = self.prepare_data(X, y)
-
-        # converting potential quantiles into there labels
-        known_orders = convert_to_labels(
-            features=self.features,
-            quantitative_features=self.quantitative_features,
-            values_orders=self.values_orders,
-            str_nan=self.str_nan,
-            dropna=True,
-        )
-
-        # grouping rare modalities for each feature
-        common_modalities = x_copy[self.features].apply(
-            find_common_modalities,
-            y=y,
-            min_freq=self.min_freq,
-            values_orders=known_orders,
-            axis=0,
-            result_type="reduce",
-        )
-
-        # converting potential labels into there respective values (quantiles)
-        self.values_orders.update(
-            convert_to_values(
-                features=self.features,
-                quantitative_features=self.quantitative_features,
-                values_orders=self.values_orders,
-                label_orders=common_modalities,
-                str_nan=self.str_nan,
-            )
-        )
-
-        # discretizing features based on each feature's values_order
-        super().fit(x_copy, y)
-
-        return self
-
-
 def find_common_modalities(
     df_feature: Series,
     y: Series,
     min_freq: float,
     values_orders: dict[str, GroupedList],
     len_df: int = None,
 ) -> dict[str, Any]:
```

### Comparing `AutoCarver-5.0.2/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.3/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,32 +44,32 @@
         super().__init__(
             features=features,
             values_orders=values_orders,
             input_dtypes='float',
             output_dtype='str',
             str_nan=str_nan,
             copy=copy,
+            verbose=verbose,
         )
 
         self.min_freq = min_freq
         self.q = round(1 / min_freq)  # number of quantiles
-        self.verbose = verbose
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """_summary_
 
         Parameters
         ----------
         X : DataFrame
             _description_
         y : Series, optional
             _description_, by default None
         """
         if self.verbose:  # verbose if requested
-            print(f" - [QuantileDiscretizer] Fit {', '.join(self.features)}")
+            print(f" - [QuantileDiscretizer] Fit {str(self.features)}")
 
         # computing quantiles for the feature
         quantiles = applied_to_dict_list(X[self.features].apply(find_quantiles, q=self.q, axis=0))
 
         # storing ordering
         for feature in self.features:
             # Converting to a groupedlist
```

### Comparing `AutoCarver-5.0.2/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.0.3/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Base tools to convert values into specific types.
 """
 
-from numpy import float32
 from pandas import DataFrame, Series
 
 from .base_discretizers import GroupedList, GroupedListDiscretizer, nan_unique
 
 
 class StringDiscretizer(GroupedListDiscretizer):
     """Converts specified columns of a DataFrame into str.
@@ -16,15 +15,17 @@
     """
 
     def __init__(
         self,
         features: list[str],
         *,
         values_orders: dict[str, GroupedList] = None,
+        str_nan: str = '__NAN__',
         copy: bool = False,
+        verbose: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
         features : list[str]
             _description_
@@ -33,31 +34,39 @@
         """
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=features,
             values_orders=values_orders,
             input_dtypes="str",
             output_dtype="str",
+            str_nan=str_nan,
             copy=copy,
+            verbose=verbose,
         )
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """_summary_
 
         Parameters
         ----------
         X : DataFrame
             _description_
         y : Series, optional
             _description_, by default None
         """
+        if self.verbose:  # verbose if requested
+            print(f" - [StringDiscretizer] Fit {str(self.features)}")
+
+        # checking for binary target and copying X
+        x_copy = self.prepare_data(X, y)  # X[self.features].fillna(self.str_nan)
+
         # converting each feature's value
         for feature in self.features:
             # unique feature values
-            unique_values = nan_unique(X[feature])
+            unique_values = nan_unique(x_copy[feature])
             values_order = GroupedList(unique_values)
 
             # formatting values
             for value in unique_values:
                 # case 0: the value is an integer
                 if isinstance(value, float) and float.is_integer(value):
                     str_value = str(int(value))  # converting value to string
@@ -65,24 +74,27 @@
                 else:
                     str_value = str(value)
 
                 # checking for string values already in the order
                 if str_value not in values_order:
                     values_order.append(str_value)  # adding string value to the order
                     values_order.group(value, str_value)  # grouping integer value into the string value
+                
+            # adding str_nan
+            if any(x_copy[feature].isna()):
+                values_order.append(self.str_nan)
 
             # updating values_orders accordingly
             # case 0: non-ordinal features, updating as is (no order provided)
             if feature not in self.values_orders:
                 self.values_orders.update({feature: values_order})
-            # case 1: ordinal features, adding to contained dict (order provide)
+            # case 1: ordinal features, adding to content dict (order provided)
             else:
                 # currently known order (only with strings)
                 known_order = self.values_orders[feature]
-                known_order.update(values_order.contained)
-
+                known_order.update(values_order.content)
                 self.values_orders.update({feature: known_order})
 
         # discretizing features based on each feature's values_order
         super().fit(X, y)
 
         return self
```

### Comparing `AutoCarver-5.0.2/AutoCarver/feature_selector.py` & `AutoCarver-5.0.3/AutoCarver/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.2/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.3/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.2
+Version: 5.0.3
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.2/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.3/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.2/LICENSE` & `AutoCarver-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.2/PKG-INFO` & `AutoCarver-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.2
+Version: 5.0.3
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.2/README.md` & `AutoCarver-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.2/setup.py` & `AutoCarver-5.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.2",
+    version="5.0.3",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.0.2/tests/test_base_discretizers.py` & `AutoCarver-5.0.3/tests/test_base_discretizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 
 def test_grouped_list_init():
     """ Tests the initialization of a GroupedList"""
     
     # init by list
     test_list = ['1', '2', '3']
     groupedlist = GroupedList(test_list)
-    assert groupedlist == test_list, "When init by list, GroupedList.contained should have only one value per key"
-    assert groupedlist.contained == {'1': ['1'], '2': ['2'], '3': ['3']}, "When init by list, GroupedList.contained should have only one value per key: itself"
+    assert groupedlist == test_list, "When init by list, GroupedList.content should have only one value per key"
+    assert groupedlist.content == {'1': ['1'], '2': ['2'], '3': ['3']}, "When init by list, GroupedList.content should have only one value per key: itself"
     
     # init by dict
     test_dict = {'1': ['1', '4'], '2': ['2'], '3': ['3']}
     groupedlist = GroupedList(test_dict)
     assert groupedlist == ['1', '2', '3'], "When init by dict, all keys should be in the list"
-    assert groupedlist.contained == {'1': ['1', '4'], '2': ['2'], '3': ['3']},"When init by dict, all values should be in stored in the contained dict"
+    assert groupedlist.content == {'1': ['1', '4'], '2': ['2'], '3': ['3']},"When init by dict, all values should be in stored in the content dict"
 
     test_dict = {'1': ['1', '4'], '2': ['2'], '3': ['3'], '4': []}
     groupedlist = GroupedList(test_dict)
     assert groupedlist == ['1', '2', '3'], "When init by dict, keys that are in another key (group) should be popped"
-    assert groupedlist.contained == {'1': ['1', '4'], '2': ['2'], '3': ['3']},"When init by dict, all values should be in stored in the contained dict"
+    assert groupedlist.content == {'1': ['1', '4'], '2': ['2'], '3': ['3']},"When init by dict, all values should be in stored in the content dict"
 
     test_dict = {'1': ['1', '4'], '2': ['2'], '3': ['3'], '4': []}
     groupedlist = GroupedList(test_dict)
     assert groupedlist == ['1', '2', '3'], "When init by dict, keys that are in another key (group) should be popped"
-    assert groupedlist.contained == {'1': ['1', '4'], '2': ['2'], '3': ['3']},"When init by dict, all values should be in stored in the contained dict"
+    assert groupedlist.content == {'1': ['1', '4'], '2': ['2'], '3': ['3']},"When init by dict, all values should be in stored in the content dict"
 
     # check that a value can not be in several keys (groups)
     with raises(AssertionError):
         test_dict = {'1': ['1', '4'], '2': ['2'], '3': ['3'], '4': ['4']}
         groupedlist = GroupedList(test_dict)
     
     test_dict = {'1': ['1', '4'], '2': ['2'], '3': ['3'], '4': [], '5': []}
     groupedlist = GroupedList(test_dict)
     assert groupedlist == ['1', '2', '3', '5'], "When init by dict, keys that are in no key (group) should be kept in the list"
-    assert groupedlist.contained == {'1': ['1', '4'], '2': ['2'], '3': ['3'], '5': ['5']},"When init by dict, keys that are in no key (group) should be added to themselves"
+    assert groupedlist.content == {'1': ['1', '4'], '2': ['2'], '3': ['3'], '5': ['5']},"When init by dict, keys that are in no key (group) should be added to themselves"
     
     # init by copy
     groupedlist_copy = GroupedList(groupedlist)
     assert groupedlist_copy == ['1', '2', '3', '5'], "When init by GroupedList, GroupedList should be an exact copy"
-    assert groupedlist_copy.contained == {'1': ['1', '4'], '2': ['2'], '3': ['3'], '5': ['5']}, "When init by GroupedList, GroupedList should be an exact copy"
+    assert groupedlist_copy.content == {'1': ['1', '4'], '2': ['2'], '3': ['3'], '5': ['5']}, "When init by GroupedList, GroupedList should be an exact copy"
 
 
 def test_grouped_list_functions():
     """Tests GroupedList functions"""
     
     # init a groupedlist
     test_dict = {'1': ['1', '4'], '2': ['2'], '3': ['3'], '4': [], '5': []}
@@ -55,58 +55,58 @@
     # test get
     assert groupedlist.get('1') == ['1', '4']
     
     
     # test group
     groupedlist.group('1', '5')
     assert groupedlist == ['2', '3', '5']
-    assert groupedlist.contained == {'2': ['2'], '3': ['3'], '5': [ '1', '4', '5']}
+    assert groupedlist.content == {'2': ['2'], '3': ['3'], '5': [ '1', '4', '5']}
     with raises(AssertionError):
         groupedlist.group('7', '5')
         groupedlist.group('5', '8')
     
     # test group_list
     groupedlist.group_list(['2', '3'], '5')
     assert groupedlist == ['5']
-    assert groupedlist.contained == {'5': [ '3', '2', '1', '4', '5']}
+    assert groupedlist.content == {'5': [ '3', '2', '1', '4', '5']}
     
     # test append
     groupedlist.append('0')
     assert groupedlist == ['5', '0']
-    assert groupedlist.contained == {'5': [ '3', '2', '1', '4', '5'], '0': ['0']}
+    assert groupedlist.content == {'5': [ '3', '2', '1', '4', '5'], '0': ['0']}
     
     # test update
     groupedlist.update({'0': ['0', '7']})
     assert groupedlist == ['5', '0']
-    assert groupedlist.contained == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
+    assert groupedlist.content == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
     
     # test sort
     groupedlist = groupedlist.sort()
     assert groupedlist == ['0', '5']
-    assert groupedlist.contained == {'0': ['0', '7'], '5': [ '3', '2', '1', '4', '5']}
+    assert groupedlist.content == {'0': ['0', '7'], '5': [ '3', '2', '1', '4', '5']}
     
     # test sort_by
     groupedlist = groupedlist.sort_by(['5', '0'])
     assert groupedlist == ['5', '0']
-    assert groupedlist.contained == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
+    assert groupedlist.content == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
     with raises(AssertionError):
         groupedlist.sort_by(['5', '0', '1'])
         groupedlist.sort_by(['5'])
     
     # test remove
     groupedlist.append('15')
     groupedlist.remove('15')
     assert groupedlist == ['5', '0']
-    assert groupedlist.contained == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
+    assert groupedlist.content == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
     
     # test pop
     groupedlist.append('15')
     groupedlist.pop(len(groupedlist) - 1)
     assert groupedlist == ['5', '0']
-    assert groupedlist.contained == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
+    assert groupedlist.content == {'5': [ '3', '2', '1', '4', '5'], '0': ['0', '7']}
     
     # test get_group
     groupedlist.append('15')
     groupedlist.pop(len(groupedlist) - 1)
     assert groupedlist.get_group('3') == '5'
     assert groupedlist.get_group('0') == '0'
```

### Comparing `AutoCarver-5.0.2/tests/test_discretizers.py` & `AutoCarver-5.0.3/tests/test_discretizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,22 +49,22 @@
 
 
     quali_expected = {
         '__OTHER__': ['Category A', 'Category D', 'Category F', '__OTHER__'],
          'Category C': ['Category C'],
          'Category E': ['Category E'],
     }
-    assert discretizer.values_orders['Qualitative'].contained == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
+    assert discretizer.values_orders['Qualitative'].content == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
     quali_lownan_expected = {
         '__NAN__': ['__NAN__'],
         '__OTHER__': ['Category D', 'Category F', '__OTHER__'],
         'Category C': ['Category C'],
         'Category E': ['Category E'],
     }
-    assert discretizer.values_orders['Qualitative_lownan'].contained == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+    assert discretizer.values_orders['Qualitative_lownan'].content == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
 
     expected_ordinal = {
         'Low+': ['Low-', 'Low', 'Low+'],
         'Medium-': ['Medium-'],
         'Medium': ['Medium'],
         'High': ['Medium+', 'High-', 'High'],
         'High+': ['High+']
@@ -73,16 +73,16 @@
         'Low+': ['Low', 'Low-', 'Low+'],
         'Medium-': ['Medium-'],
         'Medium': ['Medium'],
         'High': ['Medium+', 'High-', 'High'],
         'High+': ['High+'],
         '__NAN__': ['__NAN__']
     }
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == expected_ordinal, "Values not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].contained == expected_ordinal_lownan, "NaNs should stay by themselves."
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal, "Values not correctly grouped"
+    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan, "NaNs should stay by themselves."
 
 def test_discretizer(x_train: DataFrame, x_test_1: DataFrame):
     """Tests Discretizer
 
     Parameters
     ----------
     x_train : DataFrame
@@ -125,22 +125,22 @@
 
 
     quali_expected = {
         '__OTHER__': ['Category A', 'Category D', 'Category F', '__OTHER__'],
         'Category C': ['Category C'],
         'Category E': ['Category E'],
     }
-    assert discretizer.values_orders['Qualitative'].contained == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
+    assert discretizer.values_orders['Qualitative'].content == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
     quali_lownan_expected = {
         '__NAN__' : ['__NAN__'],
         '__OTHER__': ['Category D', 'Category F', '__OTHER__'],
         'Category C': ['Category C'],
         'Category E': ['Category E'],
     }
-    assert discretizer.values_orders['Qualitative_lownan'].contained == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+    assert discretizer.values_orders['Qualitative_lownan'].content == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
 
     expected_ordinal = {
         'Low+': ['Low-', 'Low', 'Low+'],
         'Medium-': ['Medium-'],
         'Medium': ['Medium'],
         'High': ['Medium+', 'High-', 'High'],
         'High+': ['High+']
@@ -149,42 +149,42 @@
         'Low+': ['Low', 'Low-', 'Low+'],
         'Medium-': ['Medium-'],
         'Medium': ['Medium'],
         'High': ['Medium+', 'High-', 'High'],
         'High+': ['High+'],
         '__NAN__': ['__NAN__'],
     }
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == expected_ordinal, "Values not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].contained == expected_ordinal_lownan, "NaNs should stay by themselves."
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal, "Values not correctly grouped"
+    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan, "NaNs should stay by themselves."
 
     # Testing out qualitative with int/float values inside -> StringDiscretizer
     expected = {
         '2': [2.0, '2'],
         '4': [4.0, '4'],
         '1': [1.0, '1'],
         '3': [3.0, '3'],
         '__OTHER__': [0.5, '0.5', 6.0, '6', 5.0, '5', '__OTHER__']
     }
-    assert discretizer.values_orders["Discrete_Qualitative_rarevalue_noorder"].contained == expected, "Qualitative features with float values should be converted to string and there values stored in the values_orders"
+    assert discretizer.values_orders["Discrete_Qualitative_rarevalue_noorder"].content == expected, "Qualitative features with float values should be converted to string and there values stored in the values_orders"
     expected = {
         '2': [2, '2'],
         '4': [4, '4'],
         '1': [1, '1'],
         '3': [3, '3'],
         '__OTHER__': [7, '7', 6, '6', 5, '5', '__OTHER__']
     }
-    assert discretizer.values_orders["Discrete_Qualitative_noorder"].contained == expected, "Qualitative features with int values should be converted to string and there values stored in the values_orders"
+    assert discretizer.values_orders["Discrete_Qualitative_noorder"].content == expected, "Qualitative features with int values should be converted to string and there values stored in the values_orders"
     expected = {
         '2': ['1', 2.0, '2'],
         '3': [3.0, '3'],
         '4': [4.0, '4'],
         '5': [6.0, '6', 7.0, '7', 5.0, '5'],
         '__NAN__': ['__NAN__']
     }
-    assert discretizer.values_orders["Discrete_Qualitative_highnan"].contained == expected, "Ordinal qualitative features with int or float values that contain nan should be converted to string and there values stored in the values_orders"
+    assert discretizer.values_orders["Discrete_Qualitative_highnan"].content == expected, "Ordinal qualitative features with int or float values that contain nan should be converted to string and there values stored in the values_orders"
 
     # checking for inconsistancies in tranform
     for feature in discretizer.features:
         test_unique = x_test_discretized[feature].unique()
         train_unique = x_discretized[feature].unique()
         assert all(value in test_unique for value in train_unique), "Missing value from test (at transform step)"
         assert all(value in train_unique for value in test_unique), "Missing value from train (at transform step)"
```

### Comparing `AutoCarver-5.0.2/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.3/tests/test_qualitative_discretizers.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,35 +41,35 @@
     x_discretized = discretizer.fit_transform(x_train)
 
     expected = {'High+': ['High+'],
     'Best': ['High', 'High-', 'Highs', 'Best'],
     'Mediums': ['Medium+', 'Medium-', 'Mediums'],
     'Medium': ['Medium'],
     'Worst': ['Low+', 'Low', 'Low-', 'Lows', 'Worst']}
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == expected, "Values less frequent than min_freq should be grouped"
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected, "Values less frequent than min_freq should be grouped"
     assert discretizer.values_orders['Qualitative_Ordinal'] == ['Medium', 'Mediums', 'Worst', 'High+', 'Best'], "Order of ordinal features is wrong"
 
     expected = {'Low-': ['Low-'],
     'Low': ['Low'],
     'Low+': ['Low+'],
     'Medium-': ['Medium-'],
     'Medium': ['Medium'],
     'Medium+': ['Medium+'],
     'High-': ['High-'],
     'High': ['High'],
     'High+': ['High+']}
-    assert discretizer.values_orders['Qualitative_Ordinal_highnan'].contained == expected, "Not specified features should not be modified"
+    assert discretizer.values_orders['Qualitative_Ordinal_highnan'].content == expected, "Not specified features should not be modified"
 
     expected = {'Medium': ['Medium'],
     'High+': ['High+'],
     'Best': ['High', 'High-', 'Highs', 'Best'],
     'Mediums': ['Medium+', 'Medium-', 'Mediums'],
     'Worst': ['Low+', 'Low', 'Low-', 'Lows', 'Worst'],
     '__NAN__': ['__NAN__']}
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].contained == expected, "NaNs should be added to the order and missing values from the values_orders should be added (from chained_orders)"
+    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected, "NaNs should be added to the order and missing values from the values_orders should be added (from chained_orders)"
     assert discretizer.values_orders['Qualitative_Ordinal_lownan'] == ['Medium', 'Mediums', 'Worst', 'High+', 'Best', '__NAN__'], "Order of ordinal features is wrong"
 
     # testing that it does not work when there is a vale in values_orders missing from chained_orders
     with raises(AssertionError):
         values_orders = {
             "Qualitative_Ordinal_lownan": ['-Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
             "Qualitative_Ordinal_highnan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
@@ -150,47 +150,47 @@
         "Qualitative_lownan": groupedlist_lownan,
         "Qualitative_Ordinal": groupedlist_ordinal,
     }
 
     discretizer = DefaultDiscretizer(features, min_freq, values_orders=values_orders, copy=True)
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == groupedlist_ordinal.contained, "Column names of values_orders not provided if features should not be discretized."
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == groupedlist_ordinal.content, "Column names of values_orders not provided if features should not be discretized."
     quali_expected = {
         '__OTHER__': ['Category A', '__OTHER__'],
         'Category C': ['Category C'],
         'Category F': ['Category F'],
         'Category E': ['Category E'],
         'Category D': ['Category D']
     }
     quali_expected_order = ['Category D', '__OTHER__', 'Category F', 'Category C', 'Category E']
     assert discretizer.values_orders['Qualitative'] == quali_expected_order, "Incorrect ordering by target rate"
-    assert discretizer.values_orders['Qualitative'].contained == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
+    assert discretizer.values_orders['Qualitative'].content == quali_expected, "Values less frequent than min_freq should be grouped into default_value"
     quali_lownan_expected = {
         '__NAN__': ['__NAN__'],
         'Category C': ['Category C'],
         'Category F': ['Category F'],
         'Category E': ['Category E'],
         'Category D': ['Category D']
     }
     quali_lownan_expected_order = ['Category D', 'Category F', 'Category C', 'Category E', '__NAN__']
     assert discretizer.values_orders['Qualitative_lownan'] == quali_lownan_expected_order, "Incorrect ordering by target rate"
-    assert discretizer.values_orders['Qualitative_lownan'].contained == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+    assert discretizer.values_orders['Qualitative_lownan'].content == quali_lownan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
     quali_highnan_expected = {
         '__OTHER__': ['Category A', '__OTHER__'],
         'Category C': ['Category C'],
         '__NAN__': ['__NAN__'],
         'Category E': ['Category E'],
         'Category D': ['Category D']
     }
     quali_highnan_expected_order = ['Category D', '__OTHER__', 'Category C', 'Category E', '__NAN__']
     assert discretizer.values_orders['Qualitative_highnan'] == quali_highnan_expected_order, "Incorrect ordering by target rate"
-    assert discretizer.values_orders['Qualitative_highnan'].contained == quali_highnan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
+    assert discretizer.values_orders['Qualitative_highnan'].content == quali_highnan_expected, "If any, NaN values should be put into str_nan and kept by themselves"
 
-    assert discretizer.values_orders['Qualitative_grouped'].contained == groupedlist_grouped.contained, "Grouped values should keep there group"
+    assert discretizer.values_orders['Qualitative_grouped'].content == groupedlist_grouped.content, "Grouped values should keep there group"
 
 
 def test_ordinal_discretizer(x_train: DataFrame) -> None:
     """Tests OrdinalDiscretizer
 
     # TODO: add tests for quantitative features
 
@@ -240,16 +240,16 @@
         'Medium-': ['Medium-'],
         'Medium': ['Medium'],
         'Medium+': ['High-', 'Medium+'],
         'High': ['High'],
         'High+': ['High+'],
         '__NAN__': ['__NAN__']
     }
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == expected_ordinal_01, "Missing value in order not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].contained == expected_ordinal_lownan_01, "Missing value in order not correctly grouped or introduced nans."
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal_01, "Missing value in order not correctly grouped"
+    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan_01, "Missing value in order not correctly grouped or introduced nans."
 
     # minimum frequency per modality + apply(find_common_modalities) outputs a DataFrame
     min_freq = 0.08
 
     # discretizing features
     discretizer = OrdinalDiscretizer(features, values_orders, min_freq, copy=True)
     discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
@@ -265,9 +265,9 @@
         'Low+': ['Low', 'Low-', 'Low+'],
         'Medium-': ['Medium-'],
         'Medium': ['Medium'],
         'High': ['Medium+', 'High-', 'High'],
         'High+': ['High+'],
         '__NAN__': ['__NAN__']
     }
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == expected_ordinal_08, "Values not correctly grouped"
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].contained == expected_ordinal_lownan_08, "NaNs should stay by themselves."
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected_ordinal_08, "Values not correctly grouped"
+    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected_ordinal_lownan_08, "NaNs should stay by themselves."
```

### Comparing `AutoCarver-5.0.2/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.3/tests/test_quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.2/tests/test_type_discretizers.py` & `AutoCarver-5.0.3/tests/test_type_discretizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,50 +29,53 @@
     expected = {'2': [2, '2'],
     '4': [4, '4'],
     '3': [3, '3'],
     '7': [7, '7'],
     '1': [1, '1'],
     '5': [5, '5'],
     '6': [6, '6']}
-    assert discretizer.values_orders['Discrete_Qualitative_noorder'].contained == expected, "Not correctly converted for qualitative with integers"
+    assert discretizer.values_orders['Discrete_Qualitative_noorder'].content == expected, "Not correctly converted for qualitative with integers"
 
     expected = {'2': [2.0, '2'],
     '4': [4.0, '4'],
     '3': [3.0, '3'],
     '1': [1.0, '1'],
     '5': [5.0, '5'],
-    '6': [6.0, '6']}
-    assert discretizer.values_orders['Discrete_Qualitative_lownan_noorder'].contained == expected, "Not correctly converted for qualitative with integers and nans"
+    '6': [6.0, '6'],
+    '__NAN__': ['__NAN__']}
+    assert discretizer.values_orders['Discrete_Qualitative_lownan_noorder'].content == expected, "Not correctly converted for qualitative with integers and nans"
 
     expected = {'2': [2.0, '2'],
     '4': [4.0, '4'],
     '3': [3.0, '3'],
     '0.5': [0.5, '0.5'],
     '1': [1.0, '1'],
     '5': [5.0, '5'],
     '6': [6.0, '6']}
-    assert discretizer.values_orders['Discrete_Qualitative_rarevalue_noorder'].contained == expected, "Not correctly converted for qualitative with integers and floats"
+    assert discretizer.values_orders['Discrete_Qualitative_rarevalue_noorder'].content == expected, "Not correctly converted for qualitative with integers and floats"
 
     expected = {'Low-': ['Low-'],
     'Low': ['Low'],
     'Low+': ['Low+'],
     'Medium-': ['Medium-'],
     'Medium': ['Medium'],
     'Medium+': ['Medium+'],
     'High-': ['High-'],
     'High': ['High'],
-    'High+': ['High+']}
-    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].contained == expected, "No conversion for already string features"
+    'High+': ['High+'],
+    '__NAN__': ['__NAN__']}
+    assert discretizer.values_orders['Qualitative_Ordinal_lownan'].content == expected, "No conversion for already string features"
     
     expected = {'Low-': ['Low-'],
     'Low': ['Low'],
     'Low+': ['Low+'],
     'Medium-': ['Medium-'],
     'Medium': ['Medium'],
     'Medium+': ['Medium+'],
     'High-': ['High-'],
     'High': ['High'],
     'High+': ['High+']}
-    assert discretizer.values_orders['Qualitative_Ordinal'].contained == expected, "No conversion for not specified featues"
+    assert discretizer.values_orders['Qualitative_Ordinal'].content == expected, "No conversion for not specified featues"
 
-    expected = {'1': ['1'], '2': [2.0, '2'], '3': [3.0, '3'], '4': [4.0, '4'], '5': [5.0, '5'], '6': [6.0, '6'], '7': [7.0, '7']}
-    assert discretizer.values_orders['Discrete_Qualitative_highnan'].contained == expected, "Original order should be kept for ordinal features"
+    expected = {'1': ['1'], '2': [2.0, '2'], '3': [3.0, '3'], '4': [4.0, '4'], '5': [5.0, '5'], '6': [6.0, '6'], '7': [7.0, '7'],
+    '__NAN__': ['__NAN__']}
+    assert discretizer.values_orders['Discrete_Qualitative_highnan'].content == expected, "Original order should be kept for ordinal features"
```

