# Comparing `tmp/pulumi_rke-3.3.0a1687758532.tar.gz` & `tmp/pulumi_rke-3.3.0a1689316376.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rke-3.3.0a1687758532.tar", last modified: Mon Jun 26 05:53:42 2023, max compression
+gzip compressed data, was "pulumi_rke-3.3.0a1689316376.tar", last modified: Fri Jul 14 06:43:25 2023, max compression
```

## Comparing `pulumi_rke-3.3.0a1687758532.tar` & `pulumi_rke-3.3.0a1689316376.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:53:42.818241 pulumi_rke-3.3.0a1687758532/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-26 05:53:42.818241 pulumi_rke-3.3.0a1687758532/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:53:42.818241 pulumi_rke-3.3.0a1687758532/pulumi_rke/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   393841 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   132925 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:53:42.818241 pulumi_rke-3.3.0a1687758532/pulumi_rke/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   355040 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:53:42.818241 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:53:42.818241 pulumi_rke-3.3.0a1687758532/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-26 05:53:42.000000 pulumi_rke-3.3.0a1687758532/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:43:25.574509 pulumi_rke-3.3.0a1689316376/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-14 06:43:25.574509 pulumi_rke-3.3.0a1689316376/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:43:25.574509 pulumi_rke-3.3.0a1689316376/pulumi_rke/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   393841 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132925 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:43:25.574509 pulumi_rke-3.3.0a1689316376/pulumi_rke/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   355040 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:43:25.574509 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:43:25.574509 pulumi_rke-3.3.0a1689316376/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-14 06:43:25.000000 pulumi_rke-3.3.0a1689316376/setup.py
```

### Comparing `pulumi_rke-3.3.0a1687758532/PKG-INFO` & `pulumi_rke-3.3.0a1689316376/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.3.0a1687758532
+Version: 3.3.0a1689316376
 Summary: A Pulumi package for creating and managing rke cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi rke
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.3.0a1687758532/README.md` & `pulumi_rke-3.3.0a1689316376/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/__init__.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/_inputs.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/_utilities.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/cluster.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/config/vars.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/outputs.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke/provider.py` & `pulumi_rke-3.3.0a1689316376/pulumi_rke/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1687758532/pulumi_rke.egg-info/PKG-INFO` & `pulumi_rke-3.3.0a1689316376/pulumi_rke.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rke
-Version: 3.3.0a1687758532
+Version: 3.3.0a1689316376
 Summary: A Pulumi package for creating and managing rke cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi rke
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.3.0a1687758532/setup.py` & `pulumi_rke-3.3.0a1689316376/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.3.0a1687758532"
-PLUGIN_VERSION = "3.3.0-alpha.1687758532+8eb36ea6"
+VERSION = "3.3.0a1689316376"
+PLUGIN_VERSION = "3.3.0-alpha.1689316376+2550ae16"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rke', PLUGIN_VERSION])
         except OSError as error:
```

