# Comparing `tmp/anonymeter-0.0.1.tar.gz` & `tmp/anonymeter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonymeter-0.0.1.tar", last modified: Mon Apr 24 10:23:24 2023, max compression
+gzip compressed data, was "anonymeter-0.0.2.tar", last modified: Tue Jul 11 18:21:01 2023, max compression
```

## Comparing `anonymeter-0.0.1.tar` & `anonymeter-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/
--rw-r--r--   0 me        (1000) me        (1000)     1670 2023-04-10 23:30:32.000000 anonymeter-0.0.1/LICENSE.md
--rw-r--r--   0 me        (1000) me        (1000)     7682 2023-04-24 10:23:24.348593 anonymeter-0.0.1/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     5153 2023-04-24 10:20:15.000000 anonymeter-0.0.1/README.md
--rw-r--r--   0 me        (1000) me        (1000)     2370 2023-04-24 10:23:02.000000 anonymeter-0.0.1/pyproject.toml
--rw-r--r--   0 me        (1000) me        (1000)       38 2023-04-24 10:23:24.348593 anonymeter-0.0.1/setup.cfg
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.338594 anonymeter-0.0.1/src/
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.338594 anonymeter-0.0.1/src/anonymeter/
--rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/__init__.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/src/anonymeter/evaluators/
--rw-r--r--   0 me        (1000) me        (1000)      590 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/evaluators/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     9092 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/evaluators/inference_evaluator.py
--rw-r--r--   0 me        (1000) me        (1000)    11629 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/evaluators/linkability_evaluator.py
--rw-r--r--   0 me        (1000) me        (1000)    17870 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/evaluators/singling_out_evaluator.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/src/anonymeter/neighbors/
--rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/neighbors/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     8776 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/neighbors/mixed_types_kneighbors.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/src/anonymeter/preprocessing/
--rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/preprocessing/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     3693 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/preprocessing/transformations.py
--rw-r--r--   0 me        (1000) me        (1000)     1658 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/preprocessing/type_detection.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/src/anonymeter/stats/
--rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/stats/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)     7803 2023-04-10 23:30:32.000000 anonymeter-0.0.1/src/anonymeter/stats/confidence.py
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/src/anonymeter.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     7682 2023-04-24 10:23:24.000000 anonymeter-0.0.1/src/anonymeter.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      960 2023-04-24 10:23:24.000000 anonymeter-0.0.1/src/anonymeter.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-04-24 10:23:24.000000 anonymeter-0.0.1/src/anonymeter.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)      363 2023-04-24 10:23:24.000000 anonymeter-0.0.1/src/anonymeter.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       11 2023-04-24 10:23:24.000000 anonymeter-0.0.1/src/anonymeter.egg-info/top_level.txt
-drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-04-24 10:23:24.348593 anonymeter-0.0.1/tests/
--rw-r--r--   0 me        (1000) me        (1000)     5026 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_confidence.py
--rw-r--r--   0 me        (1000) me        (1000)     4103 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_inference_evaluator.py
--rw-r--r--   0 me        (1000) me        (1000)     5463 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_linkability_evaluator.py
--rw-r--r--   0 me        (1000) me        (1000)     2859 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_mixed_types_kneigbors.py
--rw-r--r--   0 me        (1000) me        (1000)     4203 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_singling_out_evaluator.py
--rw-r--r--   0 me        (1000) me        (1000)     2885 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_transformations.py
--rw-r--r--   0 me        (1000) me        (1000)     1643 2023-04-10 23:30:32.000000 anonymeter-0.0.1/tests/test_type_detection.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.449106 anonymeter-0.0.2/
+-rw-r--r--   0 me        (1000) me        (1000)     1671 2023-05-12 13:26:20.000000 anonymeter-0.0.2/LICENSE.md
+-rw-r--r--   0 me        (1000) me        (1000)     9658 2023-07-11 18:21:01.438272 anonymeter-0.0.2/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     7035 2023-05-12 13:26:20.000000 anonymeter-0.0.2/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     2537 2023-07-07 14:19:56.000000 anonymeter-0.0.2/pyproject.toml
+-rw-r--r--   0 me        (1000) me        (1000)       38 2023-07-11 18:21:01.449106 anonymeter-0.0.2/setup.cfg
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.405772 anonymeter-0.0.2/src/
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.416606 anonymeter-0.0.2/src/anonymeter/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2023-05-10 04:20:50.000000 anonymeter-0.0.2/src/anonymeter/__init__.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.427439 anonymeter-0.0.2/src/anonymeter/evaluators/
+-rw-r--r--   0 me        (1000) me        (1000)      590 2023-04-10 23:30:32.000000 anonymeter-0.0.2/src/anonymeter/evaluators/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     9078 2023-05-12 13:26:20.000000 anonymeter-0.0.2/src/anonymeter/evaluators/inference_evaluator.py
+-rw-r--r--   0 me        (1000) me        (1000)    11666 2023-05-12 13:26:20.000000 anonymeter-0.0.2/src/anonymeter/evaluators/linkability_evaluator.py
+-rw-r--r--   0 me        (1000) me        (1000)    18133 2023-05-12 13:26:20.000000 anonymeter-0.0.2/src/anonymeter/evaluators/singling_out_evaluator.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.427439 anonymeter-0.0.2/src/anonymeter/neighbors/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.2/src/anonymeter/neighbors/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     8813 2023-05-12 13:26:20.000000 anonymeter-0.0.2/src/anonymeter/neighbors/mixed_types_kneighbors.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.427439 anonymeter-0.0.2/src/anonymeter/preprocessing/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.2/src/anonymeter/preprocessing/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     3730 2023-05-12 13:26:20.000000 anonymeter-0.0.2/src/anonymeter/preprocessing/transformations.py
+-rw-r--r--   0 me        (1000) me        (1000)     1658 2023-04-10 23:30:32.000000 anonymeter-0.0.2/src/anonymeter/preprocessing/type_detection.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.438272 anonymeter-0.0.2/src/anonymeter/stats/
+-rw-r--r--   0 me        (1000) me        (1000)        0 2023-04-10 23:30:32.000000 anonymeter-0.0.2/src/anonymeter/stats/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)     7803 2023-04-10 23:30:32.000000 anonymeter-0.0.2/src/anonymeter/stats/confidence.py
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.427439 anonymeter-0.0.2/src/anonymeter.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     9658 2023-07-11 18:21:01.000000 anonymeter-0.0.2/src/anonymeter.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      960 2023-07-11 18:21:01.000000 anonymeter-0.0.2/src/anonymeter.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-07-11 18:21:01.000000 anonymeter-0.0.2/src/anonymeter.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)      355 2023-07-11 18:21:01.000000 anonymeter-0.0.2/src/anonymeter.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       11 2023-07-11 18:21:01.000000 anonymeter-0.0.2/src/anonymeter.egg-info/top_level.txt
+drwxr-xr-x   0 me        (1000) me        (1000)        0 2023-07-11 18:21:01.438272 anonymeter-0.0.2/tests/
+-rw-r--r--   0 me        (1000) me        (1000)     5026 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_confidence.py
+-rw-r--r--   0 me        (1000) me        (1000)     4103 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_inference_evaluator.py
+-rw-r--r--   0 me        (1000) me        (1000)     5463 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_linkability_evaluator.py
+-rw-r--r--   0 me        (1000) me        (1000)     2859 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_mixed_types_kneigbors.py
+-rw-r--r--   0 me        (1000) me        (1000)     4203 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_singling_out_evaluator.py
+-rw-r--r--   0 me        (1000) me        (1000)     2885 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_transformations.py
+-rw-r--r--   0 me        (1000) me        (1000)     1643 2023-04-10 23:30:32.000000 anonymeter-0.0.2/tests/test_type_detection.py
```

### Comparing `anonymeter-0.0.1/LICENSE.md` & `anonymeter-0.0.2/LICENSE.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE IP OWNER OR
 CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
+POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `anonymeter-0.0.1/PKG-INFO` & `anonymeter-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,21 @@
-Metadata-Version: 2.1
-Name: anonymeter
-Version: 0.0.1
-Summary: Measure singling out, linkability, and inference risk for synthetic data.
-Author-email: Statice GmbH <hello@statice.ai>
-License: The Clear BSD License
-        
-        Copyright (c) 2022 Anonos IP LLC (IP Owner)
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without modification,
-        are permitted (subject to the limitations in the disclaimer below) provided that
-        the following conditions are met:
-        
-             * Redistributions of source code must retain the above copyright notice,
-             this list of conditions and the following disclaimer.
-        
-             * Redistributions in binary form must reproduce the above copyright
-             notice, this list of conditions and the following disclaimer in the
-             documentation and/or other materials provided with the distribution.
-        
-             * Neither the name of the IP owner nor the names of its
-             contributors may be used to endorse or promote products derived from this
-             software without specific prior written permission.
-        
-        NO EXPRESS OR IMPLIED LICENSES TO ANY PARTY'S PATENT RIGHTS ARE GRANTED BY
-        THIS LICENSE. THIS SOFTWARE IS PROVIDED BY THE IP OWNER AND
-        CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-        LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-        PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE IP OWNER OR
-        CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-        EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
-        PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
-        BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-        IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-        ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-        POSSIBILITY OF SUCH DAMAGE.
-Project-URL: Homepage, https://github.com/statice/anonymeter
-Project-URL: Bug Tracker, https://github.com/statice/anonymeter/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>3.7
-Description-Content-Type: text/markdown
-Provides-Extra: notebooks
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # Anonymeter: Unified Framework for Quantifying Privacy Risk in Synthetic Data
 
 `Anonymeter` is a unified statistical framework to jointly quantify different
 types of privacy risks in synthetic tabular datasets. `Anonymeter` is equipped
 with attack-based evaluations for the **Singling Out**, **Linkability**, and
 **Inference** risks, which are the three key indicators of factual anonymization
 according to the [Article 29 Working Party](https://ec.europa.eu/justice/article-29/documentation/opinion-recommendation/files/2014/wp216_en.pdf).
 
-A simple explanation of how `Anonymeter` works is provided below. For more details, a throughout
-description of the working of the framework and the attack algorithms can be found in the paper
-[A Unified Framework for Quantifying Privacy Risk in Synthetic Data](https://arxiv.org/abs/2211.10459).
-This work has been accepted at the 23rd Privacy Enhancing Technologies Symposium ([PETS 2023](https://petsymposium.org/cfp23.php)).
+
+> Anonymeter has been positively reviewed by the technical experts from the [Commission Nationale de l’Informatique et des Libertés (CNIL)](https://www.cnil.fr/en/home) which, in their words, _“have not identified any reason suggesting that the proposed set of methods could not allow to effectively evaluate the extent to which the aforementioned three criteria are fulfilled or not in the context of production and use of synthetic datasets”_. The CNIL also expressed the opinion that the results of Anonymeter (i.e. the three risk scores) **should be used by the data controller to decide whether the residual risks of re-identification are acceptable or not, and whether the dataset could be considered anonymous**.
 
 
+## `Anonymeter` in a nutshel
+
 In `Anonymeter` each privacy risk is derived from a privacy attacker whose task is to use the synthetic dataset
 to come up with a set of *guesses* of the form:
 - "there is only one person with attributes X, Y, and Z" (singling out)
 - "records A and B belong to the same person" (linkability)
 - "a person with attributes X and Y also have Z" (inference)
 
 Each evaluation consists of running three different attacks:
@@ -73,26 +25,39 @@
 
 Checking how many of these guesses are correct, the success rates of the different attacks are measured and used to
 derive an estimate of the privacy risk. In particular, the "control attack" is used to separate what the attacker
 learns from the *utility* of the synthetic data, and what is instead indication of privacy leaks.
 The "baseline attack" instead functions as a sanity check. The "main attack" attack should outperform random
 guessing in order for the results to be trusted.
 
+For more details, a throughout
+description of the framework and the attack algorithms can be found in the paper
+[A Unified Framework for Quantifying Privacy Risk in Synthetic Data](https://petsymposium.org/popets/2023/popets-2023-0055.php), accepted at the 23rd Privacy Enhancing Technologies Symposium ([PETS 2023](https://petsymposium.org/cfp23.php)).
+
+
 
 ## Setup and installation
 
-Anonymeter requires Python 3.8.x, 3.9.x or 3.10.x installed.
+`Anonymeter` requires Python 3.8.x, 3.9.x or 3.10.x installed. The simplest way to install `Anonymeter` is from `PyPi`. Simply run
+
+```
+pip install anonymeter
+```
 
-Clone the Anonymeter repository:
+and you are good to go.
+
+### Local installation
+
+To install `Anonymeter` locally, clone the repository:
 
 ```shell
 git clone git@github.com:statice/anonymeter.git
 ```
 
-Install the dependencies:
+and install the dependencies:
 
 ```shell
 cd anonymeter  # if you are not there already
 pip install . # Basic dependencies
 pip install ".[notebooks]" # Dependencies to run example notebooks
 pip install -e ".[notebooks,dev]" # Development setup
 ```
@@ -104,17 +69,23 @@
 
 Check out the example notebook in the `notebooks` folder to start playing around
 with `anonymeter`. To run this notebook you would need `jupyter` and some plotting libraries.
 This should be installed as part of the `notebooks` dependencies. If you haven't done so, please
 install them by executing:
 
 ```shell
