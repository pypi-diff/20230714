# Comparing `tmp/fgen-0.1.0.tar.gz` & `tmp/fgen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgen-0.1.0.tar", max compression
+gzip compressed data, was "fgen-0.1.1.tar", max compression
```

## Comparing `fgen-0.1.0.tar` & `fgen-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1461 2023-07-03 02:33:16.651031 fgen-0.1.0/LICENSE
--rw-r--r--   0        0        0     2076 2023-07-03 02:33:12.941248 fgen-0.1.0/README.md
--rw-r--r--   0        0        0     4209 2023-07-03 02:33:35.218283 fgen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      316 2023-06-29 03:48:37.247779 fgen-0.1.0/src/fgen/__init__.py
--rw-r--r--   0        0        0      103 2023-06-28 22:47:57.266486 fgen-0.1.0/src/fgen/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-29 01:38:35.033149 fgen-0.1.0/src/fgen/commands/base.py
--rw-r--r--   0        0        0     2450 2023-07-02 23:31:07.192648 fgen-0.1.0/src/fgen/commands/generate.py
--rw-r--r--   0        0        0     4619 2023-07-02 23:31:07.192921 fgen-0.1.0/src/fgen/fortran_parsing.py
--rw-r--r--   0        0        0      165 2023-06-29 03:34:31.992495 fgen-0.1.0/src/fgen/main.py
--rw-r--r--   0        0        0        0 2023-06-28 22:47:57.265091 fgen-0.1.0/src/fgen/py.typed
--rw-r--r--   0        0        0    11265 2023-07-03 01:49:08.795131 fgen-0.1.0/src/fgen/schema.py
--rw-r--r--   0        0        0     2119 2023-06-29 04:20:42.459486 fgen-0.1.0/src/fgen/templates/calculator_manager.f90.jinja
--rw-r--r--   0        0        0     3798 2023-07-03 02:33:12.944051 fgen-0.1.0/src/fgen/templates/python_module.py.jinja
--rw-r--r--   0        0        0     3937 2023-06-29 04:19:25.604177 fgen-0.1.0/src/fgen/templates/wrap_module.f90.jinja
--rw-r--r--   0        0        0     4889 2023-07-02 23:31:07.193510 fgen-0.1.0/src/fgen/templator.py
--rw-r--r--   0        0        0      111 2023-06-29 01:42:36.614821 fgen-0.1.0/src/fgen_runtime/__init__.py
--rw-r--r--   0        0        0     4414 2023-06-29 01:54:52.429035 fgen-0.1.0/src/fgen_runtime/base.py
--rw-r--r--   0        0        0      130 2023-06-27 08:08:59.037550 fgen-0.1.0/src/fgen_runtime/common.py
--rw-r--r--   0        0        0      543 2023-06-27 23:39:28.839213 fgen-0.1.0/src/fgen_runtime/exceptions.py
--rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 fgen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-07-14 04:41:25.452781 fgen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2094 2023-07-14 04:41:25.452781 fgen-0.1.1/README.md
+-rw-r--r--   0        0        0     5211 2023-07-14 04:41:25.454781 fgen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      316 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/commands/base.py
+-rw-r--r--   0        0        0     2450 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/commands/generate.py
+-rw-r--r--   0        0        0     4619 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/fortran_parsing.py
+-rw-r--r--   0        0        0      165 2023-07-14 04:41:25.454781 fgen-0.1.1/src/fgen/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 04:41:25.481781 fgen-0.1.1/src/fgen/py.typed
+-rw-r--r--   0        0        0    11287 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/schema.py
+-rw-r--r--   0        0        0     2119 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templates/calculator_manager.f90.jinja
+-rw-r--r--   0        0        0     3798 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templates/python_module.py.jinja
+-rw-r--r--   0        0        0     3937 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templates/wrap_module.f90.jinja
+-rw-r--r--   0        0        0     4889 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen/templator.py
+-rw-r--r--   0        0        0      111 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/__init__.py
+-rw-r--r--   0        0        0     4414 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/base.py
+-rw-r--r--   0        0        0      130 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/common.py
+-rw-r--r--   0        0        0      543 2023-07-14 04:41:25.455781 fgen-0.1.1/src/fgen_runtime/exceptions.py
+-rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 fgen-0.1.1/PKG-INFO
```

### Comparing `fgen-0.1.0/LICENSE` & `fgen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/README.md` & `fgen-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 * libfgen
 
 <!--- sec-end-description -->
 
 Full documentation can be found at:
 [fgen.readthedocs.io](https://fgen.readthedocs.io/en/latest/).
 We recommend reading the docs there because the internal documentation links
-don't render correctly on GitLab's viewer.
+don't render correctly on GitLab's viewer. TODO: Create docs
 
 ## Installation
 
 <!--- sec-begin-installation -->
 
 Fortran-Python wrapper can be installed with conda or pip:
```

### Comparing `fgen-0.1.0/pyproject.toml` & `fgen-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgen"
-version = "0.1.0"
+version = "0.1.1"
 description = "Automatically generate wrapper to integrate Fortran and Python"
 authors = ["Jared Lewis <jared.lewis@climate-energy-college.org>"]
 readme = "README.md"
 packages = [
     {include = "fgen", from = "src"},
     {include = "fgen_runtime", from = "src"},
 ]
@@ -14,63 +14,57 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering"
 ]
 homepage = "https://gitlab.com/magicc/fgen"
 
