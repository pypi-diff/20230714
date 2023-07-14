# Comparing `tmp/pulumi_mailgun-3.5.0a1687671492.tar.gz` & `tmp/pulumi_mailgun-3.5.0a1689313554.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mailgun-3.5.0a1687671492.tar", last modified: Sun Jun 25 05:46:30 2023, max compression
+gzip compressed data, was "pulumi_mailgun-3.5.0a1689313554.tar", last modified: Fri Jul 14 05:58:08 2023, max compression
```

## Comparing `pulumi_mailgun-3.5.0a1687671492.tar` & `pulumi_mailgun-3.5.0a1689313554.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:46:30.552015 pulumi_mailgun-3.5.0a1687671492/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-25 05:46:30.552015 pulumi_mailgun-3.5.0a1687671492/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:46:30.552015 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:46:30.552015 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    35337 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/domain_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16111 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14156 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:46:30.552015 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:46:30.552015 pulumi_mailgun-3.5.0a1687671492/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-25 05:46:30.000000 pulumi_mailgun-3.5.0a1687671492/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:58:08.710220 pulumi_mailgun-3.5.0a1689313554/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-14 05:58:08.710220 pulumi_mailgun-3.5.0a1689313554/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:58:08.706220 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:58:08.710220 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35337 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/domain_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16111 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14156 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:58:08.710220 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:58:08.710220 pulumi_mailgun-3.5.0a1689313554/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-14 05:58:08.000000 pulumi_mailgun-3.5.0a1689313554/setup.py
```

### Comparing `pulumi_mailgun-3.5.0a1687671492/PKG-INFO` & `pulumi_mailgun-3.5.0a1689313554/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.5.0a1687671492
+Version: 3.5.0a1689313554
 Summary: A Pulumi package for creating and managing Mailgun resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi mailgun
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.5.0a1687671492/README.md` & `pulumi_mailgun-3.5.0a1689313554/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/__init__.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/_inputs.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/_utilities.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/config/vars.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/domain.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/domain_credential.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/domain_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/get_domain.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/outputs.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/provider.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/route.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun/webhook.py` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/PKG-INFO` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-mailgun
-Version: 3.5.0a1687671492
+Version: 3.5.0a1689313554
 Summary: A Pulumi package for creating and managing Mailgun resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi mailgun
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.5.0a1687671492/pulumi_mailgun.egg-info/SOURCES.txt` & `pulumi_mailgun-3.5.0a1689313554/pulumi_mailgun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.5.0a1687671492/setup.py` & `pulumi_mailgun-3.5.0a1689313554/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.5.0a1687671492"
-PLUGIN_VERSION = "3.5.0-alpha.1687671492+525cbe49"
+VERSION = "3.5.0a1689313554"
+PLUGIN_VERSION = "3.5.0-alpha.1689313554+8a260be3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'mailgun', PLUGIN_VERSION])
         except OSError as error:
```

