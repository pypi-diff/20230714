# Comparing `tmp/jumpavg-0.4.0.tar.gz` & `tmp/jumpavg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jumpavg-0.4.0.tar", last modified: Wed Jun  7 12:53:41 2023, max compression
+gzip compressed data, was "jumpavg-0.4.1.tar", last modified: Fri Jul 14 08:51:25 2023, max compression
```

## Comparing `jumpavg-0.4.0.tar` & `jumpavg-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-06-07 12:53:41.683740 jumpavg-0.4.0/
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)    11357 2023-06-07 12:43:39.000000 jumpavg-0.4.0/LICENSE
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2317 2023-06-07 12:53:41.683740 jumpavg-0.4.0/PKG-INFO
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     1363 2023-06-07 12:19:55.000000 jumpavg-0.4.0/README.md
-drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-06-07 12:53:41.683740 jumpavg-0.4.0/jumpavg/
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      879 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/__init__.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3454 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/avg_stdev_stats.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     5703 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/bit_counting_group.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     7440 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/bit_counting_group_list.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     6493 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/bit_counting_stats.py
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3928 2023-06-07 10:49:53.000000 jumpavg-0.4.0/jumpavg/classify.py
-drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-06-07 12:53:41.683740 jumpavg-0.4.0/jumpavg.egg-info/
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2317 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/PKG-INFO
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      318 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/SOURCES.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        1 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/dependency_links.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        8 2023-06-07 12:53:41.000000 jumpavg-0.4.0/jumpavg.egg-info/top_level.txt
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      995 2023-06-07 12:53:37.000000 jumpavg-0.4.0/pyproject.toml
--rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)       38 2023-06-07 12:53:41.683740 jumpavg-0.4.0/setup.cfg
+drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-07-14 08:51:25.834437 jumpavg-0.4.1/
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)    11357 2023-07-14 08:24:07.000000 jumpavg-0.4.1/LICENSE
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2401 2023-07-14 08:51:25.834437 jumpavg-0.4.1/PKG-INFO
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     1447 2023-07-14 08:24:12.000000 jumpavg-0.4.1/README.md
+drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-07-14 08:51:25.834437 jumpavg-0.4.1/jumpavg/
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      879 2023-07-14 08:24:07.000000 jumpavg-0.4.1/jumpavg/__init__.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3454 2023-07-14 08:24:07.000000 jumpavg-0.4.1/jumpavg/avg_stdev_stats.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     5703 2023-07-14 08:24:07.000000 jumpavg-0.4.1/jumpavg/bit_counting_group.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     7440 2023-07-14 08:24:07.000000 jumpavg-0.4.1/jumpavg/bit_counting_group_list.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     6742 2023-07-14 08:24:12.000000 jumpavg-0.4.1/jumpavg/bit_counting_stats.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     3928 2023-07-14 08:24:07.000000 jumpavg-0.4.1/jumpavg/classify.py
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      138 2023-07-13 12:45:58.000000 jumpavg-0.4.1/jumpavg/m.py
+drwxr-xr-x   0 vrpolak   (1000) vrpolak   (1000)        0 2023-07-14 08:51:25.834437 jumpavg-0.4.1/jumpavg.egg-info/
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)     2401 2023-07-14 08:51:25.000000 jumpavg-0.4.1/jumpavg.egg-info/PKG-INFO
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      331 2023-07-14 08:51:25.000000 jumpavg-0.4.1/jumpavg.egg-info/SOURCES.txt
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        1 2023-07-14 08:51:25.000000 jumpavg-0.4.1/jumpavg.egg-info/dependency_links.txt
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)        8 2023-07-14 08:51:25.000000 jumpavg-0.4.1/jumpavg.egg-info/top_level.txt
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)      995 2023-07-14 08:24:12.000000 jumpavg-0.4.1/pyproject.toml
+-rw-r--r--   0 vrpolak   (1000) vrpolak   (1000)       38 2023-07-14 08:51:25.834437 jumpavg-0.4.1/setup.cfg
```

### Comparing `jumpavg-0.4.0/LICENSE` & `jumpavg-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpavg-0.4.0/PKG-INFO` & `jumpavg-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumpavg
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library for locating changes in time series by grouping results.
 Author-email: "Cisco Systems Inc. and/or its affiliates" <csit-dev@lists.fd.io>
 Maintainer-email: Vratko Polak <vrpolak@cisco.com>, Tibor Frank <tifrank@cisco.com>
 Project-URL: Bug Tracker, https://jira.fd.io/projects/CSIT/issues
 Project-URL: Source, https://gerrit.fd.io/r/gitweb?p=csit.git;a=tree;f=PyPI/jumpavg
 Keywords: progression,regression,anomaly detection,statistics,bits
 Classifier: Development Status :: 3 - Alpha
@@ -39,14 +39,16 @@
 
 TODO.
 
 ## Change log
 
 TODO: Move into a separate file?
 
++ 0.4.1: Fixed bug of not penalizing large stdev enough (at all for size 2 stats).
+
 + 0.4.0: Added "unit" and "sbps" parameters so information content
   is reasonable even if sample values are below one.
 
 + 0.3.0: Considerable speedup by avoiding unneeded copy. Dataclasses used.
   Mostly API compatible, but repr looks different.
 
 + 0.2.0: API incompatible changes. Targeted to Python 3 now.
