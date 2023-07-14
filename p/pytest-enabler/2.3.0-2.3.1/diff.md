# Comparing `tmp/pytest-enabler-2.3.0.tar.gz` & `tmp/pytest-enabler-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-enabler-2.3.0.tar", last modified: Fri Jul 14 01:07:17 2023, max compression
+gzip compressed data, was "pytest-enabler-2.3.1.tar", last modified: Fri Jul 14 01:34:33 2023, max compression
```

## Comparing `pytest-enabler-2.3.0.tar` & `pytest-enabler-2.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.683273 pytest-enabler-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.683273 pytest-enabler-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.687273 pytest-enabler-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.687273 pytest-enabler-2.3.0/pytest_enabler/
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pytest_enabler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pytest_enabler/default.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.687273 pytest-enabler-2.3.0/pytest_enabler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/tests/test_enabler.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.227943 pytest-enabler-2.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.227943 pytest-enabler-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/pytest_enabler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/pytest_enabler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/pytest_enabler/default.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/pytest_enabler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 01:34:33.000000 pytest-enabler-2.3.1/pytest_enabler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 01:34:33.000000 pytest-enabler-2.3.1/pytest_enabler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:34:33.000000 pytest-enabler-2.3.1/pytest_enabler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 01:34:33.000000 pytest-enabler-2.3.1/pytest_enabler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 01:34:33.000000 pytest-enabler-2.3.1/pytest_enabler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 01:34:33.000000 pytest-enabler-2.3.1/pytest_enabler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:34:33.231943 pytest-enabler-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/tests/test_enabler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 01:34:12.000000 pytest-enabler-2.3.1/tox.ini
```

### Comparing `pytest-enabler-2.3.0/.github/workflows/main.yml` & `pytest-enabler-2.3.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/LICENSE` & `pytest-enabler-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/NEWS.rst` & `pytest-enabler-2.3.1/NEWS.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.3.1
+======
+
+Bugfixes
+--------
+
+- Fix default config for ignore-flaky.
+
+
 v2.3.0
 ======
 
 Features
 --------
 
 - Added support for pytest-ignore-flaky.
```

### Comparing `pytest-enabler-2.3.0/PKG-INFO` & `pytest-enabler-2.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.3.0
+Version: 2.3.1
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -29,16 +29,16 @@
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
-..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/pytest-enabler/badge/?version=latest
+   :target: https://pytest-enabler.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 The ``enabler`` plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, the following config enables black to be enabled when present::
 
     [tool.pytest-enabler.black]
```

### Comparing `pytest-enabler-2.3.0/README.rst` & `pytest-enabler-2.3.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
-..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/pytest-enabler/badge/?version=latest
+   :target: https://pytest-enabler.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 The ``enabler`` plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, the following config enables black to be enabled when present::
 
     [tool.pytest-enabler.black]
```

### Comparing `pytest-enabler-2.3.0/docs/conf.py` & `pytest-enabler-2.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/pytest.ini` & `pytest-enabler-2.3.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/pytest_enabler/__init__.py` & `pytest-enabler-2.3.1/pytest_enabler/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/pytest_enabler.egg-info/PKG-INFO` & `pytest-enabler-2.3.1/pytest_enabler.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.3.0
+Version: 2.3.1
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -29,16 +29,16 @@
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
-..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/pytest-enabler/badge/?version=latest
+   :target: https://pytest-enabler.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 The ``enabler`` plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, the following config enables black to be enabled when present::
 
     [tool.pytest-enabler.black]
```

### Comparing `pytest-enabler-2.3.0/pytest_enabler.egg-info/SOURCES.txt` & `pytest-enabler-2.3.1/pytest_enabler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/setup.cfg` & `pytest-enabler-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/tests/test_enabler.py` & `pytest-enabler-2.3.1/tests/test_enabler.py`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.3.0/tox.ini` & `pytest-enabler-2.3.1/tox.ini`

 * *Files identical despite different names*

