# Comparing `tmp/aql-builder-0.0.7.tar.gz` & `tmp/aql-builder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aql-builder-0.0.7.tar", last modified: Tue Jul 11 05:52:15 2023, max compression
+gzip compressed data, was "aql-builder-0.0.8.tar", last modified: Fri Jul 14 00:47:03 2023, max compression
```

## Comparing `aql-builder-0.0.7.tar` & `aql-builder-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:52:15.015682 aql-builder-0.0.7/
--rw-rw-rw-   0 root         (0) root         (0)    11341 2023-07-11 02:37:58.000000 aql-builder-0.0.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     4023 2023-07-11 05:52:15.015682 aql-builder-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-11 02:37:58.000000 aql-builder-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:52:15.015682 aql-builder-0.0.7/aql_builder/
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-07-11 05:46:14.000000 aql-builder-0.0.7/aql_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5676 2023-07-11 02:37:58.000000 aql-builder-0.0.7/aql_builder/assumptions.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-11 02:37:58.000000 aql-builder-0.0.7/aql_builder/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    33010 2023-07-11 02:37:58.000000 aql-builder-0.0.7/aql_builder/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:52:15.015682 aql-builder-0.0.7/aql_builder.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4023 2023-07-11 05:52:14.000000 aql-builder-0.0.7/aql_builder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      320 2023-07-11 05:52:14.000000 aql-builder-0.0.7/aql_builder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 05:52:14.000000 aql-builder-0.0.7/aql_builder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-11 05:52:14.000000 aql-builder-0.0.7/aql_builder.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-11 05:52:14.000000 aql-builder-0.0.7/aql_builder.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 05:52:15.015682 aql-builder-0.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 03:54:53.000000 aql-builder-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 05:52:15.015682 aql-builder-0.0.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)    31554 2023-07-11 02:37:58.000000 aql-builder-0.0.7/tests/test_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.957038 aql-builder-0.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)    11341 2022-12-20 01:01:18.000000 aql-builder-0.0.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-07-14 00:47:03.957038 aql-builder-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2023-07-14 00:36:37.000000 aql-builder-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.949038 aql-builder-0.0.8/aql_builder/
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2023-07-14 00:46:02.000000 aql-builder-0.0.8/aql_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5676 2022-12-20 01:01:18.000000 aql-builder-0.0.8/aql_builder/assumptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-20 01:01:18.000000 aql-builder-0.0.8/aql_builder/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    33324 2023-07-14 00:36:37.000000 aql-builder-0.0.8/aql_builder/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.957038 aql-builder-0.0.8/aql_builder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 00:47:03.957038 aql-builder-0.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 03:33:38.000000 aql-builder-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.957038 aql-builder-0.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    31682 2023-07-14 00:36:37.000000 aql-builder-0.0.8/tests/test_builder.py
```

### Comparing `aql-builder-0.0.7/LICENSE.txt` & `aql-builder-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.7/PKG-INFO` & `aql-builder-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aql-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: ArangoDB AQL builder
 Home-page: https://foss.heptapod.net/aquapenguin/aql-builder
 Maintainer: Aqua Penguin
 Maintainer-email: aqua.penguin.34@gmail.com
 Project-URL: Source, https://foss.heptapod.net/aquapenguin/aql-builder
 Project-URL: Tracker, https://foss.heptapod.net/aquapenguin/aql-builder/-/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -117,7 +117,13 @@
 'FOR u IN users '
 'FILTER (u.active == true) '
 'COLLECT ageGroup = (FLOOR((u.age / 5)) * 5), gender = u.gender INTO group '
 'SORT ageGroup DESC '
 'RETURN {"ageGroup": ageGroup, "gender": gender}'
 >>> 
 ```
+
+## Acknowledgements
+
+AQL builder is a free software project hosted at https://foss.heptapod.net. Thanks
+to the support of [Clever Cloud](https://clever-cloud.com),
+[Octobus](https://octobus.net) and the sponsors of the [heptapod project](https://heptapod.net/).
```

### Comparing `aql-builder-0.0.7/README.md` & `aql-builder-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -94,8 +94,14 @@
 ...     .to_aql()
 'FOR u IN users '
 'FILTER (u.active == true) '
 'COLLECT ageGroup = (FLOOR((u.age / 5)) * 5), gender = u.gender INTO group '
 'SORT ageGroup DESC '
 'RETURN {"ageGroup": ageGroup, "gender": gender}'
 >>> 
