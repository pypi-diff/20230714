# Comparing `tmp/stepcount-2.1.6.tar.gz` & `tmp/stepcount-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-2.1.6.tar", last modified: Tue Jun 27 18:26:16 2023, max compression
+gzip compressed data, was "stepcount-2.2.0.tar", last modified: Fri Jul 14 17:14:29 2023, max compression
```

## Comparing `stepcount-2.1.6.tar` & `stepcount-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-27 18:26:06.000000 stepcount-2.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-27 18:26:16.508912 stepcount-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-27 18:26:06.000000 stepcount-2.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-27 18:26:06.000000 stepcount-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:26:16.508912 stepcount-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-27 18:26:06.000000 stepcount-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.504912 stepcount-2.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21831 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-27 18:26:06.000000 stepcount-2.1.6/src/stepcount/utils/collate_outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:26:16.508912 stepcount-2.1.6/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 18:26:16.000000 stepcount-2.1.6/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-27 18:26:06.000000 stepcount-2.1.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:14:29.610920 stepcount-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-14 17:14:14.000000 stepcount-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-14 17:14:29.610920 stepcount-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-14 17:14:14.000000 stepcount-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-14 17:14:14.000000 stepcount-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:14:29.610920 stepcount-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-14 17:14:14.000000 stepcount-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:14:29.606920 stepcount-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:14:29.610920 stepcount-2.2.0/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 17:14:29.610920 stepcount-2.2.0/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21853 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:14:29.610920 stepcount-2.2.0/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-14 17:14:14.000000 stepcount-2.2.0/src/stepcount/utils/collate_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:14:29.610920 stepcount-2.2.0/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-14 17:14:29.000000 stepcount-2.2.0/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-14 17:14:29.000000 stepcount-2.2.0/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:14:29.000000 stepcount-2.2.0/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 17:14:29.000000 stepcount-2.2.0/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 17:14:29.000000 stepcount-2.2.0/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:14:29.000000 stepcount-2.2.0/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-14 17:14:14.000000 stepcount-2.2.0/versioneer.py
```

### Comparing `stepcount-2.1.6/LICENSE.md` & `stepcount-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/PKG-INFO` & `stepcount-2.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.6
+Version: 2.2.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -21,58 +21,38 @@
 
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
 
-Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
-
-## Getting started
+## Install
 
-### Prerequisite
+We recommend using **Anaconda**:
 
-- Python 3.8 or greater
+1. Download & install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda).
+1. (Windows) Once installed, launch the **Anaconda Prompt**.
+1. Create a virtual environment:
     ```console
-    $ python --version  # or python3 --version
+    $ conda create -n stepcount python=3.9 openjdk pip
     ```
-
-- Java 8 (1.8.0) or greater
+    This creates a virtual environment called `stepcount` with Python version 3.9, OpenJDK, and Pip.
+1. Activate the environment:
     ```console
-    $ java -version
+    $ conda activate stepcount
+    ```
+    You should now see `(stepcount)` written in front of your prompt.
+1. Install `stepcount`:
+    ```console
+    $ pip install stepcount
     ```
 
-### Install (Windows)
-For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
-
-1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
-2. Install. Use the default recommended settings.
-3. From the Start menu, search and open the **Anaconda Prompt**.
-
-```console
-$ pip install stepcount
-```
-
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda-on-windows.md).
-
-### Install (Linux)
-
-<!-- ```console
-$ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-<!-- ```console
-$ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-```console
-$ pip install stepcount
-```
-
+You are all set! The next time that you want to use `stepcount`, open the Anaconda Prompt and activate the environment (step 4). If you see `(stepcount)` in front of your prompt, you are ready to go!
 
+Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
 
 ## Usage
 
 ```bash
 # Process an AX3 file
 $ stepcount sample.cwa
 
@@ -113,14 +93,20 @@
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
 
+### Troubleshooting 
+Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
+```console
+$ conda install -n stepcount openjdk=8
+```
+
 ### Output files
 By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
 
 ```console
 $ stepcount sample.cwa -o /path/to/some/folder/
 ```
```

