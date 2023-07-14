# Comparing `tmp/aztools-0.2.tar.gz` & `tmp/aztools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aztools-0.2.tar", last modified: Fri Jul 14 11:51:53 2023, max compression
+gzip compressed data, was "aztools-0.2.1.tar", last modified: Fri Jul 14 16:51:01 2023, max compression
```

## Comparing `aztools-0.2.tar` & `aztools-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.202162 aztools-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 11:51:38.000000 aztools-0.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.194162 aztools-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-14 11:51:38.000000 aztools-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-14 11:51:38.000000 aztools-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 11:51:38.000000 aztools-0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 11:51:38.000000 aztools-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-14 11:51:53.202162 aztools-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-14 11:51:38.000000 aztools-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 11:51:38.000000 aztools-0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-14 11:51:38.000000 aztools-0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 11:51:38.000000 aztools-0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 11:51:38.000000 aztools-0.2/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-14 11:51:38.000000 aztools-0.2/docs/notebooks/intro_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 11:51:38.000000 aztools-0.2/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 11:51:38.000000 aztools-0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-14 11:51:38.000000 aztools-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:51:53.202162 aztools-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-07-14 11:51:38.000000 aztools-0.2/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/aztools/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26716 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/lcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/simlc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/aztools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-14 11:51:38.000000 aztools-0.2/src/scripts/ogrppha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/simulations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11896 2023-07-14 11:51:38.000000 aztools-0.2/src/simulations/sim__bin_psd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5040 2023-07-14 11:51:38.000000 aztools-0.2/src/simulations/sim__calculate_psd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10842 2023-07-14 11:51:38.000000 aztools-0.2/src/simulations/sim__phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-14 11:51:38.000000 aztools-0.2/tests/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.202162 aztools-0.2/tests/aztools/
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-14 11:51:38.000000 aztools-0.2/tests/aztools/test_lcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-14 11:51:38.000000 aztools-0.2/tests/aztools/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-14 11:51:38.000000 aztools-0.2/tests/aztools/test_simlc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 16:50:41.000000 aztools-0.2.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.686144 aztools-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.686144 aztools-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-14 16:50:41.000000 aztools-0.2.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 16:50:41.000000 aztools-0.2.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 16:50:41.000000 aztools-0.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 16:50:41.000000 aztools-0.2.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 16:50:41.000000 aztools-0.2.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-14 16:50:41.000000 aztools-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-14 16:50:41.000000 aztools-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 16:50:41.000000 aztools-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 16:50:41.000000 aztools-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-14 16:51:01.690144 aztools-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-14 16:50:41.000000 aztools-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.686144 aztools-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 16:50:41.000000 aztools-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-14 16:50:41.000000 aztools-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-14 16:50:41.000000 aztools-0.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.686144 aztools-0.2.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-14 16:50:41.000000 aztools-0.2.1/docs/notebooks/intro_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 16:50:41.000000 aztools-0.2.1/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 16:50:41.000000 aztools-0.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-14 16:50:41.000000 aztools-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:51:01.690144 aztools-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.686144 aztools-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-07-14 16:50:41.000000 aztools-0.2.1/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/src/aztools/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 16:50:41.000000 aztools-0.2.1/src/aztools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-14 16:50:41.000000 aztools-0.2.1/src/aztools/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26716 2023-07-14 16:50:41.000000 aztools-0.2.1/src/aztools/lcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-07-14 16:50:41.000000 aztools-0.2.1/src/aztools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-07-14 16:50:41.000000 aztools-0.2.1/src/aztools/simlc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/src/aztools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 16:51:01.000000 aztools-0.2.1/src/aztools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-14 16:50:41.000000 aztools-0.2.1/src/scripts/ogrppha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/src/simulations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11896 2023-07-14 16:50:41.000000 aztools-0.2.1/src/simulations/sim__bin_psd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5040 2023-07-14 16:50:41.000000 aztools-0.2.1/src/simulations/sim__calculate_psd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10842 2023-07-14 16:50:41.000000 aztools-0.2.1/src/simulations/sim__phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-14 16:50:41.000000 aztools-0.2.1/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:51:01.690144 aztools-0.2.1/tests/aztools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-14 16:50:41.000000 aztools-0.2.1/tests/aztools/test_lcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-14 16:50:41.000000 aztools-0.2.1/tests/aztools/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-14 16:50:41.000000 aztools-0.2.1/tests/aztools/test_simlc.py
```

### Comparing `aztools-0.2/.github/workflows/build-documentation.yml` & `aztools-0.2.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `aztools-0.2/.github/workflows/linting.yml` & `aztools-0.2.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `aztools-0.2/.github/workflows/publish-to-pypi.yml` & `aztools-0.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `aztools-0.2/.github/workflows/smoke-test.yml` & `aztools-0.2.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `aztools-0.2/.github/workflows/testing-and-coverage.yml` & `aztools-0.2.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `aztools-0.2/.gitignore` & `aztools-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aztools-0.2/.pre-commit-config.yaml` & `aztools-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aztools-0.2/LICENSE` & `aztools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aztools-0.2/docs/Makefile` & `aztools-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aztools-0.2/docs/conf.py` & `aztools-0.2.1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
 extensions = ["sphinx.ext.mathjax", "sphinx.ext.napoleon", "sphinx.ext.viewcode"]
 
 extensions.append("autoapi.extension")
 extensions.append("nbsphinx")
 
 templates_path = []
-exclude_patterns = ['_build', '**.ipynb_checkpoints']
+exclude_patterns = ['_build', '**.ipynb_checkpoints',]
 
 master_doc = "index"  # This assumes that sphinx-build is called from the root directory
 html_show_sourcelink = False  # Remove 'view source code' from top of page (for html, not python)
 add_module_names = False # Remove namespaces from class/method signatures
 
 autoapi_type = "python"
 autoapi_dirs = ["../src"]
-autoapi_ignore = ["*/__main__.py", "*/_version.py"]
+autoapi_ignore = ["*/__main__.py", "*/_version.py", "*/sim__*py", "*/.ipynb_checkpoints"]
 autoapi_add_toc_tree_entry = False
 autoapi_member_order = "bysource"
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `aztools-0.2/pyproject.toml` & `aztools-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,10 @@
     "setuptools>=45", # Used to build and package the Python project
     "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/aztools/_version.py"