-```
+```
+
+## Acknowledgements
+
+AQL builder is a free software project hosted at https://foss.heptapod.net. Thanks
+to the support of [Clever Cloud](https://clever-cloud.com),
+[Octobus](https://octobus.net) and the sponsors of the [heptapod project](https://heptapod.net/).
```

### Comparing `aql-builder-0.0.7/aql_builder/__init__.py` & `aql-builder-0.0.8/aql_builder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from aql_builder import types
 
 # pylint: disable=protected-access
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 
 class _AQLBuilderMeta(type):
 
 	def __call__(cls, obj=None):
 		return types.auto_cast_token(obj)
```

### Comparing `aql-builder-0.0.7/aql_builder/assumptions.py` & `aql-builder-0.0.8/aql_builder/assumptions.py`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.7/aql_builder/types.py` & `aql-builder-0.0.8/aql_builder/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -836,29 +836,43 @@
 
 	def replace(self, expr):
 		return _PartialReplaceExpression(self, expr)
 
 
 class ForExpression(_PartialStatement):
 
-	__slots__ = ["_prev", "_varname", "_expr"]
+	__slots__ = ["_prev", "_varname", "_expr", "_options"]
 
-	def __init__(self, prev, varname, expr):
+	def __init__(self, prev, varname, expr, options=None):
 		self._prev = prev
 		self._varname = Identifier(varname)
 		self._expr = auto_cast_token(expr)
+		if options is None:
+			options = {}
+		self._options = ObjectLiteral(options)
+
+	def options(self, options):
+		return ForExpression(
+			self._prev,
+			self._varname,
+			self._expr,
+			options=options
+		)
 
 	def to_aql(self):
 		aql = []
 		if self._prev:
 			aql.append(self._prev_aql())
 		aql.append("FOR")
 		aql.append(wrap_aql(self._varname))
 		aql.append("IN")
 		aql.append(wrap_aql(self._expr))
+		if self._options:
+			aql.append("OPTIONS")
+			aql.append(wrap_aql(self._options))
 		return " ".join(aql)
 
 
 class FilterExpression(_PartialStatement):
 
 	__slots__ = ["_prev", "_expr"]
```

### Comparing `aql-builder-0.0.7/aql_builder.egg-info/PKG-INFO` & `aql-builder-0.0.8/aql_builder.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aql-builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: ArangoDB AQL builder
 Home-page: https://foss.heptapod.net/aquapenguin/aql-builder
 Maintainer: Aqua Penguin
 Maintainer-email: aqua.penguin.34@gmail.com
 Project-URL: Source, https://foss.heptapod.net/aquapenguin/aql-builder
 Project-URL: Tracker, https://foss.heptapod.net/aquapenguin/aql-builder/-/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -117,7 +117,13 @@
 'FOR u IN users '
 'FILTER (u.active == true) '
 'COLLECT ageGroup = (FLOOR((u.age / 5)) * 5), gender = u.gender INTO group '
 'SORT ageGroup DESC '
 'RETURN {"ageGroup": ageGroup, "gender": gender}'
 >>> 
 ```
+
+## Acknowledgements
+
+AQL builder is a free software project hosted at https://foss.heptapod.net. Thanks
+to the support of [Clever Cloud](https://clever-cloud.com),
+[Octobus](https://octobus.net) and the sponsors of the [heptapod project](https://heptapod.net/).
```

### Comparing `aql-builder-0.0.7/setup.py` & `aql-builder-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.7/tests/test_builder.py` & `aql-builder-0.0.8/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 		self._test_static(AB.ref(Collection(None, None, 'abcd')), 'abcd')
 		self._test_static(AB.ref(types.SimpleReference('abcd')), 'abcd')
 
 	def test_static_for(self):
 		self._test_static(AB.for_('abcd').in_('efgh'), 'FOR abcd IN efgh')
 		self._test_static(AB.for_('ab-cd').in_('ef-gh'), 'FOR `ab-cd` IN `ef-gh`')
 		self._test_static(AB.for_(Collection(None, None, 'abcd')).in_('efgh'), 'FOR abcd IN efgh')
+		self._test_static(
+			AB.for_('abcd').in_('efgh').options({'ijkl': 'mnop'}),
+			'FOR abcd IN efgh OPTIONS {"ijkl": mnop}'
+		)
 
 	def test_static_filter(self):
 		self._test_static(AB.filter('abcd'), 'FILTER abcd')
 		self._test_static(AB.filter('abcd.efgh'), 'FILTER abcd.efgh')
 		self._test_static(
 			AB.filter(AB.expr('abcd xyz efgh (1234 OR ijkl)')),
 			'FILTER abcd xyz efgh (1234 OR ijkl)'
```

