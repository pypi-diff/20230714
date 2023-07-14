# Comparing `tmp/autora-theorist-bms-1.0.2.tar.gz` & `tmp/autora-theorist-bms-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bms-1.0.2.tar", last modified: Tue Jul 11 16:15:39 2023, max compression
+gzip compressed data, was "autora-theorist-bms-1.0.3.tar", last modified: Fri Jul 14 12:40:32 2023, max compression
```

## Comparing `autora-theorist-bms-1.0.2.tar` & `autora-theorist-bms-1.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    34190 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/how-it-works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/img/BMSEquationTreeOps.png
--rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/img/BMSTempering.png
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/meta-parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/docs/search-space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.363938 autora-theorist-bms-1.0.2/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/src/autora/theorist/bms/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/fit_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    60697 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2124 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/src/autora/theorist/bms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:15:39.000000 autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:39.367938 autora-theorist-bms-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-11 16:15:28.000000 autora-theorist-bms-1.0.2/tests/test_sklearn_bms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.617390 autora-theorist-bms-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.617390 autora-theorist-bms-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.617390 autora-theorist-bms-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34190 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/how-it-works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/img/BMSEquationTreeOps.png
+-rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/img/BMSTempering.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/meta-parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/docs/search-space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.617390 autora-theorist-bms-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.617390 autora-theorist-bms-1.0.3/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.617390 autora-theorist-bms-1.0.3/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/src/autora/theorist/bms/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/fit_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60697 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2124 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/src/autora/theorist/bms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 12:40:32.000000 autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-14 12:40:32.000000 autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:40:32.000000 autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 12:40:32.000000 autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 12:40:32.000000 autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:32.621390 autora-theorist-bms-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-14 12:40:22.000000 autora-theorist-bms-1.0.3/tests/test_sklearn_bms.py
```

### Comparing `autora-theorist-bms-1.0.2/.github/workflows/python-publish.yml` & `autora-theorist-bms-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/.gitignore` & `autora-theorist-bms-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/.pre-commit-config.yaml` & `autora-theorist-bms-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/PKG-INFO` & `autora-theorist-bms-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bms
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian Machine Scientist theorist for AutoRA
 Author-email: Joshua Hewson <joshua_hewson@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bms
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-bms-1.0.2/README.md` & `autora-theorist-bms-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/Basic Usage.ipynb` & `autora-theorist-bms-1.0.3/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/how-it-works.md` & `autora-theorist-bms-1.0.3/docs/how-it-works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/img/BMSEquationTreeOps.png` & `autora-theorist-bms-1.0.3/docs/img/BMSEquationTreeOps.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/img/BMSTempering.png` & `autora-theorist-bms-1.0.3/docs/img/BMSTempering.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/index.md` & `autora-theorist-bms-1.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/meta-parameters.md` & `autora-theorist-bms-1.0.3/docs/meta-parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/docs/search-space.md` & `autora-theorist-bms-1.0.3/docs/search-space.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/mkdocs/base.yml` & `autora-theorist-bms-1.0.3/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/pyproject.toml` & `autora-theorist-bms-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/src/autora/theorist/bms/fit_prior.py` & `autora-theorist-bms-1.0.3/src/autora/theorist/bms/fit_prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/src/autora/theorist/bms/mcmc.py` & `autora-theorist-bms-1.0.3/src/autora/theorist/bms/mcmc.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/src/autora/theorist/bms/parallel.py` & `autora-theorist-bms-1.0.3/src/autora/theorist/bms/parallel.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/src/autora/theorist/bms/prior.py` & `autora-theorist-bms-1.0.3/src/autora/theorist/bms/prior.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,16 @@
             "Nopi_sqrt": 4.760686909134266,
             "Nopi_cos": 5.452564657261127,
             "Nopi_sinh": 7.955723540761046,
             "Nopi_abs": 6.333544134938385,
             "Nopi_+": 5.808163661224514,
             "Nopi_*": 5.002213595420244,
             "Nopi_fac": 10.0,
-            "Nopi2_*": 1.0,
-            "Nopi_sig": 1.0,  # arbitrarily set for now
-            "Nopi_relu": 1.0,  # arbitrarily set for now
+            "Nopi_sig": 10.0,  # arbitrarily set for now
+            "Nopi_relu": 10.0,  # arbitrarily set for now
         },
     }
     assert prior_dict[prior_name] is not None, "prior key not recognized"
     return prior_dict[prior_name]
 
 
 def __get_ops():
```

### Comparing `autora-theorist-bms-1.0.2/src/autora/theorist/bms/regressor.py` & `autora-theorist-bms-1.0.3/src/autora/theorist/bms/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/src/autora/theorist/bms/utils.py` & `autora-theorist-bms-1.0.3/src/autora/theorist/bms/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/PKG-INFO` & `autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bms
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian Machine Scientist theorist for AutoRA
 Author-email: Joshua Hewson <joshua_hewson@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bms
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-bms-1.0.2/src/autora_theorist_bms.egg-info/SOURCES.txt` & `autora-theorist-bms-1.0.3/src/autora_theorist_bms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/tests/README.md` & `autora-theorist-bms-1.0.3/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.2/tests/test_sklearn_bms.py` & `autora-theorist-bms-1.0.3/tests/test_sklearn_bms.py`

 * *Files identical despite different names*

