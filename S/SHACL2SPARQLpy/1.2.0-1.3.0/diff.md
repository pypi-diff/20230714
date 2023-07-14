# Comparing `tmp/SHACL2SPARQLpy-1.2.0.tar.gz` & `tmp/SHACL2SPARQLpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SHACL2SPARQLpy-1.2.0.tar", last modified: Thu Jul  6 08:09:53 2023, max compression
+gzip compressed data, was "SHACL2SPARQLpy-1.3.0.tar", last modified: Fri Jul 14 10:29:33 2023, max compression
```

## Comparing `SHACL2SPARQLpy-1.2.0.tar` & `SHACL2SPARQLpy-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.462941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/DependencyGraphImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    22086 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/RuleBasedValidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/SchemaImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/Literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/Query.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RuleMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/RuleBasedValidStats.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/fileManagement.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.462941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.064504 SHACL2SPARQLpy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-14 10:29:33.064504 SHACL2SPARQLpy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.060504 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/DependencyGraphImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/Eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22086 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/RuleBasedValidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/SchemaImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/ShapeNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.060504 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.064504 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/Literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/Query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/RuleMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.064504 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.064504 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/utils/RuleBasedValidStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/utils/fileManagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/utils/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:29:33.060504 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-14 10:29:33.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-14 10:29:33.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:29:33.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 10:29:33.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 10:29:33.000000 SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-14 10:29:33.064504 SHACL2SPARQLpy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-14 10:29:19.000000 SHACL2SPARQLpy-1.3.0/setup.py
```

### Comparing `SHACL2SPARQLpy-1.2.0/LICENSE` & `SHACL2SPARQLpy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/PKG-INFO` & `SHACL2SPARQLpy-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SHACL2SPARQLpy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python reference implementation of SHACL2SPARQL
 Home-page: https://github.com/SDM-TIB/SHACL2SPARQLpy
-Download-URL: https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.1.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.3.0.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SHACL2SPARQLpy-1.2.0/README.md` & `SHACL2SPARQLpy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/DependencyGraphImpl.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/DependencyGraphImpl.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Eval.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/Eval.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/RuleBasedValidation.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/RuleBasedValidation.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Shape.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/Shape.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeNetwork.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/ShapeNetwork.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeParser.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/ShapeParser.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,20 +112,20 @@
                 for res in g_file.query(queries[2].format(shape=name)):
                     target_def = str(res[0])
                     target_type = 'node'
                     break
 
             target_query = None
             if target_def is not None and target_type == 'class':
+                if urlparse(target_def).netloc != '':  # if the target node is a url, add '<>' to it
+                    target_def = '<' + target_def + '>'
                 for res in g_file.query(QUERY_TARGET_QUERY.format(shape=name)):
                     target_query = str(res[0])
                 if target_query is None:
-                    target_query = 'SELECT ?x WHERE { ?x a <' + target_def + '> }'  # come up with a query for this
-                    if urlparse(target_def).netloc != '':  # if the target node is a url, add '<>' to it
-                        target_def = '<' + target_def + '>'
+                    target_query = 'SELECT ?x WHERE { ?x a ' + target_def + ' }'  # come up with a query for this
 
             cons_dict = self.parse_all_const(g_file, name=name, target_def=target_def,
                                              target_type=target_type, query=queries)
 
             const_array = list(cons_dict.values())  # change the format to an array
             constraints = self.parse_constraints_ttl(const_array, target_def, id_)
 
