# Comparing `tmp/xhibit-9.5.1.tar.gz` & `tmp/xhibit-9.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhibit-9.5.1.tar", last modified: Fri Jul 14 06:39:18 2023, max compression
+gzip compressed data, was "xhibit-9.5.2.tar", last modified: Fri Jul 14 06:42:34 2023, max compression
```

## Comparing `xhibit-9.5.1.tar` & `xhibit-9.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:39:18.723552 xhibit-9.5.1/
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:39:18.722552 xhibit-9.5.1/Exhibition/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/__init__.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/ascii.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/color_palette.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/colors.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2641 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/image.py
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/pos.sh
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/shell.sh
--rw-r--r--   0 ayush     (1000) ayush     (1000)      627 2023-07-14 06:37:33.000000 xhibit-9.5.1/Exhibition/sysinfo.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:37:33.000000 xhibit-9.5.1/LICENSE
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:39:18.723552 xhibit-9.5.1/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:37:33.000000 xhibit-9.5.1/README.md
--rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:39:18.723552 xhibit-9.5.1/setup.cfg
--rw-r--r--   0 ayush     (1000) ayush     (1000)     1062 2023-07-14 06:38:59.000000 xhibit-9.5.1/setup.py
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:39:18.723552 xhibit-9.5.1/xhibit.egg-info/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:39:18.000000 xhibit-9.5.1/xhibit.egg-info/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:39:18.000000 xhibit-9.5.1/xhibit.egg-info/SOURCES.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:39:18.000000 xhibit-9.5.1/xhibit.egg-info/dependency_links.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:39:18.000000 xhibit-9.5.1/xhibit.egg-info/entry_points.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:39:18.000000 xhibit-9.5.1/xhibit.egg-info/requires.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:39:18.000000 xhibit-9.5.1/xhibit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:42:34.076646 xhibit-9.5.2/
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:42:34.076646 xhibit-9.5.2/Exhibition/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/__init__.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/ascii.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/color_palette.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/colors.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2641 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/image.py
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/pos.sh
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/shell.sh
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      627 2023-07-14 06:37:33.000000 xhibit-9.5.2/Exhibition/sysinfo.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:37:33.000000 xhibit-9.5.2/LICENSE
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:42:34.076646 xhibit-9.5.2/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:37:33.000000 xhibit-9.5.2/README.md
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:42:34.076646 xhibit-9.5.2/setup.cfg
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     1054 2023-07-14 06:42:29.000000 xhibit-9.5.2/setup.py
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:42:34.076646 xhibit-9.5.2/xhibit.egg-info/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:42:34.000000 xhibit-9.5.2/xhibit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      380 2023-07-14 06:42:34.000000 xhibit-9.5.2/xhibit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:42:34.000000 xhibit-9.5.2/xhibit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:42:34.000000 xhibit-9.5.2/xhibit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:42:34.000000 xhibit-9.5.2/xhibit.egg-info/requires.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:42:34.000000 xhibit-9.5.2/xhibit.egg-info/top_level.txt
```

### Comparing `xhibit-9.5.1/Exhibition/__init__.py` & `xhibit-9.5.2/Exhibition/__init__.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/ascii.py` & `xhibit-9.5.2/Exhibition/ascii.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/color_palette.py` & `xhibit-9.5.2/Exhibition/color_palette.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/colors.py` & `xhibit-9.5.2/Exhibition/colors.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/image.py` & `xhibit-9.5.2/Exhibition/image.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/pos.sh` & `xhibit-9.5.2/Exhibition/pos.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/shell.sh` & `xhibit-9.5.2/Exhibition/shell.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/Exhibition/sysinfo.py` & `xhibit-9.5.2/Exhibition/sysinfo.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/LICENSE` & `xhibit-9.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/PKG-INFO` & `xhibit-9.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.5.1
+Version: 9.5.2
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `xhibit-9.5.1/README.md` & `xhibit-9.5.2/README.md`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.1/setup.py` & `xhibit-9.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhibit",
-    version="9.5.1",
+    version="9.5.2",
     author="glowfi",
     description="A python script to exhibit your ascii arts and sytem specs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/glowfi/xhibit",
     classifiers=[
@@ -22,10 +22,10 @@
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "xhibit=Exhibition.__init__:__init__",
         ]
     },
     install_requires=["tcolorpy"],
-    scripts=["./Exhibition/pos.sh", "./Exhibition/shell.sh"],
-    data_files=[('/usr/local/bin', ['./Exhibition/pos.sh', './Exhibition/shell.sh'])],
+    scripts=["Exhibition/pos.sh", "Exhibition/shell.sh"],
+    data_files=[('/usr/local/bin', ['Exhibition/pos.sh', 'Exhibition/shell.sh'])],
 )
```

### Comparing `xhibit-9.5.1/xhibit.egg-info/PKG-INFO` & `xhibit-9.5.2/xhibit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.5.1
+Version: 9.5.2
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

