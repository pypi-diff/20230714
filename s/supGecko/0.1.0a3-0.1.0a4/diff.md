# Comparing `tmp/supGecko-0.1.0a3.tar.gz` & `tmp/supGecko-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supGecko-0.1.0a3.tar", last modified: Tue Jul 11 17:14:48 2023, max compression
+gzip compressed data, was "supGecko-0.1.0a4.tar", last modified: Fri Jul 14 11:43:34 2023, max compression
```

## Comparing `supGecko-0.1.0a3.tar` & `supGecko-0.1.0a4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.815069 supGecko-0.1.0a3/
--rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supGecko-0.1.0a3/LICENSE
--rw-rw-rw-   0        0        0      694 2023-07-11 17:14:48.815069 supGecko-0.1.0a3/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supGecko-0.1.0a3/README.md
--rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supGecko-0.1.0a3/pyproject.toml
--rw-rw-rw-   0        0        0      623 2023-07-11 17:14:48.818068 supGecko-0.1.0a3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.802068 supGecko-0.1.0a3/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.807070 supGecko-0.1.0a3/src/supGecko/
--rw-rw-rw-   0        0        0       88 2023-07-11 16:14:27.000000 supGecko-0.1.0a3/src/supGecko/__init__.py
--rw-rw-rw-   0        0        0     2675 2023-07-11 17:13:46.000000 supGecko-0.1.0a3/src/supGecko/asm.py
--rw-rw-rw-   0        0        0     9895 2023-07-11 17:12:22.000000 supGecko-0.1.0a3/src/supGecko/gecko.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:14:48.814068 supGecko-0.1.0a3/src/supGecko.egg-info/
--rw-rw-rw-   0        0        0      694 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 17:14:48.000000 supGecko-0.1.0a3/src/supGecko.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.402558 supGecko-0.1.0a4/
+-rw-rw-rw-   0        0        0     1083 2023-07-11 07:31:46.000000 supGecko-0.1.0a4/LICENSE
+-rw-rw-rw-   0        0        0      694 2023-07-14 11:43:34.402558 supGecko-0.1.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-11 07:41:27.000000 supGecko-0.1.0a4/README.md
+-rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supGecko-0.1.0a4/pyproject.toml
+-rw-rw-rw-   0        0        0      623 2023-07-14 11:43:34.404562 supGecko-0.1.0a4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.379558 supGecko-0.1.0a4/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.395558 supGecko-0.1.0a4/src/supGecko/
+-rw-rw-rw-   0        0        0       88 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/__init__.py
+-rw-rw-rw-   0        0        0     2840 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/asm.py
+-rw-rw-rw-   0        0        0      359 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/consts.py
+-rw-rw-rw-   0        0        0     8591 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/gecko.py
+-rw-rw-rw-   0        0        0     1381 2023-07-14 11:34:52.000000 supGecko-0.1.0a4/src/supGecko/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:43:34.401561 supGecko-0.1.0a4/src/supGecko.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 11:43:34.000000 supGecko-0.1.0a4/src/supGecko.egg-info/top_level.txt
```

### Comparing `supGecko-0.1.0a3/LICENSE` & `supGecko-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `supGecko-0.1.0a3/PKG-INFO` & `supGecko-0.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supGecko
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A helper library to write Gecko code
 Home-page: https://github.com/sup39/supGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supGecko/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supGecko-0.1.0a3/setup.cfg` & `supGecko-0.1.0a4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7570 4765 636b 6f0d 0a76 6572   = supGecko..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 6133 0d0a  sion = 0.1.0a3..
+00000020: 7369 6f6e 203d 2030 2e31 2e30 6134 0d0a  sion = 0.1.0a4..
 00000030: 6175 7468 6f72 203d 2073 7570 3339 0d0a  author = sup39..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
 00000050: 6d73 4073 7570 3339 2e64 6576 0d0a 6465  ms@sup39.dev..de
 00000060: 7363 7269 7074 696f 6e20 3d20 4120 6865  scription = A he
 00000070: 6c70 6572 206c 6962 7261 7279 2074 6f20  lper library to 
 00000080: 7772 6974 6520 4765 636b 6f20 636f 6465  write Gecko code
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `supGecko-0.1.0a3/src/supGecko/asm.py` & `supGecko-0.1.0a4/src/supGecko/asm.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,26 @@
 
 def system(argv, *args, **kwargs):
   r = subprocess.run(argv, *args, capture_output=True, text=True, **kwargs)
   if r.returncode:
     raise Exception(f'Fail to run {argv[0]} (code={r.returncode}): {r.stderr}')
   return r.stdout
 
