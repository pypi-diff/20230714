# Comparing `tmp/loggerr-1.0.0.tar.gz` & `tmp/loggerr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/loggerr-1.0.0.tar", last modified: Thu Aug 26 13:40:37 2021, max compression
+gzip compressed data, was "loggerr-1.1.0.tar", last modified: Fri Jul 14 13:39:03 2023, max compression
```

## Comparing `loggerr-1.0.0.tar` & `loggerr-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-26 13:40:37.000000 loggerr-1.0.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2021-08-26 13:40:37.000000 loggerr-1.0.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1739 2021-08-26 13:40:30.000000 loggerr-1.0.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-26 13:40:37.000000 loggerr-1.0.0/loggerr/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2599 2021-08-26 13:40:30.000000 loggerr-1.0.0/loggerr/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-26 13:40:37.000000 loggerr-1.0.0/loggerr.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2021-08-26 13:40:37.000000 loggerr-1.0.0/loggerr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2021-08-26 13:40:37.000000 loggerr-1.0.0/loggerr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-26 13:40:37.000000 loggerr-1.0.0/loggerr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2021-08-26 13:40:37.000000 loggerr-1.0.0/loggerr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-08-26 13:40:37.000000 loggerr-1.0.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2021-08-26 13:40:30.000000 loggerr-1.0.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-14 13:39:03.338732 loggerr-1.1.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1067 2023-07-14 13:38:53.000000 loggerr-1.1.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2274 2023-07-14 13:39:03.338732 loggerr-1.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1877 2023-07-14 13:38:53.000000 loggerr-1.1.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-14 13:39:03.338732 loggerr-1.1.0/loggerr/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2626 2023-07-14 13:38:53.000000 loggerr-1.1.0/loggerr/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-14 13:39:03.338732 loggerr-1.1.0/loggerr.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2274 2023-07-14 13:39:03.000000 loggerr-1.1.0/loggerr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      170 2023-07-14 13:39:03.000000 loggerr-1.1.0/loggerr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-14 13:39:03.000000 loggerr-1.1.0/loggerr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-07-14 13:39:03.000000 loggerr-1.1.0/loggerr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-14 13:39:03.338732 loggerr-1.1.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2023-07-14 13:38:53.000000 loggerr-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `loggerr-1.0.0/PKG-INFO` & `loggerr-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 Metadata-Version: 2.1
 Name: loggerr
-Version: 1.0.0
+Version: 1.1.0
 Summary: Zero configuration JSON logger(r)
 Home-page: https://github.com/fiverr/python-loggerr
 Author: fiverr
 Author-email: sre@fiverr.com
 License: MIT
-Description: # loggerr [![](https://img.shields.io/pypi/v/loggerr?style=flat-square)](https://pypi.org/project/loggerr/) [![](https://img.shields.io/static/v1?label=github&message=python-loggerr&labelColor=black&color=3572a5&style=flat-square&logo=github)](https://github.com/fiverr/python-loggerr) [![](https://circleci.com/gh/fiverr/python-loggerr.svg?style=svg)](https://circleci.com/gh/fiverr/python-loggerr)
-        
-        ## Zero configuration JSON logger(r)
-        
-        
-        ```py
-        from loggerr import Loggerr
-        
-        logger = Loggerr("warn")
-        
-        logger.info("Something going as expected", { "host": socket.gethostname() }) # ignored
-        logger.warn("Something must have gone terribly wrong") # sent
-        
-        except Exception as e:
-            logger.error(e, { request: "this was the request" })
-        ```
-        
-        ### Log level
-        Create logger instance with a minimal log level
-        
-        Log levels are (respectively):
-        - debug
-        - verbose
-        - info
-        - warn
-        - error
-        - critical
-        
-        For example, a logger with log level "warn" will only print logs with level "warn", "error", or "critical".
-        
-        ### Arguments
-        Loggerr class accepts one or two arguments:
-        
-        1. {string} Case insensitive name of **minimal** log level. defaults to 'info'
-        2. {dictionary} {'Key':'Value'} pairs, optional. Persistent enrichment fields for all log records
-        
-        ```py
-        logger = Loggerr("warn", { "host": socket.gethostname() })
-        ```
-        
-        Logger functions accept one or two arguments:
-        
-        1. {any} Record's "message" field. Traditionally this would be a string or an exception.
-        2. {dictionary} {'Key':'Value'} pairs, optional. Values should be JSON serializable
-        
-        ### Synonyms
-        A couple of function synonyms have been placed to your convenience:
-        
-        | function | will log with level
-        | - | -
-        | `logger.log(...)` | "info"
-        | `logger.warning(...)` | "warn"
-        | `logger.fatal(...)` | "critical"
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# loggerr [![](https://img.shields.io/pypi/v/loggerr?style=flat-square)](https://pypi.org/project/loggerr/) [![](https://img.shields.io/static/v1?label=github&message=python-loggerr&labelColor=black&color=3572a5&style=flat-square&logo=github)](https://github.com/fiverr/python-loggerr) [![](https://circleci.com/gh/fiverr/python-loggerr.svg?style=svg)](https://circleci.com/gh/fiverr/python-loggerr)
+
+## Zero configuration JSON logger(r)
+
+
+```py
+from loggerr import Loggerr
+
+logger = Loggerr("warn")
+
+logger.info("Something going as expected", { "host": socket.gethostname() }) # ignored
+logger.warn("Something must have gone terribly wrong") # sent
+
+except Exception as e:
+    logger.error(e, { request: "this was the request" })
+```
+
+### Log level
+Create logger instance with a minimal log level
+
+Log levels are (respectively):
+- debug
+- verbose
+- info
+- warn
+- error
+- critical
+
+For example, a logger with log level "warn" will only print logs with level "warn", "error", or "critical".
+
+### Synonyms
+A couple of function synonyms have been placed to your convenience:
+
+| function | will log with level
+| - | -
+| `logger.log(...)` | "info"
+| `logger.warning(...)` | "warn"
+| `logger.fatal(...)` | "critical"
+| `logger.panic(...)` | "critical"
+
+### Arguments
+**Create**: Loggerr class accepts one or two arguments:
+
+1. {string} Case insensitive name of **minimal** log level. defaults to 'info'
+2. {dictionary} {'Key':'Value'} pairs, optional. Persistent enrichment fields for all log records
+
+```py
+logger = Loggerr(os.environ["LOG_LEVEL"], { "host": socket.gethostname() })
+```
+
+**Send**:Logger functions accept one or two arguments:
+
+1. {any} Record's "message" field. Traditionally this would be a string or an exception.
+2. {dictionary} {'Key':'Value'} pairs, optional. Values should be JSON serializable
+
+```py
+logger.info("something, something", { dark: "side" })
+```
+
+
```