+
+[project.scripts]
+ogrppha = "scripts.ogrppha:main"
```

### Comparing `aztools-0.2/src/.pylintrc` & `aztools-0.2.1/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/aztools/data.py` & `aztools-0.2.1/src/aztools/data.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/aztools/lcurve.py` & `aztools-0.2.1/src/aztools/lcurve.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/aztools/misc.py` & `aztools-0.2.1/src/aztools/misc.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/aztools/simlc.py` & `aztools-0.2.1/src/aztools/simlc.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/aztools.egg-info/SOURCES.txt` & `aztools-0.2.1/src/aztools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/notebooks.rst
 docs/requirements.txt
-docs/notebooks/README.md
 docs/notebooks/intro_notebook.ipynb
 src/.pylintrc
 src/aztools/__init__.py
 src/aztools/_version.py
 src/aztools/data.py
 src/aztools/lcurve.py
 src/aztools/misc.py
 src/aztools/simlc.py
 src/aztools.egg-info/PKG-INFO
 src/aztools.egg-info/SOURCES.txt
 src/aztools.egg-info/dependency_links.txt
+src/aztools.egg-info/entry_points.txt
 src/aztools.egg-info/requires.txt
 src/aztools.egg-info/top_level.txt
 src/scripts/ogrppha.py
 src/simulations/sim__bin_psd.py
 src/simulations/sim__calculate_psd.py
 src/simulations/sim__phase.py
 tests/.pylintrc
```

### Comparing `aztools-0.2/src/scripts/ogrppha.py` & `aztools-0.2.1/src/scripts/ogrppha.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/simulations/sim__bin_psd.py` & `aztools-0.2.1/src/simulations/sim__bin_psd.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/simulations/sim__calculate_psd.py` & `aztools-0.2.1/src/simulations/sim__calculate_psd.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/src/simulations/sim__phase.py` & `aztools-0.2.1/src/simulations/sim__phase.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/tests/.pylintrc` & `aztools-0.2.1/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `aztools-0.2/tests/aztools/test_lcurve.py` & `aztools-0.2.1/tests/aztools/test_lcurve.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/tests/aztools/test_misc.py` & `aztools-0.2.1/tests/aztools/test_misc.py`

 * *Files identical despite different names*

### Comparing `aztools-0.2/tests/aztools/test_simlc.py` & `aztools-0.2.1/tests/aztools/test_simlc.py`

 * *Files identical despite different names*

