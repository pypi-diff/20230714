# Comparing `tmp/crimm-2023.7a1-py3-none-any.whl.zip` & `tmp/crimm-2023.7a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 906163 bytes, number of entries: 63
+Zip file size: 909518 bytes, number of entries: 64
 -rw-r--r--  2.0 unx     8392 b- defN 23-May-23 16:20 crimm/Fetchers.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-23 16:20 crimm/__init__.py
 -rw-r--r--  2.0 unx     4311 b- defN 23-Jun-01 01:50 crimm/Adaptors/OMMAdaptors.py
 -rw-r--r--  2.0 unx    12043 b- defN 23-Jul-14 18:34 crimm/Adaptors/PropKaAdaptors.py
 -rw-r--r--  2.0 unx     2924 b- defN 23-May-23 16:20 crimm/Adaptors/RDKitAdaptor.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 16:20 crimm/Adaptors/__init__.py
+-rw-r--r--  2.0 unx     9550 b- defN 23-Jul-14 19:47 crimm/Adaptors/charmm_struct_prep.py
 -rw-r--r--  2.0 unx     4641 b- defN 23-Jul-12 22:59 crimm/Adaptors/pyCHARMMAdaptors.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 02:30 crimm/Data/__init__.py
 -rw-r--r--  2.0 unx      528 b- defN 23-May-09 20:11 crimm/Data/connect_records.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Jun-21 01:06 crimm/Data/constants.py
 -rw-r--r--  2.0 unx    11837 b- defN 23-Jul-14 18:34 crimm/Data/propka.cfg
 -rw-r--r--  2.0 unx   159620 b- defN 23-May-23 16:20 crimm/Data/toppar/carb.prm
 -rw-r--r--  2.0 unx   292987 b- defN 23-May-23 16:20 crimm/Data/toppar/carb.rtf
@@ -53,13 +54,13 @@
 -rw-r--r--  2.0 unx      494 b- defN 23-May-23 16:20 crimm/StructEntities/__init__.py
 -rw-r--r--  2.0 unx     9264 b- defN 23-May-23 16:20 crimm/Superimpose/ChainSuperimposer.py
 -rw-r--r--  2.0 unx       65 b- defN 23-May-23 16:20 crimm/Superimpose/__init__.py
 -rw-r--r--  2.0 unx       52 b- defN 23-Jun-20 22:04 crimm/Utils/__init__.py
 -rw-r--r--  2.0 unx     6329 b- defN 23-Jun-20 22:01 crimm/Utils/cuda_avail.py
 -rw-r--r--  2.0 unx     8050 b- defN 23-Jul-07 15:47 crimm/Visualization/NGLVisualization.py
 -rw-r--r--  2.0 unx       85 b- defN 23-May-23 16:20 crimm/Visualization/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-14 18:42 crimm-2023.7a1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3041 b- defN 23-Jul-14 18:42 crimm-2023.7a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 18:42 crimm-2023.7a1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-14 18:42 crimm-2023.7a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5313 b- defN 23-Jul-14 18:42 crimm-2023.7a1.dist-info/RECORD
-63 files, 5404738 bytes uncompressed, 897811 bytes compressed:  83.4%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-14 19:50 crimm-2023.7a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3600 b- defN 23-Jul-14 19:50 crimm-2023.7a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 19:50 crimm-2023.7a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-14 19:50 crimm-2023.7a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5406 b- defN 23-Jul-14 19:50 crimm-2023.7a2.dist-info/RECORD
+64 files, 5414940 bytes uncompressed, 901018 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: crimm/Adaptors/RDKitAdaptor.py
 Comment: 
 
 Filename: crimm/Adaptors/__init__.py
 Comment: 
 
+Filename: crimm/Adaptors/charmm_struct_prep.py
+Comment: 
+
 Filename: crimm/Adaptors/pyCHARMMAdaptors.py
 Comment: 
 
 Filename: crimm/Data/__init__.py
 Comment: 
 
 Filename: crimm/Data/connect_records.py
