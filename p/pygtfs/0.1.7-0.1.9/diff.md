# Comparing `tmp/pygtfs-0.1.7.tar.gz` & `tmp/pygtfs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygtfs-0.1.7.tar", last modified: Mon May  9 16:55:26 2022, max compression
+gzip compressed data, was "pygtfs-0.1.9.tar", last modified: Fri Jul 14 17:41:19 2023, max compression
```

## Comparing `pygtfs-0.1.7.tar` & `pygtfs-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.998129 pygtfs-0.1.7/
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      109 2020-01-31 02:06:40.000000 pygtfs-0.1.7/.gitignore
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      881 2021-11-21 17:58:42.000000 pygtfs-0.1.7/.travis.yml
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      188 2020-01-31 02:06:40.000000 pygtfs-0.1.7/CHANGELOG.md
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     2727 2022-05-09 16:55:25.998129 pygtfs-0.1.7/PKG-INFO
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     2046 2020-01-31 02:06:40.000000 pygtfs-0.1.7/README.md
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.998129 pygtfs-0.1.7/docs/
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     6762 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/Makefile
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     8447 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/conf.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     1755 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/gtfs2db.rst
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      148 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/gtfs_entities.rst
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     3105 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/index.rst
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      110 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/internal.rst
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      101 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/loader.rst
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     6701 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/make.bat
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      105 2020-01-31 02:06:41.000000 pygtfs-0.1.7/docs/schedule.rst
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     1088 2020-01-31 02:06:40.000000 pygtfs-0.1.7/license.txt
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.998129 pygtfs-0.1.7/pygtfs/
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      290 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/__init__.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      142 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs/_version.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      436 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/exceptions.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     3734 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/feed.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     2601 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/gtfs2db.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)    23160 2021-11-21 17:58:42.000000 pygtfs-0.1.7/pygtfs/gtfs_entities.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     5314 2021-05-30 04:08:42.000000 pygtfs-0.1.7/pygtfs/loader.py
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     3587 2021-05-30 04:08:42.000000 pygtfs-0.1.7/pygtfs/schedule.py
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.998129 pygtfs-0.1.7/pygtfs/test/
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)        0 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/__init__.py
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.994795 pygtfs-0.1.7/pygtfs/test/data/
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.998129 pygtfs-0.1.7/pygtfs/test/data/sample_feed/
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      139 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/agency.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      162 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/calendar.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       48 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/calendar_dates.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      104 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/fare_attributes.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       94 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/fare_rules.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       93 2021-05-30 04:08:42.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/feed_info.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      345 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/frequencies.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      355 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/routes.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       72 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/shapes.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     1201 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/stop_times.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      605 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/stops.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      210 2021-11-21 17:58:42.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/transfers.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      163 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/translations.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)      421 2020-01-31 02:06:41.000000 pygtfs-0.1.7/pygtfs/test/data/sample_feed/trips.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     5834 2021-11-21 17:58:42.000000 pygtfs-0.1.7/pygtfs/test/test.py
-drwxr-xr-x   0 jarondl   (1000) jarondl   (1000)        0 2022-05-09 16:55:25.998129 pygtfs-0.1.7/pygtfs.egg-info/
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     2727 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs.egg-info/PKG-INFO
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     1220 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs.egg-info/SOURCES.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)        1 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs.egg-info/dependency_links.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       49 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs.egg-info/entry_points.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       41 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs.egg-info/requires.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)        7 2022-05-09 16:55:25.000000 pygtfs-0.1.7/pygtfs.egg-info/top_level.txt
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       72 2020-01-31 02:06:40.000000 pygtfs-0.1.7/readthedocs.yml
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)       67 2022-05-09 16:55:25.998129 pygtfs-0.1.7/setup.cfg
--rw-r--r--   0 jarondl   (1000) jarondl   (1000)     1390 2021-05-30 04:24:29.000000 pygtfs-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.778858 pygtfs-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.770858 pygtfs-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.774858 pygtfs-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-14 17:41:06.000000 pygtfs-0.1.9/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 17:41:06.000000 pygtfs-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 17:41:06.000000 pygtfs-0.1.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 17:41:06.000000 pygtfs-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-14 17:41:19.778858 pygtfs-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-14 17:41:06.000000 pygtfs-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.774858 pygtfs-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/gtfs2db.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/gtfs_entities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/loader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 17:41:06.000000 pygtfs-0.1.9/docs/schedule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-14 17:41:06.000000 pygtfs-0.1.9/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.774858 pygtfs-0.1.9/pygtfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/gtfs2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23068 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/gtfs_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.778858 pygtfs-0.1.9/pygtfs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.770858 pygtfs-0.1.9/pygtfs/test/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.778858 pygtfs-0.1.9/pygtfs/test/data/sample_feed/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/agency.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/calendar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/calendar_dates.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/fare_attributes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/fare_rules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/feed_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/frequencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/routes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/shapes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/stop_times.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/stops.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/transfers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/translations.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/data/sample_feed/trips.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-14 17:41:06.000000 pygtfs-0.1.9/pygtfs/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:41:19.774858 pygtfs-0.1.9/pygtfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 17:41:19.000000 pygtfs-0.1.9/pygtfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 17:41:06.000000 pygtfs-0.1.9/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 17:41:19.778858 pygtfs-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 17:41:06.000000 pygtfs-0.1.9/setup.py
```

### Comparing `pygtfs-0.1.7/.travis.yml` & `pygtfs-0.1.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/PKG-INFO` & `pygtfs-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pygtfs
-Version: 0.1.7
+Version: 0.1.9
 Summary: Models GTFS data in a database.
 Home-page: https://github.com/jarondl/pygtfs
 Author: Yaron de Leeuw
 Author-email: me@jarondl.net
 License: MIT
 Keywords: gtfs
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -73,9 +72,7 @@
 Why fork?
 --------------
 - natively support several gtfs feeds per database
 - less SLOC, more DRY
 - add python3 support
 - renamed to a more generic name
 - will continue to maintain
