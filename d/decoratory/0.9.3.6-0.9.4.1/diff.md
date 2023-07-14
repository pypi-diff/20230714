# Comparing `tmp/decoratory-0.9.3.6.tar.gz` & `tmp/decoratory-0.9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.3.6.tar", last modified: Mon Jul 10 12:10:22 2023, max compression
+gzip compressed data, was "decoratory-0.9.4.1.tar", last modified: Fri Jul 14 13:27:17 2023, max compression
```

## Comparing `decoratory-0.9.3.6.tar` & `decoratory-0.9.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/
--rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.3.6/License.txt
--rw-rw-rw-   0        0        0    48657 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    46898 2023-07-10 12:03:21.000000 decoratory-0.9.3.6/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.3.6/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.053933 decoratory-0.9.3.6/Sources/
-drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.100801 decoratory-0.9.3.6/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.3.6/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7623 2023-07-10 12:09:45.000000 decoratory-0.9.3.6/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5889 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14162 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12426 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36916 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     8007 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10867 2023-07-10 11:27:32.000000 decoratory-0.9.3.6/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.100801 decoratory-0.9.3.6/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    48657 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 12:10:22.000000 decoratory-0.9.3.6/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/Unittest/
--rw-rw-rw-   0        0        0    24047 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23868 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40117 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10739 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10203 2023-07-10 11:27:33.000000 decoratory-0.9.3.6/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-07-10 12:10:22.116424 decoratory-0.9.3.6/setup.cfg
--rw-rw-rw-   0        0        0     4678 2023-07-10 12:09:45.000000 decoratory-0.9.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:27:17.257698 decoratory-0.9.4.1/
+-rw-rw-rw-   0        0        0     1252 2023-06-27 11:25:14.000000 decoratory-0.9.4.1/License.txt
+-rw-rw-rw-   0        0        0    48647 2023-07-14 13:27:17.257698 decoratory-0.9.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    46898 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.4.1/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:27:16.710690 decoratory-0.9.4.1/Sources/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:27:16.960653 decoratory-0.9.4.1/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.4.1/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7623 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5889 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    19690 2023-07-14 13:26:41.000000 decoratory-0.9.4.1/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12426 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36916 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     8007 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10867 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:27:17.007527 decoratory-0.9.4.1/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    48647 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 13:27:16.000000 decoratory-0.9.4.1/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:27:17.210815 decoratory-0.9.4.1/Unittest/
+-rw-rw-rw-   0        0        0    29042 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23868 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40117 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10739 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10203 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:27:17.257698 decoratory-0.9.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     4668 2023-07-14 13:26:42.000000 decoratory-0.9.4.1/setup.py
```

### Comparing `decoratory-0.9.3.6/License.txt` & `decoratory-0.9.4.1/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.3.6/PKG-INFO` & `decoratory-0.9.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.3.6
+Version: 0.9.4.1
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu/decoratory/index.html
 Download-URL: http://evation.eu/decoratory/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -22,15 +22,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
@@ -49,17 +49,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu/decoratory"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.3.2"
-    __date__ = "2023-07-10"
-    __time__ = "14:03:21"
+    __version__ = "0.9.4.1"
+    __date__ = "2023-07-14"
+    __time__ = "15:26:41"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
```

### Comparing `decoratory-0.9.3.6/Readme.rst` & `decoratory-0.9.4.1/Readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu/decoratory"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.3.2"
-    __date__ = "2023-07-10"
-    __time__ = "14:03:21"
+    __version__ = "0.9.4.1"
+    __date__ = "2023-07-14"
+    __time__ = "15:26:41"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory/__main__.py` & `decoratory-0.9.4.1/Sources/decoratory/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.6"
-__date__ = "2023-07-10"
-__time__ = "14:09:45"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory/banner.py` & `decoratory-0.9.4.1/Sources/decoratory/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory/multiton.py` & `decoratory-0.9.4.1/Sources/decoratory/multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory/observer.py` & `decoratory-0.9.4.1/Sources/decoratory/observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,17 +407,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory/singleton.py` & `decoratory-0.9.4.1/Sources/decoratory/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory/wrapper.py` & `decoratory-0.9.4.1/Sources/decoratory/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,17 +136,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.4.1/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.3.6
+Version: 0.9.4.1
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu/decoratory/index.html
 Download-URL: http://evation.eu/decoratory/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -22,15 +22,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
