# Comparing `tmp/pyassorted-0.7.4.tar.gz` & `tmp/pyassorted-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyassorted-0.7.4.tar", max compression
+gzip compressed data, was "pyassorted-0.7.5.tar", max compression
```

## Comparing `pyassorted-0.7.4.tar` & `pyassorted-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.7.4/LICENSE
--rw-r--r--   0        0        0     6993 2023-05-27 10:25:12.261799 pyassorted-0.7.4/README.md
--rw-r--r--   0        0        0       53 2023-04-01 13:44:09.334164 pyassorted-0.7.4/pyassorted/__init__.py
--rw-r--r--   0        0        0      116 2023-02-17 09:28:12.934937 pyassorted-0.7.4/pyassorted/asyncio/__init__.py
--rw-r--r--   0        0        0     1349 2023-04-01 13:44:09.334680 pyassorted-0.7.4/pyassorted/asyncio/executor.py
--rw-r--r--   0        0        0     2943 2023-05-15 11:57:33.581730 pyassorted-0.7.4/pyassorted/asyncio/io.py
--rw-r--r--   0        0        0     1017 2023-02-15 09:50:56.450314 pyassorted-0.7.4/pyassorted/asyncio/utils.py
--rw-r--r--   0        0        0       61 2023-03-27 15:28:16.228462 pyassorted-0.7.4/pyassorted/cache/__init__.py
--rw-r--r--   0        0        0     8109 2023-03-27 15:28:16.228823 pyassorted-0.7.4/pyassorted/cache/cache.py
--rw-r--r--   0        0        0        0 2023-05-15 11:57:33.581794 pyassorted-0.7.4/pyassorted/collections/__init__.py
--rw-r--r--   0        0        0     4048 2023-07-08 16:45:02.998148 pyassorted-0.7.4/pyassorted/collections/sqlitedict.py
--rw-r--r--   0        0        0      148 2023-05-15 11:57:33.582436 pyassorted-0.7.4/pyassorted/datetime/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-15 11:57:33.582699 pyassorted-0.7.4/pyassorted/datetime/datetime.py
--rw-r--r--   0        0        0     2013 2023-05-15 11:57:33.582972 pyassorted-0.7.4/pyassorted/datetime/timer.py
--rw-r--r--   0        0        0        0 2023-06-12 12:04:26.629790 pyassorted-0.7.4/pyassorted/encrypt/__init__.py
--rw-r--r--   0        0        0     2257 2023-07-07 10:20:46.735970 pyassorted-0.7.4/pyassorted/encrypt/io.py
--rw-r--r--   0        0        0     2602 2023-05-27 10:25:12.262734 pyassorted-0.7.4/pyassorted/io/__init__.py
--rw-r--r--   0        0        0     2365 2023-05-27 10:25:12.262951 pyassorted-0.7.4/pyassorted/io/watch.py
--rw-r--r--   0        0        0       56 2023-04-01 13:44:09.335149 pyassorted-0.7.4/pyassorted/lock/__init__.py
--rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.7.4/pyassorted/lock/filelock.py
--rw-r--r--   0        0        0        0 2023-07-07 10:23:45.350340 pyassorted-0.7.4/pyassorted/standard/__init__.py
--rw-r--r--   0        0        0     2788 2023-07-07 10:57:46.398428 pyassorted-0.7.4/pyassorted/standard/language_code.py
--rw-r--r--   0        0        0      130 2023-06-08 14:19:30.918842 pyassorted-0.7.4/pyassorted/string/__init__.py
--rw-r--r--   0        0        0      269 2023-06-08 14:18:59.300447 pyassorted-0.7.4/pyassorted/string/rand.py
--rw-r--r--   0        0        0     1924 2023-06-06 09:03:20.787667 pyassorted-0.7.4/pyassorted/string/replace.py
--rw-r--r--   0        0        0       18 2023-07-08 16:58:21.841957 pyassorted-0.7.4/pyassorted/version.py
--rw-r--r--   0        0        0      546 2023-07-08 16:57:55.007260 pyassorted-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 pyassorted-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-15 09:16:45.010069 pyassorted-0.7.5/LICENSE
+-rw-r--r--   0        0        0     6993 2023-05-27 10:25:12.261799 pyassorted-0.7.5/README.md
+-rw-r--r--   0        0        0       52 2023-07-14 09:33:12.416992 pyassorted-0.7.5/pyassorted/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-14 09:33:12.449633 pyassorted-0.7.5/pyassorted/asyncio/__init__.py
+-rw-r--r--   0        0        0     1349 2023-07-14 09:33:12.453353 pyassorted-0.7.5/pyassorted/asyncio/executor.py
+-rw-r--r--   0        0        0     2943 2023-07-14 09:33:12.448926 pyassorted-0.7.5/pyassorted/asyncio/io.py
+-rw-r--r--   0        0        0     1017 2023-07-14 09:33:12.451637 pyassorted-0.7.5/pyassorted/asyncio/utils.py
+-rw-r--r--   0        0        0       60 2023-07-14 09:33:12.424129 pyassorted-0.7.5/pyassorted/cache/__init__.py
+-rw-r--r--   0        0        0     8108 2023-07-14 09:33:12.423115 pyassorted-0.7.5/pyassorted/cache/cache.py
+-rw-r--r--   0        0        0        0 2023-05-15 11:57:33.581794 pyassorted-0.7.5/pyassorted/collections/__init__.py
+-rw-r--r--   0        0        0     4047 2023-07-14 09:33:12.445122 pyassorted-0.7.5/pyassorted/collections/sqlitedict.py
+-rw-r--r--   0        0        0      147 2023-07-14 09:33:12.427231 pyassorted-0.7.5/pyassorted/datetime/__init__.py
+-rw-r--r--   0        0        0     1053 2023-07-14 09:33:12.428569 pyassorted-0.7.5/pyassorted/datetime/datetime.py
+-rw-r--r--   0        0        0     2013 2023-05-15 11:57:33.582972 pyassorted-0.7.5/pyassorted/datetime/timer.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:04:26.629790 pyassorted-0.7.5/pyassorted/encrypt/__init__.py
+-rw-r--r--   0        0        0     2257 2023-07-07 10:20:46.735970 pyassorted-0.7.5/pyassorted/encrypt/io.py
+-rw-r--r--   0        0        0       54 2023-07-14 09:50:51.578045 pyassorted-0.7.5/pyassorted/hash/__init__.py
+-rw-r--r--   0        0        0      403 2023-07-14 09:50:30.931630 pyassorted-0.7.5/pyassorted/hash/_string.py
+-rw-r--r--   0        0        0     2602 2023-07-14 09:33:12.434006 pyassorted-0.7.5/pyassorted/io/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-14 09:33:12.435706 pyassorted-0.7.5/pyassorted/io/watch.py
+-rw-r--r--   0        0        0       55 2023-07-14 09:33:12.437117 pyassorted-0.7.5/pyassorted/lock/__init__.py
+-rw-r--r--   0        0        0     4191 2023-04-01 13:44:09.335570 pyassorted-0.7.5/pyassorted/lock/filelock.py
+-rw-r--r--   0        0        0        0 2023-07-07 10:23:45.350340 pyassorted-0.7.5/pyassorted/standard/__init__.py
+-rw-r--r--   0        0        0     2788 2023-07-07 10:57:46.398428 pyassorted-0.7.5/pyassorted/standard/language_code.py
+-rw-r--r--   0        0        0      129 2023-07-14 09:33:12.441354 pyassorted-0.7.5/pyassorted/string/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-08 14:18:59.300447 pyassorted-0.7.5/pyassorted/string/rand.py
+-rw-r--r--   0        0        0     1924 2023-06-06 09:03:20.787667 pyassorted-0.7.5/pyassorted/string/replace.py
+-rw-r--r--   0        0        0       18 2023-07-14 09:54:22.732319 pyassorted-0.7.5/pyassorted/version.py
+-rw-r--r--   0        0        0      558 2023-07-14 09:54:16.130389 pyassorted-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 pyassorted-0.7.5/PKG-INFO
```

### Comparing `pyassorted-0.7.4/LICENSE` & `pyassorted-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/README.md` & `pyassorted-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/pyassorted/asyncio/executor.py` & `pyassorted-0.7.5/pyassorted/asyncio/executor.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
-import functools
 import concurrent.futures
