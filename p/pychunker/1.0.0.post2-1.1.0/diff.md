# Comparing `tmp/pychunker-1.0.0.post2.tar.gz` & `tmp/pychunker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychunker-1.0.0.post2.tar", max compression
+gzip compressed data, was "pychunker-1.1.0.tar", max compression
```

## Comparing `pychunker-1.0.0.post2.tar` & `pychunker-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1084 2023-07-13 20:10:18.964686 pychunker-1.0.0.post2/LICENSE
--rw-r--r--   0        0        0       57 2023-07-13 20:37:59.612809 pychunker-1.0.0.post2/pychunker/__init__.py
--rw-r--r--   0        0        0     2675 2023-07-13 20:28:04.083774 pychunker-1.0.0.post2/pychunker/chunk.py
--rw-r--r--   0        0        0     5832 2023-07-13 20:46:51.143097 pychunker-1.0.0.post2/pychunker/chunkfile.py
--rw-r--r--   0        0        0      844 2023-07-13 20:16:28.807145 pychunker-1.0.0.post2/pychunker/functions.py
--rw-r--r--   0        0        0      253 2023-07-13 20:18:44.069709 pychunker-1.0.0.post2/pychunker/functions.pyi
--rw-r--r--   0        0        0       47 2023-07-13 20:31:49.092363 pychunker-1.0.0.post2/pychunker/units.py
--rw-r--r--   0        0        0      541 2023-07-13 21:10:43.834535 pychunker-1.0.0.post2/pyproject.toml
--rw-r--r--   0        0        0      498 2023-07-13 21:08:41.956516 pychunker-1.0.0.post2/README.md
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 pychunker-1.0.0.post2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-13 21:18:01.318463 pychunker-1.1.0/LICENSE
+-rw-r--r--   0        0        0       81 2023-07-14 07:30:55.500467 pychunker-1.1.0/pychunker/__init__.py
+-rw-r--r--   0        0        0     2930 2023-07-14 09:15:12.279060 pychunker-1.1.0/pychunker/chunk.py
+-rw-r--r--   0        0        0     6679 2023-07-14 09:29:49.067125 pychunker-1.1.0/pychunker/chunkfile.py
+-rw-r--r--   0        0        0      732 2023-07-14 08:02:09.418233 pychunker-1.1.0/pychunker/crc.py
+-rw-r--r--   0        0        0     1043 2023-07-14 09:08:43.707711 pychunker-1.1.0/pychunker/exceptions.py
+-rw-r--r--   0        0        0      940 2023-07-14 08:38:33.627490 pychunker-1.1.0/pychunker/functions.py
+-rw-r--r--   0        0        0      278 2023-07-14 08:13:01.029759 pychunker-1.1.0/pychunker/functions.pyi
+-rw-r--r--   0        0        0       47 2023-07-13 21:18:01.320471 pychunker-1.1.0/pychunker/units.py
+-rw-r--r--   0        0        0      535 2023-07-14 09:25:39.690580 pychunker-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      498 2023-07-13 21:18:01.318463 pychunker-1.1.0/README.md
+-rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 pychunker-1.1.0/PKG-INFO
```

### Comparing `pychunker-1.0.0.post2/LICENSE` & `pychunker-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pychunker-1.0.0.post2/pychunker/chunkfile.py` & `pychunker-1.1.0/pychunker/chunkfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,116 @@
-import shutil
 from pathlib import Path
 from tempfile import TemporaryFile
 # > Typing
 from typing import IO, Union, List, Literal
 # > Local Import's
 from .chunk import Chunk
 from .functions import iocopy, initfp
 from .units import DEFAULT_CHUNK_FILE_SIGNATURE
+from .exceptions import (
+    ChunkIsDamagedError,
+    IsNotChunkFile,
+    IOReadOnlyError
+)
 
 # ! Main Class
 class ChunkFile:
     def __ischunkfile(self) -> bool:
         self.__io.seek(0)
         return self.__io.read(len(self.__cfs)) == self.__cfs
     
     def __initchunkfile(self) -> None:
-        assert self.__ischunkfile()
+        if not self.__ischunkfile():
+            raise IsNotChunkFile()
+        
         self.__io.seek(len(self.__cfs))
+        
         while len(b_size:=self.__io.read(self.__cls)) != 0:
