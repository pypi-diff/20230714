# Comparing `tmp/django_url_security-0.0.1.tar.gz` & `tmp/django_url_security-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_url_security-0.0.1.tar", max compression
+gzip compressed data, was "django_url_security-0.0.2.tar", max compression
```

## Comparing `django_url_security-0.0.1.tar` & `django_url_security-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-07-14 03:47:48.173915 django_url_security-0.0.1/LICENSE
--rw-r--r--   0        0        0      910 2023-07-14 03:47:48.173915 django_url_security-0.0.1/README.md
--rw-r--r--   0        0        0      404 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/__init__.py
--rw-r--r--   0        0        0     7029 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/core.py
--rw-r--r--   0        0        0       19 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/django_url_security.py
--rw-r--r--   0        0        0     1969 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/generate_permission_spec_file.py
--rw-r--r--   0        0        0      484 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/management/commands/export_url_security_file.py
--rw-r--r--   0        0        0        0 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/py.typed
--rw-r--r--   0        0        0    11713 2023-07-14 03:47:48.173915 django_url_security-0.0.1/django_url_security/url_security.py
--rw-r--r--   0        0        0     3182 2023-07-14 03:48:03.046019 django_url_security-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 django_url_security-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 05:15:57.338114 django_url_security-0.0.2/LICENSE
+-rw-r--r--   0        0        0      910 2023-07-14 05:15:57.338114 django_url_security-0.0.2/README.md
+-rw-r--r--   0        0        0      404 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/__init__.py
+-rw-r--r--   0        0        0     7029 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/core.py
+-rw-r--r--   0        0        0       19 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/django_url_security.py
+-rw-r--r--   0        0        0     1969 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/generate_permission_spec_file.py
+-rw-r--r--   0        0        0      484 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/management/commands/export_url_security_file.py
+-rw-r--r--   0        0        0        0 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/py.typed
+-rw-r--r--   0        0        0    11713 2023-07-14 05:15:57.338114 django_url_security-0.0.2/django_url_security/url_security.py
+-rw-r--r--   0        0        0     3182 2023-07-14 05:16:09.566638 django_url_security-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 django_url_security-0.0.2/PKG-INFO
```

### Comparing `django_url_security-0.0.1/LICENSE` & `django_url_security-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_url_security-0.0.1/README.md` & `django_url_security-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_url_security-0.0.1/django_url_security/core.py` & `django_url_security-0.0.2/django_url_security/core.py`

 * *Files identical despite different names*

### Comparing `django_url_security-0.0.1/django_url_security/generate_permission_spec_file.py` & `django_url_security-0.0.2/django_url_security/generate_permission_spec_file.py`

 * *Files identical despite different names*

### Comparing `django_url_security-0.0.1/django_url_security/url_security.py` & `django_url_security-0.0.2/django_url_security/url_security.py`

 * *Files identical despite different names*

### Comparing `django_url_security-0.0.1/pyproject.toml` & `django_url_security-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 
 [tool.poetry]
 name = "django_url_security"
-version = "v0.0.1"
+version = "v0.0.2"
 homepage = "https://github.com/Edrolo/django-url-security"
 description = "Django URL Security provides tests to ensure all the private endpoints in your Django project are private."
 authors = ["Matt Fisher <m@ttfisher.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'License :: OSI Approved :: MIT License',
@@ -18,18 +18,18 @@
 ]
 include = [
     "LICENSE",
     "django_url_security/py.typed"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-importlib_metadata = "^3.4.0"
-django = "^3.2"
-parameterized = "^0.9.0"
+python = ">=3.8"
+importlib_metadata = ">=3.4"
+django = ">=3.2"
+parameterized = ">=0.9"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^6.1.5"
 pytest = "^7.0"
 pytest-cov = "^4.1.0"
 pylint = "^2.17.0"
 mypy = "1.4.1"
```

### Comparing `django_url_security-0.0.1/PKG-INFO` & `django_url_security-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: django-url-security
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django URL Security provides tests to ensure all the private endpoints in your Django project are private.
 Home-page: https://github.com/Edrolo/django-url-security
 License: MIT
 Author: Matt Fisher
 Author-email: m@ttfisher.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.2,<4.0)
-Requires-Dist: importlib_metadata (>=3.4.0,<4.0.0)
-Requires-Dist: parameterized (>=0.9.0,<0.10.0)
+Requires-Dist: django (>=3.2)
+Requires-Dist: importlib_metadata (>=3.4)
+Requires-Dist: parameterized (>=0.9)
 Description-Content-Type: text/markdown
 
 # Django URL Security
 
 
 [![PyPI version](https://badge.fury.io/py/django-url-security.svg)](https://badge.fury.io/py/django-url-security)
 ![versions](https://img.shields.io/pypi/pyversions/django-url-security.svg)
```

