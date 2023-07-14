# Comparing `tmp/commonvars-0.2.7.tar.gz` & `tmp/commonvars-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonvars-0.2.7.tar", max compression
+gzip compressed data, was "commonvars-0.2.8.tar", max compression
```

## Comparing `commonvars-0.2.7.tar` & `commonvars-0.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9583 2023-07-13 23:56:52.011047 commonvars-0.2.7/commonvars/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 commonvars-0.2.7/commonvars/py.typed
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 commonvars-0.2.7/LICENSE
--rw-r--r--   0        0        0     3336 2023-07-13 23:56:18.025639 commonvars-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3803 2023-07-14 00:00:23.113530 commonvars-0.2.7/README.md
--rw-r--r--   0        0        0     4270 1970-01-01 00:00:00.000000 commonvars-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     9623 2023-07-14 04:52:21.802097 commonvars-0.2.8/commonvars/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 commonvars-0.2.8/commonvars/py.typed
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 commonvars-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3454 2023-07-14 04:52:48.015999 commonvars-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3917 2023-07-14 00:08:34.938392 commonvars-0.2.8/README.md
+-rw-r--r--   0        0        0     4270 1970-01-01 00:00:00.000000 commonvars-0.2.8/PKG-INFO
```

### Comparing `commonvars-0.2.7/commonvars/__init__.py` & `commonvars-0.2.8/commonvars/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """`commonvars`.
 
 A simple & straight-forward Python library for creating common variables
 (context-dependent proxy objects).
 
 (C) bswck, 2023
 """
-
+import operator
 from collections.abc import Callable
 from contextlib import suppress
 from functools import partial
 from typing import Any, Protocol, TypeVar, cast, runtime_checkable
 
 __all__ = ("commonvar", "proxy")
 
@@ -203,15 +203,15 @@
         __lt__ = descriptor()
         __le__ = descriptor()
         __eq__ = descriptor()
         __ne__ = descriptor()
         __gt__ = descriptor()
         __ge__ = descriptor()
         __hash__ = descriptor()
-        __bool__ = descriptor(undefined=lambda: False)
+        __bool__ = descriptor(undefined=lambda: False, fallback=operator.truth)
         __getattr__ = descriptor()
         __setattr__ = descriptor()
         __delattr__ = descriptor()
         if cls is None:
             __dir__ = descriptor()
             __class__ = descriptor()
         else:
