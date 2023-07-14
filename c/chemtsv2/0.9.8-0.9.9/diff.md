# Comparing `tmp/chemtsv2-0.9.8.tar.gz` & `tmp/chemtsv2-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chemtsv2-0.9.8.tar", last modified: Fri Feb  3 10:48:18 2023, max compression
+gzip compressed data, was "dist/chemtsv2-0.9.9.tar", last modified: Mon Feb  6 09:30:23 2023, max compression
```

## Comparing `chemtsv2-0.9.8.tar` & `chemtsv2-0.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     1071 2022-08-24 05:53:34.000000 chemtsv2-0.9.8/LICENSE
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     1198 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/PKG-INFO
--rw-rw-r--   0 ishida    (1000) ishida    (1000)    10533 2023-01-27 08:48:43.000000 chemtsv2-0.9.8/README.md
-drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2/
--rw-rw-r--   0 ishida    (1000) ishida    (1000)        0 2022-03-30 07:13:09.000000 chemtsv2-0.9.8/chemtsv2/__init__.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)    13364 2022-12-06 02:39:24.000000 chemtsv2-0.9.8/chemtsv2/mcts.py
-drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2/misc/
--rw-rw-r--   0 ishida    (1000) ishida    (1000)      413 2022-08-04 08:55:02.000000 chemtsv2-0.9.8/chemtsv2/misc/debug_check.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     3643 2022-03-30 07:13:09.000000 chemtsv2-0.9.8/chemtsv2/misc/manage_qsub_parallel.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     1055 2022-03-30 07:13:09.000000 chemtsv2-0.9.8/chemtsv2/misc/qsub_parallel_job.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)      448 2022-06-17 07:18:52.000000 chemtsv2-0.9.8/chemtsv2/misc/scaler.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     5404 2022-10-06 08:13:52.000000 chemtsv2-0.9.8/chemtsv2/mp_utils.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)    41121 2023-02-03 09:45:29.000000 chemtsv2-0.9.8/chemtsv2/parallel_mcts.py
--rwxrwxr-x   0 ishida    (1000) ishida    (1000)      994 2022-03-30 07:13:09.000000 chemtsv2-0.9.8/chemtsv2/preprocessing.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     7381 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2/run.py
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     6512 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2/run_mp.py
--rwxrwxr-x   0 ishida    (1000) ishida    (1000)     9002 2022-12-06 02:39:24.000000 chemtsv2-0.9.8/chemtsv2/utils.py
-drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     1198 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/PKG-INFO
--rw-rw-r--   0 ishida    (1000) ishida    (1000)      510 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/SOURCES.txt
--rw-rw-r--   0 ishida    (1000) ishida    (1000)        1 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/dependency_links.txt
--rw-rw-r--   0 ishida    (1000) ishida    (1000)       82 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/entry_points.txt
--rw-rw-r--   0 ishida    (1000) ishida    (1000)       89 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/requires.txt
--rw-rw-r--   0 ishida    (1000) ishida    (1000)        9 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/chemtsv2.egg-info/top_level.txt
--rw-rw-r--   0 ishida    (1000) ishida    (1000)       38 2023-02-03 10:48:18.000000 chemtsv2-0.9.8/setup.cfg
--rw-rw-r--   0 ishida    (1000) ishida    (1000)     2029 2023-02-03 10:46:28.000000 chemtsv2-0.9.8/setup.py
+drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     1071 2022-08-24 05:53:34.000000 chemtsv2-0.9.9/LICENSE
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     1198 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/PKG-INFO
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)    10533 2023-01-27 08:48:43.000000 chemtsv2-0.9.9/README.md
+drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2/
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)        0 2022-03-30 07:13:09.000000 chemtsv2-0.9.9/chemtsv2/__init__.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)    13364 2022-12-06 02:39:24.000000 chemtsv2-0.9.9/chemtsv2/mcts.py
+drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2/misc/
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)      413 2022-08-04 08:55:02.000000 chemtsv2-0.9.9/chemtsv2/misc/debug_check.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     3643 2022-03-30 07:13:09.000000 chemtsv2-0.9.9/chemtsv2/misc/manage_qsub_parallel.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     1055 2022-03-30 07:13:09.000000 chemtsv2-0.9.9/chemtsv2/misc/qsub_parallel_job.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)      448 2022-06-17 07:18:52.000000 chemtsv2-0.9.9/chemtsv2/misc/scaler.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     5404 2022-10-06 08:13:52.000000 chemtsv2-0.9.9/chemtsv2/mp_utils.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)    41121 2023-02-03 09:45:29.000000 chemtsv2-0.9.9/chemtsv2/parallel_mcts.py
+-rwxrwxr-x   0 ishida    (1000) ishida    (1000)      994 2022-03-30 07:13:09.000000 chemtsv2-0.9.9/chemtsv2/preprocessing.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     7381 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2/run.py
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     6530 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2/run_mp.py
+-rwxrwxr-x   0 ishida    (1000) ishida    (1000)     9002 2022-12-06 02:39:24.000000 chemtsv2-0.9.9/chemtsv2/utils.py
+drwxrwxr-x   0 ishida    (1000) ishida    (1000)        0 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     1198 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/PKG-INFO
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)      510 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)        1 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)       82 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/entry_points.txt
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)       89 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/requires.txt
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)        9 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/chemtsv2.egg-info/top_level.txt
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)       38 2023-02-06 09:30:23.000000 chemtsv2-0.9.9/setup.cfg
+-rw-rw-r--   0 ishida    (1000) ishida    (1000)     2029 2023-02-06 09:28:51.000000 chemtsv2-0.9.9/setup.py
```

### Comparing `chemtsv2-0.9.8/LICENSE` & `chemtsv2-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/PKG-INFO` & `chemtsv2-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemtsv2
-Version: 0.9.8
+Version: 0.9.9
 Summary:  ChemTSv2 is a flexible and versatile molecule generator based on reinforcement learning with natural language processing.
 Home-page: https://github.com/molecule-generator-collection/ChemTSv2
 Download-URL: https://github.com/molecule-generator-collection/ChemTSv2
 Author: Shoichi Ishida
 Author-email: ishida.sho.nm@yokohama-cu.ac.jp
 Maintainer: Shoichi Ishida
 Maintainer-email: ishida.sho.nm@yokohama-cu.ac.jp
