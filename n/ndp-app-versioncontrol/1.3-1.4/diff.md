# Comparing `tmp/ndp-app-versioncontrol-1.3.tar.gz` & `tmp/ndp-app-versioncontrol-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndp-app-versioncontrol-1.3.tar", last modified: Fri Jul 14 05:10:03 2023, max compression
+gzip compressed data, was "ndp-app-versioncontrol-1.4.tar", last modified: Fri Jul 14 05:11:40 2023, max compression
```

## Comparing `ndp-app-versioncontrol-1.3.tar` & `ndp-app-versioncontrol-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 05:10:03.056753 ndp-app-versioncontrol-1.3/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 05:10:03.056288 ndp-app-versioncontrol-1.3/PKG-INFO
--rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-14 05:09:38.000000 ndp-app-versioncontrol-1.3/README.md
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 05:10:03.054587 ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 05:10:02.000000 ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/PKG-INFO
--rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-14 05:10:02.000000 ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/SOURCES.txt
--rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-14 05:10:02.000000 ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/dependency_links.txt
--rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-14 05:10:02.000000 ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/requires.txt
--rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-14 05:10:02.000000 ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/top_level.txt
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 05:10:03.055332 ndp-app-versioncontrol-1.3/ndp_versioncontrol/
--rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.3/ndp_versioncontrol/__init__.py
--rwxrwxr-x   0 harshal    (502) staff       (20)    22591 2023-07-14 05:09:05.000000 ndp-app-versioncontrol-1.3/ndp_versioncontrol/generate_backup_sql.py
--rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-14 05:10:03.056908 ndp-app-versioncontrol-1.3/setup.cfg
--rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-14 05:09:28.000000 ndp-app-versioncontrol-1.3/setup.py
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 05:11:40.326035 ndp-app-versioncontrol-1.4/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 05:11:40.325742 ndp-app-versioncontrol-1.4/PKG-INFO
+-rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-14 05:11:31.000000 ndp-app-versioncontrol-1.4/README.md
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 05:11:40.324427 ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 05:11:40.000000 ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/PKG-INFO
+-rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-14 05:11:40.000000 ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-14 05:11:40.000000 ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-14 05:11:40.000000 ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/requires.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-14 05:11:40.000000 ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/top_level.txt
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 05:11:40.325087 ndp-app-versioncontrol-1.4/ndp_versioncontrol/
+-rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.4/ndp_versioncontrol/__init__.py
+-rwxrwxr-x   0 harshal    (502) staff       (20)    22592 2023-07-14 05:11:00.000000 ndp-app-versioncontrol-1.4/ndp_versioncontrol/generate_backup_sql.py
+-rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-14 05:11:40.326132 ndp-app-versioncontrol-1.4/setup.cfg
+-rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-14 05:11:19.000000 ndp-app-versioncontrol-1.4/setup.py
```

### Comparing `ndp-app-versioncontrol-1.3/PKG-INFO` & `ndp-app-versioncontrol-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.3
+Version: 1.4
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
-pip3 install ndp-app-versioncontrol==1.3
+pip3 install ndp-app-versioncontrol==1.4
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.3/ndp_app_versioncontrol.egg-info/PKG-INFO` & `ndp-app-versioncontrol-1.4/ndp_app_versioncontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.3
+Version: 1.4
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
-pip3 install ndp-app-versioncontrol==1.3
+pip3 install ndp-app-versioncontrol==1.4
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.3/ndp_versioncontrol/generate_backup_sql.py` & `ndp-app-versioncontrol-1.4/ndp_versioncontrol/generate_backup_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     #SET API URL AND PASS LOGIN CREDENTIALS TO THE API
     set_api_base_url(api_url)
     login(lightning_username,lightning_pass)
     #IF THE USER WANTS BACKUP, PERFORM THE BELOW OPERATIONS
     if str(vcarg1).lower().strip()=='backup':
         #CALL BACKUP PIPELINES FUNCTION AT AN INDIVIDUAL LEVEL
         print('Backup of INDIVIDUAL PIPELINES - PROCESS BEGUN')
-        get_individual_pipelines(folder_path,lightning_username,lightning_pass,api_url)
+        #get_individual_pipelines(folder_path,lightning_username,lightning_pass,api_url)
         print('Backup of INDIVIDUAL PIPELINES - PROCESS END')
         #CALL BACKUP PIPELINES FUNCTION AT A CONTAINER LEVEL
         print('Backup of PIPELINES CONTAINER - PROCESS BEGUN')
         get_pipeline_containers(folder_path,lightning_username,lightning_pass,api_url)
         print('Backup of PIPELINES CONTAINER - PROCESS END')
         #CALL BACKUP PERMANENT DATA VIEWS FUNCTION
         print('Backup of PERMANENT VIEWS - PROCESS BEGUN')
```

### Comparing `ndp-app-versioncontrol-1.3/setup.py` & `ndp-app-versioncontrol-1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
   
 setuptools.setup(
     # Here is the module name.
     name="ndp-app-versioncontrol",
   
     # version of the module
-    version="1.3",
+    version="1.4",
   
     # Name of Author
     author="Harshal Shah",
 
     #License
     license="Proprietary",
```

