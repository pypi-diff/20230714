# Comparing `tmp/miko_analyzer-0.3.2.tar.gz` & `tmp/miko_analyzer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miko_analyzer-0.3.2.tar", max compression
+gzip compressed data, was "miko_analyzer-0.3.3.tar", max compression
```

## Comparing `miko_analyzer-0.3.2.tar` & `miko_analyzer-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/LICENSE
--rw-r--r--   0        0        0      841 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/__init__.py
--rw-r--r--   0        0        0       97 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/__main__.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/cmdline/__init__.py
--rw-r--r--   0        0        0      280 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/cmdline/base.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/graph/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/graph/plotting.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/structure/__init__.py
--rw-r--r--   0        0        0     6812 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/structure/cluster.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/tesla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/__init__.py
--rw-r--r--   0        0        0     1419 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/exploration.py
--rw-r--r--   0        0        0      537 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/labeling.py
--rw-r--r--   0        0        0     1733 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/task.py
--rw-r--r--   0        0        0     1432 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/training.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/__init__.py
--rw-r--r--   0        0        0    24683 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/exploration.py
--rw-r--r--   0        0        0     4445 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/labeling.py
--rw-r--r--   0        0        0      829 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/task.py
--rw-r--r--   0        0        0     2787 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/training.py
--rw-r--r--   0        0        0        0 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/__init__.py
--rw-r--r--   0        0        0    11298 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/exploration.py
--rw-r--r--   0        0        0      725 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/labeling.py
--rw-r--r--   0        0        0     3353 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/task.py
--rw-r--r--   0        0        0     2040 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/training.py
--rw-r--r--   0        0        0       54 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/__init__.py
--rw-r--r--   0        0        0       57 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/files.py
--rw-r--r--   0        0        0      524 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/lammps.py
--rw-r--r--   0        0        0     1080 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/log_factory.py
--rw-r--r--   0        0        0       45 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/output.py
--rw-r--r--   0        0        0     1174 2023-07-05 14:19:05.164761 miko_analyzer-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 miko_analyzer-0.3.2/setup.py
--rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 miko_analyzer-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 06:51:00.149760 miko_analyzer-0.3.3/LICENSE
+-rw-r--r--   0        0        0      841 2023-07-14 06:51:00.149760 miko_analyzer-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/cmdline/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/cmdline/base.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/graph/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/graph/plotting.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/metad/__init__.py
+-rw-r--r--   0        0        0    30504 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/metad/fes.py
+-rw-r--r--   0        0        0     4392 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/metad/hills.py
+-rw-r--r--   0        0        0     6433 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/metad/profile.py
+-rw-r--r--   0        0        0    15572 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/metad/string.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/structure/__init__.py
+-rw-r--r--   0        0        0     6812 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/structure/cluster.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/ai2_kit/__init__.py
+-rw-r--r--   0        0        0     1419 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/ai2_kit/exploration.py
+-rw-r--r--   0        0        0      537 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/ai2_kit/labeling.py
+-rw-r--r--   0        0        0     1733 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/ai2_kit/task.py
+-rw-r--r--   0        0        0     1432 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/ai2_kit/training.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/base/__init__.py
+-rw-r--r--   0        0        0    24683 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/base/exploration.py
+-rw-r--r--   0        0        0     4445 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/base/labeling.py
+-rw-r--r--   0        0        0      829 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/base/task.py
+-rw-r--r--   0        0        0     2786 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/base/training.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/dpgen/__init__.py
+-rw-r--r--   0        0        0    11298 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/dpgen/exploration.py
+-rw-r--r--   0        0        0      725 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/dpgen/labeling.py
+-rw-r--r--   0        0        0     3353 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/dpgen/task.py
+-rw-r--r--   0        0        0     2040 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/tesla/dpgen/training.py
+-rw-r--r--   0        0        0       54 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/utils/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/utils/files.py
+-rw-r--r--   0        0        0      524 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/utils/lammps.py
+-rw-r--r--   0        0        0     1080 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/utils/log_factory.py
+-rw-r--r--   0        0        0       45 2023-07-14 06:51:00.165761 miko_analyzer-0.3.3/miko/utils/output.py
+-rw-r--r--   0        0        0     1117 2023-07-14 06:51:00.169761 miko_analyzer-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 miko_analyzer-0.3.3/setup.py
+-rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 miko_analyzer-0.3.3/PKG-INFO
```

### Comparing `miko_analyzer-0.3.2/LICENSE` & `miko_analyzer-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/README.md` & `miko_analyzer-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/graph/plotting.py` & `miko_analyzer-0.3.3/miko/graph/plotting.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/structure/cluster.py` & `miko_analyzer-0.3.3/miko/structure/cluster.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/ai2_kit/exploration.py` & `miko_analyzer-0.3.3/miko/tesla/ai2_kit/exploration.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/ai2_kit/labeling.py` & `miko_analyzer-0.3.3/miko/tesla/ai2_kit/labeling.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/ai2_kit/task.py` & `miko_analyzer-0.3.3/miko/tesla/ai2_kit/task.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/ai2_kit/training.py` & `miko_analyzer-0.3.3/miko/tesla/ai2_kit/training.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/base/exploration.py` & `miko_analyzer-0.3.3/miko/tesla/base/exploration.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/base/labeling.py` & `miko_analyzer-0.3.3/miko/tesla/base/labeling.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/base/task.py` & `miko_analyzer-0.3.3/miko/tesla/base/task.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/base/training.py` & `miko_analyzer-0.3.3/miko/tesla/base/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,17 @@
         axs[0].set_xlabel('Number of training batch')
         axs[0].set_ylabel('$E$(eV)')
         axs[0].legend()
 
         # force figure
         for key in lcurve_data.keys():
             if key.startswith('force_'):
