# Comparing `tmp/seaborn_image-0.6.0.tar.gz` & `tmp/seaborn_image-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn_image-0.6.0.tar", max compression
+gzip compressed data, was "seaborn_image-0.7.0.tar", max compression
```

## Comparing `seaborn_image-0.6.0.tar` & `seaborn_image-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-05-04 01:15:10.718739 seaborn_image-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2755 2023-05-04 01:15:10.718739 seaborn_image-0.6.0/README.md
--rw-r--r--   0        0        0     1373 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      535 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_colormap.py
--rw-r--r--   0        0        0     7170 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_context.py
--rw-r--r--   0        0        0     8043 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_core.py
--rw-r--r--   0        0        0     2507 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_datasets.py
--rw-r--r--   0        0        0    11282 2023-05-04 01:15:10.918742 seaborn_image-0.6.0/src/seaborn_image/_filters.py
--rw-r--r--   0        0        0    19589 2023-05-04 01:15:10.922742 seaborn_image-0.6.0/src/seaborn_image/_general.py
--rw-r--r--   0        0        0    45585 2023-05-04 01:15:10.922742 seaborn_image-0.6.0/src/seaborn_image/_grid.py
--rw-r--r--   0        0        0     4523 2023-05-04 01:15:10.922742 seaborn_image-0.6.0/src/seaborn_image/utils.py
--rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 seaborn_image-0.6.0/setup.py
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 seaborn_image-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-14 19:42:53.900012 seaborn_image-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2755 2023-07-14 19:42:53.900012 seaborn_image-0.7.0/README.md
+-rw-r--r--   0        0        0     1373 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/__init__.py
+-rw-r--r--   0        0        0     2070 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_colormap.py
+-rw-r--r--   0        0        0     7170 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_context.py
+-rw-r--r--   0        0        0     8043 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_core.py
+-rw-r--r--   0        0        0     2507 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_datasets.py
+-rw-r--r--   0        0        0    11282 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_filters.py
+-rw-r--r--   0        0        0    19589 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_general.py
+-rw-r--r--   0        0        0    45585 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/_grid.py
+-rw-r--r--   0        0        0     4523 2023-07-14 19:42:54.124015 seaborn_image-0.7.0/src/seaborn_image/utils.py
+-rw-r--r--   0        0        0     3892 1970-01-01 00:00:00.000000 seaborn_image-0.7.0/setup.py
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 seaborn_image-0.7.0/PKG-INFO
```

### Comparing `seaborn_image-0.6.0/LICENSE.txt` & `seaborn_image-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/README.md` & `seaborn_image-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/pyproject.toml` & `seaborn_image-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaborn-image"
-version = "0.6.0"
+version = "0.7.0"
 description = "Attractive, descriptive and effective image visualization with seaborn-like API built on top of matplotlib"
 authors = ["Sarthak Jariwala <contact@sarthakjariwala.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/SarthakJariwala/seaborn-image"
 repository = "https://github.com/SarthakJariwala/seaborn-image"
 documentation = "https://seaborn-image.readthedocs.io/"
```

### Comparing `seaborn_image-0.6.0/src/seaborn_image/__init__.py` & `seaborn_image-0.7.0/src/seaborn_image/__init__.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_colormap.py` & `seaborn_image-0.7.0/src/seaborn_image/_colormap.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_context.py` & `seaborn_image-0.7.0/src/seaborn_image/_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,24 +95,24 @@
     --------
         >>> import seaborn_image as isns
         >>> isns.reset_defaults()
     """
     mpl.rcParams.update(mpl.rcParamsDefault)
 
 
-def set_image(cmap="deep", origin="lower", interpolation="nearest", despine=False):
+def set_image(cmap="deep", origin="upper", interpolation="nearest", despine=False):
     """
     Set deaults for plotting images
 
     Parameters
     ----------
     cmap : str, optional
         Colormap to use accross images, by default to "deep".
     origin : str, optional
-        Image origin - same as in `matplotlib.pyplot.imshow`, by default "lower".
+        Image origin - same as in `matplotlib.pyplot.imshow`, by default "upper".
     interpolation : str, optional
         Image interpolation - same as in `matplotlib.pyplot.imshow`, by default "nearest".
     despine : bool, optional
         Despine image and colorbar axes, by default False.
 
     Examples
     --------
```

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_core.py` & `seaborn_image-0.7.0/src/seaborn_image/_core.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_datasets.py` & `seaborn_image-0.7.0/src/seaborn_image/_datasets.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_filters.py` & `seaborn_image-0.7.0/src/seaborn_image/_filters.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_general.py` & `seaborn_image-0.7.0/src/seaborn_image/_general.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/_grid.py` & `seaborn_image-0.7.0/src/seaborn_image/_grid.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/src/seaborn_image/utils.py` & `seaborn_image-0.7.0/src/seaborn_image/utils.py`

 * *Files identical despite different names*

### Comparing `seaborn_image-0.6.0/setup.py` & `seaborn_image-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'scipy>=1.5.1']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=1.7.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'seaborn-image',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Attractive, descriptive and effective image visualization with seaborn-like API built on top of matplotlib',
     'long_description': '# seaborn-image: image data visualization\n\n[![Tests](https://github.com/SarthakJariwala/seaborn-image/workflows/Tests/badge.svg)](https://github.com/SarthakJariwala/seaborn-image/actions?workflow=Tests)\n[![Codecov](https://codecov.io/gh/SarthakJariwala/seaborn-image/branch/master/graph/badge.svg)](https://codecov.io/gh/SarthakJariwala/seaborn-image)\n[![PyPI](https://img.shields.io/pypi/v/seaborn-image.svg)](https://pypi.org/project/seaborn-image/)\n[![Documentation Status](https://readthedocs.org/projects/seaborn-image/badge/?version=latest)](https://seaborn-image.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n<div class="row">\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_image_hist.html">\n  <img src="./images/sphx_glr_plot_image_hist_001.png" height="120" width="170">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_filter.html">\n  <img src="./images/sphx_glr_plot_filter_001.png" height="120" width="130">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_fft.html">\n  <img src="./images/sphx_glr_plot_fft_001.png" height="120" width="120">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_filtergrid.html">\n  <img src="./images/sphx_glr_plot_filtergrid_001.png" height="120" width="120">\n  </a>\n\n  <a href="https://seaborn-image.readthedocs.io/en/latest/auto_examples/plot_image_robust.html">\n  <img src="./images/sphx_glr_plot_image_robust_001.png" height="120" width="260">\n  </a>\n\n</div>\n\n\n## Description\n\nSeaborn-image is a Python **image** visualization library based on matplotlib\nand provides a high-level API to **draw attractive and informative images quickly and effectively**.\n\nIt is heavily inspired by [seaborn](https://seaborn.pydata.org/), a high-level visualization library\nfor drawing attractive statistical graphics in Python.\n\n## Documentation\n\nDetailed documentation can be found [here](https://seaborn-image.readthedocs.io/).\n\n- [Tutorial](https://seaborn-image.readthedocs.io/en/latest/tutorial.html)\n- [Examples](https://seaborn-image.sarthakjariwala.com/en/latest/auto_examples/index.html)\n- [API Reference](https://seaborn-image.readthedocs.io/en/latest/reference.html)\n\n## Installation\n\nFor latest release:\n\nUsing `pip`\n\n```bash\npip install -U seaborn-image\n```\n\nUsing `conda`\n\n```bash\nconda install seaborn-image -c conda-forge\n```\n\nFor latest commit\n```bash\npip install git+https://github.com/SarthakJariwala/seaborn-image\n```\n\n## Contributing\n\nPlease see the [contributing guidelines](https://github.com/SarthakJariwala/seaborn-image/blob/master/CONTRIBUTING.rst)\n',
     'author': 'Sarthak Jariwala',
     'author_email': 'contact@sarthakjariwala.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/SarthakJariwala/seaborn-image',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['seaborn_image'] package_data = \ {'': ['*']}
 install_requires = \ ['matplotlib-scalebar>=0.7.0,<0.9.0', 'matplotlib>=3.2.2',
 'palettable>=3.3.0', 'pooch>=1.2.0', 'scikit-image>=0.17.2', 'scipy>=1.5.1']
 extras_require = \ {':python_version < "3.8"':
 ['importlib_metadata>=1.7.0,<2.0.0']} setup_kwargs = { 'name': 'seaborn-image',
-'version': '0.6.0', 'description': 'Attractive, descriptive and effective image
+'version': '0.7.0', 'description': 'Attractive, descriptive and effective image
 visualization with seaborn-like API built on top of matplotlib',
 'long_description': '# seaborn-image: image data visualization\n\n[![Tests]
 (https://github.com/SarthakJariwala/seaborn-image/workflows/Tests/badge.svg)]
 (https://github.com/SarthakJariwala/seaborn-image/actions?workflow=Tests)\n[!
 [Codecov](https://codecov.io/gh/SarthakJariwala/seaborn-image/branch/master/
 graph/badge.svg)](https://codecov.io/gh/SarthakJariwala/seaborn-image)\n[!
 [PyPI](https://img.shields.io/pypi/v/seaborn-image.svg)](https://pypi.org/
```

### Comparing `seaborn_image-0.6.0/PKG-INFO` & `seaborn_image-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-image
-Version: 0.6.0
+Version: 0.7.0
 Summary: Attractive, descriptive and effective image visualization with seaborn-like API built on top of matplotlib
 Home-page: https://github.com/SarthakJariwala/seaborn-image
 License: MIT
 Author: Sarthak Jariwala
 Author-email: contact@sarthakjariwala.com
 Requires-Python: >=3.8,<3.11
 Classifier: Framework :: Matplotlib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seaborn-image Version: 0.6.0 Summary: Attractive,
+Metadata-Version: 2.1 Name: seaborn-image Version: 0.7.0 Summary: Attractive,
 descriptive and effective image visualization with seaborn-like API built on
 top of matplotlib Home-page: https://github.com/SarthakJariwala/seaborn-image
 License: MIT Author: Sarthak Jariwala Author-email: contact@sarthakjariwala.com
 Requires-Python: >=3.8,<3.11 Classifier: Framework :: Matplotlib Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

