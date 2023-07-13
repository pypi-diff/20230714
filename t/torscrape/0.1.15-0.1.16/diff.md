# Comparing `tmp/torscrape-0.1.15.tar.gz` & `tmp/torscrape-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torscrape-0.1.15.tar", last modified: Thu Jul 13 22:44:23 2023, max compression
+gzip compressed data, was "torscrape-0.1.16.tar", last modified: Thu Jul 13 22:48:08 2023, max compression
```

## Comparing `torscrape-0.1.15.tar` & `torscrape-0.1.16.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:23.706360 torscrape-0.1.15/
--rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.15/LICENSE
--rw-rw-rw-   0        0        0     1931 2023-07-13 22:44:23.705360 torscrape-0.1.15/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.15/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:23.700358 torscrape-0.1.15/TorScrape/
--rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.15/TorScrape/__init__.py
--rw-rw-rw-   0        0        0     2439 2023-07-11 18:06:04.000000 torscrape-0.1.15/TorScrape/instaData.py
--rw-rw-rw-   0        0        0     1240 2023-07-13 22:44:03.000000 torscrape-0.1.15/TorScrape/tiktokData.py
--rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 22:44:23.706360 torscrape-0.1.15/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-07-13 22:44:09.000000 torscrape-0.1.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:44:23.704359 torscrape-0.1.15/torscrape.egg-info/
--rw-rw-rw-   0        0        0     1931 2023-07-13 22:44:23.000000 torscrape-0.1.15/torscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-13 22:44:23.000000 torscrape-0.1.15/torscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 22:44:23.000000 torscrape-0.1.15/torscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-13 22:44:23.000000 torscrape-0.1.15/torscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 22:44:23.000000 torscrape-0.1.15/torscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 22:48:08.329685 torscrape-0.1.16/
+-rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.16/LICENSE
+-rw-rw-rw-   0        0        0     1931 2023-07-13 22:48:08.328684 torscrape-0.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.16/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 22:48:08.322683 torscrape-0.1.16/TorScrape/
+-rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.16/TorScrape/__init__.py
+-rw-rw-rw-   0        0        0     2439 2023-07-11 18:06:04.000000 torscrape-0.1.16/TorScrape/instaData.py
+-rw-rw-rw-   0        0        0     1240 2023-07-13 22:47:49.000000 torscrape-0.1.16/TorScrape/tiktokData.py
+-rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.16/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 22:48:08.329685 torscrape-0.1.16/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-07-13 22:47:55.000000 torscrape-0.1.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:48:08.327684 torscrape-0.1.16/torscrape.egg-info/
+-rw-rw-rw-   0        0        0     1931 2023-07-13 22:48:08.000000 torscrape-0.1.16/torscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-13 22:48:08.000000 torscrape-0.1.16/torscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 22:48:08.000000 torscrape-0.1.16/torscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-13 22:48:08.000000 torscrape-0.1.16/torscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 22:48:08.000000 torscrape-0.1.16/torscrape.egg-info/top_level.txt
```

### Comparing `torscrape-0.1.15/LICENSE` & `torscrape-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.15/PKG-INFO` & `torscrape-0.1.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.15
+Version: 0.1.16
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torscrape-0.1.15/README.md` & `torscrape-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.15/TorScrape/instaData.py` & `torscrape-0.1.16/TorScrape/instaData.py`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.15/TorScrape/tiktokData.py` & `torscrape-0.1.16/TorScrape/tiktokData.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import aiohttp
 import asyncio
 import json
 from bs4 import BeautifulSoup
 
 url = "https://www.tiktok.com/@"
-
 suffix = "/video/"
 
 async def latest_links(username, count):
     async with aiohttp.ClientSession() as session:
         async with session.get(url + username) as response:
             html = await response.text()
 
@@ -41,8 +40,8 @@
     pass
 
 def profileUrl(username):
     pass
 
 
 async def get_latest_vid_links(username, count):
-    await latest_links(username, count)
+    await latest_links(username, count)
```

### Comparing `torscrape-0.1.15/setup.py` & `torscrape-0.1.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 # Get the absolute path to the requirements.txt file
 requirements_path = r"C:\Users\Tobias\Desktop\Webscrape_Course\Webscrape Course\requirements.txt"
 with open(requirements_path) as f:
     requirements = f.read().splitlines()
 
-version = '0.1.15'
+version = '0.1.16'
 
 setup(
     name='torscrape',
     version=version,
     author='Tore.ofc, rxality',
     author_email='tore.ofc.99@gmail.com',
     description='A webscrape package',
```

### Comparing `torscrape-0.1.15/torscrape.egg-info/PKG-INFO` & `torscrape-0.1.16/torscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.15
+Version: 0.1.16
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

