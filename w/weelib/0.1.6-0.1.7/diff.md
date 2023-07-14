# Comparing `tmp/weelib-0.1.6.tar.gz` & `tmp/weelib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weelib-0.1.6.tar", last modified: Fri Jul 14 10:45:30 2023, max compression
+gzip compressed data, was "weelib-0.1.7.tar", last modified: Fri Jul 14 13:16:20 2023, max compression
```

## Comparing `weelib-0.1.6.tar` & `weelib-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 10:45:30.937830 weelib-0.1.6/
--rw-r--r--   0 katry     (1000) katry     (1001)     5421 2023-07-14 10:45:30.937830 weelib-0.1.6/PKG-INFO
--rw-r--r--   0 katry     (1000) katry     (1001)     4774 2023-07-14 10:43:49.000000 weelib-0.1.6/README.md
--rw-r--r--   0 katry     (1000) katry     (1001)       38 2023-07-14 10:45:30.937830 weelib-0.1.6/setup.cfg
--rw-r--r--   0 katry     (1000) katry     (1001)     1230 2023-01-21 11:09:08.000000 weelib-0.1.6/setup.py
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 10:45:30.937830 weelib-0.1.6/src/
--rw-r--r--   0 katry     (1000) katry     (1001)       23 2023-07-14 10:43:57.000000 weelib-0.1.6/src/__init__.py
--rw-r--r--   0 katry     (1000) katry     (1001)     5806 2023-07-13 10:17:01.000000 weelib-0.1.6/src/validator.py
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 10:45:30.937830 weelib-0.1.6/weelib.egg-info/
--rw-r--r--   0 katry     (1000) katry     (1001)     5421 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/PKG-INFO
--rw-r--r--   0 katry     (1000) katry     (1001)      171 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/SOURCES.txt
--rw-r--r--   0 katry     (1000) katry     (1001)        1 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/dependency_links.txt
--rw-r--r--   0 katry     (1000) katry     (1001)        7 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/top_level.txt
+drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 13:16:20.053258 weelib-0.1.7/
+-rw-r--r--   0 katry     (1000) katry     (1001)     5421 2023-07-14 13:16:20.053258 weelib-0.1.7/PKG-INFO
+-rw-r--r--   0 katry     (1000) katry     (1001)     4774 2023-07-14 10:43:49.000000 weelib-0.1.7/README.md
+-rw-r--r--   0 katry     (1000) katry     (1001)       38 2023-07-14 13:16:20.053258 weelib-0.1.7/setup.cfg
+-rw-r--r--   0 katry     (1000) katry     (1001)     1230 2023-01-21 11:09:08.000000 weelib-0.1.7/setup.py
+drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 13:16:20.053258 weelib-0.1.7/src/
+-rw-r--r--   0 katry     (1000) katry     (1001)       23 2023-07-14 13:15:31.000000 weelib-0.1.7/src/__init__.py
+-rw-r--r--   0 katry     (1000) katry     (1001)     5884 2023-07-14 13:15:21.000000 weelib-0.1.7/src/validator.py
+drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 13:16:20.053258 weelib-0.1.7/weelib.egg-info/
+-rw-r--r--   0 katry     (1000) katry     (1001)     5421 2023-07-14 13:16:20.000000 weelib-0.1.7/weelib.egg-info/PKG-INFO
+-rw-r--r--   0 katry     (1000) katry     (1001)      171 2023-07-14 13:16:20.000000 weelib-0.1.7/weelib.egg-info/SOURCES.txt
+-rw-r--r--   0 katry     (1000) katry     (1001)        1 2023-07-14 13:16:20.000000 weelib-0.1.7/weelib.egg-info/dependency_links.txt
+-rw-r--r--   0 katry     (1000) katry     (1001)        7 2023-07-14 13:16:20.000000 weelib-0.1.7/weelib.egg-info/top_level.txt
```

### Comparing `weelib-0.1.6/PKG-INFO` & `weelib-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weelib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Additional functions for weepy framework.
 Home-page: https://gitlab.com/katry/weelib
 Author: Patrik Katrenak
 Author-email: patrik@katryapps.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `weelib-0.1.6/README.md` & `weelib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `weelib-0.1.6/setup.py` & `weelib-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `weelib-0.1.6/src/validator.py` & `weelib-0.1.7/src/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,21 +123,21 @@
 	def check(self, value) -> tuple[bool, ValidatorError | None, str]:
 		if type(value) != self.__type:
 			return False, ValidatorError.INVALID_TYPE, ""
 		elif (
 			(self.__min is not None and self.__min > value) or  # type: ignore
 			(self.__max is not None and self.__max < value)  # type: ignore
 		):
-			return False, ValidatorError.NUMBER_NOT_IN_RANGE, ""
+			return False, ValidatorError.NUMBER_NOT_IN_RANGE, "%s-%s" % (self.__min, self.__max)
 		elif (
 			(self.__length is not None and self.__length > len(value)) or  # type: ignore
 			(self.__min_length is not None and self.__min_length > len(value)) or  # type: ignore
 			(self.__max_length is not None and self.__max_length > len(value))  # type: ignore
 		):
-			return False, ValidatorError.NUMBER_NOT_IN_RANGE, ""
+			return False, ValidatorError.LENGTH_NOT_IN_RANGE, "%s-%s" % (self.__min_length, self.__max_length)
 		elif (
 			(self.__regex and not self.__regex.match(value)) or  # type: ignore
 			(self.__check_method and not self.__check_method(value))
 		):
 			return False, ValidatorError.INVALID_VALUE, ""
 		elif self.__validator:
 			self.__validator.check(value)  # type: ignore
```

### Comparing `weelib-0.1.6/weelib.egg-info/PKG-INFO` & `weelib-0.1.7/weelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weelib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Additional functions for weepy framework.
 Home-page: https://gitlab.com/katry/weelib
 Author: Patrik Katrenak
 Author-email: patrik@katryapps.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

