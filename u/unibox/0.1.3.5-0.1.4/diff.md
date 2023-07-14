# Comparing `tmp/unibox-0.1.3.5.tar.gz` & `tmp/unibox-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.3.5.tar", max compression
+gzip compressed data, was "unibox-0.1.4.tar", max compression
```

## Comparing `unibox-0.1.3.5.tar` & `unibox-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-14 01:40:44.793897 unibox-0.1.3.5/LICENSE
--rw-r--r--   0        0        0      546 2023-07-14 01:40:44.793897 unibox-0.1.3.5/README.md
--rw-r--r--   0        0        0      464 2023-07-14 01:40:44.793897 unibox-0.1.3.5/pyproject.toml
--rw-r--r--   0        0        0       76 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/__init__.py
--rw-r--r--   0        0        0     3095 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/processing/__init__.py
--rw-r--r--   0        0        0     2095 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/processing/file_mover.py
--rw-r--r--   0        0        0     6268 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/utils/__init__.py
--rw-r--r--   0        0        0     2787 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/utils/data_loader.py
--rw-r--r--   0        0        0     3759 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/utils/logger.py
--rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 unibox-0.1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 02:03:31.604033 unibox-0.1.4/LICENSE
+-rw-r--r--   0        0        0      733 2023-07-14 02:03:31.604033 unibox-0.1.4/README.md
+-rw-r--r--   0        0        0      500 2023-07-14 02:03:31.604033 unibox-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/__init__.py
+-rw-r--r--   0        0        0     3095 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     2095 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/processing/file_mover.py
+-rw-r--r--   0        0        0     6268 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     3291 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/utils/uni_loader.py
+-rw-r--r--   0        0        0     3759 2023-07-14 02:03:31.604033 unibox-0.1.4/unibox/utils/uni_logger.py
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 unibox-0.1.4/PKG-INFO
```

### Comparing `unibox-0.1.3.5/LICENSE` & `unibox-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.5/unibox/cli.py` & `unibox-0.1.4/unibox/cli.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.5/unibox/processing/file_mover.py` & `unibox-0.1.4/unibox/processing/file_mover.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.5/unibox/processing/image_resizer.py` & `unibox-0.1.4/unibox/processing/image_resizer.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.5/unibox/utils/data_loader.py` & `unibox-0.1.4/unibox/utils/uni_loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,101 @@
+# Adding the _load_csv and _load_parquet methods to the UniLoader class
+
+from __future__ import annotations
+
+from pathlib import Path
+from typing import Callable
 import csv
 import json
-from PIL import Image
 import tomli
+import pandas as pd
+from PIL import Image
 from omegaconf import OmegaConf
-from pathlib import Path
-from .logger import UniLogger
+import pyarrow.parquet as pq
+
+from .uni_logger import UniLogger
 
 
 class UniLoader:
-    """简单的loader utils, 用于原样加载json, txt, csv, image等数据;
-    数据cleaning写在具体使用的class里
+    """A simple utility class for loading various file types.
+    Data cleaning should be done in the class that uses this loader.
     """
 
     def __init__(self, logger=None):
         if not logger:
             self.logger = UniLogger(file_suffix="UniLoader")
         else:
             self.logger = logger
 
-    def _load_data(self, file_path: Path, load_func, encoding="utf-8"):
-        """
-        使用<Load_func>读取<file_path>的内容, 并返回
-        """
-        file_type = file_path.suffix.lstrip(".")
-        if not file_path.exists():
-            self.logger.log("ERROR", f'{file_type} DOES NOT EXIST at "{file_path}"')
-            return None
+        # Mapping of file extensions to loader functions
+        self.loaders = {
+            '.json': self._load_json,
+            '.txt': self._load_txt,
+            '.csv': self._load_csv,
+            '.png': self._load_image,
+            '.jpg': self._load_image,
+            '.toml': self._load_toml,
+            '.yaml': self._load_yaml,
+            '.parquet': self._load_parquet,
+        }
 
-        try:
-            with open(file_path, "r", encoding=encoding) as f:
-                data = load_func(f)
+    def loads(self, file_path: Path | str, encoding="utf-8"):
+        """Load data from the given file path.
 