-[tool.commitizen]
-version = "0.1.0"
-version_files = ["pyproject.toml:^version"]
-tag_format = "v$version"
-major_version_zero = true
-
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 cattrs = "^23.0.0"
 attrs = "^23.0.0"
 openscm-units = "^0.5.0"
 click = "^8.0.0"
 pyyaml = "^6.0"
 black = "^23.3.0"
 jinja2 = "^3.1.2"
 
-
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
 pytest-xdist = "^3.3.1"
+[tool.poetry.group.test.dependencies]
+pytest-regressions = "^2.4.2"
 
 [tool.poetry.group.docs.dependencies]
 myst-nb = "^0.17.0"
 sphinx-rtd-theme = "^1.2.0"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-autodocgen = "^1.3"
 jupytext = "^1.14.5"
 sphinx-copybutton = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.0.0"
 coverage = "^7.2.0"
 black = "23.3.0"
 blackdoc = "0.3.8"
-commitizen = "^3.1.1"
 mypy = "^1.2.0"
 ruff = "0.0.264"
 pre-commit = "^3.3.1"
+towncrier = "^23.6.0"
 cmake = "^3.26.4"
-
-
-[tool.poetry.group.test.dependencies]
-pytest-regressions = "^2.4.2"
+# Temporary fix until next towncrier release
+importlib-resources = {"version" = "<6", python = "<=3.9" }
 
 [tool.poetry.scripts]
 fgen = 'fgen.main:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -134,14 +128,15 @@
     "PD002",  # Disable autofix for inplace as this often introduces bugs
 ]
 ignore = [
     "D200",  # One-line docstring should fit on one line with quotes
     "D400",  # First line should end with a period
     "D105",  # Missing docstring in magic method
     "TRY003",  # Avoid specifying long messages outside the exception class
+    "UP007",
 ]
 # Provide some leeway for long docstring, this is otherwise handled by black
 line-length = 110
 
 [tool.ruff.per-file-ignores]
 "test*.py" = [
     "D",  # Documentation not needed in tests
@@ -161,7 +156,51 @@
 ]
 
 [tool.ruff.isort]
 known-first-party = ["src"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
+
+[tool.towncrier]
+package = "fgen"
+package_dir = "src"
+filename = "docs/source/changelog.md"
+directory = "changelog/"
+title_format = "## fgen {version} ({project_date})"
+underlines = ["", "", ""]
+issue_format = "[#{issue}](https://gitlab.com/magicc/fgen/-/merge_requests/{issue})"
+
+  [[tool.towncrier.type]]
+  directory = "breaking"
+  name = "Breaking Changes"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "deprecation"
+  name = "Deprecations"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "feature"
+  name = "Features"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "improvement"
+  name = "Improvements"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "fix"
+  name = "Bug Fixes"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "docs"
+  name = "Improved Documentation"
+  showcontent = true
+
+  [[tool.towncrier.type]]
+  directory = "trivial"
+  name = "Trivial/Internal Changes"
+  showcontent = false
```

### Comparing `fgen-0.1.0/src/fgen/commands/generate.py` & `fgen-0.1.1/src/fgen/commands/generate.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen/fortran_parsing.py` & `fgen-0.1.1/src/fgen/fortran_parsing.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen/schema.py` & `fgen-0.1.1/src/fgen/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Configuration schema
 
 This schema is used to serialize and validate the YAML configuration files.
 """
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING, Optional, TypeVar
 
 from attrs import define, field, fields, validators
 from cattrs.preconf.pyyaml import make_converter
 
 from .fortran_parsing import (
     DIMENSION_REGEX,
     KNOWN_FORTRAN_TYPES,
@@ -104,15 +104,15 @@
     """
 
     name: str
     description: str
     unit: str
     type: str = field(validator=[validators.instance_of(str), fortran_type_validator])
     expose_to_python: bool = True
-    truncated_name: str | None = None
+    truncated_name: Optional[str] = None
 
     def python_type(self) -> type:
         """
         Determine the equivalent type for Python
 
         Raises
         ------
@@ -230,15 +230,15 @@
 
     This
     """
 
     name: str
     description: str
     parameters: dict[str, ValueDefinition]
-    returns: ValueDefinition | None
+    returns: Optional[ValueDefinition]
 
     def units(self) -> dict[str, str]:
         """
         Units used in the method
 
         Includes units from of the parameters and the return value.
 
@@ -311,15 +311,15 @@
             Inconsistent units were found
 
         Returns
         -------
             Dictionary containing value names' as keys and the associated units
             as values.
         """
-        res: dict[str, tuple[str | None, str]] = {
+        res: dict[str, tuple[Optional[str], str]] = {
             key: (None, attr.unit) for key, attr in self.attributes.items()
         }
 
         for name, method in self.methods.items():
             method_units = method.units()
 
             for k, v in method_units.items():
@@ -350,15 +350,15 @@
     TODO: document concepts
     """
 
     name: str
     description: str
     provides: CalculatorDefinition
     prefix: str = "mod_"
-    truncated_name: str | None = None
+    truncated_name: Optional[str] = None
 
     @property
     def wrapper_module_name(self) -> str:
         """
         Name for the Fortran wrapper module
 
         By default the module name is derived from the :attr:`name`, but in
```

### Comparing `fgen-0.1.0/src/fgen/templates/calculator_manager.f90.jinja` & `fgen-0.1.1/src/fgen/templates/calculator_manager.f90.jinja`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen/templates/python_module.py.jinja` & `fgen-0.1.1/src/fgen/templates/python_module.py.jinja`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen/templates/wrap_module.f90.jinja` & `fgen-0.1.1/src/fgen/templates/wrap_module.f90.jinja`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen/templator.py` & `fgen-0.1.1/src/fgen/templator.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen_runtime/base.py` & `fgen-0.1.1/src/fgen_runtime/base.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/src/fgen_runtime/exceptions.py` & `fgen-0.1.1/src/fgen_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `fgen-0.1.0/PKG-INFO` & `fgen-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: fgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically generate wrapper to integrate Fortran and Python
 Home-page: https://gitlab.com/magicc/fgen
 License: BSD-3-Clause
 Keywords: fortran
 Author: Jared Lewis
 Author-email: jared.lewis@climate-energy-college.org
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: attrs (>=23.0.0,<24.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: cattrs (>=23.0.0,<24.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
@@ -49,15 +47,15 @@
 * libfgen
 
 <!--- sec-end-description -->
 
 Full documentation can be found at:
 [fgen.readthedocs.io](https://fgen.readthedocs.io/en/latest/).
 We recommend reading the docs there because the internal documentation links
-don't render correctly on GitLab's viewer.
+don't render correctly on GitLab's viewer. TODO: Create docs
 
 ## Installation
 
 <!--- sec-begin-installation -->
 
 Fortran-Python wrapper can be installed with conda or pip:
```

