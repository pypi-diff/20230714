# Comparing `tmp/python-fspacker-0.3.1.tar.gz` & `tmp/python-fspacker-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-fspacker-0.3.1.tar", last modified: Wed Nov 16 09:45:38 2022, max compression
+gzip compressed data, was "python-fspacker-0.3.2.tar", last modified: Fri Jul 14 15:25:10 2023, max compression
```

## Comparing `python-fspacker-0.3.1.tar` & `python-fspacker-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:38.403810 python-fspacker-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10866 2022-11-16 09:45:38.403810 python-fspacker-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8642 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:38.399809 python-fspacker-0.3.1/fsPacker/
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    52582 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/_fspacker.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/_fspacker.h
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/_fspacker.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:38.399809 python-fspacker-0.3.1/fsPacker/clinic/
--rw-r--r--   0 runner    (1001) docker     (121)     9313 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/clinic/_fspacker.cpp.h
--rw-r--r--   0 runner    (1001) docker     (121)    10258 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/fallback.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:38.399809 python-fspacker-0.3.1/fsPacker/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/fsPacker/test/fsPacker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 09:45:38.399809 python-fspacker-0.3.1/python_fspacker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10866 2022-11-16 09:45:38.000000 python-fspacker-0.3.1/python_fspacker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-11-16 09:45:38.000000 python-fspacker-0.3.1/python_fspacker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 09:45:38.000000 python-fspacker-0.3.1/python_fspacker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 09:45:38.000000 python-fspacker-0.3.1/python_fspacker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-16 09:45:38.000000 python-fspacker-0.3.1/python_fspacker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-16 09:45:38.000000 python-fspacker-0.3.1/python_fspacker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 09:45:38.403810 python-fspacker-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-11-16 09:45:34.000000 python-fspacker-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:10.893652 python-fspacker-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-14 15:25:10.893652 python-fspacker-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:10.889652 python-fspacker-0.3.2/fsPacker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/_fspacker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/_fspacker.h
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/_fspacker.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:10.889652 python-fspacker-0.3.2/fsPacker/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/clinic/_fspacker.cpp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:10.889652 python-fspacker-0.3.2/fsPacker/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/fsPacker/test/fsPacker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:10.893652 python-fspacker-0.3.2/python_fspacker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-14 15:25:10.000000 python-fspacker-0.3.2/python_fspacker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-14 15:25:10.000000 python-fspacker-0.3.2/python_fspacker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:25:10.000000 python-fspacker-0.3.2/python_fspacker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:25:10.000000 python-fspacker-0.3.2/python_fspacker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 15:25:10.000000 python-fspacker-0.3.2/python_fspacker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 15:25:10.000000 python-fspacker-0.3.2/python_fspacker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:25:10.893652 python-fspacker-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-14 15:25:05.000000 python-fspacker-0.3.2/setup.py
```

### Comparing `python-fspacker-0.3.1/LICENSE.md` & `python-fspacker-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-fspacker-0.3.1/PKG-INFO` & `python-fspacker-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fspacker
-Version: 0.3.1
+Version: 0.3.2
 Summary: Fusion Solutions message packer
 Home-page: https://github.com/FusionSolutions/python-fspacker
 Author: Andor `iFA` Rajci - Fusions Solutions KFT
 Author-email: ifa@fusionsolutions.io
 License: GPL-3
 Description: [![Python package](https://github.com/FusionSolutions/python-fspacker/actions/workflows/python-package.yml/badge.svg)](https://github.com/FusionSolutions/python-fspacker/actions/workflows/python-package.yml)
         # Fusion Solutions message packer
```

### Comparing `python-fspacker-0.3.1/README.md` & `python-fspacker-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python-fspacker-0.3.1/fsPacker/__init__.py` & `python-fspacker-0.3.2/fsPacker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __doc__ = """
 FS Message Packer v{}
 Copyright (C) 2021 Fusion Solutions KFT <contact@fusionsolutions.io>
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `python-fspacker-0.3.1/fsPacker/_fspacker.cpp` & `python-fspacker-0.3.2/fsPacker/_fspacker.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -873,42 +873,65 @@
 	#if defined(FSPACKER_DEBUG)
 		printf("Packing int...\n");
 	#endif
 	if (sign == 0) {
 		return _fspacker_buffer_append(self->output, &VER2_OP_ZERO_INTERGER, 1);
 	}
 	int isNeg = sign<0;
-	Py_ssize_t nbits = _PyLong_NumBits(obj);
-	Py_ssize_t nbytes = (nbits >> 3)+1;
-	if (nbytes > ITEM_LIMIT) {
-		PyErr_SetString(self->module->PackingError, "Too big integer to pack");
-		return -1;
-	}
 	PyObject *absVal = NULL;
 	unsigned char *pdata = NULL;
 	PyObject *repr = NULL;
+	Py_ssize_t nbits = 0;
+	Py_ssize_t nbytes = 0;
 	switch (_fspacker_packer_ver2_register(self, obj)) {
 		case 1:
 			goto done;
 		case 0:
 			break;
 		case -1:
 			return -1;
 	}
-	repr = PyBytes_FromStringAndSize(NULL, nbytes);
-	if (repr == NULL) {
-		goto memoryError;
-	}
-	pdata = (unsigned char *)PyBytes_AS_STRING(repr);
-	Py_DECREF(repr);
-	absVal = isNeg ? PyNumber_Absolute(obj):NULL;
-	if (_PyLong_AsByteArray((PyLongObject *)(absVal != NULL ? absVal:obj), pdata, nbytes, 1, 0) < 0) {
-		goto memoryError;
+	if ( isNeg ) {
+		absVal = PyNumber_Absolute(obj);
+		if ( absVal == NULL ) {
+			goto memoryError;
+		}
+		nbits = _PyLong_NumBits(absVal);
+		nbytes = (nbits >> 3)+1;
+		if (nbytes > ITEM_LIMIT) {
+			PyErr_SetString(self->module->PackingError, "Too big integer to pack");
+			goto error;
+		}
+		repr = PyBytes_FromStringAndSize(NULL, nbytes);
+		if (repr == NULL) {
+			goto memoryError;
+		}
+		pdata = (unsigned char *)PyBytes_AS_STRING(repr);
+		Py_DECREF(repr);
+		if (_PyLong_AsByteArray((PyLongObject *)(absVal), pdata, nbytes, 1, 0) < 0) {
+			goto memoryError;
+		}
+		Py_DECREF(absVal);
+	} else {
+		nbits = _PyLong_NumBits(obj);
+		nbytes = (nbits >> 3)+1;
+		if (nbytes > ITEM_LIMIT) {
+			PyErr_SetString(self->module->PackingError, "Too big integer to pack");
+			goto error;
+		}
+		repr = PyBytes_FromStringAndSize(NULL, nbytes);
+		if (repr == NULL) {
+			goto memoryError;
+		}
+		pdata = (unsigned char *)PyBytes_AS_STRING(repr);
+		Py_DECREF(repr);
+		if (_PyLong_AsByteArray((PyLongObject *)(obj), pdata, nbytes, 1, 0) < 0) {
+			goto memoryError;
+		}
 	}
-	Py_XDECREF(absVal);
 	if ((nbytes*8)-nbits >= 8 ) {
 		nbytes -= 1;
 	}
 	if (nbytes == 1) {
 		if (_fspacker_buffer_append(self->output, &(isNeg ? VER2_OP_NEG_CHAR_INTERGER:VER2_OP_CHAR_INTERGER), 1) < 0) {
 			goto error;
 		}
```

### Comparing `python-fspacker-0.3.1/fsPacker/_fspacker.pyi` & `python-fspacker-0.3.2/fsPacker/_fspacker.pyi`

 * *Files identical despite different names*

### Comparing `python-fspacker-0.3.1/fsPacker/clinic/_fspacker.cpp.h` & `python-fspacker-0.3.2/fsPacker/clinic/_fspacker.cpp.h`

 * *Files identical despite different names*

### Comparing `python-fspacker-0.3.1/fsPacker/fallback.py` & `python-fspacker-0.3.2/fsPacker/fallback.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 		elif op == self.OP_ZERO_SET:
 			return set()
 		elif op == self.OP_CHAR_INTERGER:
 			r = int.from_bytes(self._read(1), "little")
 		elif op == self.OP_NEG_CHAR_INTERGER:
 			r = -int.from_bytes(self._read(1), "little")
 		elif op == self.OP_SHORT_INTERGER:
-			r = -int.from_bytes(self._read(2), "little")
+			r = int.from_bytes(self._read(2), "little")
 		elif op == self.OP_NEG_SHORT_INTERGER:
 			r = -int.from_bytes(self._read(2), "little")
 		elif op == self.OP_INTERGER:
 			l = self._read_vint()
 			r = int.from_bytes(self._read(l), "little")
 		elif op == self.OP_NEG_INTERGER:
 			l = self._read_vint()
```

### Comparing `python-fspacker-0.3.1/fsPacker/test/fsPacker.py` & `python-fspacker-0.3.2/fsPacker/test/fsPacker.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 		None,
 		True,
 		False,
 		0,
 		-1,
 		1,
 		1<<256,
+		-(1<<256),
 		0.0,
 		0.1,
 		-0.1,
 		1.234e+16,
 		1.234e-16,
 		0.1000000000000001,
 		float("inf"),
@@ -39,16 +40,16 @@
 		b'\xf0\xa4\xad\xa2'.decode(),
 		b"",
 		b"\x00",
 		b"\x00FF00",
 		tuple(),
 		dict(),
 		{"data":"ok"},
-		{1:1},
-		{(1,2,3):1},
+		{None:0, 0:3, -1:4, 1:5, 255:6, -255:7, 0xFFFFFF:8, -0xFFFFFF:9, (1,2):10, 0.1:11, -0.1:12, float("inf"):13, \
+		float("-inf"):14, "":15, "a":16, b"":17, b"a":18 },
 		set(),
 		set([1, "a", "test", "b", b"\x00"]),
 		"F"*65000,
 	)
 	def test_acceleration(self) -> None:
 		self.assertTrue(ACCELERATION_IS_AVAILABLE)
 	def test_refcheck(self) -> None:
```

### Comparing `python-fspacker-0.3.1/python_fspacker.egg-info/PKG-INFO` & `python-fspacker-0.3.2/python_fspacker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fspacker
-Version: 0.3.1
+Version: 0.3.2
 Summary: Fusion Solutions message packer
 Home-page: https://github.com/FusionSolutions/python-fspacker
 Author: Andor `iFA` Rajci - Fusions Solutions KFT
 Author-email: ifa@fusionsolutions.io
 License: GPL-3
 Description: [![Python package](https://github.com/FusionSolutions/python-fspacker/actions/workflows/python-package.yml/badge.svg)](https://github.com/FusionSolutions/python-fspacker/actions/workflows/python-package.yml)
         # Fusion Solutions message packer
```

### Comparing `python-fspacker-0.3.1/setup.py` & `python-fspacker-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 		extra_link_args=EXTRA_LINK_ARGS,
 	)])
 
 pwd = os.path.abspath(os.path.dirname(__file__))
 
 setup(
 	name                          = "python-fspacker",
-	version                       = "0.3.1",
+	version                       = "0.3.2",
 	description                   = "Fusion Solutions message packer",
 	keywords                      = "message pack packer utility fusion solutions fusionsolutions",
 	author                        = "Andor `iFA` Rajci - Fusions Solutions KFT",
 	author_email                  = "ifa@fusionsolutions.io",
 	url                           = "https://github.com/FusionSolutions/python-fspacker",
 	license                       = "GPL-3",
 	ext_modules                   = ext_modules,
@@ -59,8 +59,8 @@
 		"Topic :: Utilities",
 		"Programming Language :: Python :: 3 :: Only",
 		"Programming Language :: Python :: 3.8",
 		"Programming Language :: Python :: 3.9",
 		"Programming Language :: Python :: 3.10",
 		"License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
 	],
-)
+)
```

