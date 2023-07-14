# Comparing `tmp/labeva-2.1.0a1.dev1.tar.gz` & `tmp/labeva-2.1.0a2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeva-2.1.0a1.dev1.tar", max compression
+gzip compressed data, was "labeva-2.1.0a2.dev1.tar", max compression
```

## Comparing `labeva-2.1.0a1.dev1.tar` & `labeva-2.1.0a2.dev1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0    32473 2023-07-12 12:10:53.565183 labeva-2.1.0a1.dev1/LICENSE
--rwxr-xr-x   0        0        0     1148 2023-07-12 12:43:32.443584 labeva-2.1.0a1.dev1/README.md
--rwxr-xr-x   0        0        0     2693 2023-07-13 08:20:05.458878 labeva-2.1.0a1.dev1/pyproject.toml
--rwxr-xr-x   0        0        0      108 2023-07-13 07:25:23.426142 labeva-2.1.0a1.dev1/src/labeva/__init__.py
--rwxr-xr-x   0        0        0       25 2023-07-13 08:20:05.323059 labeva-2.1.0a1.dev1/src/labeva/__version__.py
--rwxr-xr-x   0        0        0      769 2023-07-13 07:26:23.238248 labeva-2.1.0a1.dev1/src/labeva/fit.py
--rwxr-xr-x   0        0        0      634 2023-07-13 07:22:35.922690 labeva-2.1.0a1.dev1/src/labeva/func.py
--rwxr-xr-x   0        0        0     2695 2023-07-13 07:22:35.932809 labeva-2.1.0a1.dev1/src/labeva/math.py
--rwxr-xr-x   0        0        0     2748 2023-07-13 07:22:35.947885 labeva-2.1.0a1.dev1/src/labeva/plot.py
--rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 labeva-2.1.0a1.dev1/PKG-INFO
+-rwxr-xr-x   0        0        0    32473 2023-07-14 05:45:23.392204 labeva-2.1.0a2.dev1/LICENSE
+-rwxr-xr-x   0        0        0     1248 2023-07-14 05:45:23.424469 labeva-2.1.0a2.dev1/README.md
+-rwxr-xr-x   0        0        0     2757 2023-07-14 06:41:04.643432 labeva-2.1.0a2.dev1/pyproject.toml
+-rwxr-xr-x   0        0        0      108 2023-07-14 05:45:23.732933 labeva-2.1.0a2.dev1/src/labeva/__init__.py
+-rwxr-xr-x   0        0        0       25 2023-07-14 06:41:04.531522 labeva-2.1.0a2.dev1/src/labeva/__version__.py
+-rwxr-xr-x   0        0        0     1295 2023-07-14 05:45:23.823030 labeva-2.1.0a2.dev1/src/labeva/fit.py
+-rwxr-xr-x   0        0        0     2130 2023-07-14 06:38:56.962991 labeva-2.1.0a2.dev1/src/labeva/func.py
+-rwxr-xr-x   0        0        0     3176 2023-07-14 05:45:23.924147 labeva-2.1.0a2.dev1/src/labeva/math.py
+-rwxr-xr-x   0        0        0     5769 2023-07-14 05:45:23.974761 labeva-2.1.0a2.dev1/src/labeva/plot.py
+-rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 labeva-2.1.0a2.dev1/PKG-INFO
```

### Comparing `labeva-2.1.0a1.dev1/LICENSE` & `labeva-2.1.0a2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `labeva-2.1.0a1.dev1/README.md` & `labeva-2.1.0a2.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # labeva
 
 <!-- badges-begin -->
-[![License: GNU General Public License v3 or later (GPLv3+)][license badge]][license gplv3]
+![Package version][package version badge]
 ![Python version][python version badge]
+[![License: GNU General Public License v3 or later (GPLv3+)][license badge]][license gplv3]
 
 [![Black codestyle][black badge]][black project]
 [![Conventional commits][conventional badge]][conventional commits]
 [![pre-commit enabled][pre-commit badge]][pre-commit project]
 
 [license badge]: https://badgen.net/static/license/GPLv3+/blue
 [license gplv3]: https://www.gnu.org/licenses/gpl-3.0.en.html
 
 [black badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black project]: https://github.com/psf/black
 
 [pre-commit badge]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit project]: https://pre-commit.com/
 
+[package version badge]: https://badgen.net/pypi/v/labeva
 [python version badge]: https://badgen.net/pypi/python/labeva
 
 [status badge]: https://badgen.net/badge/status/alpha/red
 
 [conventional badge]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [conventional commits]: https://www.conventionalcommits.org/en/v1.0.0/
```

