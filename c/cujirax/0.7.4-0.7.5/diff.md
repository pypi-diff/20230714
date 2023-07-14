# Comparing `tmp/cujirax-0.7.4.tar.gz` & `tmp/cujirax-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.7.4.tar", last modified: Thu Jun 22 16:27:23 2023, max compression
+gzip compressed data, was "cujirax-0.7.5.tar", last modified: Fri Jul 14 14:54:11 2023, max compression
```

## Comparing `cujirax-0.7.4.tar` & `cujirax-0.7.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.4/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.4/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.4/README.md
--rw-r--r--   0        0        0    10592 2023-06-22 16:27:07.038789 cujirax-0.7.4/cujirax/__init__.py
--rw-r--r--   0        0        0     2120 2023-06-22 16:26:46.910876 cujirax-0.7.4/cujirax/cucumber.py
--rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.4/cujirax/jira.py
--rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.4/cujirax/xray/__init__.py
--rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.4/cujirax/xray/graphql.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.4/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.4/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.7.5/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.7.5/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.7.5/README.md
+-rw-r--r--   0        0        0    10592 2023-07-14 14:53:19.473427 cujirax-0.7.5/cujirax/__init__.py
+-rw-r--r--   0        0        0     2120 2023-06-22 16:26:46.910876 cujirax-0.7.5/cujirax/cucumber.py
+-rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.7.5/cujirax/jira.py
+-rw-r--r--   0        0        0     2735 2023-04-24 16:49:30.639020 cujirax-0.7.5/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0      961 2023-04-24 16:50:20.686692 cujirax-0.7.5/cujirax/xray/graphql.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.7.5/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.7.5/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      483 2023-07-14 14:52:14.617711 cujirax-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 cujirax-0.7.5/PKG-INFO
```

### Comparing `cujirax-0.7.4/.gitignore` & `cujirax-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/LICENSE` & `cujirax-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/README.md` & `cujirax-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/cujirax/__init__.py` & `cujirax-0.7.5/cujirax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
```

### Comparing `cujirax-0.7.4/cujirax/cucumber.py` & `cujirax-0.7.5/cujirax/cucumber.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/cujirax/jira.py` & `cujirax-0.7.5/cujirax/jira.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/cujirax/xray/__init__.py` & `cujirax-0.7.5/cujirax/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/cujirax/xray/graphql.py` & `cujirax-0.7.5/cujirax/xray/graphql.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/cujirax/xray/import_results.py` & `cujirax-0.7.5/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/cujirax/xray/import_tests.py` & `cujirax-0.7.5/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.7.4/PKG-INFO` & `cujirax-0.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.7.4
+Version: 0.7.5
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: pydantic
+Requires-Dist: pydantic==1.10.10
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
 Requires-Dist: loguru
 Project-URL: Home, https://github.com/maxleow/cujirax
 
 # cujirax
 `Cu`cumber `Ji`ra and `X`ray
```

