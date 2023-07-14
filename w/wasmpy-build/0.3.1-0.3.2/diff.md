# Comparing `tmp/wasmpy-build-0.3.1.tar.gz` & `tmp/wasmpy-build-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-build-0.3.1.tar", last modified: Thu Jul 13 01:50:44 2023, max compression
+gzip compressed data, was "wasmpy-build-0.3.2.tar", last modified: Fri Jul 14 11:04:08 2023, max compression
```

## Comparing `wasmpy-build-0.3.1.tar` & `wasmpy-build-0.3.2.tar`

### file list

```diff
@@ -1,678 +1,682 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:44.055137 wasmpy-build-0.3.1/
--rw-rw-rw-   0        0        0     1068 2023-07-13 01:09:54.000000 wasmpy-build-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1560 2023-07-13 01:50:44.054139 wasmpy-build-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      822 2023-07-13 01:48:26.000000 wasmpy-build-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 01:50:44.055137 wasmpy-build-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-07-13 01:49:39.000000 wasmpy-build-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.153788 wasmpy-build-0.3.1/wasmpy_build/
--rw-rw-rw-   0        0        0     2231 2023-07-13 01:13:45.000000 wasmpy-build-0.3.1/wasmpy_build/__init__.py
--rw-rw-rw-   0        0        0       61 2023-07-13 01:13:42.000000 wasmpy-build-0.3.1/wasmpy_build/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.148788 wasmpy-build-0.3.1/wasmpy_build/include/
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.266321 wasmpy-build-0.3.1/wasmpy_build/include/cp310/
--rw-rw-rw-   0        0        0    13936 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/LICENSE
--rw-rw-rw-   0        0        0     3226 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/Python.h
--rw-rw-rw-   0        0        0      344 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/README.rst
--rw-rw-rw-   0        0        0    31405 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/abstract.h
--rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/bltinmodule.h
--rw-rw-rw-   0        0        0     1224 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/boolobject.h
--rw-rw-rw-   0        0        0     1484 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/bytearrayobject.h
--rw-rw-rw-   0        0        0     2593 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/bytesobject.h
--rw-rw-rw-   0        0        0      720 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cellobject.h
--rw-rw-rw-   0        0        0     5703 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/ceval.h
--rw-rw-rw-   0        0        0     1657 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/classobject.h
--rw-rw-rw-   0        0        0      318 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/code.h
--rw-rw-rw-   0        0        0     7071 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/codecs.h
--rw-rw-rw-   0        0        0      520 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/compile.h
--rw-rw-rw-   0        0        0     1806 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/complexobject.h
--rw-rw-rw-   0        0        0     1962 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/context.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.303396 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/
--rw-rw-rw-   0        0        0    14054 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4119 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1468 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/ceval.h
--rw-rw-rw-   0        0        0     7570 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/compile.h
--rw-rw-rw-   0        0        0     3734 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/dictobject.h
--rw-rw-rw-   0        0        0      723 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4267 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3152 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1630 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/import.h
--rw-rw-rw-   0        0        0     7597 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/initconfig.h
--rw-rw-rw-   0        0        0      387 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1243 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19613 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/object.h
--rw-rw-rw-   0        0        0     3356 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pydebug.h
--rw-rw-rw-   0        0        0     5476 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pyfpe.h
--rw-rw-rw-   0        0        0     2095 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pymem.h
--rw-rw-rw-   0        0        0    11914 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     9196 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pytime.h
--rw-rw-rw-   0        0        0      506 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      404 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/traceback.h
--rw-rw-rw-   0        0        0      975 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    44284 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9635 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/datetime.h
--rw-rw-rw-   0        0        0     3002 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/descrobject.h
--rw-rw-rw-   0        0        0     3853 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/errcode.h
--rw-rw-rw-   0        0        0      831 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/eval.h
--rw-rw-rw-   0        0        0     1098 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/exports.h
--rw-rw-rw-   0        0        0     1571 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/fileobject.h
--rw-rw-rw-   0        0        0      508 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/fileutils.h
--rw-rw-rw-   0        0        0     4360 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/frameobject.h
--rw-rw-rw-   0        0        0     4257 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/funcobject.h
--rw-rw-rw-   0        0        0      334 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/genericaliasobject.h
--rw-rw-rw-   0        0        0     3347 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/genobject.h
--rw-rw-rw-   0        0        0     3026 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/import.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.350394 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/
--rw-rw-rw-   0        0        0      479 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     2971 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    28828 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6457 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16981 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     5271 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0      870 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3484 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      696 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1045 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2809 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      822 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_context.h
--rw-rw-rw-   0        0        0      646 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1704 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      480 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_format.h
--rw-rw-rw-   0        0        0     6859 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      346 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5625 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     9289 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      350 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_list.h
--rw-rw-rw-   0        0        0     2589 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1047 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0     5989 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_object.h
--rw-rw-rw-   0        0        0      626 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_parser.h
--rw-rw-rw-   0        0        0     1981 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2733 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2314 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     4940 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3211 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3938 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4902 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      386 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5578 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      548 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     2970 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      425 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0      898 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0      629 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      633 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/interpreteridobject.h
--rw-rw-rw-   0        0        0      772 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/intrcheck.h
--rw-rw-rw-   0        0        0      593 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/iterobject.h
--rw-rw-rw-   0        0        0     1781 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/longintrepr.h
--rw-rw-rw-   0        0        0     8606 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/longobject.h
--rw-rw-rw-   0        0        0      803 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/marshal.h
--rw-rw-rw-   0        0        0     2764 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/memoryobject.h
--rw-rw-rw-   0        0        0     4147 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/methodobject.h
--rw-rw-rw-   0        0        0    10333 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/modsupport.h
--rw-rw-rw-   0        0        0     2458 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/namespaceobject.h
--rw-rw-rw-   0        0        0    28344 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/object.h
--rw-rw-rw-   0        0        0     8445 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/objimpl.h
--rw-rw-rw-   0        0        0     5509 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/opcode.h
--rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/osmodule.h
--rw-rw-rw-   0        0        0     1302 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/patchlevel.h
--rw-rw-rw-   0        0        0     2474 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/py_curses.h
--rw-rw-rw-   0        0        0     1725 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pycapsule.h
--rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pydtrace.h
--rw-rw-rw-   0        0        0    12426 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyexpat.h
--rw-rw-rw-   0        0        0      466 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyframe.h
--rw-rw-rw-   0        0        0     4223 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyhash.h
--rw-rw-rw-   0        0        0     2080 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymacro.h
--rw-rw-rw-   0        0        0     8315 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymath.h
--rw-rw-rw-   0        0        0     3891 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymem.h
--rw-rw-rw-   0        0        0    31688 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyport.h
--rw-rw-rw-   0        0        0     5250 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystate.h
--rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystrtod.h
--rw-rw-rw-   0        0        0     1110 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pythonrun.h
--rw-rw-rw-   0        0        0     5938 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/pythread.h
--rw-rw-rw-   0        0        0      628 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/rangeobject.h
--rw-rw-rw-   0        0        0     3381 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/sliceobject.h
--rw-rw-rw-   0        0        0     2074 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/structmember.h
--rw-rw-rw-   0        0        0     1390 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/structseq.h
--rw-rw-rw-   0        0        0     1242 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/token.h
--rw-rw-rw-   0        0        0      584 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/tracemalloc.h
--rw-rw-rw-   0        0        0     1614 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/tupleobject.h
--rw-rw-rw-   0        0        0     2460 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/typeslots.h
--rw-rw-rw-   0        0        0    36148 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-05-29 09:08:23.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/warnings.h
--rw-rw-rw-   0        0        0     2863 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp310/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.425430 wasmpy-build-0.3.1/wasmpy_build/include/cp311/
--rw-rw-rw-   0        0        0    13936 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/LICENSE
--rw-rw-rw-   0        0        0     2856 2023-05-29 09:11:37.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/Python.h
--rw-rw-rw-   0        0        0      344 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/README.rst
--rw-rw-rw-   0        0        0    31404 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/abstract.h
--rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/bltinmodule.h
--rw-rw-rw-   0        0        0     1212 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/boolobject.h
--rw-rw-rw-   0        0        0     1462 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/bytearrayobject.h
--rw-rw-rw-   0        0        0     2617 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/bytesobject.h
--rw-rw-rw-   0        0        0     6255 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/ceval.h
--rw-rw-rw-   0        0        0     7071 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/codecs.h
--rw-rw-rw-   0        0        0      520 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/compile.h
--rw-rw-rw-   0        0        0      724 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/complexobject.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.485275 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/
--rw-rw-rw-   0        0        0     8229 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/abstract.h
--rw-rw-rw-   0        0        0     1305 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4568 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/bytesobject.h
--rw-rw-rw-   0        0        0      723 2023-05-29 09:11:33.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/cellobject.h
--rw-rw-rw-   0        0        0     1239 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/ceval.h
--rw-rw-rw-   0        0        0     1656 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/classobject.h
--rw-rw-rw-   0        0        0    11484 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/compile.h
--rw-rw-rw-   0        0        0     1248 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/complexobject.h
--rw-rw-rw-   0        0        0     1959 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/context.h
--rw-rw-rw-   0        0        0     1642 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/descrobject.h
--rw-rw-rw-   0        0        0     3324 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/dictobject.h
--rw-rw-rw-   0        0        0      818 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/fileobject.h
--rw-rw-rw-   0        0        0      232 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/fileutils.h
--rw-rw-rw-   0        0        0      702 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/floatobject.h
--rw-rw-rw-   0        0        0     1108 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/frameobject.h
--rw-rw-rw-   0        0        0     4424 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/funcobject.h
--rw-rw-rw-   0        0        0     3279 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/genobject.h
--rw-rw-rw-   0        0        0     1526 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/import.h
--rw-rw-rw-   0        0        0     7817 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/initconfig.h
--rw-rw-rw-   0        0        0     1769 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/listobject.h
--rw-rw-rw-   0        0        0     3817 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/longintrepr.h
--rw-rw-rw-   0        0        0     4532 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/longobject.h
--rw-rw-rw-   0        0        0     2556 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/methodobject.h
--rw-rw-rw-   0        0        0     4234 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/modsupport.h
--rw-rw-rw-   0        0        0    18305 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/object.h
--rw-rw-rw-   0        0        0     2998 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     3505 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h
--rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1073 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pydebug.h
--rw-rw-rw-   0        0        0     4522 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyfpe.h
--rw-rw-rw-   0        0        0      582 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyframe.h
--rw-rw-rw-   0        0        0     2099 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pymem.h
--rw-rw-rw-   0        0        0    14351 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     1426 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pythread.h
--rw-rw-rw-   0        0        0    12158 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pytime.h
--rw-rw-rw-   0        0        0     1997 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/setobject.h
--rw-rw-rw-   0        0        0      489 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      444 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/traceback.h
--rw-rw-rw-   0        0        0     1513 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    41910 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0      560 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/warnings.h
--rw-rw-rw-   0        0        0     2103 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/weakrefobject.h
--rw-rw-rw-   0        0        0     9635 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/datetime.h
--rw-rw-rw-   0        0        0     1256 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/descrobject.h
--rw-rw-rw-   0        0        0     3852 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/errcode.h
--rw-rw-rw-   0        0        0     1098 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/exports.h
--rw-rw-rw-   0        0        0     1570 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/fileobject.h
--rw-rw-rw-   0        0        0      507 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/fileutils.h
--rw-rw-rw-   0        0        0     1530 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/floatobject.h
--rw-rw-rw-   0        0        0      336 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/frameobject.h
--rw-rw-rw-   0        0        0      334 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/genericaliasobject.h
--rw-rw-rw-   0        0        0     3025 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/import.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.605982 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/
--rw-rw-rw-   0        0        0      611 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     3031 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    29315 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6535 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16981 2023-05-29 09:11:37.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     6062 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     1424 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
--rw-rw-rw-   0        0        0     3475 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_call.h
--rw-rw-rw-   0        0        0     4409 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0    15930 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1045 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2839 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0     1239 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_context.h
--rw-rw-rw-   0        0        0     5684 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_dict.h
--rw-rw-rw-   0        0        0      704 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0      562 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
--rw-rw-rw-   0        0        0      842 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h
--rw-rw-rw-   0        0        0     7313 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     1307 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h
--rw-rw-rw-   0        0        0      480 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_format.h
--rw-rw-rw-   0        0        0     7567 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_frame.h
--rw-rw-rw-   0        0        0      413 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_function.h
--rw-rw-rw-   0        0        0     6895 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_gc.h
--rw-rw-rw-   0        0        0     1164 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_genobject.h
--rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     1436 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h
--rw-rw-rw-   0        0        0    12980 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h
--rw-rw-rw-   0        0        0     3696 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      743 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5800 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     6671 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      562 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
--rw-rw-rw-   0        0        0     1352 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_list.h
--rw-rw-rw-   0        0        0     3516 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1040 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0      392 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_namespace.h
--rw-rw-rw-   0        0        0    10037 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_object.h
--rw-rw-rw-   0        0        0    18986 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_opcode.h
--rw-rw-rw-   0        0        0      626 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_parser.h
--rw-rw-rw-   0        0        0      606 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2733 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2494 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3507 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     9435 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pymath.h
--rw-rw-rw-   0        0        0     3708 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     4107 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     5988 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0    49092 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
--rw-rw-rw-   0        0        0      937 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_signal.h
--rw-rw-rw-   0        0        0      336 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
--rw-rw-rw-   0        0        0      937 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_strhex.h
--rw-rw-rw-   0        0        0      580 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5638 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      605 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3501 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0     2089 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0     1158 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h
--rw-rw-rw-   0        0        0      898 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0     1716 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
--rw-rw-rw-   0        0        0      678 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      740 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      772 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/intrcheck.h
--rw-rw-rw-   0        0        0      593 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/iterobject.h
--rw-rw-rw-   0        0        0     1780 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/listobject.h
--rw-rw-rw-   0        0        0     3272 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/longobject.h
--rw-rw-rw-   0        0        0      827 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/marshal.h
--rw-rw-rw-   0        0        0     2810 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/memoryobject.h
--rw-rw-rw-   0        0        0     5072 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/methodobject.h
--rw-rw-rw-   0        0        0     6448 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/modsupport.h
--rw-rw-rw-   0        0        0     2374 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/moduleobject.h
--rw-rw-rw-   0        0        0    29800 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/object.h
--rw-rw-rw-   0        0        0     8428 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/objimpl.h
--rw-rw-rw-   0        0        0    11187 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/opcode.h
--rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/osmodule.h
--rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/patchlevel.h
--rw-rw-rw-   0        0        0     2471 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/py_curses.h
--rw-rw-rw-   0        0        0     5115 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pybuffer.h
--rw-rw-rw-   0        0        0     1725 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pycapsule.h
--rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pydtrace.h
--rw-rw-rw-   0        0        0    12782 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyexpat.h
--rw-rw-rw-   0        0        0      551 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyframe.h
--rw-rw-rw-   0        0        0     4154 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyhash.h
--rw-rw-rw-   0        0        0     2249 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymacconfig.h
--rw-rw-rw-   0        0        0     6064 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymacro.h
--rw-rw-rw-   0        0        0     1979 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymath.h
--rw-rw-rw-   0        0        0     3890 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymem.h
--rw-rw-rw-   0        0        0    24532 2023-05-29 09:11:37.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyport.h
--rw-rw-rw-   0        0        0     4635 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pystate.h
--rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pystrcmp.h
--rw-rw-rw-   0        0        0     1557 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pystrtod.h
--rw-rw-rw-   0        0        0     1189 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pythonrun.h
--rw-rw-rw-   0        0        0     4833 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pythread.h
--rw-rw-rw-   0        0        0      851 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/pytypedefs.h
--rw-rw-rw-   0        0        0      628 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/rangeobject.h
--rw-rw-rw-   0        0        0     1543 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-05-29 09:08:27.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/sliceobject.h
--rw-rw-rw-   0        0        0     2040 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/structmember.h
--rw-rw-rw-   0        0        0     1388 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/structseq.h
--rw-rw-rw-   0        0        0     1381 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-05-29 09:11:30.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/token.h
--rw-rw-rw-   0        0        0      583 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/tracemalloc.h
--rw-rw-rw-   0        0        0     1613 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/tupleobject.h
--rw-rw-rw-   0        0        0     2342 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/typeslots.h
--rw-rw-rw-   0        0        0    36032 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/unicodeobject.h
--rw-rw-rw-   0        0        0     1129 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/warnings.h
--rw-rw-rw-   0        0        0     1226 2023-05-29 09:11:34.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp311/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.766980 wasmpy-build-0.3.1/wasmpy_build/include/cp38/
--rw-rw-rw-   0        0        0    13937 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/LICENSE
--rw-rw-rw-   0        0        0    26491 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/Python-ast.h
--rw-rw-rw-   0        0        0     3617 2023-05-29 09:11:43.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/Python.h
--rw-rw-rw-   0        0        0    30286 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/abstract.h
--rw-rw-rw-   0        0        0     1229 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/asdl.h
--rw-rw-rw-   0        0        0      948 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/ast.h
--rw-rw-rw-   0        0        0      468 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/bitset.h
--rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/bltinmodule.h
--rw-rw-rw-   0        0        0      886 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/boolobject.h
--rw-rw-rw-   0        0        0     2114 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/bytearrayobject.h
--rw-rw-rw-   0        0        0     3301 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/bytes_methods.h
--rw-rw-rw-   0        0        0     8493 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/bytesobject.h
--rw-rw-rw-   0        0        0      713 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cellobject.h
--rw-rw-rw-   0        0        0     8366 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/ceval.h
--rw-rw-rw-   0        0        0     1710 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/classobject.h
--rw-rw-rw-   0        0        0     7178 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/code.h
--rw-rw-rw-   0        0        0     6793 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/codecs.h
--rw-rw-rw-   0        0        0     3582 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/compile.h
--rw-rw-rw-   0        0        0     1807 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/complexobject.h
--rw-rw-rw-   0        0        0     2014 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/context.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.783998 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/
--rw-rw-rw-   0        0        0    12294 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/abstract.h
--rw-rw-rw-   0        0        0     3845 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/fileobject.h
--rw-rw-rw-   0        0        0    16028 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0    15691 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/object.h
--rw-rw-rw-   0        0        0     3600 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/objimpl.h
--rw-rw-rw-   0        0        0     4717 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2263 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pymem.h
--rw-rw-rw-   0        0        0     9810 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pystate.h
--rw-rw-rw-   0        0        0      547 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46308 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9260 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/datetime.h
--rw-rw-rw-   0        0        0     3019 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/descrobject.h
--rw-rw-rw-   0        0        0     3716 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/dictobject.h
--rw-rw-rw-   0        0        0      458 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/dtoa.h
--rw-rw-rw-   0        0        0    22469 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/enumobject.h
--rw-rw-rw-   0        0        0     1695 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/errcode.h
--rw-rw-rw-   0        0        0     1209 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/eval.h
--rw-rw-rw-   0        0        0     1571 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/fileobject.h
--rw-rw-rw-   0        0        0     4352 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/fileutils.h
--rw-rw-rw-   0        0        0     4794 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/floatobject.h
--rw-rw-rw-   0        0        0     3317 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/frameobject.h
--rw-rw-rw-   0        0        0     4200 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/funcobject.h
--rw-rw-rw-   0        0        0     3720 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/grammar.h
--rw-rw-rw-   0        0        0     4926 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/import.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.809913 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/
--rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16946 2023-05-29 09:11:43.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0      966 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      542 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      779 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_context.h
--rw-rw-rw-   0        0        0     1254 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1520 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3698 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     5218 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     1548 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_long.h
--rw-rw-rw-   0        0        0     2896 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_object.h
--rw-rw-rw-   0        0        0     2037 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     1329 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3815 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     8217 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     9588 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     3076 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      418 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      591 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/interpreteridobject.h
--rw-rw-rw-   0        0        0      861 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/intrcheck.h
--rw-rw-rw-   0        0        0      567 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/iterobject.h
--rw-rw-rw-   0        0        0     2927 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/longintrepr.h
--rw-rw-rw-   0        0        0     9520 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/longobject.h
--rw-rw-rw-   0        0        0      803 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/marshal.h
--rw-rw-rw-   0        0        0     2765 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/memoryobject.h
--rw-rw-rw-   0        0        0     4406 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/methodobject.h
--rw-rw-rw-   0        0        0     9591 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/modsupport.h
--rw-rw-rw-   0        0        0     2362 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/namespaceobject.h
--rw-rw-rw-   0        0        0     1328 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/node.h
--rw-rw-rw-   0        0        0    29599 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/object.h
--rw-rw-rw-   0        0        0    10537 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/objimpl.h
--rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/odictobject.h
--rw-rw-rw-   0        0        0     5164 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/opcode.h
--rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/osmodule.h
--rw-rw-rw-   0        0        0     2958 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/parsetok.h
--rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/patchlevel.h
--rw-rw-rw-   0        0        0      847 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/picklebufobject.h
--rw-rw-rw-   0        0        0     2477 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/py_curses.h
--rw-rw-rw-   0        0        0     2744 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyarena.h
--rw-rw-rw-   0        0        0     1726 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pycapsule.h
--rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyctype.h
--rw-rw-rw-   0        0        0     1214 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pydebug.h
--rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pydtrace.h
--rw-rw-rw-   0        0        0    12786 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyexpat.h
--rw-rw-rw-   0        0        0      341 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyfpe.h
--rw-rw-rw-   0        0        0     4140 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyhash.h
--rw-rw-rw-   0        0        0     2081 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymacconfig.h
--rw-rw-rw-   0        0        0     3778 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymacro.h
--rw-rw-rw-   0        0        0     8314 2023-05-29 09:11:43.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymath.h
--rw-rw-rw-   0        0        0     5406 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymem.h
--rw-rw-rw-   0        0        0    30225 2023-05-29 09:11:43.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyport.h
--rw-rw-rw-   0        0        0     4686 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystate.h
--rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystrtod.h
--rw-rw-rw-   0        0        0     7645 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pythonrun.h
--rw-rw-rw-   0        0        0     5660 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pythread.h
--rw-rw-rw-   0        0        0     8928 2023-05-29 09:11:43.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/pytime.h
--rw-rw-rw-   0        0        0      629 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/rangeobject.h
--rw-rw-rw-   0        0        0     3362 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/setobject.h
--rw-rw-rw-   0        0        0     2517 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/sliceobject.h
--rw-rw-rw-   0        0        0     2030 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/structmember.h
--rw-rw-rw-   0        0        0     1377 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/structseq.h
--rw-rw-rw-   0        0        0     5308 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/symtable.h
--rw-rw-rw-   0        0        0     1242 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/sysmodule.h
--rw-rw-rw-   0        0        0     2429 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/token.h
--rw-rw-rw-   0        0        0      601 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/tracemalloc.h
--rw-rw-rw-   0        0        0     1661 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/tupleobject.h
--rw-rw-rw-   0        0        0     2253 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/ucnhash.h
--rw-rw-rw-   0        0        0    35732 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/warnings.h
--rw-rw-rw-   0        0        0     2866 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp38/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.931206 wasmpy-build-0.3.1/wasmpy_build/include/cp39/
--rw-rw-rw-   0        0        0    13937 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/LICENSE
--rw-rw-rw-   0        0        0    26193 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/Python-ast.h
--rw-rw-rw-   0        0        0     3534 2023-05-29 09:11:47.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/Python.h
--rw-rw-rw-   0        0        0    30476 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/abstract.h
--rw-rw-rw-   0        0        0     1224 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/asdl.h
--rw-rw-rw-   0        0        0      947 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/ast.h
--rw-rw-rw-   0        0        0      468 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/bitset.h
--rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/bltinmodule.h
--rw-rw-rw-   0        0        0      885 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/boolobject.h
--rw-rw-rw-   0        0        0     1484 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/bytearrayobject.h
--rw-rw-rw-   0        0        0     3048 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/bytesobject.h
--rw-rw-rw-   0        0        0      712 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cellobject.h
--rw-rw-rw-   0        0        0     5954 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/ceval.h
--rw-rw-rw-   0        0        0     1657 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/classobject.h
--rw-rw-rw-   0        0        0      318 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/code.h
--rw-rw-rw-   0        0        0     6793 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/codecs.h
--rw-rw-rw-   0        0        0     3778 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/compile.h
--rw-rw-rw-   0        0        0     1806 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/complexobject.h
--rw-rw-rw-   0        0        0     1962 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/context.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.979219 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/
--rw-rw-rw-   0        0        0    14200 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4114 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1537 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/ceval.h
--rw-rw-rw-   0        0        0     6989 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/code.h
--rw-rw-rw-   0        0        0     3797 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4004 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3059 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1473 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/import.h
--rw-rw-rw-   0        0        0    16979 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1364 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19358 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/object.h
--rw-rw-rw-   0        0        0     4456 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/objimpl.h
--rw-rw-rw-   0        0        0     5101 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2096 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pymem.h
--rw-rw-rw-   0        0        0    10134 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pystate.h
--rw-rw-rw-   0        0        0      575 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46154 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9255 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/datetime.h
--rw-rw-rw-   0        0        0     3019 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/descrobject.h
--rw-rw-rw-   0        0        0     3715 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/dictobject.h
--rw-rw-rw-   0        0        0    22469 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/enumobject.h
--rw-rw-rw-   0        0        0     1624 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/errcode.h
--rw-rw-rw-   0        0        0     1209 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/eval.h
--rw-rw-rw-   0        0        0     1098 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/exports.h
--rw-rw-rw-   0        0        0     1571 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/fileobject.h
--rw-rw-rw-   0        0        0      597 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/fileutils.h
--rw-rw-rw-   0        0        0     4360 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/frameobject.h
--rw-rw-rw-   0        0        0     4057 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/funcobject.h
--rw-rw-rw-   0        0        0      334 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/genericaliasobject.h
--rw-rw-rw-   0        0        0     3525 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/grammar.h
--rw-rw-rw-   0        0        0     3026 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/import.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:44.052122 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/
--rw-rw-rw-   0        0        0      953 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pegen_interface.h
--rw-rw-rw-   0        0        0      479 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16979 2023-05-29 09:11:47.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     3384 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     2620 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h
--rw-rw-rw-   0        0        0      870 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3403 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      541 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      800 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_context.h
--rw-rw-rw-   0        0        0      646 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1541 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     6647 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      473 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5233 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     5299 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_interp.h
--rw-rw-rw-   0        0        0     1548 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_long.h
--rw-rw-rw-   0        0        0     4157 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_object.h
--rw-rw-rw-   0        0        0     1936 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2032 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3741 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3363 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3583 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4452 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      548 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3056 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      442 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      633 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/interpreteridobject.h
--rw-rw-rw-   0        0        0      861 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/intrcheck.h
--rw-rw-rw-   0        0        0      521 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/iterobject.h
--rw-rw-rw-   0        0        0     1781 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/longintrepr.h
--rw-rw-rw-   0        0        0     9513 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/longobject.h
--rw-rw-rw-   0        0        0      803 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/marshal.h
--rw-rw-rw-   0        0        0     2764 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/memoryobject.h
--rw-rw-rw-   0        0        0     3775 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/methodobject.h
--rw-rw-rw-   0        0        0     9959 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/modsupport.h
--rw-rw-rw-   0        0        0     2361 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/namespaceobject.h
--rw-rw-rw-   0        0        0     1281 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/node.h
--rw-rw-rw-   0        0        0    24628 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/object.h
--rw-rw-rw-   0        0        0     8423 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/odictobject.h
--rw-rw-rw-   0        0        0     4900 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/opcode.h
--rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/osdefs.h
--rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/osmodule.h
--rw-rw-rw-   0        0        0     2958 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/parsetok.h
--rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/patchlevel.h
--rw-rw-rw-   0        0        0      846 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/picklebufobject.h
--rw-rw-rw-   0        0        0     2474 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/py_curses.h
--rw-rw-rw-   0        0        0     2744 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyarena.h
--rw-rw-rw-   0        0        0     1725 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pycapsule.h
--rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pydebug.h
--rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pydtrace.h
--rw-rw-rw-   0        0        0    12427 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyexpat.h
--rw-rw-rw-   0        0        0      444 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyfpe.h
--rw-rw-rw-   0        0        0      466 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyframe.h
--rw-rw-rw-   0        0        0     4263 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyhash.h
--rw-rw-rw-   0        0        0     2136 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymacro.h
--rw-rw-rw-   0        0        0     8582 2023-05-29 09:11:47.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymath.h
--rw-rw-rw-   0        0        0     4406 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymem.h
--rw-rw-rw-   0        0        0    31277 2023-05-29 09:11:47.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyport.h
--rw-rw-rw-   0        0        0     5250 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystate.h
--rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystrtod.h
--rw-rw-rw-   0        0        0     7673 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pythonrun.h
--rw-rw-rw-   0        0        0     5938 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pythread.h
--rw-rw-rw-   0        0        0     8930 2023-05-29 09:11:47.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/pytime.h
--rw-rw-rw-   0        0        0      628 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/rangeobject.h
--rw-rw-rw-   0        0        0     3324 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/sliceobject.h
--rw-rw-rw-   0        0        0     2030 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/structmember.h
--rw-rw-rw-   0        0        0     1390 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/structseq.h
--rw-rw-rw-   0        0        0     5307 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/symtable.h
--rw-rw-rw-   0        0        0     1242 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/sysmodule.h
--rw-rw-rw-   0        0        0     2642 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/token.h
--rw-rw-rw-   0        0        0      584 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/traceback.h
--rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/tracemalloc.h
--rw-rw-rw-   0        0        0     1614 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/tupleobject.h
--rw-rw-rw-   0        0        0     2350 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/ucnhash.h
--rw-rw-rw-   0        0        0    35426 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-05-29 09:11:38.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/warnings.h
--rw-rw-rw-   0        0        0     2863 2023-05-29 09:11:44.000000 wasmpy-build-0.3.1/wasmpy_build/include/cp39/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-07-13 01:50:43.181806 wasmpy-build-0.3.1/wasmpy_build.egg-info/
--rw-rw-rw-   0        0        0     1560 2023-07-13 01:50:43.000000 wasmpy-build-0.3.1/wasmpy_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    28773 2023-07-13 01:50:43.000000 wasmpy-build-0.3.1/wasmpy_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 01:50:43.000000 wasmpy-build-0.3.1/wasmpy_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-13 01:50:43.000000 wasmpy-build-0.3.1/wasmpy_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-07-13 01:50:43.000000 wasmpy-build-0.3.1/wasmpy_build.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 01:50:43.000000 wasmpy-build-0.3.1/wasmpy_build.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.904367 wasmpy-build-0.3.2/
+-rw-rw-rw-   0        0        0     1068 2023-07-13 12:38:30.000000 wasmpy-build-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1686 2023-07-14 11:04:08.903367 wasmpy-build-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2023-07-14 10:51:14.000000 wasmpy-build-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-14 11:04:08.904367 wasmpy-build-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-07-14 10:55:36.000000 wasmpy-build-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.626880 wasmpy-build-0.3.2/wasmpy_build/
+-rw-rw-rw-   0        0        0     2221 2023-07-14 10:38:29.000000 wasmpy-build-0.3.2/wasmpy_build/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-07-13 12:38:42.000000 wasmpy-build-0.3.2/wasmpy_build/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.618784 wasmpy-build-0.3.2/wasmpy_build/include/
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.792421 wasmpy-build-0.3.2/wasmpy_build/include/cp310/
+-rw-rw-rw-   0        0        0    13936 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/LICENSE
+-rw-rw-rw-   0        0        0     3224 2023-07-13 11:07:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/Python.h
+-rw-rw-rw-   0        0        0      344 2023-07-13 11:07:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/README.rst
+-rw-rw-rw-   0        0        0    31405 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/bltinmodule.h
+-rw-rw-rw-   0        0        0     1224 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/boolobject.h
+-rw-rw-rw-   0        0        0     1484 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2593 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytesobject.h
+-rw-rw-rw-   0        0        0      720 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cellobject.h
+-rw-rw-rw-   0        0        0     5703 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/ceval.h
+-rw-rw-rw-   0        0        0     1657 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/code.h
+-rw-rw-rw-   0        0        0     7071 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/compile.h
+-rw-rw-rw-   0        0        0     1806 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/complexobject.h
+-rw-rw-rw-   0        0        0     1962 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/context.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.843496 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/
+-rw-rw-rw-   0        0        0    14054 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4119 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1468 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/ceval.h
+-rw-rw-rw-   0        0        0     7570 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/compile.h
+-rw-rw-rw-   0        0        0     3734 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      723 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4267 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3152 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1630 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/import.h
+-rw-rw-rw-   0        0        0     7597 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      387 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1243 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-07-13 10:41:46.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19613 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/object.h
+-rw-rw-rw-   0        0        0     3356 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     1387 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     5476 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0     2095 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pymem.h
+-rw-rw-rw-   0        0        0    11914 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     9196 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pytime.h
+-rw-rw-rw-   0        0        0      506 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      404 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/traceback.h
+-rw-rw-rw-   0        0        0      975 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    44284 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9635 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/datetime.h
+-rw-rw-rw-   0        0        0     3002 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/descrobject.h
+-rw-rw-rw-   0        0        0     3853 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/errcode.h
+-rw-rw-rw-   0        0        0      831 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/exports.h
+-rw-rw-rw-   0        0        0     1571 2023-07-13 10:35:26.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/fileobject.h
+-rw-rw-rw-   0        0        0      508 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/fileutils.h
+-rw-rw-rw-   0        0        0     4360 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/frameobject.h
+-rw-rw-rw-   0        0        0     4257 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/funcobject.h
+-rw-rw-rw-   0        0        0      334 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3347 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/genobject.h
+-rw-rw-rw-   0        0        0     3026 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.917967 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/
+-rw-rw-rw-   0        0        0      479 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     2971 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    28828 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6457 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16979 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     5271 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0      870 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3484 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      696 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1045 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2809 2023-07-13 10:35:26.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      822 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      646 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1704 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      480 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     6859 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      346 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5625 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     9289 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      350 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     2589 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1047 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0     5989 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_object.h
+-rw-rw-rw-   0        0        0      626 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0     1981 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2733 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2314 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     4940 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3211 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3938 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4902 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      386 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5578 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      548 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     2970 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      425 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0      898 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0      629 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      633 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/interpreteridobject.h
+-rw-rw-rw-   0        0        0      772 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/intrcheck.h
+-rw-rw-rw-   0        0        0      593 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/iterobject.h
+-rw-rw-rw-   0        0        0     1781 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/longintrepr.h
+-rw-rw-rw-   0        0        0     8606 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/marshal.h
+-rw-rw-rw-   0        0        0     2764 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/memoryobject.h
+-rw-rw-rw-   0        0        0     4147 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/methodobject.h
+-rw-rw-rw-   0        0        0    10333 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/modsupport.h
+-rw-rw-rw-   0        0        0     2458 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/namespaceobject.h
+-rw-rw-rw-   0        0        0    28344 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/object.h
+-rw-rw-rw-   0        0        0     8445 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/objimpl.h
+-rw-rw-rw-   0        0        0     5509 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/osmodule.h
+-rw-rw-rw-   0        0        0     1302 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/patchlevel.h
+-rw-rw-rw-   0        0        0     2474 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/py_curses.h
+-rw-rw-rw-   0        0        0     1725 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pycapsule.h
+-rw-rw-rw-   0        0        0    48758 2023-07-13 12:23:44.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyconfig.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.h
+-rw-rw-rw-   0        0        0    12426 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyexpat.h
+-rw-rw-rw-   0        0        0      466 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyframe.h
+-rw-rw-rw-   0        0        0     4223 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyhash.h
+-rw-rw-rw-   0        0        0     2080 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacro.h
+-rw-rw-rw-   0        0        0     8313 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymath.h
+-rw-rw-rw-   0        0        0     3891 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymem.h
+-rw-rw-rw-   0        0        0    31684 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyport.h
+-rw-rw-rw-   0        0        0     5250 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-13 10:35:27.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrtod.h
+-rw-rw-rw-   0        0        0     1110 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythonrun.h
+-rw-rw-rw-   0        0        0     5938 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythread.h
+-rw-rw-rw-   0        0        0      628 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/rangeobject.h
+-rw-rw-rw-   0        0        0     3381 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/sliceobject.h
+-rw-rw-rw-   0        0        0     2074 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/structmember.h
+-rw-rw-rw-   0        0        0     1390 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/structseq.h
+-rw-rw-rw-   0        0        0     1242 2023-07-13 10:35:28.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/token.h
+-rw-rw-rw-   0        0        0      584 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/tracemalloc.h
+-rw-rw-rw-   0        0        0     1614 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/tupleobject.h
+-rw-rw-rw-   0        0        0     2460 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/typeslots.h
+-rw-rw-rw-   0        0        0    36148 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-07-13 10:35:28.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/warnings.h
+-rw-rw-rw-   0        0        0     2863 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp310/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.023154 wasmpy-build-0.3.2/wasmpy_build/include/cp311/
+-rw-rw-rw-   0        0        0    13936 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/LICENSE
+-rw-rw-rw-   0        0        0     2854 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/Python.h
+-rw-rw-rw-   0        0        0      344 2023-07-13 11:07:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/README.rst
+-rw-rw-rw-   0        0        0    31404 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/bltinmodule.h
+-rw-rw-rw-   0        0        0     1212 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/boolobject.h
+-rw-rw-rw-   0        0        0     1462 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2617 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytesobject.h
+-rw-rw-rw-   0        0        0     6255 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/ceval.h
+-rw-rw-rw-   0        0        0     7071 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/compile.h
+-rw-rw-rw-   0        0        0      724 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/complexobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.098708 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/
+-rw-rw-rw-   0        0        0     8229 2023-07-13 11:14:33.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/abstract.h
+-rw-rw-rw-   0        0        0     1305 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4568 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0      723 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/cellobject.h
+-rw-rw-rw-   0        0        0     1239 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/ceval.h
+-rw-rw-rw-   0        0        0     1656 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/classobject.h
+-rw-rw-rw-   0        0        0    11484 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/compile.h
+-rw-rw-rw-   0        0        0     1248 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/complexobject.h
+-rw-rw-rw-   0        0        0     1959 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/context.h
+-rw-rw-rw-   0        0        0     1642 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/descrobject.h
+-rw-rw-rw-   0        0        0     3324 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      818 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/fileobject.h
+-rw-rw-rw-   0        0        0      232 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/fileutils.h
+-rw-rw-rw-   0        0        0      702 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/floatobject.h
+-rw-rw-rw-   0        0        0     1108 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     4424 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/funcobject.h
+-rw-rw-rw-   0        0        0     3279 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/genobject.h
+-rw-rw-rw-   0        0        0     1526 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/import.h
+-rw-rw-rw-   0        0        0     7817 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/initconfig.h
+-rw-rw-rw-   0        0        0     1769 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/listobject.h
+-rw-rw-rw-   0        0        0     3817 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longintrepr.h
+-rw-rw-rw-   0        0        0     4532 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longobject.h
+-rw-rw-rw-   0        0        0     2556 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/methodobject.h
+-rw-rw-rw-   0        0        0     4234 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/modsupport.h
+-rw-rw-rw-   0        0        0    18305 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/object.h
+-rw-rw-rw-   0        0        0     2998 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     3505 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pthread_stubs.h
+-rw-rw-rw-   0        0        0     1387 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1073 2023-07-13 11:14:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     4522 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-07-13 11:07:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0      582 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyframe.h
+-rw-rw-rw-   0        0        0     2099 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pymem.h
+-rw-rw-rw-   0        0        0    14351 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     1426 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythread.h
+-rw-rw-rw-   0        0        0    12158 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pytime.h
+-rw-rw-rw-   0        0        0     1997 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/setobject.h
+-rw-rw-rw-   0        0        0      489 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      444 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1513 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    41910 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0      560 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/warnings.h
+-rw-rw-rw-   0        0        0     2103 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/weakrefobject.h
+-rw-rw-rw-   0        0        0     9635 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/datetime.h
+-rw-rw-rw-   0        0        0     1256 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/descrobject.h
+-rw-rw-rw-   0        0        0     3852 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/errcode.h
+-rw-rw-rw-   0        0        0     1098 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/exports.h
+-rw-rw-rw-   0        0        0     1570 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/fileobject.h
+-rw-rw-rw-   0        0        0      507 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/fileutils.h
+-rw-rw-rw-   0        0        0     1530 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/floatobject.h
+-rw-rw-rw-   0        0        0      336 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/frameobject.h
+-rw-rw-rw-   0        0        0      334 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3025 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.286358 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/
+-rw-rw-rw-   0        0        0      611 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     3031 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    29315 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6535 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16979 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     6062 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     1424 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
+-rw-rw-rw-   0        0        0     3475 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     4409 2023-07-13 11:14:35.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0    15930 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1045 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2839 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0     1239 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     5684 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dict.h
+-rw-rw-rw-   0        0        0      704 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0      562 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
+-rw-rw-rw-   0        0        0      842 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_exceptions.h
+-rw-rw-rw-   0        0        0     7313 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     1307 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_floatobject.h
+-rw-rw-rw-   0        0        0      480 2023-07-13 11:07:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     7567 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_frame.h
+-rw-rw-rw-   0        0        0      413 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_function.h
+-rw-rw-rw-   0        0        0     6895 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0     1164 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_genobject.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     1436 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_objects.h
+-rw-rw-rw-   0        0        0    12980 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_strings.h
+-rw-rw-rw-   0        0        0     3696 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-07-13 10:41:47.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      743 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5800 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     6671 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      562 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
+-rw-rw-rw-   0        0        0     1352 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     3516 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1040 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0      392 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_namespace.h
+-rw-rw-rw-   0        0        0    10037 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_object.h
+-rw-rw-rw-   0        0        0    18986 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_opcode.h
+-rw-rw-rw-   0        0        0      626 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0      606 2023-07-13 11:14:36.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2733 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2494 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3507 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     9435 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymath.h
+-rw-rw-rw-   0        0        0     3708 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     4107 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     5988 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0    49092 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
+-rw-rw-rw-   0        0        0      937 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_signal.h
+-rw-rw-rw-   0        0        0      336 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
+-rw-rw-rw-   0        0        0      937 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_strhex.h
+-rw-rw-rw-   0        0        0      580 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5638 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      605 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3501 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0     2089 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0     1158 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_typeobject.h
+-rw-rw-rw-   0        0        0      898 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0     1716 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
+-rw-rw-rw-   0        0        0      678 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      740 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      772 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/intrcheck.h
+-rw-rw-rw-   0        0        0      593 2023-07-13 11:07:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/iterobject.h
+-rw-rw-rw-   0        0        0     1780 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/listobject.h
+-rw-rw-rw-   0        0        0     3272 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/longobject.h
+-rw-rw-rw-   0        0        0      827 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/marshal.h
+-rw-rw-rw-   0        0        0     2810 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/memoryobject.h
+-rw-rw-rw-   0        0        0     5072 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/methodobject.h
+-rw-rw-rw-   0        0        0     6448 2023-07-13 11:14:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/modsupport.h
+-rw-rw-rw-   0        0        0     2374 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/moduleobject.h
+-rw-rw-rw-   0        0        0    29800 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/object.h
+-rw-rw-rw-   0        0        0     8428 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/objimpl.h
+-rw-rw-rw-   0        0        0    11187 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/osmodule.h
+-rw-rw-rw-   0        0        0     1300 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/patchlevel.h
+-rw-rw-rw-   0        0        0     2471 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/py_curses.h
+-rw-rw-rw-   0        0        0     5115 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pybuffer.h
+-rw-rw-rw-   0        0        0     1725 2023-07-13 10:41:48.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pycapsule.h
+-rw-rw-rw-   0        0        0    53001 2023-07-13 12:29:25.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyconfig.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.h
+-rw-rw-rw-   0        0        0    12782 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyexpat.h
+-rw-rw-rw-   0        0        0      551 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyframe.h
+-rw-rw-rw-   0        0        0     4154 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyhash.h
+-rw-rw-rw-   0        0        0     2249 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacconfig.h
+-rw-rw-rw-   0        0        0     6064 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacro.h
+-rw-rw-rw-   0        0        0     1979 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymath.h
+-rw-rw-rw-   0        0        0     3890 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymem.h
+-rw-rw-rw-   0        0        0    24528 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyport.h
+-rw-rw-rw-   0        0        0     4635 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystrcmp.h
+-rw-rw-rw-   0        0        0     1557 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystrtod.h
+-rw-rw-rw-   0        0        0     1189 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythonrun.h
+-rw-rw-rw-   0        0        0     4833 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythread.h
+-rw-rw-rw-   0        0        0      851 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/pytypedefs.h
+-rw-rw-rw-   0        0        0      628 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/rangeobject.h
+-rw-rw-rw-   0        0        0     1543 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-07-13 10:41:49.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/sliceobject.h
+-rw-rw-rw-   0        0        0     2040 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/structmember.h
+-rw-rw-rw-   0        0        0     1388 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/structseq.h
+-rw-rw-rw-   0        0        0     1381 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-07-13 11:07:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/token.h
+-rw-rw-rw-   0        0        0      583 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/tracemalloc.h
+-rw-rw-rw-   0        0        0     1613 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/tupleobject.h
+-rw-rw-rw-   0        0        0     2342 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/typeslots.h
+-rw-rw-rw-   0        0        0    36032 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/unicodeobject.h
+-rw-rw-rw-   0        0        0     1129 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/warnings.h
+-rw-rw-rw-   0        0        0     1226 2023-07-13 11:14:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp311/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.483929 wasmpy-build-0.3.2/wasmpy_build/include/cp38/
+-rw-rw-rw-   0        0        0    13937 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/LICENSE
+-rw-rw-rw-   0        0        0    26491 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python-ast.h
+-rw-rw-rw-   0        0        0     3615 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python.h
+-rw-rw-rw-   0        0        0    30286 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/abstract.h
+-rw-rw-rw-   0        0        0     1229 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/asdl.h
+-rw-rw-rw-   0        0        0      948 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/ast.h
+-rw-rw-rw-   0        0        0      468 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bltinmodule.h
+-rw-rw-rw-   0        0        0      886 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/boolobject.h
+-rw-rw-rw-   0        0        0     2114 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3301 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytes_methods.h
+-rw-rw-rw-   0        0        0     8493 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytesobject.h
+-rw-rw-rw-   0        0        0      713 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cellobject.h
+-rw-rw-rw-   0        0        0     8366 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/ceval.h
+-rw-rw-rw-   0        0        0     1710 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/classobject.h
+-rw-rw-rw-   0        0        0     7178 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/code.h
+-rw-rw-rw-   0        0        0     6793 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/codecs.h
+-rw-rw-rw-   0        0        0     3582 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/compile.h
+-rw-rw-rw-   0        0        0     1807 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/complexobject.h
+-rw-rw-rw-   0        0        0     2014 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/context.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.522810 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/
+-rw-rw-rw-   0        0        0    12294 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/abstract.h
+-rw-rw-rw-   0        0        0     3845 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/fileobject.h
+-rw-rw-rw-   0        0        0    16028 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0    15691 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/object.h
+-rw-rw-rw-   0        0        0     3600 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     4717 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2263 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pymem.h
+-rw-rw-rw-   0        0        0     9810 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pystate.h
+-rw-rw-rw-   0        0        0      547 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46308 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9260 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/datetime.h
+-rw-rw-rw-   0        0        0     3019 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/descrobject.h
+-rw-rw-rw-   0        0        0     3716 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/dictobject.h
+-rw-rw-rw-   0        0        0      458 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/dtoa.h
+-rw-rw-rw-   0        0        0    22469 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/enumobject.h
+-rw-rw-rw-   0        0        0     1695 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/errcode.h
+-rw-rw-rw-   0        0        0     1209 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/eval.h
+-rw-rw-rw-   0        0        0     1571 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileobject.h
+-rw-rw-rw-   0        0        0     4352 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileutils.h
+-rw-rw-rw-   0        0        0     4794 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/floatobject.h
+-rw-rw-rw-   0        0        0     3317 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/frameobject.h
+-rw-rw-rw-   0        0        0     4200 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/funcobject.h
+-rw-rw-rw-   0        0        0     3720 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/grammar.h
+-rw-rw-rw-   0        0        0     4926 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.576544 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16944 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0      966 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      542 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      779 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     1254 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1520 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3698 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     5218 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     1548 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     2896 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     2037 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     1329 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3815 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     8217 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     9588 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     3076 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      418 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      591 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/interpreteridobject.h
+-rw-rw-rw-   0        0        0      861 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/intrcheck.h
+-rw-rw-rw-   0        0        0      567 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/iterobject.h
+-rw-rw-rw-   0        0        0     2927 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/longintrepr.h
+-rw-rw-rw-   0        0        0     9520 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/marshal.h
+-rw-rw-rw-   0        0        0     2765 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/memoryobject.h
+-rw-rw-rw-   0        0        0     4406 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/methodobject.h
+-rw-rw-rw-   0        0        0     9591 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/modsupport.h
+-rw-rw-rw-   0        0        0     2362 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/namespaceobject.h
+-rw-rw-rw-   0        0        0     1328 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/node.h
+-rw-rw-rw-   0        0        0    29599 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/object.h
+-rw-rw-rw-   0        0        0    10537 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/objimpl.h
+-rw-rw-rw-   0        0        0     1300 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/odictobject.h
+-rw-rw-rw-   0        0        0     5164 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/osmodule.h
+-rw-rw-rw-   0        0        0     2958 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/parsetok.h
+-rw-rw-rw-   0        0        0     1300 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/patchlevel.h
+-rw-rw-rw-   0        0        0      847 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/picklebufobject.h
+-rw-rw-rw-   0        0        0     2477 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/py_curses.h
+-rw-rw-rw-   0        0        0     2744 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyarena.h
+-rw-rw-rw-   0        0        0     1726 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pycapsule.h
+-rw-rw-rw-   0        0        0    47623 2023-07-13 11:28:34.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyconfig.h
+-rw-rw-rw-   0        0        0     1387 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyctype.h
+-rw-rw-rw-   0        0        0     1214 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.h
+-rw-rw-rw-   0        0        0    12786 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyexpat.h
+-rw-rw-rw-   0        0        0      341 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyfpe.h
+-rw-rw-rw-   0        0        0     4140 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyhash.h
+-rw-rw-rw-   0        0        0     2081 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacconfig.h
+-rw-rw-rw-   0        0        0     3778 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacro.h
+-rw-rw-rw-   0        0        0     8312 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymath.h
+-rw-rw-rw-   0        0        0     5406 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymem.h
+-rw-rw-rw-   0        0        0    30221 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyport.h
+-rw-rw-rw-   0        0        0     4686 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrtod.h
+-rw-rw-rw-   0        0        0     7645 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythonrun.h
+-rw-rw-rw-   0        0        0     5660 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythread.h
+-rw-rw-rw-   0        0        0     8926 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/pytime.h
+-rw-rw-rw-   0        0        0      629 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/rangeobject.h
+-rw-rw-rw-   0        0        0     3362 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/setobject.h
+-rw-rw-rw-   0        0        0     2517 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/sliceobject.h
+-rw-rw-rw-   0        0        0     2030 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/structmember.h
+-rw-rw-rw-   0        0        0     1377 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/structseq.h
+-rw-rw-rw-   0        0        0     5308 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/symtable.h
+-rw-rw-rw-   0        0        0     1242 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/sysmodule.h
+-rw-rw-rw-   0        0        0     2429 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/token.h
+-rw-rw-rw-   0        0        0      601 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/tracemalloc.h
+-rw-rw-rw-   0        0        0     1661 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/tupleobject.h
+-rw-rw-rw-   0        0        0     2253 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/ucnhash.h
+-rw-rw-rw-   0        0        0    35732 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/warnings.h
+-rw-rw-rw-   0        0        0     2866 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp38/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.785138 wasmpy-build-0.3.2/wasmpy_build/include/cp39/
+-rw-rw-rw-   0        0        0    13937 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/LICENSE
+-rw-rw-rw-   0        0        0    26193 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python-ast.h
+-rw-rw-rw-   0        0        0     3532 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python.h
+-rw-rw-rw-   0        0        0    30476 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/abstract.h
+-rw-rw-rw-   0        0        0     1224 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/asdl.h
+-rw-rw-rw-   0        0        0      947 2023-07-13 11:29:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/ast.h
+-rw-rw-rw-   0        0        0      468 2023-07-13 11:22:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-07-13 10:19:37.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bltinmodule.h
+-rw-rw-rw-   0        0        0      885 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/boolobject.h
+-rw-rw-rw-   0        0        0     1484 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3048 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytesobject.h
+-rw-rw-rw-   0        0        0      712 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cellobject.h
+-rw-rw-rw-   0        0        0     5954 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/ceval.h
+-rw-rw-rw-   0        0        0     1657 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/code.h
+-rw-rw-rw-   0        0        0     6793 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/codecs.h
+-rw-rw-rw-   0        0        0     3778 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/compile.h
+-rw-rw-rw-   0        0        0     1806 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/complexobject.h
+-rw-rw-rw-   0        0        0     1962 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/context.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.832657 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/
+-rw-rw-rw-   0        0        0    14200 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4114 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1537 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/ceval.h
+-rw-rw-rw-   0        0        0     6989 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/code.h
+-rw-rw-rw-   0        0        0     3797 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4004 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3059 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1473 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/import.h
+-rw-rw-rw-   0        0        0    16979 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1364 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19358 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/object.h
+-rw-rw-rw-   0        0        0     4456 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     5101 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2096 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pymem.h
+-rw-rw-rw-   0        0        0    10134 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pystate.h
+-rw-rw-rw-   0        0        0      575 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46154 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9255 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/datetime.h
+-rw-rw-rw-   0        0        0     3019 2023-07-13 11:22:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/descrobject.h
+-rw-rw-rw-   0        0        0     3715 2023-07-13 11:29:20.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/dictobject.h
+-rw-rw-rw-   0        0        0    22469 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/enumobject.h
+-rw-rw-rw-   0        0        0     1624 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/errcode.h
+-rw-rw-rw-   0        0        0     1209 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/exports.h
+-rw-rw-rw-   0        0        0     1571 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileobject.h
+-rw-rw-rw-   0        0        0      597 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileutils.h
+-rw-rw-rw-   0        0        0     4360 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/frameobject.h
+-rw-rw-rw-   0        0        0     4057 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/funcobject.h
+-rw-rw-rw-   0        0        0      334 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3525 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/grammar.h
+-rw-rw-rw-   0        0        0     3026 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/import.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:08.901366 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/
+-rw-rw-rw-   0        0        0      953 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pegen_interface.h
+-rw-rw-rw-   0        0        0      479 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-07-13 10:22:11.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16977 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     3384 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     2620 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_byteswap.h
+-rw-rw-rw-   0        0        0      870 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3403 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      541 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      800 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      646 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1541 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     6647 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-07-13 10:19:38.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      473 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5233 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     5299 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0     1548 2023-07-13 11:22:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     4157 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     1936 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2032 2023-07-13 11:29:21.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3741 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3363 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3583 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4452 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      548 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3056 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      442 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      633 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/interpreteridobject.h
+-rw-rw-rw-   0        0        0      861 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/intrcheck.h
+-rw-rw-rw-   0        0        0      521 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/iterobject.h
+-rw-rw-rw-   0        0        0     1781 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/longintrepr.h
+-rw-rw-rw-   0        0        0     9513 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/marshal.h
+-rw-rw-rw-   0        0        0     2764 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/memoryobject.h
+-rw-rw-rw-   0        0        0     3775 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/methodobject.h
+-rw-rw-rw-   0        0        0     9959 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/modsupport.h
+-rw-rw-rw-   0        0        0     2361 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/namespaceobject.h
+-rw-rw-rw-   0        0        0     1281 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/node.h
+-rw-rw-rw-   0        0        0    24628 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/object.h
+-rw-rw-rw-   0        0        0     8423 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/odictobject.h
+-rw-rw-rw-   0        0        0     4900 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/osmodule.h
+-rw-rw-rw-   0        0        0     2958 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/parsetok.h
+-rw-rw-rw-   0        0        0     1300 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/patchlevel.h
+-rw-rw-rw-   0        0        0      846 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/picklebufobject.h
+-rw-rw-rw-   0        0        0     2474 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/py_curses.h
+-rw-rw-rw-   0        0        0     2744 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyarena.h
+-rw-rw-rw-   0        0        0     1725 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pycapsule.h
+-rw-rw-rw-   0        0        0    48109 2023-07-13 11:35:19.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyconfig.h
+-rw-rw-rw-   0        0        0     1387 2023-07-13 11:22:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.h
+-rw-rw-rw-   0        0        0    12427 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyexpat.h
+-rw-rw-rw-   0        0        0      444 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyfpe.h
+-rw-rw-rw-   0        0        0      466 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyframe.h
+-rw-rw-rw-   0        0        0     4263 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyhash.h
+-rw-rw-rw-   0        0        0     2136 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-07-13 10:22:12.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-07-13 11:29:22.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacro.h
+-rw-rw-rw-   0        0        0     8580 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymath.h
+-rw-rw-rw-   0        0        0     4406 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymem.h
+-rw-rw-rw-   0        0        0    31273 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyport.h
+-rw-rw-rw-   0        0        0     5250 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrtod.h
+-rw-rw-rw-   0        0        0     7673 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythonrun.h
+-rw-rw-rw-   0        0        0     5938 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythread.h
+-rw-rw-rw-   0        0        0     8928 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/pytime.h
+-rw-rw-rw-   0        0        0      628 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/rangeobject.h
+-rw-rw-rw-   0        0        0     3324 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/sliceobject.h
+-rw-rw-rw-   0        0        0     2030 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/structmember.h
+-rw-rw-rw-   0        0        0     1390 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/structseq.h
+-rw-rw-rw-   0        0        0     5307 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/symtable.h
+-rw-rw-rw-   0        0        0     1242 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/sysmodule.h
+-rw-rw-rw-   0        0        0     2642 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/token.h
+-rw-rw-rw-   0        0        0      584 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-07-13 10:19:39.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/tracemalloc.h
+-rw-rw-rw-   0        0        0     1614 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/tupleobject.h
+-rw-rw-rw-   0        0        0     2350 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/ucnhash.h
+-rw-rw-rw-   0        0        0    35426 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-07-13 11:22:24.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/warnings.h
+-rw-rw-rw-   0        0        0     2863 2023-07-13 11:29:23.000000 wasmpy-build-0.3.2/wasmpy_build/include/cp39/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-14 11:04:07.652953 wasmpy-build-0.3.2/wasmpy_build.egg-info/
+-rw-rw-rw-   0        0        0     1686 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    28923 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 11:04:07.000000 wasmpy-build-0.3.2/wasmpy_build.egg-info/top_level.txt
```

### Comparing `wasmpy-build-0.3.1/LICENSE` & `wasmpy-build-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/PKG-INFO` & `wasmpy-build-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.3.1
+Version: 0.3.2
 Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,11 +35,19 @@
 ```
 
 ### or build from source
 
 ```bash
 git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
 cd wasmpy-build
