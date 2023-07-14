# Comparing `tmp/robocorp_browser-1.0.2.tar.gz` & `tmp/robocorp_browser-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-1.0.2.tar", max compression
+gzip compressed data, was "robocorp_browser-2.0.0.tar", max compression
```

## Comparing `robocorp_browser-1.0.2.tar` & `robocorp_browser-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1583 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/README.md
--rw-r--r--   0        0        0      712 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6318 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0       81 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/src/robocorp/browser/__main__.py
--rw-r--r--   0        0        0     6725 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0     1890 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/src/robocorp/browser/_browser_engines.py
--rw-r--r--   0        0        0      825 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/src/robocorp/browser/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 14:28:15.580296 robocorp_browser-1.0.2/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 robocorp_browser-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1583 2023-07-14 11:43:38.604090 robocorp_browser-2.0.0/README.md
+-rw-r--r--   0        0        0      712 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6318 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/src/robocorp/browser/__main__.py
+-rw-r--r--   0        0        0     7104 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0     1890 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/src/robocorp/browser/_browser_engines.py
+-rw-r--r--   0        0        0      825 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/src/robocorp/browser/cli.py
+-rw-r--r--   0        0        0        0 2023-07-14 11:43:38.608090 robocorp_browser-2.0.0/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 robocorp_browser-2.0.0/PKG-INFO
```

### Comparing `robocorp_browser-1.0.2/README.md` & `robocorp_browser-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_browser-1.0.2/pyproject.toml` & `robocorp_browser-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "1.0.2"
+version = "2.0.0"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_browser-1.0.2/src/robocorp/browser/__init__.py` & `robocorp_browser-2.0.0/src/robocorp/browser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Locator,
     Page,
     Playwright,
 )
 
 from ._browser_engines import BrowserEngine
 
-__version__ = "1.0.2"
+__version__ = "2.0.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
```

### Comparing `robocorp_browser-1.0.2/src/robocorp/browser/_browser_context.py` & `robocorp_browser-2.0.0/src/robocorp/browser/_browser_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,32 +118,38 @@
     The configuration used. Can be mutated as needed until
     `browser_context_args` is called (at which point mutating it will raise an
     error since it was already used).
     """
     return _BrowserConfig()
 
 
-def _is_debugger_attached() -> bool:
-    pydevd = sys.modules.get("pydevd")
-    if not pydevd or not hasattr(pydevd, "get_global_debugger"):
-        return False
-    debugger = pydevd.get_global_debugger()
-    if not debugger or not hasattr(debugger, "is_attached"):
-        return False
-    return debugger.is_attached()
+def _get_auto_headless_state() -> bool:
+    # If in Linux and with no valid display, we can assume we are in a
+    # container which doesn't support UI.
+    return sys.platform.startswith("linux") and not (
+        os.environ.get("DISPLAY") or os.environ.get("WAYLAND_DISPLAY")
+    )
 
 
 @session_cache
 def browser_type_launch_args() -> Dict:
     launch_options = {}
-    headless = _browser_config().headless
-    if headless is None:
-        launch_options["headless"] = not _is_debugger_attached()
+
+    # RPA_HEADLESS_MODE can be used to force whether running headless.
+    rpa_headless_mode = os.environ.get("RPA_HEADLESS_MODE")
+    if rpa_headless_mode is not None:
+        launch_options["headless"] = bool(int(os.environ["RPA_HEADLESS_MODE"]))
     else:
-        launch_options["headless"] = headless
+        headless = _browser_config().headless
+        if headless is None:
+            # Heuristic is now: run showing UI (headless=False) by default
+            # and run headless when in a VM without a display.
+            launch_options["headless"] = _get_auto_headless_state()
+        else:
+            launch_options["headless"] = headless
 
     slowmo_option = _browser_config().slowmo
     if slowmo_option:
         launch_options["slow_mo"] = slowmo_option
     return launch_options
```

### Comparing `robocorp_browser-1.0.2/src/robocorp/browser/_browser_engines.py` & `robocorp_browser-2.0.0/src/robocorp/browser/_browser_engines.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-1.0.2/src/robocorp/browser/cli.py` & `robocorp_browser-2.0.0/src/robocorp/browser/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-1.0.2/PKG-INFO` & `robocorp_browser-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 1.0.2
+Version: 2.0.0
 Summary: Robocorp browser automation library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

