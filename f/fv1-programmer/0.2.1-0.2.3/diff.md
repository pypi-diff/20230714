# Comparing `tmp/fv1_programmer-0.2.1.tar.gz` & `tmp/fv1_programmer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.1.tar", max compression
+gzip compressed data, was "fv1_programmer-0.2.3.tar", max compression
```

## Comparing `fv1_programmer-0.2.1.tar` & `fv1_programmer-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/LICENSE
--rw-r--r--   0        0        0     1693 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/adaptor/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/adaptor/mcp2221.py
--rw-r--r--   0        0        0        0 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/eeprom/__init__.py
--rw-r--r--   0        0        0     5331 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/eeprom/eeprom.py
--rw-r--r--   0        0        0        0 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/fv1_programmer/__init__.py
--rw-r--r--   0        0        0     2896 2023-05-24 02:08:12.341973 fv1_programmer-0.2.1/fv1_programmer/main.py
--rw-r--r--   0        0        0     1203 2023-05-24 02:08:12.345973 fv1_programmer-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 fv1_programmer-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/LICENSE
+-rw-r--r--   0        0        0      613 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/README.md
+-rw-r--r--   0        0        0     1140 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2023-07-14 01:34:50.892645 fv1_programmer-0.2.3/asfv1/.git
+-rw-r--r--   0        0        0     1157 2023-07-14 01:34:51.748662 fv1_programmer-0.2.3/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-07-14 01:34:51.748662 fv1_programmer-0.2.3/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2023-07-14 01:34:51.748662 fv1_programmer-0.2.3/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2023-07-14 01:34:51.752662 fv1_programmer-0.2.3/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2023-07-14 01:34:51.752662 fv1_programmer-0.2.3/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2023-07-14 01:34:51.752662 fv1_programmer-0.2.3/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2023-07-14 01:34:51.168650 fv1_programmer-0.2.3/disfv1/.git
+-rw-r--r--   0        0        0     1157 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/setup.py
+-rw-r--r--   0        0        0     6747 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1780 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3429 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/main.py
+-rw-r--r--   0        0        0     2906 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    13468 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1274 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 fv1_programmer-0.2.3/PKG-INFO
```

### Comparing `fv1_programmer-0.2.1/LICENSE` & `fv1_programmer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.1/adaptor/adapter.py` & `fv1_programmer-0.2.3/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.1/adaptor/mcp2221.py` & `fv1_programmer-0.2.3/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.1/eeprom/eeprom.py` & `fv1_programmer-0.2.3/eeprom/eeprom.py`

 * *Files 23% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     @staticmethod
     def ensure_bytes(data):
         if type(data) == bytes:
             return data
         elif type(data) == int:
             return bytes([data])
-        elif type(data) == list:
+        elif type(data) in [list, bytearray]:
             return bytes(data)
         raise ValueError("Invalid data format. Acceptable values are int, list or bytes.")
 
     @staticmethod
     def split_transaction(max_size, start_address, total_bytes):
         """
         Splits a large transaction into max_size-aligned transactions.
@@ -142,7 +142,48 @@
 
     def write_bytes(self, byte_address, byte_list):
         # Perform the write, split on page boundaries
         for _addr, _offset, _len in EEPROM.split_transaction(self.page_size, byte_address, len(byte_list)):
             # logger.debug(_addr, _offset, _len)
             self.adaptor.write_bytes(_addr.to_bytes(2, 'big') + EEPROM.ensure_bytes(byte_list[_offset:_offset+_len]))
 
+
+class DummyEEPROM(EEPROM):
+    def __init__(self, filepath : Path, min_size : int, fill_byte : int=0xFF) -> None:
+        self.data = [fill_byte]*min_size
+        self.filepath = filepath
+        self.fill_byte = fill_byte
+
+        # Initialize from file, if it exists
+        if self.filepath.exists() and self.filepath.is_file():
+            with open(self.filepath, 'rb') as f:
+                _data = f.read()
+                self._ensure_length(len(_data))
+                self.data[0:len(_data)] = _data
+
+    @property
+    def size(self,):
+        return len(self.data)
+
+    @property
+    def page_size(self,):
+        return self.size
+
+    def _resize(self, new_size):
+        l = [self.fill_byte]*max(new_size, len(self.data))
+        l[0:len(self.data)] = self.data
+        self.data = l
+
+    def _ensure_length(self, min_length):
+        if len(self.data) < min_length:
+            self._resize(min_length)
+
+    def read_bytes(self, byte_address, num_bytes):
+        self._ensure_length(byte_address + num_bytes)
+        return bytes(self.data[byte_address:byte_address + num_bytes])
+
+    def write_bytes(self, byte_address, byte_list):
+        _data = EEPROM.ensure_bytes(byte_list)
+        self._ensure_length(byte_address + len(_data))
+        self.data[byte_address:byte_address + len(byte_list)] = _data
+        with open(self.filepath, 'wb') as f:
+            f.write(bytes(self.data))
```

### Comparing `fv1_programmer-0.2.1/pyproject.toml` & `fv1_programmer-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.1"
+version = "0.2.3"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -19,21 +19,24 @@
     "Typing :: Typed",
 ]
 
 packages = [
     {include = "fv1_programmer"},
     {include = "eeprom"},
     {include = "adaptor"},
+    {include = "asfv1"},
+    {include = "disfv1"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-# textual = {extras = ["dev"], version = "^0.7.0"}
+textual = {extras = ["dev"], version = "^0.28.1"}
 easymcp2221 = "^1.6.2"
 intelhex = "^2.3.0"
+pyperclip = "^1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
```

