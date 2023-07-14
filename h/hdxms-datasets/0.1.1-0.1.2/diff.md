# Comparing `tmp/hdxms_datasets-0.1.1.tar.gz` & `tmp/hdxms_datasets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdxms_datasets-0.1.1.tar", max compression
+gzip compressed data, was "hdxms_datasets-0.1.2.tar", max compression
```

## Comparing `hdxms_datasets-0.1.1.tar` & `hdxms_datasets-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-01-02 12:20:16.077284 hdxms_datasets-0.1.1/LICENSE
--rw-r--r--   0        0        0      574 2023-01-02 12:20:16.077284 hdxms_datasets-0.1.1/README.md
--rw-r--r--   0        0        0      229 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/__init__.py
--rw-r--r--   0        0        0      281 2023-01-02 12:20:29.641333 hdxms_datasets-0.1.1/hdxms_datasets/__version__.py
--rw-r--r--   0        0        0     4013 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/config.py
--rw-r--r--   0        0        0      171 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/config.yaml
--rw-r--r--   0        0        0     4863 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/datasets.py
--rw-r--r--   0        0        0     4803 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/datavault.py
--rw-r--r--   0        0        0     3110 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/process.py
--rw-r--r--   0        0        0     1491 2023-01-02 12:20:16.081284 hdxms_datasets-0.1.1/hdxms_datasets/reader.py
--rw-r--r--   0        0        0     1513 2023-01-02 12:20:29.641333 hdxms_datasets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 hdxms_datasets-0.1.1/setup.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hdxms_datasets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/LICENSE
+-rw-r--r--   0        0        0      574 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/README.md
+-rw-r--r--   0        0        0      388 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/__init__.py
+-rw-r--r--   0        0        0      281 2023-07-14 09:57:11.381758 hdxms_datasets-0.1.2/hdxms_datasets/__version__.py
+-rw-r--r--   0        0        0     4029 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/config.py
+-rw-r--r--   0        0        0      171 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/config.yaml
+-rw-r--r--   0        0        0     7200 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/datasets.py
+-rw-r--r--   0        0        0     4652 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/datavault.py
+-rw-r--r--   0        0        0     4102 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/process.py
+-rw-r--r--   0        0        0     1215 2023-07-14 09:56:58.769415 hdxms_datasets-0.1.2/hdxms_datasets/reader.py
+-rw-r--r--   0        0        0     1594 2023-07-14 09:57:11.377758 hdxms_datasets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hdxms_datasets-0.1.2/PKG-INFO
```

### Comparing `hdxms_datasets-0.1.1/LICENSE` & `hdxms_datasets-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdxms_datasets-0.1.1/README.md` & `hdxms_datasets-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hdxms_datasets-0.1.1/hdxms_datasets/config.py` & `hdxms_datasets-0.1.2/hdxms_datasets/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import os
 from pathlib import Path
 from typing import Any
 
 from omegaconf import OmegaConf, DictConfig, DictKeyType
 from packaging import version
 
-import hdxms_datasets
+PACKAGE_NAME = "hdxms_datasets"
 
 
 def reset_config():
     """Create a new config.yaml file in the user home dir/.hdxms_datasets folder"""
 
     with open(conf_home_pth, "w") as target:
         from hdxms_datasets.__version__ import __version__
 
-        version_string = "# HDXMS datasets configuration file " + __version__ + "\n\n"
+        version_string = f"# {PACKAGE_NAME} configuration file " + __version__ + "\n\n"
         target.write(version_string)
 
         with open(current_dir / "config.yaml") as source:
             for line in source:
                 target.write(line)
 
 
@@ -101,29 +101,29 @@
         self._config = {} if config is None else config
 
     def __getitem__(self, item):
         return self._config[item]
 
 
 home_dir = Path.home()
-config_dir = home_dir / ".hdxms_datasets"
+config_dir = home_dir / f".{PACKAGE_NAME}"
 config_dir.mkdir(parents=False, exist_ok=True)
 conf_home_pth = config_dir / "config.yaml"
 
 current_dir = Path(__file__).parent
 conf_src_pth = current_dir / "config.yaml"
 
 # Current config version is outdated
 if not valid_config():
     try:
         reset_config()
         conf = OmegaConf.load(conf_home_pth)
     except FileNotFoundError:
         # This will happen on conda-forge docker build.
-        # When no config.yaml file is in home_dir / '.dont_fret',
+        # When no config.yaml file is in home_dir / '.{PACKAGE_NAME}'
         # ConfigurationSettings will use the hardcoded version
         conf = OmegaConf.load(conf_src_pth)
         # (this is run twice due to import but should be OK since conf is singleton)
 else:
     conf = OmegaConf.load(conf_home_pth)
```

### Comparing `hdxms_datasets-0.1.1/hdxms_datasets/datavault.py` & `hdxms_datasets-0.1.2/hdxms_datasets/datavault.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from typing import Optional, Union, Type, TYPE_CHECKING
 
 import requests
 import yaml
 
 from hdxms_datasets.config import cfg
 from hdxms_datasets.datasets import HDXDataSet, DataFile
+from hdxms_datasets.process import parse_data_files
 
 if TYPE_CHECKING:
     from hdxms_datasets.datasets import StateParser
 
 
 class DataVault(object):
     def __init__(
         self,
         cache_dir: Optional[Union[Path[str], str]] = None,
     ):
-
         if cache_dir is None:
             self.cache_dir = cfg.database_dir
             self.cache_dir.mkdir(exist_ok=True, parents=True)
         else:
             self.cache_dir: Path = Path(cache_dir)
             if not self.cache_dir.exists():
                 raise FileNotFoundError(f"Cache directory '{self.cache_dir}' does not exist")
