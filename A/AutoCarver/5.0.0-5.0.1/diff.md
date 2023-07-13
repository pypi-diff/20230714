# Comparing `tmp/AutoCarver-5.0.0.tar.gz` & `tmp/AutoCarver-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.0.tar", last modified: Thu Jul 13 12:07:18 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.1.tar", last modified: Thu Jul 13 23:13:38 2023, max compression
```

## Comparing `AutoCarver-5.0.0.tar` & `AutoCarver-5.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.910507 AutoCarver-5.0.0/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31613 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.910507 AutoCarver-5.0.0/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34585 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.910507 AutoCarver-5.0.0/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.967907 AutoCarver-5.0.1/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29716 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38974 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26042 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.0/AutoCarver/auto_carver.py` & `AutoCarver-5.0.1/AutoCarver/auto_carver.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,109 +161,93 @@
             _description_, by default 'float'
         dropna : bool, optional
             _description_, by default True
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default True
-        """        
-        # copying quantitative features and checking for duplicates
-        self.quantitative_features = quantitative_features[:]
-        assert len(list(set(quantitative_features))) == len(
-            quantitative_features
-        ), "Column duplicates in quantitative_features"
-
-        # copying qualitative features and checking for duplicates
-        self.qualitative_features = qualitative_features[:]
-        assert len(list(set(qualitative_features))) == len(
-            qualitative_features
-        ), "Column duplicates in qualitative_features"
-
-        # copying ordinal features and checking for duplicates
+        """
+        # Lists of features
+        self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
-        self.ordinal_features = ordinal_features[:]
-        assert len(list(set(ordinal_features))) == len(
-            ordinal_features
-        ), "Column duplicates in ordinal_features"
-
-        # initiating values_orders
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.ordinal_features = list(set(ordinal_features))
 
-        # list of all features
-        self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
-
-        # minimum frequency per base bucket
-        self.min_freq = min_freq
-        # maximum number of modality per feature
-        self.max_n_mod = max_n_mod
-        # whether or not to group NaNs with other modalities
-        self.dropna = dropna
+        # initializing input_dtypes
+        self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
+        self.input_dtypes.update({feature: "float" for feature in quantitative_features})
 
-        # association measure used to find the best groups
-        measures = ["tschuprowt", "cramerv"]
-        assert (
-            sort_by in measures
-        ), f"""{sort_by} not yet implemented. Choose
-                                        from: {', '.join(measures)}."""
-        self.sort_by = sort_by
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=self.features,
+            values_orders=values_orders,
+            input_dtypes=self.input_dtypes,
+            output_dtype=output_dtype,
+            str_nan=str_nan,
+            copy=copy,
+        )
 
-        self.copy = copy
+        # class specific attributes
+        self.min_freq = min_freq  # minimum frequency per base bucket
+        self.max_n_mod = max_n_mod  # maximum number of modality per feature
+        self.dropna = dropna  # whether or not to group NaNs with other modalities
         self.verbose = verbose
-        self.str_nan = str_nan
         self.str_default = str_default
-
         self.min_carved_freq = min_carved_freq
         self.min_group_size = 1
-        self.input_dtypes = {}
-        self.output_dtype = output_dtype
+        measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
+        assert (
+            sort_by in measures
+        ), f"""Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
+        self.sort_by = sort_by
 
     def prepare_data(
         self,
         X: DataFrame,
         y: Series,
         X_test: DataFrame = None,
         y_test: Series = None,
     ) -> Tuple[DataFrame, DataFrame]:
-        """Checks validity of provided data"""
+        """Checks validity of provided data
 
-        # preparing train sample
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (
-            1 in y_values
-        ), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-
-        # Copying DataFrame if requested
-        x_copy = X
-        if self.copy:
-            x_copy = X.copy()
-
-        # preparing test sample
-        # checking for binary target
-        if y_test is not None:
-            assert X_test is not None, "y_test was provided but X_test is missing"
-            y_values = unique(y_test)
-            assert (0 in y_values) & (
-                1 in y_values
-            ), "y_test must be a binary Series (int or float, not object)"
-            assert len(y_values) == 2, "y_test must be a binary Series (int or float, not object)"
-
-        # Copying DataFrame if requested
-        x_test_copy = X_test
-        if X_test is not None:
-            assert y_test is not None, "X_test was provided but y_test is missing"
-            if self.copy:
-                x_test_copy = X_test.copy()
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series
+            _description_
+        X_test : DataFrame, optional
+            _description_, by default None
+        y_test : Series, optional
+            _description_, by default None
+
+        Returns
+        -------
+        Tuple[DataFrame, DataFrame]
+            Copies of (X, X_test)
+        """
+        # Checking for binary target and copying X
+        x_copy = super().prepare_data(X, y)
+        x_test_copy = super().prepare_data(X_test, y_test)
 
         return x_copy, x_test_copy
 
+    def remove_feature(self, feature: str) -> None:
+        """Removes a feature from all instances 
+
+        Parameters
+        ----------
+        feature : str
+            Column name
+        """        
+        if feature in self.features:
+            super().remove_feature(feature)
+            if feature in self.ordinal_features:
+                self.ordinal_features.remove(feature)
+
     def fit(
         self,
         X: DataFrame,
         y: Series,
         X_test: DataFrame = None,
         y_test: Series = None,
     ) -> None:
@@ -304,15 +288,14 @@
         self.values_orders.update(discretizer.values_orders)
 
         # removing dropped features
         for feature in self.features:
             if feature not in discretizer.values_orders:
                 self.remove_feature(feature)
 
-
         # converting potential quantiles into there respective labels
         labels_orders = convert_to_labels(
             features=self.features,
             quantitative_features=self.quantitative_features,
             values_orders=self.values_orders,
             str_nan=self.str_nan,
             dropna=False,
@@ -363,52 +346,21 @@
                 quantitative_features=self.quantitative_features,
                 values_orders=self.values_orders,
                 label_orders=labels_orders,
                 str_nan=self.str_nan,
             )
         )
 
-        # TODO convert to float
         # TODO pretty displaying
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            input_dtypes=self.input_dtypes,
-            str_nan=self.str_nan,
-            verbose=self.verbose,
-            output_dtype=self.output_dtype,
-        )
         super().fit(X, y)
 
         return self
 
-    def remove_feature(self, feature: str) -> None:
-        """Removes a feature from all instances 
-
-        Parameters
-        ----------
-        feature : str
-            Column name
-        """        
-        
-        self.features.remove(feature)
-        if feature in self.values_orders:
-            self.values_orders.pop(feature)
-        if feature in self.input_dtypes:
-            self.input_dtypes.pop(feature)
-        if feature in self.qualitative_features:
-            self.qualitative_features.remove(feature)
-        if feature in self.ordinal_features:
-            self.ordinal_features.remove(feature)
-        if feature in self.quantitative_features:
-            self.quantitative_features.remove(feature)
-
     def get_best_combination(
         self,
         order: GroupedList,
         xtab: DataFrame,
         *,
         xtab_test: DataFrame = None,
     ) -> Tuple[GroupedList, DataFrame, DataFrame]:
@@ -433,15 +385,14 @@
             best_association = get_best_association(
                 raw_xtab,
                 combinations,
                 sort_by=self.sort_by,
                 xtab_test=raw_xtab_test,
                 verbose=self.verbose,
             )
-            # TODO test missing values in test
 
             # applying best_combination to order and xtabs
             if best_association is not None:
                 order = order_apply_combination(order, best_association["combination"])
                 xtab = xtab_apply_order(xtab, order)
                 xtab_test = xtab_apply_order(xtab_test, order)
```

### Comparing `AutoCarver-5.0.0/AutoCarver/converters.py` & `AutoCarver-5.0.1/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.0/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.1/AutoCarver/discretizers/discretizers.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,110 +57,92 @@
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
 
     def __init__(
         self,
-        quantitative_features: List[str],
-        qualitative_features: List[str],
+        quantitative_features: list[str],
+        qualitative_features: list[str],
         min_freq: float,
         *,
-        ordinal_features: List[str] = None,
-        values_orders: Dict[str, GroupedList] = None,
+        ordinal_features: list[str] = None,
+        values_orders: dict[str, GroupedList] = None,
         copy: bool = False,
         verbose: bool = False,
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
     ) -> None:
         """_summary_
 
         Parameters
         ----------
-        quantitative_features : List[str]
+        quantitative_features : list[str]
             _description_
-        qualitative_features : List[str]
+        qualitative_features : list[str]
             _description_
         min_freq : float
             _description_
-        ordinal_features : List[str], optional
+        ordinal_features : list[str], optional
             _description_, by default None
-        values_orders : Dict[str, GroupedList], optional
+        values_orders : dict[str, GroupedList], optional
             _description_, by default None
-        input_dtypes : Union[str, Dict[str, str]], optional
+        input_dtypes : Union[str, dict[str, str]], optional
             String of type to be considered for all features or
             Dict of column names and associated types:
             - if 'float' uses transform_quantitative
             - if 'str' uses transform_qualitative,
             default 'str'
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         str_nan : str, optional
             _description_, by default '__NAN__'
         str_default : str, optional
             _description_, by default '__OTHER__'
         """
-        self.quantitative_features = quantitative_features[:]
-        assert len(list(set(quantitative_features))) == len(
-            quantitative_features
-        ), "Column duplicates in quantitative_features"
-
-        self.qualitative_features = qualitative_features[:]
-        assert len(list(set(qualitative_features))) == len(
-            qualitative_features
-        ), "Column duplicates in qualitative_features"
-
+        # Lists of features per type
+        self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
-        assert len(list(set(ordinal_features))) == len(
-            ordinal_features
-        ), "Column duplicates in qualitative_features"
-        self.ordinal_features = ordinal_features[:]
-
-        # adding up all qualitative features
-        self.qualitative_features = list(set(self.qualitative_features + self.ordinal_features))
-
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {feature: GroupedList(value) for feature, value in values_orders.items()}
-
-        self.min_freq = min_freq
-
-        self.copy = copy
-        self.verbose = verbose
-        self.str_nan = str_nan
-        self.str_default = str_default
-
-        self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
+        self.ordinal_features = list(set(ordinal_features))
 
         # initializing input_dtypes
-        self.input_dtypes = {feature: "str" for feature in self.features}
+        self.input_dtypes = {feature: "str" for feature in qualitative_features + ordinal_features}
         self.input_dtypes.update({feature: "float" for feature in quantitative_features})
+
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=self.features,
+            values_orders=values_orders,
+            input_dtypes=self.input_dtypes,
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+        )
+
+        # class specific attributes
+        self.min_freq = min_freq
+        self.str_default = str_default
+        self.verbose = verbose
     
     def remove_feature(self, feature: str) -> None:
         """Removes a feature from the Discretizer
 
         Parameters
         ----------
         feature : str
             Column name of the feature
         """
-        self.features.remove(feature)
-        if feature in self.ordinal_features:
-            self.ordinal_features.remove(feature)
-        if feature in self.qualitative_features:
-            self.qualitative_features.remove(feature)
-        if feature in self.quantitative_features:
-            self.quantitative_features.remove(feature)
-        if feature in self.values_orders:
-            self.values_orders.pop(feature)
-        if feature in self.input_dtypes:
-            self.input_dtypes.pop(feature)
+        if feature in self.features:
+            super().remove_feature(feature)
+            self.features.remove(feature)
+            if feature in self.ordinal_features:
+                self.ordinal_features.remove(feature)
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """_summary_
 
         Parameters
         ----------
         X : DataFrame