-python -m pip install -r requirements.txt
+pip install patch
 python patch_headers.py
 python -m pip install .
 ```
+
+# Usage
+
+Simply pass the C or C++ file and any extra arguments straight to the compiler.
+
+```bash
+wasmpy-build my_file.c -o my_file.wasm
+```
```

### Comparing `wasmpy-build-0.3.1/README.md` & `wasmpy-build-0.3.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -16,11 +16,19 @@
 ```
 
 ### or build from source
 
 ```bash
 git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
 cd wasmpy-build
-python -m pip install -r requirements.txt
+pip install patch
 python patch_headers.py
 python -m pip install .
 ```
+
+# Usage
+
+Simply pass the C or C++ file and any extra arguments straight to the compiler.
+
+```bash
+wasmpy-build my_file.c -o my_file.wasm
+```
```

### Comparing `wasmpy-build-0.3.1/setup.py` & `wasmpy-build-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             paths.append(os.path.join("..", path, file))
 
     return paths
 
 
 setuptools.setup(
     name="wasmpy-build",
-    version="0.3.1",
+    version="0.3.2",
     author="Olivia Ryan",
     author_email="olivia.r.dev@gmail.com",
     description="WebAssembly build tool for CPython C extensions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/olivi-r/wasmpy-build",
     packages=["wasmpy_build"],
@@ -33,9 +33,9 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: MIT License",
     ],
     license="MIT",
     python_requires=">=3.8",
