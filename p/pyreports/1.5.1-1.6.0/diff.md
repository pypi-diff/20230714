# Comparing `tmp/pyreports-1.5.1.tar.gz` & `tmp/pyreports-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreports-1.5.1.tar", last modified: Tue Sep 27 09:54:13 2022, max compression
+gzip compressed data, was "pyreports-1.6.0.tar", last modified: Fri Jul 14 09:43:06 2023, max compression
```

## Comparing `pyreports-1.5.1.tar` & `pyreports-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,70 @@
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2022-09-27 09:54:13.829053 pyreports-1.5.1/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2595 2022-08-04 10:18:33.000000 pyreports-1.5.1/CHANGES.md
--rwxrwxr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    34916 2019-10-26 09:26:26.000000 pyreports-1.5.1/LICENSE.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       56 2022-09-27 09:54:04.000000 pyreports-1.5.1/MANIFEST.in
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    11857 2022-09-27 09:54:13.828053 pyreports-1.5.1/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8513 2022-09-27 09:45:00.000000 pyreports-1.5.1/README.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1099 2022-09-27 09:45:00.000000 pyreports-1.5.1/__info__.py
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2022-09-27 09:54:13.827053 pyreports-1.5.1/pyreports/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1230 2022-09-27 09:45:00.000000 pyreports-1.5.1/pyreports/__init__.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8808 2022-09-27 09:45:00.000000 pyreports-1.5.1/pyreports/cli.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    16518 2022-08-04 10:18:33.000000 pyreports-1.5.1/pyreports/core.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     4886 2022-04-15 12:42:38.000000 pyreports-1.5.1/pyreports/datatools.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1102 2022-04-15 12:42:39.000000 pyreports-1.5.1/pyreports/exception.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    20114 2022-09-27 09:45:00.000000 pyreports-1.5.1/pyreports/io.py
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2022-09-27 09:54:13.828053 pyreports-1.5.1/pyreports.egg-info/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    11857 2022-09-27 09:54:13.000000 pyreports-1.5.1/pyreports.egg-info/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      383 2022-09-27 09:54:13.000000 pyreports-1.5.1/pyreports.egg-info/SOURCES.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        1 2022-09-27 09:54:13.000000 pyreports-1.5.1/pyreports.egg-info/dependency_links.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       47 2022-09-27 09:54:13.000000 pyreports-1.5.1/pyreports.egg-info/entry_points.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       88 2022-09-27 09:54:13.000000 pyreports-1.5.1/pyreports.egg-info/requires.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       10 2022-09-27 09:54:13.000000 pyreports-1.5.1/pyreports.egg-info/top_level.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       38 2022-09-27 09:54:13.829053 pyreports-1.5.1/setup.cfg
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1290 2022-09-27 09:52:37.000000 pyreports-1.5.1/setup.py
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.784167 pyreports-1.6.0/
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/.circleci/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      581 2023-07-14 09:39:08.000000 pyreports-1.6.0/.circleci/config.yml
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/.github/
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      310 2021-05-22 09:10:30.000000 pyreports-1.6.0/.github/ISSUE_TEMPLATE/reports-enhancement.md
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      350 2021-05-22 09:10:30.000000 pyreports-1.6.0/.github/ISSUE_TEMPLATE/reports-issue.md
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      330 2020-09-16 09:59:48.000000 pyreports-1.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     3272 2021-05-01 12:43:38.000000 pyreports-1.6.0/.gitignore
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     3010 2023-07-14 09:39:08.000000 pyreports-1.6.0/CHANGES.md
+-rw-rw-r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2503 2019-10-29 13:39:34.000000 pyreports-1.6.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     4049 2019-10-28 14:57:18.000000 pyreports-1.6.0/CONTRIBUTING.md
+-rwxrwxr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    34916 2019-10-26 09:26:26.000000 pyreports-1.6.0/LICENSE.md
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       22 2023-07-14 09:39:08.000000 pyreports-1.6.0/MANIFEST.in
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     9612 2023-07-14 09:43:06.783167 pyreports-1.6.0/PKG-INFO
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8513 2022-09-27 09:45:00.000000 pyreports-1.6.0/README.md
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/assets/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8196 2022-04-15 12:42:38.000000 pyreports-1.6.0/assets/.DS_Store
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/assets/css/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6148 2022-04-15 12:42:38.000000 pyreports-1.6.0/assets/css/.DS_Store
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    12830 2021-05-26 12:03:02.000000 pyreports-1.6.0/assets/css/theme-1.css
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.778167 pyreports-1.6.0/assets/js/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6148 2022-04-15 12:42:38.000000 pyreports-1.6.0/assets/js/.DS_Store
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      882 2021-05-26 12:03:02.000000 pyreports-1.6.0/assets/js/main.js
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.778167 pyreports-1.6.0/docs/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      638 2021-05-08 08:55:41.000000 pyreports-1.6.0/docs/Makefile
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      764 2021-05-08 08:55:41.000000 pyreports-1.6.0/docs/make.bat
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       80 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/requirements.txt
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.779167 pyreports-1.6.0/docs/source/
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.779167 pyreports-1.6.0/docs/source/_static/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    14659 2021-05-26 10:37:38.000000 pyreports-1.6.0/docs/source/_static/pyreports.svg
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2149 2022-07-18 07:37:08.000000 pyreports-1.6.0/docs/source/conf.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     4737 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/source/datatools.rst
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.780167 pyreports-1.6.0/docs/source/dev/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8840 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/dev/cli.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     5896 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/dev/core.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     3801 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/dev/io.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    11452 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/example.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8402 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/executors.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2066 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/source/index.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      648 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/install.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6139 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/managers.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      201 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/package.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      855 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/source/pyreports.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     7906 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/report.rst
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    15086 2021-05-26 12:03:02.000000 pyreports-1.6.0/favicon.ico
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    19453 2022-09-27 09:45:00.000000 pyreports-1.6.0/index.html
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1359 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyproject.toml
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.781167 pyreports-1.6.0/pyreports/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1279 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/__init__.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     9067 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/cli.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    18933 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/core.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     5068 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/datatools.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1145 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/exception.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    20849 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/io.py
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.782167 pyreports-1.6.0/pyreports.egg-info/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     9612 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/PKG-INFO
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1182 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/SOURCES.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        1 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/dependency_links.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       47 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/entry_points.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       88 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/requires.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       10 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/top_level.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       38 2023-07-14 09:43:06.784167 pyreports-1.6.0/setup.cfg
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1395 2023-07-14 09:39:08.000000 pyreports-1.6.0/setup.py
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.783167 pyreports-1.6.0/tests/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      882 2022-04-15 12:42:39.000000 pyreports-1.6.0/tests/__init__.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8770 2023-07-14 09:39:08.000000 pyreports-1.6.0/tests/test_core.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2390 2023-07-14 09:39:08.000000 pyreports-1.6.0/tests/test_data.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6003 2022-04-15 12:42:39.000000 pyreports-1.6.0/tests/test_db.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8192 2022-06-27 09:04:05.000000 pyreports-1.6.0/tests/test_file.py
```

### Comparing `pyreports-1.5.1/CHANGES.md` & `pyreports-1.6.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Release notes
 
