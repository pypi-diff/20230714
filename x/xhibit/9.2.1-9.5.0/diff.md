# Comparing `tmp/xhibit-9.2.1.tar.gz` & `tmp/xhibit-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhibit-9.2.1.tar", last modified: Fri Jul 14 06:12:50 2023, max compression
+gzip compressed data, was "xhibit-9.5.0.tar", last modified: Fri Jul 14 06:33:45 2023, max compression
```

## Comparing `xhibit-9.2.1.tar` & `xhibit-9.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:12:50.518768 xhibit-9.2.1/
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:12:50.518768 xhibit-9.2.1/Exhibition/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/__init__.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/ascii.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/color_palette.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/colors.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2736 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/image.py
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:12:31.000000 xhibit-9.2.1/Exhibition/pos.sh
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:09:31.000000 xhibit-9.2.1/Exhibition/shell.sh
--rw-r--r--   0 ayush     (1000) ayush     (1000)      730 2023-07-14 06:12:38.000000 xhibit-9.2.1/Exhibition/sysinfo.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:09:31.000000 xhibit-9.2.1/LICENSE
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3955 2023-07-14 06:12:50.518768 xhibit-9.2.1/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3401 2023-07-14 06:09:31.000000 xhibit-9.2.1/README.md
--rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:12:50.518768 xhibit-9.2.1/setup.cfg
--rw-r--r--   0 ayush     (1000) ayush     (1000)      975 2023-07-14 06:12:46.000000 xhibit-9.2.1/setup.py
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:12:50.518768 xhibit-9.2.1/xhibit.egg-info/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3955 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/SOURCES.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/dependency_links.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/entry_points.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/requires.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:12:50.000000 xhibit-9.2.1/xhibit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:33:45.535184 xhibit-9.5.0/
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:33:45.534185 xhibit-9.5.0/Exhibition/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:16:51.000000 xhibit-9.5.0/Exhibition/__init__.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:16:51.000000 xhibit-9.5.0/Exhibition/ascii.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:16:51.000000 xhibit-9.5.0/Exhibition/color_palette.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:16:51.000000 xhibit-9.5.0/Exhibition/colors.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2641 2023-07-14 06:32:08.000000 xhibit-9.5.0/Exhibition/image.py
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:16:51.000000 xhibit-9.5.0/Exhibition/pos.sh
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:16:51.000000 xhibit-9.5.0/Exhibition/shell.sh
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      627 2023-07-14 06:31:44.000000 xhibit-9.5.0/Exhibition/sysinfo.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:16:51.000000 xhibit-9.5.0/LICENSE
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:33:45.535184 xhibit-9.5.0/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:33:31.000000 xhibit-9.5.0/README.md
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 06:33:45.535184 xhibit-9.5.0/setup.cfg
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      975 2023-07-14 06:33:43.000000 xhibit-9.5.0/setup.py
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 06:33:45.535184 xhibit-9.5.0/xhibit.egg-info/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 06:33:45.000000 xhibit-9.5.0/xhibit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 06:33:45.000000 xhibit-9.5.0/xhibit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 06:33:45.000000 xhibit-9.5.0/xhibit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 06:33:45.000000 xhibit-9.5.0/xhibit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 06:33:45.000000 xhibit-9.5.0/xhibit.egg-info/requires.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 06:33:45.000000 xhibit-9.5.0/xhibit.egg-info/top_level.txt
```

### Comparing `xhibit-9.2.1/Exhibition/__init__.py` & `xhibit-9.5.0/Exhibition/__init__.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/Exhibition/ascii.py` & `xhibit-9.5.0/Exhibition/ascii.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/Exhibition/color_palette.py` & `xhibit-9.5.0/Exhibition/color_palette.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/Exhibition/colors.py` & `xhibit-9.5.0/Exhibition/colors.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/Exhibition/image.py` & `xhibit-9.5.0/Exhibition/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,15 @@
 def display_image(image_path, info, field_colors, image_backend, cropMode, choice):
 
     # Print ascii first for ueberzug
     if image_backend == "ueberzug":
         print_(info, field_colors, choice, image_path)
 
     # Getting Path
-    pos_loc = os.path.realpath(__file__)
-    ind = str(pos_loc).find(".local")
-    pos_loc = f"{pos_loc[0:ind-1]}/.local/bin/pos.sh"
+    pos_loc = "/usr/local/bin/pos.sh"
 
     # Running Shell script
     call_with_args = f"{pos_loc} {image_path} {image_backend} {cropMode}"
     os.system(call_with_args)
 
     # Print ascii last for kitty
     if image_backend == "kitty":
```

### Comparing `xhibit-9.2.1/Exhibition/pos.sh` & `xhibit-9.5.0/Exhibition/pos.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/Exhibition/shell.sh` & `xhibit-9.5.0/Exhibition/shell.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/Exhibition/sysinfo.py` & `xhibit-9.5.0/Exhibition/sysinfo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import os
 import subprocess
 
 # Getting Path
-shell_loc = os.path.realpath(__file__)
-ind = str(shell_loc).find(".local")
-shell_loc = f"{shell_loc[0:ind-1]}/.local/bin/shell.sh"
+shell_loc = "/usr/local/bin/shell.sh"
 
 # Running Shell script
 cmd = ["bash", f"{shell_loc}"]
 info = subprocess.run(cmd, stdout=subprocess.PIPE).stdout.decode("utf-8")
 info = str(info).split("\n")
 info.pop()
```

### Comparing `xhibit-9.2.1/LICENSE` & `xhibit-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xhibit-9.2.1/PKG-INFO` & `xhibit-9.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.2.1
+Version: 9.5.0
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -21,16 +21,18 @@
   <img src="https://raw.githubusercontent.com/glowfi/xhibit/main/image_support.png" />
 </p>
 
 ### This is an alpha software. It requires more testing.
 
 ### INSTALLATION
 
+Use sudo or doas to install this package.
+
 ```
-pip install xhibit
+sudo pip install xhibit
 ```
 
 ### DEPENDENCIES
 
 **For Ascii art only**
 
 -   **python 3.5+**
```

### Comparing `xhibit-9.2.1/README.md` & `xhibit-9.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,18 @@
   <img src="https://raw.githubusercontent.com/glowfi/xhibit/main/image_support.png" />
 </p>
 
 ### This is an alpha software. It requires more testing.
 
 ### INSTALLATION
 
+Use sudo or doas to install this package.
+
 ```
-pip install xhibit
+sudo pip install xhibit
 ```
 
 ### DEPENDENCIES
 
 **For Ascii art only**
 
 -   **python 3.5+**
```

### Comparing `xhibit-9.2.1/setup.py` & `xhibit-9.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhibit",
-    version="9.2.1",
+    version="9.5.0",
     author="glowfi",
     description="A python script to exhibit your ascii arts and sytem specs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/glowfi/xhibit",
     classifiers=[
```

### Comparing `xhibit-9.2.1/xhibit.egg-info/PKG-INFO` & `xhibit-9.5.0/xhibit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.2.1
+Version: 9.5.0
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -21,16 +21,18 @@
   <img src="https://raw.githubusercontent.com/glowfi/xhibit/main/image_support.png" />
 </p>
 
 ### This is an alpha software. It requires more testing.
 
 ### INSTALLATION
 
+Use sudo or doas to install this package.
+
 ```
-pip install xhibit
+sudo pip install xhibit
 ```
 
 ### DEPENDENCIES
 
 **For Ascii art only**
 
 -   **python 3.5+**
```