@@ -168,23 +171,23 @@
 
 Filename: crimm/Visualization/NGLVisualization.py
 Comment: 
 
 Filename: crimm/Visualization/__init__.py
 Comment: 
 
-Filename: crimm-2023.7a1.dist-info/LICENSE
+Filename: crimm-2023.7a2.dist-info/LICENSE
 Comment: 
 
-Filename: crimm-2023.7a1.dist-info/METADATA
+Filename: crimm-2023.7a2.dist-info/METADATA
 Comment: 
 
-Filename: crimm-2023.7a1.dist-info/WHEEL
+Filename: crimm-2023.7a2.dist-info/WHEEL
 Comment: 
 
-Filename: crimm-2023.7a1.dist-info/top_level.txt
+Filename: crimm-2023.7a2.dist-info/top_level.txt
 Comment: 
 
-Filename: crimm-2023.7a1.dist-info/RECORD
+Filename: crimm-2023.7a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `crimm-2023.7a1.dist-info/LICENSE` & `crimm-2023.7a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `crimm-2023.7a1.dist-info/METADATA` & `crimm-2023.7a2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: crimm
-Version: 2023.7a1
+Version: 2023.7a2
 Summary: Chemistry with the ReInvented Macromolecular
 Author-email: Truman Xu <ziqiaoxu@umich.edu>
 Project-URL: Homepage, https://github.com/Truman-Xu/crimm
 Project-URL: Bug Tracker, https://github.com/Truman-Xu/crimm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython (>=1.80)
-Requires-Dist: ipywidgets (>=7)
-Requires-Dist: nglview (>=3.0.3)
+Requires-Dist: ipywidgets (>=8)
+Requires-Dist: nglview (==3.0.6)
 Requires-Dist: scipy (>=1.7.1)
 Requires-Dist: requests (>=2.26.0)
 
 # **crimm**
 **crimm** stands for **Chemistry with the ReInvented Macromolecular Mechanics**. This project aims to integrate and supplement CHARMM with better object handle and APIs
 
 ## Why *"reinvent the wheel"*
 This is a toolkit that is under active development, where many useful macromolecular modeling routines are selected to be reimplemented. This is an attempt to unify many macromolecular preparation/modeling routine under one platform while offering proper object handles and APIs in python. While currently, we aim to integrate with CHARMM and pyCHARMM, the broader goal is to provide highly usable, integratable, and scriptable python library/platform for simplifying any macromolecular modeling pipelines.
 
 -----------------
 ## Installations
 crimm can be installed by `pip install crimm`
 
-crimm requires `python>=3.10`. The main dependencies are biopython, nglview, scipy, and requests. To use the adaptors, the respective packages need to be installed separately (e.g. pyCHARMM, rdkit, etc.)
+crimm requires `python>=3.8`. The main dependencies are biopython, nglview, scipy, and requests. To use the adaptors, the respective packages need to be installed separately (e.g. pyCHARMM, rdkit, etc.)
+
+If you are installing crimm on a fresh enviroment, it is recommended to use the `env.yaml` file. 
+
+```conda env create -f env.yaml```
+
+**Note**
+1. `OpenMM` and `pyCHARMM` still need to be installed separately in this environment if you require these in your pipeline.
+
+2. If you are using a centralized `Jupyterlab` installation and install the ipython kernel to it, the `nglview` version should match in both environment (`crimm` env and `jupyterlab` env). Otherwise the ipywidget for `nglview` could break. The required `nglview` version is currently 3.0.6
 
 -----------------
 ## Base Library and Object Handles
 This library is built upon the excellent Biopython library. The macromolecular entity representations are derived from Biopython's entity classes and follow the same hierarchy. As a result, the entities in this library remain fully compatible with all functions and routines provided in Biopython.
 ## Parser Module
 New and improved mmCIF parser is implemented to allow accurate structure representations and more complete information.
