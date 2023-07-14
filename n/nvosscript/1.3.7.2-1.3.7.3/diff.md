# Comparing `tmp/nvosscript-1.3.7.2.tar.gz` & `tmp/nvosscript-1.3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.7.2.tar", last modified: Thu Jul 13 02:51:05 2023, max compression
+gzip compressed data, was "nvosscript-1.3.7.3.tar", last modified: Fri Jul 14 07:51:24 2023, max compression
```

## Comparing `nvosscript-1.3.7.2.tar` & `nvosscript-1.3.7.3.tar`

### file list

```diff
@@ -1,46 +1,30 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.925035 nvosscript-1.3.7.2/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.7.2/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-07-13 02:51:05.924879 nvosscript-1.3.7.2/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.7.2/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.917977 nvosscript-1.3.7.2/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.7.2/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    15134 2023-07-13 02:50:36.000000 nvosscript-1.3.7.2/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     8909 2023-07-04 01:26:21.000000 nvosscript-1.3.7.2/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6293 2023-06-20 02:23:27.000000 nvosscript-1.3.7.2/nvos/run.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.919036 nvosscript-1.3.7.2/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      759 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-07-13 02:51:05.925083 nvosscript-1.3.7.2/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      808 2023-07-13 01:14:55.000000 nvosscript-1.3.7.2/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.919768 nvosscript-1.3.7.2/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.7.2/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      502 2023-05-30 09:54:35.000000 nvosscript-1.3.7.2/skyeye/handler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      802 2023-06-19 10:04:39.000000 nvosscript-1.3.7.2/skyeye/loghandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     2531 2023-06-19 10:04:39.000000 nvosscript-1.3.7.2/skyeye/remote.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.920541 nvosscript-1.3.7.2/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.7.2/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1803 2023-07-04 01:26:21.000000 nvosscript-1.3.7.2/start/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4503 2023-07-13 01:15:00.000000 nvosscript-1.3.7.2/start/main.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1182 2023-06-20 02:18:44.000000 nvosscript-1.3.7.2/start/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.916097 nvosscript-1.3.7.2/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.924265 nvosscript-1.3.7.2/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.7.2/venv/bin/activate_this.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-05-26 05:59:41.000000 nvosscript-1.3.7.2/venv/bin/jp.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      642 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2html.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      764 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      841 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      664 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2man.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      830 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      636 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      649 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      685 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      921 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      650 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      718 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rstpep2html.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.924501 nvosscript-1.3.7.2/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.7.2/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.813241 nvosscript-1.3.7.3/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7.3/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 07:51:24.812740 nvosscript-1.3.7.3/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7.3/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.794432 nvosscript-1.3.7.3/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7.3/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    15134 2023-07-14 06:45:49.000000 nvosscript-1.3.7.3/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7.3/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7.3/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.800096 nvosscript-1.3.7.3/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      335 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-07-14 07:51:24.000000 nvosscript-1.3.7.3/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-07-14 07:51:24.813322 nvosscript-1.3.7.3/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      808 2023-07-14 06:45:57.000000 nvosscript-1.3.7.3/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.807195 nvosscript-1.3.7.3/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7.3/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7.3/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      802 2023-05-31 08:56:53.000000 nvosscript-1.3.7.3/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     2529 2023-07-14 06:45:43.000000 nvosscript-1.3.7.3/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.811184 nvosscript-1.3.7.3/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7.3/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7.3/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4503 2023-07-14 06:46:02.000000 nvosscript-1.3.7.3/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7.3/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-07-14 07:51:24.811917 nvosscript-1.3.7.3/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7.3/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.7.2/LICENSE` & `nvosscript-1.3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/nvos/file.py` & `nvosscript-1.3.7.3/nvos/file.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/nvos/remote.py` & `nvosscript-1.3.7.3/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/nvos/run.py` & `nvosscript-1.3.7.3/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/setup.py` & `nvosscript-1.3.7.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.7.02',
+    version='1.3.7.03',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.7.2/skyeye/loghandler.py` & `nvosscript-1.3.7.3/skyeye/loghandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/skyeye/remote.py` & `nvosscript-1.3.7.3/skyeye/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import json
 from start import utils,login
 
 
 daemon_network = "https://nvos-toolchain.nioint.com"
 
 daemon_network_mapping = {
-    "prod": "https://nvos-toolchain.nioint.com",
-    "stg": "https://nvos-toolchain-stg.nioint.com",
+    "prod": "https://sky-eye-trace.nioint.com",
+    "stg": "https://sky-eye-trace-stg.nioint.com",
     "dev": "https://sky-eye-trace-dev.nioint.com",
     "local": "http://127.0.0.1:12800"
 }
 
 daemon_network_front_mapping = {
     "prod": "https://ndtc.nioint.com/#/nvosTool/spaceList",
     "stg": "https://ndtc-stg.nioint.com/#/nvosTool/spaceList",
```

### Comparing `nvosscript-1.3.7.2/start/login.py` & `nvosscript-1.3.7.3/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/start/main.py` & `nvosscript-1.3.7.3/start/main.py`

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
-        print("1.3.7.02")
+        print("1.3.7.03")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.7.2/start/utils.py` & `nvosscript-1.3.7.3/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7.2/win/win_auto_script.py` & `nvosscript-1.3.7.3/win/win_auto_script.py`

 * *Files identical despite different names*