### Comparing `stepcount-2.1.6/README.md` & `stepcount-2.2.0/src/stepcount.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,58 @@
+Metadata-Version: 2.1
+Name: stepcount
+Version: 2.2.0
+Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
+Home-page: https://github.com/OxWearables/stepcount
+Download-URL: https://github.com/OxWearables/stepcount
+Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
+Maintainer: Shing Chan
+Maintainer-email: shing.chan@ndph.ox.ac.uk
+License: See LICENSE file.
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Requires-Python: >=3.8, <3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE.md
+
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
 
-Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
-
-## Getting started
+## Install
 
-### Prerequisite
+We recommend using **Anaconda**:
 
-- Python 3.8 or greater
+1. Download & install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda).
+1. (Windows) Once installed, launch the **Anaconda Prompt**.
+1. Create a virtual environment:
     ```console
-    $ python --version  # or python3 --version
+    $ conda create -n stepcount python=3.9 openjdk pip
     ```
-
-- Java 8 (1.8.0) or greater
+    This creates a virtual environment called `stepcount` with Python version 3.9, OpenJDK, and Pip.
+1. Activate the environment:
     ```console
-    $ java -version
+    $ conda activate stepcount
+    ```
+    You should now see `(stepcount)` written in front of your prompt.
+1. Install `stepcount`:
+    ```console
+    $ pip install stepcount
     ```
 
-### Install (Windows)
-For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
-
-1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
-2. Install. Use the default recommended settings.
-3. From the Start menu, search and open the **Anaconda Prompt**.
-
-```console
-$ pip install stepcount
-```
-
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda-on-windows.md).
-
-### Install (Linux)
-
-<!-- ```console
-$ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-<!-- ```console
-$ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-```console
-$ pip install stepcount
-```
-
+You are all set! The next time that you want to use `stepcount`, open the Anaconda Prompt and activate the environment (step 4). If you see `(stepcount)` in front of your prompt, you are ready to go!
 
+Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
 
 ## Usage
 
 ```bash
 # Process an AX3 file
 $ stepcount sample.cwa
 
@@ -92,14 +93,20 @@
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
 
+### Troubleshooting 
+Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
+```console
+$ conda install -n stepcount openjdk=8
+```
+
 ### Output files
 By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
 
 ```console
 $ stepcount sample.cwa -o /path/to/some/folder/
 ```
```

### Comparing `stepcount-2.1.6/pyproject.toml` & `stepcount-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/setup.py` & `stepcount-2.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         "dev": [
             "flake8",
             "autopep8",
             "ipython",
             "ipdb",
             "twine",
             "tomli",
