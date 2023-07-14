# Comparing `tmp/molmap-1.3.9.7.tar.gz` & `tmp/molmap-1.3.9.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molmap-1.3.9.7.tar", last modified: Fri Jul 14 05:59:13 2023, max compression
+gzip compressed data, was "molmap-1.3.9.7.1.tar", last modified: Fri Jul 14 06:15:16 2023, max compression
```

## Comparing `molmap-1.3.9.7.tar` & `molmap-1.3.9.7.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.401748 molmap-1.3.9.7/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1094 2022-03-04 04:56:20.000000 molmap-1.3.9.7/LICENSE
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      707 2022-06-16 13:13:40.000000 molmap-1.3.9.7/MANIFEST.in
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7315 2023-07-14 05:59:13.401748 molmap-1.3.9.7/PKG-INFO
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6972 2022-06-16 13:05:46.000000 molmap-1.3.9.7/README.md
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.369747 molmap-1.3.9.7/docs/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      638 2022-03-04 04:48:27.000000 molmap-1.3.9.7/docs/Makefile
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   557944 2022-03-04 04:49:27.000000 molmap-1.3.9.7/docs/Overall.png
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   276233 2022-03-04 04:49:27.000000 molmap-1.3.9.7/docs/code_example.png
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)  5176976 2022-03-04 04:48:26.000000 molmap-1.3.9.7/docs/fmap_dynamicly.gif
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      799 2022-03-04 04:48:26.000000 molmap-1.3.9.7/docs/make.bat
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   268771 2022-03-04 04:48:26.000000 molmap-1.3.9.7/docs/molmap.log.png
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   842653 2022-03-04 04:49:27.000000 molmap-1.3.9.7/docs/net.png
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      241 2022-06-16 10:03:04.000000 molmap-1.3.9.7/docs/requirements.txt
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.369747 molmap-1.3.9.7/molmap/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      443 2023-07-14 05:54:53.000000 molmap-1.3.9.7/molmap/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    17532 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/_base.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    17443 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/agg.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.369747 molmap-1.3.9.7/molmap/config/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2868 2022-06-16 13:54:47.000000 molmap-1.3.9.7/molmap/config/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    72089 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/config/descriptor_scale.cfg.gzip
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   524598 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/config/fingerprint_scale.cfg.gzip
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12617 2022-06-16 05:19:17.000000 molmap-1.3.9.7/molmap/cpd.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.373747 molmap-1.3.9.7/molmap/dataset/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    32060 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/dataset/FreeSolv.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    11534 2022-06-16 04:24:43.000000 molmap-1.3.9.7/molmap/dataset/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   175387 2022-06-16 04:21:46.000000 molmap-1.3.9.7/molmap/dataset/bace.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    95512 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/dataset/clintox.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    96699 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/dataset/delaney-processed.csv
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.373747 molmap-1.3.9.7/molmap/feature/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)       52 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.377748 molmap-1.3.9.7/molmap/feature/descriptor/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4948 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      812 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/autocorr.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    19472 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/charge.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      779 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/connectivity.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     5945 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/constitution.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      389 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/estate.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1308 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/fragment.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      932 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/infocontent.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4458 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/kappa.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      608 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/matrix.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2101 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/moe.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4476 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/path.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6580 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/property.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14988 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/descriptor/topology.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.381748 molmap-1.3.9.7/molmap/feature/fingerprint/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4012 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      459 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/atompairs.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      403 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/fingerprint/avalonfp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      224 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/estatefp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      473 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/maccskeys.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    13970 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/maccskeys.xlsx
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4360 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/fingerprint/map4.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      549 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/fingerprint/mhfp6.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1668 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/mnimalfatures.fdef
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      517 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/fingerprint/morganfp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1894 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/pharmErGfp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2050 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/fingerprint/pharmPointfp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    47310 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/pubchemfp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    41242 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/pubchemfp.xlsx
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1163 2022-12-20 04:27:38.000000 molmap-1.3.9.7/molmap/feature/fingerprint/rdkitfp.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7155 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/smarts_maccskey.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      828 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/feature/fingerprint/smarts_pharmacophore.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    34320 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/smarts_pubchem.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      474 2022-03-04 04:56:17.000000 molmap-1.3.9.7/molmap/feature/fingerprint/torsions.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.381748 molmap-1.3.9.7/molmap/feature/sequence/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-06-15 15:18:05.000000 molmap-1.3.9.7/molmap/feature/sequence/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.381748 molmap-1.3.9.7/molmap/feature/sequence/aas/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.381748 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6320 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_AAComposition.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    33216 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_Autocorrelation.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    27039 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_CTD.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    23539 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_PseudoAAC.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    25809 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_QuasiSequenceOrder.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6263 2022-06-15 15:25:42.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.381748 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.381748 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      731 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.397748 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    64330 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   448037 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex_meta.pkl
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   181049 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    26896 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix_meta.pkl
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   110004 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14737 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix_meta.pkl
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    40387 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/Tomii_aa_group_info.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)  2764681 2022-03-04 04:56:15.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/all_data.csv
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   495135 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/all_meta.csv
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.397748 molmap-1.3.9.7/molmap/feature/sequence/nas/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-06-16 13:18:05.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/__init__.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.401748 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6224 2022-06-16 12:02:38.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12000 2022-06-16 13:12:38.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/ac.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     3308 2022-06-16 13:12:42.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/acutil.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.401748 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/data/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    15344 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/data/mmc3.data
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    19670 2022-03-04 04:56:16.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/data/mmc4.data
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     8934 2022-06-16 13:12:48.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/nac.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    23239 2022-06-16 13:13:05.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/nacutil.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    20407 2022-06-16 13:13:09.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/psenac.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     9473 2022-06-16 13:13:16.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/psenacutil.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      186 2022-06-16 13:13:20.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/test.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12773 2022-06-16 13:13:25.000000 molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/util.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12610 2022-03-04 04:56:09.000000 molmap-1.3.9.7/molmap/map.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.401748 molmap-1.3.9.7/molmap/model/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      176 2023-02-03 12:59:43.000000 molmap-1.3.9.7/molmap/model/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14328 2023-02-03 08:38:18.000000 molmap-1.3.9.7/molmap/model/cbks.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1016 2022-03-04 04:56:09.000000 molmap-1.3.9.7/molmap/model/importance.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      885 2022-03-04 04:56:09.000000 molmap-1.3.9.7/molmap/model/loss.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    28857 2023-02-04 03:45:43.000000 molmap-1.3.9.7/molmap/model/model.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7738 2022-03-04 04:56:09.000000 molmap-1.3.9.7/molmap/model/net.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14707 2022-06-16 05:14:46.000000 molmap-1.3.9.7/molmap/pdb.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    10764 2022-06-16 13:17:39.000000 molmap-1.3.9.7/molmap/seq.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2184 2022-03-04 04:56:18.000000 molmap-1.3.9.7/molmap/show.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.401748 molmap-1.3.9.7/molmap/utils/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/__init__.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2382 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/calculator.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6295 2022-03-04 04:56:20.000000 molmap-1.3.9.7/molmap/utils/distances.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4489 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/logtools.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7104 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/matrixopt.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     5489 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/multiproc.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2227 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/summary.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     8573 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/vismap.py
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     9060 2022-03-04 04:56:19.000000 molmap-1.3.9.7/molmap/utils/vismap2.py
-drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 05:59:13.369747 molmap-1.3.9.7/molmap.egg-info/
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7315 2023-07-14 05:59:13.000000 molmap-1.3.9.7/molmap.egg-info/PKG-INFO
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4265 2023-07-14 05:59:13.000000 molmap-1.3.9.7/molmap.egg-info/SOURCES.txt
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        1 2023-07-14 05:59:13.000000 molmap-1.3.9.7/molmap.egg-info/dependency_links.txt
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      326 2023-07-14 05:59:13.000000 molmap-1.3.9.7/molmap.egg-info/requires.txt
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        7 2023-07-14 05:59:13.000000 molmap-1.3.9.7/molmap.egg-info/top_level.txt
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      355 2023-07-14 05:55:12.000000 molmap-1.3.9.7/requirements.txt
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)       38 2023-07-14 05:59:13.401748 molmap-1.3.9.7/setup.cfg
--rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2244 2022-06-15 15:05:41.000000 molmap-1.3.9.7/setup.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.168910 molmap-1.3.9.7.1/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1094 2022-03-04 04:56:20.000000 molmap-1.3.9.7.1/LICENSE
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      707 2022-06-16 13:13:40.000000 molmap-1.3.9.7.1/MANIFEST.in
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7317 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/PKG-INFO
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6972 2022-06-16 13:05:46.000000 molmap-1.3.9.7.1/README.md
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.160910 molmap-1.3.9.7.1/docs/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      638 2022-03-04 04:48:27.000000 molmap-1.3.9.7.1/docs/Makefile
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   557944 2022-03-04 04:49:27.000000 molmap-1.3.9.7.1/docs/Overall.png
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   276233 2022-03-04 04:49:27.000000 molmap-1.3.9.7.1/docs/code_example.png
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)  5176976 2022-03-04 04:48:26.000000 molmap-1.3.9.7.1/docs/fmap_dynamicly.gif
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      799 2022-03-04 04:48:26.000000 molmap-1.3.9.7.1/docs/make.bat
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   268771 2022-03-04 04:48:26.000000 molmap-1.3.9.7.1/docs/molmap.log.png
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   842653 2022-03-04 04:49:27.000000 molmap-1.3.9.7.1/docs/net.png
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      241 2022-06-16 10:03:04.000000 molmap-1.3.9.7.1/docs/requirements.txt
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.160910 molmap-1.3.9.7.1/molmap/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      445 2023-07-14 06:09:07.000000 molmap-1.3.9.7.1/molmap/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    17532 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/_base.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    17443 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/agg.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.160910 molmap-1.3.9.7.1/molmap/config/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2868 2022-06-16 13:54:47.000000 molmap-1.3.9.7.1/molmap/config/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    72089 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/config/descriptor_scale.cfg.gzip
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   524598 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/config/fingerprint_scale.cfg.gzip
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12617 2022-06-16 05:19:17.000000 molmap-1.3.9.7.1/molmap/cpd.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/dataset/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    32060 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/dataset/FreeSolv.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    11534 2022-06-16 04:24:43.000000 molmap-1.3.9.7.1/molmap/dataset/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   175387 2022-06-16 04:21:46.000000 molmap-1.3.9.7.1/molmap/dataset/bace.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    95512 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/dataset/clintox.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    96699 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/dataset/delaney-processed.csv
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)       52 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/descriptor/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4948 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      812 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/autocorr.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    19472 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/charge.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      779 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/connectivity.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     5945 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/constitution.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      389 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/estate.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1308 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/fragment.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      932 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/infocontent.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4458 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/kappa.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      608 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/matrix.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2101 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/moe.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4476 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/path.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6580 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/property.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14988 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/descriptor/topology.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/fingerprint/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4012 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      459 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/atompairs.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      403 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/avalonfp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      224 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/estatefp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      473 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/maccskeys.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    13970 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/maccskeys.xlsx
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4360 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/map4.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      549 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/mhfp6.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1668 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/mnimalfatures.fdef
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      517 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/morganfp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1894 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/pharmErGfp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2050 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/pharmPointfp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    47310 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/pubchemfp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    41242 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/pubchemfp.xlsx
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1163 2022-12-20 04:27:38.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/rdkitfp.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7155 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/smarts_maccskey.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      828 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/smarts_pharmacophore.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    34320 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/smarts_pubchem.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      474 2022-03-04 04:56:17.000000 molmap-1.3.9.7.1/molmap/feature/fingerprint/torsions.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-06-15 15:18:05.000000 molmap-1.3.9.7.1/molmap/feature/sequence/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/aas/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6320 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_AAComposition.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    33216 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_Autocorrelation.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    27039 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_CTD.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    23539 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_PseudoAAC.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    25809 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_QuasiSequenceOrder.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6263 2022-06-15 15:25:42.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      731 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    64330 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   448037 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex_meta.pkl
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   181049 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    26896 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix_meta.pkl
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   110004 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14737 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix_meta.pkl
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    40387 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/Tomii_aa_group_info.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)  2764681 2022-03-04 04:56:15.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/all_data.csv
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)   495135 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/all_meta.csv
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/nas/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-06-16 13:18:05.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/__init__.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6224 2022-06-16 12:02:38.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12000 2022-06-16 13:12:38.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/ac.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     3308 2022-06-16 13:12:42.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/acutil.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/data/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    15344 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/data/mmc3.data
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    19670 2022-03-04 04:56:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/data/mmc4.data
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     8934 2022-06-16 13:12:48.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/nac.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    23239 2022-06-16 13:13:05.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/nacutil.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    20407 2022-06-16 13:13:09.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/psenac.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     9473 2022-06-16 13:13:16.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/psenacutil.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      186 2022-06-16 13:13:20.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/test.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12773 2022-06-16 13:13:25.000000 molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/util.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    12610 2022-03-04 04:56:09.000000 molmap-1.3.9.7.1/molmap/map.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/model/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      176 2023-02-03 12:59:43.000000 molmap-1.3.9.7.1/molmap/model/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14328 2023-02-03 08:38:18.000000 molmap-1.3.9.7.1/molmap/model/cbks.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     1016 2022-03-04 04:56:09.000000 molmap-1.3.9.7.1/molmap/model/importance.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      885 2022-03-04 04:56:09.000000 molmap-1.3.9.7.1/molmap/model/loss.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    28857 2023-02-04 03:45:43.000000 molmap-1.3.9.7.1/molmap/model/model.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7738 2022-03-04 04:56:09.000000 molmap-1.3.9.7.1/molmap/model/net.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    14707 2022-06-16 05:14:46.000000 molmap-1.3.9.7.1/molmap/pdb.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)    10764 2022-06-16 13:17:39.000000 molmap-1.3.9.7.1/molmap/seq.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2184 2022-03-04 04:56:18.000000 molmap-1.3.9.7.1/molmap/show.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.164910 molmap-1.3.9.7.1/molmap/utils/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/__init__.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2382 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/calculator.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     6295 2022-03-04 04:56:20.000000 molmap-1.3.9.7.1/molmap/utils/distances.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4489 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/logtools.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7104 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/matrixopt.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     5489 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/multiproc.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2227 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/summary.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     8573 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/vismap.py
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     9060 2022-03-04 04:56:19.000000 molmap-1.3.9.7.1/molmap/utils/vismap2.py
+drwxrwxr-x   0 shenwanxiang  (1001) shenwanxiang  (1001)        0 2023-07-14 06:15:16.160910 molmap-1.3.9.7.1/molmap.egg-info/
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     7317 2023-07-14 06:15:16.000000 molmap-1.3.9.7.1/molmap.egg-info/PKG-INFO
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     4265 2023-07-14 06:15:16.000000 molmap-1.3.9.7.1/molmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        1 2023-07-14 06:15:16.000000 molmap-1.3.9.7.1/molmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      302 2023-07-14 06:15:16.000000 molmap-1.3.9.7.1/molmap.egg-info/requires.txt
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)        7 2023-07-14 06:15:16.000000 molmap-1.3.9.7.1/molmap.egg-info/top_level.txt
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)      332 2023-07-14 06:15:01.000000 molmap-1.3.9.7.1/requirements.txt
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)       38 2023-07-14 06:15:16.168910 molmap-1.3.9.7.1/setup.cfg
+-rw-rw-r--   0 shenwanxiang  (1001) shenwanxiang  (1001)     2244 2022-06-15 15:05:41.000000 molmap-1.3.9.7.1/setup.py
```

### Comparing `molmap-1.3.9.7/LICENSE` & `molmap-1.3.9.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/MANIFEST.in` & `molmap-1.3.9.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/PKG-INFO` & `molmap-1.3.9.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmap
-Version: 1.3.9.7
+Version: 1.3.9.7.1
 Summary: MolMap: An Efficient Convolutional Neural Network Based Molecular Deep Learning Tool
 Home-page: https://github.com/shenwanxiang/bidd-molmap
 Author: WanXiang Shen
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molmap Version: 1.3.9.7 Summary: MolMap: An
+Metadata-Version: 2.1 Name: molmap Version: 1.3.9.7.1 Summary: MolMap: An
 Efficient Convolutional Neural Network Based Molecular Deep Learning Tool Home-
 page: https://github.com/shenwanxiang/bidd-molmap Author: WanXiang Shen
 License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE [./docs/molmap.log.png] ![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg) [![Documentation
 Status](https://readthedocs.org/projects/molmap/badge/?version=latest)](https:/
 /molmap.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://
```

### Comparing `molmap-1.3.9.7/README.md` & `molmap-1.3.9.7.1/README.md`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/Makefile` & `molmap-1.3.9.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/Overall.png` & `molmap-1.3.9.7.1/docs/Overall.png`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/code_example.png` & `molmap-1.3.9.7.1/docs/code_example.png`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/fmap_dynamicly.gif` & `molmap-1.3.9.7.1/docs/fmap_dynamicly.gif`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/make.bat` & `molmap-1.3.9.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/molmap.log.png` & `molmap-1.3.9.7.1/docs/molmap.log.png`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/docs/net.png` & `molmap-1.3.9.7.1/docs/net.png`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/_base.py` & `molmap-1.3.9.7.1/molmap/_base.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/agg.py` & `molmap-1.3.9.7.1/molmap/agg.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/config/__init__.py` & `molmap-1.3.9.7.1/molmap/config/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/config/descriptor_scale.cfg.gzip` & `molmap-1.3.9.7.1/molmap/config/descriptor_scale.cfg.gzip`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/config/fingerprint_scale.cfg.gzip` & `molmap-1.3.9.7.1/molmap/config/fingerprint_scale.cfg.gzip`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/cpd.py` & `molmap-1.3.9.7.1/molmap/cpd.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/dataset/FreeSolv.csv` & `molmap-1.3.9.7.1/molmap/dataset/FreeSolv.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/dataset/__init__.py` & `molmap-1.3.9.7.1/molmap/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/dataset/bace.csv` & `molmap-1.3.9.7.1/molmap/dataset/bace.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/dataset/clintox.csv` & `molmap-1.3.9.7.1/molmap/dataset/clintox.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/dataset/delaney-processed.csv` & `molmap-1.3.9.7.1/molmap/dataset/delaney-processed.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/__init__.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/autocorr.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/autocorr.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/charge.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/charge.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/connectivity.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/connectivity.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/constitution.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/constitution.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/fragment.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/fragment.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/infocontent.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/infocontent.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/kappa.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/kappa.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/matrix.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/matrix.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/moe.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/moe.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/path.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/path.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/property.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/property.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/descriptor/topology.py` & `molmap-1.3.9.7.1/molmap/feature/descriptor/topology.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/__init__.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/maccskeys.xlsx` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/maccskeys.xlsx`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/map4.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/map4.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/mhfp6.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/mhfp6.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/mnimalfatures.fdef` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/mnimalfatures.fdef`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/morganfp.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/morganfp.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/pharmErGfp.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/pharmErGfp.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/pharmPointfp.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/pharmPointfp.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/pubchemfp.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/pubchemfp.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/pubchemfp.xlsx` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/pubchemfp.xlsx`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/rdkitfp.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/rdkitfp.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/smarts_maccskey.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/smarts_maccskey.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/smarts_pharmacophore.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/smarts_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/fingerprint/smarts_pubchem.py` & `molmap-1.3.9.7.1/molmap/feature/fingerprint/smarts_pubchem.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_AAComposition.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_AAComposition.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_Autocorrelation.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_Autocorrelation.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_CTD.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_CTD.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_PseudoAAC.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_PseudoAAC.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/_QuasiSequenceOrder.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/_QuasiSequenceOrder.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/global_feature/__init__.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/global_feature/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/__init__.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex.csv` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex_meta.pkl` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/01_aaindex_meta.pkl`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix.csv` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix_meta.pkl` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/02_aametrix_meta.pkl`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix.csv` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix_meta.pkl` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/03_aametrix_meta.pkl`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/Tomii_aa_group_info.csv` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/Tomii_aa_group_info.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/all_data.csv` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/all_data.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/aas/local_feature/aai/result_data/all_meta.csv` & `molmap-1.3.9.7.1/molmap/feature/sequence/aas/local_feature/aai/result_data/all_meta.csv`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/__init__.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/__init__.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/ac.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/ac.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/acutil.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/acutil.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/data/mmc3.data` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/data/mmc3.data`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/data/mmc4.data` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/data/mmc4.data`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/nac.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/nac.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/nacutil.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/nacutil.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/psenac.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/psenac.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/psenacutil.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/psenacutil.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/feature/sequence/nas/global_feature/util.py` & `molmap-1.3.9.7.1/molmap/feature/sequence/nas/global_feature/util.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/map.py` & `molmap-1.3.9.7.1/molmap/map.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/model/cbks.py` & `molmap-1.3.9.7.1/molmap/model/cbks.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/model/importance.py` & `molmap-1.3.9.7.1/molmap/model/importance.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/model/loss.py` & `molmap-1.3.9.7.1/molmap/model/loss.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/model/model.py` & `molmap-1.3.9.7.1/molmap/model/model.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/model/net.py` & `molmap-1.3.9.7.1/molmap/model/net.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/pdb.py` & `molmap-1.3.9.7.1/molmap/pdb.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/seq.py` & `molmap-1.3.9.7.1/molmap/seq.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/show.py` & `molmap-1.3.9.7.1/molmap/show.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/calculator.py` & `molmap-1.3.9.7.1/molmap/utils/calculator.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/distances.py` & `molmap-1.3.9.7.1/molmap/utils/distances.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/logtools.py` & `molmap-1.3.9.7.1/molmap/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/matrixopt.py` & `molmap-1.3.9.7.1/molmap/utils/matrixopt.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/multiproc.py` & `molmap-1.3.9.7.1/molmap/utils/multiproc.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/summary.py` & `molmap-1.3.9.7.1/molmap/utils/summary.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/vismap.py` & `molmap-1.3.9.7.1/molmap/utils/vismap.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap/utils/vismap2.py` & `molmap-1.3.9.7.1/molmap/utils/vismap2.py`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/molmap.egg-info/PKG-INFO` & `molmap-1.3.9.7.1/molmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmap
-Version: 1.3.9.7
+Version: 1.3.9.7.1
 Summary: MolMap: An Efficient Convolutional Neural Network Based Molecular Deep Learning Tool
 Home-page: https://github.com/shenwanxiang/bidd-molmap
 Author: WanXiang Shen
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molmap Version: 1.3.9.7 Summary: MolMap: An
+Metadata-Version: 2.1 Name: molmap Version: 1.3.9.7.1 Summary: MolMap: An
 Efficient Convolutional Neural Network Based Molecular Deep Learning Tool Home-
 page: https://github.com/shenwanxiang/bidd-molmap Author: WanXiang Shen
 License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/markdown
 Provides-Extra: dev License-File: LICENSE [./docs/molmap.log.png] ![License:
 MIT](https://img.shields.io/badge/License-MIT-yellow.svg) [![Documentation
 Status](https://readthedocs.org/projects/molmap/badge/?version=latest)](https:/
 /molmap.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://
```

### Comparing `molmap-1.3.9.7/molmap.egg-info/SOURCES.txt` & `molmap-1.3.9.7.1/molmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molmap-1.3.9.7/setup.py` & `molmap-1.3.9.7.1/setup.py`

 * *Files identical despite different names*