@@ -198,40 +180,32 @@
         # [Quantitative features] Grouping quantitative features
         if len(self.quantitative_features) > 0:
             if self.verbose:  # verbose if requested
                 print("\n---\n[Discretizer] Fit Quantitative Features")
 
             # grouping quantitative features
             discretizer = QuantitativeDiscretizer(
-                features=self.quantitative_features,
+                quantitative_features=self.quantitative_features,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
+                input_dtypes=self.input_dtypes,
                 str_nan=self.str_nan,
-                copy=self.copy,
                 verbose=self.verbose,
             )
             discretizer.fit(X, y)
 
             # storing orders of grouped features
             self.values_orders.update(discretizer.values_orders)
 
             # removing dropped features
             for feature in self.quantitative_features:
                 if feature not in discretizer.values_orders:
                     self.remove_feature(feature)
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            verbose=self.verbose,
-            input_dtypes=self.input_dtypes,
-            str_nan=self.str_nan,
-        )
         super().fit(X, y)
 
         return self
 
 
 class QualitativeDiscretizer(GroupedListDiscretizer):
     """Automatic discretizing of categorical and categorical ordinal features.
@@ -260,77 +234,75 @@
         (smallest frequency or closest target rate), between the superior and inferior values (described
         by the `values_orders`).
         Exemple: for an `age` feature, `values_orders` could be `{'age': ['0-18', '18-30', '30-50', '50+']}`.
     """
 
     def __init__(
         self,
-        qualitative_features: List[str],
+        qualitative_features: list[str],
         min_freq: float,
         *,
-        ordinal_features: List[str] = None,
-        values_orders: Dict[str, Any] = None,
-        input_dtypes: Union[str, Dict[str, str]] = "str",
+        ordinal_features: list[str] = None,
+        values_orders: dict[str, GroupedList] = None,
+        input_dtypes: Union[str, dict[str, str]] = "str",
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
         copy: bool = False,
         verbose: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
-        qualitative_features : List[str]
+        qualitative_features : list[str]
             _description_
         min_freq : float
             _description_
-        ordinal_features : List[str], optional
+        ordinal_features : list[str], optional
             _description_, by default None
-        values_orders : Dict[str, Any], optional
+        values_orders : dict[str, GroupedList], optional
             _description_, by default None
-        input_dtypes : Union[str, Dict[str, str]], optional
+        input_dtypes : Union[str, dict[str, str]], optional
             String of type to be considered for all features or
             Dict of column names and associated types:
             - if 'float' uses transform_quantitative
             - if 'str' uses transform_qualitative,
             default 'str'
         str_nan : str, optional
             _description_, by default '__NAN__'
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         """
-        self.qualitative_features = list(set(qualitative_features))
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {
-            feature: GroupedList(values) for feature, values in values_orders.items()
-        }
+        # Lists of features
+        self.features = list(set(qualitative_features + ordinal_features))
         if ordinal_features is None:
             ordinal_features = []
         self.ordinal_features = list(set(ordinal_features))
+
+        # class specific attributes
         self.min_freq = min_freq
-        self.str_nan = str_nan
         self.str_default = str_default
-        self.copy = copy
         self.verbose = verbose
 
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=self.features,
+            values_orders=values_orders,
+            input_dtypes=input_dtypes,
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+        )
+
         # non-ordinal qualitative features
         self.non_ordinal_features = [
-            feature for feature in qualitative_features if feature not in self.ordinal_features
+            feature for feature in self.qualitative_features if feature not in self.ordinal_features
         ]
-        # all unique features
-        self.features = list(set(self.ordinal_features + self.non_ordinal_features))
-
-        if input_dtypes is None:
-            input_dtypes = {feature: "str" for feature in self.features}
-        if isinstance(input_dtypes, str):
-            input_dtypes = {feature: input_dtypes for feature in self.features}
-        self.input_dtypes = input_dtypes
 
     def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Prepares the data for bucketization, checks column types.
         Converts non-string columns into strings.
 
         Parameters
         ----------
@@ -340,16 +312,16 @@
             Model target, by default None
 
         Returns
         -------
         DataFrame
             Formatted X for bucketization
         """
-        # copying dataframe
-        x_copy = X.copy()
+        # checking for binary target, copying X
+        x_copy = super().prepare_data(X, y)
 
         # checking for ids (unique value per row)
         frequencies = x_copy[self.features].apply(
             lambda u: u.value_counts(normalize=True, dropna=False).drop(nan, errors='ignore').max(), axis=0
         )
         # for each feature, checking that at least one value is more frequent than min_freq
         for feature in self.features:
@@ -373,21 +345,14 @@
             # converting specified features into qualitative features
             stringer = StringDiscretizer(features=features_to_convert, values_orders=self.values_orders)
             x_copy = stringer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(stringer.values_orders)
 
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (
-            1 in y_values
-        ), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-
         # all known values for features
         known_values = {feature: values.values() for feature, values in self.values_orders.items()}
 
         # checking that all unique values in X are in values_orders
         check_new_values(x_copy, self.ordinal_features, known_values)
 
         return x_copy
@@ -396,24 +361,20 @@
         """Removes a feature from the Discretizer
 
         Parameters
         ----------
         feature : str
             Column name of the feature
         """
-        self.features.remove(feature)
-        if feature in self.ordinal_features:
-            self.ordinal_features.remove(feature)
-        if feature in self.non_ordinal_features:
-            self.non_ordinal_features.remove(feature)
-        if feature in self.qualitative_features:
-            self.qualitative_features.remove(feature)
-        if feature in self.values_orders:
-            self.values_orders.pop(feature)
-
+        if feature in self.features:
+            super().remove_feature(feature)
+            if feature in self.ordinal_features:
+                self.ordinal_features.remove(feature)
+            if feature in self.non_ordinal_features:
+                self.non_ordinal_features.remove(feature)
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """Learning TRAIN distribution
 
         Parameters
         ----------
         X : DataFrame
@@ -456,21 +417,14 @@
             )
             discretizer.fit(Xc, y)
 
             # storing orders of grouped features
             self.values_orders.update(discretizer.values_orders)
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            input_dtypes=self.input_dtypes,
-            str_nan=self.str_nan,
-        )
         super().fit(X, y)
 
         return self
 
 
 class QuantitativeDiscretizer(GroupedListDiscretizer):
     """Automatic discretizing of continuous features.
@@ -492,107 +446,94 @@
         cut in q=5 quantiles.
         Recommandation: `q` should be set from 10 (faster) to 20 (preciser).
 
     """
 
     def __init__(
         self,
-        features: List[str],
+        quantitative_features: list[str],
         min_freq: float,
         *,
-        values_orders: Dict[str, Any] = None,
-        input_dtypes: Union[str, Dict[str, str]] = "float",
+        values_orders: dict[str, GroupedList] = None,
+        input_dtypes: Union[str, dict[str, str]] = "float",
         str_nan: str = "__NAN__",
-        copy: bool = False,
         verbose: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
-        features : List[str]
+        features : list[str]
             _description_
         min_freq : float
             _description_
-        values_orders : Dict[str, Any], optional
+        values_orders : dict[str, GroupedList], optional
             _description_, by default None
-        input_dtypes : Union[str, Dict[str, str]], optional
+        input_dtypes : Union[str, dict[str, str]], optional
             String of type to be considered for all features or
             Dict of column names and associated types:
             - if 'float' uses transform_quantitative
             - if 'str' uses transform_qualitative,
             default 'str'
         str_nan : str, optional
             _description_, by default '__NAN__'
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         """
-        self.features = list(set(features))
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {
-            feature: GroupedList(values) for feature, values in values_orders.items()
-        }
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=quantitative_features,
+            values_orders=values_orders,
+            input_dtypes=input_dtypes,
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=True,
+        )
+
+        # class specific attributes
         self.min_freq = min_freq
-        self.str_nan = str_nan
-        self.copy = copy
         self.verbose = verbose
 
-        if input_dtypes is None:
-            input_dtypes = {feature: "float" for feature in self.features}
-        if isinstance(input_dtypes, str):
-            input_dtypes = {feature: input_dtypes for feature in self.features}
-        self.input_dtypes = input_dtypes
-
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Checking data for bucketization"""
+        # checking for binary target and copying X
+        x_copy = super().prepare_data(X, y)
 
         # checking for quantitative columns
-        dtypes = X[self.features].applymap(type).apply(unique)
+        dtypes = x_copy[self.features].applymap(type).apply(unique)
         not_numeric = dtypes.apply(lambda u: str in u)
         assert all(~not_numeric), f"Non-numeric features: {str(list(not_numeric[not_numeric].index))}"
 
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (
-            1 in y_values
-        ), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-
-        # copying dataframe
-        Xc = X.copy()
-
-        return Xc
+        return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """Learning TRAIN distribution"""
 
         # checking data before bucketization
-        Xc = self.prepare_data(X, y)
+        x_copy = self.prepare_data(X, y)
 
         # [Quantitative features] Grouping values into quantiles
         discretizer = QuantileDiscretizer(
             self.features,
             min_freq=self.min_freq,
             values_orders=self.values_orders,
-            verbose=self.verbose,
             str_nan=self.str_nan,
             copy=False,
         )
-        Xc = discretizer.fit_transform(Xc, y)
+        x_copy = discretizer.fit_transform(x_copy, y)
 
         # storing orders of grouped features
         self.values_orders.update(discretizer.values_orders)
 
         # [Quantitative features] Grouping rare quantiles into closest common one
         #  -> can exist because of overrepresented values (values more frequent than 1/q)
         # searching for features with rare quantiles: computing min frequency per feature
-        frequencies = Xc[self.features].apply(
+        frequencies = x_copy[self.features].apply(
             min_value_counts, values_orders=self.values_orders, axis=0
         )
 
         # minimal frequency of a quantile
         q_min_freq = self.min_freq / 2
 
         # identifying features that have rare modalities
@@ -604,23 +545,16 @@
                 has_rare,
                 min_freq=self.min_freq,
                 values_orders=self.values_orders,
                 str_nan=self.str_nan,
                 verbose=self.verbose,
                 input_dtypes=self.input_dtypes,
             )
-            discretizer.fit(Xc, y)
+            discretizer.fit(x_copy, y)
 
             # storing orders of grouped features
             self.values_orders.update(discretizer.values_orders)
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            input_dtypes=self.input_dtypes,
-            str_nan=self.str_nan,
-        )
         super().fit(X, y)
 
         return self
```

### Comparing `AutoCarver-5.0.0/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.1/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Base tools to build simple buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
 from typing import Any, Dict, List, Union
 
+from json import dumps
 from numpy import array, inf, isfinite, nan, ndarray, select, sort
 from pandas import DataFrame, Series, isna, notna, unique
 from sklearn.base import BaseEstimator, TransformerMixin
 
 
-def nan_unique(x: Series) -> List[Any]:
+def nan_unique(x: Series) -> list[Any]:
     """Unique non-NaN values.
 
     Parameters
     ----------
     x : Series
         Values to be deduplicated.
 