+            "jupyter",
+            "matplotlib",
         ],
         "docs": [
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "sphinxcontrib-programoutput>=0.17",
             "docutils<0.18",
```

### Comparing `stepcount-2.1.6/src/stepcount/__init__.py` & `stepcount-2.2.0/src/stepcount/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 __author__ = "Shing Chan, Scott Small, Gert Mertes, Aiden Doherty"
 __email__ = "shing.chan@ndph.ox.ac.uk, scott.small@ndph.ox.ac.uk, gert.mertes@ndph.ox.ac.uk, aiden.doherty@ndph.ox.ac.uk"
 __maintainer__ = "Shing Chan"
 __maintainer_email__ = "shing.chan@ndph.ox.ac.uk"
 __license__ = "See LICENSE file."
 
 __model_version__ = {
-    "rf": "20230210",
+    "rf": "20230713",
     "ssl": "ssl-20230208"
 }
 __model_md5__ = {
-    "rf": "8d803d175b792fff12f93ca37fbc9271",
+    "rf": "9a6ef63ca4d651c937c18b25d5af4e72",
     "ssl": "eea6179f079b554d5e2c8c98ccea8423"
 }
 
 from . import _version
 __version__ = _version.get_versions()['version']
```

### Comparing `stepcount-2.1.6/src/stepcount/features.py` & `stepcount-2.2.0/src/stepcount/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
     if len(valleys) > 0:
         acf_1st_min_loc = valleys[0]
         acf_1st_min = u[acf_1st_min_loc]
         acf_1st_min_loc /= sample_rate  # in secs
     else:
         acf_1st_min = acf_1st_min_loc = 0.0
 
-    acf_zeros = np.where(np.diff(np.signbit(u)))
-    acf_zeros = len(acf_zeros)
+    acf_zeros = np.sum(np.diff(np.signbit(u)))
 
     feats = {
         'acf_1st_max': acf_1st_max,
         'acf_1st_max_loc': acf_1st_max_loc,
         'acf_1st_min': acf_1st_min,
         'acf_1st_min_loc': acf_1st_min_loc,
         'acf_zeros': acf_zeros,
```

### Comparing `stepcount-2.1.6/src/stepcount/hmm_utils.py` & `stepcount-2.2.0/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/src/stepcount/models.py` & `stepcount-2.2.0/src/stepcount/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,15 @@
         x = fn(x)
         X.append(x)
         T.append(t)
 
     X = np.asarray(X)
 
     if return_index:
-        T = pd.DatetimeIndex(T)
+        T = pd.DatetimeIndex(T, name=data.index.name)
         return X, T
 
     return X
 
 
 def cvp(
     model, X, Y, groups,
```

### Comparing `stepcount-2.1.6/src/stepcount/sslmodel.py` & `stepcount-2.2.0/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/src/stepcount/stepcount.py` & `stepcount-2.2.0/src/stepcount/stepcount.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/src/stepcount/utils/collate_outputs.py` & `stepcount-2.2.0/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/src/stepcount.egg-info/PKG-INFO` & `stepcount-2.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,37 @@
-Metadata-Version: 2.1
-Name: stepcount
-Version: 2.1.6
-Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
-Home-page: https://github.com/OxWearables/stepcount
-Download-URL: https://github.com/OxWearables/stepcount
-Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
-Maintainer: Shing Chan
-Maintainer-email: shing.chan@ndph.ox.ac.uk
-License: See LICENSE file.
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE.md
-
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
 
-Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
-
-## Getting started
+## Install
 
-### Prerequisite
+We recommend using **Anaconda**:
 
-- Python 3.8 or greater
+1. Download & install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda).
+1. (Windows) Once installed, launch the **Anaconda Prompt**.
+1. Create a virtual environment:
     ```console
-    $ python --version  # or python3 --version
+    $ conda create -n stepcount python=3.9 openjdk pip
     ```
-
-- Java 8 (1.8.0) or greater
+    This creates a virtual environment called `stepcount` with Python version 3.9, OpenJDK, and Pip.
+1. Activate the environment:
     ```console
-    $ java -version
+    $ conda activate stepcount
+    ```
+    You should now see `(stepcount)` written in front of your prompt.
+1. Install `stepcount`:
+    ```console
+    $ pip install stepcount
     ```
 
-### Install (Windows)
-For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
-
-1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
-2. Install. Use the default recommended settings.
-3. From the Start menu, search and open the **Anaconda Prompt**.
-
-```console
-$ pip install stepcount
-```
-
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda-on-windows.md).
-
-### Install (Linux)
-
-<!-- ```console
-$ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-<!-- ```console
-$ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-```console
-$ pip install stepcount
-```
-
+You are all set! The next time that you want to use `stepcount`, open the Anaconda Prompt and activate the environment (step 4). If you see `(stepcount)` in front of your prompt, you are ready to go!
 
+Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
 
 ## Usage
 
 ```bash
 # Process an AX3 file
 $ stepcount sample.cwa
 
@@ -113,14 +72,20 @@
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
 
+### Troubleshooting 
+Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
+```console
+$ conda install -n stepcount openjdk=8
+```
+
 ### Output files
 By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
 
 ```console
 $ stepcount sample.cwa -o /path/to/some/folder/
 ```
```

### Comparing `stepcount-2.1.6/src/stepcount.egg-info/SOURCES.txt` & `stepcount-2.2.0/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.6/versioneer.py` & `stepcount-2.2.0/versioneer.py`

 * *Files identical despite different names*

