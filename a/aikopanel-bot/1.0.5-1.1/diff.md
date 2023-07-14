# Comparing `tmp/aikopanel-bot-1.0.5.tar.gz` & `tmp/aikopanel-bot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikopanel-bot-1.0.5.tar", last modified: Fri Jul 14 14:29:28 2023, max compression
+gzip compressed data, was "aikopanel-bot-1.1.tar", last modified: Fri Jul 14 14:35:26 2023, max compression
```

## Comparing `aikopanel-bot-1.0.5.tar` & `aikopanel-bot-1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:29:28.717280 aikopanel-bot-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:29:28.717280 aikopanel-bot-1.0.5/Commands/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/bind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/buyplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/checkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/getapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/idapple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/myinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/myinvite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/mysub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/myusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/sni.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/topserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/topused.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/unbind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/website.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Commands/yesterdayorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:29:28.717280 aikopanel-bot-1.0.5/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Modules/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Modules/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/Modules/ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-07-14 14:29:28.717280 aikopanel-bot-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:29:28.717280 aikopanel-bot-1.0.5/aikopanel_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-07-14 14:29:28.000000 aikopanel-bot-1.0.5/aikopanel_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-14 14:29:28.000000 aikopanel-bot-1.0.5/aikopanel_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:29:28.000000 aikopanel-bot-1.0.5/aikopanel_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 14:29:28.000000 aikopanel-bot-1.0.5/aikopanel_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 14:29:28.000000 aikopanel-bot-1.0.5/aikopanel_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:29:28.717280 aikopanel-bot-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-14 14:29:16.000000 aikopanel-bot-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/Commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/buyplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/checkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/getapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/idapple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/myinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/myinvite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/mysub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/myusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/sni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/topserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/topused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/yesterdayorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/aikopanel_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/setup.py
```

### Comparing `aikopanel-bot-1.0.5/Commands/bind.py` & `aikopanel-bot-1.1/Commands/bind.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/buyplan.py` & `aikopanel-bot-1.1/Commands/buyplan.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/check.py` & `aikopanel-bot-1.1/Commands/check.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/checkinfo.py` & `aikopanel-bot-1.1/Commands/checkinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/getapp.py` & `aikopanel-bot-1.1/Commands/getapp.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/idapple.py` & `aikopanel-bot-1.1/Commands/idapple.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/myinfo.py` & `aikopanel-bot-1.1/Commands/myinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/myinvite.py` & `aikopanel-bot-1.1/Commands/myinvite.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/mysub.py` & `aikopanel-bot-1.1/Commands/mysub.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/myusage.py` & `aikopanel-bot-1.1/Commands/myusage.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/ping.py` & `aikopanel-bot-1.1/Commands/ping.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/sni.py` & `aikopanel-bot-1.1/Commands/sni.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/start.py` & `aikopanel-bot-1.1/Commands/start.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/topserver.py` & `aikopanel-bot-1.1/Commands/topserver.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/topused.py` & `aikopanel-bot-1.1/Commands/topused.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/unbind.py` & `aikopanel-bot-1.1/Commands/unbind.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/website.py` & `aikopanel-bot-1.1/Commands/website.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Commands/yesterdayorder.py` & `aikopanel-bot-1.1/Commands/yesterdayorder.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/LICENSE` & `aikopanel-bot-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Modules/daily.py` & `aikopanel-bot-1.1/Modules/daily.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/Modules/order.py` & `aikopanel-bot-1.1/Modules/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 timezone = pytz.timezone('Asia/Ho_Chi_Minh')
 config = aikopanel_bot.config['bot']
 order_total = 0
 order_status = []
 thisEnhanced = False
 
-if bot.isEnhanced:
-    if bot.enhancedModules.count('order'):
+if aikopanel_bot.isEnhanced:
+    if aikopanel_bot.enhancedModules.count('order'):
         try:
             enhanced.initEnhanced()
             enhanced.dbEnhanced(os.path.basename(__file__).replace('.py', ''))
             thisEnhanced = True
         except Exception as err:
             print(repr(err))
```

### Comparing `aikopanel-bot-1.0.5/Modules/ticket.py` & `aikopanel-bot-1.1/Modules/ticket.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/PKG-INFO` & `aikopanel-bot-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanel-bot
-Version: 1.0.5
+Version: 1.1
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanel-bot-1.0.5/README.md` & `aikopanel-bot-1.1/README.md`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/aikopanel_bot.egg-info/PKG-INFO` & `aikopanel-bot-1.1/aikopanel_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanel-bot
-Version: 1.0.5
+Version: 1.1
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanel-bot-1.0.5/aikopanel_bot.egg-info/SOURCES.txt` & `aikopanel-bot-1.1/aikopanel_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.0.5/setup.py` & `aikopanel-bot-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='aikopanel-bot',
-    version='1.0.5',
+    version='1.1',
     author='AikoCute',
     author_email='aiko@aikocute.tech',
     description='Description of the aikopanel-bot project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Github-Aiko/AikoPanel-bot',
     packages=find_packages(),
```

