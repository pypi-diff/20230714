# Comparing `tmp/ML-Algo-1.2.7.tar.gz` & `tmp/ML-Algo-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.2.7.tar", last modified: Thu Jul 13 09:37:57 2023, max compression
+gzip compressed data, was "ML-Algo-1.2.8.tar", last modified: Fri Jul 14 05:31:55 2023, max compression
```

## Comparing `ML-Algo-1.2.7.tar` & `ML-Algo-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 09:37:57.032328 ML-Algo-1.2.7/
-drwxrwxrwx   0        0        0        0 2023-07-13 09:37:57.026329 ML-Algo-1.2.7/ML_Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.7/ML_Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     1629 2023-07-12 13:17:21.000000 ML-Algo-1.2.7/ML_Algo/FetchData.py
--rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.7/ML_Algo/Predictions.py
--rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.7/ML_Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.7/ML_Algo/Series_Time.py
--rw-rw-rw-   0        0        0     2186 2023-07-13 09:36:50.000000 ML-Algo-1.2.7/ML_Algo/TestRun.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.7/ML_Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:37:57.031331 ML-Algo-1.2.7/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0     2155 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2155 2023-07-13 09:37:57.032328 ML-Algo-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-13 09:37:57.032328 ML-Algo-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-07-13 09:37:06.000000 ML-Algo-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:31:55.976147 ML-Algo-1.2.8/
+drwxrwxrwx   0        0        0        0 2023-07-14 05:31:55.950105 ML-Algo-1.2.8/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.8/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     1909 2023-07-14 05:26:01.000000 ML-Algo-1.2.8/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.8/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.8/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.8/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0     2517 2023-07-13 11:01:26.000000 ML-Algo-1.2.8/ML_Algo/TestRun.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.8/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:31:55.970139 ML-Algo-1.2.8/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0     2198 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 05:31:55.000000 ML-Algo-1.2.8/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2198 2023-07-14 05:31:55.974136 ML-Algo-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:31:55.977141 ML-Algo-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-14 05:31:30.000000 ML-Algo-1.2.8/setup.py
```

### Comparing `ML-Algo-1.2.7/ML_Algo/DataCleaning.py` & `ML-Algo-1.2.8/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.7/ML_Algo/FetchData.py` & `ML-Algo-1.2.8/ML_Algo/FetchData.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,41 +15,51 @@
     
     except:
         print('server busy')
     dat = response.text
     dt = json.loads(dat)
     return dt
 
-def get_live_data(yesterday,today,interval=15):
-    t = calculate_completed_intervals(interval)
+def get_live_data(yesterday,today,interval=15,manual_override=0,ct=0):
+    if manual_override == 0:
+        t = calculate_completed_intervals(interval)
+    else:
+        t = ct
     if t == 0:
         live_data = pd.concat([yesterday.iloc[:, -2:], today.iloc[:, :1]], axis=1)
         return live_data
     elif t == 1:
         live_data = pd.concat([yesterday.iloc[:, -1:], today.iloc[:, :2]], axis=1)
         return live_data
     elif t == 2:
-        live_data = today[:3]
+        live_data = today.iloc[:,0:3]
         return live_data
     elif t >= 3:
         live_data = today.iloc[:,t-2:t+1]
         return live_data
     
-def get_pred_data(yesterday,pred_data,interval=15):
-    t = calculate_completed_intervals(interval)
+def get_pred_data(yesterday,pred_data,interval=15,manual_override=0,ct=0):
+    if manual_override == 0:
+        t = calculate_completed_intervals(interval)
+    else:
+        t = ct
+
     if t == 0:
         pred = pd.concat([yesterday.iloc[:, -2:], pred_data.iloc[:, :1]], axis=1)
         return pred
     elif t == 1:
         pred = pd.concat([yesterday.iloc[:, -1:], pred_data.iloc[:, :2]], axis=1)
         return pred
     elif t == 2:
         pred = pred_data.iloc[:,0:3]
         return pred
     elif t >= 3:
         pred = pred_data.iloc[:,t-2:t+1]
         return pred
     
-def get_next_pred(pred,next_pred_intervals=8):
-    t = calculate_completed_intervals(15)
+def get_next_pred(pred,next_pred_intervals=8,interval=15,manual_override=0,ct=0):
+    if manual_override == 0:
+        t = calculate_completed_intervals(interval)
+    else:
+        t = ct
     return pred.iloc[:,t:t+next_pred_intervals]
```

### Comparing `ML-Algo-1.2.7/ML_Algo/Predictions.py` & `ML-Algo-1.2.8/ML_Algo/Predictions.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.7/ML_Algo/Series_Data.py` & `ML-Algo-1.2.8/ML_Algo/Series_Data.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.7/ML_Algo/Series_Time.py` & `ML-Algo-1.2.8/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.7/ML_Algo/TestRun.py` & `ML-Algo-1.2.8/ML_Algo/TestRun.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from ML_Algo.FetchData import *
 from ML_Algo.Series_Data import *
 import numpy as np
 
 def get_test_live_data(yesterday,today,t=0):
     if t == 0:
         live_data = pd.concat([yesterday.iloc[:, -2:], today.iloc[:, :1]], axis=1)
+        # live_data = pd.concat([yesterday.iloc[:, :2], today.iloc[:, :1]], axis=1)
         return live_data.stack().dropna().tolist()
     elif t == 1:
         live_data = pd.concat([yesterday.iloc[:, -1:], today.iloc[:, :2]], axis=1)