+import functools
 from typing import Awaitable, Callable, Union
+
 from typing_extensions import ParamSpec, TypeVar
 
 from pyassorted.asyncio.utils import is_coro_func
 
-
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 async def run_func(
     func: Union[Callable[P, T], Callable[P, Awaitable[T]]],
     *args,
```

### Comparing `pyassorted-0.7.4/pyassorted/asyncio/io.py` & `pyassorted-0.7.5/pyassorted/asyncio/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 from pathlib import Path
-from typing import Iterable, List, Optional, Text, TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterable, List, Optional, Text
 
 from pyassorted.asyncio import run_func
 
 if TYPE_CHECKING:
     from _typeshed import OpenTextMode
```

### Comparing `pyassorted-0.7.4/pyassorted/asyncio/utils.py` & `pyassorted-0.7.5/pyassorted/asyncio/utils.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import functools
 from typing import Awaitable, Callable, Union
-from typing_extensions import ParamSpec, TypeVar
 
+from typing_extensions import ParamSpec, TypeVar
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def is_coro_func(func: Union[Callable[P, T], Callable[P, Awaitable[T]]]) -> bool:
     """Check the function a coroutine function or not.
```

### Comparing `pyassorted-0.7.4/pyassorted/cache/cache.py` & `pyassorted-0.7.5/pyassorted/cache/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import ABC
 from collections import OrderedDict
 from threading import RLock
 from typing import Any, Callable, Dict, Optional, Tuple, Type, TypeVar, Union
 
 from pyassorted.asyncio import is_coro_func
 
-
 KeyType = TypeVar("KeyType")
 ValueType = TypeVar("ValueType")
 EmptyType = TypeVar("EmptyType")
 
 EMPTY_CACHE: EmptyType = object()
```

### Comparing `pyassorted-0.7.4/pyassorted/collections/sqlitedict.py` & `pyassorted-0.7.5/pyassorted/collections/sqlitedict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numbers
 import pickle
 import sqlite3
 from typing import Any, Text, Union
 
 from pyassorted.asyncio.executor import run_func
 
-
 PrimitiveType = Union[str, numbers.Number]
 
 
 class SqliteDict(object):
     """The SqliteDict class is a dictionary-like object that stores its data in a SQLite database.
 
     Examples
```

### Comparing `pyassorted-0.7.4/pyassorted/datetime/datetime.py` & `pyassorted-0.7.5/pyassorted/datetime/datetime.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
-import pytz
 from typing import Text, Union
 
+import pytz
+
 
 def aware_datetime_now(
     tz: Union[Text, "pytz.BaseTzInfo"] = pytz.UTC
 ) -> "datetime.datetime":
     """Get the current datetime in the specified timezone.
 
     Parameters
```

### Comparing `pyassorted-0.7.4/pyassorted/datetime/timer.py` & `pyassorted-0.7.5/pyassorted/datetime/timer.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/pyassorted/encrypt/io.py` & `pyassorted-0.7.5/pyassorted/encrypt/io.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/pyassorted/io/__init__.py` & `pyassorted-0.7.5/pyassorted/io/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import glob
 import json
 from pathlib import Path
 from typing import Dict, Generator, List, Optional, Text, Tuple, Union
 
-from .watch import async_watch, watch
 from pyassorted.asyncio.io import aio_open
 
+from .watch import async_watch, watch
 
 __all__ = ["async_watch", "watch"]
 
 
 def merge_objects(
     obj_1: Union[Dict, List],
     obj_2: Union[Dict, List],
```

### Comparing `pyassorted-0.7.4/pyassorted/io/watch.py` & `pyassorted-0.7.5/pyassorted/io/watch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import time
 from pathlib import Path
 from typing import AsyncGenerator, Generator, Text, Tuple, Union
 
-
 PathText = Union[Path, Text]
 
 
 def watch(
     filepath: PathText,
     period: float = 0.1,
     raise_timeout_errors: Tuple = (TimeoutError,),
```

### Comparing `pyassorted-0.7.4/pyassorted/lock/filelock.py` & `pyassorted-0.7.5/pyassorted/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/pyassorted/standard/language_code.py` & `pyassorted-0.7.5/pyassorted/standard/language_code.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/pyassorted/string/replace.py` & `pyassorted-0.7.5/pyassorted/string/replace.py`

 * *Files identical despite different names*

### Comparing `pyassorted-0.7.4/pyproject.toml` & `pyassorted-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyassorted"
-version = "0.7.4"
+version = "0.7.5"
 description = "A library has light-weight assorted utils in Prue-Python."
 authors = ["Allen Chou <f1470891079@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1, <4.0.0"
@@ -14,14 +14,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "*"
 flake8 = "*"
 flake9 = "*"
 pytest = "*"
 pytest-asyncio = "*"
 yapf = "*"
+isort = "*"
 
 [tool.poetry.group.doc.dependencies]
 sphinx = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyassorted-0.7.4/PKG-INFO` & `pyassorted-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyassorted
-Version: 0.7.4
+Version: 0.7.5
 Summary: A library has light-weight assorted utils in Prue-Python.
 License: MIT
 Author: Allen Chou
 Author-email: f1470891079@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

