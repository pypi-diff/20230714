# Comparing `tmp/torscrape-0.1.21.tar.gz` & `tmp/torscrape-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torscrape-0.1.21.tar", last modified: Fri Jul 14 01:10:38 2023, max compression
+gzip compressed data, was "torscrape-0.1.22.tar", last modified: Fri Jul 14 18:14:44 2023, max compression
```

## Comparing `torscrape-0.1.21.tar` & `torscrape-0.1.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 01:10:38.063536 torscrape-0.1.21/
--rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.21/LICENSE
--rw-rw-rw-   0        0        0     1931 2023-07-14 01:10:38.062535 torscrape-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.21/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 01:10:38.057535 torscrape-0.1.21/TorScrape/
--rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.21/TorScrape/__init__.py
--rw-rw-rw-   0        0        0     3344 2023-07-13 23:53:06.000000 torscrape-0.1.21/TorScrape/instaData.py
--rw-rw-rw-   0        0        0     9520 2023-07-14 01:10:17.000000 torscrape-0.1.21/TorScrape/tiktokData.py
--rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 01:10:38.063536 torscrape-0.1.21/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-07-14 01:10:24.000000 torscrape-0.1.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 01:10:38.061535 torscrape-0.1.21/torscrape.egg-info/
--rw-rw-rw-   0        0        0     1931 2023-07-14 01:10:38.000000 torscrape-0.1.21/torscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-14 01:10:38.000000 torscrape-0.1.21/torscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 01:10:38.000000 torscrape-0.1.21/torscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 01:10:38.000000 torscrape-0.1.21/torscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 01:10:38.000000 torscrape-0.1.21/torscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 18:14:44.198346 torscrape-0.1.22/
+-rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.22/LICENSE
+-rw-rw-rw-   0        0        0     1931 2023-07-14 18:14:44.198346 torscrape-0.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.22/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 18:14:44.193345 torscrape-0.1.22/TorScrape/
+-rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.22/TorScrape/__init__.py
+-rw-rw-rw-   0        0        0     3344 2023-07-13 23:53:06.000000 torscrape-0.1.22/TorScrape/instaData.py
+-rw-rw-rw-   0        0        0     9506 2023-07-14 18:14:08.000000 torscrape-0.1.22/TorScrape/tiktokData.py
+-rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 18:14:44.199346 torscrape-0.1.22/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-07-14 18:14:33.000000 torscrape-0.1.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:14:44.197346 torscrape-0.1.22/torscrape.egg-info/
+-rw-rw-rw-   0        0        0     1931 2023-07-14 18:14:44.000000 torscrape-0.1.22/torscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-14 18:14:44.000000 torscrape-0.1.22/torscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:14:44.000000 torscrape-0.1.22/torscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 18:14:44.000000 torscrape-0.1.22/torscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 18:14:44.000000 torscrape-0.1.22/torscrape.egg-info/top_level.txt
```

### Comparing `torscrape-0.1.21/LICENSE` & `torscrape-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.21/PKG-INFO` & `torscrape-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.21
+Version: 0.1.22
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torscrape-0.1.21/README.md` & `torscrape-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.21/TorScrape/instaData.py` & `torscrape-0.1.22/TorScrape/instaData.py`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.21/TorScrape/tiktokData.py` & `torscrape-0.1.22/TorScrape/tiktokData.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,23 +269,20 @@
     if not cached_data or not cached_data.get("following"):
         data: Dict = await get_profile_data(username)
         return data.get("following")
 
     return cached_data.get("following")
 
 
-async def latest_videos(username, count):
+async def latest_videos(username, count: int = 10):
     cached_data = check_profile(username)
     if not cached_data or not cached_data.get("videos"):
         result = await get_latest_videos(username, count)
         return result
 
     return cached_data.get("videos")
 
 
 async def all_videos(username: str):
     # TODO: Eventually check cache on all videos and return that instead of long running function
     result = await get_all_videos(username)
     return result
-
-
-all_videos("tiktok")
```

### Comparing `torscrape-0.1.21/setup.py` & `torscrape-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 # Get the absolute path to the requirements.txt file
 requirements_path = r"C:\Users\Tobias\Desktop\Webscrape_Course\Webscrape Course\requirements.txt"
 with open(requirements_path) as f:
     requirements = f.read().splitlines()
 
-version = '0.1.21'
+version = '0.1.22'
 
 setup(
     name='torscrape',
     version=version,
     author='Tore.ofc, rxality',
     author_email='tore.ofc.99@gmail.com',
     description='A webscrape package',
```

### Comparing `torscrape-0.1.21/torscrape.egg-info/PKG-INFO` & `torscrape-0.1.22/torscrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.21
+Version: 0.1.22
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

