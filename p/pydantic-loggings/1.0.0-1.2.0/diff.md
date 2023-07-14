# Comparing `tmp/pydantic-loggings-1.0.0.tar.gz` & `tmp/pydantic-loggings-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-1.0.0.tar", last modified: Wed Jul 12 19:33:17 2023, max compression
+gzip compressed data, was "pydantic-loggings-1.2.0.tar", last modified: Fri Jul 14 17:57:06 2023, max compression
```

## Comparing `pydantic-loggings-1.0.0.tar` & `pydantic-loggings-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     3162 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2399 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2418 2023-07-12 19:33:06.000000 pydantic-loggings-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/loggers.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/loggings.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3162 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-14 17:56:56.000000 pydantic-loggings-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.846429 pydantic-loggings-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.846429 pydantic-loggings-1.2.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.846429 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/top_level.txt
```

### Comparing `pydantic-loggings-1.0.0/PKG-INFO` & `pydantic-loggings-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.0.0
+Version: 1.2.0
+Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
-Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
-Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
+Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
+Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
 Classifier: Environment :: Console
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# Configure Python logging from environment variables with pydantic (settings) Model [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
+# Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 
-## [Installation](https://pypi.org/project/pydantic-loggings/)
+[![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
+
+## Installation
 
 ```shell
 pip install pydantic-loggings
 ```
 
-## [Usage](./examples)
+## Usage
+
+- [examples](./examples)
 
 ### out of the box
 
 ```py
-from pydantic_loggings.base import Logging # base Logging
+from pydantic_loggings.base import Logging
 
 
-logger = Logging().get_logger()
+logger = Logging().get_logger(configure=True)
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG   debug
 # 01-01 00:00:00 INFO    info
 # 01-01 00:00:00 WARNING warning
 ```
 
-### default logging
+### Default Logging
 
 ```py
 from pydantic_loggings.not_set import Logging
 
 
-logger = Logging().get_logger()
+logger = Logging().get_logger(configure=True)
+
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # warning
 ```
 
-### config from env file
+### Configure from Environment
 
 ```py
 from pathlib import Path
 
 from pydantic_loggings.not_set import Logging
 
 
 env_file = Path(__file__).parent / '.env'
-logger = Logging(
-    _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
-).get_logger()
+logger = Logging(_env_file=env_file).get_logger(configure=True)
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 [root]   DEBUG (main.py:11) debug
 # 01-01 00:00:00 [root]    INFO (main.py:12) info
@@ -101,12 +105,12 @@
 # and/or:
 
 # log__formatters='{"my_formatter":{"datefmt":"%m-%d %H:%M:%S","format":"{asctime} [{name}] {levelname:>7} ({filename}:{lineno}) {message}","style":"{"}}'
 # log__handlers='{"my_handler":{"class_":"logging.StreamHandler","formatter":"my_formatter"}}'
 # log__loggers='{"root":{"level":"DEBUG","handlers":["my_handler"]}}'
 ```
 
-### `Logging`s
+### Loggings
 
 - not_set
 - base
 - rich
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic-loggings-1.0.0/README.md` & `pydantic-loggings-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-# Configure Python logging from environment variables with pydantic (settings) Model [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
+# Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 
-## [Installation](https://pypi.org/project/pydantic-loggings/)
+[![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
+
+## Installation
 
 ```shell
 pip install pydantic-loggings
 ```
 
-## [Usage](./examples)
+## Usage
+
+- [examples](./examples)
 
 ### out of the box
 
 ```py
-from pydantic_loggings.base import Logging # base Logging
+from pydantic_loggings.base import Logging
 
 
-logger = Logging().get_logger()
+logger = Logging().get_logger(configure=True)
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG   debug
 # 01-01 00:00:00 INFO    info
 # 01-01 00:00:00 WARNING warning
 ```
 
-### default logging
+### Default Logging
 
 ```py
 from pydantic_loggings.not_set import Logging
 
 
-logger = Logging().get_logger()
+logger = Logging().get_logger(configure=True)
+
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # warning
 ```
 
-### config from env file
+### Configure from Environment
 
 ```py
 from pathlib import Path
 
 from pydantic_loggings.not_set import Logging
 
 
 env_file = Path(__file__).parent / '.env'
-logger = Logging(
-    _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
-).get_logger()
+logger = Logging(_env_file=env_file).get_logger(configure=True)
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 [root]   DEBUG (main.py:11) debug
 # 01-01 00:00:00 [root]    INFO (main.py:12) info
@@ -82,12 +85,12 @@
 # and/or:
 
 # log__formatters='{"my_formatter":{"datefmt":"%m-%d %H:%M:%S","format":"{asctime} [{name}] {levelname:>7} ({filename}:{lineno}) {message}","style":"{"}}'
 # log__handlers='{"my_handler":{"class_":"logging.StreamHandler","formatter":"my_formatter"}}'
 # log__loggers='{"root":{"level":"DEBUG","handlers":["my_handler"]}}'
 ```
 
-### `Logging`s
+### Loggings
 
 - not_set
 - base
 - rich
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic-loggings-1.0.0/pyproject.toml` & `pydantic-loggings-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+[project.urls]
+Homepage = "https://github.com/m9810223/pydantic-loggings"
+Source = "https://github.com/m9810223/pydantic-loggings"
+
 [project]
+name = "pydantic-loggings"
+description = "Configure 🎁 Your 🤗 Python 🐍 Logging 📝"
+version = "1.2.0"
 authors = [
   { name = "m9810223", email = "m9810223@gmail.com" },
 ]
-name = "pydantic-loggings"
-readme = "README.md"
 requires-python = ">=3.9"
-version = "1.0.0"
+readme = "README.md"
 
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3",
@@ -21,23 +26,20 @@
 ]
 
 dependencies = [
   "pydantic>=2.0",
   "pydantic-settings>=2.0",
 ]
 
-[project.urls]
-Homepage = "https://github.com/m9810223/pydantic-logging-settings"
-Source = "https://github.com/m9810223/pydantic-logging-settings"
-
-[tool.semantic_release]
-# https://python-semantic-release.readthedocs.io/en/latest/configuration.html
+[tool.semantic_release] # https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 build_command = "pip install pdm && pdm build"
-# upload_to_repository = false
+upload_to_repository = true
+upload_to_release = false
 version_toml = "pyproject.toml:project.version"
+changelog_file = "./misc/CHANGELOG.md"
 
 [tool.pdm.scripts]
 debug = { composite = ["dev"], env = { DEBUG = '1' } }
 dev = "python dev.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
@@ -45,14 +47,15 @@
   "pyright>=1.1.316",
   "pytest-cov>=4.1.0",
   "hypothesis>=6.80.0",
   "pytest-xdist>=3.3.1",
   "pytest-mock>=3.11.1",
   "rich>=13.4.2",
 ]
+
 [tool.black] # https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
 skip-string-normalization = 1
 
 [tool.ruff]
 extend-select = [
   "W", # pycodestyle Warning
   "I", # isort
@@ -64,25 +67,22 @@
 ]
 ignore = [
   "E501", # line-too-long
   "S101", # Use of `assert` detected
   "TRY003", # raise-vanilla-args  # "TRY400", # error-instead-of-exception
 ]
 
-# upload_to_repository
-[tool.ruff.isort]
-# https://beta.ruff.rs/docs/settings/#isort
+[tool.ruff.isort] # https://beta.ruff.rs/docs/settings/#isort
 force-single-line = true
 lines-after-imports = 2
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
+addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short --cov=src --cov-report=term --cov-report=html:./htmlcov"
 # https://docs.pytest.org/en/stable/reference/reference.html
 # https://docs.pytest.org/en/stable/explanation/goodpractices.html
 # https://docs.pytest.org/en/stable/example/pythoncollection.html
-addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short --cov=src --cov-report=term --cov-report=html:./htmlcov"
 
-# https://coverage.readthedocs.io/en/stable/config.html
-[tool.coverage.run]
+[tool.coverage.run] # https://coverage.readthedocs.io/en/stable/config.html
 omit = ["__init__.py"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/base/loggings.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggings.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,30 +63,27 @@
     @property
     def configuration(self):
         return self.model_dump()
 
     def configure(self):
         self.configurator(self.configuration).configure()
 
-    def is_valid_logger_name(self, logger_name: str, /):
-        return logger_name in ['', 'root', *(self.loggers or {}).keys()]
-
     def get_logger(
         self,
         logger_name: str = '',
         /,
         *,
         level: t.Optional[t.Union[int, str]] = None,
         force_level: bool = False,
-        configure: bool = True,
+        configure: bool = False,
     ):
         if configure:
             self.configure()
         logger = logging.getLogger(name=logger_name)
         if level is not None:
-            if force_level is True:
+            if force_level:
                 logger.setLevel(level=level)
             elif logging.NOTSET == logger.level:
                 logger.setLevel(level=level)
             elif logging.NOTSET == logger.getEffectiveLevel():
                 logger.setLevel(level=level)
         return logger
```

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings/rich/handlers.py` & `pydantic-loggings-1.2.0/src/pydantic_loggings/rich/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.0.0
+Version: 1.2.0
+Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
-Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
-Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
+Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
+Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
 Classifier: Environment :: Console
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-# Configure Python logging from environment variables with pydantic (settings) Model [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
+# Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 
-## [Installation](https://pypi.org/project/pydantic-loggings/)
+[![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
+
+## Installation
 
 ```shell
 pip install pydantic-loggings
 ```
 
-## [Usage](./examples)
+## Usage
+
+- [examples](./examples)
 
 ### out of the box
 
 ```py
-from pydantic_loggings.base import Logging # base Logging
+from pydantic_loggings.base import Logging
 
 
-logger = Logging().get_logger()
+logger = Logging().get_logger(configure=True)
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG   debug
 # 01-01 00:00:00 INFO    info
 # 01-01 00:00:00 WARNING warning
 ```
 
-### default logging
+### Default Logging
 
 ```py
 from pydantic_loggings.not_set import Logging
 
 
-logger = Logging().get_logger()
+logger = Logging().get_logger(configure=True)
+
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # warning
 ```
 
-### config from env file
+### Configure from Environment
 
 ```py
 from pathlib import Path
 
 from pydantic_loggings.not_set import Logging
 
 
 env_file = Path(__file__).parent / '.env'
-logger = Logging(
-    _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
-).get_logger()
+logger = Logging(_env_file=env_file).get_logger(configure=True)
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 [root]   DEBUG (main.py:11) debug
 # 01-01 00:00:00 [root]    INFO (main.py:12) info
@@ -101,12 +105,12 @@
 # and/or:
 
 # log__formatters='{"my_formatter":{"datefmt":"%m-%d %H:%M:%S","format":"{asctime} [{name}] {levelname:>7} ({filename}:{lineno}) {message}","style":"{"}}'
 # log__handlers='{"my_handler":{"class_":"logging.StreamHandler","formatter":"my_formatter"}}'
 # log__loggers='{"root":{"level":"DEBUG","handlers":["my_handler"]}}'
 ```
 
-### `Logging`s
+### Loggings
 
 - not_set
 - base
 - rich
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

