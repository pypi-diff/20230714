# Comparing `tmp/discovery-core-0.2.3.tar.gz` & `tmp/discovery-core-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.3.tar", last modified: Wed Jul 12 21:09:50 2023, max compression
+gzip compressed data, was "discovery-core-0.2.4.tar", last modified: Thu Jul 13 23:39:27 2023, max compression
```

## Comparing `discovery-core-0.2.3.tar` & `discovery-core-0.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.396818 discovery-core-0.2.3/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.3/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.3/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:09:50.397028 discovery-core-0.2.3/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.3/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.378588 discovery-core-0.2.3/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-12 21:09:50.000000 discovery-core-0.2.3/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.378943 discovery-core-0.2.3/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-12 21:03:05.000000 discovery-core-0.2.3/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.381288 discovery-core-0.2.3/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.3/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21096 2023-07-12 21:06:16.000000 discovery-core-0.2.3/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.383422 discovery-core-0.2.3/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.3/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.3/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.384462 discovery-core-0.2.3/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.3/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.387719 discovery-core-0.2.3/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.3/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.3/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.3/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-12 21:09:50.397651 discovery-core-0.2.3/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.3/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.388725 discovery-core-0.2.3/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.3/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.390466 discovery-core-0.2.3/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.3/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14057 2023-07-12 21:07:34.000000 discovery-core-0.2.3/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.391867 discovery-core-0.2.3/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.3/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.3/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.393811 discovery-core-0.2.3/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.3/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.3/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-12 21:09:50.395956 discovery-core-0.2.3/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.3/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.3/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.3/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.802174 discovery-core-0.2.4/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.4/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.4/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-13 23:39:27.802355 discovery-core-0.2.4/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.4/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.783957 discovery-core-0.2.4/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-13 23:39:27.000000 discovery-core-0.2.4/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-13 23:39:27.000000 discovery-core-0.2.4/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-13 23:39:27.000000 discovery-core-0.2.4/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-13 23:39:27.000000 discovery-core-0.2.4/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.784300 discovery-core-0.2.4/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-12 21:12:39.000000 discovery-core-0.2.4/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.786753 discovery-core-0.2.4/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.4/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    22577 2023-07-13 23:11:46.000000 discovery-core-0.2.4/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.789249 discovery-core-0.2.4/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.4/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7794 2023-06-29 15:03:02.000000 discovery-core-0.2.4/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.790367 discovery-core-0.2.4/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.4/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.793533 discovery-core-0.2.4/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.4/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.4/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.4/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-13 23:39:27.802952 discovery-core-0.2.4/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.4/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.794494 discovery-core-0.2.4/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.4/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.796029 discovery-core-0.2.4/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.4/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15008 2023-07-13 23:32:33.000000 discovery-core-0.2.4/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.797399 discovery-core-0.2.4/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.4/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.4/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.799292 discovery-core-0.2.4/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.4/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.4/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-13 23:39:27.801474 discovery-core-0.2.4/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.4/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.4/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.4/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.3/LICENSE.txt` & `discovery-core-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/PKG-INFO` & `discovery-core-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.3/README.rst` & `discovery-core-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.2.4/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.3/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.2.4/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/components/abstract_component.py` & `discovery-core-0.2.4/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/components/core_commons.py` & `discovery-core-0.2.4/ds_core/components/core_commons.py`

 * *Files 6% similar despite different names*

```diff
@@ -287,14 +287,52 @@
                     working = True
                 if pa.types.is_struct(record.type):
                     t = t.flatten()
                     working = True
         return t
 
     @staticmethod
