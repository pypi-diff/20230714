# Comparing `tmp/jianglab-0.5.8.tar.gz` & `tmp/jianglab-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.8.tar", last modified: Fri Jul 14 16:34:29 2023, max compression
+gzip compressed data, was "jianglab-0.5.9.tar", last modified: Fri Jul 14 16:37:46 2023, max compression
```

## Comparing `jianglab-0.5.8.tar` & `jianglab-0.5.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:34:29.482847 jianglab-0.5.8/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:34:29.482514 jianglab-0.5.8/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.5.8/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:34:29.479443 jianglab-0.5.8/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.8/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    34599 2023-07-14 16:34:12.000000 jianglab-0.5.8/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.8/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:34:29.481966 jianglab-0.5.8/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-14 16:34:29.000000 jianglab-0.5.8/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-14 16:34:29.482980 jianglab-0.5.8/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-14 16:34:19.000000 jianglab-0.5.8/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:37:46.153680 jianglab-0.5.9/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:37:46.153367 jianglab-0.5.9/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.5.9/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:37:46.150539 jianglab-0.5.9/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.9/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    34610 2023-07-14 16:37:31.000000 jianglab-0.5.9/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.9/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:37:46.152669 jianglab-0.5.9/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:37:46.000000 jianglab-0.5.9/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-14 16:37:46.000000 jianglab-0.5.9/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-14 16:37:46.000000 jianglab-0.5.9/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-14 16:37:46.000000 jianglab-0.5.9/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-14 16:37:46.000000 jianglab-0.5.9/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-14 16:37:46.153794 jianglab-0.5.9/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-14 16:37:38.000000 jianglab-0.5.9/setup.py
```

### Comparing `jianglab-0.5.8/PKG-INFO` & `jianglab-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.8
+Version: 0.5.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.8/README.md` & `jianglab-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.5.8/jianglab/common_functions.py` & `jianglab-0.5.9/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,20 +794,20 @@
             plt.xlim((0,2))
             #plt.ylim((0,0.01))
             plt.show()
 
         return xf_diff, yf_plot
 
 
-    def batch_ERG_fft_as_npy(file_name_list):
+    def batch_ERG_fft_as_npy(self, file_name_list):
         for file_name in file_name_list:
             data = pd.read_csv(file_name, sep = ",", header = 9)
             data = data.to_numpy()
             print(file_name)
-            xf, yf_plot, yf_plot2 = plot_individual(data, full_view = False, view_20hz = True, view_2hz = False)
+            xf, yf_plot, yf_plot2 = self.plot_individual(data, full_view = False, view_20hz = True, view_2hz = False)
 
             freq_data = np.array([xf, yf_plot, yf_plot2])
             np.save(file_name[:-4]+"_freq.npy", freq_data)
 
     def plot_batch_ERG_freq(file_name_list):
         all_freq_data = []
         for file_name in file_name_list:
```

### Comparing `jianglab-0.5.8/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.9/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.8
+Version: 0.5.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.8/setup.py` & `jianglab-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.8',
+    version='0.5.9',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

