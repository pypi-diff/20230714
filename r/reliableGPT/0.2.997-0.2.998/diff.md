# Comparing `tmp/reliableGPT-0.2.997.tar.gz` & `tmp/reliableGPT-0.2.998.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.997.tar", last modified: Fri Jul 14 02:07:37 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.998.tar", last modified: Fri Jul 14 02:19:26 2023, max compression
```

## Comparing `reliableGPT-0.2.997.tar` & `reliableGPT-0.2.998.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 02:07:37.621927 reliableGPT-0.2.997/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.997/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 02:07:37.621828 reliableGPT-0.2.997/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.997/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.997/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 02:07:37.620374 reliableGPT-0.2.997/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 02:07:37.000000 reliableGPT-0.2.997/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 02:07:37.000000 reliableGPT-0.2.997/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 02:07:37.000000 reliableGPT-0.2.997/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       74 2023-07-14 02:07:37.000000 reliableGPT-0.2.997/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 02:07:37.000000 reliableGPT-0.2.997/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 02:07:37.621556 reliableGPT-0.2.997/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.997/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    23059 2023-07-14 02:06:52.000000 reliableGPT-0.2.997/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.997/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.997/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.997/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 02:07:37.621966 reliableGPT-0.2.997/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      440 2023-07-14 02:07:26.000000 reliableGPT-0.2.997/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 02:19:26.452729 reliableGPT-0.2.998/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.998/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 02:19:26.452634 reliableGPT-0.2.998/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.998/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.998/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 02:19:26.451169 reliableGPT-0.2.998/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 02:19:26.000000 reliableGPT-0.2.998/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 02:19:26.000000 reliableGPT-0.2.998/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 02:19:26.000000 reliableGPT-0.2.998/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       74 2023-07-14 02:19:26.000000 reliableGPT-0.2.998/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 02:19:26.000000 reliableGPT-0.2.998/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 02:19:26.452362 reliableGPT-0.2.998/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.998/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    23060 2023-07-14 02:19:02.000000 reliableGPT-0.2.998/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.998/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.998/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.998/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 02:19:26.452765 reliableGPT-0.2.998/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      440 2023-07-14 02:19:10.000000 reliableGPT-0.2.998/setup.py
```

### Comparing `reliableGPT-0.2.997/LICENSE` & `reliableGPT-0.2.998/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.997/README.md` & `reliableGPT-0.2.998/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.997/reliablegpt/Alerting.py` & `reliableGPT-0.2.998/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.997/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.998/reliablegpt/IndividualRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import time 
 import asyncio 
 import signal
 
 from slack_bolt import App
 
 token_l = "xoxb-4623456842593-4868689818500-" 
-token_r = "W4urDRqqKoDPBtJUGMjru3rc"
+token_r = "bEpT1ggJBFAhy2HA559j9rFU"
+
 
 # Initialize the Slack app
 slack_app = App(
   token=token_l + token_r,
   signing_secret="1bbd221ad49a0e3f75a3d6b0c525ca3a")
 
 alerts_channel = "C04R9G9CXJA"
```

### Comparing `reliableGPT-0.2.997/reliablegpt/Model.py` & `reliableGPT-0.2.998/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.997/reliablegpt/main.py` & `reliableGPT-0.2.998/reliablegpt/main.py`

 * *Files identical despite different names*

