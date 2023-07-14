# Comparing `tmp/trattoria-0.3.4.tar.gz` & `tmp/trattoria-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trattoria-0.3.4.tar", max compression
+gzip compressed data, was "trattoria-0.3.5.tar", max compression
```

## Comparing `trattoria-0.3.4.tar` & `trattoria-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     2714 2021-08-06 15:02:23.156413 trattoria-0.3.4/README.md
--rw-r--r--   0        0        0      577 2021-08-06 15:15:29.694270 trattoria-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      347 2021-06-25 15:05:22.331092 trattoria-0.3.4/trattoria/__init__.py
--rw-r--r--   0        0        0    16141 2021-08-06 15:18:39.448016 trattoria-0.3.4/trattoria/core.py
--rw-r--r--   0        0        0     3033 2021-06-25 14:54:46.471247 trattoria-0.3.4/trattoria/postselection.py
--rw-r--r--   0        0        0     3502 2021-08-06 17:18:41.837117 trattoria-0.3.4/setup.py
--rw-r--r--   0        0        0     3494 2021-08-06 17:18:41.837606 trattoria-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3045 2023-07-13 16:18:55.310579 trattoria-0.3.5/README.md
+-rw-r--r--   0        0        0      583 2023-07-14 09:46:33.110667 trattoria-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-07-13 09:43:14.854450 trattoria-0.3.5/trattoria/__init__.py
+-rw-r--r--   0        0        0    16141 2023-07-13 09:43:14.854570 trattoria-0.3.5/trattoria/core.py
+-rw-r--r--   0        0        0     3033 2023-07-13 09:43:14.854629 trattoria-0.3.5/trattoria/postselection.py
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 trattoria-0.3.5/PKG-INFO
```

### Comparing `trattoria-0.3.4/README.md` & `trattoria-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 ## Examples
 The entry point to Trattoria is the PTUFile class. This class has methods that
 give us access to the algorithms. Each of the algorithms takes as input a
 parameter object and returns a results object. For a complete list of the
 functionality see the `examples` folder.
 
 ```python
+from pathlib import Path
+
 import trattoria
 
 import matplotlib.pyplot as plt
 
 ptu_filepath = Path("/path/to/some.ptu")
 ptu = trattoria.PTUFile(ptu_filepath)
 
@@ -54,21 +56,28 @@
 [trattoria-core](https://github.com/GCBallesteros/trattoria-core) library which
 itselfs provides a lower level interface to the the
 [tttr-toolbox](https://github.com/GCBallesteros/tttr-toolbox/tree/master/tttr-toolbox)
 library. A Rust project that provides the compiled components that allows us to
 go fast.
 
 ## Changelog
+### 0.3.5
+- Bug fix. The last 1024\*16 where being ignored for performance reasons. This has
+  has been fixed upstream in `tttr-toolbox` and this version of Trattoria uses the
+  upgraded version of `trattoria-core`.
+- `trattoria-core` dropped support for Python 3.6 and 3.7 and therefore Trattoria too.
+
 ### 0.3.4
 - The g2 algorithm now supports a mode flag. With "symmetric" we use the
   prefered version of the algorithm that returns negative and positive delays.
   "asymmetric" returns only positive delays but is faster. Default is
   "symmetric".
 
 ### 0.3.3
 - The underlying TTTR Toolbox and Trattoria Core were refactored to support
   multiple custom ranges or records at once. `start_range` and `stop_range`
   have disappeared in favor of `record_ranges`. It takes a list of tuples of
   integers or `None`.
 
+
 ## Citing
```

