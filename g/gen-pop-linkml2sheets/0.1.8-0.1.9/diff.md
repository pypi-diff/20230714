# Comparing `tmp/gen_pop_linkml2sheets-0.1.8.tar.gz` & `tmp/gen_pop_linkml2sheets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_pop_linkml2sheets-0.1.8.tar", max compression
+gzip compressed data, was "gen_pop_linkml2sheets-0.1.9.tar", max compression
```

## Comparing `gen_pop_linkml2sheets-0.1.8.tar` & `gen_pop_linkml2sheets-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.8/README.md
--rw-r--r--   0        0        0     2426 2023-05-12 19:49:55.298273 gen_pop_linkml2sheets-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      111 2023-05-10 17:53:28.805534 gen_pop_linkml2sheets-0.1.8/src/gen_pop_linkml2sheets/__init__.py
--rw-r--r--   0        0        0     6990 2023-05-12 19:15:11.113218 gen_pop_linkml2sheets-0.1.8/src/gen_pop_linkml2sheets/generate_and_populate_template.py
--rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-13 13:26:50.433695 gen_pop_linkml2sheets-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     4403 2023-07-13 13:26:50.433695 gen_pop_linkml2sheets-0.1.9/README.md
+-rw-r--r--   0        0        0     2521 2023-07-14 14:18:01.234314 gen_pop_linkml2sheets-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-13 13:26:50.433695 gen_pop_linkml2sheets-0.1.9/src/gen_pop_linkml2sheets/__init__.py
+-rw-r--r--   0        0        0     7024 2023-07-13 13:35:06.828544 gen_pop_linkml2sheets-0.1.9/src/gen_pop_linkml2sheets/generate_and_populate_template.py
+-rw-r--r--   0        0        0     5121 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.9/PKG-INFO
```

### Comparing `gen_pop_linkml2sheets-0.1.8/LICENSE.md` & `gen_pop_linkml2sheets-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.8/README.md` & `gen_pop_linkml2sheets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.8/pyproject.toml` & `gen_pop_linkml2sheets-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "gen-pop-linkml2sheets"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Mark Andrew Miller <MAM@lbl.gov>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/turbomam/gen-pop-linkml2sheets"
 repository = "https://github.com/turbomam/gen-pop-linkml2sheets"
 packages = [{ include = "gen_pop_linkml2sheets", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 linkml = "^1.5.2"
-pandas = "^1.3.4"
-schemasheets = "^0.1.21"
+#pandas = "^1.3.4"
+pandas = "^2.0"
+schemasheets = "^0.1.22"
+#schemasheets = { path = "/home/mark/gitrepos/schemasheets", develop = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-sugar = "^0.9.5"
 pytest-clarity = "^1.0.1"
 pytest-random-order = "^1.0.4"
 coverage = { extras = ["toml"], version = "^6.4.4" }
```

### Comparing `gen_pop_linkml2sheets-0.1.8/src/gen_pop_linkml2sheets/generate_and_populate_template.py` & `gen_pop_linkml2sheets-0.1.9/src/gen_pop_linkml2sheets/generate_and_populate_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
                   "prefix_prefix",
                   "pv_formula",
                   "range_expression",
                   "reachable_from",
                   "structured_aliases",
                   "text",
                   "unit",
+                  "instantiates",
               ],
               help='What LinkML meta slots from the base class should be added to the report?')
 @click.option('--columns-to-use',
               multiple=True,
               help='Overrides any other determinant of which columns to use in the report.')
 @click.option('--source-schema-path',
               required=True,
```

### Comparing `gen_pop_linkml2sheets-0.1.8/PKG-INFO` & `gen_pop_linkml2sheets-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gen-pop-linkml2sheets
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/turbomam/gen-pop-linkml2sheets
 License: MIT
 Author: Mark Andrew Miller
 Author-email: MAM@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: linkml (>=1.5.2,<2.0.0)
-Requires-Dist: pandas (>=1.3.4,<2.0.0)
-Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: schemasheets (>=0.1.22,<0.2.0)
 Project-URL: Repository, https://github.com/turbomam/gen-pop-linkml2sheets
 Description-Content-Type: text/markdown
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.8 Summary: Home-
+Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.9 Summary: Home-
 page: https://github.com/turbomam/gen-pop-linkml2sheets License: MIT Author:
 Mark Andrew Miller Author-email: MAM@lbl.gov Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: linkml (>=1.5.2,<2.0.0) Requires-
-Dist: pandas (>=1.3.4,<2.0.0) Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
+Dist: pandas (>=2.0,<3.0) Requires-Dist: schemasheets (>=0.1.22,<0.2.0)
 Project-URL: Repository, https://github.com/turbomam/gen-pop-linkml2sheets
 Description-Content-Type: text/markdown
 ****** Single step population of linkml2sheets usage reports, with useful
 columns only ******
 Single step population of linkml2sheets usage reports, with useful columns only
  Repo | Report_Bug | Releases
```

