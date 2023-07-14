# Comparing `tmp/oarepo-model-builder-vocabularies-4.0.3.tar.gz` & `tmp/oarepo-model-builder-vocabularies-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.3.tar", last modified: Mon Jul  3 13:14:18 2023, max compression
+gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.4.tar", last modified: Fri Jul 14 10:29:54 2023, max compression
```

## Comparing `oarepo-model-builder-vocabularies-4.0.3.tar` & `oarepo-model-builder-vocabularies-4.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.610374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:19.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-03 13:14:18.000000 oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 13:14:18.614374 oarepo-model-builder-vocabularies-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 13:10:21.000000 oarepo-model-builder-vocabularies-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:54.901685 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:26:58.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 10:29:54.000000 oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-14 10:29:54.905685 oarepo-model-builder-vocabularies-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-14 10:26:04.000000 oarepo-model-builder-vocabularies-4.0.4/setup.py
```

### Comparing `oarepo-model-builder-vocabularies-4.0.3/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.3
+Version: 4.0.4
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/components.py` & `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/datatypes.py` & `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import marshmallow as ma
 from marshmallow import fields
 from oarepo_model_builder.datatypes.datatypes import DataType
 from oarepo_model_builder.validation import InvalidModelException
 from oarepo_model_builder_relations.datatypes import RelationDataType
+from oarepo_model_builder.datatypes.components.model.utils import array_contains_value
 
 
 class VocabularyDataType(RelationDataType):
     model_type = "vocabulary"
     facets = {
         'facet-class': "VocabularyFacet",
         'imports': [
@@ -50,15 +51,18 @@
                 pid_field = f"{vocabulary_class}.pid"
 
         # self.definition["type"] = "relation"
         self.definition["pid-field"] = pid_field
 
         # set up vocabulary argument to facets
         facets = self.definition.setdefault('facets', {})
-        facets.setdefault('args', []).append(f'vocabulary={repr(vocabulary_type)}')
+        facets_args = facets.setdefault('args', [])
+        vocabulary_attr = f'vocabulary={repr(vocabulary_type)}'
+        if not array_contains_value(facets_args, vocabulary_attr):
+            facets_args.append(vocabulary_attr)
 
         super().prepare(context)
 
     def get_facet(self, stack, parent_path):
         if not stack:
             # we are the facet, unlike normal container, for which a facet is not generated,
             # we need to generate it -> calling direct data type
```

### Comparing `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.json` & `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies/models/vocabulary.yaml` & `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies/models/vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.3
+Version: 4.0.4
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.3/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt` & `oarepo-model-builder-vocabularies-4.0.4/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.3/setup.cfg` & `oarepo-model-builder-vocabularies-4.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-vocabularies
-version = 4.0.3
+version = 4.0.4
 description = "A model builder plugin to reference vocabularies"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio vocabulary model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