### Comparing `loggerr-1.0.0/README.md` & `loggerr-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,30 +24,35 @@
 - info
 - warn
 - error
 - critical
 
 For example, a logger with log level "warn" will only print logs with level "warn", "error", or "critical".
 
+### Synonyms
+A couple of function synonyms have been placed to your convenience:
+
+| function | will log with level
+| - | -
+| `logger.log(...)` | "info"
+| `logger.warning(...)` | "warn"
+| `logger.fatal(...)` | "critical"
+| `logger.panic(...)` | "critical"
+
 ### Arguments
-Loggerr class accepts one or two arguments:
+**Create**: Loggerr class accepts one or two arguments:
 
 1. {string} Case insensitive name of **minimal** log level. defaults to 'info'
 2. {dictionary} {'Key':'Value'} pairs, optional. Persistent enrichment fields for all log records
 
 ```py
-logger = Loggerr("warn", { "host": socket.gethostname() })
+logger = Loggerr(os.environ["LOG_LEVEL"], { "host": socket.gethostname() })
 ```
 
-Logger functions accept one or two arguments:
+**Send**:Logger functions accept one or two arguments:
 
 1. {any} Record's "message" field. Traditionally this would be a string or an exception.
 2. {dictionary} {'Key':'Value'} pairs, optional. Values should be JSON serializable
 
