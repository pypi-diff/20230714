# Comparing `tmp/nvidia-smi2-0.0.1.post2.tar.gz` & `tmp/nvidia-smi2-0.0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-smi2-0.0.1.post2.tar", last modified: Thu Jul 13 10:31:24 2023, max compression
+gzip compressed data, was "nvidia-smi2-0.0.1.post3.tar", last modified: Fri Jul 14 08:54:14 2023, max compression
```

## Comparing `nvidia-smi2-0.0.1.post2.tar` & `nvidia-smi2-0.0.1.post3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 10:31:24.900681 nvidia-smi2-0.0.1.post2/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       61 2023-07-13 10:31:24.900681 nvidia-smi2-0.0.1.post2/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8992 2023-07-13 10:29:51.000000 nvidia-smi2-0.0.1.post2/README.md
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 10:31:24.900681 nvidia-smi2-0.0.1.post2/bin/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      112 2023-07-13 10:28:58.000000 nvidia-smi2-0.0.1.post2/bin/nvidia-smi2
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 10:31:24.900681 nvidia-smi2-0.0.1.post2/nvidia-smi2/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8442 2023-07-13 10:29:59.000000 nvidia-smi2-0.0.1.post2/nvidia-smi2/__init__.py
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      120 2023-07-13 10:28:41.000000 nvidia-smi2-0.0.1.post2/nvidia-smi2/__main__.py
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-13 10:31:24.900681 nvidia-smi2-0.0.1.post2/nvidia_smi2.egg-info/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       61 2023-07-13 10:31:24.000000 nvidia-smi2-0.0.1.post2/nvidia_smi2.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      256 2023-07-13 10:31:24.000000 nvidia-smi2-0.0.1.post2/nvidia_smi2.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-13 10:31:24.000000 nvidia-smi2-0.0.1.post2/nvidia_smi2.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-13 10:31:24.000000 nvidia-smi2-0.0.1.post2/nvidia_smi2.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       12 2023-07-13 10:31:24.000000 nvidia-smi2-0.0.1.post2/nvidia_smi2.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       38 2023-07-13 10:31:24.900681 nvidia-smi2-0.0.1.post2/setup.cfg
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      259 2023-07-13 10:30:49.000000 nvidia-smi2-0.0.1.post2/setup.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9117 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8992 2023-07-13 10:29:51.000000 nvidia-smi2-0.0.1.post3/README.md
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/bin/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      112 2023-07-13 10:28:58.000000 nvidia-smi2-0.0.1.post3/bin/nvidia-smi2
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/nvidia-smi2/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8442 2023-07-13 10:29:59.000000 nvidia-smi2-0.0.1.post3/nvidia-smi2/__init__.py
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      120 2023-07-13 10:28:41.000000 nvidia-smi2-0.0.1.post3/nvidia-smi2/__main__.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9117 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      256 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       12 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       38 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      470 2023-07-14 08:53:41.000000 nvidia-smi2-0.0.1.post3/setup.py
```

### Comparing `nvidia-smi2-0.0.1.post2/README.md` & `nvidia-smi2-0.0.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `nvidia-smi2-0.0.1.post2/nvidia-smi2/__init__.py` & `nvidia-smi2-0.0.1.post3/nvidia-smi2/__init__.py`

 * *Files identical despite different names*

