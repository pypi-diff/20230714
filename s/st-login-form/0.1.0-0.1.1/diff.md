# Comparing `tmp/st-login-form-0.1.0.tar.gz` & `tmp/st-login-form-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-login-form-0.1.0.tar", last modified: Fri Jul 14 11:22:49 2023, max compression
+gzip compressed data, was "st-login-form-0.1.1.tar", last modified: Fri Jul 14 11:40:18 2023, max compression
```

## Comparing `st-login-form-0.1.0.tar` & `st-login-form-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:22:49.395494 st-login-form-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-14 11:22:38.000000 st-login-form-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 11:22:38.000000 st-login-form-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 11:22:49.395494 st-login-form-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-14 11:22:38.000000 st-login-form-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:22:49.395494 st-login-form-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 11:22:38.000000 st-login-form-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:22:49.391494 st-login-form-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:22:49.395494 st-login-form-0.1.0/src/st_login_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 11:22:49.000000 st-login-form-0.1.0/src/st_login_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-14 11:22:49.000000 st-login-form-0.1.0/src/st_login_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:22:49.000000 st-login-form-0.1.0/src/st_login_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 11:22:49.000000 st-login-form-0.1.0/src/st_login_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 11:22:49.000000 st-login-form-0.1.0/src/st_login_form.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:22:49.395494 st-login-form-0.1.0/src/streamlit_login/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-14 11:22:38.000000 st-login-form-0.1.0/src/streamlit_login/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-14 11:40:10.000000 st-login-form-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 11:40:10.000000 st-login-form-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 11:40:18.807236 st-login-form-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-14 11:40:10.000000 st-login-form-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:40:18.807236 st-login-form-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 11:40:10.000000 st-login-form-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/src/st_login_form/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-14 11:40:10.000000 st-login-form-0.1.1/src/st_login_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/src/st_login_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/top_level.txt
```

### Comparing `st-login-form-0.1.0/LICENSE` & `st-login-form-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st-login-form-0.1.0/PKG-INFO` & `st-login-form-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.1.0
+Version: 0.1.1
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `st-login-form-0.1.0/README.md` & `st-login-form-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `st-login-form-0.1.0/setup.py` & `st-login-form-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-login-form",
-    version="0.1.0",
+    version="0.1.1",
     author="Siddhant Sadangi",
     author_email="siddhant.sadangi@gmail.com",
     description="A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `st-login-form-0.1.0/src/st_login_form.egg-info/PKG-INFO` & `st-login-form-0.1.1/src/st_login_form.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.1.0
+Version: 0.1.1
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `st-login-form-0.1.0/src/streamlit_login/__init__.py` & `st-login-form-0.1.1/src/st_login_form/__init__.py`

 * *Files identical despite different names*

