# Comparing `tmp/coffeepy-0.1.5.tar.gz` & `tmp/coffeepy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.5.tar", last modified: Thu Jul 13 13:37:38 2023, max compression
+gzip compressed data, was "coffeepy-0.1.6.tar", last modified: Fri Jul 14 19:33:01 2023, max compression
```

## Comparing `coffeepy-0.1.5.tar` & `coffeepy-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 13:37:24.000000 coffeepy-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 13:37:38.894291 coffeepy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-13 13:37:24.000000 coffeepy-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-13 13:37:24.000000 coffeepy-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:37:38.894291 coffeepy-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 13:37:24.000000 coffeepy-0.1.5/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 13:37:24.000000 coffeepy-0.1.5/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:37:38.894291 coffeepy-0.1.5/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 13:37:38.000000 coffeepy-0.1.5/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 19:32:51.000000 coffeepy-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-14 19:33:01.968010 coffeepy-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-14 19:32:51.000000 coffeepy-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 19:32:51.000000 coffeepy-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:33:01.968010 coffeepy-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.964010 coffeepy-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 19:32:51.000000 coffeepy-0.1.6/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-14 19:32:51.000000 coffeepy-0.1.6/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-14 19:32:51.000000 coffeepy-0.1.6/tests/test_coffeepy.py
```

### Comparing `coffeepy-0.1.5/LICENSE` & `coffeepy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.5/PKG-INFO` & `coffeepy-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/coffeepy.svg?style=flat)](https://pypi.python.org/pypi/coffeepy/) [![PyPI Version](https://img.shields.io/pypi/v/coffeepy.svg)](https://pypi.python.org/pypi/coffeepy)
 # Coffeepy
 
 Coffeepy ☕️ is a small program that prevents the system from sleeping.
```

### Comparing `coffeepy-0.1.5/README.md` & `coffeepy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.5/pyproject.toml` & `coffeepy-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 coffeepy = "coffeepy.coffeepy:run"
```

### Comparing `coffeepy-0.1.5/src/coffeepy/coffeepy.py` & `coffeepy-0.1.6/src/coffeepy/coffeepy.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,42 +42,39 @@
         if os.environ.get("WT_SESSION") is not None:
             return True
         else:
             return False
     else:
         return False
 
-def run(runtime=None, no_animation=False):
+def parse_args(args=None):
     parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
                                                  'You can set the time with -t flag\n'
                                                  'Made by kuvaus',
                                                  formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument('-t', '--time', type=int, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
+    parser.add_argument('-t', '--time', type=float, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
     parser.add_argument('-a', '--no-animation', action='store_true', help='Optional: Disable animation')
 
-    args = parser.parse_args()
+    return parser.parse_args(args)
+    
+def run(runtime=0, no_animation=False):
+
+    args = None
+    if runtime > 0 or no_animation:
+        args = ['-t', str(runtime)]
+        if no_animation:
+            args.append('-a')
 
+    args = parse_args(args)
+        
     if args.time == 0:
         duration = float('inf')  # Set duration to infinity
     else:
         duration = args.time * 60  # Convert minutes to seconds
-    
-    #if time is provided as run argument, it will overwrite args
-    #this is only relevant when coffeepy is run as a python module
-    if runtime is None:
-        duration = duration
-    elif runtime == 0:
-        duration = float('inf')
-    else:
-        duration = runtime * 60
-
-    #this disables animation when used as a module
-    if no_animation == True:
-        args.no_animation = True
 
     proc = None
 
     if 'darwin' in sys.platform:
         print('Running \'coffeepy\' on MacOS to prevent the system from sleeping')
         proc = subprocess.Popen(['caffeinate', '-dims'])
 
@@ -115,12 +112,12 @@
             proc.terminate()
         if 'linux' in sys.platform and not check_caffeinate():
             # Reset xset settings
             subprocess.Popen(['xset', 's', 'on'])
             subprocess.Popen(['xset', '+dpms'])
         if 'win32' in sys.platform:
             ctypes.windll.kernel32.SetThreadExecutionState(0x80000000)
-        sys.exit()
+        #sys.exit(0)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `coffeepy-0.1.5/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.6/src/coffeepy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/coffeepy.svg?style=flat)](https://pypi.python.org/pypi/coffeepy/) [![PyPI Version](https://img.shields.io/pypi/v/coffeepy.svg)](https://pypi.python.org/pypi/coffeepy)
 # Coffeepy
 
 Coffeepy ☕️ is a small program that prevents the system from sleeping.
```

