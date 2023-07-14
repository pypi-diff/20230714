# Comparing `tmp/jianglab-0.5.7.tar.gz` & `tmp/jianglab-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.7.tar", last modified: Fri Jul 14 16:27:30 2023, max compression
+gzip compressed data, was "jianglab-0.5.8.tar", last modified: Fri Jul 14 16:34:29 2023, max compression
```

## Comparing `jianglab-0.5.7.tar` & `jianglab-0.5.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:27:30.472697 jianglab-0.5.7/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:27:30.472361 jianglab-0.5.7/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.5.7/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:27:30.469186 jianglab-0.5.7/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.7/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    34599 2023-07-14 16:26:12.000000 jianglab-0.5.7/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.7/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:27:30.471837 jianglab-0.5.7/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-14 16:27:30.472842 jianglab-0.5.7/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-14 16:26:57.000000 jianglab-0.5.7/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:34:29.482847 jianglab-0.5.8/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:34:29.482514 jianglab-0.5.8/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.5.8/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:34:29.479443 jianglab-0.5.8/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.8/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    34599 2023-07-14 16:34:12.000000 jianglab-0.5.8/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.8/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:34:29.481966 jianglab-0.5.8/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-14 16:34:29.482980 jianglab-0.5.8/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-14 16:34:19.000000 jianglab-0.5.8/setup.py
```

### Comparing `jianglab-0.5.7/PKG-INFO` & `jianglab-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.7
+Version: 0.5.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.7/README.md` & `jianglab-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.5.7/jianglab/common_functions.py` & `jianglab-0.5.8/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -715,15 +715,15 @@
 
     anim = animation.FuncAnimation(fig, animate, init_func=init, frames=data.shape[0], repeat = True)
     if save_to_avi:
         anim.save(filename)
     return HTML(anim.to_jshtml())
 
 
-def human_erg():
+class human_erg:
     def plot_individual(data,
                     full_view = False,
                     view_20hz = True,  
                     view_2hz = False):
         y = data[:,1]
         y2= data[:,2]
         x = data[:,0]-data[0,0]
```

### Comparing `jianglab-0.5.7/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.8/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.7
+Version: 0.5.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.7/setup.py` & `jianglab-0.5.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.7',
+    version='0.5.8',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