```

### Comparing `chemtsv2-0.9.8/README.md` & `chemtsv2-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/mcts.py` & `chemtsv2-0.9.9/chemtsv2/mcts.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/misc/manage_qsub_parallel.py` & `chemtsv2-0.9.9/chemtsv2/misc/manage_qsub_parallel.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/misc/qsub_parallel_job.py` & `chemtsv2-0.9.9/chemtsv2/misc/qsub_parallel_job.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/mp_utils.py` & `chemtsv2-0.9.9/chemtsv2/mp_utils.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/parallel_mcts.py` & `chemtsv2-0.9.9/chemtsv2/parallel_mcts.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/preprocessing.py` & `chemtsv2-0.9.9/chemtsv2/preprocessing.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/run.py` & `chemtsv2-0.9.9/chemtsv2/run.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2/run_mp.py` & `chemtsv2-0.9.9/chemtsv2/run_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,11 +192,11 @@
     logger.info(f"Done MCTS execution [rank {rank}]")
 
     search.gather_results()
     comm.barrier()
     if rank==0:
         search.flush()
         logger.info("FINISH!")
-
+    MPI.Finalize()
 
 if __name__ == "__main__":
     main()
```

### Comparing `chemtsv2-0.9.8/chemtsv2/utils.py` & `chemtsv2-0.9.9/chemtsv2/utils.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-0.9.8/chemtsv2.egg-info/PKG-INFO` & `chemtsv2-0.9.9/chemtsv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemtsv2
-Version: 0.9.8
+Version: 0.9.9
 Summary:  ChemTSv2 is a flexible and versatile molecule generator based on reinforcement learning with natural language processing.
 Home-page: https://github.com/molecule-generator-collection/ChemTSv2
 Download-URL: https://github.com/molecule-generator-collection/ChemTSv2
 Author: Shoichi Ishida
 Author-email: ishida.sho.nm@yokohama-cu.ac.jp
 Maintainer: Shoichi Ishida
 Maintainer-email: ishida.sho.nm@yokohama-cu.ac.jp
```

### Comparing `chemtsv2-0.9.8/setup.py` & `chemtsv2-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     maintainer="Shoichi Ishida",
     maintainer_email="ishida.sho.nm@yokohama-cu.ac.jp",
     description=DOCLINES[0],
     long_description='\n'.join(DOCLINES[2:]),
     long_description_content_type="text/markdown",
     license="MIT LIcense",
     url="https://github.com/molecule-generator-collection/ChemTSv2",
-    version="0.9.8",
+    version="0.9.9",
     download_url="https://github.com/molecule-generator-collection/ChemTSv2",
     python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
     packages=PACKAGES,
     entry_points={'console_scripts': CONSOLE_SCRIPTS},
     classifiers=CLASSIFIERS
 )
```

