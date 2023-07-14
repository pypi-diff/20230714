# Comparing `tmp/AutoCarver-5.0.1.tar.gz` & `tmp/AutoCarver-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.1.tar", last modified: Thu Jul 13 23:13:38 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.2.tar", last modified: Fri Jul 14 00:02:19 2023, max compression
```

## Comparing `AutoCarver-5.0.1.tar` & `AutoCarver-5.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.967907 AutoCarver-5.0.1/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29716 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38974 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26042 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 23:13:38.000000 AutoCarver-5.0.1/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:13:38.971907 AutoCarver-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 23:13:27.000000 AutoCarver-5.0.1/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.708739 AutoCarver-5.0.2/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39408 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26042 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 00:02:19.000000 AutoCarver-5.0.2/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:02:19.712739 AutoCarver-5.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-14 00:02:09.000000 AutoCarver-5.0.2/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.1/AutoCarver/auto_carver.py` & `AutoCarver-5.0.2/AutoCarver/auto_carver.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
         # Initiating GroupedListDiscretizer
         super().__init__(
             features=self.features,
             values_orders=values_orders,
             input_dtypes=self.input_dtypes,
             output_dtype=output_dtype,
             str_nan=str_nan,
+            dropna=dropna,
             copy=copy,
         )
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
         self.dropna = dropna  # whether or not to group NaNs with other modalities
```

### Comparing `AutoCarver-5.0.1/AutoCarver/converters.py` & `AutoCarver-5.0.2/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.2/AutoCarver/discretizers/discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
         Parameters
         ----------
         feature : str
             Column name of the feature
         """
         if feature in self.features:
             super().remove_feature(feature)
-            self.features.remove(feature)
             if feature in self.ordinal_features:
                 self.ordinal_features.remove(feature)
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """_summary_
 
         Parameters
```

### Comparing `AutoCarver-5.0.1/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.2/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Parameters
     ----------
     x : Series
         Values to be deduplicated.
 
     Returns
     -------
-    List[Any]
+    list[Any]
         List of unique non-nan values
     """
 
     # unique values
     uniques = unique(x)
 
     # filtering out nans
@@ -39,15 +39,15 @@
     Parameters
     ----------
     applied : Union[DataFrame, Series]
         Result of pandas.DataFrame.apply
 
     Returns
     -------
-    Dict[List[Any]]
+    Dict[list[Any]]
         Dict of lists of rows values
     """
     # TODO: use this function whenever apply is used
 
     # case when it's a Series
     converted = applied.to_dict()
 
@@ -55,24 +55,24 @@
     if isinstance(applied, DataFrame):
         converted = applied.to_dict(orient="list")
 
     return converted
 
 
 # TODO: remove known_values
