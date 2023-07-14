# Comparing `tmp/cmdcomp-1.1.7.tar.gz` & `tmp/cmdcomp-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.7.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.8.tar", max compression
```

## Comparing `cmdcomp-1.1.7.tar` & `cmdcomp-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1512 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/README.md
--rw-r--r--   0        0        0       79 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2541 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/exception.py
--rw-r--r--   0        0        0       85 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1732 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1717 2023-07-14 17:41:54.178904 cmdcomp-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/README.md
+-rw-r--r--   0        0        0       79 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2451 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/exception.py
+-rw-r--r--   0        0        0       85 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/main.py
+-rw-r--r--   0        0        0      131 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1732 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1696 2023-07-14 17:57:54.925634 cmdcomp-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.1.8/PKG-INFO
```

### Comparing `cmdcomp-1.1.7/README.md` & `cmdcomp-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/cmdcomp/app.py` & `cmdcomp-1.1.8/cmdcomp/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,46 +20,44 @@
 
         parser = ArgumentParser(
             prog="cmdcomp",
             description="A command-line tool for comparing commands.",
         )
 
         parser.add_argument(
-            "--version", action="version", version=f"%(prog)s {__version__}"
+            "--version",
+            action="version",
+            version=f"%(prog)s {__version__}",
         )
 
         parser.add_argument(
             "--file",
             "-f",
             required=True,
-            metavar="FILE",
             type=FileType("rb"),
             help="config file ('.json', '.yaml', '.toml' support).",
         )
 
         parser.add_argument(
             "--shell-type",
             required=True,
-            metavar="SHELL_TYPE",
             type=ShellType,
             choices=list(ShellType),
             help="target shell type.",
         )
 
         parser.add_argument(
             "--output-file",
             "-o",
-            metavar="OUTPUT_FILE",
             type=FileType("w"),
             help="output file (Default=stdout).",
         )
 
         parser.add_argument(
             "--verbose",
-            "-v",
             action=BooleanOptionalAction,
             help="output verbose log.",
         )
 
         space = parser.parse_args(args)
 
         logging.basicConfig(
```

### Comparing `cmdcomp-1.1.7/cmdcomp/completion.py` & `cmdcomp-1.1.8/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/cmdcomp/config/app_info.py` & `cmdcomp-1.1.8/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/cmdcomp/config/command/command.py` & `cmdcomp-1.1.8/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/cmdcomp/config/config.py` & `cmdcomp-1.1.8/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.8/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.8/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.7/pyproject.toml` & `cmdcomp-1.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.7"
+version = "1.1.8"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -66,8 +66,8 @@
 exclude = ["**/__pycache__"]
 reportPrivateImportUsage = "none"
 reportUnusedImport = true
 
 [tool.mypy]
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
-module = ["colorama", "authlib"]
+module = []
```

### Comparing `cmdcomp-1.1.7/PKG-INFO` & `cmdcomp-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.7
+Version: 1.1.8
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.7 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.8 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

