# Comparing `tmp/jaime38130-0.3.tar.gz` & `tmp/jaime38130-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaime38130-0.3.tar", last modified: Fri Jul 14 21:30:16 2023, max compression
+gzip compressed data, was "dist\jaime38130-0.4.tar", last modified: Fri Jul 14 21:40:58 2023, max compression
```

## Comparing `jaime38130-0.3.tar` & `jaime38130-0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 21:30:16.000000 jaime38130-0.3/
--rw-rw-rw-   0        0        0      870 2023-07-14 21:30:16.000000 jaime38130-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 21:30:16.000000 jaime38130-0.3/jaime38130/
--rw-rw-rw-   0        0        0       49 2023-07-14 20:04:50.000000 jaime38130-0.3/jaime38130/__init__.py
--rw-rw-rw-   0        0        0     1223 2023-07-14 21:24:42.000000 jaime38130-0.3/jaime38130/script_python.py
--rw-rw-rw-   0        0        0       65 2023-07-14 20:16:59.000000 jaime38130-0.3/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-07-14 21:29:54.000000 jaime38130-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:40:58.000000 jaime38130-0.4/
+-rw-rw-rw-   0        0        0      870 2023-07-14 21:40:58.000000 jaime38130-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 21:40:58.000000 jaime38130-0.4/jaime38130/
+-rw-rw-rw-   0        0        0       49 2023-07-14 20:04:50.000000 jaime38130-0.4/jaime38130/__init__.py
+-rw-rw-rw-   0        0        0     1223 2023-07-14 21:24:42.000000 jaime38130-0.4/jaime38130/script_python.py
+-rw-rw-rw-   0        0        0       65 2023-07-14 20:16:59.000000 jaime38130-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-07-14 21:39:33.000000 jaime38130-0.4/setup.py
```

### Comparing `jaime38130-0.3/PKG-INFO` & `jaime38130-0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: jaime38130
-Version: 0.3
+Version: 0.4
 Summary: Colors!
 Home-page: https://github.com/JaimeSilva/jaime38130.git
 Author: Jaime Silva
 Author-email: jaimedcsilva@hotmail.com
 License: -
-Download-URL: https://github.com/JaimeSilva/jaime38130/archive/refs/tags/v_03.tar.gz
+Download-URL: https://github.com/JaimeSilva/jaime38130/archive/refs/tags/v_04.tar.gz
 Description: UNKNOWN
 Keywords: SOME,MEANINGFULL,COLORS
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaime38130-0.3/jaime38130/script_python.py` & `jaime38130-0.4/jaime38130/script_python.py`

 * *Files identical despite different names*

### Comparing `jaime38130-0.3/setup.py` & `jaime38130-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'jaime38130',
   packages = ['jaime38130'],
-  version = '0.3',
+  version = '0.4',
   license='-',
   description = 'Colors!',
   author = 'Jaime Silva',
   author_email = 'jaimedcsilva@hotmail.com',
   url = 'https://github.com/JaimeSilva/jaime38130.git',
-  download_url = 'https://github.com/JaimeSilva/jaime38130/archive/refs/tags/v_03.tar.gz',
+  download_url = 'https://github.com/JaimeSilva/jaime38130/archive/refs/tags/v_04.tar.gz',
   keywords = ['SOME', 'MEANINGFULL', 'COLORS'],
   install_requires=[
           'colorama',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

