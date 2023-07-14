# Comparing `tmp/visionai-data-format-1.0.4.tar.gz` & `tmp/visionai-data-format-1.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.4.tar", last modified: Mon Jul 10 09:36:08 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.5a1.tar", last modified: Fri Jul 14 04:46:09 2023, max compression
```

## Comparing `visionai-data-format-1.0.4.tar` & `visionai-data-format-1.0.5a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.927696 visionai-data-format-1.0.4/
--rw-r--r--   0 christian   (501) staff       (20)    16299 2023-07-10 09:36:08.927494 visionai-data-format-1.0.4/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)    16069 2023-07-10 09:14:49.000000 visionai-data-format-1.0.4/README.md
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-07-10 09:36:08.927750 visionai-data-format-1.0.4/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      753 2023-07-10 09:14:49.000000 visionai-data-format-1.0.4/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.921005 visionai-data-format-1.0.4/tests/
--rw-r--r--   0 christian   (501) staff       (20)     2176 2023-05-18 02:48:45.000000 visionai-data-format-1.0.4/tests/test_schemas.py
--rw-r--r--   0 christian   (501) staff       (20)     4731 2023-05-18 02:48:45.000000 visionai-data-format-1.0.4/tests/test_validators.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.922710 visionai-data-format-1.0.4/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7775 2023-05-19 03:23:30.000000 visionai-data-format-1.0.4/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.924805 visionai-data-format-1.0.4/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2551 2023-05-18 02:48:45.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.925413 visionai-data-format-1.0.4/visionai_data_format/schemas/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)    39355 2023-07-10 09:14:49.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 christian   (501) staff       (20)    27992 2023-07-10 09:14:49.000000 visionai-data-format-1.0.4/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.927231 visionai-data-format-1.0.4/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      494 2023-05-18 02:48:45.000000 visionai-data-format-1.0.4/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)     7898 2023-07-10 09:14:49.000000 visionai-data-format-1.0.4/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1991 2023-05-18 02:48:45.000000 visionai-data-format-1.0.4/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2308 2023-07-10 09:14:49.000000 visionai-data-format-1.0.4/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-18 02:48:43.000000 visionai-data-format-1.0.4/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-10 09:36:08.923563 visionai-data-format-1.0.4/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)    16299 2023-07-10 09:36:08.000000 visionai-data-format-1.0.4/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1122 2023-07-10 09:36:08.000000 visionai-data-format-1.0.4/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-07-10 09:36:08.000000 visionai-data-format-1.0.4/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       45 2023-07-10 09:36:08.000000 visionai-data-format-1.0.4/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-07-10 09:36:08.000000 visionai-data-format-1.0.4/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.573661 visionai-data-format-1.0.5a1/
+-rw-r--r--   0 christian   (501) staff       (20)    16301 2023-07-14 04:46:09.573446 visionai-data-format-1.0.5a1/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)    16069 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/README.md
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-07-14 04:46:09.573712 visionai-data-format-1.0.5a1/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      755 2023-07-14 04:45:38.000000 visionai-data-format-1.0.5a1/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.566645 visionai-data-format-1.0.5a1/tests/
+-rw-r--r--   0 christian   (501) staff       (20)     2176 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4731 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.568143 visionai-data-format-1.0.5a1/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7775 2023-05-19 03:23:30.000000 visionai-data-format-1.0.5a1/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.570572 visionai-data-format-1.0.5a1/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2551 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.571120 visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    39993 2023-07-14 04:34:28.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27992 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.573153 visionai-data-format-1.0.5a1/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      494 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)     7898 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1991 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2308 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.569285 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)    16301 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1122 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       45 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.4/PKG-INFO` & `visionai-data-format-1.0.5a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: visionai-data-format
-Version: 1.0.4
-Summary: converter tool for visionai format
-Home-page: 
-Author: LinkerVision
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
 # visionai-data-format
 
 `VisionAI` format is Dataverse["url"] standardized annotation format to label objects and sequences in the context of Autonomous Driving System(ADS). `VisionAI` provides consistent and effective driving environment description and categorization in the real-world case.
 
 This tool provides validator of `VisionAI` format schema. Currently, the library supports:
   - Validate created `VisionAI` data format
   - Validate `VisionAI` data attributes with given `Ontology` information.
