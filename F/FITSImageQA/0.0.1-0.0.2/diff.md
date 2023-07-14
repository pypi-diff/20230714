# Comparing `tmp/FITSImageQA-0.0.1.tar.gz` & `tmp/FITSImageQA-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FITSImageQA-0.0.1.tar", last modified: Fri Jul 14 13:08:35 2023, max compression
+gzip compressed data, was "FITSImageQA-0.0.2.tar", last modified: Fri Jul 14 13:26:25 2023, max compression
```

## Comparing `FITSImageQA-0.0.1.tar` & `FITSImageQA-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:08:35.471078 FITSImageQA-0.0.1/
--rw-r--r--   0 will       (501) staff       (20)        0 2023-07-12 15:29:39.000000 FITSImageQA-0.0.1/LICENSE.md
--rw-r--r--   0 will       (501) staff       (20)       45 2023-07-12 15:29:39.000000 FITSImageQA-0.0.1/MANIFEST.in
--rw-r--r--   0 will       (501) staff       (20)      939 2023-07-14 13:08:35.470900 FITSImageQA-0.0.1/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)      386 2023-07-14 13:06:21.000000 FITSImageQA-0.0.1/README.md
--rw-r--r--   0 will       (501) staff       (20)       38 2023-07-14 13:08:35.471126 FITSImageQA-0.0.1/setup.cfg
--rw-r--r--   0 will       (501) staff       (20)     1381 2023-07-14 13:06:21.000000 FITSImageQA-0.0.1/setup.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:08:35.468215 FITSImageQA-0.0.1/src/
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:08:35.469289 FITSImageQA-0.0.1/src/FITSImageQA/
--rw-r--r--   0 will       (501) staff       (20)      207 2023-07-14 13:06:21.000000 FITSImageQA-0.0.1/src/FITSImageQA/__init__.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:08:35.470569 FITSImageQA-0.0.1/src/FITSImageQA/detection/
--rw-r--r--   0 will       (501) staff       (20)       64 2023-07-14 13:06:21.000000 FITSImageQA-0.0.1/src/FITSImageQA/detection/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     6786 2023-07-14 13:06:21.000000 FITSImageQA-0.0.1/src/FITSImageQA/detection/detection.py
--rw-r--r--   0 will       (501) staff       (20)    11263 2023-07-11 22:05:56.000000 FITSImageQA-0.0.1/src/FITSImageQA/detection/detection_mrf.py
--rw-r--r--   0 will       (501) staff       (20)    14674 2023-07-14 13:06:21.000000 FITSImageQA-0.0.1/src/FITSImageQA/imageqa.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:08:35.469988 FITSImageQA-0.0.1/src/FITSImageQA.egg-info/
--rw-r--r--   0 will       (501) staff       (20)      939 2023-07-14 13:08:35.000000 FITSImageQA-0.0.1/src/FITSImageQA.egg-info/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)      372 2023-07-14 13:08:35.000000 FITSImageQA-0.0.1/src/FITSImageQA.egg-info/SOURCES.txt
--rw-r--r--   0 will       (501) staff       (20)        1 2023-07-14 13:08:35.000000 FITSImageQA-0.0.1/src/FITSImageQA.egg-info/dependency_links.txt
--rw-r--r--   0 will       (501) staff       (20)       12 2023-07-14 13:08:35.000000 FITSImageQA-0.0.1/src/FITSImageQA.egg-info/top_level.txt
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:26:25.422190 FITSImageQA-0.0.2/
+-rw-r--r--   0 will       (501) staff       (20)        0 2023-07-12 15:29:39.000000 FITSImageQA-0.0.2/LICENSE.md
+-rw-r--r--   0 will       (501) staff       (20)       45 2023-07-12 15:29:39.000000 FITSImageQA-0.0.2/MANIFEST.in
+-rw-r--r--   0 will       (501) staff       (20)      939 2023-07-14 13:26:25.422028 FITSImageQA-0.0.2/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      386 2023-07-14 13:06:21.000000 FITSImageQA-0.0.2/README.md
+-rw-r--r--   0 will       (501) staff       (20)       38 2023-07-14 13:26:25.422244 FITSImageQA-0.0.2/setup.cfg
+-rw-r--r--   0 will       (501) staff       (20)     1381 2023-07-14 13:25:12.000000 FITSImageQA-0.0.2/setup.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:26:25.419194 FITSImageQA-0.0.2/src/
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:26:25.420243 FITSImageQA-0.0.2/src/FITSImageQA/
+-rw-r--r--   0 will       (501) staff       (20)      207 2023-07-14 13:25:31.000000 FITSImageQA-0.0.2/src/FITSImageQA/__init__.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:26:25.421684 FITSImageQA-0.0.2/src/FITSImageQA/detection/
+-rw-r--r--   0 will       (501) staff       (20)       64 2023-07-14 13:06:21.000000 FITSImageQA-0.0.2/src/FITSImageQA/detection/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     6786 2023-07-14 13:06:21.000000 FITSImageQA-0.0.2/src/FITSImageQA/detection/detection.py
+-rw-r--r--   0 will       (501) staff       (20)    11263 2023-07-11 22:05:56.000000 FITSImageQA-0.0.2/src/FITSImageQA/detection/detection_mrf.py
+-rw-r--r--   0 will       (501) staff       (20)    14675 2023-07-14 13:23:20.000000 FITSImageQA-0.0.2/src/FITSImageQA/imageqa.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-14 13:26:25.420931 FITSImageQA-0.0.2/src/FITSImageQA.egg-info/
+-rw-r--r--   0 will       (501) staff       (20)      939 2023-07-14 13:26:25.000000 FITSImageQA-0.0.2/src/FITSImageQA.egg-info/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      372 2023-07-14 13:26:25.000000 FITSImageQA-0.0.2/src/FITSImageQA.egg-info/SOURCES.txt
+-rw-r--r--   0 will       (501) staff       (20)        1 2023-07-14 13:26:25.000000 FITSImageQA-0.0.2/src/FITSImageQA.egg-info/dependency_links.txt
+-rw-r--r--   0 will       (501) staff       (20)       12 2023-07-14 13:26:25.000000 FITSImageQA-0.0.2/src/FITSImageQA.egg-info/top_level.txt
```

### Comparing `FITSImageQA-0.0.1/setup.py` & `FITSImageQA-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = open("README.md").read()
 
 setup(
     name = "FITSImageQA", 
     description = "Perform quality checks on FITS images",
     long_description = long_description, 
     long_description_content_type = "text/markdown",
-    version = "0.0.1",  # TODO: how to reconcile version set here vs in the `__init__.py` file
+    version = "0.0.2",  # TODO: how to reconcile version set here vs in the `__init__.py` file
     license = "MIT",  # TODO: confirm correct 
     #author = 
     #author_email = 
     url = "https://github.com/wpb-astro/FITSImageQA",
     #include_package_data = True, # looks in MANIFEST.in
     #packages = ["src/FITSImageQA", "src/FITSImageQA/detection"], #find_packages(where="src/FITSImageQA"),
     packages = find_packages(where="src"),  #/FITSImageQA")
```

### Comparing `FITSImageQA-0.0.1/src/FITSImageQA/detection/detection.py` & `FITSImageQA-0.0.2/src/FITSImageQA/detection/detection.py`

 * *Files identical despite different names*

### Comparing `FITSImageQA-0.0.1/src/FITSImageQA/detection/detection_mrf.py` & `FITSImageQA-0.0.2/src/FITSImageQA/detection/detection_mrf.py`

 * *Files identical despite different names*

### Comparing `FITSImageQA-0.0.1/src/FITSImageQA/imageqa.py` & `FITSImageQA-0.0.2/src/FITSImageQA/imageqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         """
         super().__init__()
         # parse the header, depending on what is passed
         if isinstance(filename_or_hdr, str):
             hdr = fits.getheader(filename_or_hdr)
         elif isinstance(filename_or_hdr, fits.hdu.hdulist.HDUList):
             hdr = filename_or_hdr[0].header
-        elif isinstance(filename_or_hdr, fits.header.Header)
+        elif isinstance(filename_or_hdr, fits.header.Header):
             hdr = filename_or_hdr
         else:
             raise TypeError("filename_or_hdr is not the correct type.")
         self.hdr = hdr
         self.header_fields = set(self.hdr.keys())
         try:
             self.expected_fields = set(expected_fields)
```

