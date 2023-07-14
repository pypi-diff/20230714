# Comparing `tmp/addressformatting-1.3.1.tar.gz` & `tmp/addressformatting-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/addressformatting-1.3.1.tar", last modified: Wed Jun 15 14:54:26 2022, max compression
+gzip compressed data, was "dist/addressformatting-1.3.2.tar", last modified: Fri Jul 14 08:30:16 2023, max compression
```

## Comparing `addressformatting-1.3.1.tar` & `addressformatting-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:54:26.000000 addressformatting-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-06-15 14:54:03.000000 addressformatting-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-15 14:54:03.000000 addressformatting-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-06-15 14:54:26.000000 addressformatting-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-06-15 14:54:03.000000 addressformatting-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:54:26.000000 addressformatting-1.3.1/addressformatting/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-15 14:54:03.000000 addressformatting-1.3.1/addressformatting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:54:26.000000 addressformatting-1.3.1/addressformatting/data/
--rw-r--r--   0 runner    (1001) docker     (121)    51179 2022-06-15 14:54:03.000000 addressformatting-1.3.1/addressformatting/data/worldwide.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-06-15 14:54:03.000000 addressformatting-1.3.1/addressformatting/format.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 14:54:03.000000 addressformatting-1.3.1/addressformatting/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-15 14:54:03.000000 addressformatting-1.3.1/addressformatting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:54:26.000000 addressformatting-1.3.1/addressformatting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-06-15 14:54:25.000000 addressformatting-1.3.1/addressformatting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-06-15 14:54:26.000000 addressformatting-1.3.1/addressformatting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 14:54:25.000000 addressformatting-1.3.1/addressformatting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-15 14:54:25.000000 addressformatting-1.3.1/addressformatting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-15 14:54:26.000000 addressformatting-1.3.1/addressformatting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-15 14:54:26.000000 addressformatting-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-06-15 14:54:03.000000 addressformatting-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:30:16.000000 addressformatting-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-14 08:29:55.000000 addressformatting-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 08:29:55.000000 addressformatting-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-14 08:30:16.000000 addressformatting-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-14 08:29:55.000000 addressformatting-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 08:29:55.000000 addressformatting-1.3.2/addressformatting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    51497 2023-07-14 08:29:55.000000 addressformatting-1.3.2/addressformatting/data/worldwide.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-14 08:29:55.000000 addressformatting-1.3.2/addressformatting/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:29:55.000000 addressformatting-1.3.2/addressformatting/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-14 08:29:55.000000 addressformatting-1.3.2/addressformatting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 08:30:16.000000 addressformatting-1.3.2/addressformatting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-14 08:30:16.000000 addressformatting-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-14 08:29:55.000000 addressformatting-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:30:16.000000 addressformatting-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-14 08:29:55.000000 addressformatting-1.3.2/tests/test_germany.py
```

### Comparing `addressformatting-1.3.1/LICENSE.txt` & `addressformatting-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `addressformatting-1.3.1/PKG-INFO` & `addressformatting-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addressformatting
-Version: 1.3.1
+Version: 1.3.2
 Summary: Formatting utility for international postal addresses
 Home-page: https://github.com/pudo/addressformatting
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: BSD
 Keywords: address formatting,international
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `addressformatting-1.3.1/README.md` & `addressformatting-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `addressformatting-1.3.1/addressformatting/data/worldwide.yml` & `addressformatting-1.3.2/addressformatting/data/worldwide.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1114,15 +1114,22 @@
         {{{attention}}}
         {{{house}}}
         {{{house_number}}} {{{road}}} 
         {{#first}} {{{city}}} || {{{town}}} || {{{village}}} {{/first}}, {{#first}} {{{state}}} || {{{island}}} {{/first}}
         {{{country}}}
 # Democratic People's Republic of Korea / North Korea
 KP:
-    address_template: *generic21
+    address_template: |
+        {{{attention}}}
+        {{{house}}}
+        {{{road}}} {{{house_number}}} 
+        {{#first}} {{{suburb}}} || {{{city_district}}} || {{{neighbourhood}}} {{/first}}
+        {{#first}} {{{city}}} || {{{town}}} || {{{village}}} {{/first}} 
+        {{#first}} {{{state}}} || {{{province}}} {{/first}}
+        {{{country}}}
 
 # Republic of Korea / South Korea
 KR:
     address_template: |
         {{{attention}}}
         {{{house}}}
         {{{house_number}}} {{{road}}}
```

### Comparing `addressformatting-1.3.1/addressformatting/format.py` & `addressformatting-1.3.2/addressformatting/format.py`

 * *Files identical despite different names*

### Comparing `addressformatting-1.3.1/addressformatting/util.py` & `addressformatting-1.3.2/addressformatting/util.py`

 * *Files identical despite different names*

### Comparing `addressformatting-1.3.1/addressformatting.egg-info/PKG-INFO` & `addressformatting-1.3.2/addressformatting.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addressformatting
-Version: 1.3.1
+Version: 1.3.2
 Summary: Formatting utility for international postal addresses
 Home-page: https://github.com/pudo/addressformatting
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: BSD
 Keywords: address formatting,international
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `addressformatting-1.3.1/setup.py` & `addressformatting-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="addressformatting",
-    version="1.3.1",
+    version="1.3.2",
     description="Formatting utility for international postal addresses",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pudo/addressformatting",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     license="BSD",
```

