# Comparing `tmp/checkatlas-0.3.1.tar.gz` & `tmp/checkatlas-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.3.1.tar", max compression
+gzip compressed data, was "checkatlas-0.3.2.tar", max compression
```

## Comparing `checkatlas-0.3.1.tar` & `checkatlas-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1506 2023-07-14 13:45:51.118752 checkatlas-0.3.1/LICENSE
--rw-r--r--   0        0        0     4452 2023-07-14 13:45:51.118752 checkatlas-0.3.1/README.md
--rw-r--r--   0        0        0      111 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/__init__.py
--rw-r--r--   0        0        0     4648 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/__main__.py
--rw-r--r--   0        0        0    24201 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/atlas.py
--rw-r--r--   0        0        0     4715 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/cellranger.py
--rw-r--r--   0        0        0     8494 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/checkatlas.py
--rw-r--r--   0        0        0       45 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4108 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20177 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/seurat.py
--rw-r--r--   0        0        0      107 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4544 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     2230 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/files.py
--rw-r--r--   0        0        0     2065 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1350 2023-07-14 13:45:51.342770 checkatlas-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 checkatlas-0.3.1/setup.py
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-14 14:21:31.935068 checkatlas-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4452 2023-07-14 14:21:31.939068 checkatlas-0.3.2/README.md
+-rw-r--r--   0        0        0      111 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4648 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24201 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/atlas.py
+-rw-r--r--   0        0        0     4715 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/cellranger.py
+-rw-r--r--   0        0        0     8494 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0       45 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4108 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/seurat.py
+-rw-r--r--   0        0        0      107 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4544 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     2230 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-14 14:21:31.939068 checkatlas-0.3.2/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1350 2023-07-14 14:21:32.131070 checkatlas-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 checkatlas-0.3.2/setup.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.2/PKG-INFO
```

### Comparing `checkatlas-0.3.1/LICENSE` & `checkatlas-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/README.md` & `checkatlas-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/__main__.py` & `checkatlas-0.3.2/checkatlas/__main__.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/atlas.py` & `checkatlas-0.3.2/checkatlas/atlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/cellranger.py` & `checkatlas-0.3.2/checkatlas/cellranger.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/checkatlas.py` & `checkatlas-0.3.2/checkatlas/checkatlas.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.3.2/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/metrics/metrics.py` & `checkatlas-0.3.2/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.3.2/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.3.2/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.3.2/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.3.2/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/seurat.py` & `checkatlas-0.3.2/checkatlas/seurat.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.3.2/checkatlas/utils/checkatlas_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
         f"   Example: --metric_annot rand_index"
         f"   List of annotation metrics: {annot.__all__}",
     )
     metric_options.add_argument(
         "--metric_dimred",
         nargs="+",
         type=str,
-        default=["kruskal_stress"],
-        # default=[],
+        # default=["kruskal_stress"],
+        default=[],
         help="Specify the list of dimensionality reduction "
         "metrics to calculate.\n"
         "   Example: --metric_dimred kruskal_stress\n"
         f"   List of dim. red. metrics: {dimred.__all__}",
     )
     return parser
```

### Comparing `checkatlas-0.3.1/checkatlas/utils/files.py` & `checkatlas-0.3.2/checkatlas/utils/files.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/utils/folders.py` & `checkatlas-0.3.2/checkatlas/utils/folders.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.3.2/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.1/pyproject.toml` & `checkatlas-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.3.1"
+version = "0.3.2"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
```

### Comparing `checkatlas-0.3.1/setup.py` & `checkatlas-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.3.1/PKG-INFO` & `checkatlas-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.3.1
+Version: 0.3.2
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