```

### Comparing `commonvars-0.2.7/LICENSE` & `commonvars-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `commonvars-0.2.7/pyproject.toml` & `commonvars-0.2.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-[tool.poetry]
-name = "commonvars"
-version = "0.2.7"
-description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
-authors = ["bswck <bswck.dev@gmail.com>"]
-readme = "README.md"
-homepage = "https://github.com/bswck/commonvars"
-
-[tool.poetry.dependencies]
-python = "^3.10"
-
-
-[tool.poetry.group.dev.dependencies]
-mypy = "^1.4.1"
-ruff = "^0.0.275"
-isort = "^5.12.0"
-black = "^23.3.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-# Black section
-[tool.black]
-line-length = 100 # Must be same as tool.ruff.line-length
-target-version = ['py39']
-
-[tool.coverage.run]
-omit = ['*tests*']
-
-[tool.coverage.report]
-ignore_errors = true
-
-[tool.ruff]
-# Exclude a variety of commonly ignored directories.
-exclude = [".git", "build", "dist", "var", "share", "collections"]
-line-length = 100 # Must be same as tool.black.line-length
-# Assume Python 3.9
-target-version = "py39"
-# Enable
-select = [
-    # "E", # Pycodestyle Error
-  "F", # Pyflakes
-  "W", # Pycodestyle Warning
-  # "C90", # mccabe
-  # "I", # isort
-  # "D", # Pydocstyle
-  # "YTT", # flake8-2020
-  # "ANN", # flake8-annotations
-  # "S", # flake8-bandit
-  # "BLE", # flake8-blind-except
-  # "B", # flake8-bugbear
-  "A", # flake8-builtins
-  # "C4", # flake8-comprehensions
-  # "EM", # flake8-errmsg
-  # "ISC", # flake8-implicit-str-concat
-  # "ICN", # flake8-import-conventions
-  # "PT", # flake8-pytest-style
-  # "RET", # flake8-return
-  # "SIM", # flake8-simplify
-  "PLC", # pylint
-  "PLE", # pylint
-  "PLR", # pylint
-  # "PLW", # pylint
-  # "PIE", # flake8-pie
-  # "RUF", # ruff specific
-]
-# Always autofix, but never try to fix `F401` (unused imports).
-fix = false #fix = true
-ignore = [
-  "A001", # A001 Variable `{name}` is shadowing a python builtin
-  "A002", # A002 Argument `{name}` is shadowing a python builtin
-  "A003", # Class attribute `{name}` is shadowing a python builtin"
-  "D203",
-  "D212",
-  "D107",
-  "PLR0912", # Too many branches
-  "PLR0911", # Too many return statements
-  "PLR0913", # Too many arguments to function call
-  "PLR0915", # Too many statements
-  "PLR2004", # Magic value used in comparison, consider replacing {v} with a constant variable
-]
-unfixable = ["F401"]
-
-[tool.ruff.flake8-quotes]
-docstring-quotes = "double"
-
-[tool.ruff.pydocstyle]
-convention = "google"
-
-[tool.ruff.mccabe]
-max-complexity = 12
-
-[tool.ruff.per-file-ignores]
-"*/migrations/*.py" = [
-  "D100", # Missing docstring in public module
-  "D101", # Missing docstring in public class
-  "D102", # Missing docstring in public method
-  "D103", # Missing docstring in public function
-  "D104", # Missing docstring in public package
-]
-"cmibs/*.py" = [
-  "D100", # Missing docstring in public module
-  "D101", # Missing docstring in public class
-  "D102", # Missing docstring in public method
-  "D103", # Missing docstring in public function
-  "D104", # Missing docstring in public package
-]
-"tests/*.py" = [
-  "D100", # Missing docstring in public module
-  "D101", # Missing docstring in public class
-  "D102", # Missing docstring in public method
-  "D103", # Missing docstring in public function
-  "D104", # Missing docstring in public package
-  "S101", # Use of assert detected
-  "PLR2004", # Magic value used in comparison, consider replacing {value} with a constant variable
-  "PT011", # {exc} is to broad
-]
+[tool.poetry]
+name = "commonvars"
+version = "0.2.8"
+description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
+authors = ["bswck <bswck.dev@gmail.com>"]
+readme = "README.md"
+homepage = "https://github.com/bswck/commonvars"
+
+[tool.poetry.dependencies]
+python = "^3.10"
+
+
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.4.1"
+ruff = "^0.0.275"
+isort = "^5.12.0"
+black = "^23.3.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+# Black section
+[tool.black]
+line-length = 100 # Must be same as tool.ruff.line-length
+target-version = ['py39']
+
+[tool.coverage.run]
+omit = ['*tests*']
+
+[tool.coverage.report]
+ignore_errors = true
+
+[tool.ruff]
+# Exclude a variety of commonly ignored directories.
+exclude = [".git", "build", "dist", "var", "share", "collections"]
+line-length = 100 # Must be same as tool.black.line-length
+# Assume Python 3.9
+target-version = "py39"
+# Enable
+select = [
+    # "E", # Pycodestyle Error
+  "F", # Pyflakes
+  "W", # Pycodestyle Warning
+  # "C90", # mccabe
+  # "I", # isort
+  # "D", # Pydocstyle
+  # "YTT", # flake8-2020
+  # "ANN", # flake8-annotations
+  # "S", # flake8-bandit
+  # "BLE", # flake8-blind-except
+  # "B", # flake8-bugbear
+  "A", # flake8-builtins
+  # "C4", # flake8-comprehensions
+  # "EM", # flake8-errmsg
+  # "ISC", # flake8-implicit-str-concat
+  # "ICN", # flake8-import-conventions
+  # "PT", # flake8-pytest-style
+  # "RET", # flake8-return
+  # "SIM", # flake8-simplify
+  "PLC", # pylint
+  "PLE", # pylint
+  "PLR", # pylint
+  # "PLW", # pylint
+  # "PIE", # flake8-pie
+  # "RUF", # ruff specific
+]
+# Always autofix, but never try to fix `F401` (unused imports).
+fix = false #fix = true
+ignore = [
+  "A001", # A001 Variable `{name}` is shadowing a python builtin
+  "A002", # A002 Argument `{name}` is shadowing a python builtin
+  "A003", # Class attribute `{name}` is shadowing a python builtin"
+  "D203",
+  "D212",
+  "D107",
+  "PLR0912", # Too many branches
+  "PLR0911", # Too many return statements
+  "PLR0913", # Too many arguments to function call
+  "PLR0915", # Too many statements
+  "PLR2004", # Magic value used in comparison, consider replacing {v} with a constant variable
+]
+unfixable = ["F401"]
+
+[tool.ruff.flake8-quotes]
+docstring-quotes = "double"
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.mccabe]
+max-complexity = 12
+
+[tool.ruff.per-file-ignores]
+"*/migrations/*.py" = [
+  "D100", # Missing docstring in public module
+  "D101", # Missing docstring in public class
+  "D102", # Missing docstring in public method
+  "D103", # Missing docstring in public function
+  "D104", # Missing docstring in public package
+]
+"cmibs/*.py" = [
+  "D100", # Missing docstring in public module
+  "D101", # Missing docstring in public class
+  "D102", # Missing docstring in public method
+  "D103", # Missing docstring in public function
+  "D104", # Missing docstring in public package
+]
+"tests/*.py" = [
+  "D100", # Missing docstring in public module
+  "D101", # Missing docstring in public class
+  "D102", # Missing docstring in public method
+  "D103", # Missing docstring in public function
+  "D104", # Missing docstring in public package
+  "S101", # Use of assert detected
+  "PLR2004", # Magic value used in comparison, consider replacing {value} with a constant variable
+  "PT011", # {exc} is to broad
+]
```

