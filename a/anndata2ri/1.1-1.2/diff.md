# Comparing `tmp/anndata2ri-1.1.tar.gz` & `tmp/anndata2ri-1.2.tar.gz`

## Comparing `anndata2ri-1.1.tar` & `anndata2ri-1.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 anndata2ri-1.1/.gitignore
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 anndata2ri-1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 anndata2ri-1.1/.readthedocs.yml
--rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 anndata2ri-1.1/LICENSE
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 anndata2ri-1.1/README.rst
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 anndata2ri-1.1/demo.ipynb
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 anndata2ri-1.1/pyproject.toml
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 anndata2ri-1.1/pytest.ini
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 anndata2ri-1.1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 anndata2ri-1.1/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 anndata2ri-1.1/docs/Makefile
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 anndata2ri-1.1/docs/conf.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 anndata2ri-1.1/docs/index.rst
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 anndata2ri-1.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 anndata2ri-1.1/docs/ext/r_links.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/_version.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/conv.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/conv_name.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/py2r.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/r2py.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/rpy2_ext.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/test_utils.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/scipy2ri/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/scipy2ri/conv.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/scipy2ri/py2r.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/scipy2ri/r2py.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 anndata2ri-1.1/src/anndata2ri/scipy2ri/support.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 anndata2ri-1.1/tests/test_py2rpy.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 anndata2ri-1.1/tests/test_rpy2py.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 anndata2ri-1.1/tests/test_scipy_py2rpy.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 anndata2ri-1.1/tests/test_scipy_rpy2py.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 anndata2ri-1.1/.gitignore
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 anndata2ri-1.1/PKG-INFO
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 anndata2ri-1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 anndata2ri-1.2/.readthedocs.yml
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 anndata2ri-1.2/demo.ipynb
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 anndata2ri-1.2/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 anndata2ri-1.2/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 anndata2ri-1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 anndata2ri-1.2/docs/Makefile
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 anndata2ri-1.2/docs/conf.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 anndata2ri-1.2/docs/index.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 anndata2ri-1.2/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 anndata2ri-1.2/docs/ext/r_links.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/__init__.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/_conv.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/_conv_name.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/_py2r.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/_r2py.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/_rpy2_ext.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/py.typed
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/test_utils.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/scipy2ri/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/scipy2ri/_conv.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/scipy2ri/_py2r.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/scipy2ri/_py2r_helpers.r
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/scipy2ri/_r2py.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 anndata2ri-1.2/src/anndata2ri/scipy2ri/_support.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 anndata2ri-1.2/tests/conftest.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 anndata2ri-1.2/tests/test_py2rpy.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 anndata2ri-1.2/tests/test_rpy2py.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 anndata2ri-1.2/tests/test_scipy_py2rpy.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 anndata2ri-1.2/tests/test_scipy_rpy2py.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 anndata2ri-1.2/.gitignore
+-rw-r--r--   0        0        0    32422 2020-02-02 00:00:00.000000 anndata2ri-1.2/LICENSE
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 anndata2ri-1.2/README.rst
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 anndata2ri-1.2/pyproject.toml
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 anndata2ri-1.2/PKG-INFO
```

### Comparing `anndata2ri-1.1/LICENSE` & `anndata2ri-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anndata2ri-1.1/README.rst` & `anndata2ri-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `anndata2ri-1.1/demo.ipynb` & `anndata2ri-1.2/demo.ipynb`

 * *Files identical despite different names*

### Comparing `anndata2ri-1.1/.github/workflows/deploy.yml` & `anndata2ri-1.2/.github/workflows/deploy.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 name: Publish Python 🐍 distributions 📦 to PyPI
 
 on:
   push:
     branches:
-      - 'master'
-      - 'test_deploy'
+    - 'main'
+    - 'test_deploy'
     tags:
-      - '*'
+    - '*'
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@master
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0  # allow deriving correct version from git tags
 
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v2
+    - name: Set up Python 3.11
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.7
+        python-version: 3.11
+        cache: pip
 
     - name: Install pypa/build
       run: >-
         python -m
         pip install
         build
```

### Comparing `anndata2ri-1.1/docs/conf.py` & `anndata2ri-1.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
+"""Sphinx configuration."""
+
 import sys
 from abc import ABC
-from datetime import datetime
+from datetime import datetime, timezone
+from importlib.metadata import metadata
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 
-try:
-    from importlib.metadata import metadata
-except ImportError:
-    from importlib_metadata import metadata
-
-
-def mock_rpy2():
-    # Can’t use autodoc_mock_imports as we import anndata2ri
+def mock_rpy2() -> None:
+    """Can’t use autodoc_mock_imports as we import anndata2ri."""
     patch('rpy2.situation.get_r_home', lambda: None).start()
     sys.modules['rpy2.rinterface_lib'] = MagicMock()
     submods = ['embedded', 'conversion', 'memorymanagement', 'sexp', 'bufferprotocol', 'callbacks', '_rinterface_capi']
     sys.modules.update({f'rpy2.rinterface_lib.{sub}': MagicMock() for sub in submods})
     sexp = sys.modules['rpy2.rinterface_lib'].sexp = sys.modules['rpy2.rinterface_lib.sexp']
     sexp.Sexp = type('Sexp', (MagicMock, ABC), dict(__module__='rpy2.rinterface_lib.sexp'))
     sexp.SexpEnvironment = type('SexpEnvironment', (sexp.Sexp,), dict(__module__='rpy2.rinterface_lib.sexp'))
     sexp.SexpVector = sexp.StrSexpVector = MagicMock
     sexp.SexpVector.from_iterable = MagicMock()
 
     import rpy2.rinterface
     import rpy2.rinterface_lib.sexp
 
     rpy2.rinterface_lib = sys.modules['rpy2.rinterface_lib']
-    rpy2.rinterface._MissingArgType = object
+    rpy2.rinterface._MissingArgType = object  # noqa: SLF001
     rpy2.rinterface.initr_simple = lambda *_, **__: None
 
     assert rpy2.rinterface_lib.sexp is sexp
 
 
 HERE = Path(__file__).parent
 
@@ -44,23 +41,22 @@
 # -- General configuration ------------------------------------------------
 
 
 # General information
 project = 'anndata2ri'
 meta = metadata(project)
 author = meta['author-email'].split('"')[1]
-copyright = f'{datetime.now():%Y}, {author}.'
+copyright = f'{datetime.now(tz=timezone.utc):%Y}, {author}.'  # noqa: A001
 version = meta['version']
 release = version
 
 # default settings
 templates_path = ['_templates']
 source_suffix = '.rst'
 master_doc = 'index'
-# default_role = '?'
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 pygments_style = 'sphinx'
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx.ext.autosummary',
@@ -96,15 +92,15 @@
 html_theme_options = dict(collapse_navigation=True)
 html_static_path = ['_static']
 html_css_files = ['css/custom.css']
 html_context = dict(
     display_github=True,
     github_user='theislab',
     github_repo='anndata2ri',
-    github_version='master',
+    github_version='main',
     conf_py_path='/docs/',
 )
 
 
 # -- Options for other output formats ------------------------------------------