@@ -28,15 +29,15 @@
 
     # filtering out nans
     uniques = [u for u in uniques if notna(u)]
 
     return uniques
 
 
-def applied_to_dict_list(applied: Union[DataFrame, Series]) -> Dict[str, List[Any]]:
+def applied_to_dict_list(applied: Union[DataFrame, Series]) -> dict[str, list[Any]]:
     """Converts a DataFrame or a List in a Dict of lists
 
     Parameters
     ----------
     applied : Union[DataFrame, Series]
         Result of pandas.DataFrame.apply
 
@@ -53,14 +54,15 @@
     # case when it's a DataFrame
     if isinstance(applied, DataFrame):
         converted = applied.to_dict(orient="list")
 
     return converted
 
 
+# TODO: remove known_values
 def check_new_values(X: DataFrame, features: List[str], known_values: Dict[str, List[Any]]) -> None:
     """Checks for new, unexpected values, in X
 
     Parameters
     ----------
     X : DataFrame
         New DataFrame (at transform time)
@@ -253,15 +255,15 @@
             New key to be added.
         """
 
         self += [new_value]
         self.contained.update({new_value: [new_value]})
 
     def update(self, new_value: Dict[Any, List[Any]]) -> None:
-        """Updates the GroupedList via a dict"
+        """Updates the GroupedList via a dict
 
         Parameters
         ----------
         new_value : Dict[Any, List[Any]]
             Dict of key, values to updated `contained` dict
         """
 
@@ -439,91 +441,190 @@
 # TODO: output a json
 # TODO: add a base discretizer that implements prepare_data (add reset_index ? -> add duplicate column check)
 class GroupedListDiscretizer(BaseEstimator, TransformerMixin):
     """Discretizer that uses a dict of grouped values."""
 
     def __init__(
         self,
-        features: List[str],
-        values_orders: Dict[str, GroupedList],
+        features: list[str],
         *,
-        copy: bool = False,
-        input_dtypes: Union[str, Dict[str, str]] = None,
-        str_nan: str = None,
+        values_orders: dict[str, GroupedList] = None,
+        input_dtypes: Union[str, dict[str, str]] = 'str',
         output_dtype: str = 'str',
-        verbose: bool = False,
+        str_nan: str = None,
+        copy: bool = False,
     ) -> None:
         """Initiates a Discretizer by dict of GroupedList
 
         Parameters
         ----------
-        features : List[str]
+        features : list[str]
             List of column names to be discretized
-        values_orders : Dict[str, GroupedList]
-            Per feature ordering
-        copy : bool, optional
-            Whether or not to copy the input DataFrame, by default False
-        input_dtypes : Union[str, Dict[str, str]], optional
+        values_orders : dict[str, GroupedList], optional
+            Per feature ordering, by default None
+        input_dtypes : Union[str, dict[str, str]], optional
             String of type to be considered for all features or
             Dict of column names and associated types:
             - if 'float' uses transform_quantitative
             - if 'str' uses transform_qualitative,
-            default 'str'
+            by default 'str'
+        output_dtype : str, optional
+            _description_, by default 'str'
         str_nan : str, optional
-            Default values attributed to nan, by default None
-        verbose : bool, optional
-            If True, prints information, by default False
+            Default string value attributed to nan, by default None
+        copy : bool, optional
+            Whether or not to copy the input DataFrame, by default False
         """
-
-        self.features = features[:]
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
+        self.features = list(set(features))
+        if values_orders is None:
+            values_orders = {}
+        self.values_orders = {feature: GroupedList(values) for feature, values in values_orders.items()}
         self.copy = copy
-        if input_dtypes is None:
-            input_dtypes = {feature: "str" for feature in features}
+
+        # input feature types
         if isinstance(input_dtypes, str):
             input_dtypes = {feature: input_dtypes for feature in features}
         self.input_dtypes = input_dtypes
+
+        # output type
         self.output_dtype = output_dtype
-        self.output_labels = {}
 
-        self.verbose = verbose
+        # string value of numpy.nan
         self.str_nan = str_nan
 
+        # identifying qualitative features by there type
         self.qualitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "str"
         ]
+
+        # identifying quantitative features by there type
         self.quantitative_features = [
             feature for feature in features if self.input_dtypes[feature] == "float"
         ]
-        self.known_values = {
-            feature: self.values_orders[feature].values() for feature in self.features
-        }
+
+        # for each feature, getting label associated to each value
+        self.labels_per_values = {}  # will be initiated during fit
+
+    def get_labels_per_values(self) -> dict[str, dict[Any, Any]]:
+        """Creates a dict that contains, for each feature, for each value, the associated label
+
+        Returns
+        -------
+        dict[str, dict[Any, Any]]
+            Dict of labels per values per feature
+        """
+        # initiating dict of labels per values per feature
+        labels_per_values = {}
+
+        # iterating over each feature
+        for feature in self.features:
+            # known values of the feature(grouped)
+            values = self.values_orders[feature]
+
+            # case 0: quantitative feature -> labels per quantile (removes str_nan)
+            if feature in self.quantitative_features:
+                labels = get_labels(values, self.str_nan)
+            # case 1: qualitative feature -> by default, labels are values
+            else:
+                labels = values[:]
+            
+            # case 2: requested float output -> converting to integers
+            if self.output_dtype == 'float':
+                labels = [n for n, _ in enumerate(labels)]
+
+            # building label per value
+            label_per_value = {}
+            for group_of_values, label in zip(values, labels):
+                for value in values.get(group_of_values):
+                    label_per_value.update({value: label})
+            
+            # storing in full dict
+            labels_per_values.update({feature: label_per_value})
+        
+        return labels_per_values
+
+    def remove_feature(self, feature: str) -> None:
+        """Removes a feature from the Discretizer
+
+        Parameters
+        ----------
+        feature : str
+            Column name of the feature
+        """
+        if feature in self.features:
+            self.features.remove(feature)
+            if feature in self.qualitative_features:
+                self.qualitative_features.remove(feature)
+            if feature in self.quantitative_features:
+                self.quantitative_features.remove(feature)
+            if feature in self.values_orders:
+                self.values_orders.pop(feature)
+            if feature in self.input_dtypes:
+                self.input_dtypes.pop(feature)
+    
+    def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+
+        Returns
+        -------
+        DataFrame
+            _description_
+        """
+        # copying X
+        x_copy = X
+        if self.copy and X is not None:
+            missing_columns = [feature for feature in self.features if feature not in X]
+            assert len(missing_columns) == 0, f"Missing features from the provided DataFrame: {str(missing_columns)}"
+            x_copy = X.copy()
+
+        # checking for binary target
+        if y is not None:
+            y_values = unique(y)
+            assert (0 in y_values) & (
+                1 in y_values
+            ), "y must be a binary Series (int or float, not object)"
+            assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+
+        return x_copy
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
-        """Learns the known values for each feature
+        """Learns the labels associated to each value for each feature
 
         Parameters
         ----------
         X : DataFrame
-            Contains columns named after `values_orders` keys
+            Contains columns named after `features` attribute
         y : Series, optional
             Model target, by default None
         """
+        # checking that all features to discretize are in values_orders
+        missing_features = [feature for feature in self.features if feature not in self.values_orders]
+        assert len(missing_features) == 0, f"Missing values_orders for following features {str(missing_features)}."
+
+        # for each feature, getting label associated to each value
+        self.labels_per_values = self.get_labels_per_values()
 
         return self
 
     def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
         the `GroupedList.contained` dict.
 
         Parameters
         ----------
         X : DataFrame
-            Contains columns named after `values_orders` keys
+            Contains columns named after `features` attribute
         y : Series, optional
             Model target, by default None
 
         Returns
         -------
         DataFrame
             _description_
@@ -537,18 +638,14 @@
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
             x_copy = self.transform_quantitative(x_copy, y)
 
         # transforming qualitative features
         if len(self.qualitative_features) > 0:
             x_copy = self.transform_qualitative(x_copy, y)
-            
-        # replacing values in the output dataframe
-        if self.output_dtype == 'float':
-            x_copy = x_copy.replace(self.output_labels)
 
         return x_copy
 
     def transform_quantitative(self, X: DataFrame, y: Series) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
         the `GroupedList.contained` dict.
