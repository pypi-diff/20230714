# Comparing `tmp/weelib-0.1.5.tar.gz` & `tmp/weelib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weelib-0.1.5.tar", last modified: Sun Jan 22 01:22:53 2023, max compression
+gzip compressed data, was "weelib-0.1.6.tar", last modified: Fri Jul 14 10:45:30 2023, max compression
```

## Comparing `weelib-0.1.5.tar` & `weelib-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-01-22 01:22:53.230623 weelib-0.1.5/
--rw-r--r--   0 katry     (1000) katry     (1001)     5328 2023-01-22 01:22:53.230623 weelib-0.1.5/PKG-INFO
--rw-r--r--   0 katry     (1000) katry     (1001)     4681 2023-01-10 17:08:05.000000 weelib-0.1.5/README.md
--rw-r--r--   0 katry     (1000) katry     (1001)       38 2023-01-22 01:22:53.230623 weelib-0.1.5/setup.cfg
--rw-r--r--   0 katry     (1000) katry     (1001)     1230 2023-01-21 11:09:08.000000 weelib-0.1.5/setup.py
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-01-22 01:22:53.230623 weelib-0.1.5/src/
--rw-r--r--   0 katry     (1000) katry     (1001)       23 2023-01-22 01:04:52.000000 weelib-0.1.5/src/__init__.py
--rw-r--r--   0 katry     (1000) katry     (1001)     5858 2023-01-22 01:21:45.000000 weelib-0.1.5/src/validator.py
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-01-22 01:22:53.230623 weelib-0.1.5/weelib.egg-info/
--rw-r--r--   0 katry     (1000) katry     (1001)     5328 2023-01-22 01:22:53.000000 weelib-0.1.5/weelib.egg-info/PKG-INFO
--rw-r--r--   0 katry     (1000) katry     (1001)      171 2023-01-22 01:22:53.000000 weelib-0.1.5/weelib.egg-info/SOURCES.txt
--rw-r--r--   0 katry     (1000) katry     (1001)        1 2023-01-22 01:22:53.000000 weelib-0.1.5/weelib.egg-info/dependency_links.txt
--rw-r--r--   0 katry     (1000) katry     (1001)        7 2023-01-22 01:22:53.000000 weelib-0.1.5/weelib.egg-info/top_level.txt
+drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 10:45:30.937830 weelib-0.1.6/
+-rw-r--r--   0 katry     (1000) katry     (1001)     5421 2023-07-14 10:45:30.937830 weelib-0.1.6/PKG-INFO
+-rw-r--r--   0 katry     (1000) katry     (1001)     4774 2023-07-14 10:43:49.000000 weelib-0.1.6/README.md
+-rw-r--r--   0 katry     (1000) katry     (1001)       38 2023-07-14 10:45:30.937830 weelib-0.1.6/setup.cfg
+-rw-r--r--   0 katry     (1000) katry     (1001)     1230 2023-01-21 11:09:08.000000 weelib-0.1.6/setup.py
+drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 10:45:30.937830 weelib-0.1.6/src/
+-rw-r--r--   0 katry     (1000) katry     (1001)       23 2023-07-14 10:43:57.000000 weelib-0.1.6/src/__init__.py
+-rw-r--r--   0 katry     (1000) katry     (1001)     5806 2023-07-13 10:17:01.000000 weelib-0.1.6/src/validator.py
+drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2023-07-14 10:45:30.937830 weelib-0.1.6/weelib.egg-info/
+-rw-r--r--   0 katry     (1000) katry     (1001)     5421 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/PKG-INFO
+-rw-r--r--   0 katry     (1000) katry     (1001)      171 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/SOURCES.txt
+-rw-r--r--   0 katry     (1000) katry     (1001)        1 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/dependency_links.txt
+-rw-r--r--   0 katry     (1000) katry     (1001)        7 2023-07-14 10:45:30.000000 weelib-0.1.6/weelib.egg-info/top_level.txt
```

### Comparing `weelib-0.1.5/PKG-INFO` & `weelib-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weelib
-Version: 0.1.5
+Version: 0.1.6
 Summary: Additional functions for weepy framework.
 Home-page: https://gitlab.com/katry/weelib
 Author: Patrik Katrenak
 Author-email: patrik@katryapps.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -12,15 +12,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# weelib 