-                axs[1].plot(step[10:], lcurve_data[key][10:],
-                            alpha=0.4, label=key.replace('force_', ''))
+                axs[1].plot(
+                    step[10:], lcurve_data[key][10:], label=key.replace('force_', '')
+                )
         axs[1].axhline(0.05, linestyle='dashed', color='red', label='50 meV/Å')
         axs[1].axhline(0.1, linestyle='dashed', color='blue', label='100 meV/Å')
         axs[1].axhline(0.2, linestyle='dashed', label='200 meV/Å')
         axs[1].set_xlabel('Number of training batch')
         axs[1].set_ylabel('$F$(eV/Å)')
         axs[1].legend()
```

### Comparing `miko_analyzer-0.3.2/miko/tesla/dpgen/exploration.py` & `miko_analyzer-0.3.3/miko/tesla/dpgen/exploration.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/dpgen/labeling.py` & `miko_analyzer-0.3.3/miko/tesla/dpgen/labeling.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/dpgen/task.py` & `miko_analyzer-0.3.3/miko/tesla/dpgen/task.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/tesla/dpgen/training.py` & `miko_analyzer-0.3.3/miko/tesla/dpgen/training.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/utils/lammps.py` & `miko_analyzer-0.3.3/miko/utils/lammps.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/miko/utils/log_factory.py` & `miko_analyzer-0.3.3/miko/utils/log_factory.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.2/pyproject.toml` & `miko_analyzer-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 [tool.poetry]
 name = "miko-analyzer"