```

### Comparing `anndata2ri-1.1/src/anndata2ri/__init__.py` & `anndata2ri-1.2/src/anndata2ri/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-r"""
-Converter between Python’s AnnData and R’s SingleCellExperiment.
-
+r"""Converter between Python’s AnnData and R’s SingleCellExperiment.
 
 ==========================================================  =  ========================================================
 :rcls:`~SingleCellExperiment::SingleCellExperiment`            :class:`~anndata.AnnData`
 ==========================================================  =  ========================================================
 :rman:`~SummarizedExperiment::assay`\ ``(d, 'X')``          ⇄  ``d.``\ :attr:`~anndata.AnnData.X`
 :rman:`~SummarizedExperiment::assay`\ ``(d, 'counts')``     ⇄  ``d.``\ :attr:`~anndata.AnnData.layers`\ ``['counts']``
 :rman:`~SummarizedExperiment::colData`\ ``(d)``             ⇄  ``d.``\ :attr:`~anndata.AnnData.obs`
 :rman:`~SummarizedExperiment::rowData`\ ``(d)``             ⇄  ``d.``\ :attr:`~anndata.AnnData.var`
 :rman:`~S4Vectors::metadata`\ ``(d)``                       ⇄  ``d.``\ :attr:`~anndata.AnnData.uns`
 :rman:`~SingleCellExperiment::reducedDim`\ ``(d, 'PCA')``   ⇄  ``d.``\ :attr:`~anndata.AnnData.obsm`\ ``['X_pca']``
 :rman:`~SingleCellExperiment::reducedDim`\ ``(d, 'DM')``    ⇄  ``d.``\ :attr:`~anndata.AnnData.obsm`\ ``['X_diffmap']``
 ==========================================================  =  ========================================================
 """
-__all__ = ['activate', 'deactivate', 'py2rpy', 'rpy2py', 'converter']
+from __future__ import annotations
 
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING
+
+from . import _py2r, _r2py  # noqa: F401
+from ._conv import activate, converter, deactivate
 
-from rpy2.rinterface import Sexp
 
-from . import py2r, r2py
-from .conv import activate, converter, deactivate
+if TYPE_CHECKING:
+    from anndata import AnnData
+    from pandas import DataFrame
+    from rpy2.rinterface import Sexp
 
 
+__all__ = ['__version__', 'activate', 'deactivate', 'py2rpy', 'rpy2py', 'converter']
+
 HERE = Path(__file__).parent
 
 __author__ = 'Philipp Angerer'
 try:
     from setuptools_scm import get_version
 
     __version__ = get_version(str(HERE.parent.parent))
 except (ImportError, LookupError):
     try:
         from ._version import __version__
-    except ImportError:
-        raise ImportError('Cannot infer version. Make sure to `pip install` the project or install `setuptools-scm`.')
+    except ImportError as e:
+        msg = 'Cannot infer version. Make sure to `pip install` the project or install `setuptools-scm`.'
+        raise ImportError(msg) from e
 
 
-def py2rpy(obj: Any) -> Sexp:
-    """
-    Convert Python objects to R interface objects. Supports:
+def py2rpy(obj: AnnData) -> Sexp:
+    """Convert Python objects to R interface objects.
+
+    Supports:
 
     - :class:`~anndata.AnnData` → :rcls:`~SingleCellExperiment::SingleCellExperiment`
     """
     return converter.py2rpy(obj)
 
 
-def rpy2py(obj: Any) -> Sexp:
-    """
-    Convert R interface objects to Python objects. Supports:
+def rpy2py(obj: Sexp) -> AnnData | DataFrame:
+    """Convert R interface objects to Python objects.
+
+    Supports:
 
     - :rcls:`~SingleCellExperiment::SingleCellExperiment` → :class:`~anndata.AnnData`
     - :rcls:`S4Vectors::DataFrame` → :class:`pandas.DataFrame`
     """
     return converter.rpy2py(obj)
```

### Comparing `anndata2ri-1.1/src/anndata2ri/conv_name.py` & `anndata2ri-1.2/src/anndata2ri/_conv_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+
 dimension_reductions = {
     'pca',
     'dca',
     'tsne',  # There’s both tSNE and TSNE: https://rdrr.io/bioc/singleCellTK/man/getPCA.html
     'umap',
     ('diffmap', 'dm'),  # X_diffmap is the official scanpy name
     'magic',
```

### Comparing `anndata2ri-1.1/src/anndata2ri/py2r.py` & `anndata2ri-1.2/src/anndata2ri/_py2r.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,73 @@
+from __future__ import annotations
+
 from collections.abc import Mapping
+from typing import TYPE_CHECKING
 from warnings import warn
 
 import numpy as np
-import pandas as pd
 from anndata import AnnData
 from rpy2.robjects import conversion, default_converter, pandas2ri
 from rpy2.robjects.conversion import localconverter
-from rpy2.robjects.methods import RS4
 from rpy2.robjects.vectors import ListVector
 
-from . import conv_name
-from .conv import converter, full_converter, mat_converter
-from .rpy2_ext import importr
+from . import _conv_name
+from ._conv import converter, full_converter, mat_py2rpy
+from ._rpy2_ext import importr
+
+
+if TYPE_CHECKING:
+    import pandas as pd
+    from rpy2.robjects.methods import RS4
 
 
 class NotConvertedWarning(Warning):
-    pass
+    """A warning for elements that have not been converted."""
 
 
 dict_converter = conversion.Converter('Converter handling dicts')
 dict_converter.py2rpy.register(np.bool_, lambda x: conversion.py2rpy(bool(x)))
 dict_converter.py2rpy.register(np.int_, lambda x: conversion.py2rpy(int(x)))
 dict_converter.py2rpy.register(np.float_, lambda x: conversion.py2rpy(float(x)))
 dict_converter.py2rpy.register(np.bytes_, lambda x: conversion.py2rpy(bytes(x)))
 dict_converter.py2rpy.register(np.str_, lambda x: conversion.py2rpy(str(x)))
 
 
+# TODO(flying-sheep): #111 set stacklevel
+# https://github.com/theislab/anndata2ri/issues/111
+STACK_LEVEL = 2
+
+
 @dict_converter.py2rpy.register(Mapping)
 def py2rpy_dict(obj: Mapping) -> ListVector:
-    """Try converting everything. For nested dicts, this needs itself to be registered"""
+    """Try converting everything. For nested dicts, this needs itself to be registered."""
     converted = {}
-    for k, v in obj.items():
-        try:
+    try:
+        for k, v in obj.items():
             converted[str(k)] = conversion.py2rpy(v)
-        except NotImplementedError as e:
-            warn(str(e), NotConvertedWarning)
+    except NotImplementedError as e:
+        warn(str(e), NotConvertedWarning, stacklevel=STACK_LEVEL)
     # This tries to convert everything again. This works because py2rpy(Sexp) is the identity function
     return ListVector(converted)
 
 
 def check_no_dupes(idx: pd.Index, name: str) -> bool:
     dupes = idx.duplicated().any()
     if dupes:
-        warn(f'Duplicated {name}: {idx[idx.duplicated(False)].sort_values()}')
+        warn(f'Duplicated {name}: {idx[idx.duplicated(keep=False)].sort_values()}', stacklevel=STACK_LEVEL + 1)
     return not dupes
 
 
 @converter.py2rpy.register(AnnData)
 def py2rpy_anndata(obj: AnnData) -> RS4:
     with localconverter(default_converter):
         s4v = importr('S4Vectors')
         sce = importr('SingleCellExperiment')
-        # TODO: sparse
-        x = {} if obj.X is None else dict(X=mat_converter.py2rpy(obj.X.T))
-        layers = {k: mat_converter.py2rpy(v.T) for k, v in obj.layers.items()}
+        x = {} if obj.X is None else dict(X=mat_py2rpy(obj.X.T))
+        layers = {k: mat_py2rpy(v.T) for k, v in obj.layers.items()}
         assays = ListVector({**x, **layers})
 
         row_args = {k: pandas2ri.py2rpy(v) for k, v in obj.var.items()}
         if check_no_dupes(obj.var_names, 'var_names'):
             row_args['row.names'] = pandas2ri.py2rpy(obj.var_names)
         row_data = s4v.DataFrame(**row_args)
 
@@ -66,13 +76,13 @@
             col_args['row.names'] = pandas2ri.py2rpy(obj.obs_names)
         col_data = s4v.DataFrame(**col_args)
 
         # Convert everything we know
         with localconverter(full_converter() + dict_converter):
             metadata = ListVector(obj.uns.items())
 
-        rd_args = {conv_name.scanpy2sce(k): mat_converter.py2rpy(obj.obsm[k]) for k in obj.obsm.keys()}
+        rd_args = {_conv_name.scanpy2sce(k): mat_py2rpy(obj.obsm[k]) for k in obj.obsm}
         reduced_dims = s4v.SimpleList(**rd_args)
 
         return sce.SingleCellExperiment(
             assays=assays, rowData=row_data, colData=col_data, metadata=metadata, reducedDims=reduced_dims
         )
```

### Comparing `anndata2ri-1.1/src/anndata2ri/r2py.py` & `anndata2ri-1.2/src/anndata2ri/_r2py.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,61 @@
-from typing import Optional, Union
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
 
-import numpy as np
 import pandas as pd
 from anndata import AnnData
 from rpy2.rinterface import IntSexpVector, NULLType, Sexp, SexpS4, baseenv
-from rpy2.robjects import default_converter, numpy2ri, pandas2ri
+from rpy2.robjects import RS4, default_converter, numpy2ri, pandas2ri
 from rpy2.robjects.conversion import localconverter
 from rpy2.robjects.robject import RSlots
 
-from . import conv_name
-from .conv import converter, full_converter, mat_converter
-from .rpy2_ext import importr
+from . import _conv_name
+from ._conv import converter, full_converter, mat_rpy2py
+from ._rpy2_ext import importr
 from .scipy2ri import supported_r_matrix_classes
-from .scipy2ri.r2py import rmat_to_spmat
+from .scipy2ri._r2py import rmat_to_spmat
+
+
+if TYPE_CHECKING:
+    from collections.abc import Mapping
+
+    import numpy as np
+    from scipy.sparse import spmatrix
+
+
+R_INT_BYTES = 4
 
 
 @converter.rpy2py.register(SexpS4)
-def rpy2py_s4(obj: SexpS4) -> Optional[Union[pd.DataFrame, AnnData]]:
-    """
+def rpy2py_s4(obj: SexpS4) -> pd.DataFrame | AnnData | None:
+    """Convert known S4 class instance to Python object.
+
     See here for the slots: https://bioconductor.org/packages/release/bioc/vignettes/SingleCellExperiment/inst/doc/intro.html
     """
     r_classes = set(obj.rclass)
     if {'DataFrame', 'DFrame'} & r_classes:
         return rpy2py_data_frame(obj)
