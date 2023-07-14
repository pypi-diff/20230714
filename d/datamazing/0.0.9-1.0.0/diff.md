# Comparing `tmp/datamazing-0.0.9.tar.gz` & `tmp/datamazing-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-0.0.9.tar", max compression
+gzip compressed data, was "datamazing-1.0.0.tar", max compression
```

## Comparing `datamazing-0.0.9.tar` & `datamazing-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       21 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      126 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      826 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3818 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     2781 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      153 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2070 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0      540 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      708 2023-07-12 07:04:04.108982 datamazing-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/_conform.py
+-rw-r--r--   0        0        0      295 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     3818 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     3353 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0      868 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2064 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     1682 2023-07-14 09:16:50.024118 datamazing-1.0.0/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-14 09:16:50.024118 datamazing-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-1.0.0/PKG-INFO
```

### Comparing `datamazing-0.0.9/datamazing/pandas/testing/assertions.py` & `datamazing-1.0.0/datamazing/pandas/testing/assertions.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 
 
 def assert_frame_equal(
     left: pd.DataFrame,
     right: pd.DataFrame,
     check_order: bool = False,
 ):
-    pd.testing.assert_index_equal(left.columns, right.columns)
-
-    columns = list(left.columns)
     if check_order:
         pd.testing.assert_frame_equal(left, right)
     else:
+        columns = list(left.columns)
         pd.testing.assert_frame_equal(
             left=left.sort_values(by=columns).reset_index(drop=True),
             right=right.sort_values(by=columns).reset_index(drop=True),
             check_like=True,
         )
```

### Comparing `datamazing-0.0.9/datamazing/pandas/testing/data.py` & `datamazing-1.0.0/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.9/datamazing/pandas/transformations/basic.py` & `datamazing-1.0.0/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.9/datamazing/pandas/transformations/resampling.py` & `datamazing-1.0.0/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.9/datamazing/pandas/types.py` & `datamazing-1.0.0/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.9/datamazing/pyspark/testing/data.py` & `datamazing-1.0.0/datamazing/pyspark/testing/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datamazing.pandas.datacollection import TimeInterval
 from datamazing.pandas.testing.data import get_filepath  # noqa: F401
 
 
 def make_df(data: list[dict]):
     spark = ps.SparkSession.getActiveSession()
 
-    return spark.createDataFrame(pd.DataFrame.from_records(data))
+    return spark.createDataFrame(pdz.testing.make_df(data))
 
 
 def read_df(
     filename: str,
     subfolder: str = "data",
 ) -> ps.DataFrame:
     """
```

### Comparing `datamazing-0.0.9/pyproject.toml` & `datamazing-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "0.0.9"
+version = "1.0.0"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-0.0.9/PKG-INFO` & `datamazing-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 0.0.9
+Version: 1.0.0
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

