# Comparing `tmp/pychunker-1.1.0.tar.gz` & `tmp/pychunker-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychunker-1.1.0.tar", max compression
+gzip compressed data, was "pychunker-1.2.0.tar", max compression
```

## Comparing `pychunker-1.1.0.tar` & `pychunker-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1085 2023-07-13 21:18:01.318463 pychunker-1.1.0/LICENSE
--rw-r--r--   0        0        0       81 2023-07-14 07:30:55.500467 pychunker-1.1.0/pychunker/__init__.py
--rw-r--r--   0        0        0     2930 2023-07-14 09:15:12.279060 pychunker-1.1.0/pychunker/chunk.py
--rw-r--r--   0        0        0     6679 2023-07-14 09:29:49.067125 pychunker-1.1.0/pychunker/chunkfile.py
--rw-r--r--   0        0        0      732 2023-07-14 08:02:09.418233 pychunker-1.1.0/pychunker/crc.py
--rw-r--r--   0        0        0     1043 2023-07-14 09:08:43.707711 pychunker-1.1.0/pychunker/exceptions.py
--rw-r--r--   0        0        0      940 2023-07-14 08:38:33.627490 pychunker-1.1.0/pychunker/functions.py
--rw-r--r--   0        0        0      278 2023-07-14 08:13:01.029759 pychunker-1.1.0/pychunker/functions.pyi
--rw-r--r--   0        0        0       47 2023-07-13 21:18:01.320471 pychunker-1.1.0/pychunker/units.py
--rw-r--r--   0        0        0      535 2023-07-14 09:25:39.690580 pychunker-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      498 2023-07-13 21:18:01.318463 pychunker-1.1.0/README.md
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 pychunker-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-13 21:18:01.318463 pychunker-1.2.0/LICENSE
+-rw-r--r--   0        0        0      179 2023-07-14 11:35:51.774009 pychunker-1.2.0/pychunker/__init__.py
+-rw-r--r--   0        0        0     2880 2023-07-14 11:44:42.908390 pychunker-1.2.0/pychunker/chunk.py
+-rw-r--r--   0        0        0     6772 2023-07-14 11:48:08.528088 pychunker-1.2.0/pychunker/chunkfile.py
+-rw-r--r--   0        0        0      732 2023-07-14 08:02:09.418233 pychunker-1.2.0/pychunker/crc.py
+-rw-r--r--   0        0        0     1043 2023-07-14 09:08:43.707711 pychunker-1.2.0/pychunker/exceptions.py
+-rw-r--r--   0        0        0      940 2023-07-14 08:38:33.627490 pychunker-1.2.0/pychunker/functions.py
+-rw-r--r--   0        0        0      278 2023-07-14 08:13:01.029759 pychunker-1.2.0/pychunker/functions.pyi
+-rw-r--r--   0        0        0       47 2023-07-13 21:18:01.320471 pychunker-1.2.0/pychunker/units.py
+-rw-r--r--   0        0        0      535 2023-07-14 12:00:46.619656 pychunker-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-07-14 12:13:39.911425 pychunker-1.2.0/README.md
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 pychunker-1.2.0/PKG-INFO
```

### Comparing `pychunker-1.1.0/LICENSE` & `pychunker-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pychunker-1.1.0/pychunker/chunk.py` & `pychunker-1.2.0/pychunker/chunk.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         self.__io: IO[bytes] = io
         self.__cns: int = chunk_name_size
     
     # ! Magic Methods
     def __str__(self) -> str: return f"{self.__class__.__name__}(name={repr(self.__name)}, mode={repr(self.__mode)}, size={repr(self.size)})"
     def __repr__(self) -> str: return self.__str__()
     def __enter__(self): return self
-    def __exit__(self, exc_type, exc_value, trace) -> None:
-        if not self.closed:
-            self.close()
+    def __exit__(self, exc_type, exc_value, trace) -> None: pass
     
     # ! Property
     @property
     def name(self) -> str: return self.__name
     
     @property
     def mode(self) -> Literal["a", "r", "w"]: return self.__mode
```

### Comparing `pychunker-1.1.0/pychunker/chunkfile.py` & `pychunker-1.2.0/pychunker/chunkfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,27 +151,30 @@
     # ! Functions
     def exists_chunk(self, name: str) -> bool:
         for chunk in self.__chunks:
             if chunk.name == name:
                 return True
         return False
     
-    def create_chunk(self, name: str) -> None:
+    def get_chunk(self, name: str) -> Chunk:
+        return self.__getitem__(name)
+    
+    def create_chunk(self, name: str) -> Chunk:
         assert len(name) <= self.__cns
         assert not self.exists_chunk(name)
         if self.mode == "r":
             raise IOReadOnlyError()
-        self.__chunks.append(
-            Chunk(
-                name.ljust(self.__cns), 
-                TemporaryFile("wb+", suffix="chunk"),
-                mode=self.__mode,
-                chunk_name_size=self.__cns
-            )
+        chunk = Chunk(
+            name.ljust(self.__cns), 
+            TemporaryFile("wb+", suffix="chunk"),
+            mode=self.__mode,
+            chunk_name_size=self.__cns
         )
+        self.__chunks.append(chunk)
+        return chunk
     
     # ! IO Vars
     @property
     def closed(self) -> bool: return self.__io.closed
     
     # ! IO Functions
     def __ioclear(self) -> None:
```

### Comparing `pychunker-1.1.0/pychunker/crc.py` & `pychunker-1.2.0/pychunker/crc.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.1.0/pychunker/exceptions.py` & `pychunker-1.2.0/pychunker/exceptions.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.1.0/pychunker/functions.py` & `pychunker-1.2.0/pychunker/functions.py`

 * *Files identical despite different names*

### Comparing `pychunker-1.1.0/pyproject.toml` & `pychunker-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pychunker"
-version = "1.1.0"
+version = "1.2.0"
 description = "Module for reading/writing chunk files."
 authors = ["Romanin <semina054@gmail.com>"]
 repository = "https://github.com/romanin-rf/Chunker"
 license = "MIT"
 readme = "README.md"
 keywords = ["pychunker", "chunker", "chunkfile", "io", "file", "chunk", "read", "write"]
 classifiers = [
```

### Comparing `pychunker-1.1.0/PKG-INFO` & `pychunker-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunker
-Version: 1.1.0
+Version: 1.2.0
 Summary: Module for reading/writing chunk files.
 Home-page: https://github.com/romanin-rf/Chunker
 License: MIT
 Keywords: pychunker,chunker,chunkfile,io,file,chunk,read,write
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -18,26 +18,26 @@
 Description-Content-Type: text/markdown
 
 # Chunker
 ## Description
 Module for reading/writing chunk files.
 
 ## Using
-- `exmaple.py`:
+- `example.py`:
 ```python
 import pychunker
 
 with pychunker.open("chunkfile.bin", "w") as cf:
-    cf.create_chunk("ADAT")
-    cf.create_chunk("STR_")
+    with cf.create_chunk("DDAT") as ddat:
+        ddat.write(b'1234567890')
     
-    cf["ADAT"].write(b'1234567890')
-    cf["STR_"].write(b'STRING')
+    with cf.create_chunk("SDAT") as sdat:
+        sdat.write(b'Hello World!')
 
 with pychunker.open("chunkfile.bin") as cf:
     print(cf.chunks)
 ```
 
 - `output`:
 ```python
->>> [Chunk(name='ADAT', mode='r', size=10), Chunk(name='STR_', mode='r', size=6)]
+>>> [Chunk(name='DDAT', mode='r', size=10), Chunk(name='SDAT', mode='r', size=12)]
 ```
```

