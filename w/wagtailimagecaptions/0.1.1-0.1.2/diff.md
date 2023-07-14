# Comparing `tmp/wagtailimagecaptions-0.1.1.tar.gz` & `tmp/wagtailimagecaptions-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailimagecaptions-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtailimagecaptions-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtailimagecaptions-0.1.1.tar` & `wagtailimagecaptions-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.1/LICENSE
--rw-r--r--   0        0        0     1130 2023-07-13 20:31:47.103676 wagtailimagecaptions-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.1/media/.gitkeep
--rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.1/setup.cfg
--rw-r--r--   0        0        0      164 2023-07-14 11:31:12.202787 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/__init__.py
--rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/apps.py
--rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/migrations/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/models.py
--rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/services.py
--rw-r--r--   0        0        0     1187 2023-07-13 20:58:55.147909 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/signals.py
--rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.1/test_project/__init__.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.1/test_project/asgi.py
--rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.1/test_project/settings.py
--rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.1/test_project/urls.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.1/test_project/wsgi.py
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1202 2023-07-14 11:53:40.061369 wagtailimagecaptions-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.2/media/.gitkeep
+-rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.2/setup.cfg
+-rw-r--r--   0        0        0      164 2023-07-14 11:59:35.930790 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/apps.py
+-rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/migrations/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/models.py
+-rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/services.py
+-rw-r--r--   0        0        0     1187 2023-07-13 20:58:55.147909 wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/signals.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.2/test_project/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.2/test_project/asgi.py
+-rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.2/test_project/settings.py
+-rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.2/test_project/urls.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.2/test_project/wsgi.py
+-rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.2/PKG-INFO
```

### Comparing `wagtailimagecaptions-0.1.1/LICENSE` & `wagtailimagecaptions-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/README.md` & `wagtailimagecaptions-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 A Django app for extending the Wagtail Image model to add captions and alt fields as
 well as the extraction of IPTC image meta data.
 
 ![screenshot](https://github.com/newshour/wagtailimagecaptions/assets/14984514/278f5d01-7f2e-48a8-98fd-aaaa6c2d6b8c)
 
 ## Installing
 
+Install using pip:
+
+```sh
+pip install wagtailimagecaptions
+```
+
 ### Settings
 
-In your settings file, add `wagtailmedia` to `INSTALLED_APPS`:
+In your settings file, add `wagtailimagecaptions` to `INSTALLED_APPS`:
 
 ```python
 INSTALLED_APPS = [
     # ...
     "wagtailimagecaptions",
     # ...
 ]
```

### Comparing `wagtailimagecaptions-0.1.1/pyproject.toml` & `wagtailimagecaptions-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/setup.cfg` & `wagtailimagecaptions-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/migrations/0001_initial.py` & `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/models.py` & `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/models.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/services.py` & `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/services.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/signals.py` & `wagtailimagecaptions-0.1.2/src/wagtailimagecaptions/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/test_project/settings.py` & `wagtailimagecaptions-0.1.2/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/test_project/urls.py` & `wagtailimagecaptions-0.1.2/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.1/PKG-INFO` & `wagtailimagecaptions-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailimagecaptions
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django app for extending the Wagtail Image model to add captions and alt fields as
 Author-email: Stephan Rohde <appsupport@newshour.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,17 +23,23 @@
 A Django app for extending the Wagtail Image model to add captions and alt fields as
 well as the extraction of IPTC image meta data.
 
 ![screenshot](https://github.com/newshour/wagtailimagecaptions/assets/14984514/278f5d01-7f2e-48a8-98fd-aaaa6c2d6b8c)
 
 ## Installing
 
+Install using pip:
+
+```sh
+pip install wagtailimagecaptions
+```
+
 ### Settings
 
-In your settings file, add `wagtailmedia` to `INSTALLED_APPS`:
+In your settings file, add `wagtailimagecaptions` to `INSTALLED_APPS`:
 
 ```python
 INSTALLED_APPS = [
     # ...
     "wagtailimagecaptions",
     # ...
 ]
```

