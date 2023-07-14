# Comparing `tmp/aikopanelbot-1.0.2.tar.gz` & `tmp/aikopanelbot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikopanelbot-1.0.2.tar", last modified: Fri Jul 14 13:56:40 2023, max compression
+gzip compressed data, was "aikopanelbot-1.0.3.tar", last modified: Fri Jul 14 14:05:58 2023, max compression
```

## Comparing `aikopanelbot-1.0.2.tar` & `aikopanelbot-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:56:40.321150 aikopanelbot-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:56:40.321150 aikopanelbot-1.0.2/Commands/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/bind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/buyplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/checkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/getapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/idapple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/myinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/myinvite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/mysub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/myusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/sni.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/topserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/topused.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/unbind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/website.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Commands/yesterdayorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:56:40.321150 aikopanelbot-1.0.2/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Modules/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Modules/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/Modules/ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-14 13:56:40.321150 aikopanelbot-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:56:40.321150 aikopanelbot-1.0.2/aikopanelbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-14 13:56:40.000000 aikopanelbot-1.0.2/aikopanelbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-14 13:56:40.000000 aikopanelbot-1.0.2/aikopanelbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:56:40.000000 aikopanelbot-1.0.2/aikopanelbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 13:56:40.000000 aikopanelbot-1.0.2/aikopanelbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 13:56:40.000000 aikopanelbot-1.0.2/aikopanelbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:56:40.321150 aikopanelbot-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 13:56:25.000000 aikopanelbot-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:05:58.259052 aikopanelbot-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:05:58.259052 aikopanelbot-1.0.3/Commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/buyplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/checkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/getapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/idapple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/myinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/myinvite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/mysub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/myusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/sni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/topserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/topused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Commands/yesterdayorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:05:58.259052 aikopanelbot-1.0.3/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Modules/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Modules/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/Modules/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-14 14:05:58.259052 aikopanelbot-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:05:58.259052 aikopanelbot-1.0.3/aikopanelbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-14 14:05:58.000000 aikopanelbot-1.0.3/aikopanelbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 14:05:58.000000 aikopanelbot-1.0.3/aikopanelbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:05:58.000000 aikopanelbot-1.0.3/aikopanelbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 14:05:58.000000 aikopanelbot-1.0.3/aikopanelbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 14:05:58.000000 aikopanelbot-1.0.3/aikopanelbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 14:05:58.000000 aikopanelbot-1.0.3/aikopanelbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:05:58.259052 aikopanelbot-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-14 14:05:45.000000 aikopanelbot-1.0.3/setup.py
```

### Comparing `aikopanelbot-1.0.2/Commands/bind.py` & `aikopanelbot-1.0.3/Commands/bind.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/buyplan.py` & `aikopanelbot-1.0.3/Commands/buyplan.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/check.py` & `aikopanelbot-1.0.3/Commands/check.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/checkinfo.py` & `aikopanelbot-1.0.3/Commands/checkinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/getapp.py` & `aikopanelbot-1.0.3/Commands/getapp.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/idapple.py` & `aikopanelbot-1.0.3/Commands/idapple.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/myinfo.py` & `aikopanelbot-1.0.3/Commands/myinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/myinvite.py` & `aikopanelbot-1.0.3/Commands/myinvite.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/mysub.py` & `aikopanelbot-1.0.3/Commands/mysub.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/myusage.py` & `aikopanelbot-1.0.3/Commands/myusage.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/ping.py` & `aikopanelbot-1.0.3/Commands/ping.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/sni.py` & `aikopanelbot-1.0.3/Commands/sni.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/start.py` & `aikopanelbot-1.0.3/Commands/start.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/topserver.py` & `aikopanelbot-1.0.3/Commands/topserver.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/topused.py` & `aikopanelbot-1.0.3/Commands/topused.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/unbind.py` & `aikopanelbot-1.0.3/Commands/unbind.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/website.py` & `aikopanelbot-1.0.3/Commands/website.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Commands/yesterdayorder.py` & `aikopanelbot-1.0.3/Commands/yesterdayorder.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/LICENSE` & `aikopanelbot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Modules/daily.py` & `aikopanelbot-1.0.3/Modules/daily.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Modules/order.py` & `aikopanelbot-1.0.3/Modules/order.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/Modules/ticket.py` & `aikopanelbot-1.0.3/Modules/ticket.py`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/PKG-INFO` & `aikopanelbot-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanelbot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanelbot-1.0.2/README.md` & `aikopanelbot-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aikopanelbot-1.0.2/aikopanelbot.egg-info/PKG-INFO` & `aikopanelbot-1.0.3/aikopanelbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanelbot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanelbot-1.0.2/aikopanelbot.egg-info/SOURCES.txt` & `aikopanelbot-1.0.3/aikopanelbot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 Modules/__init__.py
 Modules/daily.py
 Modules/order.py
 Modules/ticket.py
 aikopanelbot.egg-info/PKG-INFO
 aikopanelbot.egg-info/SOURCES.txt
 aikopanelbot.egg-info/dependency_links.txt
+aikopanelbot.egg-info/entry_points.txt
 aikopanelbot.egg-info/requires.txt
 aikopanelbot.egg-info/top_level.txt
```

### Comparing `aikopanelbot-1.0.2/setup.py` & `aikopanelbot-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='aikopanelbot',
-    version='1.0.2',
+    version='1.0.3',
     author='AikoCute',
     author_email='aiko@aikocute.tech',
     description='Description of the aikopanel-bot project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Github-Aiko/AikoPanel-bot',
     packages=find_packages(),
@@ -29,8 +29,13 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    entry_points={
+        'console_scripts': [
+            'aikopanelbot = bot:run'
+        ]
+    },
 )
```

