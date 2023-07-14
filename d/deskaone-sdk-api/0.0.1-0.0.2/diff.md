# Comparing `tmp/deskaone_sdk_api-0.0.1.tar.gz` & `tmp/deskaone_sdk_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_api-0.0.1.tar", max compression
+gzip compressed data, was "deskaone_sdk_api-0.0.2.tar", max compression
```

## Comparing `deskaone_sdk_api-0.0.1.tar` & `deskaone_sdk_api-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      737 2023-06-26 04:25:13.027051 deskaone_sdk_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       28 2023-06-26 10:17:37.373451 deskaone_sdk_api-0.0.1/README.md
--rw-r--r--   0        0        0      356 2023-06-26 04:21:27.302553 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/__init__.py
--rw-r--r--   0        0        0     6184 2023-06-26 04:20:41.837278 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Client/__init__.py
--rw-r--r--   0        0        0      793 2023-06-26 04:19:31.636954 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Exceptions/__init__.py
--rw-r--r--   0        0        0     2931 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Internal/__init__.py
--rw-r--r--   0        0        0      460 2023-06-26 04:02:02.135172 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/ProgressBar.py
--rw-r--r--   0        0        0    38069 2023-06-26 04:19:31.636954 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Reverse.py
--rw-r--r--   0        0        0     2956 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Timer.py
--rw-r--r--   0        0        0     3569 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/UserAgent.py
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.1/setup.py
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      737 2023-07-03 11:53:18.312210 deskaone_sdk_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-06-26 10:17:37.373451 deskaone_sdk_api-0.0.2/README.md
+-rw-r--r--   0        0        0      356 2023-06-26 04:21:27.302553 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/__init__.py
+-rw-r--r--   0        0        0     6184 2023-06-26 04:20:41.837278 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Client/__init__.py
+-rw-r--r--   0        0        0      793 2023-06-26 04:19:31.636954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2931 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Internal/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-03 11:53:11.584451 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    38295 2023-07-03 11:52:57.986206 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Reverse.py
+-rw-r--r--   0        0        0     2956 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Timer.py
+-rw-r--r--   0        0        0     3569 2023-06-26 04:19:31.581954 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/UserAgent.py
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.2/setup.py
+-rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 deskaone_sdk_api-0.0.2/PKG-INFO
```

### Comparing `deskaone_sdk_api-0.0.1/pyproject.toml` & `deskaone_sdk_api-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-api"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_api", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Client/__init__.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Database/__init__.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Exceptions/__init__.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Internal/__init__.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/AWSViker.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Crypto.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/ProgressBar.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Proxy.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,14 +721,16 @@
                                 DATA    = API,
                                 IpPort  = IpPort
                             )
                         else:
                             self.ProxyError(IpPort=IpPort, Add=True)
                 if Count >= len(self.ListProxy):
                     self.Rescan(self.__Authorization__, self.__New__, *self.__args__, **self.__kwargs__)
+                    if os.path.exists('Database/ProxyError.txt') is True: os.unlink('Database/ProxyError.txt')
+                    if os.path.exists('Database/ProxyDetect.txt') is True: os.unlink('Database/ProxyDetect.txt')
                     Count = 0
             except ProxyError as e:
                 self.ProxyError(IpPort=IpPort, Add=True)
             except ConnectTimeout as e:
                 self.ProxyError(IpPort=IpPort, Add=True)
             except ConnectionError as e:
                 self.ProxyError(IpPort=IpPort, Add=True)
```

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Random.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Timer.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/Typer.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/src/deskaone_sdk_api/Utils/UserAgent.py` & `deskaone_sdk_api-0.0.2/src/deskaone_sdk_api/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_api-0.0.1/setup.py` & `deskaone_sdk_api-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'python-dotenv>=0.20.0,<0.21.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.27.1,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-api',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
     'long_description': 'pip install deskaone-sdk-api',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_api-0.0.1/PKG-INFO` & `deskaone_sdk_api-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