-### Synonyms
-A couple of function synonyms have been placed to your convenience:
-
-| function | will log with level
-| - | -
-| `logger.log(...)` | "info"
-| `logger.warning(...)` | "warn"
-| `logger.fatal(...)` | "critical"
+```py
+logger.info("something, something", { dark: "side" })
+```
```

### Comparing `loggerr-1.0.0/loggerr/__init__.py` & `loggerr-1.1.0/loggerr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     'critical',
     'silent'
 ]
 
 synonyms = [
     ['log', 'info'],
     ['warning', 'warn'],
-    ['fatal', 'critical']
+    ['fatal', 'critical'],
+    ['panic', 'critical']
 ]
 
 
 class Loggerr:
     """ Create a JSON logger with minimal log level
     Args:
         logLevel (str): Minimal log level (case insensitive)
```

### Comparing `loggerr-1.0.0/loggerr.egg-info/PKG-INFO` & `loggerr-1.1.0/loggerr.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 Metadata-Version: 2.1
 Name: loggerr
-Version: 1.0.0
+Version: 1.1.0
 Summary: Zero configuration JSON logger(r)
 Home-page: https://github.com/fiverr/python-loggerr
 Author: fiverr
 Author-email: sre@fiverr.com
 License: MIT
-Description: # loggerr [![](https://img.shields.io/pypi/v/loggerr?style=flat-square)](https://pypi.org/project/loggerr/) [![](https://img.shields.io/static/v1?label=github&message=python-loggerr&labelColor=black&color=3572a5&style=flat-square&logo=github)](https://github.com/fiverr/python-loggerr) [![](https://circleci.com/gh/fiverr/python-loggerr.svg?style=svg)](https://circleci.com/gh/fiverr/python-loggerr)
-        
-        ## Zero configuration JSON logger(r)
-        
-        
-        ```py
-        from loggerr import Loggerr
-        
-        logger = Loggerr("warn")
-        
-        logger.info("Something going as expected", { "host": socket.gethostname() }) # ignored
-        logger.warn("Something must have gone terribly wrong") # sent
-        
-        except Exception as e:
-            logger.error(e, { request: "this was the request" })
-        ```
-        
-        ### Log level
-        Create logger instance with a minimal log level
-        
-        Log levels are (respectively):
-        - debug
-        - verbose
-        - info
-        - warn
-        - error
-        - critical
-        
-        For example, a logger with log level "warn" will only print logs with level "warn", "error", or "critical".
-        
-        ### Arguments
-        Loggerr class accepts one or two arguments:
-        
-        1. {string} Case insensitive name of **minimal** log level. defaults to 'info'
-        2. {dictionary} {'Key':'Value'} pairs, optional. Persistent enrichment fields for all log records
-        
-        ```py
-        logger = Loggerr("warn", { "host": socket.gethostname() })
-        ```
-        
-        Logger functions accept one or two arguments:
-        
-        1. {any} Record's "message" field. Traditionally this would be a string or an exception.
-        2. {dictionary} {'Key':'Value'} pairs, optional. Values should be JSON serializable
-        
-        ### Synonyms
-        A couple of function synonyms have been placed to your convenience:
-        
-        | function | will log with level
-        | - | -
-        | `logger.log(...)` | "info"
-        | `logger.warning(...)` | "warn"
-        | `logger.fatal(...)` | "critical"
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# loggerr [![](https://img.shields.io/pypi/v/loggerr?style=flat-square)](https://pypi.org/project/loggerr/) [![](https://img.shields.io/static/v1?label=github&message=python-loggerr&labelColor=black&color=3572a5&style=flat-square&logo=github)](https://github.com/fiverr/python-loggerr) [![](https://circleci.com/gh/fiverr/python-loggerr.svg?style=svg)](https://circleci.com/gh/fiverr/python-loggerr)
+
+## Zero configuration JSON logger(r)
+
+
+```py
+from loggerr import Loggerr
+
+logger = Loggerr("warn")
+
+logger.info("Something going as expected", { "host": socket.gethostname() }) # ignored
+logger.warn("Something must have gone terribly wrong") # sent
+
+except Exception as e:
+    logger.error(e, { request: "this was the request" })
+```
+
+### Log level
+Create logger instance with a minimal log level
+
+Log levels are (respectively):
+- debug
+- verbose
+- info
+- warn
+- error
+- critical
+
+For example, a logger with log level "warn" will only print logs with level "warn", "error", or "critical".
+
+### Synonyms
+A couple of function synonyms have been placed to your convenience:
+
+| function | will log with level
+| - | -
+| `logger.log(...)` | "info"
+| `logger.warning(...)` | "warn"
+| `logger.fatal(...)` | "critical"
+| `logger.panic(...)` | "critical"
+
+### Arguments
+**Create**: Loggerr class accepts one or two arguments:
+
+1. {string} Case insensitive name of **minimal** log level. defaults to 'info'
+2. {dictionary} {'Key':'Value'} pairs, optional. Persistent enrichment fields for all log records
+
+```py
+logger = Loggerr(os.environ["LOG_LEVEL"], { "host": socket.gethostname() })
+```
+
+**Send**:Logger functions accept one or two arguments:
+
+1. {any} Record's "message" field. Traditionally this would be a string or an exception.
+2. {dictionary} {'Key':'Value'} pairs, optional. Values should be JSON serializable
+
+```py
+logger.info("something, something", { dark: "side" })
+```
+
+
```

### Comparing `loggerr-1.0.0/setup.py` & `loggerr-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="loggerr",
-    version="1.0.0",
+    version="1.1.0",
     author="fiverr",
     author_email="sre@fiverr.com",
     description="Zero configuration JSON logger(r)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fiverr/python-loggerr",
     license="MIT",
```

