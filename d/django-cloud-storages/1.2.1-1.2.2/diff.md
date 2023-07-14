# Comparing `tmp/django_cloud_storages-1.2.1.tar.gz` & `tmp/django_cloud_storages-1.2.2.tar.gz`

## Comparing `django_cloud_storages-1.2.1.tar` & `django_cloud_storages-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/cloud_storages/__init__.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/README.md
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/README.md
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 django_cloud_storages-1.2.2/PKG-INFO
```

### Comparing `django_cloud_storages-1.2.1/.readthedocs.yaml` & `django_cloud_storages-1.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/cloud_storages/utils.py` & `django_cloud_storages-1.2.2/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.2.2/cloud_storages/backends/appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.2.2/cloud_storages/backends/dropbox.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/.gitignore` & `django_cloud_storages-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/LICENSE` & `django_cloud_storages-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/README.md` & `django_cloud_storages-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.2.1/pyproject.toml` & `django_cloud_storages-1.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project.optional-dependencies]
 required = ["django", "requests"]
-dropbox = ["django-cloud-storages[required]", "dropbox"]
-appwrite = ["django-cloud-storages[required]", "appwrite"]
+dropbox = ["django-cloud-storages[required]", "dropbox>=11.36.2"]
+appwrite = ["django-cloud-storages[required]", "appwrite>=2.0.0"]
 
 [project]
 name = "django-cloud-storages"
 dynamic = ["version"]
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
 maintainers = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
 keywords = ["django", "python", "django-storages", "django-file-storages", "cloud storage", "file storage", "django dropbox"]
 description = "Cloud file storages for django."
-dependencies = ["django", "requests", "dropbox", "appwrite"]
+dependencies = ["django", "requests"]
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `django_cloud_storages-1.2.1/PKG-INFO` & `django_cloud_storages-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 1.2.1
+Version: 1.2.2
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://pypi.org/project/django-cloud-storages
 Project-URL: Source code, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Documentation, https://django-cloud-storages.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 Maintainer-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
@@ -17,24 +17,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
-Requires-Dist: appwrite
 Requires-Dist: django
-Requires-Dist: dropbox
 Requires-Dist: requests
 Provides-Extra: appwrite
-Requires-Dist: appwrite; extra == 'appwrite'
+Requires-Dist: appwrite>=2.0.0; extra == 'appwrite'
 Requires-Dist: django-cloud-storages[required]; extra == 'appwrite'
 Provides-Extra: dropbox
 Requires-Dist: django-cloud-storages[required]; extra == 'dropbox'
-Requires-Dist: dropbox; extra == 'dropbox'
+Requires-Dist: dropbox>=11.36.2; extra == 'dropbox'
 Provides-Extra: required
 Requires-Dist: django; extra == 'required'
 Requires-Dist: requests; extra == 'required'
 Description-Content-Type: text/markdown
 
 # Welcome to django-cloud-storages
```