### Comparing `labeva-2.1.0a1.dev1/pyproject.toml` & `labeva-2.1.0a2.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labeva"
-version = "2.1.0a1.dev1"
+version = "2.1.0a2.dev1"
 description = "ETs Laboratory Evaluation Suit"
 authors = ["Erik Thiel <erik.thiel@students.uni-mainz.de>"]
 license = "GPLv3+"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -18,42 +18,44 @@
 packages = [
     { from="src", include="labeva" }
 ]
 repository = "https://github.com/et15/labeva"
 documentation = "https://labeva.docs.et15.eu/"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.10,<3.13"
 numpy = ">=1.24.3"
 matplotlib = ">=3.7.1"
 scipy = ">=1.10.1"
-mkdocs-literate-nav = "^0.6.0"
-mkdocs-section-index = "^0.3.5"
-pre-commit = "^3.3.3"
 
 [tool.poetry.group.dev.dependencies]
 taskipy = ">=1.10.2"
+pre-commit = ">=3.3.3"
+pre-commit-hooks = ">=4.3.0"
 black = ">=22.10.0"
 coverage = ">=6.5.0"
+autoflake = ">=2.0.0"
 flake8-bugbear = ">=22.10.27"
 isort = ">=5.10.1"
 mypy = ">=0.990"
 pep8-naming = ">=0.13.2"
-pre-commit = ">=2.20.0"
-pre-commit-hooks = ">=4.3.0"
 pytest = ">=7.2.0"
 commitizen = ">=2.29.5"
+
+[tool.poetry.group.docs.dependencies]
 mkdocs-gen-files = ">=0.4.0"
 mkdocs-material = ">=8.3.9"
 mkdocstrings = { extras = ["crystal", "python"], version = ">=0.19.0" }
+mkdocs-literate-nav = "^0.6.0"
+mkdocs-section-index = "^0.3.5"
+python-markdown-math = "^0.8"
 pymdown-extensions = ">=9.5"
 Pygments = ">=2.12.0"
 mktestdocs = ">=0.2.0"
-autoflake = ">=2.0.0"
-
+mkdocs = "^1.4.3"
 
 [tool.taskipy.tasks]
 test = { cmd = "pytest src/tests", help = "Runs pytest on the codebase" }
 mypy = { cmd = "mypy src/labeva", help = "Runs static code anaylsis on the package" }
 format = { cmd = "isort src && black src" }
 docs-serve = { cmd = "mkdocs serve", help = "Serves the docs locally" }
 docs-regen = { cmd = "python docs/gen_ref_pages.py && git add docs", help = "Regenerates the automatic documentation" }
```

### Comparing `labeva-2.1.0a1.dev1/src/labeva/math.py` & `labeva-2.1.0a2.dev1/src/labeva/math.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,106 @@
+"""
+Tools for processing math data. Either numerical result, some kind of numpy object or rendered string.
+"""
+
 import numpy as np
 
 
 def magnitude(x: float) -> int:
     """
     calculate magnitude of given value
 
-    :param x: value
+    Args:
+        x (float): value
 
-    :return: magnitude
+    Returns:
+        Orders of magnitude in decimal system
     """
     return np.choose(
         x == 0,  # bool values, used as indices to the array
         [
             np.int_(np.log10(np.abs(x)) // 1),  # if false
             0,  # if true
-        ]
+        ],
     )
 
 
 def chisquare(y_exp, y_obs, y_obs_error) -> float:
     """
     calculate chi square value: (y_expected - y_observed)^2 / delta_y_observed^2
 
-    :param y_exp: expected y-values
-    :param y_obs: observed y-values
-    :param y_obs_error: uncertainties of observed y-values
+    Args:
+        y_exp: expected y-values
+        y_obs: observed y-values
+        y_obs_error: uncertainties of observed y-values
 
-    :return: chi square value
+    Returns:
+        chi square value
     """
     return sum(
         [
             (y_e - y) ** 2 / dy**2
             for y_e, y, dy in zip(y_exp, y_obs, y_obs_error, strict=True)
         ]
     )
 
 
 def average(series) -> (float, float):
     """
     calculate average and standard error of average
 
-    :param series: Series of values
-    :return: average, standard error of average
+    Args:
+        series: Series of values
+
+    Returns:
+        average, standard error of average
     """
     return np.average(series), np.std(series, ddof=1) / np.sqrt(len(series))
 
 