-    elif 'SingleCellExperiment' in r_classes:
+    if 'SingleCellExperiment' in r_classes:
         return rpy2py_single_cell_experiment(obj)
-    elif supported_r_matrix_classes() & r_classes:
+    if supported_r_matrix_classes() & r_classes:
         return rmat_to_spmat(obj)
-    else:  # Don’t use the registered one, it would lead to recursion.
-        return default_converter.rpy2py(obj)
+    # Don’t use the registered one, it would lead to recursion.
+    return default_converter.rpy2py(obj)
 
 
-def rpy2py_vector(v):
-    """
-    Converts vectors. Also handles NA in int vectors: https://github.com/rpy2/rpy2/issues/376
+def rpy2py_vector(v: Sexp) -> Any:  # noqa: ANN401
+    """Convert R vector to Python vectors.
+
+    Also handles NA in int vectors: https://github.com/rpy2/rpy2/issues/376
     """
     if not isinstance(v, Sexp):
         return v
     if isinstance(v, IntSexpVector):
-        assert v._R_SIZEOF_ELT == 4, 'R integer size changed away from 32 bit'
+        assert v._R_SIZEOF_ELT == R_INT_BYTES, 'R integer size changed away from 32 bit'  # noqa: SLF001
         r = pd.array(v, dtype=pd.Int32Dtype())
         v_is_na = numpy2ri.rpy2py(baseenv['is.na'](v)).astype(bool)
         if 'factor' in v.rclass:
             levels = numpy2ri.rpy2py(baseenv['levels'](v))
             codes = r.to_numpy() - 1
             # temporarily set NA values to a valid index
             codes[v_is_na] = 0
@@ -50,17 +63,15 @@
             r = pd.array(levels[codes], dtype=pd.CategoricalDtype(levels))
         r[v_is_na] = pd.NA
         return r
     return pandas2ri.rpy2py(v)
 
 
 def rpy2py_data_frame(obj: SexpS4) -> pd.DataFrame:
-    """
-    S4 DataFrame class, not data.frame
-    """
+    """S4 DataFrame class, not data.frame."""
     slots = RSlots(obj)
     with localconverter(default_converter):
         columns = {k: rpy2py_vector(v) for k, v in slots['listData'].items()}
         rownames = slots['rownames']
         if isinstance(rownames, NULLType):
             rownames = pd.RangeIndex(slots['nrows'][0])
 
@@ -69,38 +80,50 @@
 
 def rpy2py_single_cell_experiment(obj: SexpS4) -> AnnData:
     with localconverter(default_converter):
         s4v = importr('S4Vectors')
         se = importr('SummarizedExperiment')
         sce = importr('SingleCellExperiment')
 
+        def convert_mats(
+            attr: str, mats: Mapping[str, Sexp], *, transpose: bool = False
+        ) -> list[np.ndarray | spmatrix]:
+            rv = []
+            for n, mat in mats.items():
+                conv = mat_rpy2py(mat)
+                if isinstance(conv, RS4):
+                    cls_names = mat_rpy2py(conv.slots['class']).tolist()
+                    msg = f'Cannot convert {attr} “{n}” of type(s) {cls_names} to Python'
+                    raise TypeError(msg)
+                rv.append(conv.T if transpose else conv)
+            return rv
+
         assay_names = se.assayNames(obj)
         if not isinstance(assay_names, NULLType):
             assay_names = [str(a) for a in se.assayNames(obj)]
             # The assays can be stored in an env or elsewise so we don’t use obj.slots['assays']
-            assays = [mat_converter.rpy2py(assay).T for assay in (se.assay(obj, n) for n in assay_names)]
+            assays = convert_mats('assay', {n: se.assay(obj, n) for n in assay_names}, transpose=True)
             # There’s SingleCellExperiment with no assays
             exprs, layers = assays[0], dict(zip(assay_names[1:], assays[1:]))
-            assert len(exprs.shape) == 2, exprs.shape
+            assert len(exprs.shape) == 2, exprs.shape  # noqa: PLR2004
         else:
             exprs, layers = None, {}
 
         rdim_names = sce.reducedDimNames(obj)
         if not isinstance(rdim_names, NULLType):
             rdim_names = [str(t) for t in rdim_names]
-            reduced_dims = [mat_converter.rpy2py(rd) for rd in (sce.reducedDim(obj, t) for t in rdim_names)]
-            obsm = {conv_name.sce2scanpy(n): d for n, d in zip(rdim_names, reduced_dims)}
+            reduced_dims = convert_mats('reducedDim', {t: sce.reducedDim(obj, t) for t in rdim_names})
+            obsm = {_conv_name.sce2scanpy(n): d for n, d in zip(rdim_names, reduced_dims)}
         else:
             obsm = None
 
         col_data = se.colData(obj)
         row_data = se.rowData(obj)
         metadata = s4v.metadata(obj)
 
     obs = rpy2py_data_frame(col_data)
     var = rpy2py_data_frame(row_data)
     # The whole shebang: configured converter, numpy, pandas and ours
     with localconverter(full_converter()):
         uns = dict(metadata.items())
 
-    # TODO: Once the AnnData bug is fixed, remove the “or None”
-    return AnnData(exprs, obs, var, uns, obsm or None, layers=layers)
+    return AnnData(exprs, obs, var, uns, obsm, layers=layers)
```

### Comparing `anndata2ri-1.1/src/anndata2ri/scipy2ri/__init__.py` & `anndata2ri-1.2/src/anndata2ri/scipy2ri/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-r"""
-Convert scipy.sparse matrices between Python and R.
+r"""Convert scipy.sparse matrices between Python and R.
 
 For a detailed comparison between the two languages’
 sparse matrix environment, see `issue #8`_.
 
 .. _issue #8: https://github.com/flying-sheep/anndata2ri/issues/8
 
 Here’s an overview over the matching classes
@@ -17,61 +16,68 @@
 :rcls:`~Matrix::lgRMatrix`/:rcls:`~Matrix::ngRMatrix`  :class:`~scipy.sparse.csr_matrix`\ ``(dtype=bool)``
 :rcls:`~Matrix::dgTMatrix`                             :class:`~scipy.sparse.coo_matrix`\ ``(dtype=float64)``
 :rcls:`~Matrix::lgTMatrix`/:rcls:`~Matrix::ngTMatrix`  :class:`~scipy.sparse.coo_matrix`\ ``(dtype=bool)``
 :rcls:`~Matrix::ddiMatrix`                             :class:`~scipy.sparse.dia_matrix`\ ``(dtype=float64)``
 :rcls:`~Matrix::ldiMatrix`                             :class:`~scipy.sparse.dia_matrix`\ ``(dtype=bool)``
 =====================================================  ======================================================
 """
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from . import _py2r, _r2py  # noqa: F401
+from ._conv import activate, converter, deactivate
+from ._support import supported_r_matrix_classes, supported_r_matrix_storage, supported_r_matrix_types
+
+
+if TYPE_CHECKING:
+    from rpy2.rinterface import Sexp
+    from scipy import sparse
+
+
 __all__ = [
     'activate',
     'deactivate',
     'py2rpy',
     'rpy2py',
     'converter',
     'supported_r_matrix_types',
     'supported_r_matrix_storage',
     'supported_r_matrix_classes',
 ]
 
 
