# Comparing `tmp/xthread-0.0.1.tar.gz` & `tmp/xthread-0.0.2.tar.gz`

## Comparing `xthread-0.0.1.tar` & `xthread-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xthread-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 xthread-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 xthread-0.0.1/.github/workflows/test-suite.yml
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 xthread-0.0.1/scripts/build
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 xthread-0.0.1/scripts/check
--rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 xthread-0.0.1/scripts/clean
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 xthread-0.0.1/scripts/coverage
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 xthread-0.0.1/scripts/install
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xthread-0.0.1/scripts/test
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 xthread-0.0.1/tests/main.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 xthread-0.0.1/xthread/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 xthread-0.0.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 xthread-0.0.1/LICENSE
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 xthread-0.0.1/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 xthread-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 xthread-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xthread-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 xthread-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 xthread-0.0.2/.github/workflows/test-suite.yml
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 xthread-0.0.2/scripts/build
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 xthread-0.0.2/scripts/check
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 xthread-0.0.2/scripts/clean
+-rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 xthread-0.0.2/scripts/coverage
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 xthread-0.0.2/scripts/install
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xthread-0.0.2/scripts/test
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xthread-0.0.2/tests/main.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 xthread-0.0.2/xthread/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 xthread-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 xthread-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 xthread-0.0.2/README.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xthread-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 xthread-0.0.2/PKG-INFO
```

### Comparing `xthread-0.0.1/.github/workflows/publish.yml` & `xthread-0.0.2/.github/workflows/publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,14 @@
         run: pip install build
       - name: Build distribution
         run: python -m build
       - name: Publish
         uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
-      - name: Build and push Docker images
-        uses: docker/build-push-action@v4.1.1
 
   generate-changelog:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v2
       with:
         fetch-depth: 0
```

### Comparing `xthread-0.0.1/.github/workflows/test-suite.yml` & `xthread-0.0.2/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `xthread-0.0.1/tests/main.py` & `xthread-0.0.2/tests/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,44 @@
 
 
 WAIT_TIME = 0.1
 
 
 class ThreadTestCase(unittest.TestCase):
     def test_thread_running(self):
-        target = mock.Mock()
-        thread = Thread(target=target)
+        target = mock.Mock(return_value=42)
+        on_result = mock.Mock()
+        thread = Thread(target=target, on_result=on_result)
         time.sleep(WAIT_TIME)
+
+        self.assertTrue(thread.is_active)
+        self.assertTrue(thread.is_running)
+        self.assertFalse(thread.is_paused)
+
+        thread.pause()
+        self.assertTrue(thread.is_active)
+        self.assertTrue(thread.is_paused)
+        self.assertFalse(thread.is_running)
+
         thread.stop()
+        self.assertFalse(thread.is_active)
+        self.assertFalse(thread.is_running)
+        self.assertFalse(thread.is_paused)
 
         target.assert_called_with(thread)
+        on_result.assert_called_with(42)
+
+    def test_without_error_handler(self):
+        error = ValueError()
+        target = mock.Mock(side_effect=error)
+
+        thread = Thread(target=target)
+        time.sleep(WAIT_TIME)
+        thread.stop()
+
 
     def test_catch_error(self):
         error = ValueError()
         target = mock.Mock(side_effect=error)
         error_handler = mock.Mock()
 
         thread = Thread(target=target, on_error=error_handler)
```

### Comparing `xthread-0.0.1/xthread/__init__.py` & `xthread-0.0.2/xthread/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable, Optional, Any
 import threading
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 class Thread:
     """Thread API supports some features such as pause/unpause
     and terminate non-preemtively
     """
 
@@ -61,14 +61,26 @@
 
     def unpause(self):
         self.__resume.set()
 
         if self.__on_unpaused:
             self.__on_unpaused(self)
 
+    @property
+    def is_active(self):
+        return self.__is_running.is_set()
+
+    @property
+    def is_paused(self):
+        return self.is_active and not self.__resume.is_set()
+
+    @property
+    def is_running(self):
+        return self.is_active and not self.is_paused
+
     def __cycle_execution(self, target, args=None, kwargs=None):
         args = args or tuple()
         kwargs = kwargs or dict()
 
         def wrapper():
             while self.__is_running.is_set():
                 try:
```

### Comparing `xthread-0.0.1/.gitignore` & `xthread-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xthread-0.0.1/LICENSE` & `xthread-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xthread-0.0.1/README.md` & `xthread-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 <p align="center">
     <em>Threading for human.</em>
 </p>
 <p align="center">
     <a href="https://github.com/magiskboy/xthread/actions">
         <img src="https://github.com/magiskboy/xthread/actions/workflows/test-suite.yml/badge.svg" alt="Build Status">
     </a>
-    <a href="https://app.codecov.io/gh/magiskboy/xthread">
-        <img src="https://img.shields.io/codecov/c/github/magiskboy/xthread" alt="Code coverage">
+    <a href="https://codecov.io/gh/magiskboy/xthread" > 
+        <img src="https://codecov.io/gh/magiskboy/xthread/branch/master/graph/badge.svg?token=uXPvINHpRs"/> 
     </a>
     <a href="https://pypi.org/project/xthread/">
         <img src="https://img.shields.io/pypi/dd/xthread" alt="Download PyPi">
     </a>
     <a href="https://github.com/magiskboy/xthread/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/magiskboy/xthread" alt="MIT">
     </a>
```

### Comparing `xthread-0.0.1/pyproject.toml` & `xthread-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -52,13 +52,13 @@
 [tool.coverage.run]
 omit = ["tests/*"]
 
 [tool.coverage.path]
 source = "xthread"
 
 [tool.coverage.report]
-fail_under = 95
+fail_under = 100
 show_missing = true
 sort = "Cover"
 
 [tool.ruff]
 ignore = ["E501"]
```

### Comparing `xthread-0.0.1/PKG-INFO` & `xthread-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xthread
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful threading for pause/unpause and terminating
 Project-URL: Homepage, https://github.com/magiskboy/xthread
 Project-URL: Documentation, https://github.com/magiskboy/xthread#features
 Project-URL: Issues, https://github.com/magiskboy/xthread/issues/
 Project-URL: Source, https://github.com/magiskboy/xthread
 Project-URL: Changelog, https://github.com/magiskboy/xthread/blob/main/CHANGELOG.md
 Author-email: Nguyen Khac Thanh <nguyenkhacthanh244@gmail.com>
@@ -33,16 +33,16 @@
 <p align="center">
     <em>Threading for human.</em>
 </p>
 <p align="center">
     <a href="https://github.com/magiskboy/xthread/actions">
         <img src="https://github.com/magiskboy/xthread/actions/workflows/test-suite.yml/badge.svg" alt="Build Status">
     </a>
-    <a href="https://app.codecov.io/gh/magiskboy/xthread">
-        <img src="https://img.shields.io/codecov/c/github/magiskboy/xthread" alt="Code coverage">
+    <a href="https://codecov.io/gh/magiskboy/xthread" > 
+        <img src="https://codecov.io/gh/magiskboy/xthread/branch/master/graph/badge.svg?token=uXPvINHpRs"/> 
     </a>
     <a href="https://pypi.org/project/xthread/">
         <img src="https://img.shields.io/pypi/dd/xthread" alt="Download PyPi">
     </a>
     <a href="https://github.com/magiskboy/xthread/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/magiskboy/xthread" alt="MIT">
     </a>
```

