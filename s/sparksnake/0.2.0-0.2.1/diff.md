# Comparing `tmp/sparksnake-0.2.0.tar.gz` & `tmp/sparksnake-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparksnake-0.2.0.tar", last modified: Fri Jul  7 15:19:18 2023, max compression
+gzip compressed data, was "sparksnake-0.2.1.tar", last modified: Fri Jul 14 12:37:36 2023, max compression
```

## Comparing `sparksnake-0.2.0.tar` & `sparksnake-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 15:19:05.000000 sparksnake-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-07 15:19:18.933099 sparksnake-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-07 15:19:05.000000 sparksnake-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:19:18.933099 sparksnake-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 15:19:06.000000 sparksnake-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.929099 sparksnake-0.2.0/sparksnake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31988 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.929099 sparksnake-0.2.0/sparksnake/tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/tester/dataframes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/sparksnake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 15:19:06.000000 sparksnake-0.2.0/sparksnake/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.929099 sparksnake-0.2.0/sparksnake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 15:19:18.000000 sparksnake-0.2.0/sparksnake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:18.933099 sparksnake-0.2.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/helpers/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_glue_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_manager_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_tester_dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-07 15:19:06.000000 sparksnake-0.2.0/tests/test_utils_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 12:37:24.000000 sparksnake-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-14 12:37:36.159620 sparksnake-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-14 12:37:24.000000 sparksnake-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:37:36.159620 sparksnake-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-14 12:37:25.000000 sparksnake-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31988 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38455 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/tester/dataframes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-14 12:37:25.000000 sparksnake-0.2.1/sparksnake/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/sparksnake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:37:35.000000 sparksnake-0.2.1/sparksnake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 12:37:36.000000 sparksnake-0.2.1/sparksnake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:36.159620 sparksnake-0.2.1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/helpers/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_glue_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_manager_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_tester_dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 12:37:25.000000 sparksnake-0.2.1/tests/test_utils_log.py
```

### Comparing `sparksnake-0.2.0/LICENSE` & `sparksnake-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/PKG-INFO` & `sparksnake-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.2.0
+Version: 0.2.1
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sparksnake-0.2.0/README.md` & `sparksnake-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/setup.py` & `sparksnake-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Reading README.md for project description
 with open("README.md", "r", encoding='utf-8') as f:
     __long_description__ = f.read()
 
 # Setting up package information
 setup(
     name='sparksnake',
-    version='0.2.0',
+    version='0.2.1',
     author='Thiago Panini',
     author_email='panini.development@gmail.com',
     packages=find_packages(),
     install_requires=[
         "pyspark",
         "Faker"
     ],
```

### Comparing `sparksnake-0.2.0/sparksnake/glue.py` & `sparksnake-0.2.1/sparksnake/glue.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/sparksnake/manager.py` & `sparksnake-0.2.1/sparksnake/manager.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/sparksnake/tester/dataframes.py` & `sparksnake-0.2.1/sparksnake/tester/dataframes.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ___
 """
 
 # Importing libraries
 from pyspark.sql import SparkSession, DataFrame
 from pyspark.sql.types import StructType, StructField, StringType,\
     IntegerType, LongType, DecimalType, FloatType, DoubleType, BooleanType,\
-    DateType, TimestampType
+    DateType, TimestampType, ArrayType
 
 from faker import Faker
 from decimal import Decimal
 from random import random, randrange
 
 
 # Creating a faker object
@@ -66,16 +66,36 @@
         return FloatType
     elif dtype_prep == "double":
         return DoubleType
     elif dtype_prep == "boolean":
         return BooleanType
     elif dtype_prep == "date":
         return DateType
-    elif dtype == "timestamp":
+    elif dtype_prep == "timestamp":
         return TimestampType
+    elif dtype_prep[:5] == "array":
+        # Checking if there is an inner array type
+        if "<" not in dtype and ">" not in dtype:
+            raise TypeError("Invalid entry for array type in schema "
+                            f"(dtype={dtype}). When providing an array type "
+                            "for a field in this definition schema, please "
+                            "use the following approach: 'array<inner_type>' "
+                            "where the tag 'inner_type' represents a valid "
+                            "data type reference (such as 'string', 'int'). "
+                            "It's also important not to forget to put this "
+                            "inner data type between symbols < and >")
+        else:
+            # Extracting the array inner type and parsing it into a Spark dtype
+            array_inner_dtype_str = dtype_prep.split("<")[-1].split(">")[0]
+            array_inner_dtype = parse_string_to_spark_dtype(
+                dtype=array_inner_dtype_str
+            )
+
+            # Returning the array data type with its inner type
+            return ArrayType(array_inner_dtype())
     else:
         raise TypeError(f"Data type {dtype} is not valid or currently "
                         "parseable into a native Spark dtype")
 
 
 # Creating a valid Spark DataFrame schema from a list with fields information
 def generate_dataframe_schema(
@@ -129,26 +149,48 @@
             the dictionary can hold null values
 
     Returns:
         A StructType object structured in such a way that makes it possible to\
         create a Spark DataFrame with a predefined schema.
     """
 
-    # Extracing the schema based on the preconfigured dict info
-    schema = StructType([
-        StructField(
-            field_info[attribute_name_key],
-            parse_string_to_spark_dtype(field_info[dtype_key])(),
-            nullable=field_info[nullable_key]
-            if nullable_key in field_info.keys() else True
-        ) for field_info in schema_info
+    # Creating a list of Spark data types
+    dtype_list = []
+    for field_info in schema_info:
+        # Removing noise for data type info
+        dtype_prep = field_info[dtype_key].strip().lower()
+
+        # Checking a special condition when dtype is an array
+        if dtype_prep[:5] == "array":
+            dtype = parse_string_to_spark_dtype(dtype=dtype_prep)
+        else:
+            # If it's not an array, we need to call the Spark type class
+            dtype = parse_string_to_spark_dtype(dtype=dtype_prep)()
+
+        # Appending the data type into a common list
+        dtype_list.append(dtype)
+
+    # Creating a list of attribute names
+    field_names = [
+        field_info[attribute_name_key] for field_info in schema_info
+    ]
+
+    # Creating a list of nullable information
+    nullable_list = [
+        field_info[nullable_key] if nullable_key in field_info else True
+        for field_info in schema_info
+    ]
+
+    # Extracting the schema based on the preconfigured lists
+    schema_zip_elements = zip(field_names, dtype_list, nullable_list)
+    return StructType([
+        StructField(field_name, dtype, nullable)
+        for field_name, dtype, nullable in schema_zip_elements
     ])
 
-    return schema
-
 
 # Generating fake data based on native Spark data types and the Faker library
 def generate_fake_data_from_schema(
     schema: StructType,
     n_rows: int = 5
 ) -> tuple:
     """Generates fake data based on a Struct Type Spark schema object.
@@ -213,14 +255,32 @@
                 fake_row.append(float(random() * randrange(1, 100000)))
             elif dtype == "boolean":
                 fake_row.append(faker.boolean())
             elif dtype == "date":
                 fake_row.append(faker.date_this_year())
             elif dtype == "timestamp":
                 fake_row.append(faker.date_time_this_year())
+            elif dtype == "array":
+                # Extracting inner array data type
+                inner_array_dtype = field.dataType.json()\
+                    .split("elementType")[-1]\
+                    .split(",")[0]\
+                    .split(":")[-1]\
+                    .replace('"', "")\
+                    .strip()\
+                    .lower()
+
+                # Generating fake data according to array inner type
+                if inner_array_dtype == "string":
+                    array_fake_data = faker.word()
+                elif inner_array_dtype in ("int", "integer", "bigint", "long"):
+                    array_fake_data = fake_row.append(randrange(-10000, 10000))
+
+                # Transforming fake data into a list and appending to the row
+                fake_row.append([array_fake_data])
 
         # Appending the row to the data list
         fake_data_list.append(fake_row)
 
     # Generating a list of tuples
     return [tuple(row) for row in fake_data_list]
```

### Comparing `sparksnake-0.2.0/sparksnake/utils/log.py` & `sparksnake-0.2.1/sparksnake/utils/log.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/sparksnake.egg-info/PKG-INFO` & `sparksnake-0.2.1/sparksnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksnake
-Version: 0.2.0
+Version: 0.2.1
 Summary: Improving the development of Spark applications deployed as jobs on AWS services like Glue and EMR
 Home-page: https://github.com/ThiagoPanini/sparksnake
 Author: Thiago Panini
 Author-email: panini.development@gmail.com
 License: MIT
 Keywords: Cloud,AWS,Python,Spark,pyspark
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sparksnake-0.2.0/sparksnake.egg-info/SOURCES.txt` & `sparksnake-0.2.1/sparksnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/tests/conftest.py` & `sparksnake-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/tests/helpers/user_inputs.py` & `sparksnake-0.2.1/tests/helpers/user_inputs.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/tests/test_glue_module.py` & `sparksnake-0.2.1/tests/test_glue_module.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/tests/test_manager_module.py` & `sparksnake-0.2.1/tests/test_manager_module.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/tests/test_tester_dataframes.py` & `sparksnake-0.2.1/tests/test_tester_dataframes.py`

 * *Files identical despite different names*

### Comparing `sparksnake-0.2.0/tests/test_utils_log.py` & `sparksnake-0.2.1/tests/test_utils_log.py`

 * *Files identical despite different names*