-def gaussian_fwhm(d, d_d):
-    return 2 * np.sqrt(2 * np.log(2)) * d, 2 * np.sqrt(2 * np.log(2)) * d_d
+def gaussian_fwhm(std: float, d_std: float) -> (float, float):
+    """
+    Calculate full width at half maximum of a gaussian.
+
+    Args:
+        std: standard derivation \\(\\sigma\\)
+        d_std: error of standard derivation
+
+    Returns:
+        FWHM of gaussian
+    """
+    return 2 * np.sqrt(2 * np.log(2)) * std, 2 * np.sqrt(2 * np.log(2)) * d_std
 
 
 def ls_minmax(data, num: int = 1000) -> np.ndarray:
     """
     returns linear spaced samples in the interval [min(data), max(data)] with length num=1000
 
-    :param data: series of data to gain min and max values
-    :param num: number of samples
+    Args:
+        data: series of data to gain min and max values
+        num: number of samples
 
-    :return: linear spaced samples
+    Returns:
+        linear spaced samples
     """
     return np.linspace(np.min(data), np.max(data), num)
 
 
-def error_str(value: float, error: float, frmt="plain", unit=None) -> str:
+def error_str(value: float, error: float, frmt: str = "plain", unit: str | None = None) -> str:
     """
     render value with uncertainty in string with right amount of decimal numbers in magnitude of value
 
-    :param value: value
-    :param error: uncertainty of value
-    :param frmt: format `plain`, `tex` or `si`
-    :param unit: print unit behind value
+    Args:
+        value: value
+        error: uncertainty of value
+        frmt: format `plain`, `tex` or `si`
+        unit: print unit behind value
 
-    :return: (value +- error)(e+-mag)
+    Returns:
+        (value +- error)(e+-mag)
     """
     # todo implement siunitx format
     if magnitude(error) > magnitude(value):
         return ""
     mag_val = magnitude(value)
     mag_err = magnitude(error)
     decimals = mag_val - mag_err + 1
```

### Comparing `labeva-2.1.0a1.dev1/PKG-INFO` & `labeva-2.1.0a2.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: labeva
-Version: 2.1.0a1.dev1
+Version: 2.1.0a2.dev1
 Summary: ETs Laboratory Evaluation Suit
 Home-page: https://github.com/et15/labeva
 License: GPLv3+
 Author: Erik Thiel
 Author-email: erik.thiel@students.uni-mainz.de
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: matplotlib (>=3.7.1)
-Requires-Dist: mkdocs-literate-nav (>=0.6.0,<0.7.0)
-Requires-Dist: mkdocs-section-index (>=0.3.5,<0.4.0)
 Requires-Dist: numpy (>=1.24.3)
-Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: scipy (>=1.10.1)
 Project-URL: Documentation, https://labeva.docs.et15.eu/
 Project-URL: Repository, https://github.com/et15/labeva
 Description-Content-Type: text/markdown
 
 # labeva
 
 <!-- badges-begin -->
-[![License: GNU General Public License v3 or later (GPLv3+)][license badge]][license gplv3]
+![Package version][package version badge]
 ![Python version][python version badge]
+[![License: GNU General Public License v3 or later (GPLv3+)][license badge]][license gplv3]
 
 [![Black codestyle][black badge]][black project]
 [![Conventional commits][conventional badge]][conventional commits]
 [![pre-commit enabled][pre-commit badge]][pre-commit project]
 
 [license badge]: https://badgen.net/static/license/GPLv3+/blue
 [license gplv3]: https://www.gnu.org/licenses/gpl-3.0.en.html
 
 [black badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black project]: https://github.com/psf/black
 
 [pre-commit badge]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit project]: https://pre-commit.com/
 
+[package version badge]: https://badgen.net/pypi/v/labeva
 [python version badge]: https://badgen.net/pypi/python/labeva
 
 [status badge]: https://badgen.net/badge/status/alpha/red
 
 [conventional badge]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [conventional commits]: https://www.conventionalcommits.org/en/v1.0.0/
```

