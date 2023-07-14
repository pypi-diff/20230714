# Comparing `tmp/cmdcomp-1.1.5.tar.gz` & `tmp/cmdcomp-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.5.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.6.tar", max compression
```

## Comparing `cmdcomp-1.1.5.tar` & `cmdcomp-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1512 2023-07-14 16:28:13.190878 cmdcomp-1.1.5/README.md
--rw-r--r--   0        0        0       79 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2275 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/exception.py
--rw-r--r--   0        0        0       64 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1732 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1717 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/README.md
+-rw-r--r--   0        0        0       79 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2442 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/exception.py
+-rw-r--r--   0        0        0       64 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/main.py
+-rw-r--r--   0        0        0       81 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1732 2023-07-14 17:34:03.083445 cmdcomp-1.1.6/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-14 17:34:03.087445 cmdcomp-1.1.6/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1717 2023-07-14 17:34:03.087445 cmdcomp-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.1.6/PKG-INFO
```

### Comparing `cmdcomp-1.1.5/README.md` & `cmdcomp-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/cmdcomp/app.py` & `cmdcomp-1.1.6/cmdcomp/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
         *,
         throw_exception: bool = True,
     ) -> None:
         import logging
         from argparse import ArgumentParser, BooleanOptionalAction, FileType
         from logging import getLogger
 
+        from rich.console import Console
         from rich.logging import RichHandler
 
         from cmdcomp import __version__
         from cmdcomp.completion import generate
         from cmdcomp.config.config import load
         from cmdcomp.shell_type import ShellType
 
@@ -55,28 +56,30 @@
         parser.add_argument(
             "--verbose",
             "-v",
             action=BooleanOptionalAction,
             help="output verbose log.",
         )
 
+        space = parser.parse_args(args)
+
         logging.basicConfig(
             format="%(message)s",
             handlers=[
                 RichHandler(
+                    level=logging.DEBUG if space.verbose else logging.INFO,
+                    console=Console(stderr=True),
                     show_time=False,
                     show_path=False,
                     rich_tracebacks=True,
                 )
             ],
         )
         logger = getLogger(__name__)
 
-        space = parser.parse_args(args)
-
         try:
             print(
                 generate(space.shell_type, load(space.file)),
                 file=space.output_file,
             )
 
         except Exception as e:
```

### Comparing `cmdcomp-1.1.5/cmdcomp/completion.py` & `cmdcomp-1.1.6/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/cmdcomp/config/app_info.py` & `cmdcomp-1.1.6/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/cmdcomp/config/command/command.py` & `cmdcomp-1.1.6/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/cmdcomp/config/config.py` & `cmdcomp-1.1.6/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.6/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.6/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.5/pyproject.toml` & `cmdcomp-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.5"
+version = "1.1.6"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cmdcomp-1.1.5/PKG-INFO` & `cmdcomp-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.5
+Version: 1.1.6
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
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.5 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.6 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
```