@@ -561,75 +658,52 @@
             Model target, by default None
 
         Returns
         -------
         DataFrame
             _description_
         """
-        # converting potential quantiles into there respective labels
-        labels_orders = convert_to_labels(
-            self.features, self.quantitative_features, self.values_orders, self.str_nan
-        )
-
         # dataset length
         x_len = X.shape[0]
 
-        for n, feature in enumerate(self.quantitative_features):
-            if self.verbose:  # verbose if requested
-                print(
-                    f" - [GroupedListDiscretizer] Transform Quantitative {feature} ({n+1}/{len(self.quantitative_features)})"
-                )
-
+        # grouping each quantitative feature
+        for feature in self.quantitative_features:
             # feature's labels associated to each quantile
-            feature_labels = labels_orders[feature]
             feature_values = self.values_orders[feature]
 
             # keeping track of nans
             nans = isna(X[feature])
 
             # converting nans to there corresponding quantile (if it was grouped to a quantile)
             if any(nans):
                 assert (
-                    self.str_nan in feature_values.values()
+                     feature_values.contains(self.str_nan)
                 ), f"Unexpected value! Missing values found for feature '{feature}' at transform step but not during fit. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
                 nan_value = feature_values.get_group(self.str_nan)
-                # checking that nans have been grouped to a quantile otherwise they are left as numpy.nan
+                # checking that nans have been grouped to a quantile otherwise they are left as numpy.nan (for comparison purposes)
                 if nan_value != self.str_nan:
                     X.loc[nans, feature] = nan_value
 
-            # quantiles ordering of the feature (can not mix str and floats for comparison purposes)
-            feature_quantiles = feature_values[:]
-            if self.str_nan in feature_quantiles:  # filtering out nans if any
-                feature_quantiles = [val for val in feature_quantiles if val != self.str_nan]
+            # removing nans from quantiles and labels (can not mix str and floats for comparison purposes)
+            if self.str_nan in feature_values:  # filtering out nans if any
+                feature_values = [value for value in feature_values if value != self.str_nan]
 
             # list of masks of values to replace with there respective group
-            values_to_group = [X[feature] <= q for q in feature_quantiles]
+            values_to_group = [X[feature] <= quantile for quantile in feature_values]
 
             # corressponding group for each value
-            group_labels = [[label] * x_len for label in feature_labels]
+            group_labels = [[self.labels_per_values[feature][value]] * x_len for value in feature_values]
 
             # checking for values to group
             if len(values_to_group) > 0:
                 X[feature] = select(values_to_group, group_labels, default=X[feature])
 
-            # converting nans to str_nan
+            # converting nans to there value
             if any(nans):
-                nan_value = feature_values.get_group(self.str_nan)
-                # checking that nans have not been grouped to a quantile -> converting them to str_nan
-                if nan_value == self.str_nan:
-                    X.loc[nans, feature] = self.str_nan
-
-            # output as float
-            if self.output_dtype == 'float':
-                values = labels_orders[feature]
-                if any(X[feature] == self.str_nan):  # adding str_nan if not grouped
-                    values += self.str_nan
-                self.output_labels.update({
-                    feature: {value: index for index, value in enumerate(values)}
-                })
+                X.loc[nans, feature] = self.labels_per_values[feature].get(nan_value, self.str_nan)
 
         return X
 
     def transform_qualitative(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
         the `GroupedList.contained` dict.
@@ -642,60 +716,100 @@
             Model target, by default None
 
         Returns
         -------
         DataFrame
             _description_
         """
-
         # filling up nans with specified value
         if self.str_nan:
             X[self.qualitative_features] = X[self.qualitative_features].fillna(self.str_nan)
 
         # checking that all unique values in X are in values_orders
-        check_new_values(X, self.qualitative_features, self.known_values)
+        check_new_values(X, self.qualitative_features, {feature: values.values() for feature, values in self.values_orders.items()})
 
-        # iterating over each feature
-        for n, feature in enumerate(self.qualitative_features):
-            if self.verbose:  # verbose if requested
-                print(
-                    f" - [GroupedListDiscretizer] Transform Qualitative {feature} ({n+1}/{len(self.qualitative_features)})"
-                )
-
-            # keeping track of nans that should stay nans
-            nans = X[feature].isna()
-
-            # Group labels are the keys of the contained dict attribute (list elements)
-            group_labels = self.values_orders[feature]
-
-            # Group of values to discard are the corresponding values of the contained dict attribute
-            groups_to_discard = [group_labels.get(key) for key in group_labels]
-
-            # identifying bucket's key per modality
-            values_to_group = [
-                X[feature].isin(group_to_discard) for group_to_discard in groups_to_discard
-            ]
+        # replacing values for there corresponding label
+        X = X.replace({feature: label_per_value for feature, label_per_value in self.labels_per_values.items() if feature in self.qualitative_features})           
 
-            # checking for values to group
-            if len(values_to_group) > 0:
-                X[feature] = select(values_to_group, group_labels, default=X[feature])
+        return X
+    
+    def to_json(self) ->  str:
+        """Converts the GroupedListDiscretizer's values_orders to .json
+
+        Returns
+        -------
+        str
+            _description_
+        """
+        # extracting contained dictionnaries
+        content = {
+            "features": self.features,
+            "values_ordres": self.values_orders,  # TODO: adapt maybe init GroupedList with {"values": values, "contained": values.contained} ?
+            "input_dtypes": self.input_dtypes,
+            "output_dtype": self.output_dtype,
+            "str_nan": self.str_nan,
+            "copy": self.copy,
+        }
+        # contained_orders = {feature: {"values": values, "contained": values.contained} for feature, values in self.values_orders.items()}
+        # dumping as json
+        return dumps(content)
+    
+    def summary(self) -> DataFrame:
+        """Summarizes the data bucketization
+
+        Returns
+        -------
+        DataFrame
+            A summary of feature's values
+        """
+        # getting quantitative labels
+        if any(self.quantitative_features):
+            print("converting to labels\n\n")
+            labels_orders = convert_to_labels(
+                self.features, self.quantitative_features, self.values_orders, self.str_nan, dropna=False
+            )
+        # initiating summaries
+        summaries: list[dict[str, Any]] = []
+        for feature in self.features:
+            init_summary = {'feature': feature}  # initiating feature summary
             
-            # giving back nans (if they were note imputed in values_orders)
-            if any(nans):
-                X.loc[nans, feature] = nan
+            # case 0: quantitative features
+            if feature in self.quantitative_features:
+                init_summary.update({'data_type': 'quantitative'})
+                # feature's modalities
+                modalities = labels_orders[feature]
+                # values included in each modality
+                contained = modalities.contained
+                
+                # adding nans
+                if self.values_orders[feature].contains(self.str_nan):
+                    nan_group = self.values_orders[feature].get_group(self.str_nan)
+                    contained.update({nan_group: contained[nan_group] + [self.str_nan]})
+
+
+            # case 1: quantitative features
+            else:
+                init_summary.update({'data_type': 'qualitative'})
+                # feature's modalities
+                modalities = self.values_orders[feature]
+                # values included in each modality
+                contained = modalities.contained
+            
+            # adding all modalities and there content
+            for modality in modalities:
+                modality_summary = {k: v for k, v in init_summary.items()}
+                modality_summary.update({"modality": modality, "values": contained[modality]})
+
+                # case 2: when the output_dtype == 'float'
+                #if self.output_dtype == 'float':
+                #    modality_summary.update({"modality": self.output_dtype[feature][modality]})
 
-        # output as float
-        if self.output_dtype == 'float':
-            self.output_labels.update({
-                feature: {value: index for index, value in enumerate(values)}
-                for feature, values in self.values_orders.items()
-                if feature in self.qualitative_features
-            })               
+                summaries += [modality_summary]
 
