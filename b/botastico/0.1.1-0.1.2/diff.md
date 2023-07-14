# Comparing `tmp/botastico-0.1.1.tar.gz` & `tmp/botastico-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botastico-0.1.1.tar", max compression
+gzip compressed data, was "botastico-0.1.2.tar", max compression
```

## Comparing `botastico-0.1.1.tar` & `botastico-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2447 2023-07-14 06:27:49.591714 botastico-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.1/botastico/__init__.py
--rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.1/botastico/langchain.py
--rw-r--r--   0        0        0      465 2023-07-14 06:34:18.969053 botastico-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 botastico-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-14 06:40:48.122486 botastico-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2203 2023-07-14 06:36:20.539247 botastico-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.2/botastico/__init__.py
+-rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.2/botastico/langchain.py
+-rw-r--r--   0        0        0      465 2023-07-14 06:41:42.608621 botastico-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 botastico-0.1.2/PKG-INFO
```

### Comparing `botastico-0.1.1/README.md` & `botastico-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -40,12 +40,8 @@
 
 Remember to replace `'your_agent_id'` and `'your_api_key'` with your actual Botastico agent ID and API key.
 
 ## Feedback
 
 Your feedback is highly appreciated. If you have any suggestions, questions, or bug reports, please feel free to submit an issue on our GitHub page.
 
-## Disclaimer
-
-This software is provided "as is", without warranty of any kind, express or implied. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability arising from the use of the software. 
-
 Enjoy building amazing conversational experiences with Botastico!
```

### Comparing `botastico-0.1.1/botastico/langchain.py` & `botastico-0.1.2/botastico/langchain.py`

 * *Files identical despite different names*

### Comparing `botastico-0.1.1/PKG-INFO` & `botastico-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botastico
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python SDK for using the botasti.co chat API
 Author: Andres Kull
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
@@ -53,12 +53,8 @@
 
 Remember to replace `'your_agent_id'` and `'your_api_key'` with your actual Botastico agent ID and API key.
 
 ## Feedback
 
 Your feedback is highly appreciated. If you have any suggestions, questions, or bug reports, please feel free to submit an issue on our GitHub page.
 
-## Disclaimer
-
-This software is provided "as is", without warranty of any kind, express or implied. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability arising from the use of the software. 
-
 Enjoy building amazing conversational experiences with Botastico!
```