+## 1.6.0
+Jul 14, 2023
+
+- Add **deduplicate** function on datatools
+- Add **Manager** abstract class
+- Add **READABLE_MANAGER** and **WRITABLE_MANAGER** tuple
+- Add _pyproject.toml_ file
+- Add **negation** to filter method on _Executor_ class
+- Fix _max_len_ into **aggregate** function, refs #2
+- Fix _sendmail_ method addresses, refs #3
+- Rename **SQLiteConnection** class
+- Reformat code with ruff code analysis
+
 ## 1.5.0
 Aug 4, 2022
 
 - Added **cli** module
 - Added **reports** cli
 - Added **\__getitem\__** method on _Report_ class
 - Added **\__delitem\__** method on _Report_ class
```

### Comparing `pyreports-1.5.1/LICENSE.md` & `pyreports-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreports-1.5.1/PKG-INFO` & `pyreports-1.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: pyreports
-Version: 1.5.1
-Summary: pyreports is a python library that allows you to create complex report from various sources
+Version: 1.6.0
+Summary: pyreports is a python library that allows you to create complex report from various sources.
 Home-page: https://github.com/MatteoGuadrini/pyreports
 Author: Matteo Guadrini
-Author-email: matteo.guadrini@hotmail.it
+Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer: Matteo Guadrini
-Maintainer-email: matteo.guadrini@hotmail.it
+Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 License: GNU General Public License v3.0
-Keywords: pyreports reports report csv yaml export excel database ldap dataset file executor book
+Project-URL: homepage, https://github.com/MatteoGuadrini/pyreports'
+Project-URL: documentation, https://pyreports.readthedocs.io/en/latest/
+Project-URL: repository, https://github.com/MatteoGuadrini/pyreports/pyreports.git
+Project-URL: changelog, https://github.com/MatteoGuadrini/pyreports/blob/master/CHANGES.md
+Keywords: pyreports,reports,report,csv,yaml,export,excel,database,ldap,dataset,file,executor,book
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -264,76 +268,7 @@
 
 Thanks to Dane Hillard for writing the _Practices of the Python Pro_ books.
 
 Special thanks go to my wife, who understood the hours of absence for this development. 
 Thanks to my children, for the daily inspiration they give me and to make me realize, that life must be simple.
 
 Thanks Python!
