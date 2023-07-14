# Comparing `tmp/django_federation_auditlog-1.0.0.tar.gz` & `tmp/django_federation_auditlog-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_federation_auditlog-1.0.0.tar", max compression
+gzip compressed data, was "django_federation_auditlog-1.1.0.tar", max compression
```

## Comparing `django_federation_auditlog-1.0.0.tar` & `django_federation_auditlog-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2664 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/README.md
--rw-r--r--   0        0        0       22 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/__init__.py
--rw-r--r--   0        0        0      799 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/admin.py
--rw-r--r--   0        0        0      127 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/apps.py
--rw-r--r--   0        0        0     5513 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/diff.py
--rw-r--r--   0        0        0     4175 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/middleware.py
--rw-r--r--   0        0        0     3146 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/migrations/__init__.py
--rw-r--r--   0        0        0     2373 2023-07-13 19:46:19.730240 django_federation_auditlog-1.0.0/django_federation_auditlog/mixins.py
--rw-r--r--   0        0        0    14788 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/models.py
--rw-r--r--   0        0        0     2084 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/receivers.py
--rw-r--r--   0        0        0     4720 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/registry.py
--rw-r--r--   0        0        0       60 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/django_federation_auditlog/tests.py
--rw-r--r--   0        0        0      739 2023-07-13 19:46:19.734241 django_federation_auditlog-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3326 1970-01-01 00:00:00.000000 django_federation_auditlog-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2664 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/__init__.py
+-rw-r--r--   0        0        0      799 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/admin.py
+-rw-r--r--   0        0        0      127 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/apps.py
+-rw-r--r--   0        0        0     5513 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/diff.py
+-rw-r--r--   0        0        0     4175 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/middleware.py
+-rw-r--r--   0        0        0     3146 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0     2373 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/mixins.py
+-rw-r--r--   0        0        0    14788 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/models.py
+-rw-r--r--   0        0        0     2084 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/receivers.py
+-rw-r--r--   0        0        0     4720 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/registry.py
+-rw-r--r--   0        0        0       60 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/django_federation_auditlog/tests.py
+-rw-r--r--   0        0        0      736 2023-07-14 12:20:41.113984 django_federation_auditlog-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 django_federation_auditlog-1.1.0/PKG-INFO
```

### Comparing `django_federation_auditlog-1.0.0/README.md` & `django_federation_auditlog-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/admin.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/diff.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/middleware.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/migrations/0001_initial.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/mixins.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/models.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/receivers.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/receivers.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/django_federation_auditlog/registry.py` & `django_federation_auditlog-1.1.0/django_federation_auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django_federation_auditlog-1.0.0/pyproject.toml` & `django_federation_auditlog-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "django-federation-auditlog"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["Anderson Marques <anderson89marques@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 djangorestframework = "^3.11"
-djangorestframework-simplejwt = "==5.0.0"
+djangorestframework-simplejwt = "^5.2"
 django-auditlog = "==2.0.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8b1"
 flake8 = "^3.8.3"
```

### Comparing `django_federation_auditlog-1.0.0/PKG-INFO` & `django_federation_auditlog-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-federation-auditlog
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Author: Anderson Marques
 Author-email: anderson89marques@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-auditlog (==2.0.0)
 Requires-Dist: djangorestframework (>=3.11,<4.0)
-Requires-Dist: djangorestframework-simplejwt (==5.0.0)
+Requires-Dist: djangorestframework-simplejwt (>=5.2,<6.0)
 Description-Content-Type: text/markdown
 
 # Django Auditlog
 This project is totally based in [Django Auditlog](https://github.com/jazzband/django-auditlog/tree/master) library.
 
 # Instalation
```

