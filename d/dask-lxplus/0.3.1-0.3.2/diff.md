# Comparing `tmp/dask_lxplus-0.3.1.tar.gz` & `tmp/dask_lxplus-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_lxplus-0.3.1.tar", last modified: Thu Jun 29 07:16:34 2023, max compression
+gzip compressed data, was "dask_lxplus-0.3.2.tar", last modified: Fri Jul 14 14:54:00 2023, max compression
```

## Comparing `dask_lxplus-0.3.1.tar` & `dask_lxplus-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.983399 dask_lxplus-0.3.1/
--rw-r--r--   0 ben        (501) staff       (20)      589 2022-08-10 12:35:46.000000 dask_lxplus-0.3.1/LICENSE.txt
--rw-r--r--   0 ben        (501) staff       (20)       27 2022-08-10 15:10:59.000000 dask_lxplus-0.3.1/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     2799 2023-06-29 07:16:34.983469 dask_lxplus-0.3.1/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     2064 2022-08-10 14:26:52.000000 dask_lxplus-0.3.1/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.982274 dask_lxplus-0.3.1/dask_lxplus/
--rw-r--r--   0 ben        (501) staff       (20)      286 2021-11-26 14:54:16.000000 dask_lxplus-0.3.1/dask_lxplus/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     8966 2023-06-29 07:14:25.000000 dask_lxplus-0.3.1/dask_lxplus/cluster.py
--rw-r--r--   0 ben        (501) staff       (20)      525 2021-11-26 14:54:16.000000 dask_lxplus-0.3.1/dask_lxplus/config.py
--rw-r--r--   0 ben        (501) staff       (20)      743 2023-06-28 14:50:15.000000 dask_lxplus-0.3.1/dask_lxplus/jobqueue-cern.yaml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.983099 dask_lxplus-0.3.1/dask_lxplus.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2799 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      348 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)      166 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-06-29 07:16:34.000000 dask_lxplus-0.3.1/dask_lxplus.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     1010 2023-06-29 07:16:34.984005 dask_lxplus-0.3.1/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)       61 2021-11-26 14:54:16.000000 dask_lxplus-0.3.1/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-06-29 07:16:34.983225 dask_lxplus-0.3.1/tests/
--rw-r--r--   0 ben        (501) staff       (20)     4100 2023-06-28 14:50:15.000000 dask_lxplus-0.3.1/tests/test_cluster.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-14 14:54:00.662728 dask_lxplus-0.3.2/
+-rw-r--r--   0 ben        (501) staff       (20)      589 2022-08-10 12:35:46.000000 dask_lxplus-0.3.2/LICENSE.txt
+-rw-r--r--   0 ben        (501) staff       (20)       27 2022-08-10 15:10:59.000000 dask_lxplus-0.3.2/MANIFEST.in
+-rw-r--r--   0 ben        (501) staff       (20)     2799 2023-07-14 14:54:00.662810 dask_lxplus-0.3.2/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     2064 2022-08-10 14:26:52.000000 dask_lxplus-0.3.2/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-14 14:54:00.661577 dask_lxplus-0.3.2/dask_lxplus/
+-rw-r--r--   0 ben        (501) staff       (20)      286 2021-11-26 14:54:16.000000 dask_lxplus-0.3.2/dask_lxplus/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     9059 2023-07-14 14:51:12.000000 dask_lxplus-0.3.2/dask_lxplus/cluster.py
+-rw-r--r--   0 ben        (501) staff       (20)      525 2021-11-26 14:54:16.000000 dask_lxplus-0.3.2/dask_lxplus/config.py
+-rw-r--r--   0 ben        (501) staff       (20)      743 2023-06-28 14:50:15.000000 dask_lxplus-0.3.2/dask_lxplus/jobqueue-cern.yaml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-14 14:54:00.662381 dask_lxplus-0.3.2/dask_lxplus.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2799 2023-07-14 14:54:00.000000 dask_lxplus-0.3.2/dask_lxplus.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      348 2023-07-14 14:54:00.000000 dask_lxplus-0.3.2/dask_lxplus.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-14 14:54:00.000000 dask_lxplus-0.3.2/dask_lxplus.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)      150 2023-07-14 14:54:00.000000 dask_lxplus-0.3.2/dask_lxplus.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-14 14:54:00.000000 dask_lxplus-0.3.2/dask_lxplus.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      993 2023-07-14 14:54:00.663215 dask_lxplus-0.3.2/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)       61 2021-11-26 14:54:16.000000 dask_lxplus-0.3.2/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-14 14:54:00.662518 dask_lxplus-0.3.2/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     4915 2023-07-14 14:51:12.000000 dask_lxplus-0.3.2/tests/test_cluster.py
```

### Comparing `dask_lxplus-0.3.1/LICENSE.txt` & `dask_lxplus-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.1/PKG-INFO` & `dask_lxplus-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask_lxplus
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/cernops/dask-lxplus
 Author: Ben Jones
 Author-email: b.jones@cern.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `dask_lxplus-0.3.1/README.md` & `dask_lxplus-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.1/dask_lxplus/cluster.py` & `dask_lxplus-0.3.2/dask_lxplus/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,31 +185,32 @@
         See the class __init__ for the details of the arguments.
         """
         modified = kwargs.copy()
 
         container_runtime = container_runtime or dask.config.get(f"jobqueue.{cls.config_name}.container-runtime")
         worker_image = worker_image or dask.config.get(f"jobqueue.{cls.config_name}.worker-image")
 
-
-        has_logdir = "log_directory" in modified and modified["log_directory"]
-        xroot_url = get_xroot_url(modified["log_directory"]) if has_logdir and modified["log_directory"].startswith("/eos/") else None
+        logdir = modified.get("log_directory", dask.config.get(f"jobqueue.{cls.config_name}.log-directory", None))
+        if logdir:
+            modified["log_directory"] = logdir
+        xroot_url = get_xroot_url(modified["log_directory"]) if logdir and modified["log_directory"].startswith("/eos/") else None
 
         modified["job_extra_directives"] = merge(
             {"universe": "docker" if container_runtime == "docker" else "vanilla"},
             {"docker_image": f'"{worker_image}"'} if container_runtime == "docker" else None,
             {"MY.SingularityImage": f'"{worker_image}"'} if container_runtime == "singularity" else None,
             {"request_gpus": str(gpus)} if gpus is not None else None,
             {"MY.IsDaskWorker": "true"},
             # getenv justified in case of LCG as both sides have to be the same environment
             {"getenv": "true"} if lcg else None,
             {"output_destination": f"{xroot_url}"} if xroot_url else None,
             {"Output": "worker-$(ClusterId).$(ProcId).out"} if xroot_url else None,
             {"Error": "worker-$(ClusterId).$(ProcId).err"} if xroot_url else None,
             {"Log": "worker-$(ClusterId).log"} if xroot_url else None,
-            {"MY.SpoolOnEvict": False} if has_logdir else None,
+            {"MY.SpoolOnEvict": False} if logdir else None,
             # extra user input
             kwargs.get("job_extra_directives", dask.config.get(f"jobqueue.{cls.config_name}.job_extra_directives")),
             kwargs.get("job_extra", dask.config.get(f"jobqueue.{cls.config_name}.job_extra")),
             {"JobBatchName": f'"{batch_name or dask.config.get(f"jobqueue.{cls.config_name}.batch-name")}"'},
             # never transfer files
             {"transfer_output_files": '""'}
         )
```