### Comparing `commonvars-0.2.7/README.md` & `commonvars-0.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: commonvars
+Version: 0.2.8
+Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
+Home-page: https://github.com/bswck/commonvars
+Author: bswck
+Author-email: bswck.dev@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 ## `commonvars`
 
 A simple & straight-forward Python library for creating type-safe, context-dependent proxy objects.
 
 ## Example
 
 The following example shows how to use `commonvars` with `contextvars`:
@@ -108,7 +121,8 @@
 Creates a context-dependent proxy object.
 
 #### Parameters
 * `manager`: Manager object. Must implement the `Manager` protocol. Matches `contextvars.ContextVar`.
 * `cls`: The class of the underlying variable accessed within the manager. Optional.
 * `getter`: A function that returns the underlying variable from the manager. Optional.
 * `setter`: A function that sets the underlying variable within the manager. Optional.
+
```

### Comparing `commonvars-0.2.7/PKG-INFO` & `commonvars-0.2.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,114 @@
-Metadata-Version: 2.1
-Name: commonvars
-Version: 0.2.7
-Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
-Home-page: https://github.com/bswck/commonvars
-Author: bswck
-Author-email: bswck.dev@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
-## `commonvars`
-
-A simple & straight-forward Python library for creating type-safe, context-dependent proxy objects.
-
-## Example
-
-The following example shows how to use `commonvars` with `contextvars`:
-
-```python
->>> from contextvars import ContextVar
->>> from commonvars import commonvar
-...
->>> count_var = ContextVar("count_var")
->>> count = commonvar(counter, int)
-...
->>> count
-<unbound 'int' object>
->>> count_var.set(0)
->>> count
-0
->>> count += 1
->>> count
-1
->>> count_var.get()
-1
->>> count -= 1
->>> count
-0
->>> count_var.set(1000)
-<Token var=<ContextVar name='count_var' at ...> at ...>
->>> count
-1000
-```
-
-## Ok, but what is this?
-
-`commonvars` is a Python module for creating context-dependent proxy objects.
-
-By 'proxy' we mean any object that forwards attribute access to another
-object. By 'context-dependent' we mean that the object to which the proxy
-forwards attribute access can change depending on the context in which the
-proxy is used.
-
-### Have you ever wondered how `flask.request` works?
-
-How is it possible
-that [`flask.request`](https://tedboy.github.io/flask/interface_api.incoming_request_data.html?highlight=request#flask.request)
-is different for each request, despite being a global variable?
-
-The answer is that `flask.request` is a such a proxy object as an instance of `werkzeug.local.LocalProxy`.
-For every request, `flask.request` forwards attribute access to a different `flask.Request` object.
-
-The functionality of `commonvars.commonvar()` (or, as you prefer, `commonvars.proxy()`) is a more generic version of `werkzeug.local.LocalProxy`.
-
-It takes a `Manager` object and the class of the object to which the proxy points.
-
-The `Manager` object must have `get` and `set` methods. The `get` method returns
-the object to which the would forward attribute access. The `set` method sets it, obviously.
-`set` is called when the proxy is being inplace modified, for example within the `+=` reassigning operator.
-The class parameter is optional, but it is strongly recommended for some corner-cases.
-The user might provide custom `getter` and `setter` functions that change the way 
-`Manager.get()` and `Manage.set()` are called.
-This might be useful when there is the need to keep track of the tokens
-returned by `ContextVar.set()`, if using `ContextVar` as the manager.
-
-## When would you use `commonvars`?
-
-You could use `commonvars` when...
-* ...writing a thread-safe application that operates on resources specific for separate threads.
-* ...improving code readability by avoiding passing around the same object to every function.
-* ...writing a web application that operates on resources specific per request.
-* ...writing an asynchronous application that operates on resources specific between tasks.
-* ...having any other case where you could use common variables that are context-dependent!
-
-## Installation
-
-### pip
-```bash
-$ pip install commonvars
-```
-
-### poetry
-
-You can add `commonvars` as a dependency with the following command:
-
-```bash
-$ poetry add commonvars
-```
-
-Or by directly specifying it in the configuration like so:
-
-```toml
-[tool.poetry.dependencies]
-"commonvars" = "^0.2.0"
-```
-
-Alternatively, you can add it directly from the source:
-
-```toml
-[tool.poetry.dependencies.commonvars]
-git = "https://github.com/bswck/commonvars.git"
-```
-
-## Documentation
-
-### `commonvars.commonvar(mgr, cls=None, getter=None, setter=None)`
-
-Creates a context-dependent proxy object.
-
-#### Parameters
-* `manager`: Manager object. Must implement the `Manager` protocol. Matches `contextvars.ContextVar`.
-* `cls`: The class of the underlying variable accessed within the manager. Optional.
-* `getter`: A function that returns the underlying variable from the manager. Optional.
-* `setter`: A function that sets the underlying variable within the manager. Optional.
-
+## `commonvars`
+
+A simple & straight-forward Python library for creating type-safe, context-dependent proxy objects.
+
+## Example
+
+The following example shows how to use `commonvars` with `contextvars`:
+
+```python
+>>> from contextvars import ContextVar
+>>> from commonvars import commonvar
+...
+>>> count_var = ContextVar("count_var")
+>>> count = commonvar(counter, int)
+...
+>>> count
+<unbound 'int' object>
+>>> count_var.set(0)
+>>> count
+0
+>>> count += 1
+>>> count
+1
+>>> count_var.get()
+1
+>>> count -= 1
+>>> count
+0
+>>> count_var.set(1000)
+<Token var=<ContextVar name='count_var' at ...> at ...>
+>>> count
+1000
+```
+
+## Ok, but what is this?
+
+`commonvars` is a Python module for creating context-dependent proxy objects.
+
+By 'proxy' we mean any object that forwards attribute access to another
+object. By 'context-dependent' we mean that the object to which the proxy
+forwards attribute access can change depending on the context in which the
+proxy is used.
+
+### Have you ever wondered how `flask.request` works?
+
+How is it possible
+that [`flask.request`](https://tedboy.github.io/flask/interface_api.incoming_request_data.html?highlight=request#flask.request)
+is different for each request, despite being a global variable?
+
+The answer is that `flask.request` is a such a proxy object as an instance of `werkzeug.local.LocalProxy`.
+For every request, `flask.request` forwards attribute access to a different `flask.Request` object.
+
+The functionality of `commonvars.commonvar()` (or, as you prefer, `commonvars.proxy()`) is a more generic version of `werkzeug.local.LocalProxy`.
+
+It takes a `Manager` object and the class of the object to which the proxy points.
+
+The `Manager` object must have `get` and `set` methods. The `get` method returns
+the object to which the would forward attribute access. The `set` method sets it, obviously.
+`set` is called when the proxy is being inplace modified, for example within the `+=` reassigning operator.
+The class parameter is optional, but it is strongly recommended for some corner-cases.
+The user might provide custom `getter` and `setter` functions that change the way 
+`Manager.get()` and `Manage.set()` are called.
+This might be useful when there is the need to keep track of the tokens
+returned by `ContextVar.set()`, if using `ContextVar` as the manager.
+
+## When would you use `commonvars`?
+
+You could use `commonvars` when...
+* ...writing a thread-safe application that operates on resources specific for separate threads.
+* ...improving code readability by avoiding passing around the same object to every function.
+* ...writing a web application that operates on resources specific per request.
+* ...writing an asynchronous application that operates on resources specific between tasks.
+* ...having any other case where you could use common variables that are context-dependent!
+
+## Installation
+
+### pip
+```bash
+$ pip install commonvars
+```
+
+### poetry
+
+You can add `commonvars` as a dependency with the following command:
+
+```bash
+$ poetry add commonvars
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+"commonvars" = "^0.2.0"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.commonvars]
+git = "https://github.com/bswck/commonvars.git"
+```
+
+## Documentation
+
+### `commonvars.commonvar(mgr, cls=None, getter=None, setter=None)`
+
+Creates a context-dependent proxy object.
+
+#### Parameters
+* `manager`: Manager object. Must implement the `Manager` protocol. Matches `contextvars.ContextVar`.
+* `cls`: The class of the underlying variable accessed within the manager. Optional.
+* `getter`: A function that returns the underlying variable from the manager. Optional.
+* `setter`: A function that sets the underlying variable within the manager. Optional.
```

