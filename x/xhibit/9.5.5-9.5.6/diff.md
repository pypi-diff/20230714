# Comparing `tmp/xhibit-9.5.5.tar.gz` & `tmp/xhibit-9.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhibit-9.5.5.tar", last modified: Fri Jul 14 06:51:02 2023, max compression
+gzip compressed data, was "xhibit-9.5.6.tar", last modified: Fri Jul 14 06:57:56 2023, max compression
```

## Comparing `xhibit-9.5.5.tar` & `xhibit-9.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:51:02.877654 xhibit-9.5.5/
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:51:02.876654 xhibit-9.5.5/Exhibition/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/__init__.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/ascii.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/color_palette.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/colors.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2641 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/image.py
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/pos.sh
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/shell.sh
--rw-r--r--   0 ayush     (1000) ayush     (1000)      627 2023-07-14 06:37:33.000000 xhibit-9.5.5/Exhibition/sysinfo.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:37:33.000000 xhibit-9.5.5/LICENSE
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:51:02.877654 xhibit-9.5.5/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:37:33.000000 xhibit-9.5.5/README.md
--rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:51:02.877654 xhibit-9.5.5/setup.cfg
--rw-r--r--   0 ayush     (1000) ayush     (1000)     1047 2023-07-14 06:50:58.000000 xhibit-9.5.5/setup.py
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:51:02.877654 xhibit-9.5.5/xhibit.egg-info/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:51:02.000000 xhibit-9.5.5/xhibit.egg-info/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:51:02.000000 xhibit-9.5.5/xhibit.egg-info/SOURCES.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:51:02.000000 xhibit-9.5.5/xhibit.egg-info/dependency_links.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:51:02.000000 xhibit-9.5.5/xhibit.egg-info/entry_points.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:51:02.000000 xhibit-9.5.5/xhibit.egg-info/requires.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:51:02.000000 xhibit-9.5.5/xhibit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:57:56.006133 xhibit-9.5.6/
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:57:56.005133 xhibit-9.5.6/Exhibition/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/__init__.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/ascii.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/color_palette.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/colors.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2641 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/image.py
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/pos.sh
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/shell.sh
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      627 2023-07-14 06:37:33.000000 xhibit-9.5.6/Exhibition/sysinfo.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:37:33.000000 xhibit-9.5.6/LICENSE
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:57:56.006133 xhibit-9.5.6/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:37:33.000000 xhibit-9.5.6/README.md
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:57:56.006133 xhibit-9.5.6/setup.cfg
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     1097 2023-07-14 06:57:54.000000 xhibit-9.5.6/setup.py
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:57:56.006133 xhibit-9.5.6/xhibit.egg-info/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:57:55.000000 xhibit-9.5.6/xhibit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:57:55.000000 xhibit-9.5.6/xhibit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:57:55.000000 xhibit-9.5.6/xhibit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:57:55.000000 xhibit-9.5.6/xhibit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:57:55.000000 xhibit-9.5.6/xhibit.egg-info/requires.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:57:55.000000 xhibit-9.5.6/xhibit.egg-info/top_level.txt
```

### Comparing `xhibit-9.5.5/Exhibition/__init__.py` & `xhibit-9.5.6/Exhibition/__init__.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/ascii.py` & `xhibit-9.5.6/Exhibition/ascii.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/color_palette.py` & `xhibit-9.5.6/Exhibition/color_palette.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/colors.py` & `xhibit-9.5.6/Exhibition/colors.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/image.py` & `xhibit-9.5.6/Exhibition/image.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/pos.sh` & `xhibit-9.5.6/Exhibition/pos.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/shell.sh` & `xhibit-9.5.6/Exhibition/shell.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/Exhibition/sysinfo.py` & `xhibit-9.5.6/Exhibition/sysinfo.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/LICENSE` & `xhibit-9.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/PKG-INFO` & `xhibit-9.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.5.5
+Version: 9.5.6
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `xhibit-9.5.5/README.md` & `xhibit-9.5.6/README.md`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.5/setup.py` & `xhibit-9.5.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import setuptools
+import os
+
+root_dir = os.path.abspath("/usr/local/bin/")
+
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhibit",
-    version="9.5.5",
+    version="9.5.6",
     author="glowfi",
     description="A python script to exhibit your ascii arts and sytem specs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/glowfi/xhibit",
     classifiers=[
@@ -23,11 +27,11 @@
     entry_points={
         "console_scripts": [
             "xhibit=Exhibition.__init__:__init__",
         ]
     },
     install_requires=["tcolorpy"],
     data_files=[
-        ("/usr/local/bin/", ["./Exhibition/pos.sh"]),
-        ("/usr/local/bin/", ["./Exhibition/shell.sh"]),
+        (f"{root_dir}", ["./Exhibition/pos.sh"]),
+        (f"{root_dir}", ["./Exhibition/shell.sh"]),
     ],
 )
```

### Comparing `xhibit-9.5.5/xhibit.egg-info/PKG-INFO` & `xhibit-9.5.6/xhibit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.5.5
+Version: 9.5.6
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