```

### Comparing `jumpavg-0.4.0/README.md` & `jumpavg-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 TODO.
 
 ## Change log
 
 TODO: Move into a separate file?
 
++ 0.4.1: Fixed bug of not penalizing large stdev enough (at all for size 2 stats).
+
 + 0.4.0: Added "unit" and "sbps" parameters so information content
   is reasonable even if sample values are below one.
 
 + 0.3.0: Considerable speedup by avoiding unneeded copy. Dataclasses used.
   Mostly API compatible, but repr looks different.
 
 + 0.2.0: API incompatible changes. Targeted to Python 3 now.
```

### Comparing `jumpavg-0.4.0/jumpavg/__init__.py` & `jumpavg-0.4.1/jumpavg/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpavg-0.4.0/jumpavg/avg_stdev_stats.py` & `jumpavg-0.4.1/jumpavg/avg_stdev_stats.py`

 * *Files identical despite different names*

### Comparing `jumpavg-0.4.0/jumpavg/bit_counting_group.py` & `jumpavg-0.4.1/jumpavg/bit_counting_group.py`

 * *Files identical despite different names*

### Comparing `jumpavg-0.4.0/jumpavg/bit_counting_group_list.py` & `jumpavg-0.4.1/jumpavg/bit_counting_group_list.py`

 * *Files identical despite different names*

### Comparing `jumpavg-0.4.0/jumpavg/bit_counting_stats.py` & `jumpavg-0.4.1/jumpavg/bit_counting_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,18 +93,21 @@
             norm = prev_avg * prev_avg
             norm -= (prev_avg - 1) * max_value
             norm += max_value * max_value / 2
             self.bits -= math.log((abs(avg - prev_avg) + 1) / norm, 2)
         if self.size < 2:
             return
         stdev = self.stdev / self.unit
-        # Stdev is considered to be uniformly distributed
-        # from zero to max_value. That is quite a bad expectation,
-        # but resilient to negative samples etc.
-        self.bits += math.log(max_value + 1, 2)
+        # Stdev can be anything between zero and max value.
+        # For size==2, sphere surface is 2 points regardless of radius,
+        # we need to penalize large stdev already when encoding the stdev.
+        # The simplest way is to use the same distribution as with size...
+        self.bits += math.log((stdev + 1) * (stdev + 2), 2)
+        # .. just with added normalization from the max value cut-off.
+        self.bits += math.log(1 - 1 / (max_value + 2), 2)
         # Now we know the samples lie on sphere in size-1 dimensions.
         # So it is (size-2)-sphere, with radius^2 == stdev^2 * size.
         # https://en.wikipedia.org/wiki/N-sphere
         sphere_area_ln = math.log(2)
         sphere_area_ln += math.log(math.pi) * ((self.size - 1) / 2)
         sphere_area_ln -= math.lgamma((self.size - 1) / 2)
         sphere_area_ln += math.log(stdev + 1) * (self.size - 2)
```

### Comparing `jumpavg-0.4.0/jumpavg/classify.py` & `jumpavg-0.4.1/jumpavg/classify.py`

 * *Files identical despite different names*

### Comparing `jumpavg-0.4.0/jumpavg.egg-info/PKG-INFO` & `jumpavg-0.4.1/jumpavg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumpavg
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library for locating changes in time series by grouping results.
 Author-email: "Cisco Systems Inc. and/or its affiliates" <csit-dev@lists.fd.io>
 Maintainer-email: Vratko Polak <vrpolak@cisco.com>, Tibor Frank <tifrank@cisco.com>
 Project-URL: Bug Tracker, https://jira.fd.io/projects/CSIT/issues
 Project-URL: Source, https://gerrit.fd.io/r/gitweb?p=csit.git;a=tree;f=PyPI/jumpavg
 Keywords: progression,regression,anomaly detection,statistics,bits
 Classifier: Development Status :: 3 - Alpha
@@ -39,14 +39,16 @@
 
 TODO.
 
 ## Change log
 
 TODO: Move into a separate file?
 
++ 0.4.1: Fixed bug of not penalizing large stdev enough (at all for size 2 stats).
+
 + 0.4.0: Added "unit" and "sbps" parameters so information content
   is reasonable even if sample values are below one.
 
 + 0.3.0: Considerable speedup by avoiding unneeded copy. Dataclasses used.
   Mostly API compatible, but repr looks different.
 
 + 0.2.0: API incompatible changes. Targeted to Python 3 now.
```

### Comparing `jumpavg-0.4.0/pyproject.toml` & `jumpavg-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jumpavg"
-version = "0.4.0"
+version = "0.4.1"
 description = "Library for locating changes in time series by grouping results."
 authors = [
     { name = "Cisco Systems Inc. and/or its affiliates", email = "csit-dev@lists.fd.io" },
 ]
 maintainers = [
     { name = "Vratko Polak", email = "vrpolak@cisco.com" },
     { name = "Tibor Frank", email = "tifrank@cisco.com" },
```