```

### Comparing `visionai-data-format-1.0.4/README.md` & `visionai-data-format-1.0.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: visionai-data-format
+Version: 1.0.5a1
+Summary: converter tool for visionai format
+Home-page: 
+Author: LinkerVision
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+Provides-Extra: test
+
 # visionai-data-format
 
 `VisionAI` format is Dataverse["url"] standardized annotation format to label objects and sequences in the context of Autonomous Driving System(ADS). `VisionAI` provides consistent and effective driving environment description and categorization in the real-world case.
 
 This tool provides validator of `VisionAI` format schema. Currently, the library supports:
   - Validate created `VisionAI` data format
   - Validate `VisionAI` data attributes with given `Ontology` information.
```

### Comparing `visionai-data-format-1.0.4/setup.py` & `visionai-data-format-1.0.5a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.4"
+PACKAGE_VERSION = "1.0.5a1"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic==1.*"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.4/tests/test_schemas.py` & `visionai-data-format-1.0.5a1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/tests/test_validators.py` & `visionai-data-format-1.0.5a1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.5a1/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.5a1/visionai_data_format/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,18 +388,14 @@
     for frame_no, frame_obj in frames.items():
         cur_frame_no = int(frame_no)
         if not frame_obj.get(root_key):
             continue
         for uuid, data in frame_obj[root_key].items():
             for attr_type, attr_list in data[sub_root_key].items():
                 for attr in attr_list:
-                    # skip uuid that we doesn't want to validate
-                    # TODO: find better implementation
-                    if (uuid, attr["name"]) not in data_pointers:
-                        continue
                     dynamic_attrs[(uuid, attr["name"])][cur_frame_no] = {
                         "type": attr_type,
                         "val": attr["val"],
                     }
 
     return dynamic_attrs
 
@@ -729,14 +725,42 @@
                 )
 
     if msg:
         return False, msg
     return True, ""
 
 
+def gen_missing_attributes_error_message(
+    extra_attributes_name: Set[str],
+    missing_attributes_name: Set[str],
+    dynamic_attrs: dict,
+) -> str:
+    msg = ""
+    if extra_attributes_name:
+        msg += "Extra attributes from data pointers : \n"
+        for attr_name in extra_attributes_name:
+            if attr_name in dynamic_attrs:
+                msg += (
+                    f"{attr_name} with frames {list(dynamic_attrs[attr_name].keys())}\n"
+                )
+            else:
+                msg += f"{attr_name} \n"
+
+    if missing_attributes_name:
+        msg += "Missing attributes from data pointers : "
+        for attr_name in missing_attributes_name:
+            if attr_name in dynamic_attrs:
+                msg += (
+                    f"{attr_name} with frames {list(dynamic_attrs[attr_name].keys())}\n"
+                )
+            else:
+                msg += f"{attr_name} \n"
+    return msg
+
+
 def validate_visionai_data(
     data_under_vai: Dict,
     frames: Dict[str, Dict],
     root_key: str = "contexts",
     sub_root_key: str = "context_data",
     pointer_type: str = "context_data_pointers",
     tags_count: int = -1,
@@ -780,22 +804,20 @@
     )
 
     # validate if combinations of static and dynamic equals to data pointers
     combination_attrs = static_attrs_keys | dynamic_attrs_keys
     if combination_attrs ^ data_pointers_keys:
         extra_attributes_name: Set[str] = combination_attrs - data_pointers_keys
         missing_attributes_name: Set[str] = data_pointers_keys - combination_attrs
-        msg = ""
-        if extra_attributes_name:
-            msg += f"Extra attributes from data pointers : {extra_attributes_name} \n"
-
-        if missing_attributes_name:
-            msg += (
-                f"Missing attributes from data pointers : {missing_attributes_name} \n"
-            )
+        msg: str = gen_missing_attributes_error_message(
+            extra_attributes_name=extra_attributes_name,
+            missing_attributes_name=missing_attributes_name,
+            dynamic_attrs=dynamic_attrs,
+        )
+
         return False, msg
 
     # retrieve frame numbers
     frame_numbers = [int(frame_num) for frame_num in frames.keys()]
 
     # create frame intervals from frame numbers in case the frames is not continuous
     visionai_frame_intervals: List[Tuple[int, int]] = gen_intervals(frame_numbers)
```

### Comparing `visionai-data-format-1.0.4/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/visionai_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.5a1/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.5a1/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.4/visionai_data_format.egg-info/PKG-INFO` & `visionai-data-format-1.0.5a1/visionai_data_format.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.0.4
+Version: 1.0.5a1
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.0.4/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.5a1/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

