# Comparing `tmp/nordvpn-tray-1.0.6.tar.gz` & `tmp/nordvpn-tray-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordvpn-tray-1.0.6.tar", last modified: Thu Jul 13 22:54:25 2023, max compression
+gzip compressed data, was "nordvpn-tray-1.0.7.tar", last modified: Thu Jul 13 22:56:11 2023, max compression
```

## Comparing `nordvpn-tray-1.0.6.tar` & `nordvpn-tray-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 22:54:25.393237 nordvpn-tray-1.0.6/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     4531 2023-07-13 22:54:25.387238 nordvpn-tray-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2023-07-13 19:16:01.000000 nordvpn-tray-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 22:54:25.394238 nordvpn-tray-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2517 2023-07-13 19:17:24.000000 nordvpn-tray-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:54:25.346687 nordvpn-tray-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 22:54:25.360687 nordvpn-tray-1.0.6/src/nordvpn_tray/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.6/src/nordvpn_tray/__init__.py
--rw-rw-rw-   0        0        0     6342 2023-07-13 18:59:04.000000 nordvpn-tray-1.0.6/src/nordvpn_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:54:25.383708 nordvpn-tray-1.0.6/src/nordvpn_tray/resources/
--rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.6/src/nordvpn_tray/resources/nvt.ico
-drwxrwxrwx   0        0        0        0 2023-07-13 22:54:25.381709 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/
--rw-rw-rw-   0        0        0     4531 2023-07-13 22:54:25.000000 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-13 22:54:25.000000 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 22:54:25.000000 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-13 22:54:25.000000 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-07-13 22:54:25.000000 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 22:54:25.000000 nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.680185 nordvpn-tray-1.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4531 2023-07-13 22:56:11.675166 nordvpn-tray-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2023-07-13 22:56:08.000000 nordvpn-tray-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 22:56:11.681166 nordvpn-tray-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2517 2023-07-13 22:56:08.000000 nordvpn-tray-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.635003 nordvpn-tray-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.648133 nordvpn-tray-1.0.7/src/nordvpn_tray/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.7/src/nordvpn_tray/__init__.py
+-rw-rw-rw-   0        0        0     6342 2023-07-13 18:59:04.000000 nordvpn-tray-1.0.7/src/nordvpn_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.671166 nordvpn-tray-1.0.7/src/nordvpn_tray/resources/
+-rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.7/src/nordvpn_tray/resources/nvt.ico
+drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.669166 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/
+-rw-rw-rw-   0        0        0     4531 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/top_level.txt
```

### Comparing `nordvpn-tray-1.0.6/LICENSE` & `nordvpn-tray-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.6/PKG-INFO` & `nordvpn-tray-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.6
+Version: 1.0.7
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
@@ -40,15 +40,15 @@
 
 ## Preview
 
 <img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.8 or higher
 
 ## Installation
 
 To install NordVPN Tray, run the following command:
 
     pip install nordvpn-tray
```

### Comparing `nordvpn-tray-1.0.6/README.md` & `nordvpn-tray-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ## Preview
 
 <img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.8 or higher
 
 ## Installation
 
 To install NordVPN Tray, run the following command:
 
     pip install nordvpn-tray
```

### Comparing `nordvpn-tray-1.0.6/setup.py` & `nordvpn-tray-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='nordvpn-tray',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "nordvpn_tray": ["*.py"],
         "nordvpn_tray.resources": ["*.ico"],
     },
     description='A cross-platform system tray application for interacting with NordVPN.',
```

### Comparing `nordvpn-tray-1.0.6/src/nordvpn_tray/__main__.py` & `nordvpn-tray-1.0.7/src/nordvpn_tray/__main__.py`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.6/src/nordvpn_tray/resources/nvt.ico` & `nordvpn-tray-1.0.7/src/nordvpn_tray/resources/nvt.ico`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.6/src/nordvpn_tray.egg-info/PKG-INFO` & `nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.6
+Version: 1.0.7
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
@@ -40,15 +40,15 @@
 
 ## Preview
 
 <img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.8 or higher
 
 ## Installation
 
 To install NordVPN Tray, run the following command:
 
     pip install nordvpn-tray
```

