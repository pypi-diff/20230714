# Comparing `tmp/whoi_uwapm-0.0.1.tar.gz` & `tmp/whoi_uwapm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoi_uwapm-0.0.1.tar", last modified: Tue Jul 11 22:19:40 2023, max compression
+gzip compressed data, was "whoi_uwapm-0.0.2.tar", last modified: Thu Jul 13 22:32:39 2023, max compression
```

## Comparing `whoi_uwapm-0.0.1.tar` & `whoi_uwapm-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:19:40.372479 whoi_uwapm-0.0.1/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1496 2023-07-11 18:26:07.000000 whoi_uwapm-0.0.1/LICENSE
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       16 2023-07-11 18:26:07.000000 whoi_uwapm-0.0.1/MANIFEST.in
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      476 2023-07-11 22:19:40.372479 whoi_uwapm-0.0.1/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      234 2023-07-11 22:18:48.000000 whoi_uwapm-0.0.1/README.md
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-11 22:19:40.372479 whoi_uwapm-0.0.1/setup.cfg
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      468 2023-07-11 22:15:12.000000 whoi_uwapm-0.0.1/setup.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:19:40.372479 whoi_uwapm-0.0.1/whoi_uwapm/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      512 2023-07-11 18:26:07.000000 whoi_uwapm-0.0.1/whoi_uwapm/__init__.py
--rw-rw-r--   0 brennan   (1000) brennan   (1000)    24808 2023-07-11 18:27:09.000000 whoi_uwapm-0.0.1/whoi_uwapm/uwapm.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:19:40.372479 whoi_uwapm-0.0.1/whoi_uwapm.egg-info/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      476 2023-07-11 22:19:40.000000 whoi_uwapm-0.0.1/whoi_uwapm.egg-info/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      250 2023-07-11 22:19:40.000000 whoi_uwapm-0.0.1/whoi_uwapm.egg-info/SOURCES.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-11 22:19:40.000000 whoi_uwapm-0.0.1/whoi_uwapm.egg-info/dependency_links.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       25 2023-07-11 22:19:40.000000 whoi_uwapm-0.0.1/whoi_uwapm.egg-info/requires.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       11 2023-07-11 22:19:40.000000 whoi_uwapm-0.0.1/whoi_uwapm.egg-info/top_level.txt
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-13 22:32:39.675042 whoi_uwapm-0.0.2/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1496 2023-07-11 18:26:07.000000 whoi_uwapm-0.0.2/LICENSE
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       16 2023-07-13 21:01:53.000000 whoi_uwapm-0.0.2/MANIFEST.in
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1830 2023-07-13 22:32:39.675042 whoi_uwapm-0.0.2/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1579 2023-07-13 21:31:09.000000 whoi_uwapm-0.0.2/README.md
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-13 22:32:39.675042 whoi_uwapm-0.0.2/setup.cfg
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      518 2023-07-13 22:32:11.000000 whoi_uwapm-0.0.2/setup.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-13 22:32:39.675042 whoi_uwapm-0.0.2/whoi_uwapm/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-13 21:08:51.000000 whoi_uwapm-0.0.2/whoi_uwapm/__init__.py
+-rwxrwxr-x   0 brennan   (1000) brennan   (1000)  5740896 2023-07-13 21:26:48.000000 whoi_uwapm-0.0.2/whoi_uwapm/bellhopcxx
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)    24905 2023-07-13 21:20:43.000000 whoi_uwapm-0.0.2/whoi_uwapm/uwapm.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-13 22:32:39.675042 whoi_uwapm-0.0.2/whoi_uwapm.egg-info/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1830 2023-07-13 22:32:39.000000 whoi_uwapm-0.0.2/whoi_uwapm.egg-info/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      272 2023-07-13 22:32:39.000000 whoi_uwapm-0.0.2/whoi_uwapm.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-13 22:32:39.000000 whoi_uwapm-0.0.2/whoi_uwapm.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       25 2023-07-13 22:32:39.000000 whoi_uwapm-0.0.2/whoi_uwapm.egg-info/requires.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       11 2023-07-13 22:32:39.000000 whoi_uwapm-0.0.2/whoi_uwapm.egg-info/top_level.txt
```

### Comparing `whoi_uwapm-0.0.1/LICENSE` & `whoi_uwapm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whoi_uwapm-0.0.1/whoi_uwapm/uwapm.py` & `whoi_uwapm-0.0.2/whoi_uwapm/uwapm.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,16 +335,17 @@
             self._unlink(fname_base+'.log')
             self._unlink(fname_base+'.arr')
             self._unlink(fname_base+'.ray')
             self._unlink(fname_base+'.shd')
         return results
 
     def _bellhop(self, *args):
-        try:
-            _proc.run(f'bellhop.exe {" ".join(list(args))}', 
+        try: 
+            bellhop_file_path = _os.path.join(_os.path.dirname(__file__), 'bellhopcxx')
+            _proc.run(f'{bellhop_file_path} {" ".join(list(args))}', 
                       stderr=_proc.STDOUT, stdout=_proc.PIPE,
                       shell=True)
         except OSError:
             return False
         return True
 
     def _unlink(self, f):
```