-    install_requires=["appdirs", "patch", "requests", "tqdm"],
+    install_requires=["appdirs", "requests", "tqdm"],
 )
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/__init__.py` & `wasmpy-build-0.3.2/wasmpy_build/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,21 +57,20 @@
     # find cpython include files
     include_dir = os.path.join(os.path.dirname(__file__), "include", "cp")
     version = "".join(str(i) for i in sys.version_info[:2])
     include_dir += version
 
     args = [
         f"{sdk_dir}/sdk-{platform.system()}/bin/clang",
-        "--target=wasm32-unknown-wasi",
         f"--sysroot={sdk_dir}/sdk-{platform.system()}/share/wasi-sysroot",
+        "--target=wasm32-wasi-threads",
+        "-pthread",
         "-nostartfiles",
-        "-D_POSIX_THREADS",
-        "-DHAVE_PTHREAD_STUBS",
-        "-DSIZEOF_WCHAR_T=2",
         f"-I{include_dir}",
+        "-Wl,--no-entry,-export-dynamic,--allow-undefined",
     ] + command
 
     print(" ".join(args))
     try:
         subprocess.call(args)
 
     except FileNotFoundError:
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/LICENSE` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/Python.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/Python.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #ifndef Py_PYTHON_H
 #define Py_PYTHON_H
 /* Since this is a "meta-include" file, no #ifdef __cplusplus / extern "C" { */
 
 /* Include nearly all Python header files */
 
 #include "patchlevel.h"
-//#include "pyconfig.h"
+#include "pyconfig.h"
 #include "pymacconfig.h"
 
 #include <limits.h>
 
 #ifndef UCHAR_MAX
 #error "Something's broken.  UCHAR_MAX should be defined in limits.h."
 #endif
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/boolobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cellobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/classobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/codecs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/complexobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/frameobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/odictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/picklebufobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pyctype.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pydebug.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pythonrun.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/pytime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/cpython/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/datetime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/descrobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/dynamic_annotations.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/errcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/eval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/exports.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/floatobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/funcobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/genobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_accu.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_asdl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ast.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_atomic.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic.h`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #endif
 
 #ifndef Py_BUILD_CORE
 #  error "this header requires Py_BUILD_CORE define"
 #endif
 
 #include "dynamic_annotations.h"   /* _Py_ANNOTATE_MEMORY_ORDER */
