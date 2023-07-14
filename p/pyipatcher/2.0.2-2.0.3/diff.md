# Comparing `tmp/pyipatcher-2.0.2.tar.gz` & `tmp/pyipatcher-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipatcher-2.0.2.tar", max compression
+gzip compressed data, was "pyipatcher-2.0.3.tar", max compression
```

## Comparing `pyipatcher-2.0.2.tar` & `pyipatcher-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-2.0.2/LICENSE
--rw-r--r--   0        0        0     1029 2023-06-10 14:08:14.786228 pyipatcher-2.0.2/README.md
--rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-2.0.2/pyipatcher/__init__.py
--rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-2.0.2/pyipatcher/__main__.py
--rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-2.0.2/pyipatcher/cli/ibootpatcher.py
--rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-2.0.2/pyipatcher/cli/kernelpatcher.py
--rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-2.0.2/pyipatcher/cli/ramdiskpatcher.py
--rw-r--r--   0        0        0     9635 2023-07-14 15:41:58.612124 pyipatcher-2.0.2/pyipatcher/ipatcher.py
--rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-2.0.2/pyipatcher/logger.py
--rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-2.0.2/pyipatcher/patchfinder/asrpatchfinder.py
--rw-r--r--   0        0        0    23969 2023-07-14 16:55:05.710118 pyipatcher-2.0.2/pyipatcher/patchfinder/ibootpatchfinder.py
--rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-2.0.2/pyipatcher/patchfinder/insn.py
--rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-2.0.2/pyipatcher/patchfinder/kernelpatchfinder.py
--rw-r--r--   0        0        0     5542 2023-06-07 03:32:51.657221 pyipatcher-2.0.2/pyipatcher/patchfinder/patchfinder64.py
--rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-2.0.2/pyipatcher/patchfinder/rextpatchfinder.py
--rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-2.0.2/pyipatcher/wikiproxy.py
--rw-r--r--   0        0        0      927 2023-07-14 16:50:00.578118 pyipatcher-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 pyipatcher-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-2.0.3/LICENSE
+-rw-r--r--   0        0        0     1029 2023-06-10 14:08:14.786228 pyipatcher-2.0.3/README.md
+-rw-r--r--   0        0        0      200 2023-06-10 09:58:56.044644 pyipatcher-2.0.3/pyipatcher/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-07 05:10:10.736779 pyipatcher-2.0.3/pyipatcher/__main__.py
+-rw-r--r--   0        0        0     2740 2023-06-09 12:31:48.365994 pyipatcher-2.0.3/pyipatcher/cli/ibootpatcher.py
+-rw-r--r--   0        0        0     2231 2023-06-09 12:31:43.011240 pyipatcher-2.0.3/pyipatcher/cli/kernelpatcher.py
+-rw-r--r--   0        0        0     1529 2023-06-09 12:31:43.012870 pyipatcher-2.0.3/pyipatcher/cli/ramdiskpatcher.py
+-rw-r--r--   0        0        0     9635 2023-07-14 16:58:28.682318 pyipatcher-2.0.3/pyipatcher/ipatcher.py
+-rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-2.0.3/pyipatcher/logger.py
+-rw-r--r--   0        0        0     1509 2023-06-10 13:49:18.286869 pyipatcher-2.0.3/pyipatcher/patchfinder/asrpatchfinder.py
+-rw-r--r--   0        0        0    24278 2023-07-14 18:41:38.842414 pyipatcher-2.0.3/pyipatcher/patchfinder/ibootpatchfinder.py
+-rw-r--r--   0        0        0     8738 2023-06-07 11:30:09.571267 pyipatcher-2.0.3/pyipatcher/patchfinder/insn.py
+-rwxr-xr-x   0        0        0     5187 2023-06-10 13:49:18.294098 pyipatcher-2.0.3/pyipatcher/patchfinder/kernelpatchfinder.py
+-rw-r--r--   0        0        0     5674 2023-07-14 18:28:45.385682 pyipatcher-2.0.3/pyipatcher/patchfinder/patchfinder64.py
+-rw-r--r--   0        0        0     2084 2023-06-10 13:49:18.295150 pyipatcher-2.0.3/pyipatcher/patchfinder/rextpatchfinder.py
+-rw-r--r--   0        0        0     1827 2023-06-10 12:50:47.362374 pyipatcher-2.0.3/pyipatcher/wikiproxy.py
+-rw-r--r--   0        0        0      927 2023-07-14 18:26:23.780851 pyipatcher-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 pyipatcher-2.0.3/PKG-INFO
```

### Comparing `pyipatcher-2.0.2/LICENSE` & `pyipatcher-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/README.md` & `pyipatcher-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/cli/ibootpatcher.py` & `pyipatcher-2.0.3/pyipatcher/cli/ibootpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/cli/kernelpatcher.py` & `pyipatcher-2.0.3/pyipatcher/cli/kernelpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/cli/ramdiskpatcher.py` & `pyipatcher-2.0.3/pyipatcher/cli/ramdiskpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/ipatcher.py` & `pyipatcher-2.0.3/pyipatcher/ipatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/logger.py` & `pyipatcher-2.0.3/pyipatcher/logger.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/patchfinder/asrpatchfinder.py` & `pyipatcher-2.0.3/pyipatcher/patchfinder/asrpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/patchfinder/ibootpatchfinder.py` & `pyipatcher-2.0.3/pyipatcher/patchfinder/ibootpatchfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 class ibootpatchfinder(patchfinder64):
     def __init__(self, buf: bytes, verbose: bool):
         super().__init__(buf)
         self.verbose = verbose
         logger = get_my_logger(self.verbose, name='ibootpatchfinder')
         self.vers, self.minor_vers = self.get_iboot_ver()
         logger.debug(f'iBoot-{self.vers} inputted')
