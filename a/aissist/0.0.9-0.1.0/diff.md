# Comparing `tmp/aissist-0.0.9.tar.gz` & `tmp/aissist-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissist-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissist-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissist-0.0.9.tar` & `aissist-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.9/LICENSE
--rw-r--r--   0        0        0       59 2023-06-25 04:29:52.904018 aissist-0.0.9/Makefile
--rw-r--r--   0        0        0      247 2023-06-26 09:38:32.789716 aissist-0.0.9/Pipfile
--rw-r--r--   0        0        0    47145 2023-06-25 04:28:58.425264 aissist-0.0.9/Pipfile.lock
--rw-r--r--   0        0        0     1342 2023-06-25 03:52:36.697190 aissist-0.0.9/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.9/aissist/__init__.py
--rw-r--r--   0        0        0     3501 2023-06-26 10:01:57.305104 aissist-0.0.9/aissist/aissistant.py
--rw-r--r--   0        0        0     2513 2023-06-26 10:06:26.009018 aissist-0.0.9/aissist/config.py
--rw-r--r--   0        0        0      741 2023-06-25 04:30:03.600530 aissist-0.0.9/aissist/spinner.py
--rw-r--r--   0        0        0       21 2023-06-26 10:06:48.571978 aissist-0.0.9/aissist/version.py
--rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.9/images/screenshot.png
--rw-r--r--   0        0        0      898 2023-06-26 10:06:58.335541 aissist-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 aissist-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      650 2023-07-06 04:30:01.951143 aissist-0.1.0/.github/workflows/on-push.yml
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.1.0/LICENSE
+-rw-r--r--   0        0        0      212 2023-07-08 00:57:08.478681 aissist-0.1.0/Makefile
+-rw-r--r--   0        0        0      386 2023-07-09 14:55:19.582242 aissist-0.1.0/Pipfile
+-rw-r--r--   0        0        0    87890 2023-07-09 14:55:19.582242 aissist-0.1.0/Pipfile.lock
+-rw-r--r--   0        0        0     2645 2023-07-08 00:57:19.306634 aissist-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.1.0/aissist/__init__.py
+-rw-r--r--   0        0        0     3488 2023-07-14 04:31:04.384789 aissist-0.1.0/aissist/aissist.py
+-rw-r--r--   0        0        0     2485 2023-07-08 00:57:08.482681 aissist-0.1.0/aissist/code_formatter.py
+-rw-r--r--   0        0        0     5407 2023-07-08 00:57:08.482681 aissist-0.1.0/aissist/config.py
+-rw-r--r--   0        0        0      201 2023-07-08 00:57:08.482681 aissist-0.1.0/aissist/exceptions.py
+-rw-r--r--   0        0        0     5464 2023-07-09 14:55:19.582242 aissist-0.1.0/aissist/model.py
+-rw-r--r--   0        0        0      359 2023-06-27 01:39:32.367617 aissist-0.1.0/aissist/prompts.py
+-rw-r--r--   0        0        0      813 2023-06-29 02:45:27.583312 aissist-0.1.0/aissist/spinner.py
+-rw-r--r--   0        0        0       79 2023-07-08 00:57:08.482681 aissist-0.1.0/aissist/version.py
+-rw-r--r--   0        0        0    64621 2023-07-14 04:34:07.328252 aissist-0.1.0/images/screenshot.png
+-rw-r--r--   0        0        0      959 2023-07-14 04:36:01.535828 aissist-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 21:05:26.062826 aissist-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-04 21:09:15.044593 aissist-0.1.0/tests/test_models.py
+-rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 aissist-0.1.0/PKG-INFO
```

### Comparing `aissist-0.0.9/LICENSE` & `aissist-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aissist-0.0.9/aissist/spinner.py` & `aissist-0.1.0/aissist/spinner.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import time
 from typing import Optional
 
 
 class Spinner:
     """Simple implementation of a spinner"""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.spinner_flag: bool = True
         self.thread: Optional[threading.Thread] = None
 
-    def spinner(self, spin_delay: float = 0.12):
+    def spinner(self, spin_delay: float = 0.12) -> None:
         while self.spinner_flag:
             for char in "|/-\\":
                 sys.stdout.write("\r" + char)
                 sys.stdout.flush()
                 time.sleep(spin_delay)
         sys.stdout.write("\r")
 
-    def stop(self):
+    def stop(self) -> None:
         self.spinner_flag = False
-        self.thread.join()
+        if self.thread is not None:
+            self.thread.join()
 
-    def start(self):
+    def start(self) -> None:
         self.spinner_flag = True
         self.thread = threading.Thread(target=self.spinner)
         self.thread.start()
```

### Comparing `aissist-0.0.9/pyproject.toml` & `aissist-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+
+[build-system]
+requires = ["flit_core >=3.2,<4", "importlib_metadata"]
+build-backend = "flit_core.buildapi"
+
 [project]
 name = "aissist"
-version = "0.0.9"
-description = "A simple GPT command line interface"
+version = "0.1.0"
+description = "A simple GPT command line chat interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
 
 readme = "README.md"
 
@@ -16,24 +21,22 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 
 requires-python = ">=3.7"
 
 dependencies = [
-  "openai<0.28",
+  "importlib_metadata<7",
+  "openai<1",
   "prompt_toolkit<4",
   "pygments<3",
-  "requests<3",
+  "retry<1",
+  "tiktoken<1",
   "tomlkit<1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/craigmbooth/aissist"
 "Bug Tracker" = "https://github.com/craigmbooth/aissist/issues"
 
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
 [project.scripts]
-ai = "aissist.aissistant:main"
+ai = "aissist.aissist:main"
```