### Comparing `dask_lxplus-0.3.1/dask_lxplus/config.py` & `dask_lxplus-0.3.2/dask_lxplus/config.py`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.1/dask_lxplus/jobqueue-cern.yaml` & `dask_lxplus-0.3.2/dask_lxplus/jobqueue-cern.yaml`

 * *Files identical despite different names*

### Comparing `dask_lxplus-0.3.1/dask_lxplus.egg-info/PKG-INFO` & `dask_lxplus-0.3.2/dask_lxplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-lxplus
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/cernops/dask-lxplus
 Author: Ben Jones
 Author-email: b.jones@cern.ch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
```

### Comparing `dask_lxplus-0.3.1/setup.cfg` & `dask_lxplus-0.3.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dask_lxplus
-version = 0.3.1
+version = 0.3.2
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.txt
 author = Ben Jones
 author_email = b.jones@cern.ch
 url = https://github.com/cernops/dask-lxplus
 classifiers = 
@@ -24,15 +24,14 @@
 	dask_lxplus
 install_requires = 
 	click>=7.0
 	click-didyoumean
 	cryptography
 	dask
 	dask-jobqueue>=0.8.1
-	htcondor>=8.9.8
 	humanize
 	psutil
 	pyyaml
 	watchdog
 	importlib-metadata>=1.0;python_version < "3.9"
 python_requires = >=3.6
 include_package_data = True
```

### Comparing `dask_lxplus-0.3.1/tests/test_cluster.py` & `dask_lxplus-0.3.2/tests/test_cluster.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import os
 import unittest
+from pyfakefs.fake_filesystem_unittest import TestCase
 from unittest.mock import patch
 from dask_lxplus.cluster import check_job_script_prologue
 from dask_lxplus.cluster import get_xroot_url
 from dask_lxplus import CernCluster
 
 
-class TestCluster(unittest.TestCase):
+class TestCluster(TestCase):
+
+    def setUp(self):
+        self.setUpPyfakefs()
 
     def test_job_script_prologue(self):
         job_script_prologue = ["export PYTHONHOME=/usr/local/bin/python", 'export LD_LIBRARY_PATH="/usr/local/lib"']
         self.assertFalse(check_job_script_prologue("PATH", []))
         self.assertTrue(check_job_script_prologue("PYTHONHOME", job_script_prologue))
         self.assertTrue(check_job_script_prologue("LD_LIBRARY_PATH", job_script_prologue))
         self.assertFalse(check_job_script_prologue("PATH", job_script_prologue))
@@ -80,10 +84,31 @@
                 env_extra=["FOO=BAR, PATH=/one/two/three:/four/five/six"],
         ) as cluster:
             job_script = cluster.job_script()
             self.assertIn('FOO=BAR', job_script)
             self.assertIn('PATH=/one/two/three:/four/five/six', job_script)
             self.assertIn('getenv = true', job_script)
 
+    def test_job_script_outputdest(self):
+        with CernCluster(
+            cores=4,
+            processes=4,
+            memory="2000MB",
+            disk="1000MB",
+            log_directory="/eos/user/e/etejedor/dasklogs/"
+        ) as cluster:
+            job_script = cluster.job_script()
+            self.assertIn("output_destination = root://eosuser.cern.ch//eos/user/e/etejedor/dasklogs/", job_script)
+
+    def test_job_script_nooutputdest(self):
+        with CernCluster(
+            cores=4,
+            processes=4,
+            memory="2000MB",
+            disk="1000MB",
+        ) as cluster:
+            job_script = cluster.job_script()
+            self.assertNotIn("output_destination", job_script)
+
 
 if __name__ == '__main__':
     unittest.main()
```

