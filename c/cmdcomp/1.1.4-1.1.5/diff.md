# Comparing `tmp/cmdcomp-1.1.4.tar.gz` & `tmp/cmdcomp-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.4.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.5.tar", max compression
```

## Comparing `cmdcomp-1.1.4.tar` & `cmdcomp-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1512 2023-07-14 15:11:02.127905 cmdcomp-1.1.4/README.md
--rw-r--r--   0        0        0       79 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2123 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/exception.py
--rw-r--r--   0        0        0       64 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1732 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1277 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1700 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 cmdcomp-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-14 16:28:13.190878 cmdcomp-1.1.5/README.md
+-rw-r--r--   0        0        0       79 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2275 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/exception.py
+-rw-r--r--   0        0        0       64 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/main.py
+-rw-r--r--   0        0        0       81 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1732 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1717 2023-07-14 16:28:13.194878 cmdcomp-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 cmdcomp-1.1.5/PKG-INFO
```

### Comparing `cmdcomp-1.1.4/README.md` & `cmdcomp-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/cmdcomp/completion.py` & `cmdcomp-1.1.5/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/cmdcomp/config/app_info.py` & `cmdcomp-1.1.5/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/cmdcomp/config/command/command.py` & `cmdcomp-1.1.5/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/cmdcomp/config/config.py` & `cmdcomp-1.1.5/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.5/cmdcomp/templates/bash.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.5/cmdcomp/templates/zsh.sh.jinja`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.4/pyproject.toml` & `cmdcomp-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.4"
+version = "1.1.5"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -28,14 +28,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0"
 jinja2 = "^3.1.2"
 mergedeep = "^1.3.4"
 pyyaml = "^6.0"
+rich = "^13.4.2"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
 pyright = "^1.1.300"
```

### Comparing `cmdcomp-1.1.4/PKG-INFO` & `cmdcomp-1.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.4
+Version: 1.1.5
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Project-URL: Repository, https://github.com/yassun4dev/cmdcomp
 Description-Content-Type: text/markdown
 
 # Command Completion Generator Tool
 
 <p align="center">
     <a href="https://github.com/yassun4dev/cmdcomp/actions">
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.4 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.5 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Software Development Classifier: Typing :: Typed Requires-Dist: jinja2
 (>=3.1.2,<4.0.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
-pydantic (>=2.0,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Project-URL:
-Repository, https://github.com/yassun4dev/cmdcomp Description-Content-Type:
-text/markdown # Command Completion Generator Tool
+pydantic (>=2.0,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: rich
+(>=13.4.2,<14.0.0) Project-URL: Repository, https://github.com/yassun4dev/
+cmdcomp Description-Content-Type: text/markdown # Command Completion Generator
+Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
 `cmdcomp` generate shell completion file (bash or zsh) from config toml file.
 ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
 --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
 --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
 shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
 TOML file formats. ### Sample ```toml [cmdcomp] version = "1" [app] name =
```

