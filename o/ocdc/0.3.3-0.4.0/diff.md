# Comparing `tmp/ocdc-0.3.3.tar.gz` & `tmp/ocdc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdc-0.3.3.tar", max compression
+gzip compressed data, was "ocdc-0.4.0.tar", max compression
```

## Comparing `ocdc-0.3.3.tar` & `ocdc-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1077 2022-05-20 21:07:15.950349 ocdc-0.3.3/LICENSE
--rw-r--r--   0        0        0     1262 2022-08-02 08:05:27.288802 ocdc-0.3.3/README.md
--rw-r--r--   0        0        0       22 2022-08-10 14:47:16.571371 ocdc-0.3.3/ocdc/__init__.py
--rw-r--r--   0        0        0     2324 2022-08-02 17:24:11.240543 ocdc-0.3.3/ocdc/__main__.py
--rw-r--r--   0        0        0      186 2022-07-31 19:26:27.068081 ocdc-0.3.3/ocdc/api.py
--rw-r--r--   0        0        0      801 2022-08-10 14:47:16.571692 ocdc-0.3.3/ocdc/ast.py
--rw-r--r--   0        0        0     8128 2022-08-07 20:16:56.312858 ocdc-0.3.3/ocdc/parser.py
--rw-r--r--   0        0        0     2256 2022-08-06 14:49:48.755515 ocdc-0.3.3/ocdc/renderer.py
--rw-r--r--   0        0        0      741 2022-08-10 14:47:16.572016 ocdc-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2126 2022-08-10 14:47:27.516913 ocdc-0.3.3/setup.py
--rw-r--r--   0        0        0     2047 2022-08-10 14:47:27.517062 ocdc-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-05-20 21:07:15.950349 ocdc-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1262 2023-07-13 19:56:17.482658 ocdc-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-13 22:37:30.829234 ocdc-0.4.0/ocdc/__init__.py
+-rw-r--r--   0        0        0     2332 2023-07-13 22:37:30.829392 ocdc-0.4.0/ocdc/__main__.py
+-rw-r--r--   0        0        0      186 2022-07-31 19:26:27.068081 ocdc-0.4.0/ocdc/api.py
+-rw-r--r--   0        0        0      801 2022-08-10 14:47:16.571692 ocdc-0.4.0/ocdc/ast.py
+-rw-r--r--   0        0        0     8128 2023-07-13 19:29:45.677136 ocdc-0.4.0/ocdc/parser.py
+-rw-r--r--   0        0        0     2256 2022-08-06 14:49:48.755515 ocdc-0.4.0/ocdc/renderer.py
+-rw-r--r--   0        0        0      741 2023-07-13 22:37:30.829830 ocdc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 ocdc-0.4.0/PKG-INFO
```

### Comparing `ocdc-0.3.3/LICENSE` & `ocdc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdc-0.3.3/README.md` & `ocdc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ocdc-0.3.3/ocdc/__main__.py` & `ocdc-0.4.0/ocdc/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     else:
         path = _full_path(args.path)
         orig = path.read_text()
 
     result = api.format(orig)
 
     if is_stdin:
-        print(result)
+        print(result, end="")
     elif result != orig:
         if args.check:
             sys.exit(f"ERROR: {path} would be reformatted")
         else:
             path.write_text(result)
             print(f"{path} was reformatted")
     else:
```

### Comparing `ocdc-0.3.3/ocdc/ast.py` & `ocdc-0.4.0/ocdc/ast.py`

 * *Files identical despite different names*

### Comparing `ocdc-0.3.3/ocdc/parser.py` & `ocdc-0.4.0/ocdc/parser.py`

 * *Files identical despite different names*

### Comparing `ocdc-0.3.3/ocdc/renderer.py` & `ocdc-0.4.0/ocdc/renderer.py`

 * *Files identical despite different names*

### Comparing `ocdc-0.3.3/pyproject.toml` & `ocdc-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "ocdc"
-version = "0.3.3"
+version = "0.4.0"
 description = 'A changelog formatter for "people", neat freaks, and sloppy typists.'
 authors = ["Matteo De Wint <matteo@mailfence.com>"]
 packages = [{ include = "ocdc" }]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mdwint/ocdc"
 keywords = ["changelog", "markdown", "formatter"]
 
 [tool.poetry.scripts]
 ocdc = "ocdc.__main__:main"
 
 [tool.poetry.dependencies]
-packaging = "^21.3"
-pydantic = "^1.9.1"
-python = "^3.7"
+packaging = "^23.1"
+pydantic = "^2.0.2"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^22.6.0"
+black = "^23.7.0"
 bump2version = "^1.0.1"
-coverage = "^6.4.2"
-flake8 = "^5.0.0"
-isort = "^5.10.1"
-mypy = "^0.971"
-pytest = "^7.1.2"
+coverage = "^7.2.7"
+flake8 = "^5.0.4"
+isort = "^5.12.0"
+mypy = "^1.4.1"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ocdc-0.3.3/PKG-INFO` & `ocdc-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ocdc
-Version: 0.3.3
+Version: 0.4.0
 Summary: A changelog formatter for "people", neat freaks, and sloppy typists.
 Home-page: https://github.com/mdwint/ocdc
 License: MIT
 Keywords: changelog,markdown,formatter
 Author: Matteo De Wint
 Author-email: matteo@mailfence.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Project-URL: Repository, https://github.com/mdwint/ocdc
 Description-Content-Type: text/markdown
 
 ![OCDC Logo](/logo.png)
 
 <h2 align="center">Obsessive-Compulsive Development Changelogs</h2>
```