@@ -186,16 +186,24 @@
         QUERY_CONSTRAINTS = '''SELECT ?constraint WHERE {{
               <{shape}> a <http://www.w3.org/ns/shacl#NodeShape> .
               <{shape}> <http://www.w3.org/ns/shacl#property> ?constraint .
             }}
             '''
 
         QUERY_CONSTRAINT_DETAILS = '''SELECT ?p ?o WHERE {{
-              ?s ?p ?o .
-              FILTER( str(?s) = "{constraint}" )
+                {{
+                    ?s ?p ?o .
+                    FILTER( str(?s) = "{constraint}" )
+                    FILTER( ?p != <http://www.w3.org/ns/shacl#path> || !isBlank(?o) )
+                }} UNION {{
+                    ?s <http://www.w3.org/ns/shacl#path>/<http://www.w3.org/ns/shacl#inversePath> ?o .
+                    BIND(<http://www.w3.org/ns/shacl#path> AS ?p)
+                    BIND(CONCAT('^', str(?o)) AS ?o)
+                    FILTER( str(?s) = "{constraint}" )
+                }}
             }}'''
 
         QUERY_QVS_REF_1 = '''SELECT ?shape_ref WHERE {{
                   ?s <http://www.w3.org/ns/shacl#node> ?shape_ref .
                   FILTER ( str(?s) = "{qvs}" )
                 }}'''
 
@@ -309,24 +317,32 @@
         max = obj.get("max")
         shapeRef = obj.get("shape")
         datatype = obj.get("datatype")
         value = obj.get("value")
         path = obj.get("path")
         negated = obj.get("negated")
 
+        if path is not None and str(path).startswith('^'):
+            is_inverse_path = True
+            path = str(path)[1:]
+        else:
+            is_inverse_path = False
+
         oMin = None if (min is None) else int(min)
         oMax = None if (max is None) else int(max)
         oShapeRef = None if (shapeRef is None) else str(shapeRef)
         oDatatype = None if (datatype is None) else str(datatype)
         oValue = None if (value is None) else str(value)
         oPath = None if (path is None) else str(path)
         oNeg = True if (negated is None) else not negated  # True means it is a positive constraint
 
         if path is not None and urlparse(path).netloc != '':  # if the predicate is a URL, add '<>' to it
             oPath = '<' + path + '>'
+        if is_inverse_path:
+            oPath = '^' + oPath
 
         if shapeRef is not None and urlparse(shapeRef).netloc != '':  # if the shape reference is a URL, add '<>' to it
             oShapeRef = '<' + shapeRef + '>'
 
         if value is not None and urlparse(value).netloc != '':  # if the value reference is a URL, add '<>' to it
             oValue = '<' + value + '>'
```

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/VariableGenerator.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/Constraint.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinMaxConstraint.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/MinMaxConstraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/Literal.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/Literal.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RuleMap.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/RuleMap.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RulePattern.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/QueryGenerator.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/sparql/QueryGenerator.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/RuleBasedValidStats.py` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy/utils/RuleBasedValidStats.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/PKG-INFO` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SHACL2SPARQLpy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python reference implementation of SHACL2SPARQL
 Home-page: https://github.com/SDM-TIB/SHACL2SPARQLpy
-Download-URL: https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.1.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.3.0.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/SOURCES.txt` & `SHACL2SPARQLpy-1.3.0/SHACL2SPARQLpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.2.0/setup.py` & `SHACL2SPARQLpy-1.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+VERSION = '1.3.0'
+
 setup(
     name='SHACL2SPARQLpy',
-    version='1.2.0',
+    version=VERSION,
     packages=['SHACL2SPARQLpy', 'SHACL2SPARQLpy.constraints', 'SHACL2SPARQLpy.core', 'SHACL2SPARQLpy.sparql', 'SHACL2SPARQLpy.utils'],
     license='MIT',
     author='Mónica Figuera, Philipp D. Rohde',
     author_email='philipp.rohde@tib.eu',
     url='https://github.com/SDM-TIB/SHACL2SPARQLpy',
-    download_url='https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.1.0.tar.gz',
+    download_url='https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v' + VERSION + '.tar.gz',
     description='Python reference implementation of SHACL2SPARQL',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['SPARQLWrapper>=1.8.5', 'rdflib>=6.0.0'],
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 4 - Beta',
```

