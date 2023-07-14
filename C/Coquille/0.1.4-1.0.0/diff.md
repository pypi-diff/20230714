# Comparing `tmp/Coquille-0.1.4.tar.gz` & `tmp/Coquille-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-0.1.4.tar", last modified: Wed May  3 12:15:11 2023, max compression
+gzip compressed data, was "Coquille-1.0.0.tar", last modified: Fri Jul 14 10:59:06 2023, max compression
```

## Comparing `Coquille-0.1.4.tar` & `Coquille-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.4/.gitignore
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.4/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-03 12:15:11.740973 Coquille-0.1.4/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2515 2023-05-03 12:04:51.000000 Coquille-0.1.4/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.737640 Coquille-0.1.4/examples/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.737640 Coquille-0.1.4/examples/coquille_context/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.4/examples/coquille_context/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.4/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/examples/coquille_write/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      436 2023-05-03 12:04:51.000000 Coquille-0.1.4/examples/coquille_write/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       45 2023-05-03 12:04:51.000000 Coquille-0.1.4/examples/coquille_write/output.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    44980 2023-05-03 12:04:51.000000 Coquille-0.1.4/examples/coquille_write/screenshot.png
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-03 12:14:56.000000 Coquille-0.1.4/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-03 12:15:11.740973 Coquille-0.1.4/setup.cfg
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 21:08:25.000000 Coquille-0.1.4/setup.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.737640 Coquille-0.1.4/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/src/Coquille.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      610 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-03 12:15:11.000000 Coquille-0.1.4/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/src/coquille/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.4/src/coquille/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     6283 2023-05-03 12:14:29.000000 Coquille-0.1.4/src/coquille/coquille.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 21:08:25.000000 Coquille-0.1.4/src/coquille/sequences.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.4/src/coquille/typeshed.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-03 12:15:11.740973 Coquille-0.1.4/tests/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:08:25.000000 Coquille-0.1.4/tests/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 21:08:25.000000 Coquille-0.1.4/tests/coquille_test.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 21:08:25.000000 Coquille-0.1.4/tests/sequences_test.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.0.0/.gitignore
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.0.0/LICENSE
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4690 2023-07-14 10:59:06.371747 Coquille-1.0.0/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     3086 2023-07-14 10:50:09.000000 Coquille-1.0.0/README.md
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.365081 Coquille-1.0.0/examples/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.368414 Coquille-1.0.0/examples/coquille_context/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_context/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    31985 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.368414 Coquille-1.0.0/examples/coquille_write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      436 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_write/output.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    44980 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_write/screenshot.png
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      533 2023-07-14 10:54:29.000000 Coquille-1.0.0/pyproject.toml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-14 10:59:06.371747 Coquille-1.0.0/setup.cfg
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.365081 Coquille-1.0.0/src/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/src/Coquille.egg-info/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4690 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      601 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       29 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/src/coquille/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.0.0/src/coquille/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     6327 2023-07-14 10:57:15.000000 Coquille-1.0.0/src/coquille/coquille.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.0.0/src/coquille/sequences.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      340 2023-07-14 10:50:09.000000 Coquille-1.0.0/src/coquille/typeshed.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/tests/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.0.0/tests/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-14 10:50:09.000000 Coquille-1.0.0/tests/coquille_test.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.0.0/tests/sequences_test.py
```

### Comparing `Coquille-0.1.4/.gitignore` & `Coquille-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.4/.pre-commit-config.yaml` & `Coquille-1.0.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v4.4.0
       hooks:
           - id: trailing-whitespace
           - id: end-of-file-fixer
           - id: check-yaml
           - id: debug-statements
-    - repo: https://github.com/asottile/reorder_python_imports
-      rev: v3.9.0
+    - repo: https://github.com/asottile/reorder-python-imports
+      rev: v3.10.0
       hooks:
           - id: reorder-python-imports
             args: [--py311-plus]
     - repo: https://github.com/asottile/add-trailing-comma
-      rev: v2.4.0
+      rev: v3.0.0
       hooks:
           - id: add-trailing-comma
             args: [--py36-plus]
```

### Comparing `Coquille-0.1.4/LICENSE` & `Coquille-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.4/PKG-INFO` & `Coquille-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: Coquille
-Version: 0.1.4
-Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
-Author: Qexat
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Coquille
 
 Coquille (IPA: `/kɔ.kij/`, english: 'shell' or 'typo') is a library that wraps terminal escape sequences to easily apply them to a stream.
 
 ## Notes
 
 Requires Python 3.9 or higher.
@@ -95,7 +82,15 @@
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_write/screenshot.png)
 
 Source code: [examples/coquille_write/](https://github.com/qexat/Coquille/blob/main/examples/coquille_write/__main__.py)
 
 ## Documentation
 
 Coming soon! 🚧
+
+## Related projects
+
+If you like Coquille, you might want to check these projects as well:
+
+- [Colorama](https://github.com/tartley/colorama): a simple cross-platform colored terminal text in Python, by [Jonathan Hartley](https://github.com/tartley)
+- [Rich_](https://github.com/Textualize/rich): a Python library for rich text and beautiful formatting in the terminal, by [Dave Pearson](https://github.com/davep)
+- [Dahlia](https://github.com/dahlia-lib/dahlia): a simple text formatting package, inspired by the game Minecraft, by [trag1c](https://github.com/trag1c/)
```

### Comparing `Coquille-0.1.4/examples/coquille_context/screenshot.png` & `Coquille-1.0.0/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.4/examples/coquille_write/screenshot.png` & `Coquille-1.0.0/examples/coquille_write/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.4/src/Coquille.egg-info/SOURCES.txt` & `Coquille-1.0.0/src/Coquille.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
-setup.py
 examples/coquille_context/__main__.py
 examples/coquille_context/screenshot.png
 examples/coquille_write/__main__.py
 examples/coquille_write/output.txt
 examples/coquille_write/screenshot.png
 src/Coquille.egg-info/PKG-INFO
 src/Coquille.egg-info/SOURCES.txt
```

### Comparing `Coquille-0.1.4/src/coquille/coquille.py` & `Coquille-1.0.0/src/coquille/coquille.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pyright: reportUnusedCallResult = false
+
 from __future__ import annotations
 
 import sys
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import overload
 from typing import TYPE_CHECKING
@@ -80,15 +82,15 @@
 ) -> None:
     """
     Apply an escape sequence to a stream (by default, stdout).
     """
 
     string: EscapeSequence = prepare(sequence, *args, **kwargs)
     target = file or sys.stdout
-    target.write(string)  # type: ignore[unused]
+    target.write(string)
 
 
 class _ContextCoquille:
     __slots__ = ("__sequences", "__file")  # private slots
 
     def __init__(
         self,
@@ -243,7 +245,10 @@
         """
         Leave the Coquille context.
 
         Soft reset the escape sequences applied since then.
         """
 
         apply(soft_reset, self.file)
+
+
+write = Coquille.write
```

### Comparing `Coquille-0.1.4/src/coquille/sequences.py` & `Coquille-1.0.0/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.4/tests/coquille_test.py` & `Coquille-1.0.0/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.4/tests/sequences_test.py` & `Coquille-1.0.0/tests/sequences_test.py`

 * *Files identical despite different names*