### Comparing `trattoria-0.3.4/pyproject.toml` & `trattoria-0.3.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "trattoria"
-version = "0.3.4"
+version = "0.3.5"
 description = "The fastest streaming algorithms for your TTTR data"
 authors = ["Guillem Ballesteros <dev+pypi@maxwellrules.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/GCBallesteros/trattoria"
 repository = "https://github.com/GCBallesteros/trattoria"
 
 [tool.poetry.dependencies]
-python = ">=3.6"
-numpy = ">=1.16"
-scipy = ">=1.5"
-trattoria-core = "0.4.3"
+python = ">=3.8,<3.12"
+numpy = ">=1.20"
+scipy = ">=1.8"
+trattoria-core = "0.4.4"
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `trattoria-0.3.4/trattoria/core.py` & `trattoria-0.3.5/trattoria/core.py`

 * *Files identical despite different names*

### Comparing `trattoria-0.3.4/trattoria/postselection.py` & `trattoria-0.3.5/trattoria/postselection.py`

 * *Files identical despite different names*

### Comparing `trattoria-0.3.4/setup.py` & `trattoria-0.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,105 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: trattoria
+Version: 0.3.5
+Summary: The fastest streaming algorithms for your TTTR data
+Home-page: https://github.com/GCBallesteros/trattoria
+License: MIT
+Author: Guillem Ballesteros
+Author-email: dev+pypi@maxwellrules.com
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.20)
+Requires-Dist: scipy (>=1.8)
+Requires-Dist: trattoria-core (==0.4.4)
+Project-URL: Repository, https://github.com/GCBallesteros/trattoria
+Description-Content-Type: text/markdown
+
+# 🍕 Trattoria 🍕
+Trattoria delivers you the fastest streaming algorithms to analyze your TTTR data. We
+currenlty support the following algorithms:
+- __Second order autocorrelations__: Calculate the autocorrelation between two channels of
+  your TCSPC.
+- __Third Order autocorrelations__: Calculate the coincidences between 3 channels. A sync
+version is provided were it uses the fact that the sync channel is periodic and known.
+- __Intensity time trace__: Calculate the intensity on each (or all) channels versus time.
+- __Zero finder__: Given two uncorrelated channels (e.g. a laser behind a 50/50 splitter)
+  compute the delay between the input channels.
+- __Lifetime__: Compute the lifetime histogram from a pulsed excitation experiment.
+
+## Supported file formats
+Currently Trattoria can only read PTU files from PicoQuant. If you want support
+for more or want to help providing it please put a ticket on the tttr-toolbox
+project.
+
+## Installing
+```
+pip install trattoria
+```
+
+## Examples
+The entry point to Trattoria is the PTUFile class. This class has methods that
+give us access to the algorithms. Each of the algorithms takes as input a
+parameter object and returns a results object. For a complete list of the
+functionality see the `examples` folder.
+
+```python
+from pathlib import Path
+
+import trattoria
+
+import matplotlib.pyplot as plt
+
+ptu_filepath = Path("/path/to/some.ptu")
+ptu = trattoria.PTUFile(ptu_filepath)
+
+timetrace_params = trattoria.TimeTraceParameters(
+    resolution=10.0,
+    channel=None,
+)
+tt_res = ptu.timetrace(timetrace_params)
+
+plt.plot(tt_res.t, tt_res.tt / timetrace_params.resolution)
+plt.xlabel("Time (s)")
+plt.ylabel("Intensity (Hz)")
+plt.show()
+```
+
+The examples folders contains examples of all the functionality available in
+Trattoria.  For more details check the docstrings in `core.py`.
+
+## Design
+Trattoria is just a very thin wrapper around the
+[trattoria-core](https://github.com/GCBallesteros/trattoria-core) library which
+itselfs provides a lower level interface to the the
+[tttr-toolbox](https://github.com/GCBallesteros/tttr-toolbox/tree/master/tttr-toolbox)
+library. A Rust project that provides the compiled components that allows us to
+go fast.
+
+## Changelog
+### 0.3.5
+- Bug fix. The last 1024\*16 where being ignored for performance reasons. This has
+  has been fixed upstream in `tttr-toolbox` and this version of Trattoria uses the
+  upgraded version of `trattoria-core`.
+- `trattoria-core` dropped support for Python 3.6 and 3.7 and therefore Trattoria too.
+
+### 0.3.4
+- The g2 algorithm now supports a mode flag. With "symmetric" we use the
+  prefered version of the algorithm that returns negative and positive delays.
+  "asymmetric" returns only positive delays but is faster. Default is
+  "symmetric".
+
+### 0.3.3
+- The underlying TTTR Toolbox and Trattoria Core were refactored to support
+  multiple custom ranges or records at once. `start_range` and `stop_range`
+  have disappeared in favor of `record_ranges`. It takes a list of tuples of
+  integers or `None`.
 
-packages = \
-['trattoria']
 
-package_data = \
-{'': ['*']}
+## Citing
 
-install_requires = \
-['numpy>=1.16', 'scipy>=1.5', 'trattoria-core==0.4.3']
-
-setup_kwargs = {
-    'name': 'trattoria',
-    'version': '0.3.4',
-    'description': 'The fastest streaming algorithms for your TTTR data',
-    'long_description': '# 🍕 Trattoria 🍕\nTrattoria delivers you the fastest streaming algorithms to analyze your TTTR data. We\ncurrenlty support the following algorithms:\n- __Second order autocorrelations__: Calculate the autocorrelation between two channels of\n  your TCSPC.\n- __Third Order autocorrelations__: Calculate the coincidences between 3 channels. A sync\nversion is provided were it uses the fact that the sync channel is periodic and known.\n- __Intensity time trace__: Calculate the intensity on each (or all) channels versus time.\n- __Zero finder__: Given two uncorrelated channels (e.g. a laser behind a 50/50 splitter)\n  compute the delay between the input channels.\n- __Lifetime__: Compute the lifetime histogram from a pulsed excitation experiment.\n\n## Supported file formats\nCurrently Trattoria can only read PTU files from PicoQuant. If you want support\nfor more or want to help providing it please put a ticket on the tttr-toolbox\nproject.\n\n## Installing\n```\npip install trattoria\n```\n\n## Examples\nThe entry point to Trattoria is the PTUFile class. This class has methods that\ngive us access to the algorithms. Each of the algorithms takes as input a\nparameter object and returns a results object. For a complete list of the\nfunctionality see the `examples` folder.\n\n```python\nimport trattoria\n\nimport matplotlib.pyplot as plt\n\nptu_filepath = Path("/path/to/some.ptu")\nptu = trattoria.PTUFile(ptu_filepath)\n\ntimetrace_params = trattoria.TimeTraceParameters(\n    resolution=10.0,\n    channel=None,\n)\ntt_res = ptu.timetrace(timetrace_params)\n\nplt.plot(tt_res.t, tt_res.tt / timetrace_params.resolution)\nplt.xlabel("Time (s)")\nplt.ylabel("Intensity (Hz)")\nplt.show()\n```\n\nThe examples folders contains examples of all the functionality available in\nTrattoria.  For more details check the docstrings in `core.py`.\n\n## Design\nTrattoria is just a very thin wrapper around the\n[trattoria-core](https://github.com/GCBallesteros/trattoria-core) library which\nitselfs provides a lower level interface to the the\n[tttr-toolbox](https://github.com/GCBallesteros/tttr-toolbox/tree/master/tttr-toolbox)\nlibrary. A Rust project that provides the compiled components that allows us to\ngo fast.\n\n## Changelog\n### 0.3.4\n- The g2 algorithm now supports a mode flag. With "symmetric" we use the\n  prefered version of the algorithm that returns negative and positive delays.\n  "asymmetric" returns only positive delays but is faster. Default is\n  "symmetric".\n\n### 0.3.3\n- The underlying TTTR Toolbox and Trattoria Core were refactored to support\n  multiple custom ranges or records at once. `start_range` and `stop_range`\n  have disappeared in favor of `record_ranges`. It takes a list of tuples of\n  integers or `None`.\n\n## Citing\n\n',
-    'author': 'Guillem Ballesteros',
-    'author_email': 'dev+pypi@maxwellrules.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/GCBallesteros/trattoria',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6',
-}
 
-
-setup(**setup_kwargs)
```

