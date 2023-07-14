# Comparing `tmp/xml_sitemap_writer-0.5.0.tar.gz` & `tmp/xml_sitemap_writer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xml_sitemap_writer-0.5.0.tar", last modified: Sat Jan 29 17:43:48 2022, max compression
+gzip compressed data, was "xml_sitemap_writer-0.5.1.tar", last modified: Fri Jul 14 10:01:29 2023, max compression
```

## Comparing `xml_sitemap_writer-0.5.0.tar` & `xml_sitemap_writer-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 17:43:48.766024 xml_sitemap_writer-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-29 17:43:39.000000 xml_sitemap_writer-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-29 17:43:39.000000 xml_sitemap_writer-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-01-29 17:43:48.766024 xml_sitemap_writer-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-01-29 17:43:39.000000 xml_sitemap_writer-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-29 17:43:48.766024 xml_sitemap_writer-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-01-29 17:43:39.000000 xml_sitemap_writer-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-29 17:43:48.766024 xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-01-29 17:43:48.000000 xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-01-29 17:43:48.000000 xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-29 17:43:48.000000 xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-01-29 17:43:48.000000 xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-01-29 17:43:48.000000 xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-01-29 17:43:39.000000 xml_sitemap_writer-0.5.0/xml_sitemap_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:01:29.751059 xml_sitemap_writer-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 10:01:19.000000 xml_sitemap_writer-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 10:01:19.000000 xml_sitemap_writer-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-14 10:01:29.751059 xml_sitemap_writer-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-14 10:01:19.000000 xml_sitemap_writer-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:01:29.751059 xml_sitemap_writer-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-14 10:01:19.000000 xml_sitemap_writer-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:01:29.751059 xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-14 10:01:29.000000 xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 10:01:29.000000 xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:01:29.000000 xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 10:01:29.000000 xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 10:01:29.000000 xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-14 10:01:19.000000 xml_sitemap_writer-0.5.1/xml_sitemap_writer.py
```

### Comparing `xml_sitemap_writer-0.5.0/LICENSE` & `xml_sitemap_writer-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xml_sitemap_writer-0.5.0/PKG-INFO` & `xml_sitemap_writer-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: xml_sitemap_writer
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python3 package for writing large XML sitemaps with no external dependencies
 Home-page: https://github.com/pigs-will-fly/py-xml-sitemap-writer
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # py-xml-sitemap-writer
 [![PyPI](https://img.shields.io/pypi/v/xml-sitemap-writer.svg)](https://pypi.python.org/pypi/xml-sitemap-writer)
 [![Downloads](https://pepy.tech/badge/xml-sitemap-writer)](https://pepy.tech/project/xml-sitemap-writer)
@@ -73,9 +73,7 @@
 ```
 
 For easier discovery of your sitemap add its URL to `/robots.txt` file:
 
 ```
 Sitemap: https://your.site.io/sitemap.xml
 ```
-
-
```

### Comparing `xml_sitemap_writer-0.5.0/README.md` & `xml_sitemap_writer-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `xml_sitemap_writer-0.5.0/setup.py` & `xml_sitemap_writer-0.5.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Package definition
 """
 from setuptools import setup
 
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 
 # @see https://packaging.python.org/tutorials/packaging-projects/#creating-setup-py
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # @see https://github.com/pypa/sampleproject/blob/master/setup.py
 setup(
@@ -28,18 +28,19 @@
         #   5 - Production/Stable
         "Development Status :: 5 - Production/Stable",
         # Pick your license as you wish
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here.
         "Programming Language :: Python :: 3",
     ],
+    python_requires=">=3.8",
     py_modules=["xml_sitemap_writer"],
     extras_require={
         "dev": [
-            "black==21.12b0",
+            "black==23.7.0",
             "coveralls==3.3.1",
-            "pylint==2.12.2",
-            "pytest==6.2.5",
-            "pytest-cov==3.0.0",
+            "pylint==2.17.4",
+            "pytest==7.4.0",
+            "pytest-cov==4.1.0",
         ]
     },
 )
```

### Comparing `xml_sitemap_writer-0.5.0/xml_sitemap_writer.egg-info/PKG-INFO` & `xml_sitemap_writer-0.5.1/xml_sitemap_writer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: xml-sitemap-writer
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python3 package for writing large XML sitemaps with no external dependencies
 Home-page: https://github.com/pigs-will-fly/py-xml-sitemap-writer
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # py-xml-sitemap-writer
 [![PyPI](https://img.shields.io/pypi/v/xml-sitemap-writer.svg)](https://pypi.python.org/pypi/xml-sitemap-writer)
 [![Downloads](https://pepy.tech/badge/xml-sitemap-writer)](https://pepy.tech/project/xml-sitemap-writer)
@@ -73,9 +73,7 @@
 ```
 
 For easier discovery of your sitemap add its URL to `/robots.txt` file:
 
 ```
 Sitemap: https://your.site.io/sitemap.xml
 ```
-
-
```

### Comparing `xml_sitemap_writer-0.5.0/xml_sitemap_writer.py` & `xml_sitemap_writer-0.5.1/xml_sitemap_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Provides XMLSitemap class used to generate large XML sitemap from iterators
 """
 import gzip  # https://docs.python.org/3/library/gzip.html
 import logging
 
-from typing import List, Iterator
-from typing.io import IO  # pylint:disable=import-error
+from typing import List, Iterator, IO
 from xml.sax.saxutils import escape as escape_xml
 
 POWERED_BY_URL = "https://github.com/pigs-will-fly/py-xml-sitemap-writer"
 
 
 # pylint:disable=too-many-instance-attributes
 class XMLSitemap:
```