```

## Comparing `crimm-2023.7a1.dist-info/RECORD` & `crimm-2023.7a2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 crimm/Fetchers.py,sha256=hcr_1juTwBN_rFQ0jCoEGgfgFjHSTAbt9qSthrSCXU8,8392
 crimm/__init__.py,sha256=85WLB6GVoxD0CjuJoVxtw867y7ZgBWTHXPa1PkzJqB0,283
 crimm/Adaptors/OMMAdaptors.py,sha256=9ZSHVHNKCb4WR-DHPXxtSO9l7RTeCTrZq5axojRNbu8,4311
 crimm/Adaptors/PropKaAdaptors.py,sha256=HE1HvvmKKUfzN4m6J6UjDTSdjH8AyM1Rq8GwcdltgSQ,12043
 crimm/Adaptors/RDKitAdaptor.py,sha256=kNaaxdnku8apO6X7WPOup0ib6L1J6e3HCeG-tuX2sEk,2924
 crimm/Adaptors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+crimm/Adaptors/charmm_struct_prep.py,sha256=EsZmewOn9x_iPLmMCmq5Mu75Bl-RJP232CO4__nTfSw,9550
 crimm/Adaptors/pyCHARMMAdaptors.py,sha256=HU3yIEBxY_d73mdWFDH5kvd61L6TRV6S7Zg_GRBZM1M,4641
 crimm/Data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 crimm/Data/connect_records.py,sha256=PF1OwvlDwPWOvVydVCsTjneqL-5a5iBgrQRESp46l84,528
 crimm/Data/constants.py,sha256=5AjVTxJphY4SoP6t7pU8wttDlDQohHYL6fcxUtcLj-0,77
 crimm/Data/propka.cfg,sha256=LHOhaJgP4IXgQHojx4TTsRftfjzu9bDfotFOpZdYwuY,11837
 crimm/Data/toppar/carb.prm,sha256=ms1fHYh6-vXizcDkIEQKuRLMK1hPeHEg1oRd0HfVjuY,159620
 crimm/Data/toppar/carb.rtf,sha256=YoTbNM4AOLZHmB1_rfrTU-wXFao8buBJDPP5TkjXXNk,292987
@@ -52,12 +53,12 @@
 crimm/StructEntities/__init__.py,sha256=DLz6nR8DtWi8NcN80o81_UK-1BhwjtlsRRawLl9TDFU,494
 crimm/Superimpose/ChainSuperimposer.py,sha256=u_GUprrMcIxgX0ZiIdWcVh5Mtg2s4VQJe770Gnet0-8,9264
 crimm/Superimpose/__init__.py,sha256=EVr-1WXnwrcf5fG0n5cqWx-0Qbpehn4wgiP84srHw4w,65
 crimm/Utils/__init__.py,sha256=cxiQpI5zc3qV7fj-kIB11P5Qbpxpr6IxTyKkNdN9OPI,52
 crimm/Utils/cuda_avail.py,sha256=xGM_tu5ab9I3umZRZr_C3mtX6gXFkG6dKvJ9f1nUSnc,6329
 crimm/Visualization/NGLVisualization.py,sha256=AZoVVX8g7-QKnOBNWTMjEi4cyTv_X4EaslEY3LdEG84,8050
 crimm/Visualization/__init__.py,sha256=ZSs4-SVsG0URA3zkexnm2WL8xSB446Lg1SOo4rleCug,85
-crimm-2023.7a1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-crimm-2023.7a1.dist-info/METADATA,sha256=fTvy1IKMb9oiBASmOhcAw6M5uaib66NIwulZZ_Z9Pwg,3041
-crimm-2023.7a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-crimm-2023.7a1.dist-info/top_level.txt,sha256=ILqOjbvY8wu0ZdDaZxTx19ZTJS__dFPnmiFHN-3I1h4,6
-crimm-2023.7a1.dist-info/RECORD,,
+crimm-2023.7a2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+crimm-2023.7a2.dist-info/METADATA,sha256=jYl64eziRgdNXP9_8f78YIhVTM98ZqIqjouO4TrVRR8,3600
+crimm-2023.7a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+crimm-2023.7a2.dist-info/top_level.txt,sha256=ILqOjbvY8wu0ZdDaZxTx19ZTJS__dFPnmiFHN-3I1h4,6
+crimm-2023.7a2.dist-info/RECORD,,
```

