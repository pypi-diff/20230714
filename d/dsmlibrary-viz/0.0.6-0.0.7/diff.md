# Comparing `tmp/dsmlibrary_viz-0.0.6.tar.gz` & `tmp/dsmlibrary_viz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary_viz-0.0.6.tar", last modified: Fri Jul 14 06:15:37 2023, max compression
+gzip compressed data, was "dsmlibrary_viz-0.0.7.tar", last modified: Fri Jul 14 06:23:30 2023, max compression
```

## Comparing `dsmlibrary_viz-0.0.6.tar` & `dsmlibrary_viz-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.371340 dsmlibrary_viz-0.0.6/
--rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.6/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:15:37.370991 dsmlibrary_viz-0.0.6/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      368 2023-07-14 05:57:14.000000 dsmlibrary_viz-0.0.6/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.364927 dsmlibrary_viz-0.0.6/dsmlibrary_viz/
--rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-14 06:15:29.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/base.py
--rw-r--r--   0 naii       (501) staff       (20)     2221 2023-07-13 09:19:09.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/data_viz.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.369968 dsmlibrary_viz-0.0.6/dsmlibrary_viz/scripts/
--rw-r--r--   0 naii       (501) staff       (20)       25 2023-07-14 06:11:01.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/scripts/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      133 2023-07-14 06:13:28.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/scripts/install_ext.py
--rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/utils.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.367986 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      389 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       39 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-14 06:15:37.371480 dsmlibrary_viz-0.0.6/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1497 2023-07-14 06:14:33.000000 dsmlibrary_viz-0.0.6/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.476266 dsmlibrary_viz-0.0.7/
+-rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.7/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:23:30.475580 dsmlibrary_viz-0.0.7/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      368 2023-07-14 05:57:14.000000 dsmlibrary_viz-0.0.7/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.468950 dsmlibrary_viz-0.0.7/dsmlibrary_viz/
+-rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-14 06:23:22.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     2221 2023-07-13 09:19:09.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/data_viz.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.474403 dsmlibrary_viz-0.0.7/dsmlibrary_viz/scripts/
+-rw-r--r--   0 naii       (501) staff       (20)       25 2023-07-14 06:11:01.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/scripts/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      122 2023-07-14 06:21:45.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/scripts/install_ext.py
+-rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz/utils.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:23:30.472397 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      389 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       39 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-14 06:23:30.000000 dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-14 06:23:30.476477 dsmlibrary_viz-0.0.7/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     2005 2023-07-14 06:22:36.000000 dsmlibrary_viz-0.0.7/setup.py
```

### Comparing `dsmlibrary_viz-0.0.6/LICENSE` & `dsmlibrary_viz-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.6/PKG-INFO` & `dsmlibrary_viz-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary_viz
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.6/dsmlibrary_viz/base.py` & `dsmlibrary_viz-0.0.7/dsmlibrary_viz/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.6/dsmlibrary_viz/data_viz.py` & `dsmlibrary_viz-0.0.7/dsmlibrary_viz/data_viz.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.6/dsmlibrary_viz/utils.py` & `dsmlibrary_viz-0.0.7/dsmlibrary_viz/utils.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/PKG-INFO` & `dsmlibrary_viz-0.0.7/dsmlibrary_viz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary-viz
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.6/setup.py` & `dsmlibrary_viz-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,30 @@
     
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
+from setuptools.command.develop import develop
+from setuptools.command.install import install
+
+
+class PostDevelopCommand(develop):
+    """Post-installation for development mode."""
+    def run(self):
+        develop.run(self)
+        scripts.install_ext.install_ext()
+
+class PostInstallCommand(install):
+    """Post-installation for installation mode."""
+    def run(self):
+        install.run(self)
+        scripts.install_ext.install_ext()
+
 setup(
     name='dsmlibrary_viz',
     version=get_version(),
     url='https://github.com/storemesh/dsmlibrary-viz',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
@@ -40,11 +56,13 @@
     ],
     install_requires=[
         'requests',
         's3fs',
         'duckdb',
         'pandas',
         'matplotlib'
-    ]
-)
-
-scripts.install_ext.install_ext()
+    ],
+    cmdclass={
+        'develop': PostDevelopCommand,
+        'install': PostInstallCommand,
+    }
+)
```

