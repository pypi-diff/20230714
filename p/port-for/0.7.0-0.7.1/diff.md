# Comparing `tmp/port-for-0.7.0.tar.gz` & `tmp/port-for-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port-for-0.7.0.tar", last modified: Thu Jun 15 08:13:13 2023, max compression
+gzip compressed data, was "port-for-0.7.1.tar", last modified: Fri Jul 14 15:09:50 2023, max compression
```

## Comparing `port-for-0.7.0.tar` & `port-for-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-15 08:13:04.000000 port-for-0.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 08:13:04.000000 port-for-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 08:13:04.000000 port-for-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-15 08:13:13.653290 port-for-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 08:13:04.000000 port-for-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/port_for/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/_download_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/docopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/port_for.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-15 08:13:04.000000 port-for-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 08:13:13.657290 port-for-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-15 08:13:04.000000 port-for-0.7.0/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:09:50.060018 port-for-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-14 15:09:39.000000 port-for-0.7.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 15:09:39.000000 port-for-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 15:09:39.000000 port-for-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-14 15:09:50.060018 port-for-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-14 15:09:39.000000 port-for-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:09:50.060018 port-for-0.7.1/port_for/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/_download_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/docopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 15:09:39.000000 port-for-0.7.1/port_for/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:09:50.060018 port-for-0.7.1/port_for.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-14 15:09:50.000000 port-for-0.7.1/port_for.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 15:09:50.000000 port-for-0.7.1/port_for.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:09:50.000000 port-for-0.7.1/port_for.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 15:09:50.000000 port-for-0.7.1/port_for.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 15:09:50.000000 port-for-0.7.1/port_for.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:09:49.000000 port-for-0.7.1/port_for.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-14 15:09:39.000000 port-for-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 15:09:50.060018 port-for-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:09:50.060018 port-for-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-07-14 15:09:39.000000 port-for-0.7.1/tests/test_cases.py
```

### Comparing `port-for-0.7.0/CHANGES.rst` & `port-for-0.7.1/CHANGES.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+0.7.1 (2023-07-14)
+==================
+
+Features
+--------
+
+- Add `PortType` type alias for easier typing related code (`#149 <https://github.com/kmike/port-for/issues/149>`_)
+
+
 0.7.0 (2023-06-15)
 ==================
 
 Features
 --------
 
-- get_port will now allow passing additional exclude_ports parameter - these ports will not be chosen. (`#143 <https://https://github.com/kmike/port-for/issues/143>`_)
+- get_port will now allow passing additional exclude_ports parameter - these ports will not be chosen. (`#143 <https://github.com/kmike/port-for/issues/143>`_)
 
 
 0.6.3 (2022-12-15)
 ==================
 
 Features
 --------
 
-- Add python 3.11 to the list of supported python versions. (`#111 <https://https://github.com/kmike/port-for/issues/111>`_)
+- Add python 3.11 to the list of supported python versions. (`#111 <https://github.com/kmike/port-for/issues/111>`_)
 
 
 Miscellaneus
 ------------
 
-- Use towncrier as a changelog management tool. (`#107 <https://https://github.com/kmike/port-for/issues/107>`_)
+- Use towncrier as a changelog management tool. (`#107 <https://github.com/kmike/port-for/issues/107>`_)
 - Moved development dependencies to be managed by pipenv.
-  All development process can be managed  with it - which means automatic isolation. (`#108 <https://https://github.com/kmike/port-for/issues/108>`_)
-- Migrate versioning tool to tbump, and move package definition to pyproject.toml (`#109 <https://https://github.com/kmike/port-for/issues/109>`_)
+  All development process can be managed  with it - which means automatic isolation. (`#108 <https://github.com/kmike/port-for/issues/108>`_)
+- Migrate versioning tool to tbump, and move package definition to pyproject.toml (`#109 <https://github.com/kmike/port-for/issues/109>`_)
 - Moved as much of the setup.cfg settings into the pyproject.toml as possible.
-  Dropped pydocstyle support. (`#112 <https://https://github.com/kmike/port-for/issues/112>`_)
+  Dropped pydocstyle support. (`#112 <https://github.com/kmike/port-for/issues/112>`_)
 
 
 0.6.2
 ----------
 
 Misc
 ++++
```

### Comparing `port-for-0.7.0/LICENSE.txt` & `port-for-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/PKG-INFO` & `port-for-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-for
-Version: 0.7.0
+Version: 0.7.1
 Summary: Utility that helps with local TCP ports management. It can find an unused TCP localhost port and remember the association.
 Author-email: Mikhail Korobov <kmike84@gmail.com>
 Maintainer-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License: Copyright (c) 2012 Mikhail Korobov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,15 +22,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Source, https://github.com/kmike/port-for/
 Project-URL: Bug Tracker, https://github.com/kmike/port-for/issues
-Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.7.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.7.1/CHANGES.rst
 Keywords: port,posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `port-for-0.7.0/README.rst` & `port-for-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/__init__.py` & `port-for-0.7.1/port_for/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """port_for package."""
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 from ._ranges import UNASSIGNED_RANGES
 from .api import (
     available_good_ports,
     available_ports,
     is_available,
     good_port_ranges,
```

### Comparing `port-for-0.7.0/port_for/_download_ranges.py` & `port-for-0.7.1/port_for/_download_ranges.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/_ranges.py` & `port-for-0.7.1/port_for/_ranges.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/api.py` & `port-for-0.7.1/port_for/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,28 +130,30 @@
 
 
 def filter_by_type(lst: Iterable, type_of: Type[T]) -> List[T]:
     """Returns a list of elements with given type."""
     return [e for e in lst if isinstance(e, type_of)]
 
 
+PortType = Union[
+    str,
+    int,
+    Tuple[int, int],
+    Set[int],
+    List[str],
+    List[int],
+    List[Tuple[int, int]],
+    List[Set[int]],
+    List[Union[Set[int], Tuple[int, int]]],
+    List[Union[str, int, Tuple[int, int], Set[int]]],
+]
+
+
 def get_port(
-    ports: Union[
-        None,
-        str,
-        int,
-        Tuple[int, int],
-        Set[int],
-        List[str],
-        List[int],
-        List[Tuple[int, int]],
-        List[Set[int]],
-        List[Union[Set[int], Tuple[int, int]]],
-        List[Union[str, int, Tuple[int, int], Set[int]]],
-    ],
+    ports: Optional[PortType],
     exclude_ports: Optional[Iterable[int]] = None,
 ) -> Optional[int]:
     """
     Retuns a random available port. If there's only one port passed
     (e.g. 5000 or '5000') function does not check if port is available.
     If there's -1 passed as an argument, function returns None.
```

### Comparing `port-for-0.7.0/port_for/cmd.py` & `port-for-0.7.1/port_for/cmd.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/docopt.py` & `port-for-0.7.1/port_for/docopt.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/ephemeral.py` & `port-for-0.7.1/port_for/ephemeral.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/store.py` & `port-for-0.7.1/port_for/store.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for/utils.py` & `port-for-0.7.1/port_for/utils.py`

 * *Files identical despite different names*

### Comparing `port-for-0.7.0/port_for.egg-info/PKG-INFO` & `port-for-0.7.1/port_for.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-for
-Version: 0.7.0
+Version: 0.7.1
 Summary: Utility that helps with local TCP ports management. It can find an unused TCP localhost port and remember the association.
 Author-email: Mikhail Korobov <kmike84@gmail.com>
 Maintainer-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License: Copyright (c) 2012 Mikhail Korobov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,15 +22,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Source, https://github.com/kmike/port-for/
 Project-URL: Bug Tracker, https://github.com/kmike/port-for/issues
-Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.7.0/CHANGES.rst
+Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.7.1/CHANGES.rst
 Keywords: port,posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `port-for-0.7.0/pyproject.toml` & `port-for-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "port-for"
-version = "0.7.0"
+version = "0.7.1"
 description = "Utility that helps with local TCP ports management. It can find an unused TCP localhost port and remember the association."
 readme = "README.rst"
 keywords = ["port", "posix"]
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Mikhail Korobov", email = "kmike84@gmail.com"}
 ]
@@ -29,15 +29,15 @@
     "Topic :: Internet :: WWW/HTTP :: Site Management",
 ]
 requires-python = ">= 3.7"
 
 [project.urls]
 "Source" = "https://github.com/kmike/port-for/"
 "Bug Tracker" = "https://github.com/kmike/port-for/issues"
-"Changelog" = "https://github.com/kmike/port-for/blob/v0.7.0/CHANGES.rst"
+"Changelog" = "https://github.com/kmike/port-for/blob/v0.7.1/CHANGES.rst"
 
 [project.scripts]
 port-for = "port_for.cmd:main"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -54,15 +54,15 @@
 testpaths = "tests"
 filterwarnings = "error"
 
 [tool.towncrier]
 directory = "newsfragments"
 single_file=true
 filename="CHANGES.rst"
-issue_format="`#{issue} <https://https://github.com/kmike/port-for/issues/{issue}>`_"
+issue_format="`#{issue} <https://github.com/kmike/port-for/issues/{issue}>`_"
 
 [tool.towncrier.fragment.feature]
 name = "Features"
 showcontent = true
 
 [tool.towncrier.fragment.bugfix]
 name = "Bugfixes"
@@ -83,15 +83,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.7.0"
+current = "0.7.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `port-for-0.7.0/tests/test_cases.py` & `port-for-0.7.1/tests/test_cases.py`

 * *Files identical despite different names*

