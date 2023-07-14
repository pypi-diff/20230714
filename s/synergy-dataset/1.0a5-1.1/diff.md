# Comparing `tmp/synergy-dataset-1.0a5.tar.gz` & `tmp/synergy-dataset-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synergy-dataset-1.0a5.tar", last modified: Mon Apr 17 10:50:59 2023, max compression
+gzip compressed data, was "synergy-dataset-1.1.tar", last modified: Fri Jul 14 10:38:43 2023, max compression
```

## Comparing `synergy-dataset-1.0a5.tar` & `synergy-dataset-1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.071821 synergy-dataset-1.0a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.075821 synergy-dataset-1.0a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:50:59.083821 synergy-dataset-1.0a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/synergy_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/synergy_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/synergy_dataset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 10:50:58.000000 synergy-dataset-1.0a5/synergy_dataset/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/synergy_dataset/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/synergy_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 10:50:59.000000 synergy-dataset-1.0a5/synergy_dataset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:50:59.079820 synergy-dataset-1.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 10:50:46.000000 synergy-dataset-1.0a5/tests/test_synergy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.114902 synergy-dataset-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.110902 synergy-dataset-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.110902 synergy-dataset-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 10:38:29.000000 synergy-dataset-1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 10:38:29.000000 synergy-dataset-1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 10:38:29.000000 synergy-dataset-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-14 10:38:43.114902 synergy-dataset-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-14 10:38:29.000000 synergy-dataset-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 10:38:29.000000 synergy-dataset-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:38:43.114902 synergy-dataset-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.110902 synergy-dataset-1.1/synergy_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 10:38:29.000000 synergy-dataset-1.1/synergy_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-14 10:38:29.000000 synergy-dataset-1.1/synergy_dataset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 10:38:42.000000 synergy-dataset-1.1/synergy_dataset/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-14 10:38:29.000000 synergy-dataset-1.1/synergy_dataset/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.114902 synergy-dataset-1.1/synergy_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 10:38:43.000000 synergy-dataset-1.1/synergy_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:38:43.114902 synergy-dataset-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-14 10:38:29.000000 synergy-dataset-1.1/tests/test_synergy.py
```

### Comparing `synergy-dataset-1.0a5/.github/workflows/python-package.yml` & `synergy-dataset-1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a5/.github/workflows/python-publish.yml` & `synergy-dataset-1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a5/.gitignore` & `synergy-dataset-1.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -159,7 +159,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.ruff_cache
```

### Comparing `synergy-dataset-1.0a5/LICENSE` & `synergy-dataset-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a5/PKG-INFO` & `synergy-dataset-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a5
+Version: 1.1
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `synergy-dataset-1.0a5/README.md` & `synergy-dataset-1.1/README.md`

 * *Files identical despite different names*

### Comparing `synergy-dataset-1.0a5/pyproject.toml` & `synergy-dataset-1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 license = {text = "MIT"}
 dynamic = ["version"]
 requires-python = ">=3.7"
-dependencies = ["pyalex", "tabulate", "tqdm"]
+dependencies = ["requests", "pyalex", "tabulate", "tqdm"]
 
 [project.optional-dependencies]
 lint = ["flake8", "flake8-import-order"]
 test = ["pytest"]
 
 [project.scripts]
 synergy-dataset = "synergy_dataset.__main__:main"
@@ -33,7 +33,16 @@
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 
 [tool.setuptools]
 packages = ["synergy_dataset"]
 
 [tool.setuptools_scm]
 write_to = "synergy_dataset/_version.py"
+
+[tool.ruff]
+select = ["E", "F", "UP", "I", "B"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.isort]
+force-single-line = true
```

### Comparing `synergy-dataset-1.0a5/synergy_dataset/__main__.py` & `synergy-dataset-1.1/synergy_dataset/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import sys
 from pathlib import Path
 
 from tabulate import tabulate
 from tqdm import tqdm
 
 from synergy_dataset._version import __version__
-from synergy_dataset.base import Dataset
 from synergy_dataset.base import WORK_MAPPING