-from typing import Any
-
-from rpy2.rinterface import Sexp
-
-from . import py2r, r2py
-from .conv import activate, converter, deactivate
-from .support import supported_r_matrix_classes, supported_r_matrix_storage, supported_r_matrix_types
-
-
 supported_r_matrix_types = supported_r_matrix_types
 """The Matrix data types supported by this module; Double, Logical, and patterN."""
 
 supported_r_matrix_storage = supported_r_matrix_storage
 """The Matrix storage types supported by this module; Column-sparse, Row-Sparse, Triplets, and DIagonal."""
 
 
-def py2rpy(obj: Any) -> Sexp:
-    """
-    Convert scipy sparse matrices objects to R sparse matrices. Supports:
+def py2rpy(obj: sparse.spmatrix) -> Sexp:
+    """Convert scipy sparse matrices objects to R sparse matrices.
+
+    Supports:
 
     :class:`~scipy.sparse.csc_matrix` (dtype in {float32, float64, bool}) →
         :rcls:`~Matrix::dgCMatrix` or :rcls:`~Matrix::lgCMatrix`
     :class:`~scipy.sparse.csr_matrix` (dtype in {float32, float64, bool}) →
         :rcls:`~Matrix::dgRMatrix` or :rcls:`~Matrix::lgRMatrix`
     :class:`~scipy.sparse.coo_matrix` (dtype in {float32, float64, bool}) →
         :rcls:`~Matrix::dgTMatrix` or :rcls:`~Matrix::lgTMatrix`
     :class:`~scipy.sparse.dia_matrix` (dtype in {float32, float64, bool}) →
         :rcls:`~Matrix::ddiMatrix` or :rcls:`~Matrix::ldiMatrix`
     """
     return converter.py2rpy(obj)
 
 
-def rpy2py(obj: Any) -> Sexp:
-    """
-    Convert R sparse matrices to scipy sparse matrices. Supports:
+def rpy2py(obj: Sexp) -> sparse.spmatrix:
+    """Convert R sparse matrices to scipy sparse matrices.
+
+    Supports:
 
     :rcls:`~Matrix::dgCMatrix`, :rcls:`~Matrix::lgCMatrix`, or :rcls:`~Matrix::ngCMatrix` →
         :class:`~scipy.sparse.csc_matrix` (dtype float64 or bool)
     :rcls:`~Matrix::dgRMatrix`, :rcls:`~Matrix::lgRMatrix`, or :rcls:`~Matrix::ngRMatrix` →
         :class:`~scipy.sparse.csr_matrix` (dtype float64 or bool)
     :rcls:`~Matrix::dgTMatrix`, :rcls:`~Matrix::lgTMatrix`, or :rcls:`~Matrix::ngTMatrix` →
         :class:`~scipy.sparse.coo_matrix` (dtype float64 or bool)
```

### Comparing `anndata2ri-1.1/src/anndata2ri/scipy2ri/conv.py` & `anndata2ri-1.2/src/anndata2ri/_conv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,79 @@
-from typing import Optional
+from __future__ import annotations
 
-from rpy2.robjects import conversion, numpy2ri
+from typing import TYPE_CHECKING
+
+import numpy as np
+import pandas as pd
+from rpy2.robjects import conversion, numpy2ri, pandas2ri
 from rpy2.robjects.conversion import overlay_converter
 
+from . import scipy2ri
 
-original_converter: Optional[conversion.Converter] = None
-converter = conversion.Converter('original scipy conversion')
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
 
-def activate():
-    """
-    Activate conversion between sparse matrices from Scipy and R’s Matrix package.
+    from rpy2.rinterface import Sexp
+    from scipy.sparse import spmatrix
 
