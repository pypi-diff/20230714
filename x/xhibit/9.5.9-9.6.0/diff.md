# Comparing `tmp/xhibit-9.5.9.tar.gz` & `tmp/xhibit-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhibit-9.5.9.tar", last modified: Fri Jul 14 07:13:03 2023, max compression
+gzip compressed data, was "xhibit-9.6.0.tar", last modified: Fri Jul 14 07:17:34 2023, max compression
```

## Comparing `xhibit-9.5.9.tar` & `xhibit-9.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 07:13:03.274205 xhibit-9.5.9/
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 07:13:03.273205 xhibit-9.5.9/Exhibition/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/__init__.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/ascii.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/color_palette.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/colors.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)     2641 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/image.py
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/pos.sh
--rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/shell.sh
--rw-r--r--   0 ayush     (1000) ayush     (1000)      627 2023-07-14 06:37:33.000000 xhibit-9.5.9/Exhibition/sysinfo.py
--rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:37:33.000000 xhibit-9.5.9/LICENSE
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 07:13:03.274205 xhibit-9.5.9/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:37:33.000000 xhibit-9.5.9/README.md
--rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 07:13:03.274205 xhibit-9.5.9/setup.cfg
--rw-r--r--   0 ayush     (1000) ayush     (1000)     1044 2023-07-14 07:13:02.000000 xhibit-9.5.9/setup.py
-drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 07:13:03.274205 xhibit-9.5.9/xhibit.egg-info/
--rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 07:13:03.000000 xhibit-9.5.9/xhibit.egg-info/PKG-INFO
--rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 07:13:03.000000 xhibit-9.5.9/xhibit.egg-info/SOURCES.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 07:13:03.000000 xhibit-9.5.9/xhibit.egg-info/dependency_links.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 07:13:03.000000 xhibit-9.5.9/xhibit.egg-info/entry_points.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 07:13:03.000000 xhibit-9.5.9/xhibit.egg-info/requires.txt
--rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 07:13:03.000000 xhibit-9.5.9/xhibit.egg-info/top_level.txt
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 07:17:34.263194 xhibit-9.6.0/
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 07:17:34.262194 xhibit-9.6.0/Exhibition/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     6472 2023-07-14 06:37:33.000000 xhibit-9.6.0/Exhibition/__init__.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    11945 2023-07-14 06:37:33.000000 xhibit-9.6.0/Exhibition/ascii.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2364 2023-07-14 06:37:33.000000 xhibit-9.6.0/Exhibition/color_palette.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    37691 2023-07-14 06:37:33.000000 xhibit-9.6.0/Exhibition/colors.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     2644 2023-07-14 07:15:08.000000 xhibit-9.6.0/Exhibition/image.py
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)     4812 2023-07-14 06:37:33.000000 xhibit-9.6.0/Exhibition/pos.sh
+-rwxr-xr-x   0 ayush     (1000) ayush     (1000)    15892 2023-07-14 06:37:33.000000 xhibit-9.6.0/Exhibition/shell.sh
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      631 2023-07-14 07:16:15.000000 xhibit-9.6.0/Exhibition/sysinfo.py
+-rw-r--r--   0 ayush     (1000) ayush     (1000)    35149 2023-07-14 06:37:33.000000 xhibit-9.6.0/LICENSE
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 07:17:34.263194 xhibit-9.6.0/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     3449 2023-07-14 06:37:33.000000 xhibit-9.6.0/README.md
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       38 2023-07-14 07:17:34.263194 xhibit-9.6.0/setup.cfg
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     1044 2023-07-14 07:17:28.000000 xhibit-9.6.0/setup.py
+drwxr-xr-x   0 ayush     (1000) ayush     (1000)        0 2023-07-14 07:17:34.263194 xhibit-9.6.0/xhibit.egg-info/
+-rw-r--r--   0 ayush     (1000) ayush     (1000)     4003 2023-07-14 07:17:34.000000 xhibit-9.6.0/xhibit.egg-info/PKG-INFO
+-rw-r--r--   0 ayush     (1000) ayush     (1000)      384 2023-07-14 07:17:34.000000 xhibit-9.6.0/xhibit.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        1 2023-07-14 07:17:34.000000 xhibit-9.6.0/xhibit.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       56 2023-07-14 07:17:34.000000 xhibit-9.6.0/xhibit.egg-info/entry_points.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)        9 2023-07-14 07:17:34.000000 xhibit-9.6.0/xhibit.egg-info/requires.txt
+-rw-r--r--   0 ayush     (1000) ayush     (1000)       11 2023-07-14 07:17:34.000000 xhibit-9.6.0/xhibit.egg-info/top_level.txt
```

### Comparing `xhibit-9.5.9/Exhibition/__init__.py` & `xhibit-9.6.0/Exhibition/__init__.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/Exhibition/ascii.py` & `xhibit-9.6.0/Exhibition/ascii.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/Exhibition/color_palette.py` & `xhibit-9.6.0/Exhibition/color_palette.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/Exhibition/colors.py` & `xhibit-9.6.0/Exhibition/colors.py`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/Exhibition/image.py` & `xhibit-9.6.0/Exhibition/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,21 +45,20 @@
     )
     print(
         tcolor(f"{spc}{username}@{host}     ", color=field_colors[2], styles=["bold"])
     )
 
 
 def display_image(image_path, info, field_colors, image_backend, cropMode, choice):
-
     # Print ascii first for ueberzug
     if image_backend == "ueberzug":
         print_(info, field_colors, choice, image_path)
 
     # Getting Path
-    pos_loc = "/usr/local/bin/pos.sh"
+    pos_loc = "/usr/xhibitscripts/pos.sh"
 
     # Running Shell script
     call_with_args = f"{pos_loc} {image_path} {image_backend} {cropMode}"
     os.system(call_with_args)
 
     # Print ascii last for kitty
     if image_backend == "kitty":
```

### Comparing `xhibit-9.5.9/Exhibition/pos.sh` & `xhibit-9.6.0/Exhibition/pos.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/Exhibition/shell.sh` & `xhibit-9.6.0/Exhibition/shell.sh`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/Exhibition/sysinfo.py` & `xhibit-9.6.0/Exhibition/sysinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 
 # Getting Path
-shell_loc = "/usr/local/bin/shell.sh"
+shell_loc = "/usr/xhibitscripts/shell.sh"
 
 # Running Shell script
 cmd = ["bash", f"{shell_loc}"]
 info = subprocess.run(cmd, stdout=subprocess.PIPE).stdout.decode("utf-8")
 info = str(info).split("\n")
 info.pop()
```

### Comparing `xhibit-9.5.9/LICENSE` & `xhibit-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/PKG-INFO` & `xhibit-9.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.5.9
+Version: 9.6.0
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `xhibit-9.5.9/README.md` & `xhibit-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `xhibit-9.5.9/setup.py` & `xhibit-9.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xhibit",
-    version="9.5.9",
+    version="9.6.0",
     author="glowfi",
     description="A python script to exhibit your ascii arts and sytem specs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/glowfi/xhibit",
     classifiers=[
```

### Comparing `xhibit-9.5.9/xhibit.egg-info/PKG-INFO` & `xhibit-9.6.0/xhibit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhibit
-Version: 9.5.9
+Version: 9.6.0
 Summary: A python script to exhibit your ascii arts and sytem specs
 Home-page: https://github.com/glowfi/xhibit
 Author: glowfi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

