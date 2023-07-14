# Comparing `tmp/nvosscript-1.3.7.3.tar.gz` & `tmp/nvosscript-1.3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.7.3.tar", last modified: Fri Jul 14 07:51:24 2023, max compression
+gzip compressed data, was "nvosscript-1.3.7.4.tar", last modified: Fri Jul 14 09:05:26 2023, max compression
```

## Comparing `nvosscript-1.3.7.3.tar` & `nvosscript-1.3.7.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.813241 nvosscript-1.3.7.3/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.3/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 07:51:24.812740 nvosscript-1.3.7.3/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.3/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.794432 nvosscript-1.3.7.3/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.3/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.3/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7.3/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.3/nvos/run.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.800096 nvosscript-1.3.7.3/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-14 07:51:24.813322 nvosscript-1.3.7.3/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-14 06:45:57.000000 nvosscript-1.3.7.3/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.807195 nvosscript-1.3.7.3/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.3/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.3/skyeye/handler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      802 2023-05-31 08:56:53.000000 nvosscript-1.3.7.3/skyeye/loghandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     2529 2023-07-14 06:45:43.000000 nvosscript-1.3.7.3/skyeye/remote.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.811184 nvosscript-1.3.7.3/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.3/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.3/start/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-14 06:46:02.000000 nvosscript-1.3.7.3/start/main.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.3/start/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.811917 nvosscript-1.3.7.3/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.3/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.148304 nvosscript-1.3.7.4/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.4/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 09:05:26.148050 nvosscript-1.3.7.4/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.4/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.137767 nvosscript-1.3.7.4/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.4/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.4/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7.4/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.4/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.141550 nvosscript-1.3.7.4/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-14 09:05:26.000000 nvosscript-1.3.7.4/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-14 09:05:26.148355 nvosscript-1.3.7.4/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-14 09:04:49.000000 nvosscript-1.3.7.4/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.144357 nvosscript-1.3.7.4/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.4/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.4/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1024 2023-07-14 09:04:44.000000 nvosscript-1.3.7.4/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     2529 2023-07-14 06:45:43.000000 nvosscript-1.3.7.4/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.146919 nvosscript-1.3.7.4/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.4/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.4/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-14 09:04:53.000000 nvosscript-1.3.7.4/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.4/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 09:05:26.147492 nvosscript-1.3.7.4/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.4/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.7.3/LICENSE` & `nvosscript-1.3.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/nvos/file.py` & `nvosscript-1.3.7.4/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/nvos/remote.py` & `nvosscript-1.3.7.4/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/nvos/run.py` & `nvosscript-1.3.7.4/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/setup.py` & `nvosscript-1.3.7.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.7.03',
+    version='1.3.7.04',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.7.3/skyeye/loghandler.py` & `nvosscript-1.3.7.4/skyeye/loghandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,18 @@
         return
 
     with open(path, 'r') as f:
         for line in f:
             matchObj = re.search("\d\|\d+\|\d+\|.*", line, re.M | re.I)
             if matchObj:
                 logger_list.append(line)
+            if len(logger_list) == 1000:
+                logger.info(f"filter logger info data is {logger_list}")
+                remote.upload_file(logger_list, os.path.basename(path))
+                logger_list.clear()
 
     logger.info(f"filter logger info data is {logger_list}")
     remote.upload_file(logger_list, os.path.basename(path))
```

### Comparing `nvosscript-1.3.7.3/skyeye/remote.py` & `nvosscript-1.3.7.4/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/start/login.py` & `nvosscript-1.3.7.4/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/start/main.py` & `nvosscript-1.3.7.4/start/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.7.03")
+        print("1.3.7.04")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.7.3/start/utils.py` & `nvosscript-1.3.7.4/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.3/win/win_auto_script.py` & `nvosscript-1.3.7.4/win/win_auto_script.py`

 * *Files identical despite different names*