-    Does nothing if this is the active conversion.
-    """
-    global original_converter
 
-    if original_converter is not None:
-        return
+original_converter: conversion.Converter | None = None
+converter = conversion.Converter('original anndata conversion')
+
+_mat_converter = numpy2ri.converter + scipy2ri.converter
+
+
+def mat_py2rpy(obj: np.ndarray | spmatrix | pd.DataFrame) -> Sexp:
+    if isinstance(obj, pd.DataFrame):
+        numeric_cols = obj.dtypes <= np.number
+        if not numeric_cols.all():
+            non_num = numeric_cols.index[~numeric_cols]
+            msg = f'DataFrame contains non-numeric columns {list(non_num)}'
+            raise ValueError(msg)
+        obj = obj.to_numpy()
+    return _mat_converter.py2rpy(obj)
+
+
+mat_rpy2py: Callable[[Sexp], np.ndarray | spmatrix | Sexp] = _mat_converter.rpy2py
 
-    original_converter = conversion.converter
 
-    numpy2ri.activate()
-    new_converter = conversion.Converter('scipy conversion', template=conversion.converter)
-    numpy2ri.deactivate()
+def full_converter() -> conversion.Converter:
+    pandas2ri.activate()
+    new_converter = conversion.Converter('anndata conversion', template=conversion.get_conversion())
+    pandas2ri.deactivate()
 
+    overlay_converter(scipy2ri.converter, new_converter)
+    # overwrite the scipy2ri Sexp4 converter and add our others
     overlay_converter(converter, new_converter)
 
+    return new_converter
+
+
+def activate() -> None:
+    r"""Activate conversion for supported objects.
+
+    This includes :class:`~anndata.AnnData` objects
+    as well as :ref:`numpy:arrays` and :class:`pandas.DataFrame`\ s
+    via ``rpy2.robjects.numpy2ri`` and ``rpy2.robjects.pandas2ri``.
+
+    Does nothing if this is the active converter.
+    """
+    global original_converter  # noqa: PLW0603
+
+    if original_converter is not None:
+        return
+
+    new_converter = full_converter()
+    original_converter = conversion.get_conversion()
     conversion.set_conversion(new_converter)
 
 
-def deactivate():
+def deactivate() -> None:
     """Deactivate the conversion described above if it is active."""
-    global original_converter
+    global original_converter  # noqa: PLW0603
 
     if original_converter is None:
         return
 
     conversion.set_conversion(original_converter)
     original_converter = None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anndata2ri-1.1/src/anndata2ri/scipy2ri/py2r.py` & `anndata2ri-1.2/src/anndata2ri/scipy2ri/_py2r.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,119 @@
-from functools import wraps
-from typing import Callable, Optional
+from __future__ import annotations
+
+from functools import lru_cache, wraps
+from typing import TYPE_CHECKING
+
+
+try:
+    from importlib.resources import files
+except ImportError:  # Python < 3.9
+    from importlib_resources import files
 
 import numpy as np
-from rpy2.rinterface import Sexp
 from rpy2.robjects import default_converter, numpy2ri
 from rpy2.robjects.conversion import localconverter
 from rpy2.robjects.packages import Package, SignatureTranslatedAnonymousPackage
 from scipy import sparse
 
-from ..rpy2_ext import importr
-from .conv import converter
+from anndata2ri._rpy2_ext import importr
+
+from ._conv import converter
+
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
 
-matrix: Optional[SignatureTranslatedAnonymousPackage] = None
-base: Optional[Package] = None
+    from rpy2.rinterface import Sexp
+
+
+matrix: SignatureTranslatedAnonymousPackage | None = None
+base: Package | None = None
+
+
+@lru_cache
+def get_r_code() -> str:
+    return files('anndata2ri').joinpath('scipy2ri', '_py2r_helpers.r').read_text()
 
 
 def get_type_conv(dtype: np.dtype) -> Callable[[np.ndarray], Sexp]:
-    global base
+    global base  # noqa: PLW0603
     if base is None:
         base = importr('base')
     if np.issubdtype(dtype, np.floating):
         return base.as_double
-    elif np.issubdtype(dtype, np.bool_):
+    if np.issubdtype(dtype, np.bool_):
         return base.as_logical
-    else:
-        raise ValueError(f'Unknown dtype {dtype!r} cannot be converted to ?gRMatrix.')
+    msg = f'Unknown dtype {dtype!r} cannot be converted to ?gRMatrix.'
+    raise ValueError(msg)
+
 
+def py2r_context(f: Callable[[sparse.spmatrix], Sexp]) -> Callable[[sparse.spmatrix], Sexp]:
+    """R globalenv context with some helper functions."""
 
-def py2r_context(f):
     @wraps(f)
-    def wrapper(obj):
-        global as_logical, as_integer, as_double, matrix
+    def wrapper(obj: sparse.spmatrix) -> Sexp:
+        global matrix  # noqa: PLW0603
         if matrix is None:
             importr('Matrix')  # make class available
-            matrix = SignatureTranslatedAnonymousPackage(
-                """
-                sparse_matrix <- function(x, conv_data, dims, ...) {
-                    Matrix::sparseMatrix(
-                        ...,
-                        x=conv_data(x),
-                        dims=as.integer(dims),
-                        index1=FALSE
-                    )
-                }
-
-                from_csc <- function(i, p, x, dims, conv_data) {
-                    sparse_matrix(
-                        i=as.integer(i),
-                        p=as.integer(p),
-                        x=x,
-                        conv_data=conv_data,
-                        dims=dims,
-                        repr="C"
-                    )
-                }
-
-                from_csr <- function(j, p, x, dims, conv_data) {
-                    sparse_matrix(
-                        j=as.integer(j),
-                        p=as.integer(p),
-                        x=x,
-                        conv_data=conv_data,
-                        dims=dims,
-                        repr="R"
-                    )
-                }
-
-                from_coo <- function(i, j, x, dims, conv_data) {
-                    sparse_matrix(
-                        i=as.integer(i),
-                        j=as.integer(j),
-                        x=x,
-                        conv_data=conv_data,
-                        dims=dims,
-                        repr="T"
-                    )
-                }
-
-                from_dia <- function(n, x, conv_data) {
-                    Matrix::Diagonal(n=as.integer(n), x=conv_data(x))
-                }
-                """,
-                'matrix',
-            )
+            r_code = get_r_code()
+            matrix = SignatureTranslatedAnonymousPackage(r_code, 'matrix')
 
         return f(obj)
 
     return wrapper
 
 
 @converter.py2rpy.register(sparse.csc_matrix)
 @py2r_context
-def csc_to_rmat(csc: sparse.csc_matrix):
+def csc_to_rmat(csc: sparse.csc_matrix) -> Sexp:
     csc.sort_indices()
     conv_data = get_type_conv(csc.dtype)
     with localconverter(default_converter + numpy2ri.converter):
         return matrix.from_csc(i=csc.indices, p=csc.indptr, x=csc.data, dims=list(csc.shape), conv_data=conv_data)
 
 
 @converter.py2rpy.register(sparse.csr_matrix)
 @py2r_context
-def csr_to_rmat(csr: sparse.csr_matrix):
+def csr_to_rmat(csr: sparse.csr_matrix) -> Sexp:
     csr.sort_indices()
     conv_data = get_type_conv(csr.dtype)
     with localconverter(default_converter + numpy2ri.converter):
         return matrix.from_csr(
             j=csr.indices,
             p=csr.indptr,
             x=csr.data,
             conv_data=conv_data,
             dims=list(csr.shape),
         )
 
 
 @converter.py2rpy.register(sparse.coo_matrix)
 @py2r_context
-def coo_to_rmat(coo: sparse.coo_matrix):
+def coo_to_rmat(coo: sparse.coo_matrix) -> Sexp:
     conv_data = get_type_conv(coo.dtype)
     with localconverter(default_converter + numpy2ri.converter):
         return matrix.from_coo(
             i=coo.row,
             j=coo.col,
             x=coo.data,
             conv_data=conv_data,
             dims=list(coo.shape),
         )
 
 
 @converter.py2rpy.register(sparse.dia_matrix)
 @py2r_context
-def dia_to_rmat(dia: sparse.dia_matrix):
+def dia_to_rmat(dia: sparse.dia_matrix) -> Sexp:
     conv_data = get_type_conv(dia.dtype)
     if len(dia.offsets) > 1:
-        raise ValueError(
+        msg = (
             'Cannot convert a dia_matrix with more than 1 diagonal to a *diMatrix. '
             f'R diagonal matrices only support 1 diagonal, but this has {len(dia.offsets)}.'
         )
+        raise ValueError(msg)
     with localconverter(default_converter + numpy2ri.converter):
         return matrix.from_dia(
             n=dia.shape[0],
             x=dia.data,
             conv_data=conv_data,
         )
```

### Comparing `anndata2ri-1.1/src/anndata2ri/scipy2ri/r2py.py` & `anndata2ri-1.2/src/anndata2ri/scipy2ri/_r2py.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,66 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 from warnings import warn
 
 import numpy as np
 from rpy2.rinterface import NULL, SexpS4
 from rpy2.robjects import baseenv, default_converter, numpy2ri
 from rpy2.robjects.conversion import localconverter
 from rpy2.robjects.robject import RSlots
 from scipy import sparse
 
-from .conv import converter
-from .support import supported_r_matrix_classes
+from ._conv import converter
+from ._support import SupportedMatStor, supported_r_matrix_classes
+
+
+if TYPE_CHECKING:
+    from collections.abc import Callable, Iterable
+
+    CoordSpec = tuple[np.ndarray, ...] | tuple[tuple[np.ndarray, ...]] | tuple[list[int]]
+
+
+OPTIONS: Iterable[
+    tuple[
+        SupportedMatStor,
+        type[sparse.spmatrix],
+        Callable[[RSlots], CoordSpec],
+        Callable[[CoordSpec], int] | None,
+    ]
+] = [
+    ('C', sparse.csc_matrix, lambda slots: (slots['i'], slots['p']), lambda c: len(c[0])),
+    ('R', sparse.csr_matrix, lambda slots: (slots['j'], slots['p']), lambda c: len(c[0])),
+    ('T', sparse.coo_matrix, lambda slots: ((slots['i'], slots['j']),), lambda c: len(c[0][0])),
+    ('di', sparse.dia_matrix, lambda _: ([0],), None),
+]
 
 
 @converter.rpy2py.register(SexpS4)
-def rmat_to_spmat(rmat: SexpS4):
+def rmat_to_spmat(rmat: SexpS4) -> sparse.spmatrix:
+    """Convert R sparse matrices to scipy sparse matrices."""
     slots = RSlots(rmat)
     with localconverter(default_converter + numpy2ri.converter):
         shape = baseenv['dim'](rmat)
         shape = None if shape is NULL else tuple(shape)
         r_classes = set(rmat.rclass)
         if not supported_r_matrix_classes() & r_classes:
             if any(c.endswith('Matrix') for c in r_classes):
-                warn(f'Encountered Matrix class that is not supported: {r_classes}')
+                # TODO(flying-sheep): #111 set stacklevel
+                # https://github.com/theislab/anndata2ri/issues/111
+                warn(f'Encountered Matrix class that is not supported: {r_classes}', stacklevel=2)
             return rmat
-        for storage, mat_cls, idx, nnz in [
-            ('C', sparse.csc_matrix, lambda: [slots['i'], slots['p']], lambda c: len(c[0])),
-            ('R', sparse.csr_matrix, lambda: [slots['j'], slots['p']], lambda c: len(c[0])),
-            ('T', sparse.coo_matrix, lambda: [(slots['i'], slots['j'])], lambda c: len(c[0][0])),
-            ('di', sparse.dia_matrix, lambda: [[0]], None),
-        ]:
+        for storage, mat_cls, idx, nnz in OPTIONS:
             if not supported_r_matrix_classes(storage=storage) & r_classes:
                 continue
-            coord_spec = idx()
-            if supported_r_matrix_classes(types='n') & r_classes:
+            coord_spec = idx(slots)
+            data = (
+                np.repeat(a=True, repeats=nnz(coord_spec))
                 # we have pattern matrix without data (but always i and j!)
-                data = np.repeat(True, nnz(coord_spec))
-            else:
-                data = slots['x']
-            return mat_cls((data, *coord_spec), shape=shape)
-        else:
-            assert False, 'Should have hit one of the branches'
+                if supported_r_matrix_classes(types='n') & r_classes
+                else slots['x']
+            )
+            dtype = np.bool_ if supported_r_matrix_classes(types=('n', 'l')) & r_classes else np.floating
+            return mat_cls((data, *coord_spec), shape=shape, dtype=dtype)
+
+        msg = 'Should have hit one of the branches'
+        raise AssertionError(msg)
```

### Comparing `anndata2ri-1.1/src/anndata2ri/scipy2ri/support.py` & `anndata2ri-1.2/src/anndata2ri/scipy2ri/_support.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,44 @@
+from __future__ import annotations
+
 from functools import lru_cache
-from typing import FrozenSet, Iterable, Union
+from typing import TYPE_CHECKING, Literal, get_args
+
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+SupportedMatType = Literal['d', 'l', 'n']
+SupportedMatStor = Literal['C', 'R', 'T', 'di']
 
 # these are documented in __init__.py because of sphinx limitations
-supported_r_matrix_types = frozenset({'d', 'l', 'n'})
-supported_r_matrix_storage = frozenset({'C', 'R', 'T', 'di'})
+supported_r_matrix_types: frozenset[SupportedMatType] = frozenset(get_args(SupportedMatType))
+supported_r_matrix_storage: frozenset[SupportedMatStor] = frozenset(get_args(SupportedMatStor))
 
 
 @lru_cache(maxsize=None)
 def supported_r_matrix_classes(
-    types: Union[Iterable[str], str] = supported_r_matrix_types,
-    storage: Union[Iterable[str], str] = supported_r_matrix_storage,
-) -> FrozenSet[str]:
-    """
-    Get supported classes, possibly limiting data types or storage types.
+    types: Iterable[SupportedMatType] | SupportedMatType = supported_r_matrix_types,
+    storage: Iterable[SupportedMatStor] | SupportedMatStor = supported_r_matrix_storage,
+) -> frozenset[str]:
+    """Get supported classes, possibly limiting data types or storage types.
 
     :param types: Data type character(s) from :data:`supported_r_matrix_types`
     :param storage: Storage mode(s) from :data:`supported_r_matrix_storage`
     :return: All supported classes with those characters
     """
     types = {types} if isinstance(types, str) else set(types)
     storage = {storage} if isinstance(storage, str) else set(storage)
 
     bad_types = types - supported_r_matrix_types
     if bad_types:
