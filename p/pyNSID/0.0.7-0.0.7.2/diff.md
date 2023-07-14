# Comparing `tmp/pyNSID-0.0.7.tar.gz` & `tmp/pyNSID-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNSID-0.0.7.tar", last modified: Sat Jan  7 00:09:44 2023, max compression
+gzip compressed data, was "pyNSID-0.0.7.2.tar", last modified: Fri Jul 14 15:34:49 2023, max compression
```

## Comparing `pyNSID-0.0.7.tar` & `pyNSID-0.0.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 00:09:44.647874 pyNSID-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-07 00:08:30.000000 pyNSID-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-07 00:09:44.647874 pyNSID-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-01-07 00:08:30.000000 pyNSID-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 00:09:44.643874 pyNSID-0.0.7/pyNSID/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-07 00:08:30.000000 pyNSID-0.0.7/pyNSID/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-07 00:08:30.000000 pyNSID-0.0.7/pyNSID/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 00:09:44.647874 pyNSID-0.0.7/pyNSID/io/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-07 00:08:30.000000 pyNSID-0.0.7/pyNSID/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-01-07 00:08:30.000000 pyNSID-0.0.7/pyNSID/io/hdf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-01-07 00:08:30.000000 pyNSID-0.0.7/pyNSID/io/hdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 00:09:44.647874 pyNSID-0.0.7/pyNSID.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-07 00:09:44.000000 pyNSID-0.0.7/pyNSID.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-01-07 00:09:44.000000 pyNSID-0.0.7/pyNSID.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 00:09:44.000000 pyNSID-0.0.7/pyNSID.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-07 00:09:44.000000 pyNSID-0.0.7/pyNSID.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-07 00:09:44.000000 pyNSID-0.0.7/pyNSID.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-07 00:09:44.647874 pyNSID-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-01-07 00:08:30.000000 pyNSID-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:34:49.722550 pyNSID-0.0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-14 15:34:49.722550 pyNSID-0.0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:34:49.718550 pyNSID-0.0.7.2/pyNSID/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/pyNSID/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/pyNSID/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:34:49.722550 pyNSID-0.0.7.2/pyNSID/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/pyNSID/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/pyNSID/io/hdf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20321 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/pyNSID/io/hdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:34:49.722550 pyNSID-0.0.7.2/pyNSID.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-14 15:34:49.000000 pyNSID-0.0.7.2/pyNSID.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-14 15:34:49.000000 pyNSID-0.0.7.2/pyNSID.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:34:49.000000 pyNSID-0.0.7.2/pyNSID.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 15:34:49.000000 pyNSID-0.0.7.2/pyNSID.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 15:34:49.000000 pyNSID-0.0.7.2/pyNSID.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 15:34:49.722550 pyNSID-0.0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-14 15:33:26.000000 pyNSID-0.0.7.2/setup.py
```

### Comparing `pyNSID-0.0.7/LICENSE` & `pyNSID-0.0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyNSID-0.0.7/PKG-INFO` & `pyNSID-0.0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNSID
-Version: 0.0.7
+Version: 0.0.7.2
 Summary: Framework for storing, visualizing, and processing N-Dimensional Spectroscopic and Imaging Data (NSID)
 Home-page: https://pycroscopy.github.io/pyUSID/about.html
 Author: G. Duscher, S. Somnath, and contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: imaging,spectra,multidimensional,data format,universal,hdf5
```

### Comparing `pyNSID-0.0.7/README.rst` & `pyNSID-0.0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyNSID-0.0.7/pyNSID/io/hdf_io.py` & `pyNSID-0.0.7.2/pyNSID/io/hdf_io.py`

 * *Files identical despite different names*

### Comparing `pyNSID-0.0.7/pyNSID/io/hdf_utils.py` & `pyNSID-0.0.7.2/pyNSID/io/hdf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,20 @@
     if not isinstance(dset, h5py.Dataset):
         raise TypeError('can only read single Dataset, use read_all_in_group or read_all function instead')
 
     if not check_if_main(dset):
         raise TypeError('can only read NSID datasets, not general one, try to import with from_array')
 
     # create vanilla dask array
-    data_array = np.empty(dset.shape)
+    #find out if data is complex or not
+    if 'complex' in str(dset.dtype): 
+        data_array = np.empty(dset.shape, dtype = 'complex64')
+    else:
+        data_array = np.empty(dset.shape, dtype = 'float')
+
     dset.read_direct(data_array)
     dataset = Dataset.from_array(data_array)
 
     if 'title' in dset.attrs:
         dataset.title = dset.attrs['title']
     else:
         dataset.title = dset.name
```

### Comparing `pyNSID-0.0.7/pyNSID.egg-info/PKG-INFO` & `pyNSID-0.0.7.2/pyNSID.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNSID
-Version: 0.0.7
+Version: 0.0.7.2
 Summary: Framework for storing, visualizing, and processing N-Dimensional Spectroscopic and Imaging Data (NSID)
 Home-page: https://pycroscopy.github.io/pyUSID/about.html
 Author: G. Duscher, S. Somnath, and contributors
 Author-email: pycroscopy@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: imaging,spectra,multidimensional,data format,universal,hdf5
```

### Comparing `pyNSID-0.0.7/setup.py` & `pyNSID-0.0.7.2/setup.py`

 * *Files identical despite different names*