-
-
```

### Comparing `pygtfs-0.1.7/README.md` & `pygtfs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/docs/Makefile` & `pygtfs-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/docs/conf.py` & `pygtfs-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/docs/gtfs2db.rst` & `pygtfs-0.1.9/docs/gtfs2db.rst`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/docs/index.rst` & `pygtfs-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/docs/make.bat` & `pygtfs-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/license.txt` & `pygtfs-0.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs/feed.py` & `pygtfs-0.1.9/pygtfs/feed.py`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs/gtfs2db.py` & `pygtfs-0.1.9/pygtfs/gtfs2db.py`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs/gtfs_entities.py` & `pygtfs-0.1.9/pygtfs/gtfs_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,21 +78,17 @@
         return float_value
     return in_range
 
 
 def _validate_float_none(*field_names):
     @validates(*field_names)
     def is_float_none(self, key, value):
-        try:
-            return float(value)
-        except ValueError:
-            if value is None or value == "":
-                return None
-            else:
-                raise
+        if value is None or value == "":
+            return None
+        return float(value)
     return is_float_none
 
 
 class Feed(Base):
     __tablename__ = '_feed'
     _plural_name_ = 'feeds'
     feed_id = Column(Integer, primary_key=True)
```

### Comparing `pygtfs-0.1.7/pygtfs/loader.py` & `pygtfs-0.1.9/pygtfs/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,14 +85,37 @@
 
             try:
                 instance = gtfs_class(feed_id=feed_id, **record._asdict())
             except:
                 print("Failure while writing {0}".format(record))
                 raise
             schedule.session.add(instance)
+
+            if isinstance(instance, ServiceException):
+                service = schedule.session.execute(
+                    select(Service).where(Service.service_id == instance.service_id).where(Service.feed_id == feed_id)
+                ).one_or_none()
+                if service is None:
+                    # ServiceException was added for a day that has no associated regular service
+                    # Create a dummy service object for this service exception
+                    dummy = Service(
+                        feed_id=feed_id, 
+                        service_id=instance.service_id,
+                        monday='0',
+                        tuesday='0',
+                        wednesday='0',
+                        thursday='0',
+                        friday='0',
+                        saturday='0',
+                        sunday='0',
+                        start_date=instance.date.strftime('%Y%m%d'),
+                        end_date=instance.date.strftime('%Y%m%d'))
+                    schedule.session.add(dummy)
+                
+
             if i % chunk_size == 0 and i > 0:
                 schedule.session.flush()
                 sys.stdout.write('.')
                 sys.stdout.flush()
         print('%d record%s read for %s.' % ((i+1), '' if i == 0 else 's',
                                             gtfs_class))
     schedule.session.flush()
```

### Comparing `pygtfs-0.1.7/pygtfs/schedule.py` & `pygtfs-0.1.9/pygtfs/schedule.py`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs/test/data/sample_feed/stop_times.txt` & `pygtfs-0.1.9/pygtfs/test/data/sample_feed/stop_times.txt`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs/test/data/sample_feed/stops.txt` & `pygtfs-0.1.9/pygtfs/test/data/sample_feed/stops.txt`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs/test/test.py` & `pygtfs-0.1.9/pygtfs/test/test.py`

 * *Files identical despite different names*

### Comparing `pygtfs-0.1.7/pygtfs.egg-info/PKG-INFO` & `pygtfs-0.1.9/pygtfs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pygtfs
-Version: 0.1.7
+Version: 0.1.9
 Summary: Models GTFS data in a database.
 Home-page: https://github.com/jarondl/pygtfs
 Author: Yaron de Leeuw
 Author-email: me@jarondl.net
 License: MIT
 Keywords: gtfs
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -73,9 +72,7 @@
 Why fork?
 --------------
 - natively support several gtfs feeds per database
 - less SLOC, more DRY
 - add python3 support
 - renamed to a more generic name
 - will continue to maintain
-
-
```

### Comparing `pygtfs-0.1.7/pygtfs.egg-info/SOURCES.txt` & `pygtfs-0.1.9/pygtfs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .travis.yml
 CHANGELOG.md
 README.md
 license.txt
 readthedocs.yml
 setup.cfg
 setup.py
+.github/workflows/publish-to-pypi.yaml
 docs/Makefile
 docs/conf.py
 docs/gtfs2db.rst
 docs/gtfs_entities.rst
 docs/index.rst
 docs/internal.rst
 docs/loader.rst
```

### Comparing `pygtfs-0.1.7/setup.py` & `pygtfs-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     description='Models GTFS data in a database.',
     long_description=long_description,
     license='MIT',
     keywords='gtfs',
     url='https://github.com/jarondl/pygtfs',
     packages=find_packages(),
     install_requires=['sqlalchemy>=0.7.8',
-                      'pytz>=2012d',
+                      'pytz>=2014.9',
                       'six',
                       'docopt'
                       ],
     tests_require=['nose'],
     test_suite='nose.collector',
     setup_requires=['setuptools_scm'],
     use_scm_version={'write_to': os.path.join('pygtfs', '_version.py')},
```

