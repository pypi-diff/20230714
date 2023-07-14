# Comparing `tmp/djsm-0.0.3.tar.gz` & `tmp/djsm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsm-0.0.3.tar", last modified: Mon Jun 12 07:57:11 2023, max compression
+gzip compressed data, was "djsm-0.0.4.tar", last modified: Fri Jul 14 16:29:50 2023, max compression
```

## Comparing `djsm-0.0.3.tar` & `djsm-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:57:11.667058 djsm-0.0.3/
--rw-rw-rw-   0        0        0     1104 2023-06-04 21:28:33.000000 djsm-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    12942 2023-06-12 07:57:11.661066 djsm-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12098 2023-06-12 07:42:42.000000 djsm-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:57:11.517455 djsm-0.0.3/djsm/
--rw-rw-rw-   0        0        0      625 2023-06-12 07:55:20.000000 djsm-0.0.3/djsm/__init__.py
--rw-rw-rw-   0        0        0     7999 2023-06-10 07:29:05.000000 djsm-0.0.3/djsm/crypt.py
--rw-rw-rw-   0        0        0     7337 2023-06-09 21:21:42.000000 djsm-0.0.3/djsm/jcrypt.py
--rw-rw-rw-   0        0        0    14349 2023-06-12 07:54:36.000000 djsm-0.0.3/djsm/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:57:11.656037 djsm-0.0.3/djsm.egg-info/
--rw-rw-rw-   0        0        0    12942 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1041 2023-06-12 07:55:11.000000 djsm-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 07:57:11.668064 djsm-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 16:29:50.313317 djsm-0.0.4/
+-rw-rw-rw-   0        0        0     1104 2023-06-04 21:28:33.000000 djsm-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    12995 2023-07-14 16:29:50.305322 djsm-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12107 2023-07-14 16:22:57.000000 djsm-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 16:29:50.169320 djsm-0.0.4/djsm/
+-rw-rw-rw-   0        0        0      646 2023-07-10 14:58:24.000000 djsm-0.0.4/djsm/__init__.py
+-rw-rw-rw-   0        0        0     7999 2023-06-10 07:29:05.000000 djsm-0.0.4/djsm/crypt.py
+-rw-rw-rw-   0        0        0     7337 2023-06-09 21:21:42.000000 djsm-0.0.4/djsm/jcrypt.py
+-rw-rw-rw-   0        0        0    14462 2023-07-10 14:56:29.000000 djsm-0.0.4/djsm/manager.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:29:50.297315 djsm-0.0.4/djsm.egg-info/
+-rw-rw-rw-   0        0        0    12995 2023-07-14 16:29:49.000000 djsm-0.0.4/djsm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-14 16:29:50.000000 djsm-0.0.4/djsm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:29:49.000000 djsm-0.0.4/djsm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-14 16:29:50.000000 djsm-0.0.4/djsm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 16:29:50.000000 djsm-0.0.4/djsm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1181 2023-07-14 16:28:29.000000 djsm-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:29:50.313317 djsm-0.0.4/setup.cfg
```

### Comparing `djsm-0.0.3/LICENSE` & `djsm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djsm-0.0.3/PKG-INFO` & `djsm-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.0.3
+Version: 0.0.4
 Summary: DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project.
-Author-email: ti-oluwa <tioluwa.dev@gmail.com>
-Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
+Author-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
+Maintainer-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DJSM - Django JSON Secrets Manager
 
 ## What is DJSM?
 
@@ -35,19 +35,19 @@
 ```
 
 * Initial setup:
 
 Copy this into a .env file just outside your project (adjust as needed)
 
 ```.env
-DJSM_SECRETS_FILE_PATH = ".hidden_folder/pathtofile/secrets_file.json"
+DJSM_SECRETS_FILE_PATH = "/.hidden_folder/pathtofile/secrets_file.json"
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
-DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
+DJSM_SECRET_KEY_FILE_PATH = "/.hidden_folder/pathtofile/secret_key_file.json"
 ```
 
 Your project structure should look like this:
 
 ```bash
 
 |-- my_project
@@ -96,15 +96,15 @@
 Before starting, a '.env' file as to be created just outside the django project directory.
 In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