+pip install anonymeter[notebooks]
+```
+if you are installing anonymeter from `PyPi`, or:
+
+```shell
 pip install ".[notebooks]"
 ```
 
+if you have opted for a local installation.
 
 ## Basic usage pattern
 
 For each of the three privacy risks anonymeter provide an `Evaluator` class. The high-level classes `SinglingOutEvaluator`, `LinkabilityEvaluator`, and `InferenceEvaluator` are the only thing that you need to import from `Anonymeter`.
 
 Despite the different nature of the privacy risks they evaluate, these classes have the same interface and are used in the same way. To instantiate the evaluator you have to provide three dataframes: the original dataset `ori` which has been used to generate the synthetic data, the synthetic data `syn`, and a `control` dataset containing original records which have not been used to generate the synthetic data.
 
@@ -130,20 +101,52 @@
 Once instantiated the evaluation pipeline is executed when calling the `evaluate`, and the resulting estimate of the risk can be accessed using the `risk()` method.
 
 ```python
 evaluator.evaluate()
 risk = evaluator.risk()
 ```
 
+## Configuring logging
+
+`Anonymeter` uses the standard Python logger named `anonymeter`.
+You can configure the logging level and the output destination
+using the standard Python logging API (see [here](https://docs.python.org/3/library/logging.html) for more details).
+
+For example, to set the logging level to `DEBUG` you can use the following snippet:
+
+```python
+import logging
+
+# set the logging level to DEBUG
+logging.getLogger("anonymeter").setLevel(logging.DEBUG)
+```
+
+And if you want to log to a file, you can use the following snippet:
+
+```python
+import logging
+
+# create a file handler
+file_handler = logging.FileHandler("anonymeter.log")
+
+# set the logging level for the file handler
+file_handler.setLevel(logging.DEBUG)
+
+# add the file handler to the logger
+logger = logging.getLogger("anonymeter")
+logger.addHandler(file_handler)
+logger.setLevel(logging.DEBUG)
+```
+
+
 ## Cite this work
 
 If you use anonymeter in your work, we would appreciate citations to the following paper:
 
 "A Unified Framework for Quantifying Privacy Risk in Synthetic Data", M. Giomi *et al*, PoPETS 2023.
-
 This `bibtex` entry can be used to refer to the paper:
 
 ```text
 @misc{anonymeter,
   doi = {https://doi.org/10.56553/popets-2023-0055},
   url = {https://petsymposium.org/popets/2023/popets-2023-0055.php},
   journal = {Proceedings of Privacy Enhancing Technologies Symposium},
```

### Comparing `anonymeter-0.0.1/pyproject.toml` & `anonymeter-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # See https://github.com/statice/anonymeter/blob/main/LICENSE.md for details.
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anonymeter"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Statice GmbH", email="hello@statice.ai" },
 ]
 description = "Measure singling out, linkability, and inference risk for synthetic data."
 readme = "README.md"
 requires-python = "<3.11, >3.7" # limited by Numba support
 license = {file = "LICENSE.md"}
@@ -33,32 +33,40 @@
 notebooks = [
     "jupyterlab~=3.4",
     "matplotlib~=3.5",
     "seaborn~=0.11",
 ]
 
 dev = [
+    # Linting and code checks
     "flake8~=5.0",
     "flake8-docstrings~=1.6.0",
     "flake8-eradicate~=1.4.0",
     "flake8-broken-line~=0.5",
     "flake8-bugbear~=23.2",
+    "pre-commit==2.20.0",
+    "mypy~=1.2.0",
+
+    # Code formatting
     "isort~=5.10",
     "black~=22.10",
-    "pre-commit==2.20.0",
+
+    # Testing
     "pytest==7.1.2",
     "pytest-cov==3.0.0",
-    "mypy==0.961",
-    "pytest-mypy==0.9.1",
+
+    # Building and packaging
     "build~=0.10",
+    "twine~=4.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/statice/anonymeter"
 "Bug Tracker" = "https://github.com/statice/anonymeter/issues"
+"Changelog" = "https://github.com/statice/anonymeter/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = "black"
 known_first_party = "anonymeter"
 line_length = 120
 skip = [
     ".git",
```

### Comparing `anonymeter-0.0.1/src/anonymeter/evaluators/__init__.py` & `anonymeter-0.0.2/src/anonymeter/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/src/anonymeter/evaluators/inference_evaluator.py` & `anonymeter-0.0.2/src/anonymeter/evaluators/inference_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     syn: pd.DataFrame,
     n_attacks: int,
     aux_cols: List[str],
     secret: str,
     n_jobs: int,
     naive: bool,
     regression: Optional[bool],
-) -> np.ndarray:
+) -> int:
     if regression is None:
         regression = pd.api.types.is_numeric_dtype(target[secret])
 
     targets = target.sample(n_attacks, replace=False)
 
     if naive:
         guesses = syn.sample(n_attacks)[secret]
@@ -155,15 +155,15 @@
         self._control = control
         self._n_attacks = n_attacks
         self._secret = secret
         self._regression = regression
         self._aux_cols = aux_cols
         self._evaluated = False
 
-    def _attack(self, target: pd.DataFrame, naive: bool, n_jobs: int) -> np.ndarray:
+    def _attack(self, target: pd.DataFrame, naive: bool, n_jobs: int) -> int:
         return _run_attack(
             target=target,
             syn=self._syn,
             n_attacks=self._n_attacks,
             aux_cols=self._aux_cols,
             secret=self._secret,
             n_jobs=n_jobs,
```

### Comparing `anonymeter-0.0.1/src/anonymeter/evaluators/linkability_evaluator.py` & `anonymeter-0.0.2/src/anonymeter/evaluators/linkability_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import numpy as np
 import pandas as pd
 
 from anonymeter.neighbors.mixed_types_kneighbors import MixedTypeKNeighbors
 from anonymeter.stats.confidence import EvaluationResults, PrivacyRisk
 
+logger = logging.getLogger(__name__)
+
 
 class LinkabilityIndexes:
     """Utility class to store indexes from linkability attack.
 
     Parameters
     ----------
     idx_0 : np.ndarray
@@ -46,15 +48,15 @@
         -------
         Dict[int, Set[int]]
             Dictionary mapping the index of the linking synthetic record
             to the index of the linked original record.
 
         """
         if n_neighbors > self._idx_0.shape[0]:
-            logging.warning(f"Neighbors too large ({n_neighbors}, using {self._idx_0.shape[0]}) instead.")
+            logger.warning(f"Neighbors too large ({n_neighbors}, using {self._idx_0.shape[0]}) instead.")
             n_neighbors = self._idx_0.shape[0]
 
         if n_neighbors < 1:
             raise ValueError(f"Invalid neighbors value ({n_neighbors}): must be positive.")
 
         links = {}
         for ii, (row0, row1) in enumerate(zip(self._idx_0, self._idx_1)):
```

### Comparing `anonymeter-0.0.1/src/anonymeter/evaluators/singling_out_evaluator.py` & `anonymeter-0.0.2/src/anonymeter/evaluators/singling_out_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pandas as pd
 from pandas.api.types import is_bool_dtype, is_categorical_dtype, is_numeric_dtype
 from scipy.optimize import curve_fit
 
 from anonymeter.stats.confidence import EvaluationResults, PrivacyRisk
 
 rng = np.random.default_rng()
+logger = logging.getLogger(__name__)
 
 
 def _escape_quotes(string: str) -> str:
     return string.replace('"', '\\"').replace("'", "\\'")
 
 
 def _query_expression(col: str, val: Any, dtype: np.dtype) -> str:
@@ -118,15 +119,15 @@
 
 
 def safe_query_counts(query: str, df: pd.DataFrame) -> Optional[int]:
     """Return number of elements satisfying a given query."""
     try:
         return len(df.query(query, engine="python"))
     except Exception as ex:
-        logging.debug(f"Query {query} failed with {ex}.")
+        logger.debug(f"Query {query} failed with {ex}.")
         return None
 
 
 def singling_out_probability_integral(n: int, w_min: float, w_max: float) -> float:
     """Integral of the singling out probability within a given range.
 
     The probability that a query singles out in a population of size
@@ -342,15 +343,15 @@
     return so_queries.queries
 
 
 def _evaluate_queries(df: pd.DataFrame, queries: List[str]) -> List[str]:
     counts = np.array([safe_query_counts(query=q, df=df) for q in queries], dtype=float)
 
     if np.any(np.isnan(counts)) > 0:
-        logging.warning(
+        logger.warning(
             f"Found {np.sum(np.isnan(counts))} failed queries "
             f"out of {len(queries)}. Check DEBUG messages for more details."
         )
 
     success = counts == 1
     return [q for iq, q in enumerate(queries) if success[iq]]
 
@@ -362,15 +363,15 @@
     elif mode == "multivariate":
         queries = multivariate_singling_out_queries(df=df, n_queries=n_attacks, n_cols=n_cols)
 
     else:
         raise RuntimeError(f"Parameter `mode` can be either `univariate` or `multivariate`. Got {mode} instead.")
 
     if len(queries) < n_attacks:
-        logging.warning(
+        logger.warning(
             f"Attack `{mode}` could generate only {len(queries)} "
             f"singling out queries out of the requested {n_attacks}. "
             "This can probably lead to an underestimate of the "
             "singling out risk."
         )
     return queries
 
@@ -440,30 +441,35 @@
         -------
         List[str]:
             successful singling out queries.
 
         """
         return self._random_queries if baseline else self._queries
 
-    def evaluate(self, mode: str) -> "SinglingOutEvaluator":
+    def evaluate(self, mode: str = "multivariate") -> "SinglingOutEvaluator":
         """Run the attack and evaluate the guesses on the original dataset.
 
         Parameters
         ----------
-        mode : str
+        mode : str, default is "multivariate"
             Name of the algorithm used to generate the singling out queries.
             Could be either `multivariate` or `univariate`.
 
         Returns
         -------
         self
             The evaluated singling out evaluator.
 
         """
-        n_cols = 1 if mode == "univariate" else self._n_cols
+        if mode == "multivariate":
+            n_cols = self._n_cols
+        elif mode == "univariate":
+            n_cols = 1
+        else:
+            raise ValueError(f"mode must be either 'multivariate' or 'univariate', got {mode} instead.")
 
         baseline_queries = _random_queries(df=self._syn, n_queries=self._n_attacks, n_cols=n_cols)
         self._baseline_queries = _evaluate_queries(df=self._ori, queries=baseline_queries)
         self._n_baseline = len(self._baseline_queries)
 
         queries = _generate_singling_out_queries(
             df=self._syn, n_attacks=self._n_attacks, n_cols=self._n_cols, mode=mode
```

### Comparing `anonymeter-0.0.1/src/anonymeter/neighbors/mixed_types_kneighbors.py` & `anonymeter-0.0.2/src/anonymeter/neighbors/mixed_types_kneighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import pandas as pd
 from joblib import Parallel, delayed
 from numba import float64, int64, jit
 
 from anonymeter.preprocessing.transformations import mixed_types_transform
 from anonymeter.preprocessing.type_detection import detect_consistent_col_types
 
+logger = logging.getLogger(__name__)
+
 
 @jit(nopython=True, nogil=True)
 def gower_distance(r0: np.ndarray, r1: np.ndarray, cat_cols_index: np.ndarray) -> float64:
     r"""Distance between two records inspired by the Gower distance [1].
 
     To handle mixed type data, the distance is specialized for numerical (continuous)
     and categorical data. For numerical records, we use the L1 norm,
@@ -195,15 +197,15 @@
             it is returned only if ``return_distances`` is ``True``
 
         """
         if n_neighbors is None:
             n_neighbors = self._n_neighbors
 
         if n_neighbors > self._candidates.shape[0]:
-            logging.warning(
+            logger.warning(
                 f"Parameter ``n_neighbors``={n_neighbors} cannot be "
                 f"larger than the size of the training data {self._candidates.shape[0]}."
             )
             n_neighbors = self._candidates.shape[0]
 
         if self._ctypes is None:
             self._ctypes = detect_consistent_col_types(df1=self._candidates, df2=queries)
```

### Comparing `anonymeter-0.0.1/src/anonymeter/preprocessing/transformations.py` & `anonymeter-0.0.2/src/anonymeter/preprocessing/transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 """Data pre-processing and transformations for the privacy evaluators."""
 import logging
 from typing import List, Tuple
 
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 
+logger = logging.getLogger(__name__)
+
 
 def _encode_categorical(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Encode dataframes with categorical values keeping label consistend."""
     encoded = pd.concat((df1, df2), keys=["df1", "df2"])
@@ -29,15 +31,15 @@
 
     mins = df1_min.where(df1_min < df2_min, df2_min)
     maxs = df1_max.where(df1_max > df2_max, df2_max)
     ranges = maxs - mins
 
     if any(ranges == 0):
         cnames = ", ".join(ranges[ranges == 0].index.values)
-        logging.debug(
+        logger.debug(
             f"Numerical column(s) {cnames} have a null-range: all elements "
             "have the same value. These column(s) won't be scaled."
         )
         ranges[ranges == 0] = 1
 
     df1_scaled = df1.apply(lambda x: x / ranges[x.name])
     df2_scaled = df2.apply(lambda x: x / ranges[x.name])
```

### Comparing `anonymeter-0.0.1/src/anonymeter/preprocessing/type_detection.py` & `anonymeter-0.0.2/src/anonymeter/preprocessing/type_detection.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/src/anonymeter/stats/confidence.py` & `anonymeter-0.0.2/src/anonymeter/stats/confidence.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/src/anonymeter.egg-info/PKG-INFO` & `anonymeter-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonymeter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Measure singling out, linkability, and inference risk for synthetic data.
 Author-email: Statice GmbH <hello@statice.ai>
 License: The Clear BSD License
         
         Copyright (c) 2022 Anonos IP LLC (IP Owner)
         All rights reserved.
         
@@ -31,16 +31,18 @@
         CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
         EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
         PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
         BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
         IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
         ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
         POSSIBILITY OF SUCH DAMAGE.
+        
 Project-URL: Homepage, https://github.com/statice/anonymeter
 Project-URL: Bug Tracker, https://github.com/statice/anonymeter/issues
+Project-URL: Changelog, https://github.com/statice/anonymeter/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.11,>3.7
 Description-Content-Type: text/markdown
 Provides-Extra: notebooks
 Provides-Extra: dev
@@ -50,20 +52,20 @@
 
 `Anonymeter` is a unified statistical framework to jointly quantify different
 types of privacy risks in synthetic tabular datasets. `Anonymeter` is equipped
 with attack-based evaluations for the **Singling Out**, **Linkability**, and
 **Inference** risks, which are the three key indicators of factual anonymization
 according to the [Article 29 Working Party](https://ec.europa.eu/justice/article-29/documentation/opinion-recommendation/files/2014/wp216_en.pdf).
 
-A simple explanation of how `Anonymeter` works is provided below. For more details, a throughout
-description of the working of the framework and the attack algorithms can be found in the paper
-[A Unified Framework for Quantifying Privacy Risk in Synthetic Data](https://arxiv.org/abs/2211.10459).
-This work has been accepted at the 23rd Privacy Enhancing Technologies Symposium ([PETS 2023](https://petsymposium.org/cfp23.php)).
+
+> Anonymeter has been positively reviewed by the technical experts from the [Commission Nationale de l’Informatique et des Libertés (CNIL)](https://www.cnil.fr/en/home) which, in their words, _“have not identified any reason suggesting that the proposed set of methods could not allow to effectively evaluate the extent to which the aforementioned three criteria are fulfilled or not in the context of production and use of synthetic datasets”_. The CNIL also expressed the opinion that the results of Anonymeter (i.e. the three risk scores) **should be used by the data controller to decide whether the residual risks of re-identification are acceptable or not, and whether the dataset could be considered anonymous**.
 
 
+## `Anonymeter` in a nutshel
+
 In `Anonymeter` each privacy risk is derived from a privacy attacker whose task is to use the synthetic dataset
 to come up with a set of *guesses* of the form:
 - "there is only one person with attributes X, Y, and Z" (singling out)
 - "records A and B belong to the same person" (linkability)
 - "a person with attributes X and Y also have Z" (inference)
 
 Each evaluation consists of running three different attacks:
@@ -73,26 +75,39 @@
 
 Checking how many of these guesses are correct, the success rates of the different attacks are measured and used to
 derive an estimate of the privacy risk. In particular, the "control attack" is used to separate what the attacker
 learns from the *utility* of the synthetic data, and what is instead indication of privacy leaks.
 The "baseline attack" instead functions as a sanity check. The "main attack" attack should outperform random
 guessing in order for the results to be trusted.
 
+For more details, a throughout
+description of the framework and the attack algorithms can be found in the paper
+[A Unified Framework for Quantifying Privacy Risk in Synthetic Data](https://petsymposium.org/popets/2023/popets-2023-0055.php), accepted at the 23rd Privacy Enhancing Technologies Symposium ([PETS 2023](https://petsymposium.org/cfp23.php)).
+
+
 
 ## Setup and installation
 
-Anonymeter requires Python 3.8.x, 3.9.x or 3.10.x installed.
+`Anonymeter` requires Python 3.8.x, 3.9.x or 3.10.x installed. The simplest way to install `Anonymeter` is from `PyPi`. Simply run
+
+```
+pip install anonymeter
+```
 
-Clone the Anonymeter repository:
+and you are good to go.
+
+### Local installation
+
+To install `Anonymeter` locally, clone the repository:
 
 ```shell
 git clone git@github.com:statice/anonymeter.git
 ```
 
-Install the dependencies:
+and install the dependencies:
 
 ```shell
 cd anonymeter  # if you are not there already
 pip install . # Basic dependencies
 pip install ".[notebooks]" # Dependencies to run example notebooks
 pip install -e ".[notebooks,dev]" # Development setup
 ```
@@ -104,17 +119,23 @@
 
 Check out the example notebook in the `notebooks` folder to start playing around
 with `anonymeter`. To run this notebook you would need `jupyter` and some plotting libraries.
 This should be installed as part of the `notebooks` dependencies. If you haven't done so, please
 install them by executing:
 
 ```shell
+pip install anonymeter[notebooks]
+```
+if you are installing anonymeter from `PyPi`, or:
+
+```shell
 pip install ".[notebooks]"
 ```
 
+if you have opted for a local installation.
 
 ## Basic usage pattern
 
 For each of the three privacy risks anonymeter provide an `Evaluator` class. The high-level classes `SinglingOutEvaluator`, `LinkabilityEvaluator`, and `InferenceEvaluator` are the only thing that you need to import from `Anonymeter`.
 
 Despite the different nature of the privacy risks they evaluate, these classes have the same interface and are used in the same way. To instantiate the evaluator you have to provide three dataframes: the original dataset `ori` which has been used to generate the synthetic data, the synthetic data `syn`, and a `control` dataset containing original records which have not been used to generate the synthetic data.
 
@@ -130,20 +151,52 @@
 Once instantiated the evaluation pipeline is executed when calling the `evaluate`, and the resulting estimate of the risk can be accessed using the `risk()` method.
 
 ```python
 evaluator.evaluate()
 risk = evaluator.risk()
 ```
 
+## Configuring logging
+
+`Anonymeter` uses the standard Python logger named `anonymeter`.
+You can configure the logging level and the output destination
+using the standard Python logging API (see [here](https://docs.python.org/3/library/logging.html) for more details).
+
+For example, to set the logging level to `DEBUG` you can use the following snippet:
+
+```python
+import logging
+
+# set the logging level to DEBUG
+logging.getLogger("anonymeter").setLevel(logging.DEBUG)
+```
+
+And if you want to log to a file, you can use the following snippet:
+
+```python
+import logging
+
+# create a file handler
+file_handler = logging.FileHandler("anonymeter.log")
+
+# set the logging level for the file handler
+file_handler.setLevel(logging.DEBUG)
+
+# add the file handler to the logger
+logger = logging.getLogger("anonymeter")
+logger.addHandler(file_handler)
+logger.setLevel(logging.DEBUG)
+```
+
+
 ## Cite this work
 
 If you use anonymeter in your work, we would appreciate citations to the following paper:
 
 "A Unified Framework for Quantifying Privacy Risk in Synthetic Data", M. Giomi *et al*, PoPETS 2023.
-
 This `bibtex` entry can be used to refer to the paper:
 
 ```text
 @misc{anonymeter,
   doi = {https://doi.org/10.56553/popets-2023-0055},
   url = {https://petsymposium.org/popets/2023/popets-2023-0055.php},
   journal = {Proceedings of Privacy Enhancing Technologies Symposium},
```

### Comparing `anonymeter-0.0.1/src/anonymeter.egg-info/SOURCES.txt` & `anonymeter-0.0.2/src/anonymeter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_confidence.py` & `anonymeter-0.0.2/tests/test_confidence.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_inference_evaluator.py` & `anonymeter-0.0.2/tests/test_inference_evaluator.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_linkability_evaluator.py` & `anonymeter-0.0.2/tests/test_linkability_evaluator.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_mixed_types_kneigbors.py` & `anonymeter-0.0.2/tests/test_mixed_types_kneigbors.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_singling_out_evaluator.py` & `anonymeter-0.0.2/tests/test_singling_out_evaluator.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_transformations.py` & `anonymeter-0.0.2/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `anonymeter-0.0.1/tests/test_type_detection.py` & `anonymeter-0.0.2/tests/test_type_detection.py`

 * *Files identical despite different names*