@@ -49,17 +49,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu/decoratory"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.3.2"
-    __date__ = "2023-07-10"
-    __time__ = "14:03:21"
+    __version__ = "0.9.4.1"
+    __date__ = "2023-07-14"
+    __time__ = "15:26:41"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
```

### Comparing `decoratory-0.9.3.6/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.4.1/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.3.6/Unittest/test_basic.py` & `decoratory-0.9.4.1/Unittest/test_basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
-from decoratory.basic import (Activation, F, Parser, X)
+from decoratory.basic import (Activation, F, Parser, X, BaseDecorator)
 
 
 # -----------------------------------------------------------------------------
 # Test functions
 def cmp(f: F, t: tuple):
     """Compare F with tuple"""
     return (x == y for x, y in zip(f, t))
@@ -589,12 +589,132 @@
         # Unittest: eval()
         self.assertListEqual(Parser.eval(F('a')), [F('a')])
         self.assertListEqual(Parser.eval(function), [F(function)])
         self.assertListEqual(Parser.eval('function'), [F('function')])
         self.assertListEqual(Parser.eval(('function',)), [F('function')])
         self.assertListEqual(Parser.eval(['function']), [F('function')])
 
+    def test_BaseDecorator(self):
+        """Unittest: Base Decorator"""
+
+        # ---------------------------------------------------------------------
+        # Unittest: BaseDecorator
+        self.assertTrue(hasattr(BaseDecorator, "__init__"))
+        self.assertTrue(hasattr(BaseDecorator, "__post_init__"))
+        self.assertTrue(hasattr(BaseDecorator, "__call__"))
+        self.assertTrue(hasattr(BaseDecorator, "decorator"))
+
+        # BaseDecorator is an abstract class
+        try:
+            BaseDecorator()
+        except TypeError:
+            pass
+        else:
+            raise AssertionError
+
+        # ---------------------------------------------------------------------
+        # Unittest: Decorator class inherited from BaseDecorator
+        class Decorator(BaseDecorator):
+            pass
+
+        self.assertTrue(hasattr(Decorator, "__init__"))
+        self.assertTrue(hasattr(Decorator, "__post_init__"))
+        self.assertTrue(hasattr(Decorator, "__call__"))
+        self.assertTrue(hasattr(Decorator, "decorator"))
+
+        # Decorator has not overwritten the decorator() method
+        try:
+            Decorator()
+        except TypeError:
+            pass
+        else:
+            raise AssertionError
+
+        # Override the decorator() method
+        class Decorator(BaseDecorator):
+            def decorator(self, *args: object, **kwargs: object) -> object:
+                return True
+
+        # This is not really a reasonable call to Decorator, but ok...
+        d = Decorator()
+        self.assertIsInstance(d, BaseDecorator)
+        self.assertIsInstance(d, Decorator)
+        self.assertIsNone(d._substitute)
+        self.assertTupleEqual(d._args, ())
+        self.assertDictEqual(d._kwargs, {})
+        self.assertTupleEqual(d._deco_args, ())
+        self.assertDictEqual(d._deco_kwargs, {})
+        self.assertEqual(d._call_method, d.__post_init__)
+        self.assertTrue(d.decorator())
+
+        # Invalid call to Decorator with deco params (1. deco is not None!)
+        try:
+            Decorator()()
+        except AttributeError:
+            pass
+        else:
+            raise AssertionError
+
+        # Valid call to Decorator without any parameters
+        prnt = Decorator(print)
+        self.assertEqual(prnt._substitute, print)
+        self.assertTupleEqual(prnt._args, ())
+        self.assertDictEqual(prnt._kwargs, {})
+        self.assertTupleEqual(prnt._deco_args, ())
+        self.assertDictEqual(prnt._deco_kwargs, {})
+        self.assertEqual(prnt._call_method, prnt.decorator)
+        self.assertTrue(prnt.decorator())
+
+        # Valid call to Decorator without deco params
+        prnt = Decorator(print, 1, key="value")
+        self.assertEqual(prnt._substitute, print)
+        self.assertTupleEqual(prnt._args, (1,))
+        self.assertDictEqual(prnt._kwargs, dict(key="value"))
+        self.assertTupleEqual(prnt._deco_args, ())
+        self.assertDictEqual(prnt._deco_kwargs, {})
+        self.assertEqual(prnt._call_method, prnt.decorator)
+        self.assertTrue(prnt.decorator())
+
+        # Valid call to Decorator with empty deco params
+        prnt = Decorator()(print, 1, key="value")
+        self.assertEqual(prnt._substitute, print)
+        self.assertTupleEqual(prnt._args, (1,))
+        self.assertDictEqual(prnt._kwargs, dict(key="value"))
+        self.assertTupleEqual(prnt._deco_args, ())
+        self.assertDictEqual(prnt._deco_kwargs, {})
+        self.assertEqual(prnt._call_method, prnt.decorator)
+        self.assertTrue(prnt.decorator())
+
+        # Valid call to Decorator with keyword deco params
+        prnt = Decorator(b="any stuff")(print, 1, key="value")
+        self.assertEqual(prnt._substitute, print)
+        self.assertTupleEqual(prnt._args, (1,))
+        self.assertDictEqual(prnt._kwargs, dict(key="value"))
+        self.assertTupleEqual(prnt._deco_args, ())
+        self.assertDictEqual(prnt._deco_kwargs, dict(b="any stuff"))
+        self.assertEqual(prnt._call_method, prnt.decorator)
+        self.assertTrue(prnt.decorator())
+
+        # Valid call to Decorator with deco params (1. deco is None!)
+        prnt = Decorator(None, 2, b="any stuff")(print, 1, key="value")
+        self.assertEqual(prnt._substitute, print)
+        self.assertTupleEqual(prnt._args, (1,))
+        self.assertDictEqual(prnt._kwargs, dict(key="value"))
+        self.assertTupleEqual(prnt._deco_args, (2,))
+        self.assertDictEqual(prnt._deco_kwargs, dict(b="any stuff"))
+        self.assertEqual(prnt._call_method, prnt.decorator)
+        self.assertTrue(prnt.decorator())
+
+        # Invalid call to Decorator with deco params (1. deco is not None!)
+        prnt = Decorator(2, 3, b="any stuff")(print, 1, key="value")
+        try:
+            self.assertEqual(prnt._substitute, 2)
+        except AttributeError:
+            pass
+        else:
+            raise AssertionError
+
 
 # -----------------------------------------------------------------------------
 # Execution
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `decoratory-0.9.3.6/Unittest/test_multiton.py` & `decoratory-0.9.4.1/Unittest/test_multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.3.6/Unittest/test_observer.py` & `decoratory-0.9.4.1/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.3.6/Unittest/test_singleton.py` & `decoratory-0.9.4.1/Unittest/test_singleton.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.3.6/Unittest/test_wrapper.py` & `decoratory-0.9.4.1/Unittest/test_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.1"
-__date__ = "2023-07-10"
-__time__ = "13:27:32"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.3.6/setup.py` & `decoratory-0.9.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu/decoratory"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.3.6"
-__date__ = "2023-07-10"
-__time__ = "14:09:45"
+__version__ = "0.9.4.1"
+__date__ = "2023-07-14"
+__time__ = "15:26:41"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
@@ -87,15 +87,15 @@
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: Implementation',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Education',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Utilities'],
     # Modules, Files and Data
```

