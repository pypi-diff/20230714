# Comparing `tmp/request_url_2023-1.0.0.tar.gz` & `tmp/request_url_2023-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\request_url_2023-1.0.0.tar", last modified: Fri Jul 14 03:49:51 2023, max compression
+gzip compressed data, was "dist\request_url_2023-1.0.1.tar", last modified: Fri Jul 14 11:13:10 2023, max compression
```

## Comparing `request_url_2023-1.0.0.tar` & `request_url_2023-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/
--rw-rw-rw-   0        0        0     1089 2023-07-14 03:36:37.000000 request_url_2023-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      784 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-07-14 03:34:01.000000 request_url_2023-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023/
--rw-rw-rw-   0        0        0        0 2023-07-14 03:38:43.000000 request_url_2023-1.0.0/request_url_2023/__init__.py
--rw-rw-rw-   0        0        0      393 2023-07-14 03:39:55.000000 request_url_2023-1.0.0/request_url_2023/main.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023.egg-info/
--rw-rw-rw-   0        0        0      784 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/request_url_2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 03:49:51.000000 request_url_2023-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1068 2023-07-14 03:49:20.000000 request_url_2023-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-07-14 03:36:37.000000 request_url_2023-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      784 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-07-14 03:34:01.000000 request_url_2023-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023/
+-rw-rw-rw-   0        0        0        0 2023-07-14 03:38:43.000000 request_url_2023-1.0.1/request_url_2023/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-07-14 11:12:33.000000 request_url_2023-1.0.1/request_url_2023/send_requests.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023.egg-info/
+-rw-rw-rw-   0        0        0      784 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/request_url_2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 11:13:10.000000 request_url_2023-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2023-07-14 10:50:54.000000 request_url_2023-1.0.1/setup.py
```

### Comparing `request_url_2023-1.0.0/LICENSE` & `request_url_2023-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `request_url_2023-1.0.0/PKG-INFO` & `request_url_2023-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request_url_2023
-Version: 1.0.0
+Version: 1.0.1
 Summary: send bulk requests to a url
 Home-page: https://www.linkedin.com/in/chandlersong/
 Author: chandler song
 Author-email: 275737875@qq.com
 License: MIT
 Keywords: requests url
 Platform: all
```

### Comparing `request_url_2023-1.0.0/request_url_2023.egg-info/PKG-INFO` & `request_url_2023-1.0.1/request_url_2023.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: request-url-2023
-Version: 1.0.0
+Version: 1.0.1
 Summary: send bulk requests to a url
 Home-page: https://www.linkedin.com/in/chandlersong/
 Author: chandler song
 Author-email: 275737875@qq.com
 License: MIT
 Keywords: requests url
 Platform: all
```

### Comparing `request_url_2023-1.0.0/setup.py` & `request_url_2023-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
   long_description = f.read()
 setup(name='request_url_2023',  # 包名
-      version='1.0.0',  # 版本号
+      version='1.0.1',  # 版本号
       description='send bulk requests to a url',
       long_description=long_description,
       author='chandler song',
       author_email='275737875@qq.com',
       url='https://www.linkedin.com/in/chandlersong/',
       keywords = "requests url",
       license='MIT',
       packages = find_packages(),
       install_requires=[
-          "requests",
+          "aiohttp",
+          "asyncio",
+          "fake_headers",
       ],
       platforms=["all"],
       classifiers=[
           'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Natural Language :: Chinese (Simplified)',
           'Programming Language :: Python :: 3.7',
```