-//#include "pyconfig.h"
+#include "pyconfig.h"
 
 #ifdef HAVE_STD_ATOMIC
 #  include <stdatomic.h>
 #endif
 
 
 #if defined(_MSC_VER)
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_call.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_condvar.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_gc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_gil.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_hamt.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_interp.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_long.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_parser.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_runtime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_symtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/internal/pycore_warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/intrcheck.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/iterobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/longintrepr.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/longobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/marshal.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/memoryobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/modsupport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/moduleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/opcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/osdefs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/patchlevel.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/patchlevel.h`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 #define PY_RELEASE_LEVEL_FINAL  0xF     /* Serial should be 0 here */
                                         /* Higher for patch releases */
 
 /* Version parsed out into numeric values */
 /*--start constants--*/
 #define PY_MAJOR_VERSION        3
 #define PY_MINOR_VERSION        10
-#define PY_MICRO_VERSION        11
+#define PY_MICRO_VERSION        12
 #define PY_RELEASE_LEVEL        PY_RELEASE_LEVEL_FINAL
 #define PY_RELEASE_SERIAL       0
 
 /* Version as a string */
-#define PY_VERSION              "3.10.11+"
+#define PY_VERSION              "3.10.12+"
 /*--end constants--*/
 
 /* Version as a single 4-byte hex number, e.g. 0x010502B2 == 1.5.2b2.
    Use this for numeric comparisons, e.g. #if PY_VERSION_HEX >= ... */
 #define PY_VERSION_HEX ((PY_MAJOR_VERSION << 24) | \
                         (PY_MINOR_VERSION << 16) | \
                         (PY_MICRO_VERSION <<  8) | \
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/py_curses.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pycapsule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pydtrace.d` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pydtrace.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyexpat.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymacconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymacro.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymath.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYMATH_H
 #define Py_PYMATH_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 /**************************************************************************
 Symbols and macros to supply platform-independent interfaces to mathematical
 functions and constants
 **************************************************************************/
 
 /* Python provides implementations for copysign, round and hypot in
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pyport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pyport.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYPORT_H
 #define Py_PYPORT_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 #include <inttypes.h>
 
 
 /* Defines to build Python and its standard library:
  *
  * - Py_BUILD_CORE: Build Python core. Give access to Python internals, but
@@ -739,15 +739,15 @@
 
 #if LONG_BIT != 8 * SIZEOF_LONG
 /* 04-Oct-2000 LONG_BIT is apparently (mis)defined as 64 on some recent
  * 32-bit platforms using gcc.  We try to catch that here at compile-time
  * rather than waiting for integer multiplication to trigger bogus
  * overflows.
  */