+    def table_nest(t: pa.Table) -> list:
+        """ turns a flattened table back to a nested pattern """
+
+        def set_dict(tree, vector, value):
+            key = vector[0]
+            tree[key] = value if len(vector) == 1 else set_dict(tree[key] if key in tree else {}, vector[1:], value)
+            return tree
+
+        def set_list(struct, keys, tree):
+            for key in tuple(struct.keys()):
+                if isinstance(struct.get(key), dict) and len(struct.get(key)) > 0:
+                    keys.append(key)
+                    set_list(struct.get(key), keys, tree)
+                if str(key).isnumeric():
+                    snippet = list([struct.get(key, {})])
+                    if snippet[0] == {}:
+                        continue
+                    branch = tree
+                    for k in keys[:-1]:
+                        branch = branch.get(k)
+                    snippet = list(struct.values())
+                    struct.clear()
+                    branch[keys[-1]] = snippet
+            if len(keys) > 0:
+                keys.pop()
+            return tree
+
+        rtn_lst = []
+        for idx in range(t.num_rows):
+            rtn_value = {}
+            for n in t.column_names:
+                values = t.column(n).to_pylist()
+                rtn_value = set_dict(rtn_value, n.split('.'), values[idx])
+            rtn_value = set_list(rtn_value, [], rtn_value)
+            rtn_lst.append(rtn_value)
+        return rtn_lst
+
+    @staticmethod
     def column_cast(a: pa.Array, ty: pa.DataType) -> pa.Array:
         """ attempt to cast a pyarrow array to the given type """
         try:
             return a.cast(ty)
         except (ArrowInvalid, ArrowTypeError, ArrowNotImplementedError):
             return a
```

### Comparing `discovery-core-0.2.3/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.2.4/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.2.4/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/intent/abstract_intent.py` & `discovery-core-0.2.4/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/properties/abstract_properties.py` & `discovery-core-0.2.4/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/properties/decorator_patterns.py` & `discovery-core-0.2.4/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/ds_core/properties/property_manager.py` & `discovery-core-0.2.4/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/setup.py` & `discovery-core-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/components/abstract_component_test.py` & `discovery-core-0.2.4/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/components/commons_test.py` & `discovery-core-0.2.4/test/components/commons_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,33 @@
         control = ['_id',
                    'interactionDate.endDateTime', 'interactionDate.startDateTime',
                    'relatedParty.0._id', 'relatedParty.0.engagedParty.referredType', 'relatedParty.0.role',
                    'relatedParty.1._id', 'relatedParty.1.engagedParty.referredType', 'relatedParty.1.role',
                    'productId.0']
         self.assertEqual(control, result.column_names)
 
+    def test_table_nest(self):
+        document = [
+            {"_id": "PI1832341",
+             "interactionDate": {"startDateTime": "2023-01-02 04:49:06.955000",
+                                 "endDateTime": "2023-01-02 04:50:35.130000"},
+             "relatedParty": [{"_id": "C5089669",
+                               "role": "Customer",
+                               "engagedParty": {"referredType": "Individual"}},
+                              {"_id": "dclmappuser1",
+                               "role": "CSRAgent"}],
+             "productId": ["PR716796"],
+             }
+        ]
+        tbl = CoreCommons.table_flatten(pa.Table.from_pylist(document))
+        result = CoreCommons.table_nest(tbl)
+        self.assertCountEqual(['_id', 'interactionDate', 'relatedParty', 'productId'], result[0].keys())
+        self.assertIsInstance(result[0].get('relatedParty'), list)
+        self.assertEqual(len(result[0].get('relatedParty')), 2)
+
     def test_array_cast(self):
         num = pa.array([1.0, 12.0, 5.0, None], pa.float64())
         date = pa.array(["2023-01-02 04:49:06", "2023-01-02 04:57:12", None, "2023-01-02 05:23:50"], pa.string())
         text = pa.array(["Blue", "Green", None, 'Blue'], pa.string())
         bool1 = pa.array([1, 0, 1, None], pa.int64())
         bool2 = pa.array(['true', 'true', None, 'false'], pa.string())
         bool3 = pa.array([None, 'no', 'yes', 'yes'], pa.string())
```

### Comparing `discovery-core-0.2.3/test/handlers/connector_contract_test.py` & `discovery-core-0.2.4/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/handlers/handler_factory_test.py` & `discovery-core-0.2.4/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/intent/abstract_intent_test.py` & `discovery-core-0.2.4/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/intent/pyarrow_intent_model.py` & `discovery-core-0.2.4/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.2.4/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.3/test/properties/property_manager_test.py` & `discovery-core-0.2.4/test/properties/property_manager_test.py`

 * *Files identical despite different names*