+# weelib
 <i>(experimental)</i><br>
 
 Library of additional functions for [`weepy`](https://gitlab.com/katry/weepy) framework.
 
 ## Installation
 
 <b>
@@ -72,20 +72,20 @@
 `ValidationError` provides enum of basic errors that may occur during validation -intended for extending to meet requirements of `_validate` wraps. <br>
 `ValidationError` contents:
 ```py
 from enum import Enum
 
 
 class ValidatorError(Enum):
-	MISSING_KEY = 1
-	INVALID_TYPE = 2
-	INVALID_VALUE = 3
-	NUMBER_NOT_IN_RANGE = 4
-	LENGTH_NOT_IN_RANGE = 5
-	INVALID_SCHEMA = 6
+	MISSING_KEY = "MISSING_KEY"
+	INVALID_TYPE = "INVALID_TYPE"
+	INVALID_VALUE = "INVALID_VALUE"
+	NUMBER_NOT_IN_RANGE = "NUMBER_NOT_IN_RANGE"
+	LENGTH_NOT_IN_RANGE = "LENGTH_NOT_IN_RANGE"
+	INVALID_SCHEMA = "INVALID_SCHEMA"
 ```
 
 
 General example:
 ```py
 import re
 from weelib.validator import Validator, Rule
```

### Comparing `weelib-0.1.5/README.md` & `weelib-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# weelib 
+# weelib
 <i>(experimental)</i><br>
 
 Library of additional functions for [`weepy`](https://gitlab.com/katry/weepy) framework.
 
 ## Installation
 
 <b>
@@ -54,20 +54,20 @@
 `ValidationError` provides enum of basic errors that may occur during validation -intended for extending to meet requirements of `_validate` wraps. <br>
 `ValidationError` contents:
 ```py
 from enum import Enum
 
 
 class ValidatorError(Enum):
-	MISSING_KEY = 1
-	INVALID_TYPE = 2
-	INVALID_VALUE = 3
-	NUMBER_NOT_IN_RANGE = 4
-	LENGTH_NOT_IN_RANGE = 5
-	INVALID_SCHEMA = 6
+	MISSING_KEY = "MISSING_KEY"
+	INVALID_TYPE = "INVALID_TYPE"
+	INVALID_VALUE = "INVALID_VALUE"
+	NUMBER_NOT_IN_RANGE = "NUMBER_NOT_IN_RANGE"
+	LENGTH_NOT_IN_RANGE = "LENGTH_NOT_IN_RANGE"
+	INVALID_SCHEMA = "INVALID_SCHEMA"
 ```
 
 
 General example:
 ```py
 import re
 from weelib.validator import Validator, Rule
```

### Comparing `weelib-0.1.5/setup.py` & `weelib-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `weelib-0.1.5/src/validator.py` & `weelib-0.1.6/src/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from enum import Enum
 from re import Pattern
 from typing import Callable, Any
 
 
 class ValidatorError(Enum):
-	MISSING_KEY = 1
-	INVALID_TYPE = 2
-	INVALID_VALUE = 3
-	NUMBER_NOT_IN_RANGE = 4
-	LENGTH_NOT_IN_RANGE = 5
-	INVALID_SCHEMA = 6
+	MISSING_KEY = "MISSING_KEY"
+	INVALID_TYPE = "INVALID_TYPE"
+	INVALID_VALUE = "INVALID_VALUE"
+	NUMBER_NOT_IN_RANGE = "NUMBER_NOT_IN_RANGE"
+	LENGTH_NOT_IN_RANGE = "LENGTH_NOT_IN_RANGE"
+	INVALID_SCHEMA = "INVALID_SCHEMA"
 
 
 class Validator:
 	_exact_keys = False
 	_schema: dict = {}
 
 	def __init__(self, data: dict | list | None = None, exact_keys: bool = False):
@@ -35,33 +35,30 @@
 		# TODO: output swagger format
 		return ""
 
 	def __call__(self, data, *args, **kwargs) -> tuple[bool, Any, str]:
 		if self.__class__._exact_keys:
 			for key in data:
 				if key not in self.__class__._schema.keys():
-					return False, ValidatorError.INVALID_SCHEMA, ""
+					return False, ValidatorError.INVALID_SCHEMA, key
 		for key, rule in self.__class__._schema.items():
 			if key not in data:
 				if rule.optional:
 					self.__dict__[key] = None
 					continue
 				else:
 					return False, ValidatorError.MISSING_KEY, key
 			result = rule.check(data[key])
 			if not result[0]:
 				return (
 					False,
 					result[1],
-					"%s%s%s" % (key, "->" if len(result[-1]) else "", result[-1])
+					key
 				)
 			self.__dict__[key] = data[key]
-		return self._validate(data)
-
-	def _validate(self, data) -> tuple[bool, Any | None, str]:
 		return True, None, ""
 
 
 class Rule:
 	def __init__(
 		self,
 		data_type: type,
@@ -200,11 +197,11 @@
 			result = call(req.data)
 			if result[0]:
 				return await method(req, resp, *args, data=self, **kwargs)
 			else:
 				await resp.abort(400, {
 					"status": False,
 					"code": 401,
-					"message": "BAD_REQUEST",
+					"message": "INVALID_INPUT",
 					"additional_info": [result[1], result[2]]
 				})
 		return wrapper
```

### Comparing `weelib-0.1.5/weelib.egg-info/PKG-INFO` & `weelib-0.1.6/weelib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weelib
-Version: 0.1.5
+Version: 0.1.6
 Summary: Additional functions for weepy framework.
 Home-page: https://gitlab.com/katry/weelib
 Author: Patrik Katrenak
 Author-email: patrik@katryapps.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -12,15 +12,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# weelib 
+# weelib
 <i>(experimental)</i><br>
 
 Library of additional functions for [`weepy`](https://gitlab.com/katry/weepy) framework.
 
 ## Installation
 
 <b>
@@ -72,20 +72,20 @@
 `ValidationError` provides enum of basic errors that may occur during validation -intended for extending to meet requirements of `_validate` wraps. <br>
 `ValidationError` contents:
 ```py
 from enum import Enum
 
 
 class ValidatorError(Enum):
-	MISSING_KEY = 1
-	INVALID_TYPE = 2
-	INVALID_VALUE = 3
-	NUMBER_NOT_IN_RANGE = 4
-	LENGTH_NOT_IN_RANGE = 5
-	INVALID_SCHEMA = 6
+	MISSING_KEY = "MISSING_KEY"
+	INVALID_TYPE = "INVALID_TYPE"
+	INVALID_VALUE = "INVALID_VALUE"
+	NUMBER_NOT_IN_RANGE = "NUMBER_NOT_IN_RANGE"
+	LENGTH_NOT_IN_RANGE = "LENGTH_NOT_IN_RANGE"
+	INVALID_SCHEMA = "INVALID_SCHEMA"
 ```
 
 
 General example:
 ```py
 import re
 from weelib.validator import Validator, Rule
```