-        raise ValueError(f'Type(s) {bad_types} not supported.')
+        msg = f'Type(s) {bad_types} not supported.'
+        raise ValueError(msg)
     bad_storage = storage - supported_r_matrix_storage
     if bad_storage:
-        raise ValueError(f'Storage type(s) {bad_storage} not supported.')
+        msg = f'Storage type(s) {bad_storage} not supported.'
+        raise ValueError(msg)
 
     classes = {f'{t}g{s}Matrix' for t in types for s in storage - {'di'}}
     if 'di' in storage:
         classes |= {f'{t}diMatrix' for t in types - {'n'}}
     return frozenset(classes)
```

### Comparing `anndata2ri-1.1/tests/test_py2rpy.py` & `anndata2ri-1.2/tests/test_py2rpy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,103 @@
-from typing import List
-from warnings import WarningMessage, catch_warnings, simplefilter
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+from warnings import catch_warnings, simplefilter
 
 import numpy as np
 import pytest
 import scanpy as sc
 from anndata import AnnData
+from pandas import DataFrame
 from rpy2.robjects import baseenv, globalenv
+from rpy2.robjects.conversion import localconverter
 
 import anndata2ri
-from anndata2ri.rpy2_ext import importr
-from anndata2ri.test_utils import py2r  # noqa
+from anndata2ri._rpy2_ext import importr
+
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
 
+    from rpy2.rinterface import Sexp
 
-def mk_ad_simple():
+    from anndata2ri.test_utils import Py2R
+
+
+def mk_ad_simple() -> AnnData:
     return AnnData(
         np.array([[1, 2, 3], [0.3, 0.2, 0.1]]),
         dict(cluster=[1, 2]),
         obsm=dict(X_pca=np.array([[1, 3, 5, 7], [2, 4, 6, 8]])),
     )
 
 
-def check_empty(ex):
+def check_empty(_: Sexp) -> None:
     pass
 
 
-def check_pca(ex):
+def check_pca(ex: Sexp) -> None:
     sce = importr('SingleCellExperiment')
     assert [str(n) for n in sce.reducedDimNames(ex)] == ['PCA']
     pca = sce.reducedDim(ex, 'PCA')
     assert tuple(baseenv['dim'](pca)) == (2, 4)
 
 
 datasets = [
     pytest.param(check_empty, (0, 0), AnnData, id='empty'),
     pytest.param(check_pca, (2, 3), mk_ad_simple, id='simple'),
     pytest.param(check_empty, (640, 11), sc.datasets.krumsiek11, id='krumsiek'),
-    # pytest.param(check_empty, (2730, 3451), sc.datasets.paul15, id="paul"),
 ]
 
 