+from synergy_dataset.base import Dataset
 from synergy_dataset.base import _dataset_available
 from synergy_dataset.base import _get_path_raw_dataset
 from synergy_dataset.base import download_raw_dataset
 from synergy_dataset.base import iter_datasets
 
 LEGAL_NOTE = """
 Due to legal constraints, paper abstracts in SYNERGY cannot be published in
@@ -57,15 +57,15 @@
         "Use the commands 'get', 'list', 'show' or 'attribute'.",
     )
     # version
     parser.add_argument(
         "-V",
         "--version",
         action="version",
-        version="%(prog)s {version}".format(version=__version__),
+        version=f"%(prog)s {__version__}",
     )
 
     args, _ = parser.parse_known_args()
 
     parser.print_usage()
 
 
@@ -160,24 +160,18 @@
     parser.add_argument(
         "--tablefmt",
         default="simple",
         help="Table format.",
     )
     parser.add_argument(
         "--n-topics",
-        default=2,
+        default=3,
         type=int,
         help="The number of topics to display in the table.",
     )
-    parser.add_argument(
-        "--topic-level",
-        default=0,
-        type=int,
-        help="The level of the topics to display.",
-    )
     args = parser.parse_args(argv)
 
     # download the dataset if note available
     if not _dataset_available():
         download_raw_dataset()
 
     table_values = []
@@ -185,24 +179,15 @@
     n = 0
     n_incl = 0
 
     for i, dataset in enumerate(iter_datasets()):
         n += dataset.metadata["data"]["n_records"]
         n_incl += dataset.metadata["data"]["n_records_included"]
 
-        # if "concepts" not in dataset.metadata["publication"]:
-        #     print(dataset.metadata["publication"]["openalex_id"], "No concepts found")
-
-        concepts = list(
-            filter(
-                lambda x: x["level"] == args.topic_level,
-                dataset.metadata["publication"]["concepts"],
-            )
-        )
-
+        concepts = dataset.metadata["data"]["concepts"]["included"]
         n_topics = args.n_topics if args.n_topics != -1 else len(concepts)
         concepts_str = ", ".join([x["display_name"] for x in concepts[0:n_topics]])
         table_values.append(
             [
                 i + 1,
                 "{}".format(dataset.metadata["key"]),
                 concepts_str,
@@ -301,21 +286,21 @@
     if not _dataset_available():
         download_raw_dataset()
 
     # without url
     if args.format == "text":
         authors = []
 
-        for i, dataset in enumerate(iter_datasets()):
+        for dataset in iter_datasets():
             for a in dataset.metadata["publication"]["authorships"]:
                 authors.append(a["author"]["display_name"])
     elif args.format == "markdown":
         authors = []
 
-        for i, dataset in enumerate(iter_datasets()):
+        for dataset in iter_datasets():
             for a in dataset.metadata["publication"]["authorships"]:
                 if "orcid" in a["author"] and a["author"]["orcid"]:
                     authors.append(
                         f"[{a['author']['display_name']}]({a['author']['orcid']})"
                     )
                 else:
                     authors.append(a["author"]["display_name"])
@@ -328,27 +313,27 @@
     )
 
     print(", ".join(list(set(authors))), "\n")
 
     print("\nReferences to datasets:\n")
     prefix = "" if args.format == "text" else "> "
 
-    for i, dataset in enumerate(iter_datasets()):
+    for dataset in iter_datasets():
         print(
             f"{prefix}[{dataset.metadata['key']}]",
             dataset.cite,
         )
 
     print(
         "\nWe thank the authors of the following collections",
         "of systematic reviews:\n",
     )
 
     collections = []
-    for i, dataset in enumerate(iter_datasets()):
+    for dataset in iter_datasets():
         try:
             collections.append(dataset.cite_collection)
         except FileNotFoundError:
             pass
 
     for c in sorted(list(set(collections))):
         print(f"{prefix}{c}")
```

### Comparing `synergy-dataset-1.0a5/synergy_dataset.egg-info/PKG-INFO` & `synergy-dataset-1.1/synergy_dataset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synergy-dataset
-Version: 1.0a5
+Version: 1.1
 Summary: Python package for the SYNERGY dataset
 Author-email: Jonathan de Bruin <asreview@uu.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `synergy-dataset-1.0a5/synergy_dataset.egg-info/SOURCES.txt` & `synergy-dataset-1.1/synergy_dataset.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.flake8
 .gitignore
+.pre-commit-config.yaml
 CITATION.cff
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-lint.yml
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
```