-SECRETS_FILE_PATH = ".secrets/pathtofile/secrets.json"
+SECRETS_FILE_PATH = "/.secrets/pathtofile/secrets.json"
 ```
 
 It is advisable to save secrets in an hidden folder(by prefixing the path with a period - '.'
 
 * **`DJSM_SECRET_KEY_NAME`** -> Name with which the Django secret key should be stored.
 Example:
 
@@ -113,15 +113,15 @@
 ```
 
 * **`DJSM_SECRET_KEY_FILE_PATH`** -> DJSM stores the Django secret key in a separate file, whose file path is provided by this variable, otherwise, the Django secret key is stored in the secrets file.
 Example:
 
 ```.env
 
-DJSM_SECRET_KEY_FILE_PATH = ".secrets/pathtofile/secret_key.json"
+DJSM_SECRET_KEY_FILE_PATH = "/.secrets/pathtofile/secret_key.json"
 ```
 
 ### Import djsm
 
 `djsm` is a pre-instanciated object of the class DJSM. You can import it using the following code.
 For most use cases, this is the only import you will need.
 
@@ -206,15 +206,15 @@
 How to use the `DjangoJSONSecretManager` class:
 
 ```python
 import os
 from djsm import DJSM  # DJSM is an alias for DjangoJSONSecretManager
 
 # Instantiation
-djsm = DJSM(os.getenv('SECRETS_FILE_PATH'))
+djsm = DJSM(os.getenv('DJSM_SECRETS_FILE_PATH'))
 
 # get a secret, say DB_PASSWORD
 db_password = djsm.get_secret("DB_PASSWORD")
 
 # generate a new secret key
 new_secret_key = djsm.generate_django_secret_key()
```