-//#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
+#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 
 /*
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystrhex.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pystrtod.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pythonrun.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/pythread.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/rangeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/setobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/sliceobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/structmember.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/structseq.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/token.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/tracemalloc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/typeslots.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp310/weakrefobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp310/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/LICENSE` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/Python.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/Python.h`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #ifndef Py_PYTHON_H
 #define Py_PYTHON_H
 
 // Since this is a "meta-include" file, no #ifdef __cplusplus / extern "C" {
 
 // Include Python header files
 #include "patchlevel.h"
-//#include "pyconfig.h"
+#include "pyconfig.h"
 #include "pymacconfig.h"
 
 #if defined(__sgi) && !defined(_SGI_MP_SOURCE)
 #  define _SGI_MP_SOURCE
 #endif
 
 // stdlib.h, stdio.h, errno.h and string.h headers are not used by Python
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/boolobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/codecs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/complexobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/cellobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/classobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/complexobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/descrobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/floatobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/frameobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/funcobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/genobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/longintrepr.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/longobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/modsupport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/odictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/picklebufobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pthread_stubs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyctype.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pydebug.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pyframe.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pythonrun.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pythread.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/pytime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/setobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/cpython/weakrefobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/cpython/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/datetime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/descrobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/dynamic_annotations.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/errcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/exports.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/floatobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_accu.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_asdl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ast.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_atomic.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic.h`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #endif
 
 #ifndef Py_BUILD_CORE
 #  error "this header requires Py_BUILD_CORE define"
 #endif
 
 #include "dynamic_annotations.h"   /* _Py_ANNOTATE_MEMORY_ORDER */
