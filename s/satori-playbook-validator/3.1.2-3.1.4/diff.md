# Comparing `tmp/satori_playbook_validator-3.1.2.tar.gz` & `tmp/satori_playbook_validator-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-3.1.2.tar", last modified: Thu Jul 13 21:03:23 2023, max compression
+gzip compressed data, was "satori_playbook_validator-3.1.4.tar", last modified: Fri Jul 14 18:45:45 2023, max compression
```

## Comparing `satori_playbook_validator-3.1.2.tar` & `satori_playbook_validator-3.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       30 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/README.md
--rw-r--r--   0        0        0      518 2023-07-13 21:03:23.111551 satori_playbook_validator-3.1.2/pyproject.toml
--rw-r--r--   0        0        0      301 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     6168 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      298 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1906 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     2361 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      100 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/src/satorici/validator/warnings.py
--rw-r--r--   0        0        0     2659 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-07-13 21:03:08.359171 satori_playbook_validator-3.1.2/tests/test_reference_finder.py
--rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/README.md
+-rw-r--r--   0        0        0      518 2023-07-14 18:45:45.158146 satori_playbook_validator-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     6168 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      298 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1906 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     2361 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      100 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/src/satorici/validator/warnings.py
+-rw-r--r--   0        0        0     2659 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-07-14 18:45:26.909091 satori_playbook_validator-3.1.4/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      311 1970-01-01 00:00:00.000000 satori_playbook_validator-3.1.4/PKG-INFO
```

### Comparing `satori_playbook_validator-3.1.2/pyproject.toml` & `satori_playbook_validator-3.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "satori-playbook-validator"
-version = "3.1.2"
+version = "3.1.4"
 description = ""
 authors = [
     { name = "Satori CI", email = "info@satori-ci.com" },
 ]
 dependencies = [
     "fastjsonschema>=2.17.1",
     "aws-cron-expression-validator>=1.1.6",
```

### Comparing `satori_playbook_validator-3.1.2/src/satorici/validator/_validator.py` & `satori_playbook_validator-3.1.4/src/satorici/validator/_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.2/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-3.1.4/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.2/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-3.1.4/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.2/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-3.1.4/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.2/tests/test_playbook_validator.py` & `satori_playbook_validator-3.1.4/tests/test_playbook_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-3.1.2/tests/test_reference_finder.py` & `satori_playbook_validator-3.1.4/tests/test_reference_finder.py`

 * *Files identical despite different names*

