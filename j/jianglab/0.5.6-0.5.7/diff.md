# Comparing `tmp/jianglab-0.5.6.tar.gz` & `tmp/jianglab-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.6.tar", last modified: Wed Jul 12 19:27:23 2023, max compression
+gzip compressed data, was "jianglab-0.5.7.tar", last modified: Fri Jul 14 16:27:30 2023, max compression
```

## Comparing `jianglab-0.5.6.tar` & `jianglab-0.5.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-12 19:27:23.356721 jianglab-0.5.6/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-12 19:27:23.356193 jianglab-0.5.6/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1172 2023-07-12 19:22:38.000000 jianglab-0.5.6/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-12 19:27:23.352324 jianglab-0.5.6/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.6/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    30559 2023-07-12 19:27:19.000000 jianglab-0.5.6/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.6/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-12 19:27:23.355279 jianglab-0.5.6/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-12 19:27:23.000000 jianglab-0.5.6/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-12 19:27:23.357118 jianglab-0.5.6/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-12 19:27:11.000000 jianglab-0.5.6/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:27:30.472697 jianglab-0.5.7/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:27:30.472361 jianglab-0.5.7/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.5.7/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:27:30.469186 jianglab-0.5.7/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.7/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    34599 2023-07-14 16:26:12.000000 jianglab-0.5.7/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.7/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-14 16:27:30.471837 jianglab-0.5.7/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-14 16:27:30.000000 jianglab-0.5.7/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-14 16:27:30.472842 jianglab-0.5.7/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-14 16:26:57.000000 jianglab-0.5.7/setup.py
```

### Comparing `jianglab-0.5.6/PKG-INFO` & `jianglab-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.6
+Version: 0.5.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.6/README.md` & `jianglab-0.5.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 dist, build and *.egg-info should be in root when created
 
 
 1. Upload the new version:
 Now you can upload the new version of your package to PyPI using twine:
 
 ```bash
-twine upload dist/*
+twine upload dist/*1.7*
 
 ```
 Since the version number has been incremented, you should not encounter the "file already exists" error, and your package should be uploaded successfully. Users can now install the new version of your package using pip.
 
 
 
 To use video output.
```

### Comparing `jianglab-0.5.6/jianglab/common_functions.py` & `jianglab-0.5.7/jianglab/common_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import os
 from treelib import Tree, Node 
 import numpy as np
 import McsPy.McsCMOSMEA as McsCMOSMEA
 from tqdm import tqdm
+import scipy
 from scipy.signal import find_peaks
 import matplotlib.pyplot as plt
 import gspread
 import pandas as pd
 from oauth2client.service_account import ServiceAccountCredentials
 import scipy.signal as signal
 from tqdm import tqdm
 import pickle
 import cv2
 import xmltodict
 import matplotlib.animation as animation
 from IPython.display import HTML
 import matplotlib
+from scipy.fftpack import fft, fftfreq
+
+
 
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
@@ -708,8 +712,126 @@
         im0.set_data(data[i])
 
         return im0
 
     anim = animation.FuncAnimation(fig, animate, init_func=init, frames=data.shape[0], repeat = True)
     if save_to_avi:
         anim.save(filename)