-            if not data:
-                self.logger.log("WARNING", f'EMPTY {file_type} file at "{file_path}"')
-                return None
+        The type of data returned depends on the file extension.
+        """
+        if isinstance(file_path, str):
+            file_path = Path(file_path)
 
-            return data
-        except Exception as e:
-            self.logger.log("ERROR", f'{file_type} LOAD ERROR at "{file_path}": {e}')
+        file_type = file_path.suffix
+
+        if not file_path.exists():
+            self.logger.log("WARNING", f'{file_type} DOES NOT EXIST at "{file_path}"')
             return None
 
-    def load_json(self, json_path: Path, encoding="utf-8"):
-        # *.json
-        return self._load_data(json_path, json.load, encoding)
-
-    def load_txt(self, txt_path: Path, encoding="utf-8"):
-        # *.txt
-        return self._load_data(txt_path, lambda f: f.read(), encoding)
-
-    def load_csv(self, csv_path: Path, delimiter=",", encoding="utf-8"):
-        # *.csv
-        return self._load_data(
-            csv_path, lambda f: list(csv.reader(f, delimiter=delimiter)), encoding
-        )
+        if file_type not in self.loaders:
+            self.logger.log("ERROR", f'Unsupported file type "{file_type}"')
+            return None
 
-    def load_image(self, image_path: Path):
         try:
-            return Image.open(image_path)
+            return self.loaders[file_type](file_path, encoding)
         except Exception as e:
-            self.logger.log("ERROR", f"image load error at {image_path}: {e}")
+            self.logger.log("ERROR", f'{file_type} LOAD ERROR at "{file_path}": {e}')
             return None
 
-    def load_toml(self, toml_path: Path, encoding="utf-8"):
-        return self._load_data(toml_path, tomli.load, encoding)
-
-    def load_yaml(self, yaml_path: Path, encoding="utf-8"):
-        return self._load_data(yaml_path, lambda f: OmegaConf.load(f), encoding)
-
+    def _load_json(self, file_path: Path, encoding):
+        with open(file_path, "r", encoding=encoding) as f:
+            return json.load(f)
+
+    def _load_txt(self, file_path: Path, encoding):
+        with open(file_path, "r", encoding=encoding) as f:
+            return f.readlines()
+
+    def _load_csv(self, file_path: Path, encoding):
+        return pd.read_csv(file_path, delimiter=',')
+
+    def _load_image(self, file_path: Path, encoding):
+        return Image.open(file_path)
+
+    def _load_toml(self, file_path: Path, encoding):
+        with open(file_path, "r", encoding=encoding) as f:
+            return tomli.load(f)
+
+    def _load_yaml(self, file_path: Path, encoding):
+        with open(file_path, "r", encoding=encoding) as f:
+            return OmegaConf.load(f)
 
+    def _load_parquet(self, file_path: Path, encoding):
+        return pd.read_parquet(file_path)
 
-# todo: implement unibox.loads() function
 
 if __name__ == "__main__":
     # Usage example
     logger = UniLogger("logs", file_suffix="data_loader")
     data_loader = UniLoader(logger)
-    json_data = data_loader.load_json(Path("example.json"))
-    txt_data = data_loader.load_txt(Path("example.txt"))
-    csv_data = data_loader.load_csv(Path("example.csv"))
-    image_data = data_loader.load_image(Path("example.png"))
-    toml_data = data_loader.load_toml(Path("example.toml"))
-    yaml_data = data_loader.load_yaml(Path("example.yaml"))
+    json_data = data_loader.loads("example.json")
+    txt_data = data_loader.loads(Path("example.txt"))
+    csv_data = data_loader.loads(Path("example.csv"))
+    image_data = data_loader.loads(Path("example.png"))
+    toml_data = data_loader.loads(Path("example.toml"))
+    yaml_data = data_loader.loads(Path("example.yaml"))
+    parquet_data = data_loader.loads(Path("example.parquet"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `unibox-0.1.3.5/unibox/utils/logger.py` & `unibox-0.1.4/unibox/utils/uni_logger.py`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.5/PKG-INFO` & `unibox-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.1.3.5
+Version: 0.1.4
 Summary: one toolbox to rule'em all
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.4,<9.0.0)
+Requires-Dist: click (>=8.1.5,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Unibox
 
 Unibox is a tool that aims to provide a unified interface for various common daily operations.
 
 ## Features
 
 **CLI**:
 - `unibox resize <dir>`: resizes a directory of images using either `pillow` or `libvips`
+- `unibox copy <dir>`: an awscli-like tool for copying files with certain suffix to a new dir, keeping the same directory structure
+- `unibox move <dir>`: like `copy`, but moves insteads
 
 **utils**:
 - `UniLogger`: uniformed logger class
 - `UniLoader`: uniformed data loader class
 
 ## Install
```