-version = "0.3.2"
+version = "0.3.3"
 description = "Analyzing tool for deep learning based chemical research."
 authors = ["Cloudac7 <scottryuu@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cloudac7/miko-analysis"
 packages = [{include = "miko"}]
 
-[tool.poetry-dynamic-versioning]
-enable = true
-
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
 ase = "^3.21.1"
 matplotlib = "^3.7.1"
 numpy = "<1.24,>=1.18"
 pandas = "^1.3.3"
-dpdata = "*"
-dscribe = "*"
-dynaconf = "*"
+dscribe = "^2.0"
 mdanalysis = "^2.2"
 scipy = "^1.10.1"
-seaborn = "*"
-tqdm = "^4.65.0"
+seaborn = "^0.12.2"
 pymatgen = "^2023.5.10"
 ai2-kit = "^0.3.18"
 
 [tool.poetry.group.test.dependencies]
 flake8 = "*"
 pytest = "*"
 pytest-mock = "*"
@@ -38,14 +32,15 @@
 [tool.poetry.group.docs.dependencies]
 mkdocstrings = { version = ">=0.18", extras = ["python"] }
 mkdocs-material = "*"
 mike = "*"
 mkdocs-gen-files = "*"
 mkdocs-literate-nav = "^0.5.0"
 mkdocs-section-index = "*"
+mkdocs-jupyter = "^0.24.2"
 
 [tool.poetry.scripts]
 miko = 'miko.cmdline.base:cli'
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `miko_analyzer-0.3.2/setup.py` & `miko_analyzer-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['miko',
  'miko.cmdline',
  'miko.graph',
+ 'miko.metad',
  'miko.structure',
  'miko.tesla',
  'miko.tesla.ai2_kit',
  'miko.tesla.base',
  'miko.tesla.dpgen',
  'miko.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ai2-kit>=0.3.18,<0.4.0',
  'ase>=3.21.1,<4.0.0',
- 'dpdata',
- 'dscribe',
- 'dynaconf',
+ 'dscribe>=2.0,<3.0',
  'matplotlib>=3.7.1,<4.0.0',
  'mdanalysis>=2.2,<3.0',
  'numpy>=1.18,<1.24',
  'pandas>=1.3.3,<2.0.0',
  'pymatgen>=2023.5.10,<2024.0.0',
  'scipy>=1.10.1,<2.0.0',
- 'seaborn',
- 'tqdm>=4.65.0,<5.0.0']
+ 'seaborn>=0.12.2,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['miko = miko.cmdline.base:cli']}
 
 setup_kwargs = {
     'name': 'miko-analyzer',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Analyzing tool for deep learning based chemical research.',
     'long_description': '# Miko-Analyzer\n\n[![Python package](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml/badge.svg)](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml)\n[![Coverage Status](https://coveralls.io/repos/github/Cloudac7/miko-analyzer/badge.svg?branch=master)](https://coveralls.io/github/Cloudac7/miko-analyzer?branch=master)\n\n> コードで占う巫女。\n> Miko using code to perform divinition.\n\nAn analysis plugin for [Deep Potential](https://github.com/deepmodeling/deepmd-kit) based chemical research.\n\nSupporting simple calculation workflow with the help of [DPDispatcher](https://github.com/deepmodeling/dpdispatcher).\n\n## Installation\n\nTo install, clone the repository:\n\n```\ngit clone https://github.com/cloudac7/miko-analyzer.git\n```\n\nand then install with `pip`:\n\n```\ncd miko-analyzer\npip install .\n```\n\n',
     'author': 'Cloudac7',
     'author_email': 'scottryuu@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cloudac7/miko-analysis',
```

### Comparing `miko_analyzer-0.3.2/PKG-INFO` & `miko_analyzer-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: miko-analyzer
-Version: 0.3.2
+Version: 0.3.3
 Summary: Analyzing tool for deep learning based chemical research.
 Home-page: https://github.com/cloudac7/miko-analysis
 License: Apache-2.0
 Author: Cloudac7
 Author-email: scottryuu@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ai2-kit (>=0.3.18,<0.4.0)
 Requires-Dist: ase (>=3.21.1,<4.0.0)
-Requires-Dist: dpdata
-Requires-Dist: dscribe
-Requires-Dist: dynaconf
+Requires-Dist: dscribe (>=2.0,<3.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mdanalysis (>=2.2,<3.0)
 Requires-Dist: numpy (>=1.18,<1.24)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: pymatgen (>=2023.5.10,<2024.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Requires-Dist: seaborn
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Project-URL: Repository, https://github.com/cloudac7/miko-analysis
 Description-Content-Type: text/markdown
 
 # Miko-Analyzer
 
 [![Python package](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml/badge.svg)](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/Cloudac7/miko-analyzer/badge.svg?branch=master)](https://coveralls.io/github/Cloudac7/miko-analyzer?branch=master)
```