-//#include "pyconfig.h"
+#include "pyconfig.h"
 
 #ifdef HAVE_STD_ATOMIC
 #  include <stdatomic.h>
 #endif
 
 
 #if defined(_MSC_VER)
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_call.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_condvar.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_dict.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dict.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_exceptions.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_frame.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_frame.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_gc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_genobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_gil.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_objects.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_global_strings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_hamt.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_interp.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_list.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_list.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_long.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_opcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_parser.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pymath.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_runtime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_runtime_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_signal.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_strhex.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_strhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_structseq.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_symtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_tuple.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_tuple.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_typeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/internal/pycore_warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/intrcheck.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/iterobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/longobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/marshal.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/memoryobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/modsupport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/moduleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/opcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/osdefs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/patchlevel.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/patchlevel.h`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 #define PY_RELEASE_LEVEL_GAMMA  0xC     /* For release candidates */
 #define PY_RELEASE_LEVEL_FINAL  0xF     /* Serial should be 0 here */
                                         /* Higher for patch releases */
 
 /* Version parsed out into numeric values */
 /*--start constants--*/
 #define PY_MAJOR_VERSION        3
-#define PY_MINOR_VERSION        11
-#define PY_MICRO_VERSION        3
+#define PY_MINOR_VERSION        8
+#define PY_MICRO_VERSION        17
 #define PY_RELEASE_LEVEL        PY_RELEASE_LEVEL_FINAL
 #define PY_RELEASE_SERIAL       0
 
 /* Version as a string */
-#define PY_VERSION              "3.11.3+"
+#define PY_VERSION              "3.8.17+"
 /*--end constants--*/
 
 /* Version as a single 4-byte hex number, e.g. 0x010502B2 == 1.5.2b2.
    Use this for numeric comparisons, e.g. #if PY_VERSION_HEX >= ... */
 #define PY_VERSION_HEX ((PY_MAJOR_VERSION << 24) | \
                         (PY_MINOR_VERSION << 16) | \
                         (PY_MICRO_VERSION <<  8) | \
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/py_curses.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pybuffer.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pybuffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pycapsule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pydtrace.d` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pydtrace.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyexpat.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyframe.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymacconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymacro.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymath.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pyport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pyport.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYPORT_H
 #define Py_PYPORT_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 #include <inttypes.h>
 
 #include <limits.h>
 #ifndef UCHAR_MAX
 #  error "limits.h must define UCHAR_MAX"
 #endif
