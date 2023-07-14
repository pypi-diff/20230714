# Comparing `tmp/torscrape-0.1.18.tar.gz` & `tmp/torscrape-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torscrape-0.1.18.tar", last modified: Thu Jul 13 23:05:35 2023, max compression
+gzip compressed data, was "torscrape-0.1.2.tar", last modified: Fri Jul 14 01:02:28 2023, max compression
```

## Comparing `torscrape-0.1.18.tar` & `torscrape-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:05:35.349372 torscrape-0.1.18/
--rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.18/LICENSE
--rw-rw-rw-   0        0        0     1931 2023-07-13 23:05:35.349372 torscrape-0.1.18/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.18/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 23:05:35.344370 torscrape-0.1.18/TorScrape/
--rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.18/TorScrape/__init__.py
--rw-rw-rw-   0        0        0     2439 2023-07-11 18:06:04.000000 torscrape-0.1.18/TorScrape/instaData.py
--rw-rw-rw-   0        0        0     1308 2023-07-13 23:04:05.000000 torscrape-0.1.18/TorScrape/tiktokData.py
--rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 23:05:35.349372 torscrape-0.1.18/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-07-13 23:05:23.000000 torscrape-0.1.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:05:35.348371 torscrape-0.1.18/torscrape.egg-info/
--rw-rw-rw-   0        0        0     1931 2023-07-13 23:05:35.000000 torscrape-0.1.18/torscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-13 23:05:35.000000 torscrape-0.1.18/torscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:05:35.000000 torscrape-0.1.18/torscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-13 23:05:35.000000 torscrape-0.1.18/torscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 23:05:35.000000 torscrape-0.1.18/torscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:28.593873 torscrape-0.1.2/
+-rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1930 2023-07-14 01:02:28.593873 torscrape-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:28.588872 torscrape-0.1.2/TorScrape/
+-rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.2/TorScrape/__init__.py
+-rw-rw-rw-   0        0        0     3344 2023-07-13 23:53:06.000000 torscrape-0.1.2/TorScrape/instaData.py
+-rw-rw-rw-   0        0        0     9506 2023-07-14 01:02:04.000000 torscrape-0.1.2/TorScrape/tiktokData.py
+-rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 01:02:28.593873 torscrape-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-07-14 01:02:09.000000 torscrape-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:28.592872 torscrape-0.1.2/torscrape.egg-info/
+-rw-rw-rw-   0        0        0     1930 2023-07-14 01:02:28.000000 torscrape-0.1.2/torscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-14 01:02:28.000000 torscrape-0.1.2/torscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 01:02:28.000000 torscrape-0.1.2/torscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 01:02:28.000000 torscrape-0.1.2/torscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 01:02:28.000000 torscrape-0.1.2/torscrape.egg-info/top_level.txt
```

### Comparing `torscrape-0.1.18/LICENSE` & `torscrape-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.18/PKG-INFO` & `torscrape-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.18
+Version: 0.1.2
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torscrape-0.1.18/README.md` & `torscrape-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.18/TorScrape/instaData.py` & `torscrape-0.1.2/TorScrape/instaData.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import aiohttp
+import asyncio
 import requests
 from bs4 import BeautifulSoup
 
 def get_insta_followers(username):
     # Send a GET request to fetch the profile page
     response = requests.get(f"https://www.instagram.com/{username}/")
 
@@ -51,8 +53,33 @@
 
             # Extract the posts count from the meta description
             posts_count = meta_description.split("-")[0].strip().split(" ")[4]
             return posts_count
         except (KeyError, ValueError):
             return "Unable to fetch posts count."
     else:
-        return "Unable to fetch profile page. Please check the profile name."
+        return "Unable to fetch profile page. Please check the profile name."
+
+
+def search_insta_comments(username, keyword):
+    url = f"https://www.instagram.com/{username}/"
+
+    response = requests.get(url)
+    if response.ok:
+        soup = BeautifulSoup(response.text, "html.parser")
+        comments = soup.find_all("div", class_="_a9zo")
+
+        for comment in comments:
+            profile_picture = comment.find("img")["src"]
+            username = comment.find("a", class_="x1qjc9v5").text
+            comment_text = comment.find("span", class_="_aacl").text
+
+            if keyword in comment_text:
+                print(f"Profile Picture: {profile_picture}")
+                print(f"Username: {username}")
+                print(f"Comment: {comment_text}")
+                print()
+
+def get_insta_comment(username, keyword):
+    search_insta_comments(username, keyword)
+
+get_insta_comment("oskarwesterlin", "TOP")
```

### Comparing `torscrape-0.1.18/setup.py` & `torscrape-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 # Get the absolute path to the requirements.txt file
 requirements_path = r"C:\Users\Tobias\Desktop\Webscrape_Course\Webscrape Course\requirements.txt"
 with open(requirements_path) as f:
     requirements = f.read().splitlines()
 
-version = '0.1.18'
+version = '0.1.2'
 
 setup(
     name='torscrape',
     version=version,
     author='Tore.ofc, rxality',
     author_email='tore.ofc.99@gmail.com',
     description='A webscrape package',
```

### Comparing `torscrape-0.1.18/torscrape.egg-info/PKG-INFO` & `torscrape-0.1.2/torscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.18
+Version: 0.1.2
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