-# Release notes
-
-## 1.5.0
-Aug 4, 2022
-
-- Added **cli** module
-- Added **reports** cli
-- Added **\__getitem\__** method on _Report_ class
-- Added **\__delitem\__** method on _Report_ class
-- Added **\__getitem\__** method on _ReportBook_ class
-- Added **\__delitem\__** method on _ReportBook_ class
-- Added **\__contains\__** on _Executor_ class
-- Fix **NoSQLManager** creation into _manager_ function
-- Fix **print_data** on _Report_ class
-
-## 1.4.0
-Jun 27, 2022
-
-- Added **\__bool\__** method on _Report_ class
-- Added **\__iter\__** method on _Report_ class
-- Added **\__bool\__** method on _ReportBook_ class
-- Added **\__iter\__** method on _Connection_ and _File_ classes
-- Added **\__iter\__** method on _FileManager_ class
-- Added **\__iter\__** method on _DatabaseManager_ class
-- Added **\__getitem\__** on _Executor_ class
-- Added **\__delitem\__** on _Executor_ class
-- Fix name of attachment on **send** method of _Report_ class
-- Fix **write** method on _LogFile_ class
-
-## 1.3.0
-Apr 15, 2022
-
-- Added **NoSQLManager** class; this class extend _Manager_ class on the [nosqlapi](https://github.com/MatteoGuadrini/nosqlapi) package
-- Added **LogFile** class; this class load a log file and _read_ method accept regular expression
-- Added **\__bool\__** and **\__repr\__** method on _File_ and _Connection_ abstract classes
-- Fix documentation API section
-- Fix tests package
-- Fix CircleCi docker image
-
-## 1.2.0
-Aug 5, 2021
-
-- Added _fill_value_ argument on **aggregate** function; this value also is callable without arguments
-- Added _send_ method on **Report** class; with this method you send report via email
-- Added _send_ method on **ReportBook** class; with this method you send report via email
-- Fix \*__str__* method on **Report** class
-
-## 1.1.0
-Jun 5, 2021
-
-- Created abstract **File** class
-- Created **TextFile** class
-- Added *\__str__* method for pretty representation of **Executor** class
-- Added *\__repr__* method for representation of **DatabaseManager** class
-- Added *\__repr__* method for representation of **FileManager** class
-- Added *\__repr__* method for representation of **LdapManager** class
-- Fix documentation for new abstract **File** class
-
-## 1.0.0
-May 26, 2021
-
-- Created abstract **Connection** class
-- Created **\*Connection** classes
-- Created **\*File** classes
-- Created **FileManager**, **DatabaseManager** and **LdapManager** classes
-- Created **Executor** class
-- Created **Report** class
-- Created **ReportBook** class
-- Created **average**, **most_common**, **percentage**, **counter**, **aggregate**, **merge**, **chunks**, functions
```

### Comparing `pyreports-1.5.1/README.md` & `pyreports-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyreports-1.5.1/__info__.py` & `pyreports-1.6.0/tests/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
-# __info__ -- pyreports
+# __init__ -- pyreports
 #
 #     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
@@ -15,14 +15,7 @@
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""Information variable used by modules on this package."""
-
-__version__ = '1.5.1'
-__author__ = 'Matteo Guadrini'
-__email__ = 'matteo.guadrini@hotmail.it'
-__homepage__ = 'https://github.com/MatteoGuadrini/pyreports'
```

### Comparing `pyreports-1.5.1/pyreports/__init__.py` & `pyreports-1.6.0/pyreports/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # __init__ -- pyreports
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -18,12 +18,12 @@
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Build complex pyreports from/to various formats."""
 
-from .io import manager
+from .io import manager, READABLE_MANAGER, WRITABLE_MANAGER
 from .core import Executor, Report, ReportBook
 from .exception import ReportDataError, ReportManagerError
-from .datatools import average, most_common, percentage, counter, aggregate, chunks, merge
+from .datatools import average, most_common, percentage, counter, aggregate, chunks, merge, deduplicate
 from .cli import make_manager, get_data, load_config, validate_config
```

### Comparing `pyreports-1.5.1/pyreports/cli.py` & `pyreports-1.6.0/pyreports/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # cli -- pyreports
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -63,15 +63,15 @@
     args = parser.parse_args()
     filename = args.config.name
 
     # Check if file is a YAML file
     try:
         args.config = load_config(args.config)
     except yaml.YAMLError as err:
-        parser.error(f'file {args.config} is not a valid YAML file: {err}')
+        parser.error(f'file {filename} is not a valid YAML file: \n{err}')
 
     # Validate config file
     try:
         validate_config(args.config)
     except yaml.YAMLError as err:
         parser.error(str(err))
 
@@ -98,15 +98,17 @@
     """
     try:
         reports = config['reports']
         if reports is None or not isinstance(reports, list):
             raise yaml.YAMLError('"reports" section have not "report" list sections')
         datas = all([bool(report.get('report').get('input')) for report in reports])
         if not datas:
-            raise yaml.YAMLError('one of "report" section does not have "input" section')
+            raise yaml.YAMLError(
+                'one of "report" section does not have "input" section'
+            )
     except KeyError as err:
         raise yaml.YAMLError(f'there is no "{err}" section')
     except AttributeError:
         raise yaml.YAMLError('correctly indents the "report" section or "report" section not exists')
 
 
 def make_manager(input_config):
@@ -141,27 +143,29 @@
         if params and isinstance(params, (list, tuple)):
             data = manager.read(*params)
         elif params and isinstance(params, dict):
             data = manager.read(**params)
         else:
             data = manager.read()
     # DatabaseManager
-    elif manager.type == 'database':
+    elif manager.type == 'sql':
         if params and isinstance(params, (list, tuple)):
-            data = manager.execute(*params)
+            manager.execute(*params)
+            data = manager.fetchall()
         elif params and isinstance(params, dict):
-            data = manager.execute(**params)
+            manager.execute(**params)
+            data = manager.fetchall()
     # LdapManager
     elif manager.type == 'ldap':
         if params and isinstance(params, (list, tuple)):
             data = manager.query(*params)
         elif params and isinstance(params, dict):
             data = manager.query(**params)
     # NosqlManager
-    else:
+    elif manager.type == 'nosql':
         if params and isinstance(params, (list, tuple)):
             data = manager.find(*params)
         elif params and isinstance(params, dict):
             data = manager.find(**params)
 
     return data
 
@@ -182,46 +186,50 @@
 
     # Get command line args
     args = get_args()
     # Take reports
     config = args.config
     reports = config.get('reports', ())
 
-    print_verbose(f'found {len(config.get("reports", ()))} report(s)', verbose=args.verbose)
+    print_verbose(f'found {len(config.get("reports", ()))} report(s)',
+                  verbose=args.verbose)
 
     # Build the data and report
     for report in reports:
         # Check if report isn't in excluded list
         if args.exclude and report.get('report').get('title') in args.exclude:
-            print_verbose(f'exclude report "{report.get("report").get("title")}"', verbose=args.verbose)
+            print_verbose(f'exclude report "{report.get("report").get("title")}"',
+                          verbose=args.verbose)
             continue
         # Make a manager object
         input_ = report.get('report').get('input')
-        print_verbose(f'make an input manager of type {input_.get("manager")}', verbose=args.verbose)
+        print_verbose(f'make an input manager of type {input_.get("manager")}',
+                      verbose=args.verbose)
         manager = make_manager(input_)
         # Get data
         print_verbose(f'get data from manager {manager}', verbose=args.verbose)
-        report_ = pyreports.Report(tablib.Dataset())
         try:
             # Make a report object
             data = get_data(manager, input_.get('params'))
             if 'map' in report.get('report'):
                 exec(report.get('report').get('map'))
             map_func = globals().get('map_func')
             report_ = pyreports.Report(
                 input_data=data,
                 title=report.get('report').get('title'),
                 filters=report.get('report').get('filters'),
                 map_func=map_func,
+                negation=report.get('report').get('negation', False),
                 column=report.get('report').get('column'),
                 count=report.get('report').get('count', False),
                 output=make_manager(report.get('report').get('output')) if 'output' in report.get('report') else None
             )
             print_verbose(f'created report "{report_.title}"', verbose=args.verbose)
         except Exception as err:
+            pyreports.Report(tablib.Dataset())
             exit(f'error: {err}')
         # Check output
         if report_.output:
             # Check if export or send report
             if report.get('report').get('mail'):
                 print_verbose(f'send report to {report.get("report").get("mail").get("to")}', verbose=args.verbose)
                 mail_settings = report.get('report').get('mail')
@@ -234,19 +242,20 @@
                     subject=mail_settings.get('subject'),
                     body=mail_settings.get('body'),
                     auth=tuple(mail_settings.get('auth')) if 'auth' in mail_settings else None,
                     _ssl=bool(mail_settings.get('ssl')),
                     headers=mail_settings.get('headers')
                 )
             else:
-                print_verbose(f'export report to {report_.output.data.file}', verbose=args.verbose)
+                print_verbose(f'export report to {report_.output}',
+                              verbose=args.verbose)
                 report_.export()
         else:
             # Print report in stdout
-            print_verbose(f'print report to stdout', verbose=args.verbose)
+            print_verbose('print report to stdout', verbose=args.verbose)
             title = report.get('report').get('title')
             report_.exec()
             print(f"{title}\n{'=' * len(title)}\n")
             print(report_)
 
 
 # endregion
```

### Comparing `pyreports-1.5.1/pyreports/core.py` & `pyreports-1.6.0/pyreports/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # core -- pyreports
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -27,33 +27,47 @@
 import ssl
 import tablib
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email import encoders
 from email.mime.base import MIMEBase
-from .io import FileManager
-from .exception import ReportManagerError, ReportDataError
+from .io import Manager, WRITABLE_MANAGER
+from .exception import ReportManagerError, ReportDataError, ExecutorError
 
 
 # endregion
 
 # region Classes
 
 class Executor:
-
     """Executor receives, processes, transforms and writes data"""
 
     def __init__(self, data, header=None):
         """Create Executor object
 
         :param data: everything type of data
         :param header: list header of data
         """
-        self.data = tablib.Dataset(*data) if not isinstance(data, tablib.Dataset) else data
+        # Check type of input data
+        err_msg = "input data must be a Dataset, tuple, list, List[dict] or List[tuple] object"
+        if isinstance(data, (tuple, list)):
+            if all((isinstance(obj, (tuple, list)) for obj in data)):
+                self.data = tablib.Dataset(*data)
+            elif not all((isinstance(obj, (tuple, list)) for obj in data)):
+                self.data = tablib.Dataset()
+                self.data.append(data)
+            else:
+                raise ExecutorError(err_msg)
+        elif isinstance(data, dict):
+            self.data = tablib.Dataset(*list(data.values()))
+        elif isinstance(data, tablib.Dataset):
+            self.data = data
+        else:
+            raise ExecutorError(err_msg)
         # Set header
         if header or header is None:
             self.headers(header)
         self.origin = tablib.Dataset()
         self.origin.extend(self.data)
 
     def __len__(self):
@@ -122,37 +136,47 @@
         """Set header
 
         :param header: header of data
         :return: None
         """
         self.data.headers = header
 
-    def filter(self, flist=None, key=None, column=None):
+    def filter(self, flist=None, key=None, column=None, negation=False):
         """Filter data through a list of strings (equal operator) and/or function key
 
         :param flist: list of strings
         :param key: function that takes a single argument and returns data
         :param column: select column name or index number
+        :param negation: enable negation for flist or key
         :return: None
         """
         if flist is None:
             flist = []
         ret_data = tablib.Dataset(headers=self.data.headers)
         # Filter data through filter list
         for row in self:
             for f in flist:
-                if f in row:
-                    ret_data.append(row)
-                    break
-            # Filter data through function
-            if key and callable(key):
-                for field in row:
-                    if bool(key(field)):
+                if negation:
+                    if f not in row:
+                        ret_data.append(row)
+                        break
+                else:
+                    if f in row:
                         ret_data.append(row)
                         break
+            # Filter data through function (key)
+            if key and callable(key):
+                if negation:
+                    if not any([bool(key(field)) for field in row]):
+                        ret_data.append(row)
+                        continue
+                else:
+                    if any([bool(key(field)) for field in row]):
+                        ret_data.append(row)
+                        continue
         self.data = ret_data
         # Single column
         if column and self.data.headers:
             self.data = self.select_column(column)
 
     def map(self, key, column=None):
         """Apply function to data
@@ -223,50 +247,55 @@
 
         :return: executor
         """
         return Executor(self.origin, header=self.origin.headers)
 
 
 class Report:
-
     """Report represents the workflow for generating a report"""
 
     def __init__(self,
                  input_data: tablib.Dataset,
                  title=None,
                  filters=None,
                  map_func=None,
+                 negation=False,
                  column=None,
                  count=False,
-                 output: FileManager = None):
+                 output: Manager = None):
         """Create Report object
 
         :param input_data: Dataset object
         :param title: title of Report object
         :param filters: list or function for filter data
         :param map_func: function for modifying data
+        :param negation: enable negation for filters or map_func
         :param column: select column name or index
         :param count: count rows
-        :param output: FileManager object
+        :param output: Manager object
         """
         # Discard all objects that are not Datasets
         if isinstance(input_data, tablib.Dataset):
             self.data = input_data
         else:
             raise ReportDataError('Only Dataset object is allowed for input')
         # Set other arguments
         self.title = title
         self.filter = filters
         self.map = map_func
+        self.negation = negation
         self.column = column
         self.count = bool(count)
-        if isinstance(output, FileManager) or output is None:
+        if isinstance(output, Manager) or output is None:
+            if output:
+                if output.__class__.__name__ not in WRITABLE_MANAGER:
+                    raise ReportManagerError(f'Only {WRITABLE_MANAGER} object is allowed for output')
             self.output = output
         else:
-            raise ReportManagerError('Only FileManager object is allowed for output')
+            raise ReportManagerError('Only Manager object is allowed for output')
         # Data for report
         self.report = None
 
     def __repr__(self):
         """Representation of Report object
 
         :return: string
@@ -331,37 +360,56 @@
         ex = Executor(self.data, header=self.data.headers)
         # Apply map function
         if self.map:
             ex.map(self.map)
         # Apply filters
         if self.filter:
             if callable(self.filter):
-                ex.filter(key=self.filter)
+                ex.filter(key=self.filter, negation=self.negation)
             else:
-                ex.filter(self.filter)
+                ex.filter(self.filter, negation=self.negation)
         # Count element
         if bool(self.count):
             self.count = len(ex)
         self.report = ex.get_data()
 
     def export(self):
         """Process and save data on output
 
         :return: if count is True, return row count
         """
         # Process data before export
         self.exec()
-        # Verify if output is FileManager object
-        if isinstance(self.output, FileManager) or self.output is None:
-            if self.output:
+        if self.output is not None:
+            if self.output.type == 'file':
                 self.output.write(self.report)
-            else:
-                print(self)
+            elif self.output.type == 'sql':
+                if not self.report.headers:
+                    raise ReportDataError("Dataset object doesn't have a header")
+                table_name = self.title.replace(' ', '_').lower()
+                fields = ','.join([
+                    f'{field} VARCHAR(255)'
+                    for field in self.report.headers
+                ])
+                # Create table with header
+                self.output.execute(
+                    f"CREATE TABLE IF NOT EXISTS {table_name} ({fields});"
+                )
+                # Insert data into table
+                table_header = ','.join(field for field in self.report.headers)
+                for row in self.report:
+                    row_table = [f"'{element}'" for element in row]
+                    self.output.execute(
+                        f"INSERT INTO {table_name} "
+                        f"({table_header}) "
+                        f"VALUES ({','.join(element for element in row_table)});"
+                    )
+                self.output.commit()
         else:
-            raise ReportManagerError('the output object must be FileManager or NoneType object')
+            print(self)
 
     def send(self, server, _from, to, cc=None, bcc=None, subject=None, body='', auth=None, _ssl=True, headers=None):
         """Send saved report to email
 
         :param server: server SMTP
         :param _from: email address 'from:'
         :param to: email address 'to:'
@@ -389,15 +437,15 @@
         if headers:
             if all([isinstance(header, (tuple, list)) for header in headers]):
                 for header in headers:
                     message.add_header(*header)
             elif isinstance(headers, (tuple, list)):
                 message.add_header(*headers)
             else:
-                raise ValueError(f'headers must be tuple or List[tuple]')
+                raise ValueError('headers must be tuple or List[tuple]')
 
         # Prepare body
         part = MIMEText(body, "html")
         message.attach(part)
 
         # Prepare attachment
         self.export()
@@ -417,19 +465,18 @@
         else:
             port = smtplib.SMTP_PORT
             protocol = smtplib.SMTP
             kwargs = {}
         with protocol(server, port, **kwargs) as srv:
             if auth:
                 srv.login(*auth)
-            srv.sendmail(_from, to, message.as_string())
+            srv.sendmail(_from, [receiver for receiver in (to, cc, bcc) if receiver], message.as_string())
 
 
 class ReportBook:
-
     """ReportBook represent a collection of Report's object"""
 
     def __init__(self, reports=None, title=None):
         """Create a ReportBook object
 
         :param reports: Report's object list
         :param title: title of report book
```

### Comparing `pyreports-1.5.1/pyreports/datatools.py` & `pyreports-1.6.0/pyreports/datatools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # datatools -- pyreports
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -116,24 +116,24 @@
     :param columns: columns added
     :param fill_empty: fill the empty field of data with "fill_value" argument
     :param fill_value: fill value for empty field if "fill_empty" argument is specified
     :return: Dataset
     """
     if len(columns) >= 2:
         new_data = Dataset()
-        # Check len of all columns
-        last_list = columns[0]
-        for list_ in columns[1:]:
+        # Check max len of all columns
+        max_len = max([len(column) for column in columns])
+        for list_ in columns:
             if fill_empty:
-                while len(last_list) != len(list_):
+                while max_len != len(list_):
                     list_.append(fill_value() if callable(fill_value) else fill_value)
             else:
-                if len(last_list) != len(list_):
+                if max_len != len(list_):
                     raise InvalidDimensions('the columns are not the same length')
-                last_list = list_
+                max_len = len(list_)
         # Aggregate columns
         for column in columns:
             new_data.append_col(column)
         return new_data
     else:
         raise ReportDataError('you can aggregate two or more columns')
 
@@ -164,8 +164,18 @@
 
     :param data: Dataset object
     :param length: n-sized chunks
     :return: generator
     """
     for i in range(0, len(data), length):
         yield data[i:i + length]
+
+
+def deduplicate(data):
+    """Remove duplicated rows
+
+    :param data: Dataset object
+    :return: Dataset
+    """
+    return Dataset(*list(dict.fromkeys(data)))
+
 # endregion
```

### Comparing `pyreports-1.5.1/pyreports/exception.py` & `pyreports-1.6.0/pyreports/exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # exception.py -- pyreports
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -19,14 +19,18 @@
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Contains all custom exception."""
 
 
+class ExecutorError(Exception):
+    pass
+
+
 # ReportException hierarchy
 class ReportException(Exception):
     pass
 
 
 class ReportDataError(ReportException):
     pass
```

### Comparing `pyreports-1.5.1/pyreports/io.py` & `pyreports-1.6.0/pyreports/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # io -- pyreports
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -28,24 +28,24 @@
 import nosqlapi
 import pymssql
 import mysql.connector as mdb
 import psycopg2
 import tablib
 import ldap3
 import re
-from nosqlapi import Manager
+from nosqlapi import Manager as APIManager
+from nosqlapi import Connection as APIConnection
 from abc import ABC, abstractmethod
 
 
 # endregion
 
 
 # region Classes
 class Connection(ABC):
-
     """Connection base class"""
 
     def __init__(self, *args, **kwargs):
         """Connection base object."""
 
         self.connection = None
         self.cursor = None
@@ -70,15 +70,14 @@
         if self.cursor:
             return (e for e in self.cursor)
         else:
             return iter([])
 
 
 class File(ABC):
-
     """File base class"""
 
     def __init__(self, filename):
         """File base object
 
         :param filename: file path
         """
@@ -109,16 +108,20 @@
 
     def __iter__(self):
         with open(self.file) as file:
             for line in file:
                 yield line
 
 
-class TextFile(File):
+class Manager(ABC):
+    """Manager base class"""
+    pass
 
+
+class TextFile(File):
     """Text file class"""
 
     def write(self, data):
         """Write data on file
 
         :param data: data to write on file
         :return: None
@@ -137,15 +140,14 @@
         with open(self.file) as file:
             for line in file:
                 data.append([line.strip('\n')])
         return data
 
 
 class LogFile(File):
-
     """Log file class"""
 
     def write(self, data):
         """Write data on file
 
         :param data: data to write on file
         :return: None
@@ -170,15 +172,14 @@
                         data.append(*result)
                     else:
                         data.append([result])
         return data
 
 
 class CsvFile(File):
-
     """CSV file class"""
 
     def write(self, data):
         """Write data on csv file
 
         :param data: data to write on csv file
         :return: None
@@ -194,15 +195,14 @@
         :return: Dataset object
         """
         with open(self.file) as file:
             return tablib.Dataset().load(file, **kwargs)
 
 
 class JsonFile(File):
-
     """JSON file class"""
 
     def write(self, data):
         """Write data on json file
 
         :param data: data to write on json file
         :return: None
@@ -218,15 +218,14 @@
         :return: Dataset object
         """
         with open(self.file) as file:
             return tablib.Dataset().load(file, **kwargs)
 
 
 class YamlFile(File):
-
     """YAML file class"""
 
     def write(self, data):
         """Write data on yaml file
 
         :param data: data to write on yaml file
         :return: None
@@ -242,15 +241,14 @@
         :return: Dataset object
         """
         with open(self.file) as file:
             return tablib.Dataset().load(file, **kwargs)
 
 
 class ExcelFile(File):
-
     """Excel file class"""
 
     def write(self, data):
         """Write data on xlsx file
 
         :param data: data to write on yaml file
         :return: None
@@ -265,76 +263,71 @@
 
         :return: Dataset object
         """
         with open(self.file, 'rb') as file:
             return tablib.import_set(file, **kwargs)
 
 
-class SQLliteConnection(Connection):
-
+class SQLiteConnection(Connection):
     """Connection sqlite class"""
 
     def connect(self):
         self.connection = sqlite3.connect(*self.args, **self.kwargs)
         self.cursor = self.connection.cursor()
 
     def close(self):
         self.connection.close()
         self.cursor.close()
 
 
 class MSSQLConnection(Connection):
-
     """Connection microsoft sql class"""
 
     def connect(self):
         self.connection = pymssql.connect(*self.args, **self.kwargs)
         self.cursor = self.connection.cursor()
 
     def close(self):
         self.connection.close()
         self.cursor.close()
 
 
 class MySQLConnection(Connection):
-
     """Connection mysql class"""
 
     def connect(self):
         self.connection = mdb.connect(*self.args, **self.kwargs)
         self.cursor = self.connection.cursor()
 
     def close(self):
         self.connection.close()
         self.cursor.close()
 
 
 class PostgreSQLConnection(Connection):
-
     """Connection postgresql class"""
 
     def connect(self):
         self.connection = psycopg2.connect(*self.args, **self.kwargs)
         self.cursor = self.connection.cursor()
 
     def close(self):
         self.connection.close()
         self.cursor.close()
 
 
-class DatabaseManager:
-
+class DatabaseManager(Manager):
     """Database manager class for SQL connection"""
 
     def __init__(self, connection: Connection):
         """Database manager object for SQL connection
 
         :param connection: Connection based object
         """
-        self.type = 'database'
+        self.type = 'sql'
         self.connector = connection
         # Connect database
         self.connector.connect()
         # Set description
         self.description = None
         self.data = None
         # Row properties
@@ -342,15 +335,17 @@
         self.rowcount = 0
 
     def __repr__(self):
         """Representation of DatabaseManager object
 
         :return: string
         """
-        return f"<{self.__class__.__name__} object, connection={self.connector.__class__.__name__}>"
+        ret = f"<{self.__class__.__name__} object, "
+        ret += f"connection={self.connector.__class__.__name__}>"
+        return ret
 
     def __iter__(self):
         if self.connector.cursor:
             return (e for e in self.connector.cursor)
         else:
             return iter([])
 
@@ -367,15 +362,18 @@
     def execute(self, query, params=None):
         """Execute query on database cursor
 
         :param query: SQL query language
         :param params: parameters of the query
         :return: None
         """
-        self.connector.cursor.execute(query, params)
+        if params:
+            self.connector.cursor.execute(query, params)
+        else:
+            self.connector.cursor.execute(query)
         # Set last row id
         self.lastrowid = self.connector.cursor.lastrowid
         # Set row cont
         self.rowcount = self.connector.cursor.rowcount
         # Set description
         self.description = self.connector.cursor.description
 
@@ -446,20 +444,25 @@
         """This method sends a COMMIT statement to the server
 
         :return: None
         """
         self.connector.connection.commit()
 
 
-class NoSQLManager(Manager):
-
+class NoSQLManager(Manager, APIManager):
     """Database manager class for NOSQL connection"""
 
+    def __init__(self, connection: APIConnection, *args, **kwargs):
+        APIManager.__init__(self, connection, *args, **kwargs)
+        self.type = 'nosql'
+
     @staticmethod
-    def _response_to_dataset(obj: Union[List[tuple], List[list], dict, nosqlapi.Response]) -> tablib.Dataset:
+    def _response_to_dataset(
+            obj: Union[List[tuple], List[list], dict, nosqlapi.Response]
+    ) -> tablib.Dataset:
         """Transform receive data into Dataset object"""
         data = tablib.Dataset()
         if isinstance(obj, (list, tuple)):
             data = tablib.Dataset([row for row in obj])
         elif isinstance(obj, dict):
             data = tablib.Dataset([obj[key] for key in obj], headers=list(obj.keys()))
         elif isinstance(obj, nosqlapi.Response):
@@ -477,16 +480,15 @@
         return self._response_to_dataset(self.session.get(*args, **kwargs))
 
     def find(self, *args, **kwargs) -> tablib.Dataset:
         """Find data from database session"""
         return self._response_to_dataset(self.session.find(*args, **kwargs))
 
 
-class FileManager:
-
+class FileManager(Manager):
     """File manager class for various readable file format"""
 
     def __init__(self, file: File):
         """File manager object for various readable file format
 
         :param file: file object
         """
@@ -521,45 +523,48 @@
         if pattern:
             data = self.data.read(pattern=pattern, **kwargs)
         else:
             data = self.data.read(**kwargs)
         return data
 
 
-class LdapManager:
-
+class LdapManager(Manager):
     """LDAP manager class"""
 
     def __init__(self, server, username, password, ssl=False, tls=True):
         """LDAP manager object
 
         :param server: fqdn server name or ip address
         :param username: username for bind operation
         :param password: password of the username used for bind operation
         :param ssl: disable or enable SSL. Default is False.
         :param tls: disable or enable TLS. Default is True.
         """
         self.type = 'ldap'
         # Check ssl connection
         port = 636 if ssl else 389
-        self.connector = ldap3.Server(server, get_info=ldap3.ALL, port=port, use_ssl=ssl)
+        self.connector = ldap3.Server(server,
+                                      get_info=ldap3.ALL,
+                                      port=port,
+                                      use_ssl=ssl)
         # Check tls connection
         self.auto_bind = ldap3.AUTO_BIND_TLS_BEFORE_BIND if tls else ldap3.AUTO_BIND_NONE
         # Create a bind connection with user and password
         self.bind = ldap3.Connection(self.connector, user=f'{username}', password=f'{password}',
                                      auto_bind=self.auto_bind, raise_exceptions=True)
         self.bind.bind()
 
     def __repr__(self):
         """Representation of LdapManager object
 
         :return: string
         """
         obj_repr = f"<{self.__class__.__name__} object, "
-        obj_repr += f"server={self.connector.host}, ssl={self.connector.ssl}, tls={self.connector.tls}>"
+        obj_repr += f"server={self.connector.host}, "
+        obj_repr += f"ssl={self.connector.ssl}, tls={self.connector.tls}>"
         return obj_repr
 
     def rebind(self, username, password):
         """Re-bind with specified username and password
 
         :param username: username for bind operation
         :param password: password of the username used for bind operation
@@ -602,29 +607,33 @@
 
 
 # endregion
 
 
 # region Variables
 DBTYPE = {
-    'sqlite': SQLliteConnection,
+    'sqlite': SQLiteConnection,
     'mssql': MSSQLConnection,
     'mysql': MySQLConnection,
     'postgresql': PostgreSQLConnection
 }
 
 FILETYPE = {
     'file': TextFile,
     'log': LogFile,
     'csv': CsvFile,
     'json': JsonFile,
     'yaml': YamlFile,
     'xlsx': ExcelFile,
 }
 
+READABLE_MANAGER = ('FileManager', 'DatabaseManager', 'LdapManager', 'NoSQLManager')
+
+WRITABLE_MANAGER = ('FileManager', 'DatabaseManager', 'NoSQLManager')
+
 
 # endregion
 
 
 # region Functions
 def create_database_manager(dbtype, *args, **kwargs):
     """Creates a DatabaseManager object
@@ -666,15 +675,15 @@
     """Creates a NoSQLManager object
 
     :param connection: Connection object
     :return: NoSQLManager
     """
     # Check if connection class is API compliant with nosqlapi
     if not hasattr(connection, 'connect'):
-        raise nosqlapi.ConnectError('the connection class is not API compliant. see https://nosqlapi.rtfd.io/')
+        raise nosqlapi.ConnectError('the Connection class is not API compliant. See https://nosqlapi.rtfd.io/')
     # Create NoSQLManager object
     return NoSQLManager(connection=connection, *args, **kwargs)
 
 
 def manager(datatype, *args, **kwargs):
     """Creates manager object based on datatype
```

### Comparing `pyreports-1.5.1/pyreports.egg-info/PKG-INFO` & `pyreports-1.6.0/pyreports.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: pyreports
-Version: 1.5.1
-Summary: pyreports is a python library that allows you to create complex report from various sources
+Version: 1.6.0
+Summary: pyreports is a python library that allows you to create complex report from various sources.
 Home-page: https://github.com/MatteoGuadrini/pyreports
 Author: Matteo Guadrini
-Author-email: matteo.guadrini@hotmail.it
+Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer: Matteo Guadrini
-Maintainer-email: matteo.guadrini@hotmail.it
+Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 License: GNU General Public License v3.0
-Keywords: pyreports reports report csv yaml export excel database ldap dataset file executor book
+Project-URL: homepage, https://github.com/MatteoGuadrini/pyreports'
+Project-URL: documentation, https://pyreports.readthedocs.io/en/latest/
+Project-URL: repository, https://github.com/MatteoGuadrini/pyreports/pyreports.git
+Project-URL: changelog, https://github.com/MatteoGuadrini/pyreports/blob/master/CHANGES.md
+Keywords: pyreports,reports,report,csv,yaml,export,excel,database,ldap,dataset,file,executor,book
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -264,76 +268,7 @@
 
 Thanks to Dane Hillard for writing the _Practices of the Python Pro_ books.
 
 Special thanks go to my wife, who understood the hours of absence for this development. 
 Thanks to my children, for the daily inspiration they give me and to make me realize, that life must be simple.
 
 Thanks Python!
-# Release notes
-
-## 1.5.0
-Aug 4, 2022
-
-- Added **cli** module
-- Added **reports** cli
-- Added **\__getitem\__** method on _Report_ class
-- Added **\__delitem\__** method on _Report_ class
-- Added **\__getitem\__** method on _ReportBook_ class
-- Added **\__delitem\__** method on _ReportBook_ class
-- Added **\__contains\__** on _Executor_ class
-- Fix **NoSQLManager** creation into _manager_ function
-- Fix **print_data** on _Report_ class
-
-## 1.4.0
-Jun 27, 2022
-
-- Added **\__bool\__** method on _Report_ class
-- Added **\__iter\__** method on _Report_ class
-- Added **\__bool\__** method on _ReportBook_ class
-- Added **\__iter\__** method on _Connection_ and _File_ classes
-- Added **\__iter\__** method on _FileManager_ class
-- Added **\__iter\__** method on _DatabaseManager_ class
-- Added **\__getitem\__** on _Executor_ class
-- Added **\__delitem\__** on _Executor_ class
-- Fix name of attachment on **send** method of _Report_ class
-- Fix **write** method on _LogFile_ class
-
-## 1.3.0
-Apr 15, 2022
-
-- Added **NoSQLManager** class; this class extend _Manager_ class on the [nosqlapi](https://github.com/MatteoGuadrini/nosqlapi) package
-- Added **LogFile** class; this class load a log file and _read_ method accept regular expression
-- Added **\__bool\__** and **\__repr\__** method on _File_ and _Connection_ abstract classes
-- Fix documentation API section
-- Fix tests package
-- Fix CircleCi docker image
-
-## 1.2.0
-Aug 5, 2021
-
-- Added _fill_value_ argument on **aggregate** function; this value also is callable without arguments
-- Added _send_ method on **Report** class; with this method you send report via email
-- Added _send_ method on **ReportBook** class; with this method you send report via email
-- Fix \*__str__* method on **Report** class
-
-## 1.1.0
-Jun 5, 2021
-
-- Created abstract **File** class
-- Created **TextFile** class
-- Added *\__str__* method for pretty representation of **Executor** class
-- Added *\__repr__* method for representation of **DatabaseManager** class
-- Added *\__repr__* method for representation of **FileManager** class
-- Added *\__repr__* method for representation of **LdapManager** class
-- Fix documentation for new abstract **File** class
-
-## 1.0.0
-May 26, 2021
-
-- Created abstract **Connection** class
-- Created **\*Connection** classes
-- Created **\*File** classes
-- Created **FileManager**, **DatabaseManager** and **LdapManager** classes
-- Created **Executor** class
-- Created **Report** class
-- Created **ReportBook** class
-- Created **average**, **most_common**, **percentage**, **counter**, **aggregate**, **merge**, **chunks**, functions
```

