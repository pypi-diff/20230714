# Comparing `tmp/BTM-1.1.2.tar.gz` & `tmp/BTM-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/BTM/dist/.tmp-jlh5x09i/BTM-1.1.2.tar", last modified: Fri Jul 14 13:23:50 2023, max compression
+gzip compressed data, was "/Users/shuzhao/li.github/BTM/dist/.tmp-s43sg6gt/BTM-1.1.3.tar", last modified: Fri Jul 14 13:43:23 2023, max compression
```

## Comparing `BTM-1.1.2.tar` & `BTM-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-07-14 13:23:50.000000 BTM-1.1.2/
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM/
--rw-r--r--   0 shuzhao    (501) staff       (20)    88465 2021-05-02 18:52:45.000000 BTM-1.1.2/BTM/BTM_Plus.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       34 2023-07-14 01:28:28.000000 BTM-1.1.2/BTM/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  4332831 2023-07-14 01:22:49.000000 BTM-1.1.2/BTM/affy.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    90287 2023-07-14 01:25:22.000000 BTM-1.1.2/BTM/btm2013.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      450 2023-07-14 01:25:44.000000 BTM-1.1.2/BTM/btm_example_data.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     3443 2023-07-14 13:23:36.000000 BTM-1.1.2/BTM/btm_plus_tool.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    13915 2023-07-14 01:28:28.000000 BTM-1.1.2/BTM/btm_tool.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     5116 2021-05-03 13:47:22.000000 BTM-1.1.2/BTM/permutate.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     4065 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      319 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       12 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-07-14 13:23:50.000000 BTM-1.1.2/BTM.egg-info/zip-safe
--rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 BTM-1.1.2/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     4065 2023-07-14 13:23:50.000000 BTM-1.1.2/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)     3266 2023-07-14 13:23:36.000000 BTM-1.1.2/README.md
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-07-14 13:23:50.000000 BTM-1.1.2/setup.cfg
--rw-r--r--   0 shuzhao    (501) staff       (20)      991 2023-07-14 13:06:51.000000 BTM-1.1.2/setup.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-07-14 13:43:23.000000 BTM-1.1.3/
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM/
+-rw-r--r--   0 shuzhao    (501) staff       (20)    88465 2021-05-02 18:52:45.000000 BTM-1.1.3/BTM/BTM_Plus.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       34 2023-07-14 13:41:24.000000 BTM-1.1.3/BTM/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)  4332831 2023-07-14 01:22:49.000000 BTM-1.1.3/BTM/affy.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    90287 2023-07-14 01:25:22.000000 BTM-1.1.3/BTM/btm2013.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      450 2023-07-14 01:25:44.000000 BTM-1.1.3/BTM/btm_example_data.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     3572 2023-07-14 13:41:24.000000 BTM-1.1.3/BTM/btm_plus_tool.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    13915 2023-07-14 01:28:28.000000 BTM-1.1.3/BTM/btm_tool.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5116 2021-05-03 13:47:22.000000 BTM-1.1.3/BTM/permutate.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4065 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)      319 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/SOURCES.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/dependency_links.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       12 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/requires.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/top_level.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-07-14 13:43:23.000000 BTM-1.1.3/BTM.egg-info/zip-safe
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 BTM-1.1.3/LICENSE
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4065 2023-07-14 13:43:23.000000 BTM-1.1.3/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)     3266 2023-07-14 13:23:36.000000 BTM-1.1.3/README.md
+-rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-07-14 13:43:23.000000 BTM-1.1.3/setup.cfg
+-rw-r--r--   0 shuzhao    (501) staff       (20)      991 2023-07-14 13:41:24.000000 BTM-1.1.3/setup.py
```

### Comparing `BTM-1.1.2/BTM/BTM_Plus.py` & `BTM-1.1.3/BTM/BTM_Plus.py`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/BTM/affy.py` & `BTM-1.1.3/BTM/affy.py`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/BTM/btm2013.py` & `BTM-1.1.3/BTM/btm2013.py`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/BTM/btm_plus_tool.py` & `BTM-1.1.3/BTM/btm_plus_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 
 >>> gd, header = read_gene_data('mydata.txt', gene_col=0, start_col=3, sep='\t')
 >>> gene_data_to_activityscores(gd, header, B2, zscore=True, outfile='btmplus_mydata.txt')
 
 '''
 
 import numpy as np
-from scipy import stats
+
+def zscore(a):
+    m, std = np.mean(a), np.std(a)
+    if std == 0:
+        return np.zeros(a.shape)
+    else:
+        return (a-m)/std
 
 def dequote(s): return s.replace('"', '').replace("'", "")
 
 def read_gene_data(infile, gene_col=0, start_col=1, sep='\t'):
     '''
     returns gene_data dictionary and header.
     gene_col : column for gene names/symbols.
@@ -40,28 +46,28 @@
     print("Got %d lines of gene data: " %len(gene_data))
 
     return gene_data, header
 
 def gene_data_to_activityscores(gene_data,
                                 header, 
                                 module_list,
-                                zscore=True,
+                                zstandardize=True,
                                 outfile='btm_plus_converted_activities.tsv'):
     '''
     Convert gene level data to BTM activity scores.
     
     Note: this works without zscore when difference of expression is taken between time points,
     which self-normalize to subjects. 
     Standardization is needed if the activity score is computed for original gene expression,
     e.g. z-scores are calculated across samples and module scores are then computed on z-scores. 
     Default for gene_data_to_activityscores.
     '''
-    if zscore:
+    if zstandardize:
         for g,v in gene_data.items():
-            v = stats.zscore(v)
+            gene_data[g] = zscore(v)
         
     s = '\t'.join(['id', 'name', 'src'] + header[1:]) + '\n'
     for x in module_list:
         ascores = compute_activity_score(x['genes'], gene_data)
         s += '\t'.join([x['id'], x['name'], str(x['src'])] + [str(d.round(3)) for d in ascores]) + '\n'
         
     out = open(outfile, 'w')
```

### Comparing `BTM-1.1.2/BTM/btm_tool.py` & `BTM-1.1.3/BTM/btm_tool.py`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/BTM/permutate.py` & `BTM-1.1.3/BTM/permutate.py`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/BTM.egg-info/PKG-INFO` & `BTM-1.1.3/BTM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTM
-Version: 1.1.2
+Version: 1.1.3
 Summary: Blood Transcription Modules for transcriptomics analysis
 Home-page: https://github.com/shuzhao-li/BTM
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: MIT
 Keywords: transcriptomics analysis bioinformatics immunology systems biology
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `BTM-1.1.2/LICENSE` & `BTM-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/PKG-INFO` & `BTM-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTM
-Version: 1.1.2
+Version: 1.1.3
 Summary: Blood Transcription Modules for transcriptomics analysis
 Home-page: https://github.com/shuzhao-li/BTM
 Author: Shuzhao Li
 Author-email: shuzhao.li@gmail.com
 License: MIT
 Keywords: transcriptomics analysis bioinformatics immunology systems biology
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `BTM-1.1.2/README.md` & `BTM-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `BTM-1.1.2/setup.py` & `BTM-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
   name='BTM',
-  version='1.1.2',
+  version='1.1.3',
 
   author='Shuzhao Li',
   author_email='shuzhao.li@gmail.com',
   description='Blood Transcription Modules for transcriptomics analysis',
   long_description=open('README.md').read(),
   url='https://github.com/shuzhao-li/BTM',
   license='MIT',
```

