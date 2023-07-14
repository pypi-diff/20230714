# Comparing `tmp/xhibit-9.2.0.tar.gz` & `tmp/xhibit-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhibit-9.2.0.tar", last modified: Fri Jul 14 06:05:49 2023, max compression
+gzip compressed data, was "xhibit-9.2.1.tar", last modified: Fri Jul 14 06:12:50 2023, max compression
```

## Comparing `xhibit-9.2.0.tar` & `xhibit-9.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:05:49.791782 xhibit-9.2.0/
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:05:49.791782 xhibit-9.2.0/Exhibition/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/__init__.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/ascii.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/color_palette.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/colors.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2736 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/image.py
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)     3866 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/pos.sh
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:04:38.000000 xhibit-9.2.0/Exhibition/shell.sh
--rw-r--r--   0 ayush     (1000) ayush     (1000)      728 2023-07-14 06:02:12.000000 xhibit-9.2.0/Exhibition/sysinfo.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:02:12.000000 xhibit-9.2.0/LICENSE
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3955 2023-07-14 06:05:49.791782 xhibit-9.2.0/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3401 2023-07-14 06:02:12.000000 xhibit-9.2.0/README.md
--rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:05:49.791782 xhibit-9.2.0/setup.cfg
--rw-r--r--   0 ayush     (1000) ayush     (1000)      975 2023-07-14 06:05:16.000000 xhibit-9.2.0/setup.py
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:05:49.791782 xhibit-9.2.0/xhibit.egg-info/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3955 2023-07-14 06:05:49.000000 xhibit-9.2.0/xhibit.egg-info/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:05:49.000000 xhibit-9.2.0/xhibit.egg-info/SOURCES.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:05:49.000000 xhibit-9.2.0/xhibit.egg-info/dependency_links.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:05:49.000000 xhibit-9.2.0/xhibit.egg-info/entry_points.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:05:49.000000 xhibit-9.2.0/xhibit.egg-info/requires.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:05:49.000000 xhibit-9.2.0/xhibit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:12:50.518768 xhibit-9.2.1/
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:12:50.518768 xhibit-9.2.1/Exhibition/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/__init__.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/ascii.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/color_palette.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/colors.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2736 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/image.py
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:12:31.000000 xhibit-9.2.1/Exhibition/pos.sh
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/shell.sh
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      730 2023-07-14 06:12:38.000000 xhibit-9.2.1/Exhibition/sysinfo.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:09:31.000000 xhibit-9.2.1/LICENSE
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3955 2023-07-14 06:12:50.518768 xhibit-9.2.1/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3401 2023-07-14 06:09:31.000000 xhibit-9.2.1/README.md
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:12:50.518768 xhibit-9.2.1/setup.cfg
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      975 2023-07-14 06:12:46.000000 xhibit-9.2.1/setup.py
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:12:50.518768 xhibit-9.2.1/xhibit.egg-info/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3955 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/requires.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/top_level.txt
```

### Comparing `xhibit-9.2.0/Exhibition/__init__.py` & `xhibit-9.2.1/Exhibition/__init__.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/Exhibition/ascii.py` & `xhibit-9.2.1/Exhibition/ascii.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/Exhibition/color_palette.py` & `xhibit-9.2.1/Exhibition/color_palette.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/Exhibition/colors.py` & `xhibit-9.2.1/Exhibition/colors.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/Exhibition/image.py` & `xhibit-9.2.1/Exhibition/image.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/Exhibition/shell.sh` & `xhibit-9.2.1/Exhibition/shell.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/Exhibition/sysinfo.py` & `xhibit-9.2.1/Exhibition/sysinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Getting Path
 shell_loc = os.path.realpath(__file__)
 ind = str(shell_loc).find(".local")
 shell_loc = f"{shell_loc[0:ind-1]}/.local/bin/shell.sh"
 
 # Running Shell script
-cmd = ["sh", f"{shell_loc}"]
+cmd = ["bash", f"{shell_loc}"]
 info = subprocess.run(cmd, stdout=subprocess.PIPE).stdout.decode("utf-8")
 info = str(info).split("\n")
 info.pop()
 
 
 def get_kernel():
     return info[1]
```

### Comparing `xhibit-9.2.0/LICENSE` & `xhibit-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/PKG-INFO` & `xhibit-9.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.2.0
+Version: 9.2.1
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `xhibit-9.2.0/README.md` & `xhibit-9.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.0/setup.py` & `xhibit-9.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhibit",
-    version="9.2.0",
+    version="9.2.1",
     author="glowfi",
     description="A python script to exhibit your ascii arts and sytem specs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/glowfi/xhibit",
     classifiers=[
```

### Comparing `xhibit-9.2.0/xhibit.egg-info/PKG-INFO` & `xhibit-9.2.1/xhibit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.2.0
+Version: 9.2.1
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