@@ -594,15 +594,15 @@
 
 #if LONG_BIT != 8 * SIZEOF_LONG
 /* 04-Oct-2000 LONG_BIT is apparently (mis)defined as 64 on some recent
  * 32-bit platforms using gcc.  We try to catch that here at compile-time
  * rather than waiting for integer multiplication to trigger bogus
  * overflows.
  */
-//#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
+#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 
 /*
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pystrtod.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pythonrun.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pythread.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/pytypedefs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/pytypedefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/rangeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/setobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/sliceobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/structmember.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/structseq.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/token.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/tracemalloc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/typeslots.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp311/weakrefobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/LICENSE` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/Python-ast.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/Python.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/Python.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #ifndef Py_PYTHON_H
 #define Py_PYTHON_H
 /* Since this is a "meta-include" file, no #ifdef __cplusplus / extern "C" { */
 
 /* Include nearly all Python header files */
 
 #include "patchlevel.h"
-//#include "pyconfig.h"
+#include "pyconfig.h"
 #include "pymacconfig.h"
 
 #include <limits.h>
 
 #ifndef UCHAR_MAX
 #error "Something's broken.  UCHAR_MAX should be defined in limits.h."
 #endif
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/asdl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/ast.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/boolobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/bytes_methods.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cellobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/classobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/codecs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/complexobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/cpython/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/datetime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/descrobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/dynamic_annotations.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/errcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/eval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/floatobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/frameobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/funcobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/genobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/graminit.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/grammar.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_accu.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_atomic.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_atomic.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 #ifndef Py_BUILD_CORE
 #  error "this header requires Py_BUILD_CORE define"
 #endif
 
 #include "dynamic_annotations.h"
 
-//#include "pyconfig.h"
+#include "pyconfig.h"
 
 #if defined(HAVE_STD_ATOMIC)
 #include <stdatomic.h>
 #endif
 
 
 #if defined(_MSC_VER)
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_condvar.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_gil.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_hamt.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_long.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/internal/pycore_warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/intrcheck.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/iterobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/longintrepr.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/longobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/marshal.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/memoryobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/modsupport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/moduleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/node.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/odictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/opcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/osdefs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/parsetok.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/patchlevel.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/patchlevel.h`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 #define PY_RELEASE_LEVEL_GAMMA  0xC     /* For release candidates */
 #define PY_RELEASE_LEVEL_FINAL  0xF     /* Serial should be 0 here */
                                         /* Higher for patch releases */
 
 /* Version parsed out into numeric values */
 /*--start constants--*/
 #define PY_MAJOR_VERSION        3
-#define PY_MINOR_VERSION        8
-#define PY_MICRO_VERSION        16
+#define PY_MINOR_VERSION        9
+#define PY_MICRO_VERSION        17
 #define PY_RELEASE_LEVEL        PY_RELEASE_LEVEL_FINAL
 #define PY_RELEASE_SERIAL       0
 
 /* Version as a string */
-#define PY_VERSION              "3.8.16+"
+#define PY_VERSION              "3.9.17+"
 /*--end constants--*/
 
 /* Version as a single 4-byte hex number, e.g. 0x010502B2 == 1.5.2b2.
    Use this for numeric comparisons, e.g. #if PY_VERSION_HEX >= ... */
 #define PY_VERSION_HEX ((PY_MAJOR_VERSION << 24) | \
                         (PY_MINOR_VERSION << 16) | \
                         (PY_MICRO_VERSION <<  8) | \
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/picklebufobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/py_curses.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyarena.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pycapsule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyctype.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pydebug.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pydtrace.d` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pydtrace.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyexpat.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymacconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymacro.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymath.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYMATH_H
 #define Py_PYMATH_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 /**************************************************************************
 Symbols and macros to supply platform-independent interfaces to mathematical
 functions and constants
 **************************************************************************/
 
 /* Python provides implementations for copysign, round and hypot in
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pyport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pyport.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYPORT_H
 #define Py_PYPORT_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 #include <inttypes.h>
 
 
 /* Defines to build Python and its standard library:
  *
  * - Py_BUILD_CORE: Build Python core. Give access to Python internals, but
@@ -719,15 +719,15 @@
 
 #if LONG_BIT != 8 * SIZEOF_LONG
 /* 04-Oct-2000 LONG_BIT is apparently (mis)defined as 64 on some recent
  * 32-bit platforms using gcc.  We try to catch that here at compile-time
  * rather than waiting for integer multiplication to trigger bogus
  * overflows.
  */
