# Comparing `tmp/django_postgresql_reconnect-1.0.3.tar.gz` & `tmp/django_postgresql_reconnect-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_postgresql_reconnect-1.0.3.tar", max compression
+gzip compressed data, was "django_postgresql_reconnect-1.0.4.tar", max compression
```

## Comparing `django_postgresql_reconnect-1.0.3.tar` & `django_postgresql_reconnect-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      479 2023-01-19 15:10:00.118461 django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 15:10:00.118461 django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/backend/__init__.py
--rw-r--r--   0        0        0     1364 2023-01-19 15:10:00.118461 django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/backend/base.py
--rw-r--r--   0        0        0      536 2023-01-19 15:10:00.118461 django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/decorator.py
--rw-r--r--   0        0        0      433 2023-01-19 15:10:00.118461 django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/helpers.py
--rw-r--r--   0        0        0      332 2023-01-19 15:10:00.118461 django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/middleware.py
--rw-r--r--   0        0        0     1468 2023-01-19 15:10:50.774822 django_postgresql_reconnect-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 django_postgresql_reconnect-1.0.3/setup.py
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 django_postgresql_reconnect-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      479 2023-07-14 15:47:49.969271 django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:47:49.969271 django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/backend/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-14 15:47:49.969271 django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/backend/base.py
+-rw-r--r--   0        0        0      536 2023-07-14 15:47:49.969271 django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/decorator.py
+-rw-r--r--   0        0        0      433 2023-07-14 15:47:49.969271 django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/helpers.py
+-rw-r--r--   0        0        0      332 2023-07-14 15:47:49.969271 django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/middleware.py
+-rw-r--r--   0        0        0     1472 2023-07-14 15:48:33.681758 django_postgresql_reconnect-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 django_postgresql_reconnect-1.0.4/PKG-INFO
```

### Comparing `django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/backend/base.py` & `django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/backend/base.py`

 * *Files identical despite different names*

### Comparing `django_postgresql_reconnect-1.0.3/django_postgresql_reconnect/decorator.py` & `django_postgresql_reconnect-1.0.4/django_postgresql_reconnect/decorator.py`

 * *Files identical despite different names*

### Comparing `django_postgresql_reconnect-1.0.3/pyproject.toml` & `django_postgresql_reconnect-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "django-postgresql-reconnect"
 homepage = "https://github.com/cloudblue/django-postgresql-reconnect"
 repository = "https://github.com/cloudblue/django-postgresql-reconnect"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = ["CloudBlue LLC"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: Unix",
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Django = "^3.2"
+Django = ">=3.2,<5"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.*"
 pytest-cov = "3.*"
 pytest-factoryboy = "2.*"
 pytest-mock = "3.*"
 flake8 = "4.*"
```

### Comparing `django_postgresql_reconnect-1.0.3/PKG-INFO` & `django_postgresql_reconnect-1.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: django-postgresql-reconnect
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Home-page: https://github.com/cloudblue/django-postgresql-reconnect
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
-Requires-Dist: Django (>=3.2,<4.0)
+Requires-Dist: Django (>=3.2,<5)
 Project-URL: Repository, https://github.com/cloudblue/django-postgresql-reconnect
```

