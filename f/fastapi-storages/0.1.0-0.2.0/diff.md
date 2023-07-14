# Comparing `tmp/fastapi_storages-0.1.0.tar.gz` & `tmp/fastapi_storages-0.2.0.tar.gz`

## Comparing `fastapi_storages-0.1.0.tar` & `fastapi_storages-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/base.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/exceptions.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/filesystem.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/s3.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/integrations/__init__.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/fastapi_storages/integrations/sqlalchemy.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/README.md
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 fastapi_storages-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/base.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/exceptions.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/filesystem.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/s3.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/integrations/__init__.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/fastapi_storages/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/README.md
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 fastapi_storages-0.2.0/PKG-INFO
```

### Comparing `fastapi_storages-0.1.0/fastapi_storages/base.py` & `fastapi_storages-0.2.0/fastapi_storages/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import BinaryIO
 
 
 class BaseStorage:  # pragma: no cover
+    OVERWRITE_EXISTING_FILES = True
+    """Whether to overwrite existing files
+    if the name is the same or add a suffix to the filename."""
+
     def get_name(self, name: str) -> str:
         ...
 
     def get_path(self, name: str) -> str:
         ...
 
     def get_size(self, name: str) -> int:
@@ -13,14 +17,17 @@
 
     def open(self, name: str) -> BinaryIO:
         ...
 
     def write(self, file: BinaryIO, name: str) -> str:
         ...
 
+    def generate_new_filename(self, filename: str) -> str:
+        ...
+
 
 class StorageFile(str):
     """
     The file obect returned by the storage.
     """
 
     def __new__(cls, name: str, storage: BaseStorage) -> "StorageFile":
@@ -56,14 +63,17 @@
         return self._storage.open(self._name)
 
     def write(self, file: BinaryIO) -> str:
         """
         Write input file which is opened in binary mode to destination.
         """
 
+        if not self._storage.OVERWRITE_EXISTING_FILES:
+            self._name = self._storage.generate_new_filename(self._name)
+
         return self._storage.write(file=file, name=self._name)
 
     def __str__(self) -> str:
         return self.path
 
 
 class StorageImage(StorageFile):
```

### Comparing `fastapi_storages-0.1.0/fastapi_storages/filesystem.py` & `fastapi_storages-0.2.0/fastapi_storages/filesystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     File system storage which stores files in the local filesystem.
     You might want to use this with the `FileType` type.
     """
 
     default_chunk_size = 64 * 1024
 
-    def __init__(self, path: str):
+    def __init__(self, path: str) -> None:
         self._path = Path(path)
         self._path.mkdir(parents=True, exist_ok=True)
 
     def get_name(self, name: str) -> str:
         """
         Get the normalized name of the file.
         """
@@ -59,7 +59,18 @@
             while True:
                 chunk = file.read(self.default_chunk_size)
                 if not chunk:
                     break
                 output.write(chunk)
 
         return str(path)
+
+    def generate_new_filename(self, filename: str) -> str:
+        counter = 0
+        path = self._path / filename
+        stem, extension = Path(filename).stem, Path(filename).suffix
+
+        while path.exists():
+            counter += 1
+            path = self._path / f"{stem}_{counter}{extension}"
+
+        return path.name
```

### Comparing `fastapi_storages-0.1.0/fastapi_storages/integrations/sqlalchemy.py` & `fastapi_storages-0.2.0/fastapi_storages/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_storages-0.1.0/LICENSE.txt` & `fastapi_storages-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_storages-0.1.0/README.md` & `fastapi_storages-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_storages-0.1.0/pyproject.toml` & `fastapi_storages-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "fastapi-storages"
 description = 'FastAPI Storages'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["sqlalchemy", "django", "orm"]
+keywords = ["sqlalchemy", "django", "orm", "fastapi"]
 authors = [
   { name = "Amin Alaee", email = "me@aminalaee.dev" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
@@ -83,17 +83,17 @@
   "black .",
   "ruff --fix .",
 ]
 test = "coverage run -m pytest {args}"
 
 [tool.hatch.envs.docs]
 dependencies = [
-  "mkdocs-material==8.5.7",
-  "mkdocs==1.4.1",
-  "mkdocstrings[python]==0.18.1",
+  "mkdocs-material==9.1.18",
+  "mkdocs==1.4.3",
+  "mkdocstrings[python]==0.22.0",
 ]
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build"
 serve = "mkdocs serve --dev-addr localhost:8080"
 deploy = "mkdocs gh-deploy --force"
```

### Comparing `fastapi_storages-0.1.0/PKG-INFO` & `fastapi_storages-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fastapi-storages
-Version: 0.1.0
+Version: 0.2.0
 Summary: FastAPI Storages
 Project-URL: Documentation, https://github.com/aminalaee/fastapi-storages#readme
 Project-URL: Issues, https://github.com/aminalaee/fastapi-storages/issues
 Project-URL: Source, https://github.com/aminalaee/fastapi-storages
 Author-email: Amin Alaee <me@aminalaee.dev>
 License-Expression: MIT
 License-File: LICENSE.txt
-Keywords: django,orm,sqlalchemy
+Keywords: django,fastapi,orm,sqlalchemy
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
```

