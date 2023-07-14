# Comparing `tmp/bastila_search-0.4.4.tar.gz` & `tmp/bastila_search-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.4.4.tar", last modified: Fri Jul 14 19:22:33 2023, max compression
+gzip compressed data, was "bastila_search-0.4.5.tar", last modified: Fri Jul 14 19:31:37 2023, max compression
```

## Comparing `bastila_search-0.4.4.tar` & `bastila_search-0.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:22:33.438031 bastila_search-0.4.4/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.4.4/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)      621 2023-07-14 19:22:33.438031 bastila_search-0.4.4/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      292 2023-07-14 19:21:50.000000 bastila_search-0.4.4/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:22:33.438031 bastila_search-0.4.4/bastila_search/
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.4.4/bastila_search/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     5155 2023-07-11 00:58:56.000000 bastila_search-0.4.4/bastila_search/bastila_search.py
--rw-rw-r--   0 joe       (1000) joe       (1000)      444 2023-07-14 19:12:46.000000 bastila_search-0.4.4/bastila_search/setup_config.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:22:33.438031 bastila_search-0.4.4/bastila_search.egg-info/
--rw-rw-r--   0 joe       (1000) joe       (1000)      621 2023-07-14 19:22:33.000000 bastila_search-0.4.4/bastila_search.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-14 19:22:33.000000 bastila_search-0.4.4/bastila_search.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-14 19:22:33.000000 bastila_search-0.4.4/bastila_search.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)      116 2023-07-14 19:22:33.000000 bastila_search-0.4.4/bastila_search.egg-info/entry_points.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.4.4/bastila_search.egg-info/not-zip-safe
--rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-14 19:22:33.000000 bastila_search-0.4.4/bastila_search.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-14 19:22:33.000000 bastila_search-0.4.4/bastila_search.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-14 19:22:33.438031 bastila_search-0.4.4/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)      789 2023-07-14 19:21:56.000000 bastila_search-0.4.4/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:31:37.326990 bastila_search-0.4.5/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.4.5/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1103 2023-07-14 19:31:37.326990 bastila_search-0.4.5/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      775 2023-07-14 19:30:52.000000 bastila_search-0.4.5/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:31:37.326990 bastila_search-0.4.5/bastila_search/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.4.5/bastila_search/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     5155 2023-07-11 00:58:56.000000 bastila_search-0.4.5/bastila_search/bastila_search.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      444 2023-07-14 19:12:46.000000 bastila_search-0.4.5/bastila_search/setup_config.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:31:37.326990 bastila_search-0.4.5/bastila_search.egg-info/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1103 2023-07-14 19:31:37.000000 bastila_search-0.4.5/bastila_search.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-14 19:31:37.000000 bastila_search-0.4.5/bastila_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-14 19:31:37.000000 bastila_search-0.4.5/bastila_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      116 2023-07-14 19:31:37.000000 bastila_search-0.4.5/bastila_search.egg-info/entry_points.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.4.5/bastila_search.egg-info/not-zip-safe
+-rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-14 19:31:37.000000 bastila_search-0.4.5/bastila_search.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-14 19:31:37.000000 bastila_search-0.4.5/bastila_search.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-14 19:31:37.326990 bastila_search-0.4.5/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)      789 2023-07-14 19:31:08.000000 bastila_search-0.4.5/setup.py
```

### Comparing `bastila_search-0.4.4/LICENSE` & `bastila_search-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bastila_search-0.4.4/PKG-INFO` & `bastila_search-0.4.5/bastila_search.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
-Name: bastila_search
-Version: 0.4.4
+Name: bastila-search
+Version: 0.4.5
 Summary: A python script that catches commits that introduce predefined deprecated patterns
 Home-page: https://github.com/GetBastila/bastila-hook
 Author: Bastila
 Author-email: hello@bastila.app
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Bastila
 
+[Bastila](https://bastila.app/) is a tool for removing deprecated code. You define deprecated patterns using regex in the app and then prevent additional usages of those deprecated patterns from being used. The tool can also be used to track the removal of these patterns as well.
+
 ### Installation Instructions
 
 1. Install the package `pip install bastila-search`
 2. Create a precommit file `touch .git/hooks/pre-commit`
 3. Add execute access to that file `chmod +x .git/hooks/pre-commit`
 4. Add the script to your pre-commit file
-
 ```
 #!/bin/sh
 bastila_run
 ```
+5. Run the setup command to create a config file with your env vars `bastila_setup`. This will create a config.json file that should be kept in the root of your repository.
+
+Support: hello@bastila.app
```

### Comparing `bastila_search-0.4.4/bastila_search/bastila_search.py` & `bastila_search-0.4.5/bastila_search/bastila_search.py`

 * *Files identical despite different names*

### Comparing `bastila_search-0.4.4/bastila_search.egg-info/PKG-INFO` & `bastila_search-0.4.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
-Name: bastila-search
-Version: 0.4.4
+Name: bastila_search
+Version: 0.4.5
 Summary: A python script that catches commits that introduce predefined deprecated patterns
 Home-page: https://github.com/GetBastila/bastila-hook
 Author: Bastila
 Author-email: hello@bastila.app
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Bastila
 
+[Bastila](https://bastila.app/) is a tool for removing deprecated code. You define deprecated patterns using regex in the app and then prevent additional usages of those deprecated patterns from being used. The tool can also be used to track the removal of these patterns as well.
+
 ### Installation Instructions
 
 1. Install the package `pip install bastila-search`
 2. Create a precommit file `touch .git/hooks/pre-commit`
 3. Add execute access to that file `chmod +x .git/hooks/pre-commit`
 4. Add the script to your pre-commit file
-
 ```
 #!/bin/sh
 bastila_run
 ```
+5. Run the setup command to create a config file with your env vars `bastila_setup`. This will create a config.json file that should be kept in the root of your repository.
+
+Support: hello@bastila.app
```

### Comparing `bastila_search-0.4.4/setup.py` & `bastila_search-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='bastila_search',
-    version='0.4.4',
+    version='0.4.5',
     description='A python script that catches commits that introduce predefined deprecated patterns',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/GetBastila/bastila-hook',
     author='Bastila',
     author_email='hello@bastila.app',
     license='MIT',
```