-        return X
+        return summaries
 
 
 def convert_to_labels(
     features: List[str],
     quantitative_features: List[str],
     values_orders: Dict[str, GroupedList],
     str_nan: str,
@@ -728,22 +842,24 @@
     if not dropna:
         for feature in features:
             if str_nan in values_orders[feature]:
                 order = labels_orders[feature]
                 order.append(str_nan)  # adding back nans at the end of the order
                 labels_orders.update({feature: order})
 
+
+
     return labels_orders
 
 
 def convert_to_values(
-    features: List[str],
-    quantitative_features: List[str],
-    values_orders: Dict[str, GroupedList],
-    label_orders: Dict[str, GroupedList],
+    features: list[str],
+    quantitative_features: list[str],
+    values_orders: dict[str, GroupedList],
+    label_orders: dict[str, GroupedList],
     str_nan: str,
 ):
     # for quantitative features getting labels per quantile
     if any(quantitative_features):
         # getting quantile per group "name"
         labels_to_quantiles = get_labels_quantiles(quantitative_features, values_orders, str_nan)
```

### Comparing `AutoCarver-5.0.0/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.1/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,24 +53,26 @@
         str_nan : str, optional
             _description_, by default "__NAN__"
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         """
-        self.features = features[:]
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=features,
+            values_orders=values_orders,
+            input_dtypes='str',
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+        )
+        
         self.min_freq = min_freq
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-
         self.str_default = str_default
-        self.str_nan = str_nan
-
-        self.copy = copy
         self.verbose = verbose
 
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Called during fit step
 
         Parameters
         ----------
@@ -80,39 +82,35 @@
             _description_
 
         Returns
         -------
         DataFrame
             _description_
         """
+        # checking for binary target
+        x_copy = super().prepare_data(X, y)
+
         # checks and initilizes values_orders
         for feature in self.features:
             # initiating features missing from values_orders
             if feature not in self.values_orders:
-                self.values_orders.update({feature: GroupedList(nan_unique(X[feature]))})
+                self.values_orders.update({feature: GroupedList(nan_unique(x_copy[feature]))})
 
         # checking that all unique values in X are in values_orders
-        check_new_values(X, self.features, self.values_orders)
+        check_new_values(x_copy, self.features, self.values_orders)
         # checking that all unique values in values_orders are in X
-        check_missing_values(X, self.features, self.values_orders)
+        check_missing_values(x_copy, self.features, self.values_orders)
 
         # adding NANS
         for feature in self.features:
-            if any(X[feature].isna()):
+            if any(x_copy[feature].isna()):
                 self.values_orders[feature].append(self.str_nan)
 
         # filling up NaNs
-        x_copy = X[self.features].fillna(self.str_nan)
-
-        # checking for binary target
-        y_values = unique(y)
-        assert (0 in y_values) & (
-            1 in y_values
-        ), "y must be a binary Series (int or float, not object)"
-        assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
+        x_copy = x_copy[self.features].fillna(self.str_nan)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """Learns modalities that are common enough (greater than min_freq)
 
         Parameters
@@ -120,22 +118,22 @@
         X : DataFrame
             _description_
         y : Series
             _description_
         """
         # copying dataframe and checking data before bucketization
         x_copy = self.prepare_data(X, y)
+        
+        if self.verbose:  # verbose if requested
+            print(f" - [DefaultDiscretizer] Fit {', '.join(self.features)}")
 
         # computing frequencies of each modality
         frequencies = x_copy.apply(value_counts, normalize=True, axis=0)
 
-        for n, feature in enumerate(self.features):
-            if self.verbose:  # verbose if requested
-                print(f" - [DefaultDiscretizer] Fit {feature} ({n+1}/{len(self.features)})")
-
+        for feature in self.features:
             # sorting orders based on target rates
             order = self.values_orders[feature]
 
             # checking for rare values
             values_to_group = [
                 val
                 for val, freq in frequencies[feature].items()
@@ -167,20 +165,14 @@
                 new_order.remove(self.str_nan)
                 new_order += [self.str_nan]
 
             # sorting order updating values_orders
             self.values_orders.update({feature: order.sort_by(new_order)})
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            str_nan=self.str_nan,
-        )
         super().fit(X, y)
 
         return self
 
 class BaseQualitativeDiscretizer(GroupedListDiscretizer):
     """TODO: to implement to mutualize prepare_data and remove_feature across qualitative discretizers"""
 
@@ -229,60 +221,63 @@
             Value used to replace nan. If set, same value should be used across
             all Discretizers, by default "__NAN__"
         copy : bool, optional
             Whether or not to copy the dataset, by default False
         verbose : bool, optional
             Whether or not to print information during fit, by default False
         """
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=features,
+            values_orders=values_orders,
+            input_dtypes='str',
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+        )
+
         self.min_freq = min_freq
-        self.features = list(set(features))
+
         self.chained_orders = [GroupedList(values) for values in chained_orders]
 
         # parameters to handle missing/unknown values
         self.remove_unknown = remove_unknown
-        self.str_nan = str_nan
 
         # known_values: all ordered values describe in each level of the chained_orders
         # starting off with first level 
         known_values = self.chained_orders[0].values()
-
         # adding each level
         for next_level in self.chained_orders[1:]:
             # highest value per group of the level
             highest_ranking_value = {group: [value for value in values if value!=group][-1] for group, values in next_level.contained.items()}
             
             # adding next_level group to the order
             for group, highest_value in highest_ranking_value.items():
                 highest_index = known_values.index(highest_value)
                 known_values = known_values[:highest_index + 1] + [group] + known_values[highest_index + 1:]
         self.known_values = known_values
 
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {feature: GroupedList(value) for feature, value in values_orders.items()}
-
         # adding known_values to each feature's order
         for feature in self.features:
             # checking for already known values of the feature
             if feature in self.values_orders:
                 order = self.values_orders[feature]
             # no known values for the feature
             else:
                 order = GroupedList([])
             # checking that all values from the order are in known_values
             for value in order:
-                assert value in self.known_values, "Value {value} from feature {feature} provided in values_orders is missing from levels of chained_orders. Add value to a level of chained_orders or adapt values_orders."
+                assert value in self.known_values, f"Value {value} from feature {feature} provided in values_orders is missing from levels of chained_orders. Add value to a level of chained_orders or adapt values_orders."
             # adding known values if missing from the order
             for value in self.known_values:
                 if value not in order.values():
                     order.append(value)
             order = order.sort_by(self.known_values)
             self.values_orders.update({feature: order})
 
-        self.copy = copy
         self.verbose = verbose
 
     def prepare_data(self, X: DataFrame, y: Series = None) -> DataFrame:
         """Prepares the data for bucketization, checks column types.
         Converts non-string columns into strings.
 
         Parameters
@@ -389,15 +384,15 @@
             # alerting user
             else:
                 assert (
                     not len(missing) > 0
                 ), f"Order for feature '{feature}' needs to be provided for values: {str(missing)}, otherwise set remove_unknown=True"
 
             # iterating over each specified orders
-            for level_order in self.chained_orders:
+            for level_order in self.chained_orders:  # TODO replace all of this with labels_per_orders
                 # values that are frequent enough
                 to_keep = list(values[frequencies >= self.min_freq])
 
                 # values from the order to group (not frequent enough or absent)
                 values_to_group = [value for value in level_order.values() if value not in to_keep]
 
                 # values to group into discarded values
@@ -413,21 +408,14 @@
                 for discarded, kept in zip(values_to_group, groups_value):
                     self.values_orders.get(feature).group(discarded, kept)
 
                 # updating frequencies of each modality for the next ordering
                 frequencies = x_copy[feature].value_counts(normalize=True)
                 values, frequencies = frequencies.index, frequencies.values
 
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            str_nan=self.str_nan,
-            copy=self.copy,
-            input_dtypes="str",
-        )
         super().fit(X, y)
 
         return self
 
 
 class OrdinalDiscretizer(GroupedListDiscretizer):
     """Discretizes ordered qualitative features into groups more frequent than min_freq.
@@ -437,20 +425,20 @@
     The choosen modality is:
     - the closest in target rate
     - or the one with the lowest frequency
     """
 
     def __init__(
         self,
-        features: List[str],
-        values_orders: Dict[str, Any],
+        features: list[str],
+        values_orders: dict[str, GroupedList],
         min_freq: float,
         *,
         str_nan: str = "__NAN__",
-        input_dtypes: Union[str, Dict[str, str]] = None,
+        input_dtypes: Union[str, dict[str, str]] = "str",
         copy: bool = False,
         verbose: bool = False,
     ):
         """Initializes a OrdinalDiscretizer
 
         Parameters
         ----------
@@ -469,33 +457,26 @@
             - if 'str' uses transform_qualitative,
             default 'str'
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         """
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=features,
+            values_orders=values_orders,
+            input_dtypes=input_dtypes,
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+        )
 
-        self.features = features[:]
         self.min_freq = min_freq
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.copy = copy
         self.verbose = verbose
-        self.str_nan = str_nan
-        if input_dtypes is None:
-            input_dtypes = {feature: "str" for feature in features}
-        if isinstance(input_dtypes, str):
-            input_dtypes = {feature: input_dtypes for feature in features}
-        self.input_dtypes = input_dtypes
-
-        self.quantitative_features = [
-            feature for feature in features if input_dtypes[feature] == "float"
-        ]
-        self.qualitative_features = [
-            feature for feature in features if input_dtypes[feature] == "str"
-        ]
 
     def prepare_data(self, X: DataFrame, y: Series) -> DataFrame:
         """Called during fit step
 
         Parameters
         ----------
         X : DataFrame
@@ -533,16 +514,15 @@
         Parameters
         ----------
         X : DataFrame
             Training set that contains columns named after `values_orders` keys.
         y : Series
             Model target.
         """