+def write_extra_input(x, file):
+  if type(x) == str:
+    print(x, file=file)
+  else:
+    for line in x:
+      print(line, file=file)
+
 def compile(
   input_path, addr=None,
   extra_c_flags=[],
-  extra_as_input='', extra_as_flags=[],
-  extra_ld_input='', extra_ld_flags=[],
+  extra_as_input=[], extra_as_flags=[],
+  extra_ld_input=[], extra_ld_flags=[],
 ):
   distDir = tempfile.mkdtemp()
   distASM, distOBJ, distLD, distLOBJ, distBIN = (f'{distDir}/_.{ext}' for ext in ['s', 'o', 'ld', 'l.o', 'bin'])
 
   try:
     input_name = input_path.rsplit('.', 1)[0]
 
@@ -37,15 +44,15 @@
         '-c', '-o', distOBJ,
         *extra_c_flags,
         input_path,
       ])
     else: # treat as ASM file
       # make ASM file
       with open(distASM, 'w') as fw, open(input_path, 'r') as fr:
-        print(extra_as_input, file=fw)
+        write_extra_input(extra_as_input, file=fw)
         for line in fr: fw.write(line)
       # assemble to OBJ
       system([
         'powerpc-eabi-as',
         '-mregnames', '-mgekko',
         '-o', distOBJ,
         *extra_as_flags,
@@ -61,15 +68,15 @@
           fw.write(f.read())
       ## section
       print('SECTIONS {', file=fw)
       if addr is not None: print(f'  . = {addr};', file=fw)
       print('  .text : ALIGN(4) { *(.text) }', file=fw)
       if addr is not None: print('.rodata : ALIGN(4) { *(.rodata) }', file=fw)
       print('}', file=fw)
-      print(extra_ld_input, file=fw)
+      write_extra_input(extra_ld_input, file=fw)
     system([
       'powerpc-eabi-ld',
       '-o', distLOBJ,
       '-T', distLD,
       *extra_ld_flags,
       distOBJ,
     ])
```

### Comparing `supGecko-0.1.0a3/src/supGecko/gecko.py` & `supGecko-0.1.0a4/src/supGecko/gecko.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,34 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2023 sup39
 
 from .asm import compile
-
-def cw_addr(ct, addr, po, endif=False):
-  return (ct+0x10 if po else ct)<<24 | (addr+1 if endif else addr)&0x1ff_ffff
-def cw_go(ct, if_, n):
-  return ct<<24 | [True, False, None].index(if_)<<20 | n&0xffff
-def parse_regop(ct, lhs, op, rhs):
-  if op.endswith('='): op = op[:-1] # drop trailing =
-  lhs, lhs_flag = parse_bracket_operand(lhs, 'lhs')
-  rhs, rhs_flag = parse_bracket_operand(rhs, 'rhs')
-  cw = ct<<24 | REGOP_IDX[op]<<20 | lhs_flag<<16 | rhs_flag<<17 | lhs&0xf
-  return cw, rhs
-def parse_regidx(ct, x, name):
-  if x == 'ba': x = 0xf
-  elif x == 'po': x = 0xf; ct |= 0x10
-  else: x &= 0xf; assert x!=0xf, f'{name} cannot be F'
-  return ct, x
-def parse_bracket_operand(x, name): # returns (value, hasBracket)
-  if type(x) == list:
-    assert len(x)==1, f'`{name}` must be "x" or "[x]"'
-    return x, 1
-  return x, 0
-def make_asm_code(input_path, raw, kwargs):
-  if raw is not None: # raw code
-    code = parse_binarg(raw)
-    assert len(code)%4 == 0, \
-      f'len(raw) should a multiple of 4, got {len(raw)}'
-  else: # compile from file
-    assert input_path is not None, 'either `input_path` or `raw` should be set'
-    code, symbols = compile(input_path, **kwargs)
-  return code
-
-parse_binarg = lambda x: \
-  b''.join(map(parse_binarg, x)) if type(x)==list else \
-  bytes.fromhex(x) if type(x)==str else \
-    x.to_bytes(4, 'big') if type(x)==int else x
-
-CMP_IDX = {'==': 0, '!=': 2, '>': 4, '<': 6}
-UNIT_IDX = {
-   8: 0, 'b': 0, 'byte': 0,
-  16: 1, 'h': 1, 'halfword': 1,
-  32: 2, 'w': 2, 'word': 2,
-}
-REGOP_IDX = {
-  'add': 0, '+': 0,
-  'mul': 1, '*': 1,
-  'or' : 2, '|': 2,
-  'and': 3, '&': 3,
-  'xor': 4, '^': 4,
-  'slw': 5, '<<': 5,
-  'srw': 6, '>>': 6,
-  'rol': 7,
-  'asr': 8,
-  'fadds': 9,
-  'fmuls': 10,
-}
+from .utils import *
+from .consts import *
 
 # TODO: assert range of arg
 class Gecko():
-  def __init__(self):
+  def __init__(self, compile_flags={}):
     self.code = bytearray()
+    self.compile_flags = compile_flags
   def append(self, *payloads):
     self.code += b''.join(map(parse_binarg, payloads))
     return self
   def dump_txt(self, indent=''):
     if type(indent) == int: indent = ' '*indent
     return '\n'.join(
       indent+' '.join(self.code[j:j+4].hex().upper() for j in [i, i+4])
       for i in range(0, len(self.code), 8)
     )
+  def compile(self, input_path, addr=None, **kwargs0):
+    kwargs = {'extra_'+k: v for k, v in self.compile_flags.items()}
+    for k, v in kwargs0.items():
+      if type(v) == str: v = [v]
+      kwargs[k] = kwargs[k] + v if k in kwargs else v
+    return compile(input_path, addr, **kwargs)
   ''' 00 '''
   def write8(self, addr, val, count=1, po=False):
     return self.append(
       cw_addr(0x00, addr, po),
       ((count-1)&0xffff) << 16 | val&0xff,
     )
   ''' 02 '''
@@ -231,21 +185,21 @@
     T = (8 if reset_on_true else 0) + (1 if endif else 0)
     return self.append(
       (0xA8 | CMP_IDX[op])<<24 | (cnt&0xffff)<<4 | T,
       ~mask<<16 | val&0xffff,
     )
   ''' C0 '''
   def C0(self, input_path=None, raw=None, **kwargs):
-    code = make_asm_code(input_path, raw, kwargs)
+    code = make_asm_code(self.compile, input_path, raw, kwargs)
     if len(code)%8 == 4: # pad code with blr
       code += b'\x4E\x80\x00\x20'
     return self.append(0xC000_0000, len(code)>>3, code)
   ''' C2 '''
   def C2(self, addr, input_path, raw=None, po=False, **kwargs):
-    code = make_asm_code(input_path, raw, kwargs)
+    code = make_asm_code(self.compile, input_path, raw, kwargs)
     if len(code)%8 == 0: # pad code with nop
       code += b'\x60\x00\x00\x00'
     code += b'\x00\x00\x00\x00' # append 0
     return self.append(cw_addr(0xC2, addr, po), len(code)>>3, code)
   ''' C6 '''
   def branch(self, addr, dst, po=False):
     return self.append(cw_addr(0xC6, addr, po), dst&0xffffffff)
@@ -272,15 +226,15 @@
     )
   ''' F0 '''
   def end_of_code(self):
     return self.append(0xF000_0000, 0)
 
   ''' C Kit '''
   def c_kit(self, addr_code, input_path, entries, **kwargs):
-    code, symbols = compile(input_path, addr_code, **kwargs)
+    code, symbols = self.compile(input_path, addr_code, **kwargs)
     # 06
     self.write_string(addr_code, code, po=False)
     # 04/C6
     for addr_src, action, name in entries:
       assert name in symbols, f'symbol "{name}" is not found in the .text section of {input_path}'
       addr_dst = symbols[name]
       if action == 'b':
```

### Comparing `supGecko-0.1.0a3/src/supGecko.egg-info/PKG-INFO` & `supGecko-0.1.0a4/src/supGecko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supGecko
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A helper library to write Gecko code
 Home-page: https://github.com/sup39/supGecko
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supGecko/issues
 Classifier: Programming Language :: Python :: 3
```