-//#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
+#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 
 /*
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystrhex.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pystrtod.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pythonrun.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pythread.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/pytime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/pytime.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #ifndef Py_LIMITED_API
 #ifndef Py_PYTIME_H
 #define Py_PYTIME_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 #include "object.h"
 
 /**************************************************************************
 Symbols and macros to supply platform-independent interfaces to time related
 functions and constants
 **************************************************************************/
 #ifdef __cplusplus
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/rangeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/setobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/sliceobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/structmember.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/structseq.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/symtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/token.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/tracemalloc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/typeslots.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/ucnhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp38/weakrefobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp38/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/LICENSE` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/Python-ast.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/Python.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/Python.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #ifndef Py_PYTHON_H
 #define Py_PYTHON_H
 /* Since this is a "meta-include" file, no #ifdef __cplusplus / extern "C" { */
 
 /* Include nearly all Python header files */
 
 #include "patchlevel.h"
-//#include "pyconfig.h"
+#include "pyconfig.h"
 #include "pymacconfig.h"
 
 #include <limits.h>
 
 #ifndef UCHAR_MAX
 #error "Something's broken.  UCHAR_MAX should be defined in limits.h."
 #endif
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/asdl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/ast.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/boolobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cellobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/classobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/codecs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/compile.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/complexobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/abstract.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/bytesobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/frameobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/cpython/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/datetime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/descrobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/dictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/dynamic_annotations.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/errcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/eval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/exports.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/fileobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/floatobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/funcobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/genobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/graminit.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/grammar.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/import.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pegen_interface.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pegen_interface.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_accu.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_atomic.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_atomic.h`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #endif
 
 #ifndef Py_BUILD_CORE
 #  error "this header requires Py_BUILD_CORE define"
 #endif
 
 #include "dynamic_annotations.h"   /* _Py_ANNOTATE_MEMORY_ORDER */
-//#include "pyconfig.h"
+#include "pyconfig.h"
 
 #if defined(HAVE_STD_ATOMIC)
 #include <stdatomic.h>
 #endif
 
 
 #if defined(_MSC_VER)
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_byteswap.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_call.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_ceval.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_code.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_condvar.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_context.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_gc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_gil.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_hamt.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_interp.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_long.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_runtime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/internal/pycore_warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/intrcheck.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/iterobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/listobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/longintrepr.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/longobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/marshal.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/memoryobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/methodobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/modsupport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/moduleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/node.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/object.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/objimpl.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/odictobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/opcode.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/osdefs.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/parsetok.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/patchlevel.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp311/patchlevel.h`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 #define PY_RELEASE_LEVEL_GAMMA  0xC     /* For release candidates */
 #define PY_RELEASE_LEVEL_FINAL  0xF     /* Serial should be 0 here */
                                         /* Higher for patch releases */
 
 /* Version parsed out into numeric values */
 /*--start constants--*/
 #define PY_MAJOR_VERSION        3
-#define PY_MINOR_VERSION        9
-#define PY_MICRO_VERSION        16
+#define PY_MINOR_VERSION        11
+#define PY_MICRO_VERSION        4
 #define PY_RELEASE_LEVEL        PY_RELEASE_LEVEL_FINAL
 #define PY_RELEASE_SERIAL       0
 
 /* Version as a string */
-#define PY_VERSION              "3.9.16+"
+#define PY_VERSION              "3.11.4+"
 /*--end constants--*/
 
 /* Version as a single 4-byte hex number, e.g. 0x010502B2 == 1.5.2b2.
    Use this for numeric comparisons, e.g. #if PY_VERSION_HEX >= ... */
 #define PY_VERSION_HEX ((PY_MAJOR_VERSION << 24) | \
                         (PY_MINOR_VERSION << 16) | \
                         (PY_MICRO_VERSION <<  8) | \
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/picklebufobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/py_curses.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyarena.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pycapsule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyctype.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pydebug.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pydtrace.d` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pydtrace.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyerrors.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyexpat.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pylifecycle.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymacconfig.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymacro.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymath.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYMATH_H
 #define Py_PYMATH_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 /**************************************************************************
 Symbols and macros to supply platform-independent interfaces to mathematical
 functions and constants
 **************************************************************************/
 
 /* Python provides implementations for copysign, round and hypot in
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pymem.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pyport.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pyport.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #ifndef Py_PYPORT_H
 #define Py_PYPORT_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 
 #include <inttypes.h>
 
 
 /* Defines to build Python and its standard library:
  *
  * - Py_BUILD_CORE: Build Python core. Give access to Python internals, but
@@ -734,15 +734,15 @@
 
 #if LONG_BIT != 8 * SIZEOF_LONG
 /* 04-Oct-2000 LONG_BIT is apparently (mis)defined as 64 on some recent
  * 32-bit platforms using gcc.  We try to catch that here at compile-time
  * rather than waiting for integer multiplication to trigger bogus
  * overflows.
  */
-//#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
+#error "LONG_BIT definition appears wrong for platform (bad gcc/glibc config?)."
 #endif
 
 #ifdef __cplusplus
 }
 #endif
 
 /*
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystate.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystrhex.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pystrtod.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pythonrun.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pythread.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/pytime.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/pytime.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #ifndef Py_LIMITED_API
 #ifndef Py_PYTIME_H
 #define Py_PYTIME_H
 
-//#include "pyconfig.h" /* include for defines */
+#include "pyconfig.h" /* include for defines */
 #include "object.h"
 
 /**************************************************************************
 Symbols and macros to supply platform-independent interfaces to time related
 functions and constants
 **************************************************************************/
 #ifdef __cplusplus
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/rangeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/setobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/sliceobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/structmember.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/structseq.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/symtable.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/sysmodule.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/token.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/traceback.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/tracemalloc.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/tupleobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/typeslots.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/ucnhash.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/unicodeobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/warnings.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build/include/cp39/weakrefobject.h` & `wasmpy-build-0.3.2/wasmpy_build/include/cp39/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.3.1/wasmpy_build.egg-info/PKG-INFO` & `wasmpy-build-0.3.2/wasmpy_build.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.3.1
+Version: 0.3.2
 Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,11 +35,19 @@
 ```
 
 ### or build from source
 
 ```bash
 git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
 cd wasmpy-build
-python -m pip install -r requirements.txt
+pip install patch
 python patch_headers.py
 python -m pip install .
 ```
+
+# Usage
+
+Simply pass the C or C++ file and any extra arguments straight to the compiler.
+
+```bash
+wasmpy-build my_file.c -o my_file.wasm
+```
```

### Comparing `wasmpy-build-0.3.1/wasmpy_build.egg-info/SOURCES.txt` & `wasmpy-build-0.3.2/wasmpy_build.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 wasmpy_build/include/cp310/objimpl.h
 wasmpy_build/include/cp310/opcode.h
 wasmpy_build/include/cp310/osdefs.h
 wasmpy_build/include/cp310/osmodule.h
 wasmpy_build/include/cp310/patchlevel.h
 wasmpy_build/include/cp310/py_curses.h
 wasmpy_build/include/cp310/pycapsule.h
+wasmpy_build/include/cp310/pyconfig.h
 wasmpy_build/include/cp310/pydtrace.d
 wasmpy_build/include/cp310/pydtrace.h
 wasmpy_build/include/cp310/pyerrors.h
 wasmpy_build/include/cp310/pyexpat.h
 wasmpy_build/include/cp310/pyframe.h
 wasmpy_build/include/cp310/pyhash.h
 wasmpy_build/include/cp310/pylifecycle.h
@@ -212,14 +213,15 @@
 wasmpy_build/include/cp311/opcode.h
 wasmpy_build/include/cp311/osdefs.h
 wasmpy_build/include/cp311/osmodule.h
 wasmpy_build/include/cp311/patchlevel.h
 wasmpy_build/include/cp311/py_curses.h
 wasmpy_build/include/cp311/pybuffer.h
 wasmpy_build/include/cp311/pycapsule.h
+wasmpy_build/include/cp311/pyconfig.h
 wasmpy_build/include/cp311/pydtrace.d
 wasmpy_build/include/cp311/pydtrace.h
 wasmpy_build/include/cp311/pyerrors.h
 wasmpy_build/include/cp311/pyexpat.h
 wasmpy_build/include/cp311/pyframe.h
 wasmpy_build/include/cp311/pyhash.h
 wasmpy_build/include/cp311/pylifecycle.h
@@ -422,14 +424,15 @@
 wasmpy_build/include/cp38/osmodule.h
 wasmpy_build/include/cp38/parsetok.h
 wasmpy_build/include/cp38/patchlevel.h
 wasmpy_build/include/cp38/picklebufobject.h
 wasmpy_build/include/cp38/py_curses.h
 wasmpy_build/include/cp38/pyarena.h
 wasmpy_build/include/cp38/pycapsule.h
+wasmpy_build/include/cp38/pyconfig.h
 wasmpy_build/include/cp38/pyctype.h
 wasmpy_build/include/cp38/pydebug.h
 wasmpy_build/include/cp38/pydtrace.d
 wasmpy_build/include/cp38/pydtrace.h
 wasmpy_build/include/cp38/pyerrors.h
 wasmpy_build/include/cp38/pyexpat.h
 wasmpy_build/include/cp38/pyfpe.h
@@ -558,14 +561,15 @@
 wasmpy_build/include/cp39/osmodule.h
 wasmpy_build/include/cp39/parsetok.h
 wasmpy_build/include/cp39/patchlevel.h
 wasmpy_build/include/cp39/picklebufobject.h
 wasmpy_build/include/cp39/py_curses.h
 wasmpy_build/include/cp39/pyarena.h
 wasmpy_build/include/cp39/pycapsule.h
+wasmpy_build/include/cp39/pyconfig.h
 wasmpy_build/include/cp39/pyctype.h
 wasmpy_build/include/cp39/pydebug.h
 wasmpy_build/include/cp39/pydtrace.d
 wasmpy_build/include/cp39/pydtrace.h
 wasmpy_build/include/cp39/pyerrors.h
 wasmpy_build/include/cp39/pyexpat.h
 wasmpy_build/include/cp39/pyfpe.h
```