-def check_new_values(X: DataFrame, features: List[str], known_values: Dict[str, List[Any]]) -> None:
+def check_new_values(X: DataFrame, features: list[str], known_values: dict[str, list[Any]]) -> None:
     """Checks for new, unexpected values, in X
 
     Parameters
     ----------
     X : DataFrame
         New DataFrame (at transform time)
-    features : List[str]
+    features : list[str]
         List of column names
-    known_values : Dict[str, List[Any]]
+    known_values : dict[str, list[Any]]
         Dict of known values per column name
     """
     # unique non-nan values in new dataframe
     uniques = X[features].apply(
         nan_unique,
         axis=0,
         result_type="expand",
@@ -84,25 +84,25 @@
         unexpected = [val for val in uniques[feature] if val not in known_values[feature]]
         assert (
             len(unexpected) == 0
         ), f"Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was not provided. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
 
 
 def check_missing_values(
-    X: DataFrame, features: List[str], known_values: Dict[str, List[Any]]
+    X: DataFrame, features: list[str], known_values: dict[str, list[Any]]
 ) -> None:
     """Checks for missing values from X, (unexpected values in values_orders)
 
     Parameters
     ----------
     X : DataFrame
         New DataFrame (at transform time)
-    features : List[str]
+    features : list[str]
         List of column names
-    known_values : Dict[str, List[Any]]
+    known_values : dict[str, list[Any]]
         Dict of known values per column name
     """
     # unique non-nan values in new dataframe
     uniques = X[features].apply(
         nan_unique,
         axis=0,
         result_type="expand",
@@ -182,25 +182,25 @@
         elif isinstance(iterable, list):
             # initiating the list with the provided list of keys
             super().__init__(iterable)
 
             # initiating the values with the provided list of keys
             self.contained = {v: [v] for v in iterable}
 
-    def get(self, key: Any) -> List[Any]:
+    def get(self, key: Any) -> list[Any]:
         """List of values contained in key
 
         Parameters
         ----------
         key : Any
             Group.
 
         Returns
         -------
-        List[Any]
+        list[Any]
             Values contained in key
         """
 
         # default to fing an element
         found = self.contained.get(key)
 
         return found
@@ -228,20 +228,20 @@
 
             # updating contained dict
             self.contained.update({kept: contained_discarded + contained_kept, discarded: []})
 
             # removing discarded from the list
             self.remove(discarded)
 
-    def group_list(self, to_discard: List[Any], to_keep: Any) -> None:
+    def group_list(self, to_discard: list[Any], to_keep: Any) -> None:
         """Groups elements to_discard into values to_keep
 
         Parameters
         ----------
-        to_discard : List[Any]
+        to_discard : list[Any]
             Values to be grouped into the key `to_keep`.
         to_keep : Any
             Key value in which to group `to_discard` values.
         """
 
         for discarded, kept in zip(to_discard, [to_keep] * len(to_discard)):
             self.group(discarded, kept)
@@ -254,20 +254,20 @@
         new_value : Any
             New key to be added.
         """
 
         self += [new_value]
         self.contained.update({new_value: [new_value]})
 
-    def update(self, new_value: Dict[Any, List[Any]]) -> None:
+    def update(self, new_value: Dict[Any, list[Any]]) -> None:
         """Updates the GroupedList via a dict
 
         Parameters
         ----------
-        new_value : Dict[Any, List[Any]]
+        new_value : Dict[Any, list[Any]]
             Dict of key, values to updated `contained` dict
         """
 
         # adding keys to the order if they are new values
         self += [key for key, _ in new_value.items() if key not in self]
 
         # updating contained according to new_value
@@ -291,20 +291,20 @@
         keys = list(sort(keys_str)) + list(sort(keys_float))
 
         # recreating an ordered GroupedList
         sorted = GroupedList({k: self.get(k) for k in keys})
 
         return sorted
 
-    def sort_by(self, ordering: List[Any]) -> None:
+    def sort_by(self, ordering: list[Any]) -> None:
         """Sorts the values of the list and dict according to `ordering`, if any, NaNs are the last.
 
         Parameters
         ----------
-        ordering : List[Any]
+        ordering : list[Any]
             Order used for ordering of the list of keys.
 
         Returns
         -------
         GroupedList
             Sorted GroupedList
         """
@@ -365,20 +365,20 @@
         ]
 
         if any(found):
             return found[0]
 
         return value
 
-    def values(self) -> List[Any]:
+    def values(self) -> list[Any]:
         """All values contained in all groups
 
         Returns
         -------
-        List[Any]
+        list[Any]
             List of all values in the GroupedList
         """
 
         known = [value for values in self.contained.values() for value in values]
 
         return known
 
@@ -396,30 +396,30 @@
             Whether the value is in the GroupedList
         """
 
         known_values = self.values()
 
         return any(is_equal(value, known) for known in known_values)
 
-    def get_repr(self, char_limit: int = 6) -> List[str]:
+    def get_repr(self, char_limit: int = 6) -> list[str]:
         """Returns a representative list of strings of values of groups.
 
         Parameters
         ----------
         char_limit : int, optional
             Maximum number of character per string, by default 6
 
         Returns
         -------
-        List[str]
+        list[str]
             List of short str representation of the keys' values
         """
 
         # initiating list of group representation
-        repr: List[str] = []
+        repr: list[str] = []
 
         # iterating over each group
         for group in self:
             # accessing group's values
             values = self.get(group)
 
             if len(values) == 0:  # case 0: there are no value in this group
@@ -447,14 +447,15 @@
         self,
         features: list[str],
         *,
         values_orders: dict[str, GroupedList] = None,
         input_dtypes: Union[str, dict[str, str]] = 'str',
         output_dtype: str = 'str',
         str_nan: str = None,
+        dropna: bool = True,
         copy: bool = False,
     ) -> None:
         """Initiates a Discretizer by dict of GroupedList
 
         Parameters
         ----------
         features : list[str]
@@ -472,71 +473,74 @@
         str_nan : str, optional
             Default string value attributed to nan, by default None
         copy : bool, optional
             Whether or not to copy the input DataFrame, by default False
         """
         self.features = list(set(features))
         if values_orders is None:
-            values_orders = {}
+            values_orders: dict[str, GroupedList] = {}
         self.values_orders = {feature: GroupedList(values) for feature, values in values_orders.items()}
         self.copy = copy
 
         # input feature types
         if isinstance(input_dtypes, str):
             input_dtypes = {feature: input_dtypes for feature in features}
         self.input_dtypes = input_dtypes
 
         # output type
         self.output_dtype = output_dtype
 
         # string value of numpy.nan
         self.str_nan = str_nan
 
+        # whether or not to reinstate numpy nan after bucketization
+        self.dropna = dropna
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
-        self.labels_per_values = {}  # will be initiated during fit
+        self.labels_per_values: dict[str, dict[Any, Any]]= {}  # will be initiated during fit
 
     def get_labels_per_values(self) -> dict[str, dict[Any, Any]]:
         """Creates a dict that contains, for each feature, for each value, the associated label
 
         Returns
         -------
         dict[str, dict[Any, Any]]
             Dict of labels per values per feature
         """
         # initiating dict of labels per values per feature
-        labels_per_values = {}
+        labels_per_values: dict[str, dict[Any, Any]] = {}
 
         # iterating over each feature
         for feature in self.features:
             # known values of the feature(grouped)
             values = self.values_orders[feature]
 
             # case 0: quantitative feature -> labels per quantile (removes str_nan)
             if feature in self.quantitative_features:
                 labels = get_labels(values, self.str_nan)
             # case 1: qualitative feature -> by default, labels are values
             else:
-                labels = values[:]
+                labels = [value for value in values if value != self.str_nan]  # (removing str_nan)
             
             # case 2: requested float output -> converting to integers
             if self.output_dtype == 'float':
                 labels = [n for n, _ in enumerate(labels)]
 
             # building label per value
-            label_per_value = {}
+            label_per_value: dict[Any, Any] = {}
             for group_of_values, label in zip(values, labels):
                 for value in values.get(group_of_values):
                     label_per_value.update({value: label})
             
             # storing in full dict
             labels_per_values.update({feature: label_per_value})
         
@@ -638,14 +642,18 @@
         # transforming quantitative features
         if len(self.quantitative_features) > 0:
             x_copy = self.transform_quantitative(x_copy, y)
 
         # transforming qualitative features
         if len(self.qualitative_features) > 0:
             x_copy = self.transform_qualitative(x_copy, y)
+        
+        # reinstating nans
+        if not self.dropna:
+            x_copy[self.features] = x_copy[self.features].replace(self.str_nan, nan)
 
         return x_copy
 
     def transform_quantitative(self, X: DataFrame, y: Series) -> DataFrame:
         """Groups values of features (values_orders keys) according to
         there corresponding GroupedList (values_orders values) based on
         the `GroupedList.contained` dict.
@@ -805,20 +813,20 @@
 
                 summaries += [modality_summary]
 
         return summaries
 
 
 def convert_to_labels(
-    features: List[str],
-    quantitative_features: List[str],
-    values_orders: Dict[str, GroupedList],
+    features: list[str],
+    quantitative_features: list[str],
+    values_orders: dict[str, GroupedList],
     str_nan: str,
     dropna: bool = True,
-) -> Dict[str, GroupedList]:
+) -> dict[str, GroupedList]:
     """Converts a values_orders values to labels (quantiles)"""
 
     # copying values_orders without nans
     labels_orders = {
         feature: GroupedList([value for value in values_orders[feature] if value != str_nan])
         for feature in features
     }
@@ -900,25 +908,25 @@
         values_orders.update({feature: order})
 
     return values_orders
 
 
 def min_value_counts(
     x: Series,
-    values_orders: Dict[str, GroupedList] = None,
+    values_orders: dict[str, GroupedList] = None,
     dropna: bool = False,
     normalize: bool = True,
 ) -> float:
     """Minimum of modalities' frequencies.
 
     Parameters
     ----------
     x : Series
         _description_
-    values_orders : Dict[str, GroupedList]
+    values_orders : dict[str, GroupedList]
         _description_
 
     Returns
     -------
     float
         _description_
     """
@@ -1033,29 +1041,29 @@
     # Case where a and b are NaNs
     if isna(a) and isna(b):
         equal = True
 
     return equal
 
 
-def get_labels(quantiles: List[float], str_nan: str) -> List[str]:
+def get_labels(quantiles: list[float], str_nan: str) -> list[str]:
     """_summary_
 
     Parameters
     ----------
     feature : str
         _description_
     order : GroupedList
         _description_
     str_nan : str
         _description_
 
     Returns
     -------
-    List[str]
+    list[str]
         _description_
     """
     # filtering out nan for formatting
     if str_nan in quantiles:
         quantiles = [val for val in quantiles if val != str_nan]
 
     # filtering out inf for formatting
@@ -1065,30 +1073,30 @@
     # converting quantiles in string
     labels = format_quantiles(quantiles)
 
     return labels
 
 
 def get_quantiles_labels(
-    features: List[str], values_orders: Dict[str, GroupedList], str_nan: str
-) -> Dict[str, GroupedList]:
+    features: list[str], values_orders: dict[str, GroupedList], str_nan: str
+) -> dict[str, GroupedList]:
     """Converts a values_orders of quantiles into a values_orders of string quantiles
 
     Parameters
     ----------
-    features : List[str]
+    features : list[str]
         _description_
-    values_orders : Dict[str, GroupedList]
+    values_orders : dict[str, GroupedList]
         _description_
     str_nan : str
         _description_
 
     Returns
     -------
-    Dict[str, GroupedList]
+    dict[str, GroupedList]
         _description_
     """
     # applying quantiles formatting to orders of specified features
     quantiles_to_labels = {}
     for feature in features:
         quantiles = list(values_orders[feature])
         labels = get_labels(quantiles, str_nan)
@@ -1097,30 +1105,30 @@
             {feature: {quantile: alias for quantile, alias in zip(quantiles, labels)}}
         )
 
     return quantiles_to_labels
 
 
 def get_labels_quantiles(
-    features: List[str], values_orders: Dict[str, GroupedList], str_nan: str
-) -> Dict[str, GroupedList]:
+    features: list[str], values_orders: dict[str, GroupedList], str_nan: str
+) -> dict[str, GroupedList]:
     """Converts a values_orders of quantiles into a values_orders of string quantiles
 
     Parameters
     ----------
-    features : List[str]
+    features : list[str]
         _description_
-    values_orders : Dict[str, GroupedList]
+    values_orders : dict[str, GroupedList]
         _description_
     str_nan : str
         _description_
 
     Returns
     -------
-    Dict[str, GroupedList]
+    dict[str, GroupedList]
         _description_
     """
     # applying quantiles formatting to orders of specified features
     labels_to_quantiles = {}
     for feature in features:
         quantiles = list(values_orders[feature])
         labels = get_labels(quantiles, str_nan)
@@ -1128,40 +1136,40 @@
         labels_to_quantiles.update(
             {feature: {alias: quantile for quantile, alias in zip(quantiles, labels)}}
         )
 
     return labels_to_quantiles
 
 
-def format_quantiles(a_list: List[float]) -> List[str]:
+def format_quantiles(a_list: list[float]) -> list[str]:
     """Formats a list of float quantiles into a list of boundaries.
 
     Rounds quantiles to the closest power of 1000.
 
     Parameters
     ----------
-    a_list : List[float]
+    a_list : list[float]
         Sorted list of quantiles to convert into string
 
     Returns
     -------
-    List[str]
+    list[str]
         List of boundaries per quantile
     """
 
     # finding the closest power of thousands for each element
     closest_powers = [
         next((k for k in range(-3, 4) if abs(elt) / 100 // 1000 ** (k) < 10)) for elt in a_list
     ]
 
     # rounding elements to the closest power of thousands
     rounded_to_powers = [elt / 1000 ** (k) for elt, k in zip(a_list, closest_powers)]
 
     # computing optimal decimal per unique power of thousands
-    optimal_decimals: Dict[str, int] = {}
+    optimal_decimals: dict[str, int] = {}
     for power in unique(closest_powers):  # iterating over each power of thousands found
         # filtering on the specific power of thousands
         sub_array = array([elt for elt, p in zip(rounded_to_powers, closest_powers) if power == p])
 
         # number of distinct values
         n_uniques = sub_array.shape[0]
 
@@ -1172,15 +1180,15 @@
             None,
         )
 
         # storing in the dict
         optimal_decimals.update({power: optimal_decimal})
 
     # rounding according to each optimal_decimal
-    rounded_list: List[float] = []
+    rounded_list: list[float] = []
     for elt, power in zip(rounded_to_powers, closest_powers):
         # rounding each element
         rounded = elt  # by default None (no rounding)
         optimal_decimal = optimal_decimals.get(power)
         if optimal_decimal:  # checking that the optimal decimal exists
             rounded = round(elt, optimal_decimal)
 
@@ -1202,15 +1210,15 @@
 
     # stripping whitespaces
     formatted_list = [string.strip() for string in formatted_list]
 
     # low and high bounds per quantiles
     upper_bounds = formatted_list + [nan]
     lower_bounds = [nan] + formatted_list
-    order: List[str] = []
+    order: list[str] = []
     for lower, upper in zip(lower_bounds, upper_bounds):
         if isna(lower):
             order += [f"x <= {upper}"]
         elif isna(upper):
             order += [f"{lower} < x"]
         else:
             order += [f"{lower} < x <= {upper}"]
```

### Comparing `AutoCarver-5.0.1/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.2/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.2/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.0.2/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/AutoCarver/feature_selector.py` & `AutoCarver-5.0.2/AutoCarver/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.2/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.1
+Version: 5.0.2
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.1/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.2/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/LICENSE` & `AutoCarver-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/PKG-INFO` & `AutoCarver-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.1
+Version: 5.0.2
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `AutoCarver-5.0.1/README.md` & `AutoCarver-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/setup.py` & `AutoCarver-5.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.1",
+    version="5.0.2",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.0.1/tests/test_auto_carver.py` & `AutoCarver-5.0.2/tests/test_auto_carver.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         qualitative_features=qualitative_features,
         ordinal_features=ordinal_features,
         values_orders=values_orders,
         min_freq=min_freq,
         max_n_mod=max_n_mod,
         sort_by='tschuprowt',
         output_dtype='str',
+        dropna=True,
         copy=True,
         verbose=False,
     )
     x_discretized = auto_carver.fit_transform(x_train, x_train["quali_ordinal_target"], X_test=x_test_1, y_test=x_test_1["quali_ordinal_target"])
     x_test_discretized = auto_carver.transform(x_test_1)
 
     assert all(x_discretized[auto_carver.features].nunique() <= max_n_mod), "Too many values after carving of train sample"
@@ -55,14 +56,15 @@
         quantitative_features=quantitative_features,
         qualitative_features=qualitative_features,
         ordinal_features=ordinal_features,
         values_orders=values_orders,
         min_freq=min_freq,
         max_n_mod=max_n_mod,
         sort_by='cramerv',
+        dropna=True,
         copy=True,
         verbose=False,
     )
     x_discretized = auto_carver.fit_transform(x_train, x_train["quali_ordinal_target"], X_test=x_test_1, y_test=x_test_1["quali_ordinal_target"])
     x_test_discretized = auto_carver.transform(x_test_1)
 
     assert all(x_discretized[auto_carver.features].nunique() <= max_n_mod), "Too many values after carving of train sample"
@@ -70,10 +72,27 @@
     assert all(x_discretized[auto_carver.features].nunique() == x_test_discretized[auto_carver.features].nunique()), "More values in train or test samples"
 
     # test that all values still are in the values_orders
     for feature in auto_carver.qualitative_features:
         fitted_values = auto_carver.values_orders[feature].values()
         init_values = x_train[feature].fillna('__NAN__').unique()
         assert all(value in fitted_values for value in init_values), feature
+    
+    # tests with dropna=False
+    auto_carver = AutoCarver(
+        quantitative_features=quantitative_features,
+        qualitative_features=qualitative_features,
+        ordinal_features=ordinal_features,
+        values_orders=values_orders,
+        min_freq=0.06,
+        max_n_mod=max_n_mod,
+        sort_by='cramerv',
+        dropna=False,
+        copy=True,
+        verbose=False,
+    )
+    x_discretized = auto_carver.fit_transform(x_train, x_train["quali_ordinal_target"])
+
+    assert all(x_train[auto_carver.features].isna().mean()  == x_discretized[auto_carver.features].isna().mean()), "Some Nans are being dropped (grouped)"
 
     # TODO: test output 'float'
     # TODO test missing values in test
```

### Comparing `AutoCarver-5.0.1/tests/test_base_discretizers.py` & `AutoCarver-5.0.2/tests/test_base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/tests/test_discretizers.py` & `AutoCarver-5.0.2/tests/test_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.2/tests/test_qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.2/tests/test_quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.1/tests/test_type_discretizers.py` & `AutoCarver-5.0.2/tests/test_type_discretizers.py`

 * *Files identical despite different names*