-@pytest.mark.parametrize('check,shape,dataset', datasets)
-def test_py2rpy(py2r, check, shape, dataset):
+@pytest.mark.parametrize(('check', 'shape', 'dataset'), datasets)
+def test_py2rpy(
+    py2r: Py2R,
+    check: Callable[[Sexp], None],
+    shape: tuple[int, ...],
+    dataset: Callable[[], AnnData],
+) -> None:
     if dataset is sc.datasets.krumsiek11:
         with pytest.warns(UserWarning, match=r'Duplicated obs_names'):
             ex = py2r(anndata2ri, dataset())
     else:
         ex = py2r(anndata2ri, dataset())
     assert tuple(baseenv['dim'](ex)[::-1]) == shape
     check(ex)
 
 
-def test_py2rpy2_numpy_pbmc68k():
-    """This has some weird metadata"""
+def test_py2rpy2_numpy_pbmc68k() -> None:
+    """Not tested above as the pbmc68k dataset has some weird metadata."""
     from scanpy.datasets import pbmc68k_reduced
 
     try:
         anndata2ri.activate()
-        with catch_warnings(record=True) as logs:  # type: List[WarningMessage]
+        with catch_warnings(record=True) as logs:
             simplefilter('ignore', DeprecationWarning)
             globalenv['adata'] = pbmc68k_reduced()
         assert len(logs) == 0, [m.message for m in logs]
     finally:
         anndata2ri.deactivate()
+
+
+@pytest.mark.parametrize('attr', ['X', 'layers', 'obsm'])
+def test_dfs(attr: str) -> None:
+    """X, layers, obsm can contain dataframes."""
+    adata = mk_ad_simple()
+    if attr == 'X':
+        adata.X = DataFrame(adata.X, index=adata.obs_names)
+    elif attr == 'layers':
+        adata.layers['X2'] = DataFrame(adata.X, index=adata.obs_names)
+    elif attr == 'obsm':
+        adata.obsm['X_pca'] = DataFrame(adata.obsm['X_pca'], index=adata.obs_names)
+    else:
+        pytest.fail('Forgot to add a case')
+
+    with localconverter(anndata2ri.converter):
+        globalenv['adata_obsm_pd'] = adata
+
+
+def test_df_error() -> None:
+    adata = mk_ad_simple()
+    adata.obsm['stuff'] = DataFrame(dict(a=[1, 2], b=list('ab'), c=[1.0, 2.0]), index=adata.obs_names)
+    with pytest.raises(ValueError, match=r"DataFrame contains non-numeric columns \['b'\]"):
+        anndata2ri.converter.py2rpy(adata)
```

### Comparing `anndata2ri-1.1/tests/test_rpy2py.py` & `anndata2ri-1.2/tests/test_rpy2py.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,48 @@
+from __future__ import annotations
+
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pandas as pd
 import pytest
 from anndata import AnnData
 from rpy2.robjects import conversion, r
 
 import anndata2ri
-from anndata2ri.rpy2_ext import importr
-from anndata2ri.test_utils import r2py  # noqa
+from anndata2ri._rpy2_ext import importr
+
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from rpy2.rinterface import Sexp
+
+    from anndata2ri.test_utils import R2Py
 
 
 as_ = getattr(importr('methods'), 'as')
 se = importr('SummarizedExperiment')
 sce = importr('SingleCellExperiment')
 eh = importr('ExperimentHub')
 seq = importr('scRNAseq')
 
 
 # avoid prompt
 Path(eh.getExperimentHubOption('CACHE')[0]).mkdir(parents=True, exist_ok=True)
 
 
-def check_allen(adata):
+def check_allen(adata: AnnData) -> None:
     assert adata.uns.keys() == {'SuppInfo', 'which_qc'}
     assert set(adata.obs.keys()) > {'NREADS', 'NALIGNED', 'Animal.ID', 'passes_qc_checks_s'}
     assert adata.obs['Secondary.Type'][:4].tolist() == ['L4 Ctxn3', '', 'L5a Batf3', None], 'NAs not conserved?'
     assert adata.obs['Animal.ID'][:4].tolist() == [133632, 133632, 151560, pd.NA], 'NAs not conserved?'
 
 