### Comparing `djsm-0.0.3/README.md` & `djsm-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 ```
 
 * Initial setup:
 
 Copy this into a .env file just outside your project (adjust as needed)
 
 ```.env
-DJSM_SECRETS_FILE_PATH = ".hidden_folder/pathtofile/secrets_file.json"
+DJSM_SECRETS_FILE_PATH = "/.hidden_folder/pathtofile/secrets_file.json"
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
-DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
+DJSM_SECRET_KEY_FILE_PATH = "/.hidden_folder/pathtofile/secret_key_file.json"
 ```
 
 Your project structure should look like this:
 
 ```bash
 
 |-- my_project
@@ -77,15 +77,15 @@
 Before starting, a '.env' file as to be created just outside the django project directory.
 In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
-SECRETS_FILE_PATH = ".secrets/pathtofile/secrets.json"
+SECRETS_FILE_PATH = "/.secrets/pathtofile/secrets.json"
 ```
 
 It is advisable to save secrets in an hidden folder(by prefixing the path with a period - '.'
 
 * **`DJSM_SECRET_KEY_NAME`** -> Name with which the Django secret key should be stored.
 Example:
 
@@ -94,15 +94,15 @@
 ```
 
 * **`DJSM_SECRET_KEY_FILE_PATH`** -> DJSM stores the Django secret key in a separate file, whose file path is provided by this variable, otherwise, the Django secret key is stored in the secrets file.
 Example:
 
 ```.env
 
-DJSM_SECRET_KEY_FILE_PATH = ".secrets/pathtofile/secret_key.json"
+DJSM_SECRET_KEY_FILE_PATH = "/.secrets/pathtofile/secret_key.json"
 ```
 
 ### Import djsm
 
 `djsm` is a pre-instanciated object of the class DJSM. You can import it using the following code.
 For most use cases, this is the only import you will need.
 
@@ -187,15 +187,15 @@
 How to use the `DjangoJSONSecretManager` class:
 
 ```python
 import os
 from djsm import DJSM  # DJSM is an alias for DjangoJSONSecretManager
 
 # Instantiation
-djsm = DJSM(os.getenv('SECRETS_FILE_PATH'))
+djsm = DJSM(os.getenv('DJSM_SECRETS_FILE_PATH'))
 
 # get a secret, say DB_PASSWORD
 db_password = djsm.get_secret("DB_PASSWORD")
 
 # generate a new secret key
 new_secret_key = djsm.generate_django_secret_key()
```

### Comparing `djsm-0.0.3/djsm/__init__.py` & `djsm-0.0.4/djsm/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 djsm - Django JSON Secrets Manager
 ==================================
 djsm helps create, store, retrieve, update and manage secrets in Django
 
 LICENSE: MIT
 """
 
-__version__ = "0.0.3"
-__author__ = "ti-oluwa"
+__version__ = "0.0.4"
+__author__ = "Daniel T. Afolayan (ti-oluwa)"
 __license__ = "MIT"
 
 import os
 import sys
 
 from .manager import DjangoJSONSecretManager as DJSM
 from .manager import (EnvLoadError, find_and_load_env_var, CryptKeysNotFound, check_setup_ok, env_variables)
```

### Comparing `djsm-0.0.3/djsm/crypt.py` & `djsm-0.0.4/djsm/crypt.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.3/djsm/jcrypt.py` & `djsm-0.0.4/djsm/jcrypt.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.3/djsm/manager.py` & `djsm-0.0.4/djsm/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     print("DJSM: Checking that .env file has been properly setup...\n")
     env_file_dict = dotenv_values(find_dotenv(raise_error_if_not_found=True))
     if not env_file_dict.get('DJSM_SECRETS_FILE_PATH', None):
         print('DJSM: DJSM_SECRETS_FILE_PATH not set in .env file\n')
         setup_ok = False
     if setup_ok:
         print('DJSM: Setup OK!\n')
+    else:
+        print('DJSM: Visit https://github.com/ti-oluwa/djsm/#usage for help on how to setup DJSM\n')
     return setup_ok
  
 
 
 class EnvLoadError(Exception):
     """Unable to load .env file mainly because it was not found"""
```

### Comparing `djsm-0.0.3/djsm.egg-info/PKG-INFO` & `djsm-0.0.4/djsm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.0.3
+Version: 0.0.4
 Summary: DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project.
-Author-email: ti-oluwa <tioluwa.dev@gmail.com>
-Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
+Author-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
+Maintainer-email: "Daniel T. Afolayan (ti-oluwa)" <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DJSM - Django JSON Secrets Manager
 
 ## What is DJSM?
 
@@ -35,19 +35,19 @@
 ```
 
 * Initial setup:
 
 Copy this into a .env file just outside your project (adjust as needed)
 
 ```.env
-DJSM_SECRETS_FILE_PATH = ".hidden_folder/pathtofile/secrets_file.json"
+DJSM_SECRETS_FILE_PATH = "/.hidden_folder/pathtofile/secrets_file.json"
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
-DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
+DJSM_SECRET_KEY_FILE_PATH = "/.hidden_folder/pathtofile/secret_key_file.json"
 ```
 
 Your project structure should look like this:
 
 ```bash
 
 |-- my_project
@@ -96,15 +96,15 @@
 Before starting, a '.env' file as to be created just outside the django project directory.
 In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
-SECRETS_FILE_PATH = ".secrets/pathtofile/secrets.json"
+SECRETS_FILE_PATH = "/.secrets/pathtofile/secrets.json"
 ```
 
 It is advisable to save secrets in an hidden folder(by prefixing the path with a period - '.'
 
 * **`DJSM_SECRET_KEY_NAME`** -> Name with which the Django secret key should be stored.
 Example:
 
@@ -113,15 +113,15 @@
 ```
 
 * **`DJSM_SECRET_KEY_FILE_PATH`** -> DJSM stores the Django secret key in a separate file, whose file path is provided by this variable, otherwise, the Django secret key is stored in the secrets file.
 Example:
 
 ```.env
 
-DJSM_SECRET_KEY_FILE_PATH = ".secrets/pathtofile/secret_key.json"
+DJSM_SECRET_KEY_FILE_PATH = "/.secrets/pathtofile/secret_key.json"
 ```
 
 ### Import djsm
 
 `djsm` is a pre-instanciated object of the class DJSM. You can import it using the following code.
 For most use cases, this is the only import you will need.
 
@@ -206,15 +206,15 @@
 How to use the `DjangoJSONSecretManager` class:
 
 ```python
 import os
 from djsm import DJSM  # DJSM is an alias for DjangoJSONSecretManager
 
 # Instantiation
-djsm = DJSM(os.getenv('SECRETS_FILE_PATH'))
+djsm = DJSM(os.getenv('DJSM_SECRETS_FILE_PATH'))
 
 # get a secret, say DB_PASSWORD
 db_password = djsm.get_secret("DB_PASSWORD")
 
 # generate a new secret key
 new_secret_key = djsm.generate_django_secret_key()
```

### Comparing `djsm-0.0.3/pyproject.toml` & `djsm-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.dynamic]
+version = {attr = "djsm.__version__"}
+
 [project]
 name = "djsm"
-version = "0.0.3"
+dynamic = ["version"]
+
 authors = [
-  { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
+  { name="Daniel T. Afolayan (ti-oluwa)", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
-  { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
+  { name="Daniel T. Afolayan (ti-oluwa)", email="tioluwa.dev@gmail.com" },
 ]
 description = "DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project."
 keywords = [
     "Django", "Django Secrets Encryption"
 ]
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
 ]
 dependencies = [
-    'py-dotenv',
-    'bs4-web-scraper',
-    'rsa',
+    'python-dotenv>=0.19.2',
+    'bs4-web-scraper>=0.1.3',
+    'rsa>=4.7.2',
     'cryptography',
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ti-oluwa/djsm"
 "Bug Tracker" = "https://github.com/ti-oluwa/djsm/issues"
 "Repository" = "https://github.com/ti-oluwa/djsm"
```

