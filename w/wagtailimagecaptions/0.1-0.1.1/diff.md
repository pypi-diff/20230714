# Comparing `tmp/wagtailimagecaptions-0.1.tar.gz` & `tmp/wagtailimagecaptions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailimagecaptions-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtailimagecaptions-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtailimagecaptions-0.1.tar` & `wagtailimagecaptions-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1/LICENSE
--rw-r--r--   0        0        0     1130 2023-07-13 20:31:47.103676 wagtailimagecaptions-0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1/media/.gitkeep
--rw-r--r--   0        0        0     1178 2023-07-13 18:37:25.131714 wagtailimagecaptions-0.1/pyproject.toml
--rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1/setup.cfg
--rw-r--r--   0        0        0      162 2023-07-13 11:31:58.111652 wagtailimagecaptions-0.1/src/wagtailimagecaptions/__init__.py
--rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1/src/wagtailimagecaptions/apps.py
--rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1/src/wagtailimagecaptions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1/src/wagtailimagecaptions/migrations/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1/src/wagtailimagecaptions/models.py
--rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1/src/wagtailimagecaptions/services.py
--rw-r--r--   0        0        0     1187 2023-07-13 20:58:55.147909 wagtailimagecaptions-0.1/src/wagtailimagecaptions/signals.py
--rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1/test_project/__init__.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1/test_project/asgi.py
--rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1/test_project/settings.py
--rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1/test_project/urls.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1/test_project/wsgi.py
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1130 2023-07-13 20:31:47.103676 wagtailimagecaptions-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.1/media/.gitkeep
+-rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.1/setup.cfg
+-rw-r--r--   0        0        0      164 2023-07-14 11:31:12.202787 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/apps.py
+-rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/migrations/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/models.py
+-rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/services.py
+-rw-r--r--   0        0        0     1187 2023-07-13 20:58:55.147909 wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/signals.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.1/test_project/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.1/test_project/asgi.py
+-rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.1/test_project/settings.py
+-rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.1/test_project/urls.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.1/test_project/wsgi.py
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.1/PKG-INFO
```

### Comparing `wagtailimagecaptions-0.1/LICENSE` & `wagtailimagecaptions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/README.md` & `wagtailimagecaptions-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/pyproject.toml` & `wagtailimagecaptions-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "wagtailimagecaptions"
-authors = [{name = "Stephan Rohde", email = "srohde@newshour.org"}]
+authors = [{name = "Stephan Rohde", email = "appsupport@newshour.org"}]
 license = {file = "LICENSE"}
+readme = "README.md"
 dynamic = ["version", "description"]
 classifiers = [
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `wagtailimagecaptions-0.1/setup.cfg` & `wagtailimagecaptions-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/src/wagtailimagecaptions/migrations/0001_initial.py` & `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/src/wagtailimagecaptions/models.py` & `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/models.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/src/wagtailimagecaptions/services.py` & `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/services.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/src/wagtailimagecaptions/signals.py` & `wagtailimagecaptions-0.1.1/src/wagtailimagecaptions/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/test_project/settings.py` & `wagtailimagecaptions-0.1.1/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1/test_project/urls.py` & `wagtailimagecaptions-0.1.1/test_project/urls.py`

 * *Files identical despite different names*