+        # live_data = pd.concat([yesterday.iloc[:, :1], today.iloc[:, :2]], axis=1)
         return live_data.stack().dropna().tolist()
     elif t == 2:
         live_data = today.iloc[:,0:3]
         return live_data.stack().dropna().tolist()
     elif t >= 3:
         live_data = today.iloc[:,t-2:t+1]
         return live_data.stack().dropna().tolist()
     
 def get_test_pred_data(yesterday,pred_data,t=0):
     if t == 0:
+        # pred = pd.concat([yesterday.iloc[:, :2], pred_data.iloc[:, :1]], axis=1)
         pred = pd.concat([yesterday.iloc[:, -2:], pred_data.iloc[:, :1]], axis=1)
         return pred.stack().dropna().tolist()
     elif t == 1:
+        # pred = pd.concat([yesterday.iloc[:, :1], pred_data.iloc[:, :2]], axis=1)
         pred = pd.concat([yesterday.iloc[:, -1:], pred_data.iloc[:, :2]], axis=1)
         return pred.stack().dropna().tolist()
     elif t == 2:
         pred = pred_data.iloc[:,0:3]
         return pred.stack().dropna().tolist()
     elif t >= 3:
         pred = pred_data.iloc[:,t-2:t+1]
@@ -47,11 +51,10 @@
         prev_day_err = prev_day_err.mean()
         # print(prev_day_err)
         # print(n)
         output_values= []
         for i in n:
             corr = (i+(i*prev_day_err))
             output_values.append(corr)
-            
-        Complete_Day.append(output_values)
+        Complete_Day.append(output_values[:jump])
     return Complete_Day
```

### Comparing `ML-Algo-1.2.7/ML_Algo.egg-info/PKG-INFO` & `ML-Algo-1.2.8/ML_Algo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.2.7
+Version: 1.2.8
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,10 +47,12 @@
 
 Please ensure that you adhere to the code style and format used in the project.
 License
 
 ML-Algo is licensed under the MIT License. See the LICENSE file for more information.
 Contact
 
+`Changes Made as 14/07/2023 at 10:57am`
+
 If you have any questions, suggestions, or issues, please feel free to reach out to the project maintainer, Arunraj, at <a href="mailto:srvnn_arunraj@gmail.com." target="_new">srvnn_arunraj@gmail.com.</a>
 
 <a href="https://pypi.org/project/ml-algo/" target="_new"><img src="https://img.shields.io/pypi/v/ml-algo.svg" alt="PyPI Version"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.7 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.8 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
@@ -16,10 +16,11 @@
 welcome contributions from the community to enhance ML-Algo. If you want to
 contribute, please follow these guidelines: Fork the repository and clone it
 locally. Create a new branch for your feature or bug fix. Make your changes and
 ensure that the code passes all tests. Write tests for any new functionality
 you add. Commit your changes and push them to your fork. Submit a pull request,
 describing your changes in detail. Please ensure that you adhere to the code
 style and format used in the project. License ML-Algo is licensed under the MIT
-License. See the LICENSE file for more information. Contact If you have any
-questions, suggestions, or issues, please feel free to reach out to the project
-maintainer, Arunraj, at srvnn_arunraj@gmail.com. [PyPI_Version]
+License. See the LICENSE file for more information. Contact `Changes Made as
+14/07/2023 at 10:57am` If you have any questions, suggestions, or issues,
+please feel free to reach out to the project maintainer, Arunraj, at
+srvnn_arunraj@gmail.com. [PyPI_Version]
```

### Comparing `ML-Algo-1.2.7/PKG-INFO` & `ML-Algo-1.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.2.7
+Version: 1.2.8
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -47,10 +47,12 @@
 
 Please ensure that you adhere to the code style and format used in the project.
 License
 
 ML-Algo is licensed under the MIT License. See the LICENSE file for more information.
 Contact
 
+`Changes Made as 14/07/2023 at 10:57am`
+
 If you have any questions, suggestions, or issues, please feel free to reach out to the project maintainer, Arunraj, at <a href="mailto:srvnn_arunraj@gmail.com." target="_new">srvnn_arunraj@gmail.com.</a>
 
 <a href="https://pypi.org/project/ml-algo/" target="_new"><img src="https://img.shields.io/pypi/v/ml-algo.svg" alt="PyPI Version"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.7 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.8 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
@@ -16,10 +16,11 @@
 welcome contributions from the community to enhance ML-Algo. If you want to
 contribute, please follow these guidelines: Fork the repository and clone it
 locally. Create a new branch for your feature or bug fix. Make your changes and
 ensure that the code passes all tests. Write tests for any new functionality
 you add. Commit your changes and push them to your fork. Submit a pull request,
 describing your changes in detail. Please ensure that you adhere to the code
 style and format used in the project. License ML-Algo is licensed under the MIT
-License. See the LICENSE file for more information. Contact If you have any
-questions, suggestions, or issues, please feel free to reach out to the project
-maintainer, Arunraj, at srvnn_arunraj@gmail.com. [PyPI_Version]
+License. See the LICENSE file for more information. Contact `Changes Made as
+14/07/2023 at 10:57am` If you have any questions, suggestions, or issues,
+please feel free to reach out to the project maintainer, Arunraj, at
+srvnn_arunraj@gmail.com. [PyPI_Version]
```

### Comparing `ML-Algo-1.2.7/setup.py` & `ML-Algo-1.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ML-Algo',
-    version='1.2.7',
+    version='1.2.8',
     author='Mr Raj',
     author_email='arunraj14092002@gmail.com',
     description='A package for calculating Series Time Data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['ML_Algo'],
     install_requires=['pandas','requests'],
```