@@ -77,16 +77,19 @@
             # Download n new datasets to cache_dir
             ...
 
     def fetch_dataset(self, data_id: str) -> bool:
         """
         Download a dataset from the online repository to the cache dir
 
-        :param data_id:
-        :return:
+        Args:
+            data_id: The ID of the dataset to download.
+
+        Returns:
+            `True` if the dataset was downloaded successfully, `False`  otherwise.
         """
 
         output_pth = self.cache_dir / data_id
         if output_pth.exists():
             return False
         else:
             output_pth.mkdir()
@@ -135,22 +138,13 @@
         for dir in self.cache_dir.iterdir():
             shutil.rmtree(dir)
 
     def load_dataset(self, data_id: str) -> HDXDataSet:
         hdx_spec = yaml.safe_load((self.cache_dir / data_id / "hdx_spec.yaml").read_text())
         dataset_metadata = yaml.safe_load((self.cache_dir / data_id / "metadata.yaml").read_text())
 
-        data_files = {}
-        for name, spec in hdx_spec["data_files"].items():
-            datafile = DataFile(
-                name=name,
-                filepath_or_buffer=Path(self.cache_dir / data_id / spec["filename"]),
-                **{k: v for k, v in spec.items() if k != "filename"},
-            )
-            data_files[name] = datafile
-
-        return HDXDataSet(
-            data_id=data_id,
-            data_files=data_files,
+        return HDXDataSet.from_spec(
             hdx_spec=hdx_spec,
-            metadata=dataset_metadata,
+            data_dir=self.cache_dir / data_id,
+            data_id=data_id,
+            metadata=dataset_metadata
         )
```

### Comparing `hdxms_datasets-0.1.1/hdxms_datasets/reader.py` & `hdxms_datasets-0.1.2/hdxms_datasets/reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 """
 Reader functions for various file formats
 """
 
 from __future__ import annotations
 
-from io import StringIO
 from pathlib import Path
-from typing import Union, Literal
+from typing import Union, Literal, IO, Optional
+
 import pandas as pd
 
 
 def read_dynamx(
-    filepath_or_buffer: Union[Path[str], str, StringIO],
-    time_conversion: tuple[Literal["h", "min", "s"], Literal["h", "min", "s"]] = ("min", "s"),
+    filepath_or_buffer: Union[Path[str], str, IO],
+    time_conversion: Optional[tuple[Literal["h", "min", "s"], Literal["h", "min", "s"]]] = (
+        "min",
+        "s",
+    ),
 ) -> pd.DataFrame:
-
     """
     Reads DynamX .csv files and returns the resulting peptide table as a pandas DataFrame.
 
     Args:
         filepath_or_buffer: File path of the .csv file or :class:`~io.StringIO` object.
         time_conversion: How to convert the time unit of the field 'exposure'. Format is ('<from>', <'to'>).
             Unit options are 'h', 'min' or 's'.
 
     Returns:
         Peptide table as a pandas DataFrame.
     """
 
-    if isinstance(filepath_or_buffer, StringIO):
-        hdr = filepath_or_buffer.readline().strip("# \n\t")
-        filepath_or_buffer.seek(0)
-    else:
-        with open(filepath_or_buffer, "r") as f_obj:
-            hdr = f_obj.readline().strip("# \n\t")
-
-    names = [name.lower().strip("\r\t\n") for name in hdr.split(",")]
-    df = pd.read_csv(filepath_or_buffer, header=0, names=names)
+    df = pd.read_csv(filepath_or_buffer)
+    df.columns = df.columns.str.replace(" ", "_").str.lower()
 
     df.insert(df.columns.get_loc("end") + 1, "stop", df["end"] + 1)
 
-    time_lut = {"h": 3600, "min": 60, "s": 1}
-    time_factor = time_lut[time_conversion[0]] / time_lut[time_conversion[1]]
-
-    df["exposure"] *= time_factor
-    df.columns = df.columns.str.replace(" ", "_")
+    if time_conversion is not None:
+        time_lut = {"h": 3600, "min": 60, "s": 1}
+        time_factor = time_lut[time_conversion[0]] / time_lut[time_conversion[1]]
+        df["exposure"] *= time_factor
 
     return df
```

### Comparing `hdxms_datasets-0.1.1/pyproject.toml` & `hdxms_datasets-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 max-complexity = 10
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "hdxms-datasets"
-version = "0.1.1" # placeholder
+version = "0.1.2" # placeholder
 description = "Download and parse curated HDX-MS datasets"
 authors = ["Jochem Smit <jhsmit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "hdxms_datasets"}]
 exclude = ["hdxms_datasets/_version.py"]
 
@@ -41,21 +41,24 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.0"
 mypy = "^0.991"
 pylint = "^2.15.9"
 poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.2"}
+ipykernel = "^6.24.0"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocstrings = {extras = ["python"], version = "^0.19.1"}
 mkdocs-material = "^8.5.11"
 pygments = "^2.13.0"
+mkdocs-gen-files = "^0.4.0"
+mkdocs-literate-nav = "^0.5.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 metadata = false
```

### Comparing `hdxms_datasets-0.1.1/PKG-INFO` & `hdxms_datasets-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdxms-datasets
-Version: 0.1.1
+Version: 0.1.2
 Summary: Download and parse curated HDX-MS datasets
 License: MIT
 Author: Jochem Smit
 Author-email: jhsmit@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

