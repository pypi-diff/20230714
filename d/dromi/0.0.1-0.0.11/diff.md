# Comparing `tmp/dromi-0.0.1.tar.gz` & `tmp/dromi-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dromi-0.0.1.tar", last modified: Sat Jun 17 14:32:00 2023, max compression
+gzip compressed data, was "dromi-0.0.11.tar", last modified: Fri Jul 14 16:28:24 2023, max compression
```

## Comparing `dromi-0.0.1.tar` & `dromi-0.0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-17 14:32:00.365440 dromi-0.0.1/
--rw-rw-r--   0 lys       (1000) lys       (1000)     6556 2022-12-08 13:40:45.000000 dromi-0.0.1/LICENSE.md
--rw-rw-r--   0 lys       (1000) lys       (1000)      644 2023-06-17 14:32:00.365440 dromi-0.0.1/PKG-INFO
--rw-rw-r--   0 lys       (1000) lys       (1000)        8 2023-06-17 14:13:17.000000 dromi-0.0.1/README.md
--rw-rw-r--   0 lys       (1000) lys       (1000)      617 2023-06-17 14:32:00.369440 dromi-0.0.1/setup.cfg
--rw-rw-r--   0 lys       (1000) lys       (1000)     2518 2023-06-17 14:21:39.000000 dromi-0.0.1/setup.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-17 14:32:00.365440 dromi-0.0.1/src/
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-17 14:32:00.365440 dromi-0.0.1/src/dromi/
--rw-rw-r--   0 lys       (1000) lys       (1000)        0 2023-06-17 14:17:25.000000 dromi-0.0.1/src/dromi/__init__.py
--rw-rw-r--   0 lys       (1000) lys       (1000)        0 2023-06-17 14:28:11.000000 dromi-0.0.1/src/dromi/encoding.py
--rw-rw-r--   0 lys       (1000) lys       (1000)        0 2023-06-17 14:17:56.000000 dromi-0.0.1/src/dromi/similarities.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-06-17 14:32:00.365440 dromi-0.0.1/src/dromi.egg-info/
--rw-rw-r--   0 lys       (1000) lys       (1000)      644 2023-06-17 14:32:00.000000 dromi-0.0.1/src/dromi.egg-info/PKG-INFO
--rw-rw-r--   0 lys       (1000) lys       (1000)      305 2023-06-17 14:32:00.000000 dromi-0.0.1/src/dromi.egg-info/SOURCES.txt
--rw-rw-r--   0 lys       (1000) lys       (1000)        1 2023-06-17 14:32:00.000000 dromi-0.0.1/src/dromi.egg-info/dependency_links.txt
--rw-rw-r--   0 lys       (1000) lys       (1000)        1 2023-06-17 14:32:00.000000 dromi-0.0.1/src/dromi.egg-info/not-zip-safe
--rw-rw-r--   0 lys       (1000) lys       (1000)      104 2023-06-17 14:32:00.000000 dromi-0.0.1/src/dromi.egg-info/requires.txt
--rw-rw-r--   0 lys       (1000) lys       (1000)        6 2023-06-17 14:32:00.000000 dromi-0.0.1/src/dromi.egg-info/top_level.txt
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-07-14 16:28:24.840861 dromi-0.0.11/
+-rw-rw-r--   0 lys       (1000) lys       (1000)     6556 2022-12-08 13:40:45.000000 dromi-0.0.11/LICENSE.md
+-rw-rw-r--   0 lys       (1000) lys       (1000)     1112 2023-07-14 16:28:24.840861 dromi-0.0.11/PKG-INFO
+-rw-rw-r--   0 lys       (1000) lys       (1000)      474 2023-07-14 16:26:54.000000 dromi-0.0.11/README.md
+-rw-rw-r--   0 lys       (1000) lys       (1000)      618 2023-07-14 16:28:24.840861 dromi-0.0.11/setup.cfg
+-rw-rw-r--   0 lys       (1000) lys       (1000)     2519 2023-07-14 16:24:29.000000 dromi-0.0.11/setup.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-07-14 16:28:24.840861 dromi-0.0.11/src/
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-07-14 16:28:24.840861 dromi-0.0.11/src/dromi/
+-rw-rw-r--   0 lys       (1000) lys       (1000)       48 2023-06-19 08:19:55.000000 dromi-0.0.11/src/dromi/__init__.py
+-rw-rw-r--   0 lys       (1000) lys       (1000)    38032 2023-06-24 17:54:47.000000 dromi-0.0.11/src/dromi/similarities.py
+-rw-rw-r--   0 lys       (1000) lys       (1000)    19288 2023-06-28 19:48:42.000000 dromi-0.0.11/src/dromi/utils.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2023-07-14 16:28:24.840861 dromi-0.0.11/src/dromi.egg-info/
+-rw-rw-r--   0 lys       (1000) lys       (1000)     1112 2023-07-14 16:28:24.000000 dromi-0.0.11/src/dromi.egg-info/PKG-INFO
+-rw-rw-r--   0 lys       (1000) lys       (1000)      302 2023-07-14 16:28:24.000000 dromi-0.0.11/src/dromi.egg-info/SOURCES.txt
+-rw-rw-r--   0 lys       (1000) lys       (1000)        1 2023-07-14 16:28:24.000000 dromi-0.0.11/src/dromi.egg-info/dependency_links.txt
+-rw-rw-r--   0 lys       (1000) lys       (1000)        1 2023-06-17 14:32:00.000000 dromi-0.0.11/src/dromi.egg-info/not-zip-safe
+-rw-rw-r--   0 lys       (1000) lys       (1000)      104 2023-07-14 16:28:24.000000 dromi-0.0.11/src/dromi.egg-info/requires.txt
+-rw-rw-r--   0 lys       (1000) lys       (1000)        6 2023-07-14 16:28:24.000000 dromi-0.0.11/src/dromi.egg-info/top_level.txt
```

### Comparing `dromi-0.0.1/LICENSE.md` & `dromi-0.0.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dromi-0.0.1/setup.cfg` & `dromi-0.0.11/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dromi-artistworking43
-version = 0.0.1
+version = 0.0.11
 author = Lys Sanz Moreta
 author_email = lys.sanz.moreta@outlook.com
 description = Dromi
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LysSanzMoreta/Dromi
 project_urls =
```

### Comparing `dromi-0.0.1/setup.py` & `dromi-0.0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Get the long description from the TOREAD_gleipnir.md file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 setup(name='dromi',
-      version='0.0.1',
+      version='0.0.11',
       # list folders, not files
       packages=find_packages('src'),
       package_dir={'': 'src'},
       py_modules=[splitext(basename(path))[0] for path in glob('dromi/src/dromi/*.py')],
       #scripts=['bin/script1.py'],
       package_data={'dromi': ['data/*']},
       description= '',
```