-    return HTML(anim.to_jshtml())
+    return HTML(anim.to_jshtml())
+
+
+def human_erg():
+    def plot_individual(data,
+                    full_view = False,
+                    view_20hz = True,  
+                    view_2hz = False):
+        y = data[:,1]
+        y2= data[:,2]
+        x = data[:,0]-data[0,0]
+        N = data.shape[0]
+        T = 1.0/5000 # sampling rate
+        yf = fft(y)
+        yf2 = fft(y2)
+
+        yf_plot = 2.0/N * np.abs(yf[0:N//2])
+        yf_plot = scipy.signal.medfilt(yf_plot, kernel_size = 101)
+        yf_plot2 = 2.0/N * np.abs(yf2[0:N//2])
+        yf_plot2 = scipy.signal.medfilt(yf_plot2, kernel_size = 101)
+        xf = fftfreq(N, T)[:N//2]
+        
+        if full_view:
+            plt.plot(xf, yf_plot, c="red")
+            plt.plot(xf, yf_plot2)
+            plt.show()
+
+        if view_20hz: 
+            plt.plot(xf, yf_plot, c="red")
+            plt.plot(xf, yf_plot2)
+            plt.xlim((0,20))
+            #plt.ylim(0,100*yf_plot2.std())
+            plt.show()
+            plt.show()
+
+        if view_2hz:
+            plt.plot(xf, yf_plot, c="red")
+            plt.plot(xf, yf_plot2)
+            plt.xlim((0,2))
+            #plt.ylim((0,0.01))
+            plt.show()
+
+        return xf, yf_plot, yf_plot2
+
+    def plot_individual_subtraction(data,
+                                    sampling_rate = 5000,
+                                    full_view = False,
+                                    view_20hz = True,  
+                                    view_2hz = True):
+        y_diff = data[:,2]-data[:,1]
+        x_diff = data[:,0]-data[0,0]
+    
+        N_diff = data.shape[0]
+        
+        T = 1.0/sampling_rate # sampling rate
+        yf = fft(y_diff)
+        yf_plot = 2.0/N_diff * np.abs(yf[0:N_diff//2])
+        yf_plot = scipy.signal.medfilt(yf_plot, kernel_size = 101)
+        xf_diff = fftfreq(N_diff, T)[:N_diff//2]
+
+        if full_view:
+            plt.plot(xf_diff, yf_plot, c="red")
+            #plt.plot(xf_dark, yf_plot2)
+            plt.show()
+
+        if view_20hz: 
+            plt.plot(xf_diff, yf_plot, c="red")
+            #plt.plot(xf_dark, yf_plot2)
+            plt.xlim((0,20))
+            #plt.ylim(0,100*yf_plot2.std())
+            plt.show()
+
+        if view_2hz:
+            plt.plot(xf_diff, yf_plot, c="red")
+            #plt.plot(xf_dark, yf_plot2)
+            plt.xlim((0,2))
+            #plt.ylim((0,0.01))
+            plt.show()
+
+        return xf_diff, yf_plot
+
+
+    def batch_ERG_fft_as_npy(file_name_list):
+        for file_name in file_name_list:
+            data = pd.read_csv(file_name, sep = ",", header = 9)
+            data = data.to_numpy()
+            print(file_name)
+            xf, yf_plot, yf_plot2 = plot_individual(data, full_view = False, view_20hz = True, view_2hz = False)
+
+            freq_data = np.array([xf, yf_plot, yf_plot2])
+            np.save(file_name[:-4]+"_freq.npy", freq_data)
+
+    def plot_batch_ERG_freq(file_name_list):
+        all_freq_data = []
+        for file_name in file_name_list:
+            freq_data = np.load(file_name)
+            xf = freq_data[0,:]
+            yf_plot = freq_data[1,:]
+            yf_plot2 = freq_data[2,:]
+            all_freq_data.append(yf_plot)
+            all_freq_data.append(yf_plot2)
+            plt.plot(xf, yf_plot, alpha = 0.2)
+            plt.plot(xf, yf_plot2, alpha = 0.2)
+            plt.xlim((0,2)) # adjust the range of x axis
+        
+        return xf, all_freq_data
+    
+    def normalize_all_freq_data(freq_x_axis, all_freq_data, mode = "mean", range = [1.0, 2.0]):
+        all_norm_data = []
+        for freq_data in all_freq_data:
+            range_mask = (freq_x_axis>range[0]) & (freq_x_axis<[range[1]])
+            if mode == "mean":
+                norm_freq_data = freq_data/np.mean(freq_data[range_mask])
+            elif mode == "max":
+                norm_freq_data = freq_data/np.max(freq_data[range_mask])
+            else:
+                print("mode not recognized, use mean or max")
+            all_norm_data.append(norm_freq_data)
+        return all_norm_data
```

### Comparing `jianglab-0.5.6/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.7/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.6
+Version: 0.5.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.6/setup.py` & `jianglab-0.5.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.6',
+    version='0.5.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

