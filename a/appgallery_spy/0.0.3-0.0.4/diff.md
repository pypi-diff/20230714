# Comparing `tmp/appgallery_spy-0.0.3.tar.gz` & `tmp/appgallery_spy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appgallery_spy-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "appgallery_spy-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `appgallery_spy-0.0.3.tar` & `appgallery_spy-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       50 2023-07-13 19:36:57.498942 appgallery_spy-0.0.3/.dockerignore
--rw-r--r--   0        0        0     3082 2023-07-14 16:00:38.011538 appgallery_spy-0.0.3/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 appgallery_spy-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      925 2023-07-13 19:15:59.819245 appgallery_spy-0.0.3/Dockerfile
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appgallery_spy-0.0.3/LICENSE
--rw-r--r--   0        0        0      369 2023-07-14 17:46:54.399112 appgallery_spy-0.0.3/Makefile
--rw-r--r--   0        0        0        0 2023-07-12 00:21:08.098160 appgallery_spy-0.0.3/README.md
--rw-r--r--   0        0        0       22 2023-07-14 17:53:38.062037 appgallery_spy-0.0.3/appgallery_spy/__init__.py
--rw-r--r--   0        0        0       28 2023-07-14 17:39:28.508878 appgallery_spy-0.0.3/appgallery_spy/__main__.py
--rw-r--r--   0        0        0      911 2023-07-14 17:39:28.528870 appgallery_spy-0.0.3/appgallery_spy/api.py
--rw-r--r--   0        0        0      247 2023-07-14 17:39:27.765186 appgallery_spy-0.0.3/appgallery_spy/cli.py
--rw-r--r--   0        0        0     2563 2023-07-14 17:39:43.935138 appgallery_spy-0.0.3/appgallery_spy/crawl.py
--rw-r--r--   0        0        0      735 2023-07-14 17:39:28.532868 appgallery_spy-0.0.3/appgallery_spy/crud.py
--rw-r--r--   0        0        0      219 2023-07-14 17:39:27.721205 appgallery_spy-0.0.3/appgallery_spy/models.py
--rwxr-xr-x   0        0        0 15039112 2023-05-27 00:10:14.000000 appgallery_spy-0.0.3/chromedriver
--rw-r--r--   0        0        0      409 2023-07-13 22:04:01.035978 appgallery_spy-0.0.3/docker-compose.yml
--rw-r--r--   0        0        0     2463 2023-07-14 17:53:26.242031 appgallery_spy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      249 2023-07-14 17:53:26.262031 appgallery_spy-0.0.3/requirements.txt
--rw-r--r--   0        0        0      193 2023-07-13 19:16:53.619566 appgallery_spy-0.0.3/setup.cfg
--rw-r--r--   0        0        0      114 2023-07-13 19:16:53.159564 appgallery_spy-0.0.3/test_build.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 appgallery_spy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-13 19:36:57.498942 appgallery_spy-0.0.4/.dockerignore
+-rw-r--r--   0        0        0     3082 2023-07-14 16:00:38.011538 appgallery_spy-0.0.4/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 appgallery_spy-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      925 2023-07-13 19:15:59.819245 appgallery_spy-0.0.4/Dockerfile
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appgallery_spy-0.0.4/LICENSE
+-rw-r--r--   0        0        0      369 2023-07-14 17:46:54.399112 appgallery_spy-0.0.4/Makefile
+-rw-r--r--   0        0        0        0 2023-07-12 00:21:08.098160 appgallery_spy-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2023-07-14 18:11:06.902648 appgallery_spy-0.0.4/appgallery_spy/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-14 17:39:28.508878 appgallery_spy-0.0.4/appgallery_spy/__main__.py
+-rw-r--r--   0        0        0      911 2023-07-14 17:39:28.528870 appgallery_spy-0.0.4/appgallery_spy/api.py
+-rw-r--r--   0        0        0      247 2023-07-14 17:39:27.765186 appgallery_spy-0.0.4/appgallery_spy/cli.py
+-rw-r--r--   0        0        0     2829 2023-07-14 18:09:57.578670 appgallery_spy-0.0.4/appgallery_spy/crawl.py
+-rw-r--r--   0        0        0      836 2023-07-14 18:09:53.552911 appgallery_spy-0.0.4/appgallery_spy/crud.py
+-rw-r--r--   0        0        0      219 2023-07-14 17:39:27.721205 appgallery_spy-0.0.4/appgallery_spy/models.py
+-rwxr-xr-x   0        0        0 15039112 2023-05-27 00:10:14.000000 appgallery_spy-0.0.4/chromedriver
+-rw-r--r--   0        0        0      409 2023-07-13 22:04:01.035978 appgallery_spy-0.0.4/docker-compose.yml
+-rw-r--r--   0        0        0     2463 2023-07-14 17:53:26.242031 appgallery_spy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-14 17:53:26.262031 appgallery_spy-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      193 2023-07-13 19:16:53.619566 appgallery_spy-0.0.4/setup.cfg
+-rw-r--r--   0        0        0      114 2023-07-13 19:16:53.159564 appgallery_spy-0.0.4/test_build.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 appgallery_spy-0.0.4/PKG-INFO
```

### Comparing `appgallery_spy-0.0.3/.gitignore` & `appgallery_spy-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.3/Dockerfile` & `appgallery_spy-0.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.3/LICENSE` & `appgallery_spy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.3/appgallery_spy/api.py` & `appgallery_spy-0.0.4/appgallery_spy/api.py`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.3/appgallery_spy/crawl.py` & `appgallery_spy-0.0.4/appgallery_spy/crawl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import pathlib
 from time import sleep
 
 from bs4 import BeautifulSoup
+from pymongo.errors import ServerSelectionTimeoutError
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 
+from appgallery_spy import crud
+
 COMMENT_ITEMS_LOCATORS = (
     "body > div > div.box > div > div.componentContainer > div.CommentList > div.listContainer > div.comment_item"
 )
 VIEW_ALL_BTN = (By.CSS_SELECTOR, "div.pcscorecommentlistcard span[data-v-892a7f08]")
 USERNAME_SELECTOR = "div.userName"
 DATE_SELECTOR = "div.right > div.part_top > div > div.deviceName > div"
 COMMENT_SELECTOR = "div.right > div"
@@ -65,9 +68,16 @@
 
 def crawl(app_id: str) -> None:
     driver = driver_setup(app_id)
     click_view_all(driver)
     html = load_source(driver)
     soup = BeautifulSoup(html, "html.parser")
     reviews_data = get_comment_items(soup)
-    print(reviews_data)
+
+    try:
+        crud.insert_data(reviews_data)
+    except ServerSelectionTimeoutError as e:
+        print("ServerSelectionTimeoutError:", e)
+    except Exception as e:
+        print("Exception:", e)
+
     driver.quit()
```

### Comparing `appgallery_spy-0.0.3/appgallery_spy/crud.py` & `appgallery_spy-0.0.4/appgallery_spy/crud.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,11 +18,14 @@
         )
         for review in recent_reviews
     ]
 
     return reviews
 
 
-def insert_data(data: list[dict], reviews_collection) -> None:
+def insert_data(data: list[dict], reviews_collection=None) -> None:
+    if not reviews_collection:
+        db = get_db()
+        reviews_collection = db["reviews"]
     print("Saving data...")
     reviews_collection.insert_many(data)
     print("Data is saved.")
```

### Comparing `appgallery_spy-0.0.3/chromedriver` & `appgallery_spy-0.0.4/chromedriver`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.3/pyproject.toml` & `appgallery_spy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appgallery_spy-0.0.3/PKG-INFO` & `appgallery_spy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appgallery_spy
-Version: 0.0.3
+Version: 0.0.4
 Summary: appgallery_spy - Huauwi AppGallery Crawler
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

