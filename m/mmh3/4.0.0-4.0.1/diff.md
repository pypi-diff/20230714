# Comparing `tmp/mmh3-4.0.0.tar.gz` & `tmp/mmh3-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmh3-4.0.0.tar", last modified: Mon May 22 06:59:22 2023, max compression
+gzip compressed data, was "mmh3-4.0.1.tar", last modified: Fri Jul 14 15:46:05 2023, max compression
```

## Comparing `mmh3-4.0.0.tar` & `mmh3-4.0.1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:59:22.337931 mmh3-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-22 06:59:18.000000 mmh3-4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 06:59:18.000000 mmh3-4.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 06:59:18.000000 mmh3-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 06:59:18.000000 mmh3-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-05-22 06:59:22.333931 mmh3-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-22 06:59:18.000000 mmh3-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-22 06:59:18.000000 mmh3-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:59:22.337931 mmh3-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 06:59:18.000000 mmh3-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:59:22.333931 mmh3-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:59:22.333931 mmh3-4.0.0/src/mmh3/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-22 06:59:18.000000 mmh3-4.0.0/src/mmh3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-22 06:59:18.000000 mmh3-4.0.0/src/mmh3/hashlib.h
--rw-r--r--   0 runner    (1001) docker     (123)    37684 2023-05-22 06:59:18.000000 mmh3-4.0.0/src/mmh3/mmh3module.c
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-22 06:59:18.000000 mmh3-4.0.0/src/mmh3/murmurhash3.c
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-22 06:59:18.000000 mmh3-4.0.0/src/mmh3/murmurhash3.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:59:18.000000 mmh3-4.0.0/src/mmh3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:59:22.333931 mmh3-4.0.0/src/mmh3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-05-22 06:59:21.000000 mmh3-4.0.0/src/mmh3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-22 06:59:21.000000 mmh3-4.0.0/src/mmh3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:59:21.000000 mmh3-4.0.0/src/mmh3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 06:59:21.000000 mmh3-4.0.0/src/mmh3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 06:59:21.000000 mmh3-4.0.0/src/mmh3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:46:05.165116 mmh3-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-14 15:46:02.000000 mmh3-4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-14 15:46:02.000000 mmh3-4.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 15:46:02.000000 mmh3-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 15:46:02.000000 mmh3-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-07-14 15:46:05.165116 mmh3-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-14 15:46:02.000000 mmh3-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-14 15:46:02.000000 mmh3-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:46:05.165116 mmh3-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-14 15:46:02.000000 mmh3-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:46:05.161116 mmh3-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:46:05.165116 mmh3-4.0.1/src/mmh3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:46:05.165116 mmh3-4.0.1/src/mmh3/_mmh3/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/_mmh3/FILE_HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/_mmh3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/_mmh3/murmurhash3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/_mmh3/murmurhash3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/_mmh3/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/hashlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37690 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/mmh3module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:46:02.000000 mmh3-4.0.1/src/mmh3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:46:05.165116 mmh3-4.0.1/src/mmh3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-07-14 15:46:04.000000 mmh3-4.0.1/src/mmh3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-14 15:46:04.000000 mmh3-4.0.1/src/mmh3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:46:04.000000 mmh3-4.0.1/src/mmh3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 15:46:04.000000 mmh3-4.0.1/src/mmh3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 15:46:04.000000 mmh3-4.0.1/src/mmh3.egg-info/top_level.txt
```

### Comparing `mmh3-4.0.0/CHANGELOG.md` & `mmh3-4.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # Changelog
+## 4.0.1 (2023-07-14)
+* Fix incorrect type hints.
+* Refactor the project structure (<https://github.com/hajimes/mmh3/issues/48>).
+
 ## 4.0.0 (2023-05-22)
 * Add experimental support for `hashlib`-compliant hasher classes (<https://github.com/hajimes/mmh3/issues/39>). Note that they are not yet fully tuned for performance.
 * Add support for type hints (<https://github.com/hajimes/mmh3/issues/44>).
 * Add wheels for more platforms (`musllinux`, `s390x`, `win_arm64`, and `macosx_universal2`).
 * Drop support for Python 3.7, as it will reach the end of life on 2023-06-27.
 * Switch license from CC0 to MIT (<https://github.com/hajimes/mmh3/issues/43>).
 * Add a code of conduct (the ACM Code of Ethics and Professional Conduct).
```

### Comparing `mmh3-4.0.0/LICENSE` & `mmh3-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmh3-4.0.0/PKG-INFO` & `mmh3-4.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmh3
-Version: 4.0.0
+Version: 4.0.1
 Summary: Python extension for MurmurHash (MurmurHash3), a set of fast and robust hash functions.
 Author-email: Hajime Senuma <hajime.senuma@gmail.com>
 License: MIT License
         
         Copyright (c) 2011-2023 Hajime Senuma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,15 +113,15 @@
 ```
 
 ### `hashlib`-style hashers
 `mmh3` implements hashers whose interfaces are similar to `hashlib` in the standard library: `mmh3_32()` for 32 bit hashing, `mmh3_x64_128()` for 128 bit hashing optimized for x64 architectures, and `mmh3_x86_128()` for 128 bit hashing optimized for x86 architectures.
 
 In addition to the standard `digest()` method, each hasher has `sintdigest()`, which returns a signed integer, and `uintdigest()`, which returns an unsigned integer. 128 bit hashers also have `stupledigest()` and `utupledigest()` which return two 64 bit integers.
 
-Note that as of version 4.0.0, the implementation is still experimental and its performance can be unsatisfactory (especially `mmh3_x86_128()`). Also, `hexdigest()` is not supported. Use `digest().hex()` instead.
+Note that as of version 4.0.1, the implementation is still experimental and its performance can be unsatisfactory (especially `mmh3_x86_128()`). Also, `hexdigest()` is not supported. Use `digest().hex()` instead.
 
 ```shell
 >>> import mmh3
 >>> hasher = mmh3.mmh3_x64_128(seed=42)
 >>> hasher.update(b"foo")
 >>> hasher.update(b"bar")
 >>> hasher.update("foo") # str inputs are not allowed for hashers
@@ -137,14 +137,18 @@
 >>> hasher.stupledigest() # two 64 bit signed ints
 (7689522670935629698, -159584473158936081)
 >>> hasher.utupledigest() # two 64 bit unsigned ints
 (7689522670935629698, 18287159600550615535)
 ```
 
 ## Changelog
+### 4.0.1 (2023-07-14)
+* Fix incorrect type hints.
+* Refactor the project structure (<https://github.com/hajimes/mmh3/issues/48>).
+
 ### 4.0.0 (2023-05-22)
 * Add experimental support for `hashlib`-compliant hasher classes (<https://github.com/hajimes/mmh3/issues/39>). Note that they are not yet fully tuned for performance.
 * Add support for type hints (<https://github.com/hajimes/mmh3/issues/44>).
 * Add wheels for more platforms (`musllinux`, `s390x`, `win_arm64`, and `macosx_universal2`).
 * Drop support for Python 3.7, as it will reach the end of life on 2023-06-27.
 * Switch license from CC0 to MIT (<https://github.com/hajimes/mmh3/issues/43>).
 * Add a code of conduct (the ACM Code of Ethics and Professional Conduct).
@@ -155,22 +159,14 @@
 ### 3.1.0 (2023-03-24)
 * Add support for Python 3.10 and 3.11. Thanks [wouter bolsterlee](https://github.com/wbolster) and [Dušan Nikolić](https://github.com/n-dusan)!
 * Drop support for Python 3.6; remove legacy code for Python 2.x at the source code level.
 * Add support for 32-bit architectures such as `i686` and `armv7l`. From now on, `hash` and `hash_from_buffer` on these architectures will generate the same hash values as those on other environments. Thanks [Danil Shein](https://github.com/dshein-alt)!
 * In relation to the above, `manylinux2014_i686` wheels are now available.
 * Support for hashing huge data (>16GB). Thanks [arieleizenberg](https://github.com/arieleizenberg)!
 
-### 3.0.0 (2021-02-23)
-* Python wheels are now available, thanks to the power of [cibuildwheel](https://github.com/joerick/cibuildwheel).
-  * Supported platforms are `manylinux1_x86_64`, `manylinux2010_x86_64`, `manylinux2014_aarch64`, `win32`, `win_amd64`, `macosx_10_9_x86_64`, and `macosx_11_0_arm64` (Apple Silicon).
-* Add support for newer macOS environments. Thanks [Matthew Honnibal](https://github.com/honnibal)!
-* Drop support for Python 2.7, 3.3, 3.4, and 3.5.
-* Add support for Python 3.7, 3.8, and 3.9.
-* Migrate CI from Travis CI and AppVeyor to GitHub Actions.
-
 See [CHANGELOG.md](./CHANGELOG.md) for the complete changelog.
 
 ## License
 [MIT](./LICENSE), unless otherwise noted within a file.
 
 ## Known Issues
 ### Getting different results from other MurmurHash3-based libraries
```

### Comparing `mmh3-4.0.0/README.md` & `mmh3-4.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ```
 
 ### `hashlib`-style hashers
 `mmh3` implements hashers whose interfaces are similar to `hashlib` in the standard library: `mmh3_32()` for 32 bit hashing, `mmh3_x64_128()` for 128 bit hashing optimized for x64 architectures, and `mmh3_x86_128()` for 128 bit hashing optimized for x86 architectures.
 
 In addition to the standard `digest()` method, each hasher has `sintdigest()`, which returns a signed integer, and `uintdigest()`, which returns an unsigned integer. 128 bit hashers also have `stupledigest()` and `utupledigest()` which return two 64 bit integers.
 
-Note that as of version 4.0.0, the implementation is still experimental and its performance can be unsatisfactory (especially `mmh3_x86_128()`). Also, `hexdigest()` is not supported. Use `digest().hex()` instead.
+Note that as of version 4.0.1, the implementation is still experimental and its performance can be unsatisfactory (especially `mmh3_x86_128()`). Also, `hexdigest()` is not supported. Use `digest().hex()` instead.
 
 ```shell
 >>> import mmh3
 >>> hasher = mmh3.mmh3_x64_128(seed=42)
 >>> hasher.update(b"foo")
 >>> hasher.update(b"bar")
 >>> hasher.update("foo") # str inputs are not allowed for hashers
@@ -92,14 +92,18 @@
 >>> hasher.stupledigest() # two 64 bit signed ints
 (7689522670935629698, -159584473158936081)
 >>> hasher.utupledigest() # two 64 bit unsigned ints
 (7689522670935629698, 18287159600550615535)
 ```
 
 ## Changelog
+### 4.0.1 (2023-07-14)
+* Fix incorrect type hints.
+* Refactor the project structure (<https://github.com/hajimes/mmh3/issues/48>).
+
 ### 4.0.0 (2023-05-22)
 * Add experimental support for `hashlib`-compliant hasher classes (<https://github.com/hajimes/mmh3/issues/39>). Note that they are not yet fully tuned for performance.
 * Add support for type hints (<https://github.com/hajimes/mmh3/issues/44>).
 * Add wheels for more platforms (`musllinux`, `s390x`, `win_arm64`, and `macosx_universal2`).
 * Drop support for Python 3.7, as it will reach the end of life on 2023-06-27.
 * Switch license from CC0 to MIT (<https://github.com/hajimes/mmh3/issues/43>).
 * Add a code of conduct (the ACM Code of Ethics and Professional Conduct).
@@ -110,22 +114,14 @@
 ### 3.1.0 (2023-03-24)
 * Add support for Python 3.10 and 3.11. Thanks [wouter bolsterlee](https://github.com/wbolster) and [Dušan Nikolić](https://github.com/n-dusan)!
 * Drop support for Python 3.6; remove legacy code for Python 2.x at the source code level.
 * Add support for 32-bit architectures such as `i686` and `armv7l`. From now on, `hash` and `hash_from_buffer` on these architectures will generate the same hash values as those on other environments. Thanks [Danil Shein](https://github.com/dshein-alt)!
 * In relation to the above, `manylinux2014_i686` wheels are now available.
 * Support for hashing huge data (>16GB). Thanks [arieleizenberg](https://github.com/arieleizenberg)!
 
-### 3.0.0 (2021-02-23)
-* Python wheels are now available, thanks to the power of [cibuildwheel](https://github.com/joerick/cibuildwheel).
-  * Supported platforms are `manylinux1_x86_64`, `manylinux2010_x86_64`, `manylinux2014_aarch64`, `win32`, `win_amd64`, `macosx_10_9_x86_64`, and `macosx_11_0_arm64` (Apple Silicon).
-* Add support for newer macOS environments. Thanks [Matthew Honnibal](https://github.com/honnibal)!
-* Drop support for Python 2.7, 3.3, 3.4, and 3.5.
-* Add support for Python 3.7, 3.8, and 3.9.
-* Migrate CI from Travis CI and AppVeyor to GitHub Actions.
-
 See [CHANGELOG.md](./CHANGELOG.md) for the complete changelog.
 
 ## License
 [MIT](./LICENSE), unless otherwise noted within a file.
 
 ## Known Issues
 ### Getting different results from other MurmurHash3-based libraries
```

### Comparing `mmh3-4.0.0/pyproject.toml` & `mmh3-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mmh3"
-version = "4.0.0"
+version = "4.0.1"
 description = "Python extension for MurmurHash (MurmurHash3), a set of fast and robust hash functions."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["utility", "hash", "MurmurHash"]
 authors = [
   {name = "Hajime Senuma", email="hajime.senuma@gmail.com"}
 ]
```

### Comparing `mmh3-4.0.0/src/mmh3/__init__.pyi` & `mmh3-4.0.1/src/mmh3/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # to use list, tuple, dict ... in Python 3.7 and 3.8
 from __future__ import annotations
 
-from typing import Protocol, Union
+from typing import Protocol, Union, final
 
 class IntArrayLike(Protocol):
     def __getitem__(self, index) -> int: ...
 
 Hashable = Union[bytes, bytearray, memoryview, IntArrayLike]
 StrHashable = Union[str, Hashable]
 
 def hash(key: StrHashable, seed: int = 0, signed: bool = True) -> int: ...
 def hash_from_buffer(key: StrHashable, seed: int = 0, signed: bool = True) -> int: ...
-def hash64(key: StrHashable, seed: int = 0, signed: bool = True) -> (int, int): ...
+def hash64(key: StrHashable, seed: int = 0, signed: bool = True) -> tuple[int, int]: ...
 def hash128(key: StrHashable, seed: int = 0, signed: bool = True) -> int: ...
 def hash_bytes(key: StrHashable, seed: int = 0, signed: bool = True) -> bytes: ...
 
 class Hasher:
     def __init__(self, seed: int = 0) -> None: ...
     def update(self, input: Hashable) -> None: ...
     def digest(self) -> bytes: ...
@@ -30,14 +30,14 @@
     def name(self) -> str: ...
 
 @final
 class mmh3_32(Hasher): ...
 
 @final
 class mmh3_x64_128(Hasher):
-    def stupledigest(self) -> (int, int): ...
-    def utupledigest(self) -> (int, int): ...
+    def stupledigest(self) -> tuple[int, int]: ...
+    def utupledigest(self) -> tuple[int, int]: ...
 
 @final
 class mmh3_x86_128(Hasher):
-    def stupledigest(self) -> (int, int): ...
-    def utupledigest(self) -> (int, int): ...
+    def stupledigest(self) -> tuple[int, int]: ...
+    def utupledigest(self) -> tuple[int, int]: ...
```

### Comparing `mmh3-4.0.0/src/mmh3/hashlib.h` & `mmh3-4.0.1/src/mmh3/hashlib.h`

 * *Files identical despite different names*

### Comparing `mmh3-4.0.0/src/mmh3/mmh3module.c` & `mmh3-4.0.1/src/mmh3/mmh3module.c`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #include <stdio.h>
 #include <string.h>
 
 #if defined(__BYTE_ORDER__) && (__BYTE_ORDER__ == __ORDER_BIG_ENDIAN__)
 #include <byteswap.h>
 #endif
 
+#include "_mmh3/murmurhash3.h"
 #include "hashlib.h"
-#include "murmurhash3.h"
 
 #if defined(_MSC_VER)
 typedef signed __int8 int8_t;
 typedef signed __int32 int32_t;
 typedef signed __int64 int64_t;
 typedef unsigned __int8 uint8_t;
 typedef unsigned __int32 uint32_t;
```

### Comparing `mmh3-4.0.0/src/mmh3/murmurhash3.c` & `mmh3-4.0.1/src/mmh3/_mmh3/murmurhash3.c`

 * *Files 3% similar despite different names*

```diff
@@ -292,48 +292,48 @@
     const uint8_t *tail = (const uint8_t *)(data + nblocks * 16);
 
     uint64_t k1 = 0;
     uint64_t k2 = 0;
 
     switch (len & 15) {
         case 15:
-            k2 ^= (uint64_t)tail[14] << 48;
+            k2 ^= ((uint64_t)tail[14]) << 48;
         case 14:
-            k2 ^= (uint64_t)tail[13] << 40;
+            k2 ^= ((uint64_t)tail[13]) << 40;
         case 13:
-            k2 ^= (uint64_t)tail[12] << 32;
+            k2 ^= ((uint64_t)tail[12]) << 32;
         case 12:
-            k2 ^= (uint64_t)tail[11] << 24;
+            k2 ^= ((uint64_t)tail[11]) << 24;
         case 11:
-            k2 ^= (uint64_t)tail[10] << 16;
+            k2 ^= ((uint64_t)tail[10]) << 16;
         case 10:
-            k2 ^= (uint64_t)tail[9] << 8;
+            k2 ^= ((uint64_t)tail[9]) << 8;
         case 9:
-            k2 ^= (uint64_t)tail[8] << 0;
+            k2 ^= ((uint64_t)tail[8]) << 0;
             k2 *= c2;
             k2 = ROTL64(k2, 33);
             k2 *= c1;
             h2 ^= k2;
 
         case 8:
-            k1 ^= (uint64_t)tail[7] << 56;
+            k1 ^= ((uint64_t)tail[7]) << 56;
         case 7:
-            k1 ^= (uint64_t)tail[6] << 48;
+            k1 ^= ((uint64_t)tail[6]) << 48;
         case 6:
-            k1 ^= (uint64_t)tail[5] << 40;
+            k1 ^= ((uint64_t)tail[5]) << 40;
         case 5:
-            k1 ^= (uint64_t)tail[4] << 32;
+            k1 ^= ((uint64_t)tail[4]) << 32;
         case 4:
-            k1 ^= (uint64_t)tail[3] << 24;
+            k1 ^= ((uint64_t)tail[3]) << 24;
         case 3:
-            k1 ^= (uint64_t)tail[2] << 16;
+            k1 ^= ((uint64_t)tail[2]) << 16;
         case 2:
-            k1 ^= (uint64_t)tail[1] << 8;
+            k1 ^= ((uint64_t)tail[1]) << 8;
         case 1:
-            k1 ^= (uint64_t)tail[0] << 0;
+            k1 ^= ((uint64_t)tail[0]) << 0;
             k1 *= c1;
             k1 = ROTL64(k1, 31);
             k1 *= c2;
             h1 ^= k1;
     };
 
     //----------
```

### Comparing `mmh3-4.0.0/src/mmh3.egg-info/PKG-INFO` & `mmh3-4.0.1/src/mmh3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmh3
-Version: 4.0.0
+Version: 4.0.1
 Summary: Python extension for MurmurHash (MurmurHash3), a set of fast and robust hash functions.
 Author-email: Hajime Senuma <hajime.senuma@gmail.com>
 License: MIT License
         
         Copyright (c) 2011-2023 Hajime Senuma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,15 +113,15 @@
 ```
 
 ### `hashlib`-style hashers
 `mmh3` implements hashers whose interfaces are similar to `hashlib` in the standard library: `mmh3_32()` for 32 bit hashing, `mmh3_x64_128()` for 128 bit hashing optimized for x64 architectures, and `mmh3_x86_128()` for 128 bit hashing optimized for x86 architectures.
 
 In addition to the standard `digest()` method, each hasher has `sintdigest()`, which returns a signed integer, and `uintdigest()`, which returns an unsigned integer. 128 bit hashers also have `stupledigest()` and `utupledigest()` which return two 64 bit integers.
 
-Note that as of version 4.0.0, the implementation is still experimental and its performance can be unsatisfactory (especially `mmh3_x86_128()`). Also, `hexdigest()` is not supported. Use `digest().hex()` instead.
+Note that as of version 4.0.1, the implementation is still experimental and its performance can be unsatisfactory (especially `mmh3_x86_128()`). Also, `hexdigest()` is not supported. Use `digest().hex()` instead.
 
 ```shell
 >>> import mmh3
 >>> hasher = mmh3.mmh3_x64_128(seed=42)
 >>> hasher.update(b"foo")
 >>> hasher.update(b"bar")
 >>> hasher.update("foo") # str inputs are not allowed for hashers
@@ -137,14 +137,18 @@
 >>> hasher.stupledigest() # two 64 bit signed ints
 (7689522670935629698, -159584473158936081)
 >>> hasher.utupledigest() # two 64 bit unsigned ints
 (7689522670935629698, 18287159600550615535)
 ```
 
 ## Changelog
+### 4.0.1 (2023-07-14)
+* Fix incorrect type hints.
+* Refactor the project structure (<https://github.com/hajimes/mmh3/issues/48>).
+
 ### 4.0.0 (2023-05-22)
 * Add experimental support for `hashlib`-compliant hasher classes (<https://github.com/hajimes/mmh3/issues/39>). Note that they are not yet fully tuned for performance.
 * Add support for type hints (<https://github.com/hajimes/mmh3/issues/44>).
 * Add wheels for more platforms (`musllinux`, `s390x`, `win_arm64`, and `macosx_universal2`).
 * Drop support for Python 3.7, as it will reach the end of life on 2023-06-27.
 * Switch license from CC0 to MIT (<https://github.com/hajimes/mmh3/issues/43>).
 * Add a code of conduct (the ACM Code of Ethics and Professional Conduct).
@@ -155,22 +159,14 @@
 ### 3.1.0 (2023-03-24)
 * Add support for Python 3.10 and 3.11. Thanks [wouter bolsterlee](https://github.com/wbolster) and [Dušan Nikolić](https://github.com/n-dusan)!
 * Drop support for Python 3.6; remove legacy code for Python 2.x at the source code level.
 * Add support for 32-bit architectures such as `i686` and `armv7l`. From now on, `hash` and `hash_from_buffer` on these architectures will generate the same hash values as those on other environments. Thanks [Danil Shein](https://github.com/dshein-alt)!
 * In relation to the above, `manylinux2014_i686` wheels are now available.
 * Support for hashing huge data (>16GB). Thanks [arieleizenberg](https://github.com/arieleizenberg)!
 
-### 3.0.0 (2021-02-23)
-* Python wheels are now available, thanks to the power of [cibuildwheel](https://github.com/joerick/cibuildwheel).
-  * Supported platforms are `manylinux1_x86_64`, `manylinux2010_x86_64`, `manylinux2014_aarch64`, `win32`, `win_amd64`, `macosx_10_9_x86_64`, and `macosx_11_0_arm64` (Apple Silicon).
-* Add support for newer macOS environments. Thanks [Matthew Honnibal](https://github.com/honnibal)!
-* Drop support for Python 2.7, 3.3, 3.4, and 3.5.
-* Add support for Python 3.7, 3.8, and 3.9.
-* Migrate CI from Travis CI and AppVeyor to GitHub Actions.
-
 See [CHANGELOG.md](./CHANGELOG.md) for the complete changelog.
 
 ## License
 [MIT](./LICENSE), unless otherwise noted within a file.
 
 ## Known Issues
 ### Getting different results from other MurmurHash3-based libraries
```