-        # verbose
-        if self.verbose:
+        if self.verbose:  # verbose if requested
             print(f" - [OrdinalDiscretizer] Fit {', '.join(self.features)}")
 
         # checking values orders
         x_copy = self.prepare_data(X, y)
 
         # converting potential quantiles into there labels
         known_orders = convert_to_labels(
@@ -571,33 +551,26 @@
                 values_orders=self.values_orders,
                 label_orders=common_modalities,
                 str_nan=self.str_nan,
             )
         )
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            str_nan=self.str_nan,
-            input_dtypes=self.input_dtypes,
-        )
         super().fit(x_copy, y)
 
         return self
 
 
 def find_common_modalities(
     df_feature: Series,
     y: Series,
     min_freq: float,
-    values_orders: Dict[str, GroupedList],
+    values_orders: dict[str, GroupedList],
     len_df: int = None,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Découpage en modalités de fréquence minimal (Cas des variables ordonnées).
 
     Fonction récursive : on prend l'échantillon et on cherche des valeurs sur-représentées
     Si la valeur existe on la met dans une classe et on cherche à gauche et à droite de celle-ci, d'autres variables sur-représentées
     Une fois il n'y a plus de valeurs qui soient sur-représentées,
     on fait un découpage classique avec qcut en multipliant le nombre de classes souhaité par le pourcentage de valeurs restantes sur le total
```

### Comparing `AutoCarver-5.0.0/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.1/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 
 class QuantileDiscretizer(GroupedListDiscretizer):
     """Builds per-feature buckets of quantiles"""
 
     def __init__(
         self,
-        features: List[str],
+        features: list[str],
         min_freq: float,
         *,
-        values_orders: Dict[str, Any] = None,
+        values_orders: dict[str, Any] = None,
         str_nan: str = "__NAN__",
         copy: bool = False,
         verbose: bool = False,
     ) -> None:
         """Discretizes quantitative features into groups of q quantiles
 
         Parameters
@@ -36,27 +36,27 @@
         str_nan : str, optional
             _description_, by default '__NAN__'
         copy : bool, optional
             _description_, by default False
         verbose : bool, optional
             _description_, by default False
         """
+        # Initiating GroupedListDiscretizer
+        super().__init__(
+            features=features,
+            values_orders=values_orders,
+            input_dtypes='float',
+            output_dtype='str',
+            str_nan=str_nan,
+            copy=copy,
+        )
 
-        self.features = features[:]
         self.min_freq = min_freq
-
-        if values_orders is None:
-            values_orders = {}
-        self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.str_nan = str_nan
-
-        self.copy = copy
-        self.verbose = verbose
-
         self.q = round(1 / min_freq)  # number of quantiles
+        self.verbose = verbose
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """_summary_
 
         Parameters
         ----------
         X : DataFrame
@@ -79,21 +79,14 @@
             if any(isna(X[feature])):
                 order.append(self.str_nan)
 
             # storing into the values_orders
             self.values_orders.update({feature: order})
 
         # discretizing features based on each feature's values_order
-        super().__init__(
-            features=self.features,
-            values_orders=self.values_orders,
-            copy=self.copy,
-            input_dtypes="float",
-            str_nan=self.str_nan,
-        )
         super().fit(X, y)
 
         return self
 
 
 def find_quantiles(
     df_feature: Series,
```

### Comparing `AutoCarver-5.0.0/AutoCarver/feature_selector.py` & `AutoCarver-5.0.1/AutoCarver/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.0/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,8 @@
-Metadata-Version: 2.1
-Name: AutoCarver
-Version: 5.0.0
-Summary: Automatic Bucketizing of Features with Optimal Association
-Home-page: https://github.com/mdefrance/AutoCarver
-Author: Mario DEFRANCE
-Author-email: defrancemario@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-\n</p>
+</p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
 </p>
 
 This is a work in progress.
@@ -52,68 +32,16 @@
 One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
 
 ```python
 # defining training and testing sets
 X_train, y_train = ...  # used to fit the AutoCarver and the model
 X_dev, y_dev = ...  # used to validate the AutoCarver's buckets and optimize the model's parameters/hyperparameters
 X_test, y_test = ...  # used to evaluate the final model's performances
-
-pipe = []  # initiating as an empty list that will be filled along the feature engineering
 ```
 
-### Quickly build basic buckets with Discretizer
-
-The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
-
-**TODO: add info from `QuantitativeDiscretizer` and `QuantitativeDiscretizer`**
-**TODO: add stringconverter**
-`Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
-
-Following parameters must be set for `Discretizer`:
-- `quanti_features`, list of column names of quantitative data to discretize
-- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
-- `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
-  - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
-  - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
-  - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
-- `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
-  - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
-
-```python
-from AutoCarver.Discretizers import Discretizer
-
-quanti_features = ['amount', 'distance', 'length', 'height']  # quantitative features to be discretized
-quali_features = ['age', 'type', 'grade', 'city']  # qualitative features to be discretized
-
-# specifying orders of qualitative ordinal features
-values_orders = {
-    'age': ['0-18', '18-30', '30-50', '50+'],
-    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-}
-
-# pre-processing of features into categorical ordinal features
-discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
-discretizer.fit_transform(X_train, y_train)
-discretizer.transform(X_dev)
-
-# storing built buckets
-values_orders.update(discretizer.values_orders)
-
-# append the discretizer to the feature engineering pipeline
-pipe += [('Discretizer', discretizer)]
-```
-
-
-Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
-
-For more details and further functionnalities look into AutoCarver.Discretizers README.
-
-For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
-
-By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
 
 
 ### Maximize target association of features' buckets with AutoCarver
 
 All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
 
 All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
@@ -122,25 +50,47 @@
   - Use `sort_by='cramerv'` for more modalities, less robust.
   - Use `sort_by='tschuprowt'` for more robust modalities.
   - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
 - `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
 - `keep_nans`, whether or not to try groupin missing values to non-missing values. Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
 
 ```python
-from AutoCarver.AutoCarver import AutoCarver
+from AutoCarver.auto_carver import AutoCarver
+
+quantitative_features = ['Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative', 'Discrete_Quantitative_rarevalue']
+qualitative_features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan", "Discrete_Qualitative_noorder", "Discrete_Qualitative_lownan_noorder", "Discrete_Qualitative_rarevalue_noorder"]
+ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan", "Discrete_Qualitative_highnan"]
+values_orders = {
+    "Qualitative_Ordinal": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+    "Qualitative_Ordinal_lownan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+    "Discrete_Qualitative_highnan" : ["1", "2", "3", "4", "5", "6", "7"],
+}
+target = "quali_ordinal_target"
 
 # intiating AutoCarver
-auto_carver = AutoCarver(values_orders=values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
+auto_carver = AutoCarver(
+    quantitative_features=quantitative_features,
+    qualitative_features=qualitative_features,
+    ordinal_features=ordinal_features,
+    values_orders=values_orders,
+    min_freq=0.05,  # minimum frequency per modality
+    max_n_mod=4,  # maximum number of modality per feature
+    sort_by='cramerv',
+    output_dtype='float',
+    copy=True,
+    verbose=True,
+)
+
+# fitting on training sample, a dev sample can be specified to evaluate carving robustness
+x_discretized = auto_carver.fit_transform(x_train, x_train[target], X_test=x_dev, y_test=x_dev[target])
 
-# fitting on training sample, a test sample can be specified to evaluate carving robustness
-auto_carver.fit_transform(X_train, y_train, X_test=X_dev, y_test=y_dev)
-auto_carver.transform(X_dev)
+# transforming dev/test sample accordingly
+x_dev_discretized = auto_carver.transform(x_dev)
+x_test_discretized = auto_carver.transform(x_test)
 
-# append the auto_carver to the feature engineering pipeline
-pipe += [('AutoCarver', auto_carver)]
 ```
 <p align="left">
   <img width="500" src="/docs/auto_carver_fit.PNG" />
 </p>
 
 
 ### Cherry picking the most target-associated features with FeatureSelector
@@ -159,26 +109,28 @@
 
 **TODO: add by default measures and filters + add ranking according to several measures  + say that it filters out non-selected columns**
 
 
 **TODO; add pictures say that it does not make sense to use zscore_measure as last measure**
 
 ```python
-from AutoCarver.FeatureSelector import FeatureSelector
-from AutoCarver.FeatureSelector import tschuprowt_measure, cramerv_measure, cramerv_filter, tschuprowt_filter, measure_filter
+from AutoCarver.feature_selector import FeatureSelector
+from AutoCarver.feature_selector import tschuprowt_measure, cramerv_measure, cramerv_filter, tschuprowt_filter, measure_filter
 
-features = quanti_features + quali_features  # after AutoCarver, everything is qualitative
+features = auto_carver.features  # after AutoCarver, everything is qualitative
+values_orders = auto_carver.values_orders
 
 measures = [cramerv_measure, tschuprowt_measure]  # measures of interest (the last one is used for ranking)
 filters = [tschuprowt_filter, measure_filter]  # filtering out by inter-feature correlation
 
 # select the best 25 most target associated qualitative features
 quali_selector = FeatureSelector(
     features=features,  # features to select from
     n_best=25,  # best 25 features
+    values_orders=values_orders,
     measures=measures, filters=filters,   # selected measures and filters
     thresh_mode=0.9,  # filters out features with more than 90% of their mode
     thresh_nan=0.9,  # filters out features with more than 90% of missing values
     thresh_corr=0.5,  # filters out features with spearman greater than 0.5 with a better feature
     name_measure='cramerv_measure', thresh_measure=0.06,  # filters out features with cramerv_measure lower than 0.06
     verbose=True  # displays statistics
 )
@@ -189,30 +141,45 @@
 pipe += [('QualiFeatureSelector', quali_selector)]
 ```
 
 
 
 ### Storing, reusing the AutoCarver
 
-The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
+**TODO:** The `AutoCarver` can be stored as a .json file.
 
 ```python
-from pickle import dump
-from sklearn.pipeline import Pipeline
+import json
 
-# storing fitted Discretizer, AutoCarver and FeatureSelector in a Pipeline
-pipe = Pipeline(pipe)
-
-# storing as pickle file
-dump(pipe, open('my_pipe.pkl', 'wb'))
+# storing as json file
+with open('my_carver.json', 'wb') as my_carver_json:
+    json.dump({feature: values.contained for feature, values in auto_carver.values_orders.items()}, my_carver_json)
 ```
 
-The stored `Pipeline`, can then be used to transform new datasets.
+The stored .json, can then be used to initialize a new `base_discretizers.GroupedListDiscretizer`.
 
+```python
+from AutoCarver.discretizers.utils.base_discretizers import GroupedListDiscretizer
 
+# storing as json file
+with open('my_carver.json', 'rb') as my_carver_json:
+    values_orders = json.load(my_carver_json)
+
+# initiating AutoCarver
+auto_carver = GroupedListDiscretizer(
+    features=self.features,
+    values_orders=self.values_orders,
+    copy=self.copy,
+    input_dtypes=self.input_dtypes,
+    str_nan=self.str_nan,
+    verbose=self.verbose,
+    output_dtype=self.output_dtype,
+)
+
+```
 
 
 
 
 
 
 
@@ -235,14 +202,64 @@
 ```
 
 
 ### Discretizers Examples
 
 The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
 
+#### Quickly build basic buckets with Discretizer
+
+The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
+
+`Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
+
+Following parameters must be set for `Discretizer`:
+- `quanti_features`, list of column names of quantitative data to discretize
+- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
+- `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
+  - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
+  - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
+  - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
+- `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
+  - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
+
+```python
+from AutoCarver.Discretizers import Discretizer
+
+quanti_features = ['amount', 'distance', 'length', 'height']  # quantitative features to be discretized
+quali_features = ['age', 'type', 'grade', 'city']  # qualitative features to be discretized
+
+# specifying orders of qualitative ordinal features
+values_orders = {
+    'age': ['0-18', '18-30', '30-50', '50+'],
+    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
+}
+
+# pre-processing of features into categorical ordinal features
+discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
+discretizer.fit_transform(X_train, y_train)
+discretizer.transform(X_dev)
+
+# storing built buckets
+values_orders.update(discretizer.values_orders)
+
+# append the discretizer to the feature engineering pipeline
+pipe += [('Discretizer', discretizer)]
+```
+
+
+Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
+
+For more details and further functionnalities look into AutoCarver.Discretizers README.
+
+For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
+
+By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
+
+
 #### QualitativeDiscretizer Example
 
 **TODO: add StringConverter**
 
 `QualitativeDiscretizer` enables the transformation of qualitative data into statistically relevant categories, facilitating model robustness.
  - *Qualitative Data* consists of categorical variables without any inherent order
  - *Qualitative Ordinal Data* consists of categorical variables with a predefined order or hierarchy
```

### Comparing `AutoCarver-5.0.0/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.1/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.0/LICENSE` & `AutoCarver-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.0/PKG-INFO` & `AutoCarver-5.0.1/AutoCarver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.0
+Version: 5.0.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
@@ -52,69 +52,17 @@
 One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
 
 ```python
 # defining training and testing sets
 X_train, y_train = ...  # used to fit the AutoCarver and the model
 X_dev, y_dev = ...  # used to validate the AutoCarver's buckets and optimize the model's parameters/hyperparameters
 X_test, y_test = ...  # used to evaluate the final model's performances
-
-pipe = []  # initiating as an empty list that will be filled along the feature engineering
-```
-
-### Quickly build basic buckets with Discretizer
-
-The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
-
-**TODO: add info from `QuantitativeDiscretizer` and `QuantitativeDiscretizer`**
-**TODO: add stringconverter**
-`Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
-
-Following parameters must be set for `Discretizer`:
-- `quanti_features`, list of column names of quantitative data to discretize
-- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
-- `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
-  - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
-  - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
-  - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
-- `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
-  - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
-
-```python
-from AutoCarver.Discretizers import Discretizer
-
-quanti_features = ['amount', 'distance', 'length', 'height']  # quantitative features to be discretized
-quali_features = ['age', 'type', 'grade', 'city']  # qualitative features to be discretized
-
-# specifying orders of qualitative ordinal features
-values_orders = {
-    'age': ['0-18', '18-30', '30-50', '50+'],
-    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-}
-
-# pre-processing of features into categorical ordinal features
-discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
-discretizer.fit_transform(X_train, y_train)
-discretizer.transform(X_dev)
-
-# storing built buckets
-values_orders.update(discretizer.values_orders)
-
-# append the discretizer to the feature engineering pipeline
-pipe += [('Discretizer', discretizer)]
 ```
 
 
-Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
-
-For more details and further functionnalities look into AutoCarver.Discretizers README.
-
-For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
-
-By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
-
 
 ### Maximize target association of features' buckets with AutoCarver
 
 All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
 
 All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
 - `values_orders`, dict of all features matched to the order of their modalities
@@ -122,25 +70,47 @@
   - Use `sort_by='cramerv'` for more modalities, less robust.
   - Use `sort_by='tschuprowt'` for more robust modalities.
   - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
 - `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
 - `keep_nans`, whether or not to try groupin missing values to non-missing values. Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
 
 ```python
-from AutoCarver.AutoCarver import AutoCarver
+from AutoCarver.auto_carver import AutoCarver
+
+quantitative_features = ['Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative', 'Discrete_Quantitative_rarevalue']
+qualitative_features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan", "Discrete_Qualitative_noorder", "Discrete_Qualitative_lownan_noorder", "Discrete_Qualitative_rarevalue_noorder"]
+ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan", "Discrete_Qualitative_highnan"]
+values_orders = {
+    "Qualitative_Ordinal": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+    "Qualitative_Ordinal_lownan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+    "Discrete_Qualitative_highnan" : ["1", "2", "3", "4", "5", "6", "7"],
+}
+target = "quali_ordinal_target"
 
 # intiating AutoCarver
-auto_carver = AutoCarver(values_orders=values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
+auto_carver = AutoCarver(
+    quantitative_features=quantitative_features,
+    qualitative_features=qualitative_features,
+    ordinal_features=ordinal_features,
+    values_orders=values_orders,
+    min_freq=0.05,  # minimum frequency per modality
+    max_n_mod=4,  # maximum number of modality per feature
+    sort_by='cramerv',
+    output_dtype='float',
+    copy=True,
+    verbose=True,
+)
+
+# fitting on training sample, a dev sample can be specified to evaluate carving robustness
+x_discretized = auto_carver.fit_transform(x_train, x_train[target], X_test=x_dev, y_test=x_dev[target])
 
-# fitting on training sample, a test sample can be specified to evaluate carving robustness
-auto_carver.fit_transform(X_train, y_train, X_test=X_dev, y_test=y_dev)
-auto_carver.transform(X_dev)
+# transforming dev/test sample accordingly
+x_dev_discretized = auto_carver.transform(x_dev)
+x_test_discretized = auto_carver.transform(x_test)
 
-# append the auto_carver to the feature engineering pipeline
-pipe += [('AutoCarver', auto_carver)]
 ```
 <p align="left">
   <img width="500" src="/docs/auto_carver_fit.PNG" />
 </p>
 
 
 ### Cherry picking the most target-associated features with FeatureSelector
@@ -159,26 +129,28 @@
 
 **TODO: add by default measures and filters + add ranking according to several measures  + say that it filters out non-selected columns**
 
 
 **TODO; add pictures say that it does not make sense to use zscore_measure as last measure**
 
 ```python
-from AutoCarver.FeatureSelector import FeatureSelector
-from AutoCarver.FeatureSelector import tschuprowt_measure, cramerv_measure, cramerv_filter, tschuprowt_filter, measure_filter
+from AutoCarver.feature_selector import FeatureSelector
+from AutoCarver.feature_selector import tschuprowt_measure, cramerv_measure, cramerv_filter, tschuprowt_filter, measure_filter
 
-features = quanti_features + quali_features  # after AutoCarver, everything is qualitative
+features = auto_carver.features  # after AutoCarver, everything is qualitative
+values_orders = auto_carver.values_orders
 
 measures = [cramerv_measure, tschuprowt_measure]  # measures of interest (the last one is used for ranking)
 filters = [tschuprowt_filter, measure_filter]  # filtering out by inter-feature correlation
 
 # select the best 25 most target associated qualitative features
 quali_selector = FeatureSelector(
     features=features,  # features to select from
     n_best=25,  # best 25 features
+    values_orders=values_orders,
     measures=measures, filters=filters,   # selected measures and filters
     thresh_mode=0.9,  # filters out features with more than 90% of their mode
     thresh_nan=0.9,  # filters out features with more than 90% of missing values
     thresh_corr=0.5,  # filters out features with spearman greater than 0.5 with a better feature
     name_measure='cramerv_measure', thresh_measure=0.06,  # filters out features with cramerv_measure lower than 0.06
     verbose=True  # displays statistics
 )
@@ -189,30 +161,45 @@
 pipe += [('QualiFeatureSelector', quali_selector)]
 ```
 
 
 
 ### Storing, reusing the AutoCarver
 
-The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
+**TODO:** The `AutoCarver` can be stored as a .json file.
 
 ```python
-from pickle import dump
-from sklearn.pipeline import Pipeline
-
-# storing fitted Discretizer, AutoCarver and FeatureSelector in a Pipeline
-pipe = Pipeline(pipe)
+import json
 
-# storing as pickle file
-dump(pipe, open('my_pipe.pkl', 'wb'))
+# storing as json file
+with open('my_carver.json', 'wb') as my_carver_json:
+    json.dump({feature: values.contained for feature, values in auto_carver.values_orders.items()}, my_carver_json)
 ```
 
-The stored `Pipeline`, can then be used to transform new datasets.
+The stored .json, can then be used to initialize a new `base_discretizers.GroupedListDiscretizer`.
 
+```python
+from AutoCarver.discretizers.utils.base_discretizers import GroupedListDiscretizer
+
+# storing as json file
+with open('my_carver.json', 'rb') as my_carver_json:
+    values_orders = json.load(my_carver_json)
+
+# initiating AutoCarver
+auto_carver = GroupedListDiscretizer(
+    features=self.features,
+    values_orders=self.values_orders,
+    copy=self.copy,
+    input_dtypes=self.input_dtypes,
+    str_nan=self.str_nan,
+    verbose=self.verbose,
+    output_dtype=self.output_dtype,
+)
 
+```
 
 
 
 
 
 
 
@@ -235,14 +222,64 @@
 ```
 
 
 ### Discretizers Examples
 
 The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
 
+#### Quickly build basic buckets with Discretizer
+
+The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
+
+`Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
+
+Following parameters must be set for `Discretizer`:
+- `quanti_features`, list of column names of quantitative data to discretize
+- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
+- `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
+  - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
+  - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
+  - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
+- `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
+  - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
+
+```python
+from AutoCarver.Discretizers import Discretizer
+
+quanti_features = ['amount', 'distance', 'length', 'height']  # quantitative features to be discretized
+quali_features = ['age', 'type', 'grade', 'city']  # qualitative features to be discretized
+
+# specifying orders of qualitative ordinal features
+values_orders = {
+    'age': ['0-18', '18-30', '30-50', '50+'],
+    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
+}
+
+# pre-processing of features into categorical ordinal features
+discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
+discretizer.fit_transform(X_train, y_train)
+discretizer.transform(X_dev)
+
+# storing built buckets
+values_orders.update(discretizer.values_orders)
+
+# append the discretizer to the feature engineering pipeline
+pipe += [('Discretizer', discretizer)]
+```
+
+
+Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
+
+For more details and further functionnalities look into AutoCarver.Discretizers README.
+
+For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
+
+By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
+
+
 #### QualitativeDiscretizer Example
 
 **TODO: add StringConverter**
 
 `QualitativeDiscretizer` enables the transformation of qualitative data into statistically relevant categories, facilitating model robustness.
  - *Qualitative Data* consists of categorical variables without any inherent order
  - *Qualitative Ordinal Data* consists of categorical variables with a predefined order or hierarchy
```

### Comparing `AutoCarver-5.0.0/README.md` & `AutoCarver-5.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,28 @@
-</p>
+Metadata-Version: 2.1
+Name: AutoCarver
+Version: 5.0.1
+Summary: Automatic Bucketizing of Features with Optimal Association
+Home-page: https://github.com/mdefrance/AutoCarver
+Author: Mario DEFRANCE
+Author-email: defrancemario@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+\n</p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
 </p>
 
 This is a work in progress.
@@ -32,68 +52,16 @@
 One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
 
 ```python
 # defining training and testing sets
 X_train, y_train = ...  # used to fit the AutoCarver and the model
 X_dev, y_dev = ...  # used to validate the AutoCarver's buckets and optimize the model's parameters/hyperparameters
 X_test, y_test = ...  # used to evaluate the final model's performances
-
-pipe = []  # initiating as an empty list that will be filled along the feature engineering
 ```
 
-### Quickly build basic buckets with Discretizer
-
-The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
-
-**TODO: add info from `QuantitativeDiscretizer` and `QuantitativeDiscretizer`**
-**TODO: add stringconverter**
-`Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
-
-Following parameters must be set for `Discretizer`:
-- `quanti_features`, list of column names of quantitative data to discretize
-- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
-- `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
-  - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
-  - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
-  - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
-- `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
-  - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
-
-```python
-from AutoCarver.Discretizers import Discretizer
-
-quanti_features = ['amount', 'distance', 'length', 'height']  # quantitative features to be discretized
-quali_features = ['age', 'type', 'grade', 'city']  # qualitative features to be discretized
-
-# specifying orders of qualitative ordinal features
-values_orders = {
-    'age': ['0-18', '18-30', '30-50', '50+'],
-    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
-}
-
-# pre-processing of features into categorical ordinal features
-discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
-discretizer.fit_transform(X_train, y_train)
-discretizer.transform(X_dev)
-
-# storing built buckets
-values_orders.update(discretizer.values_orders)
-
-# append the discretizer to the feature engineering pipeline
-pipe += [('Discretizer', discretizer)]
-```
-
-
-Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
-
-For more details and further functionnalities look into AutoCarver.Discretizers README.
-
-For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
-
-By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
 
 
 ### Maximize target association of features' buckets with AutoCarver
 
 All features need to be discretized via a `Discretizer` so `AutoCarver` can group their modalities. Following parameters must be set for `Discretizer`:
 
 All specified features can now automatically be carved in an association maximising grouping of their modalities while reducing their number. Following parameters must be set for `AutoCarver`:
@@ -102,25 +70,47 @@
   - Use `sort_by='cramerv'` for more modalities, less robust.
   - Use `sort_by='tschuprowt'` for more robust modalities.
   - **Tip:** a combination of features carved with `sort_by='cramerv'` and `sort_by='tschuprowt'` can sometime prove to be better than only one of those.
 - `max_n_mod`, maximum number of modalities for the carved features (excluding `numpy.nan`). All possible combinations of less than `max_n_mod` groups of modalities will be tested. Should be set from 4 (faster) to 6 (preciser).
 - `keep_nans`, whether or not to try groupin missing values to non-missing values. Use `keep_nans=True` if you want `numpy.nan` to remain as a specific modality.
 
 ```python
-from AutoCarver.AutoCarver import AutoCarver
+from AutoCarver.auto_carver import AutoCarver
+
+quantitative_features = ['Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative', 'Discrete_Quantitative_rarevalue']
+qualitative_features = ["Qualitative", "Qualitative_grouped", "Qualitative_lownan", "Qualitative_highnan", "Discrete_Qualitative_noorder", "Discrete_Qualitative_lownan_noorder", "Discrete_Qualitative_rarevalue_noorder"]
+ordinal_features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan", "Discrete_Qualitative_highnan"]
+values_orders = {
+    "Qualitative_Ordinal": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+    "Qualitative_Ordinal_lownan": ['Low-', 'Low', 'Low+', 'Medium-', 'Medium', 'Medium+', 'High-', 'High', 'High+'],
+    "Discrete_Qualitative_highnan" : ["1", "2", "3", "4", "5", "6", "7"],
+}
+target = "quali_ordinal_target"
 
 # intiating AutoCarver
-auto_carver = AutoCarver(values_orders=values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
+auto_carver = AutoCarver(
+    quantitative_features=quantitative_features,
+    qualitative_features=qualitative_features,
+    ordinal_features=ordinal_features,
+    values_orders=values_orders,
+    min_freq=0.05,  # minimum frequency per modality
+    max_n_mod=4,  # maximum number of modality per feature
+    sort_by='cramerv',
+    output_dtype='float',
+    copy=True,
+    verbose=True,
+)
+
+# fitting on training sample, a dev sample can be specified to evaluate carving robustness
+x_discretized = auto_carver.fit_transform(x_train, x_train[target], X_test=x_dev, y_test=x_dev[target])
 
-# fitting on training sample, a test sample can be specified to evaluate carving robustness
-auto_carver.fit_transform(X_train, y_train, X_test=X_dev, y_test=y_dev)
-auto_carver.transform(X_dev)
+# transforming dev/test sample accordingly
+x_dev_discretized = auto_carver.transform(x_dev)
+x_test_discretized = auto_carver.transform(x_test)
 
-# append the auto_carver to the feature engineering pipeline
-pipe += [('AutoCarver', auto_carver)]
 ```
 <p align="left">
   <img width="500" src="/docs/auto_carver_fit.PNG" />
 </p>
 
 
 ### Cherry picking the most target-associated features with FeatureSelector
@@ -139,26 +129,28 @@
 
 **TODO: add by default measures and filters + add ranking according to several measures  + say that it filters out non-selected columns**
 
 
 **TODO; add pictures say that it does not make sense to use zscore_measure as last measure**
 
 ```python
-from AutoCarver.FeatureSelector import FeatureSelector
-from AutoCarver.FeatureSelector import tschuprowt_measure, cramerv_measure, cramerv_filter, tschuprowt_filter, measure_filter
+from AutoCarver.feature_selector import FeatureSelector
+from AutoCarver.feature_selector import tschuprowt_measure, cramerv_measure, cramerv_filter, tschuprowt_filter, measure_filter
 
-features = quanti_features + quali_features  # after AutoCarver, everything is qualitative
+features = auto_carver.features  # after AutoCarver, everything is qualitative
+values_orders = auto_carver.values_orders
 
 measures = [cramerv_measure, tschuprowt_measure]  # measures of interest (the last one is used for ranking)
 filters = [tschuprowt_filter, measure_filter]  # filtering out by inter-feature correlation
 
 # select the best 25 most target associated qualitative features
 quali_selector = FeatureSelector(
     features=features,  # features to select from
     n_best=25,  # best 25 features
+    values_orders=values_orders,
     measures=measures, filters=filters,   # selected measures and filters
     thresh_mode=0.9,  # filters out features with more than 90% of their mode
     thresh_nan=0.9,  # filters out features with more than 90% of missing values
     thresh_corr=0.5,  # filters out features with spearman greater than 0.5 with a better feature
     name_measure='cramerv_measure', thresh_measure=0.06,  # filters out features with cramerv_measure lower than 0.06
     verbose=True  # displays statistics
 )
@@ -169,30 +161,45 @@
 pipe += [('QualiFeatureSelector', quali_selector)]
 ```
 
 
 
 ### Storing, reusing the AutoCarver
 
-The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
+**TODO:** The `AutoCarver` can be stored as a .json file.
 
 ```python
-from pickle import dump
-from sklearn.pipeline import Pipeline
+import json
 
-# storing fitted Discretizer, AutoCarver and FeatureSelector in a Pipeline
-pipe = Pipeline(pipe)
-
-# storing as pickle file
-dump(pipe, open('my_pipe.pkl', 'wb'))
+# storing as json file
+with open('my_carver.json', 'wb') as my_carver_json:
+    json.dump({feature: values.contained for feature, values in auto_carver.values_orders.items()}, my_carver_json)
 ```
 
-The stored `Pipeline`, can then be used to transform new datasets.
+The stored .json, can then be used to initialize a new `base_discretizers.GroupedListDiscretizer`.
 
+```python
+from AutoCarver.discretizers.utils.base_discretizers import GroupedListDiscretizer
 
+# storing as json file
+with open('my_carver.json', 'rb') as my_carver_json:
+    values_orders = json.load(my_carver_json)
+
+# initiating AutoCarver
+auto_carver = GroupedListDiscretizer(
+    features=self.features,
+    values_orders=self.values_orders,
+    copy=self.copy,
+    input_dtypes=self.input_dtypes,
+    str_nan=self.str_nan,
+    verbose=self.verbose,
+    output_dtype=self.output_dtype,
+)
+
+```
 
 
 
 
 
 
 
@@ -215,14 +222,64 @@
 ```
 
 
 ### Discretizers Examples
 
 The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
 
+#### Quickly build basic buckets with Discretizer
+
+The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
+
+`Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
+
+Following parameters must be set for `Discretizer`:
+- `quanti_features`, list of column names of quantitative data to discretize
+- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
+- `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
+  - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
+  - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
+  - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
+- `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
+  - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
+
+```python
+from AutoCarver.Discretizers import Discretizer
+
+quanti_features = ['amount', 'distance', 'length', 'height']  # quantitative features to be discretized
+quali_features = ['age', 'type', 'grade', 'city']  # qualitative features to be discretized
+
+# specifying orders of qualitative ordinal features
+values_orders = {
+    'age': ['0-18', '18-30', '30-50', '50+'],
+    'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
+}
+
+# pre-processing of features into categorical ordinal features
+discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
+discretizer.fit_transform(X_train, y_train)
+discretizer.transform(X_dev)
+
+# storing built buckets
+values_orders.update(discretizer.values_orders)
+
+# append the discretizer to the feature engineering pipeline
+pipe += [('Discretizer', discretizer)]
+```
+
+
+Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
+
+For more details and further functionnalities look into AutoCarver.Discretizers README.
+
+For qualitative features, unknown modalities passed to `Discretizer.transform` (that where not passed to `Discretizer.fit`) are automaticaly grouped to the `default_value='__OTHER__'` modality.
+
+By default, samples are modified and not copied (recommanded for large datasets). Use `copy=True` if you want a new `DataFrame` to be returned.
+
+
 #### QualitativeDiscretizer Example
 
 **TODO: add StringConverter**
 
 `QualitativeDiscretizer` enables the transformation of qualitative data into statistically relevant categories, facilitating model robustness.
  - *Qualitative Data* consists of categorical variables without any inherent order
  - *Qualitative Ordinal Data* consists of categorical variables with a predefined order or hierarchy
```

### Comparing `AutoCarver-5.0.0/setup.py` & `AutoCarver-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.0",
+    version="5.0.1",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.0.0/tests/test_auto_carver.py` & `AutoCarver-5.0.1/tests/test_auto_carver.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,9 +65,15 @@
     x_discretized = auto_carver.fit_transform(x_train, x_train["quali_ordinal_target"], X_test=x_test_1, y_test=x_test_1["quali_ordinal_target"])
     x_test_discretized = auto_carver.transform(x_test_1)
 
     assert all(x_discretized[auto_carver.features].nunique() <= max_n_mod), "Too many values after carving of train sample"
     assert all(x_test_discretized[auto_carver.features].nunique() <= max_n_mod), "Too many values after carving of test sample"
     assert all(x_discretized[auto_carver.features].nunique() == x_test_discretized[auto_carver.features].nunique()), "More values in train or test samples"
 
+    # test that all values still are in the values_orders
+    for feature in auto_carver.qualitative_features:
+        fitted_values = auto_carver.values_orders[feature].values()
+        init_values = x_train[feature].fillna('__NAN__').unique()
+        assert all(value in fitted_values for value in init_values), feature
+
     # TODO: test output 'float'
-    
+    # TODO test missing values in test
```

### Comparing `AutoCarver-5.0.0/tests/test_base_discretizers.py` & `AutoCarver-5.0.1/tests/test_base_discretizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     values_orders = {
         "Qualitative_Ordinal": groupedlist,
         "Qualitative_Ordinal_lownan": groupedlist_lownan,
     }
     features = ["Qualitative_Ordinal", "Qualitative_Ordinal_lownan"]
     
     # initiating discretizer 
-    discretizer = GroupedListDiscretizer(features, values_orders, str_nan=str_nan, input_dtypes='str', copy=True)
+    discretizer = GroupedListDiscretizer(features=features, values_orders=values_orders, str_nan=str_nan, input_dtypes='str', copy=True)
     x_discretized = discretizer.fit_transform(x_train)
 
     # testing ordinal qualitative feature discretization
     x_expected = x_train.copy()
     x_expected["Qualitative_Ordinal"] = x_expected["Qualitative_Ordinal"].replace('Low-', 'Low+')\
         .replace('Low', 'Low+')\
         .replace('Low+', 'Low+')\
```

### Comparing `AutoCarver-5.0.0/tests/test_discretizers.py` & `AutoCarver-5.0.1/tests/test_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     x_train : DataFrame
         Simulated Train DataFrame
     """
 
     features = ['Quantitative', 'Discrete_Quantitative', 'Discrete_Quantitative_highnan', 'Discrete_Quantitative_lownan', 'Discrete_Quantitative_rarevalue']
     min_freq = 0.1
 
-    discretizer = discretizers.QuantitativeDiscretizer(features, min_freq, copy=True)
+    discretizer = discretizers.QuantitativeDiscretizer(features, min_freq=min_freq)
     x_discretized = discretizer.fit_transform(x_train, x_train["quali_ordinal_target"])
 
     assert '__NAN__' in discretizer.values_orders["Discrete_Quantitative_lownan"], "Missing order should not be grouped with ordinal_discretizer"
     assert all(x_discretized.Quantitative.value_counts(normalize=True) >= min_freq), "Non-nan value was not grouped"
     assert discretizer.values_orders["Discrete_Quantitative_lownan"] == [1.0, 2.0, 3.0, inf, '__NAN__'], "NaNs should not be grouped whatsoever"
     assert discretizer.values_orders["Discrete_Quantitative_rarevalue"] == [1.0, 2.0, 3.0, inf], "Rare values should be grouped to the closest one (OrdinalDiscretizer)"
```

### Comparing `AutoCarver-5.0.0/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.1/tests/test_qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.0/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.1/tests/test_quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.0/tests/test_type_discretizers.py` & `AutoCarver-5.0.1/tests/test_type_discretizers.py`

 * *Files identical despite different names*