-def check_example(adata):
+def check_example(adata: AnnData) -> None:
     assert set(adata.obsm.keys()) == {'X_pca', 'X_tsne'}
     assert adata.obsm['X_pca'].shape == (100, 5)
 
 
 code_example = """
 local({
     ncells <- 100
@@ -49,38 +59,43 @@
 expression_sets = [
     pytest.param(
         check_allen,
         (379, 20816),
         lambda: as_(seq.ReprocessedAllenData(assays='tophat_counts'), 'SingleCellExperiment'),
         id='allen',
     ),
-    pytest.param(lambda x: None, (0, 0), sce.SingleCellExperiment, id='empty'),
+    pytest.param(lambda _: None, (0, 0), sce.SingleCellExperiment, id='empty'),
     pytest.param(check_example, (100, 200), lambda: r(code_example), id='example'),
 ]
 
 
-@pytest.mark.parametrize('check,shape,dataset', expression_sets)
-def test_convert_manual(r2py, check, shape, dataset):
+@pytest.mark.parametrize(('check', 'shape', 'dataset'), expression_sets)
+def test_convert_manual(
+    r2py: R2Py,
+    check: Callable[[AnnData], None],
+    shape: tuple[int, ...],
+    dataset: Callable[[], Sexp],
+) -> None:
     ad = r2py(anndata2ri, dataset)
     assert isinstance(ad, AnnData)
     assert ad.shape == shape
     check(ad)
 
 
-def test_convert_empty_df_with_rows(r2py):
+def test_convert_empty_df_with_rows(r2py: R2Py) -> None:
     df = r('S4Vectors::DataFrame(a=1:10)[, -1]')
     assert df.slots['nrows'][0] == 10
 
     df_py = r2py(anndata2ri, lambda: conversion.rpy2py(df))
     assert isinstance(df_py, pd.DataFrame)
 
 
-def test_convert_factor(r2py):
+def test_convert_factor(r2py: R2Py) -> None:
     code = """
     SingleCellExperiment::SingleCellExperiment(
         assays = list(counts = matrix(rpois(6*4, 5), ncol=4)),
         colData = S4Vectors::DataFrame(a_factor = factor(c(rep('A', 2), NA, rep('B', 1))))
     )
     """
     ad = r2py(anndata2ri, lambda: r(code))
     assert isinstance(ad.obs['a_factor'].values, pd.Categorical)
-    assert ad.obs['a_factor'].values.tolist() == pd.Categorical.from_codes([0, 0, -1, 1], ['A', 'B']).tolist()
+    assert ad.obs['a_factor'].to_numpy().tolist() == pd.Categorical.from_codes([0, 0, -1, 1], ['A', 'B']).tolist()
```

### Comparing `anndata2ri-1.1/tests/test_scipy_py2rpy.py` & `anndata2ri-1.2/tests/test_scipy_py2rpy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,44 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Literal
+
 import numpy as np
 import pytest
 from rpy2.robjects import baseenv, numpy2ri
 from scipy import sparse
 
 from anndata2ri import scipy2ri
-from anndata2ri.test_utils import conversions_py2rpy
+
+
+if TYPE_CHECKING:
+    from anndata2ri.test_utils import Py2R
 
 
 mats = [
     pytest.param((0, 0), sparse.csr_matrix((0, 0)), 'gR', id='csr-empty'),
     pytest.param((2, 3), sparse.csr_matrix([[2.0, 0.0, 1.0], [0.0, 0.1, 0.0]]), 'gR', id='csr'),
     pytest.param((3, 2), sparse.csc_matrix([[2.0, 0.0], [1.0, 0.0], [0.1, 0.0]]), 'gC', id='csc'),
     pytest.param((2, 4), sparse.coo_matrix([[2.0, 0.0, 1.0, 0.0], [0.0, 0.1, 0.0, 3.0]]), 'gT', id='coo'),
     pytest.param((4, 4), sparse.dia_matrix(([2.0, 0.4, 1.0, 0.0], [0]), (4, 4)), 'di', id='dia'),
     pytest.param((3, 3), sparse.dia_matrix(([0.0, 0.0, 0.0], [0]), (3, 3)), 'di', id='dia_empty'),
     pytest.param((4, 4), sparse.dia_matrix(([1.0, 1.0, 1.0, 1.0], [0]), (4, 4)), 'di', id='dia_unit'),
 ]
 
 
 @pytest.mark.parametrize('typ', ['l', 'd'])
-@pytest.mark.parametrize('conversion', conversions_py2rpy)
-@pytest.mark.parametrize('shape,dataset,cls', mats)
-def test_py2rpy(typ, conversion, shape, dataset, cls):
+@pytest.mark.parametrize(('shape', 'dataset', 'cls'), mats)
+def test_py2rpy(
+    py2r: Py2R,
+    typ: Literal['l', 'd'],
+    shape: tuple[int, ...],
+    dataset: sparse.spmatrix,
+    cls: str,
+) -> None:
     if typ == 'l':
         dataset = dataset.astype(bool)
-    sm = conversion(scipy2ri, dataset)
+    sm = py2r(scipy2ri, dataset)
     assert f'{typ}{cls}Matrix' in set(sm.rclass)
     assert tuple(baseenv['dim'](sm)) == shape
 
     dm = numpy2ri.converter.py2rpy(baseenv['as.matrix'](sm))
     assert np.allclose(dataset.toarray(), dm)
```

### Comparing `anndata2ri-1.1/tests/test_scipy_rpy2py.py` & `anndata2ri-1.2/tests/test_scipy_rpy2py.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+from __future__ import annotations
+
 from functools import partial
-from typing import Callable, Tuple, Type
+from typing import TYPE_CHECKING
 
 import numpy as np
 import pytest
-from rpy2.rinterface import Sexp
 from rpy2.robjects import baseenv, numpy2ri, r
 from scipy import sparse
 
 from anndata2ri import scipy2ri
-from anndata2ri.rpy2_ext import importr
-from anndata2ri.test_utils import ConversionModule, conversions_rpy2py
+from anndata2ri._rpy2_ext import importr
+
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from rpy2.rinterface import Sexp
+
+    from anndata2ri.test_utils import R2Py
 
 
 matrix = importr('Matrix')
 methods = importr('methods')
 
 
 dgc_empty = partial(methods.new, 'dgCMatrix')
@@ -26,21 +34,21 @@
 dgt = partial(r, 'Matrix::sparseMatrix(1:2, 3:2, x = 1:2, giveCsparse = FALSE)')
 coo_f = [[0.0, 0.0, 1.0], [0.0, 2.0, 0.0]]
 
 lgc = partial(r, 'Matrix::Matrix(c(T, T, F, T, F, T), 2, sparse = TRUE)')
 csc_b1 = [[1, 0, 0], [1, 1, 1]]
 lgr = partial(r, "new('lgRMatrix', j = 1:0, p = c(0L, 0L, 1L, 2L), x = c(T, F), Dim = c(3L, 3L))")
 csr_b1 = [[0, 0, 0], [0, 1, 0], [0, 0, 0]]
-# lgt = ...
-# coo_b1 = ...
+# TODO(flying-sheep): lgt & coo_b1 matrices
+# https://github.com/theislab/anndata2ri/issues/110
 
 ngc = partial(r, "as(Matrix::Matrix(c(T, T, F, T, F, T), 2, sparse = TRUE), 'nMatrix')")
 csc_b2 = [[1, 0, 0], [1, 1, 1]]
-# ngr = ...
-# csr_b2 = ...
+# TODO(flying-sheep): ngr & csr_b2 matrices
+# https://github.com/theislab/anndata2ri/issues/110
 ngt = partial(r, 'Matrix::sparseMatrix(1:2, 3:2, dims = c(3, 3), giveCsparse = FALSE)')
 coo_b2 = [[0, 0, 1], [0, 1, 0], [0, 0, 0]]
 
 mats = [
     pytest.param((0, 0), sparse.csc_matrix, np.floating, csc_empty, dgc_empty, id='dgC_empty'),
     pytest.param((3, 2), sparse.csc_matrix, np.floating, csc_f, dgc, id='dgC'),
     pytest.param((2, 3), sparse.csr_matrix, np.floating, csr_f, dgr, id='dgR'),
@@ -50,24 +58,24 @@
     # pytest.param((?, ?), sparse.coo_matrix, np.bool_, coo_b1, lgt, id="lgT"),
     pytest.param((2, 3), sparse.csc_matrix, np.bool_, csc_b2, ngc, id='ngC'),
     # pytest.param((?, ?), sparse.csr_matrix, np.bool_, csr_b2, ngr, id="ngR"),
     pytest.param((3, 3), sparse.coo_matrix, np.bool_, coo_b2, ngt, id='ngT'),
 ]
 
 
-@pytest.mark.parametrize('conversion', conversions_rpy2py)
-@pytest.mark.parametrize('shape,cls,dtype,arr,dataset', mats)
+@pytest.mark.parametrize(('shape', 'cls', 'dtype', 'arr', 'dataset'), mats)
 def test_py2rpy(
-    conversion: Callable[[ConversionModule, Callable[[], Sexp]], sparse.spmatrix],
-    shape: Tuple[int, int],
-    cls: Type[sparse.spmatrix],
+    r2py: R2Py,
+    shape: tuple[int, int],
+    cls: type[sparse.spmatrix],
     dtype: np.dtype,
     arr: np.ndarray,
     dataset: Callable[[], Sexp],
-):
-    sm = conversion(scipy2ri, dataset)
+) -> None:
+    sm = r2py(scipy2ri, dataset)
     assert isinstance(sm, cls)
     assert sm.shape == shape
+    assert sm.dtype == dtype
     assert np.allclose(sm.toarray(), np.array(arr))
 
     dm = numpy2ri.converter.rpy2py(baseenv['as.matrix'](dataset()))
     assert np.allclose(sm.toarray(), dm)
```

### Comparing `anndata2ri-1.1/PKG-INFO` & `anndata2ri-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: anndata2ri
-Version: 1.1
+Version: 1.2
 Project-URL: Documentation, https://icb-anndata2ri.readthedocs-hosted.com/
-Project-URL: Issue Tracker, https://github.com/theislab/anndata2ri/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Source Code, https://github.com/theislab/anndata2ri
+Project-URL: Issue Tracker, https://github.com/theislab/anndata2ri/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Author-email: "Philipp A." <flying-sheep@web.de>
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: anndata
-Requires-Dist: get-version
 Requires-Dist: rpy2>=3.4.3
 Requires-Dist: tzlocal
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: setuptools-scm; extra == 'dev'
 Provides-Extra: doc
-Requires-Dist: importlib-metadata; python_version < '3.8' and extra == 'doc'
+Requires-Dist: importlib-resources; python_version < '3.9' and extra == 'doc'
 Requires-Dist: lxml; extra == 'doc'
 Requires-Dist: scanpydoc; extra == 'doc'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme>=0.5; extra == 'doc'
 Requires-Dist: sphinx>=3.0; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pygments; extra == 'test'
```

