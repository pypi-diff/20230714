# Comparing `tmp/whatsapp-chatbot-python-0.5.1.tar.gz` & `tmp/whatsapp-chatbot-python-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.5.1.tar", last modified: Thu Jul  6 11:53:38 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.5.2.tar", last modified: Fri Jul 14 05:42:14 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.5.1.tar` & `whatsapp-chatbot-python-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.687980 whatsapp-chatbot-python-0.5.1/
--rw-rw-rw-   0        0        0    18829 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    15842 2023-07-06 11:53:38.687980 whatsapp-chatbot-python-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    14404 2023-07-06 09:38:10.000000 whatsapp-chatbot-python-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 11:53:38.687980 whatsapp-chatbot-python-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1809 2023-07-06 11:51:48.000000 whatsapp-chatbot-python-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.675948 whatsapp-chatbot-python-0.5.1/tests/
--rw-rw-rw-   0        0        0     1459 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.678957 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      270 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     4091 2023-07-06 09:38:10.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.686977 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-26 06:28:50.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     4513 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     2022 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-07-06 11:42:14.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/router.py
--rw-rw-rw-   0        0        0     2643 2023-07-06 09:38:10.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/state.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:53:38.682967 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0    15842 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-06 11:53:38.000000 whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.956021 whatsapp-chatbot-python-0.5.2/
+-rw-rw-rw-   0        0        0    18829 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    15842 2023-07-14 05:42:14.955019 whatsapp-chatbot-python-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14404 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:42:14.956021 whatsapp-chatbot-python-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-14 05:23:03.000000 whatsapp-chatbot-python-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.941969 whatsapp-chatbot-python-0.5.2/tests/
+-rw-rw-rw-   0        0        0     1459 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.943990 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      270 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     4091 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.954016 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     4513 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     2022 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/router.py
+-rw-rw-rw-   0        0        0     2643 2023-07-09 08:40:58.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/state.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:42:14.949003 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    15842 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-14 05:42:14.000000 whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.5.1/LICENSE` & `whatsapp-chatbot-python-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/PKG-INFO` & `whatsapp-chatbot-python-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.1
+Version: 0.5.2
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.5.1/README.md` & `whatsapp-chatbot-python-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/setup.py` & `whatsapp-chatbot-python-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.5.1",
+    version="0.5.2",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
@@ -38,10 +38,10 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     license=(
         "Creative Commons Attribution-NoDerivatives 4.0 International"
         " (CC BY-ND 4.0)"
     ),
-    install_requires=["whatsapp-api-client-python==0.0.39"],
+    install_requires=["whatsapp-api-client-python==0.0.40"],
     python_requires=">=3.7"
 )
```

### Comparing `whatsapp-chatbot-python-0.5.1/tests/test_manager.py` & `whatsapp-chatbot-python-0.5.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/filters.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/handler.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/observer.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python/manager/state.py` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python/manager/state.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.5.1
+Version: 0.5.2
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatsapp-chatbot-python-0.5.1/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.5.2/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