+        if self.vers >= 6671:
+            if 8419 <= self.vers <= 9000:
+                logger.info('iOS 16 iBoot detected!')
+            elif 7429 <= self.vers < 8419:
+                logger.info('iOS 15 iBoot detected!')
+            elif self.vers < 7429:
+                logger.info('iOS 14 iBoot detected!')
         if self.vers < 3406:
             raise NotImplementedError(f'Unsupported iBoot (iBoot-{self.vers}.{self.minor_vers}), only iOS 10 or later iBoot is supported')
         self.stage1 = (self._buf[0x200:0x200+5] == b'iBSS' or self._buf[0x200:0x200+11] == b'iBootStage1')
         logger.debug(f'stage1={self.stage1}')
         self.stage2 = (self._buf[0x200:0x200+5] == b'iBEC' or self._buf[0x200:0x200+11] == b'iBootStage2')
         logger.debug(f'stage2={self.stage2}')
         self.cpid = 0
@@ -392,15 +399,15 @@
                     logger.error('Could not find img4interposercallback_ret2')
                     return -1
                 logger.debug(f'img4interposercallback_ret2={hex(img4interposercallback_ret2 + self.base)}')
                 self.apply_patch(img4interposercallback_ret2 - 4, b'\x00\x00\x80\xD2')
             else:
                 self.apply_patch(img4interposercallback_ret - 4, b'\x00\x00\x80\xD2')
                 boff = self.step_back(real_img4interposercallback, real_img4interposercallback, 0x14000000, 0xFC000000)
-                if self.step_back(boff, boff, 0xa94000f0, 0xfff000f0) == 0:
+                if self.step_back(boff, 4, 0xa94000f0, 0xfff000f0) == 0:
                     boff = self.step_back(real_img4interposercallback, real_img4interposercallback, 0x14000000, 0xFC000000)                
                     if self.step_back(boff, boff, 0xa94000f0, 0xfff000f0) == 0:
                         logger.error('img4interposercallback couldn\'t find branch for ret2')
                         return -1
                     else:
                         img4interposercallback_mov_x20 = self.step_back(boff, boff, 0xd2000000, 0xff000000)
                         logger.debug(f'img4interposercallback_mov_x20={hex(img4interposercallback_mov_x20 + self.base)}')
```

### Comparing `pyipatcher-2.0.2/pyipatcher/patchfinder/insn.py` & `pyipatcher-2.0.3/pyipatcher/patchfinder/insn.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/patchfinder/kernelpatchfinder.py` & `pyipatcher-2.0.3/pyipatcher/patchfinder/kernelpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/patchfinder/patchfinder64.py` & `pyipatcher-2.0.3/pyipatcher/patchfinder/patchfinder64.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import sys
 import binascii
 
 def BIT_RANGE(v, begin, end):   return (v >> begin) % (1 << (end - begin + 1))
 def BIT_AT(v, pos): return (v >> pos) % 2
 def SET_BITS(v, begin): return v << begin
 
+def log(msg):
+    print(f'patchfinder64: [DEBUG] {msg}')
+
 def arm64_branch_instruction(_from, to):
     _from = ctypes.c_ulonglong(_from).value
     to = ctypes.c_ulonglong(to).value
     return ctypes.c_uint(int(0x18000000 - (_from - to) / 4 if _from > to else 0x14000000 + (to - _from) / 4)).value
 
 class patchfinder64:
     def __init__(self, buf):
@@ -134,14 +137,15 @@
             if op & 0x7C000000 == 0x14000000:
                 where = self.follow_call(i)
                 if where == what:
                     return i
         return 0
 
     def apply_patch(self, where, patch):
+        log(f'Applying patch at {hex(where)}: {binascii.hexlify(patch)}')
         self._buf[where:where+len(patch)] = patch
 
 
 def test():
     #set_package_name("test")
     kernel = open("kcache.raw", "rb").read()
     pf = patchfinder64(kernel)
```

### Comparing `pyipatcher-2.0.2/pyipatcher/patchfinder/rextpatchfinder.py` & `pyipatcher-2.0.3/pyipatcher/patchfinder/rextpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyipatcher/wikiproxy.py` & `pyipatcher-2.0.3/pyipatcher/wikiproxy.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-2.0.2/pyproject.toml` & `pyipatcher-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyipatcher"
-version = "2.0.2"
+version = "2.0.3"
 description = "iOS ARM64 patchfinder & iOS ARM64 bootchain patcher"
 authors = ["mini_exploit <61931266+Mini-Exploit@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/Mini-Exploit/pyipatcher"
 
 [tool.poetry.dependencies]
```

### Comparing `pyipatcher-2.0.2/PKG-INFO` & `pyipatcher-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipatcher
-Version: 2.0.2
+Version: 2.0.3
 Summary: iOS ARM64 patchfinder & iOS ARM64 bootchain patcher
 Home-page: https://github.com/Mini-Exploit/pyipatcher
 License: GPL-3.0-only
 Author: mini_exploit
 Author-email: 61931266+Mini-Exploit@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

