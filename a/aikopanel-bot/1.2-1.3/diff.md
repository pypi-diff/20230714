# Comparing `tmp/aikopanel-bot-1.2.tar.gz` & `tmp/aikopanel-bot-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikopanel-bot-1.2.tar", last modified: Fri Jul 14 16:16:35 2023, max compression
+gzip compressed data, was "aikopanel-bot-1.3.tar", last modified: Fri Jul 14 16:59:41 2023, max compression
```

## Comparing `aikopanel-bot-1.2.tar` & `aikopanel-bot-1.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/Commands/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/bind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/buyplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/checkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/getapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/idapple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/myinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/myinvite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/mysub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/myusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/sni.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/topserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/topused.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/unbind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/website.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/aikopanel_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:59:41.481449 aikopanel-bot-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:59:41.481449 aikopanel-bot-1.3/Commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/buyplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/checkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/getapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/idapple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/myinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/myinvite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/mysub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/myusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/sni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/topserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/topused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Commands/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:59:41.481449 aikopanel-bot-1.3/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Modules/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Modules/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/Modules/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 16:59:41.481449 aikopanel-bot-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:59:41.481449 aikopanel-bot-1.3/aikopanel_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 16:59:41.000000 aikopanel-bot-1.3/aikopanel_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-14 16:59:41.000000 aikopanel-bot-1.3/aikopanel_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:59:41.000000 aikopanel-bot-1.3/aikopanel_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 16:59:41.000000 aikopanel-bot-1.3/aikopanel_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 16:59:41.000000 aikopanel-bot-1.3/aikopanel_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 16:59:41.000000 aikopanel-bot-1.3/aikopanel_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:59:41.481449 aikopanel-bot-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-14 16:59:31.000000 aikopanel-bot-1.3/setup.py
```

### Comparing `aikopanel-bot-1.2/Commands/bind.py` & `aikopanel-bot-1.3/Commands/bind.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/buyplan.py` & `aikopanel-bot-1.3/Commands/buyplan.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/check.py` & `aikopanel-bot-1.3/Commands/check.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/checkinfo.py` & `aikopanel-bot-1.3/Commands/checkinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/getapp.py` & `aikopanel-bot-1.3/Commands/getapp.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/idapple.py` & `aikopanel-bot-1.3/Commands/idapple.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/myinfo.py` & `aikopanel-bot-1.3/Commands/myinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/myinvite.py` & `aikopanel-bot-1.3/Commands/myinvite.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/mysub.py` & `aikopanel-bot-1.3/Commands/mysub.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/myusage.py` & `aikopanel-bot-1.3/Commands/myusage.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/ping.py` & `aikopanel-bot-1.3/Commands/ping.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/sni.py` & `aikopanel-bot-1.3/Commands/sni.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/start.py` & `aikopanel-bot-1.3/Commands/start.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/topserver.py` & `aikopanel-bot-1.3/Commands/topserver.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/topused.py` & `aikopanel-bot-1.3/Commands/topused.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/unbind.py` & `aikopanel-bot-1.3/Commands/unbind.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Commands/website.py` & `aikopanel-bot-1.3/Commands/website.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/LICENSE` & `aikopanel-bot-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Modules/daily.py` & `aikopanel-bot-1.3/Modules/daily.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Modules/order.py` & `aikopanel-bot-1.3/Modules/order.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/Modules/ticket.py` & `aikopanel-bot-1.3/Modules/ticket.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/PKG-INFO` & `aikopanel-bot-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanel-bot
-Version: 1.2
+Version: 1.3
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanel-bot-1.2/README.md` & `aikopanel-bot-1.3/README.md`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.2/aikopanel_bot.egg-info/PKG-INFO` & `aikopanel-bot-1.3/aikopanel_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanel-bot
-Version: 1.2
+Version: 1.3
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanel-bot-1.2/aikopanel_bot.egg-info/SOURCES.txt` & `aikopanel-bot-1.3/aikopanel_bot.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -22,9 +22,10 @@
 Modules/__init__.py
 Modules/daily.py
 Modules/order.py
 Modules/ticket.py
 aikopanel_bot.egg-info/PKG-INFO
 aikopanel_bot.egg-info/SOURCES.txt
 aikopanel_bot.egg-info/dependency_links.txt
+aikopanel_bot.egg-info/entry_points.txt
 aikopanel_bot.egg-info/requires.txt
 aikopanel_bot.egg-info/top_level.txt
```

### Comparing `aikopanel-bot-1.2/setup.py` & `aikopanel-bot-1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='aikopanel-bot',
-    version='1.2',
+    version='1.3',
     author='AikoCute',
     author_email='aiko@aikocute.tech',
     description='Description of the aikopanel-bot project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Github-Aiko/AikoPanel-bot',
     packages=find_packages(),
@@ -19,14 +19,19 @@
         'PyMySQL==1.0.2',
         'python-telegram-bot==20.0a4',
         'PyYAML==6.0',
         'requests==2.27.1',
         'sshtunnel==0.4.0',
         'qrcode==7.4.2'
     ],
+    entry_points={
+        'console_scripts': [
+            'aikopanel_bot = aikopanel_bot:main'
+        ]
+    },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