+            cio = TemporaryFile("wb+", suffix="chunk")
             size = int.from_bytes(b_size, 'big')
             name = self.__io.read(self.__cns).decode(errors="ignore")
-            cio = TemporaryFile("wb+", suffix="chunk")
-            iocopy(self.__io, cio, size, buffer_size=self.__bfs)
-            self.__chunks.append(
-                Chunk(
-                    name, cio, self.__mode,
-                    chunk_name_size=self.__cns
+            
+            ccrc = iocopy(self.__io, cio, size, self.__bfs)
+            fcrc = int.from_bytes(self.__io.read(4), 'big')
+            
+            if fcrc == ccrc.crc:
+                self.__chunks.append(
+                    Chunk(
+                        name, cio, self.__mode,
+                        chunk_name_size=self.__cns
+                    )
                 )
-            )
+            else:
+                if not self.__icrc:
+                    raise ChunkIsDamagedError(fcrc, ccrc)
     
     def __init__(
         self,
         fp: Union[str, Path, IO[bytes]],
         mode: Literal["a", "r", "w"],
         *,
-        buffer_size: int=4096,
+        buffer_size: int=8192,
         chunk_file_signature: bytes=DEFAULT_CHUNK_FILE_SIGNATURE,
         chunk_name_size: int=4,
-        chunk_length_size: int=4
+        chunk_length_size: int=4,
+        ignore_crc: bool=False
     ) -> None:
-        """!!! USE THE `ChunkFile.open` METHOD !!!!"""
+        """!!! USE THE `ChunkFile.open` METHOD !!!"""
         self.__name, self.__io = initfp(fp)
         self.__mode = mode
-        self.__chunks: List[Chunk] = []
+        self.__chunks = []
         self.__bfs = buffer_size
         self.__cfs = chunk_file_signature
         self.__cns = chunk_name_size
         self.__cls = chunk_length_size
+        self.__icrc = ignore_crc
         
         # ! Initialize Chunk File
         self.__initchunkfile()
     
     @staticmethod
     def create(
         fp: Union[str, Path, IO[bytes]],
         mode: Literal["a", "r", "w"],
         *,
-        buffer_size: int=4096,
+        buffer_size: int=8192,
         chunk_file_signature: bytes=DEFAULT_CHUNK_FILE_SIGNATURE,
         chunk_name_size: int=4,
-        chunk_length_size: int=4
+        chunk_length_size: int=4,
+        ignore_crc: bool=False
     ):
-        """!!! USE THE `ChunkFile.open` METHOD !!!!"""
+        """!!! USE THE `ChunkFile.open` METHOD !!!"""
         name, cfio = initfp(fp)
+        
         if not cfio.closed:
             cfio.close()
+        
         cfio = open(name, 'wb+')
         cfio.seek(0)
         cfio.write(chunk_file_signature)
+        
         return ChunkFile(
             cfio, mode,
             buffer_size=buffer_size,
             chunk_file_signature=chunk_file_signature,
             chunk_name_size=chunk_name_size,
-            chunk_length_size=chunk_length_size
+            chunk_length_size=chunk_length_size,
+            ignore_crc=ignore_crc
         )
     
     @staticmethod
     def open( 
         fp: Union[str, Path, IO[bytes]],
         mode: Literal["a", "r", "w"]="r",
         *,
-        buffer_size: int=4096,
+        buffer_size: int=8192,
         chunk_file_signature: bytes=DEFAULT_CHUNK_FILE_SIGNATURE,
         chunk_name_size: int=4,
-        chunk_length_size: int=4
+        chunk_length_size: int=4,
+        ignore_crc: bool=False
     ):
         """
         Opening a chunk file.
 
         * `mode`: 
         
         \t- `"a"`:  First reads, then opens in read/write mode.
@@ -102,15 +124,16 @@
         else:
             raise ValueError(f"The 'mode' argument cannot be equal: {repr(mode)}")
         return fpopen(
             fp, mode,
             buffer_size=buffer_size,
             chunk_file_signature=chunk_file_signature,
             chunk_name_size=chunk_name_size,
-            chunk_length_size=chunk_length_size
+            chunk_length_size=chunk_length_size,
+            ignore_crc=ignore_crc
         )
     
     # ! Magic Methods
     def __getitem__(self, key: str) -> Chunk:
         for chunk in self.__chunks:
             if key == chunk.name:
                 return chunk
@@ -122,24 +145,25 @@
     # ! Vars
     @property
     def chunks(self) -> List[Chunk]: return self.__chunks
     @property
     def mode(self) -> Literal["a", "r", "w"]: return self.__mode
     
     # ! Functions
-    def chunk_exists(self, name: str) -> bool:
+    def exists_chunk(self, name: str) -> bool:
         for chunk in self.__chunks:
             if chunk.name == name:
                 return True
         return False
     
     def create_chunk(self, name: str) -> None:
         assert len(name) <= self.__cns
-        assert not self.chunk_exists(name)
-        assert self.__mode != "r"
+        assert not self.exists_chunk(name)
+        if self.mode == "r":
+            raise IOReadOnlyError()
         self.__chunks.append(
             Chunk(
                 name.ljust(self.__cns), 
                 TemporaryFile("wb+", suffix="chunk"),
                 mode=self.__mode,
                 chunk_name_size=self.__cns
             )
@@ -151,28 +175,34 @@
     
     # ! IO Functions
     def __ioclear(self) -> None:
         if self.__mode != "r":
             if not self.__io.closed:
                 self.__io.close()
             self.__io = open(self.__name, "wb+")
+        else:
+            raise IOReadOnlyError()
     
     def flush(self) -> None:
         if self.__mode != "r":
             assert not self.__io.closed
             self.__ioclear()
             self.__io.seek(0)
             self.__io.write(self.__cfs)
             for chunk in self.__chunks:
                 if not chunk.closed:
                     self.__io.write(chunk.size.to_bytes(self.__cls, 'big'))
                     self.__io.write(chunk.name.encode(errors="ignore"))
                     chunk.seek(0)
-                    shutil.copyfileobj(chunk, self.__io)
+                    crc = iocopy(chunk, self.__io, chunk.size)
+                    self.__io.write(crc.crc_bytes)
+        else:
+            raise IOReadOnlyError()
     
     def close(self) -> None:
-        self.flush()
+        if self.__mode != "r":
+            self.flush()
         for chunk in self.__chunks:
             if not chunk.closed:
                 chunk.close()
         if not self.__io.closed:
             self.__io.close()
```

### Comparing `pychunker-1.0.0.post2/pychunker/functions.py` & `pychunker-1.1.0/pychunker/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from pathlib import Path
+from .crc import CRC32
 
 # ! Functions
 def initfp(fp):
     if isinstance(fp, str) or isinstance(fp, Path):
         path = str(Path(fp))
         if os.path.exists(path):
             assert os.path.isfile(path)
@@ -15,14 +16,18 @@
         assert fp.readable()
         assert fp.seekable()
         assert fp.writable()
         assert hasattr(fp, "name")
         assert isinstance(fp.name, str)
         return fp.name, fp
 
-def iocopy(from_io, to_io, size, buffer_size=4096) -> None:
+def iocopy(from_io, to_io, size, buffer_size=8192):
+    crc = CRC32()
     while size > 0:
         if size >= buffer_size:
             rsize, size = buffer_size, size - buffer_size
         else:
             rsize, size = size, 0
-        to_io.write(from_io.read(rsize))
+        d: bytes = from_io.read(rsize)
+        crc.update(d)
+        to_io.write(d)
+    return crc
```

### Comparing `pychunker-1.0.0.post2/pyproject.toml` & `pychunker-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pychunker"
-version = "1.0.0.post2"
+version = "1.1.0"
 description = "Module for reading/writing chunk files."
 authors = ["Romanin <semina054@gmail.com>"]
 repository = "https://github.com/romanin-rf/Chunker"
 license = "MIT"
 readme = "README.md"
 keywords = ["pychunker", "chunker", "chunkfile", "io", "file", "chunk", "read", "write"]
 classifiers = [
```

### Comparing `pychunker-1.0.0.post2/PKG-INFO` & `pychunker-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychunker
-Version: 1.0.0.post2
+Version: 1.1.0
 Summary: Module for reading/writing chunk files.
 Home-page: https://github.com/romanin-rf/Chunker
 License: MIT
 Keywords: pychunker,chunker,chunkfile,io,file,chunk,read,write
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
```

