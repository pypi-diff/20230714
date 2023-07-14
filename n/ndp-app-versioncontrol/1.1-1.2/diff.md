# Comparing `tmp/ndp-app-versioncontrol-1.1.tar.gz` & `tmp/ndp-app-versioncontrol-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndp-app-versioncontrol-1.1.tar", last modified: Tue Jul 11 06:42:18 2023, max compression
+gzip compressed data, was "ndp-app-versioncontrol-1.2.tar", last modified: Fri Jul 14 03:16:36 2023, max compression
```

## Comparing `ndp-app-versioncontrol-1.1.tar` & `ndp-app-versioncontrol-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 06:42:18.862455 ndp-app-versioncontrol-1.1/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-11 06:42:18.862146 ndp-app-versioncontrol-1.1/PKG-INFO
--rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-11 06:41:26.000000 ndp-app-versioncontrol-1.1/README.md
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 06:42:18.860951 ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-11 06:42:18.000000 ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/PKG-INFO
--rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-11 06:42:18.000000 ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/SOURCES.txt
--rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-11 06:42:18.000000 ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/dependency_links.txt
--rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-11 06:42:18.000000 ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/requires.txt
--rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-11 06:42:18.000000 ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/top_level.txt
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 06:42:18.861564 ndp-app-versioncontrol-1.1/ndp_versioncontrol/
--rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.1/ndp_versioncontrol/__init__.py
--rwxrwxr-x   0 harshal    (502) staff       (20)    22570 2023-07-11 06:39:00.000000 ndp-app-versioncontrol-1.1/ndp_versioncontrol/generate_backup_sql.py
--rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-11 06:42:18.862554 ndp-app-versioncontrol-1.1/setup.cfg
--rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-11 06:39:13.000000 ndp-app-versioncontrol-1.1/setup.py
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 03:16:36.462139 ndp-app-versioncontrol-1.2/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 03:16:36.461479 ndp-app-versioncontrol-1.2/PKG-INFO
+-rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-14 03:15:23.000000 ndp-app-versioncontrol-1.2/README.md
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 03:16:36.459668 ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 03:16:36.000000 ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/PKG-INFO
+-rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-14 03:16:36.000000 ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-14 03:16:36.000000 ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-14 03:16:36.000000 ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/requires.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-14 03:16:36.000000 ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/top_level.txt
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 03:16:36.460577 ndp-app-versioncontrol-1.2/ndp_versioncontrol/
+-rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.2/ndp_versioncontrol/__init__.py
+-rwxrwxr-x   0 harshal    (502) staff       (20)    22574 2023-07-14 03:14:38.000000 ndp-app-versioncontrol-1.2/ndp_versioncontrol/generate_backup_sql.py
+-rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-14 03:16:36.462352 ndp-app-versioncontrol-1.2/setup.cfg
+-rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-14 03:15:07.000000 ndp-app-versioncontrol-1.2/setup.py
```

### Comparing `ndp-app-versioncontrol-1.1/PKG-INFO` & `ndp-app-versioncontrol-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.1
+Version: 1.2
 Summary: Version Control Mechanism for Zetaris Platform (https://www.zetaris.com/)
 Home-page: https://github.com/zetaris/versioncontrol
 Author: Harshal Shah
 Author-email: harshal.shah@zetaris.com
 License: Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ### Usage and Installation
 ```
-pip3 install ndp-app-versioncontrol==1.1
+pip3 install ndp-app-versioncontrol==1.2
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.1/ndp_app_versioncontrol.egg-info/PKG-INFO` & `ndp-app-versioncontrol-1.2/ndp_app_versioncontrol.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.1
+Version: 1.2
 Summary: Version Control Mechanism for Zetaris Platform (https://www.zetaris.com/)
 Home-page: https://github.com/zetaris/versioncontrol
 Author: Harshal Shah
 Author-email: harshal.shah@zetaris.com
 License: Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ### Usage and Installation
 ```
-pip3 install ndp-app-versioncontrol==1.1
+pip3 install ndp-app-versioncontrol==1.2
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.1/ndp_versioncontrol/generate_backup_sql.py` & `ndp-app-versioncontrol-1.2/ndp_versioncontrol/generate_backup_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     global refresh_token
     auth = get_auth(refresh_token)
     response = requests.get(url=f'{api_url}/api/v1.0/auth/refresh',headers=auth)
     response = json.loads(response.text)
     bearer_token = f"Bearer {response['idToken']}"
     refresh_token = f"Bearer {response['refreshToken']}"
 
-def get_pipeline_containers():
+def get_pipeline_containers_api():
     auth = get_auth()
     response = requests.get(url=f'{api_url}/api/v1.0/pipeline/containers',headers=auth)
     response = json.loads(response.text)
     return response
 
 def get_pipeline_relations(pipeline_container_id:int):
     auth = get_auth()
```

### Comparing `ndp-app-versioncontrol-1.1/setup.py` & `ndp-app-versioncontrol-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
   
 setuptools.setup(
     # Here is the module name.
     name="ndp-app-versioncontrol",
   
     # version of the module
-    version="1.1",
+    version="1.2",
   
     # Name of Author
     author="Harshal Shah",
 
     #License
     license="Proprietary",
```

