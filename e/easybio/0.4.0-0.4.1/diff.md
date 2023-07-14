# Comparing `tmp/easybio-0.4.0.tar.gz` & `tmp/easybio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.4.0.tar", last modified: Tue Jul 11 04:08:09 2023, max compression
+gzip compressed data, was "easybio-0.4.1.tar", last modified: Fri Jul 14 10:42:01 2023, max compression
```

## Comparing `easybio-0.4.0.tar` & `easybio-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.217344 easybio-0.4.0/
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-11 04:08:09.217344 easybio-0.4.0/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)       30 2023-04-21 05:50:43.000000 easybio-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.209345 easybio-0.4.0/easyBio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.217344 easybio-0.4.0/easyBio/Utils/
--rw-rw-r--   0 root         (0) root         (0)      661 2023-07-07 11:47:13.000000 easybio-0.4.0/easyBio/Utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2854 2023-07-07 09:45:10.000000 easybio-0.4.0/easyBio/Utils/downLoadBAM.py
--rw-rw-r--   0 root         (0) root         (0)     2901 2023-07-07 02:09:13.000000 easybio-0.4.0/easyBio/Utils/downLoadSRA.py
--rw-rw-r--   0 root         (0) root         (0)     8221 2023-07-07 02:07:55.000000 easybio-0.4.0/easyBio/Utils/download.py
--rw-rw-r--   0 root         (0) root         (0)     4193 2023-07-07 11:51:19.000000 easybio-0.4.0/easyBio/Utils/downloadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     9077 2023-07-06 12:33:28.000000 easybio-0.4.0/easyBio/Utils/easyBioUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-07-06 13:07:59.000000 easybio-0.4.0/easyBio/Utils/easyCellranger.py
--rw-rw-r--   0 root         (0) root         (0)    12122 2023-07-06 13:13:28.000000 easybio-0.4.0/easyBio/Utils/gsaDownLoadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2117 2023-04-26 10:50:17.000000 easybio-0.4.0/easyBio/Utils/netUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2594 2023-07-07 11:45:29.000000 easybio-0.4.0/easyBio/Utils/runvelocityc.py
--rw-rw-r--   0 root         (0) root         (0)     7817 2023-07-11 04:04:53.000000 easybio-0.4.0/easyBio/Utils/toFastq.py
--rw-rw-r--   0 root         (0) root         (0)     3735 2023-07-07 09:45:19.000000 easybio-0.4.0/easyBio/Utils/toolsUtils.py
--rw-rw-r--   0 root         (0) root         (0)      426 2023-07-06 12:55:32.000000 easybio-0.4.0/easyBio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6283 2023-07-06 12:31:50.000000 easybio-0.4.0/easyBio/changeSRAName.py
--rw-rw-r--   0 root         (0) root         (0)     2142 2023-07-07 01:45:29.000000 easybio-0.4.0/easyBio/downloadSRA.py
--rw-rw-r--   0 root         (0) root         (0)      200 2023-04-26 10:50:00.000000 easybio-0.4.0/easyBio/easyBio.py
--rw-rw-r--   0 root         (0) root         (0)     2692 2023-07-06 13:12:50.000000 easybio-0.4.0/easyBio/gsaPipline.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-10 12:28:56.000000 easybio-0.4.0/easyBio/pipline.py
--rw-rw-r--   0 root         (0) root         (0)     1324 2023-07-06 13:03:21.000000 easybio-0.4.0/easyBio/run_cellranger.py
--rw-rw-r--   0 root         (0) root         (0)      110 2023-04-26 10:48:58.000000 easybio-0.4.0/easyBio/run_test.py
--rw-rw-r--   0 root         (0) root         (0)     1247 2023-07-07 02:24:02.000000 easybio-0.4.0/easyBio/runvelocyto.py
--rw-rw-r--   0 root         (0) root         (0)     1479 2023-04-29 17:22:45.000000 easybio-0.4.0/easyBio/splitSRA.py
--rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 17:25:20.000000 easybio-0.4.0/easyBio/test.py
--rw-rw-r--   0 root         (0) root         (0)     2301 2023-05-29 01:59:25.000000 easybio-0.4.0/easyBio/tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 04:08:09.217344 easybio-0.4.0/easybio.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      538 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      831 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      345 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-22 17:45:52.000000 easybio-0.4.0/easybio.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)       43 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        8 2023-07-11 04:08:09.000000 easybio-0.4.0/easybio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 04:08:09.217344 easybio-0.4.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1539 2023-07-07 02:28:58.000000 easybio-0.4.0/setup.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-14 10:42:01.258853 easybio-0.4.1/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-07-14 10:42:01.258853 easybio-0.4.1/PKG-INFO
+-rwxrwxr-x   0 lei       (1003) lei       (1004)       30 2023-04-21 05:50:43.000000 easybio-0.4.1/README.md
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-14 10:42:01.254853 easybio-0.4.1/easyBio/
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-14 10:42:01.254853 easybio-0.4.1/easyBio/Utils/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      661 2023-07-07 11:47:13.000000 easybio-0.4.1/easyBio/Utils/__init__.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2854 2023-07-07 09:45:10.000000 easybio-0.4.1/easyBio/Utils/downLoadBAM.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2901 2023-07-07 02:09:13.000000 easybio-0.4.1/easyBio/Utils/downLoadSRA.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     8221 2023-07-07 02:07:55.000000 easybio-0.4.1/easyBio/Utils/download.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     4193 2023-07-07 11:51:19.000000 easybio-0.4.1/easyBio/Utils/downloadUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     9077 2023-07-06 12:33:28.000000 easybio-0.4.1/easyBio/Utils/easyBioUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2216 2023-07-06 13:07:59.000000 easybio-0.4.1/easyBio/Utils/easyCellranger.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)    12112 2023-07-14 10:32:06.000000 easybio-0.4.1/easyBio/Utils/gsaDownLoadUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2117 2023-04-26 10:50:17.000000 easybio-0.4.1/easyBio/Utils/netUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2594 2023-07-07 11:45:29.000000 easybio-0.4.1/easyBio/Utils/runvelocityc.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     7773 2023-07-14 10:39:20.000000 easybio-0.4.1/easyBio/Utils/toFastq.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3735 2023-07-07 09:45:19.000000 easybio-0.4.1/easyBio/Utils/toolsUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      426 2023-07-06 12:55:32.000000 easybio-0.4.1/easyBio/__init__.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     6283 2023-07-12 07:12:26.000000 easybio-0.4.1/easyBio/changeSRAName.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2136 2023-07-14 04:32:24.000000 easybio-0.4.1/easyBio/downloadSRA.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      200 2023-07-12 06:59:45.000000 easybio-0.4.1/easyBio/easyBio.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2636 2023-07-14 04:40:35.000000 easybio-0.4.1/easyBio/gsaPipline.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     5024 2023-07-14 10:32:46.000000 easybio-0.4.1/easyBio/pipline.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1324 2023-07-12 07:12:35.000000 easybio-0.4.1/easyBio/run_cellranger.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      110 2023-07-12 11:04:38.000000 easybio-0.4.1/easyBio/run_test.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1247 2023-07-12 07:12:38.000000 easybio-0.4.1/easyBio/runvelocyto.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1479 2023-07-12 07:12:42.000000 easybio-0.4.1/easyBio/splitSRA.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1006 2023-04-29 17:25:20.000000 easybio-0.4.1/easyBio/test.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2671 2023-07-12 07:12:49.000000 easybio-0.4.1/easyBio/tidy.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-07-14 10:42:01.258853 easybio-0.4.1/easybio.egg-info/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-07-14 10:42:01.000000 easybio-0.4.1/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1003) lei       (1004)      831 2023-07-14 10:42:01.000000 easybio-0.4.1/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-07-14 10:42:01.000000 easybio-0.4.1/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)      344 2023-07-14 10:42:01.000000 easybio-0.4.1/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-07-14 10:41:43.000000 easybio-0.4.1/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 lei       (1003) lei       (1004)       27 2023-07-14 10:42:01.000000 easybio-0.4.1/easybio.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-07-14 10:42:01.000000 easybio-0.4.1/easybio.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-07-14 10:42:01.258853 easybio-0.4.1/setup.cfg
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1562 2023-07-14 10:39:27.000000 easybio-0.4.1/setup.py
```

### Comparing `easybio-0.4.0/PKG-INFO` & `easybio-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.4.0
+Version: 0.4.1
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
@@ -12,9 +12,7 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 
 # easyBio_conda
 easyBio_conda
-
-
```

### Comparing `easybio-0.4.0/easyBio/Utils/__init__.py` & `easybio-0.4.1/easyBio/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/downLoadBAM.py` & `easybio-0.4.1/easyBio/Utils/downLoadBAM.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/downLoadSRA.py` & `easybio-0.4.1/easyBio/Utils/downLoadSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/download.py` & `easybio-0.4.1/easyBio/Utils/download.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/downloadUtils.py` & `easybio-0.4.1/easyBio/Utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/easyBioUtils.py` & `easybio-0.4.1/easyBio/Utils/easyBioUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/easyCellranger.py` & `easybio-0.4.1/easyBio/Utils/easyCellranger.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/gsaDownLoadUtils.py` & `easybio-0.4.1/easyBio/Utils/gsaDownLoadUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,27 +255,25 @@
         else:
             files, srr_counts = self.count_hrr_occurrences_fq(folder_path)
             self.rename_files(self.getFileMapping(), files,
                               srr_counts, folder_path)
             print("\033[1;32m Rename completed\033[0m")
     
     def cellrangerRun(self, db, expectcellnum = 3000, fq_dir = "", otherItem="", matricespath=""):
-
         if matricespath == "":
             matricespath = f"{self.raw_path}/matrices"
             
         if fq_dir == "":
             # 获取文件夹中的所有文件名
             fq_dir = self.fq_path
 
         ec = easyCellranger(fq_dir, expectcellnum,
                             db, otherItem, matricespath)
         ec.cellrangerRun()
         
-        
         # if fq_dir == "":
         #     # 获取文件夹中的所有文件名
         #     fq_dir = self.fq_path
         #     filenames = os.listdir(self.fq_path)
         
     #     current_dir = os.getcwd()
     #     # 获取目录中所有的子目录
```

### Comparing `easybio-0.4.0/easyBio/Utils/netUtils.py` & `easybio-0.4.1/easyBio/Utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/runvelocityc.py` & `easybio-0.4.1/easyBio/Utils/runvelocityc.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/Utils/toFastq.py` & `easybio-0.4.1/easyBio/Utils/toFastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,26 @@
             print(f"fastq文件已进行改名")
         else:
             self.BtF(self.dataDir, tofqPath)
             self.mvtoFastq(tofqPath)
             print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
             
     def mvtoFastq(self, tofqPath):
+        if not tofqPath.endswith("/"):
+            tofqPath = tofqPath + "/"
         for filepath, dirnames, filenames in os.walk(tofqPath):
             for filename in filenames:
-                # print(filename)
                 filedir = os.path.join(filepath, filename)
-                # print(filedir)
-                sampleid = filedir.split("/tofq/")[1].split("/")[0]
+                sampleid = filedir.split(tofqPath)[1].split("/")[0]
                 sampleid = os.path.split(filedir)[0].split("/")
                 sampleid = sampleid[len(sampleid)-2]
                 sampleid = sampleid.replace("_", "-")
-                # sampleid
                 fileName = os.path.split(filedir)[1].split("_")
                 fileName[0] = sampleid
                 fileName = "_".join(fileName)
-                # fileName
                 fileName = os.path.join(self.FastqDir, fileName)
                 print(filedir, " to ", fileName)
                 os.renames(filedir, fileName)
         
 
     def BamfastqExist(self, tofqPath, simpleName):
         sampletofqPath = os.path.join(tofqPath, simpleName)
```

### Comparing `easybio-0.4.0/easyBio/Utils/toolsUtils.py` & `easybio-0.4.1/easyBio/Utils/toolsUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/changeSRAName.py` & `easybio-0.4.1/easyBio/changeSRAName.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/downloadSRA.py` & `easybio-0.4.1/easyBio/downloadSRA.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # Description:
 import argparse
 import os
 
 from .Utils import downLoadSRA, getProResults
 from .Utils import get_num_threads, sraMd5Cal
 
-
 def main():
     num_threads = get_num_threads()
 
     parser = argparse.ArgumentParser(
         description="Process GSE number, directory and threads")
     parser.add_argument("-g", "--gsenumber", help="GSE number")
     parser.add_argument("-d", "--dirs", default=os.getcwd(),
@@ -61,11 +60,10 @@
     reDownloadSra = [1, 2, 3]
     while len(reDownloadSra) > 1:
         check=False
         while not check:
             # print(results)
             check = downLoadSRA(gsenumber, results, dirs, threads)
         reDownloadSra = sraMd5Cal(filedirs, md5List, rawdirs)
-    
 
 if __name__ == "__main__":
     main()
```

### Comparing `easybio-0.4.0/easyBio/gsaPipline.py` & `easybio-0.4.1/easyBio/gsaPipline.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 from .Utils import tidySummary, getProResults, sraMd5Cal
 from .Utils import get_num_threads, calMd5, gsaProject
 
 from .changeSRAName import renames1, renames2, renames3
 from .Utils import check_file_exists, cellrangerRun, splitSRAfun, downLoadSRA, cellrangerRun2
 import argparse
 
-# inputName = "PRJCA014236"
-# inputName = "HRA003747"
-
-
 def main():
     num_threads = get_num_threads()
     # Set up argument parser
     parser = argparse.ArgumentParser(
         description="Process GSA number, directory and threads")
     parser.add_argument("-i", "--inputName", help="Project Number")
     parser.add_argument("-d", "--dirs", default=os.getcwd(),
```

### Comparing `easybio-0.4.0/easyBio/pipline.py` & `easybio-0.4.1/easyBio/pipline.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/run_cellranger.py` & `easybio-0.4.1/easyBio/run_cellranger.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/runvelocyto.py` & `easybio-0.4.1/easyBio/runvelocyto.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/splitSRA.py` & `easybio-0.4.1/easyBio/splitSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/test.py` & `easybio-0.4.1/easyBio/test.py`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/easyBio/tidy.py` & `easybio-0.4.1/easyBio/tidy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 
-import os
-import shutil
-
-
-matricespath = "/home/data/user/lei/SRAData/GSE/GSE162454/raw//matrices"
-outputpath = "/home/data/user/lei/SRAData/GSE/GSE162454/raw//output"
-
-
-def tidySummary(matrices_base, output_base):
-    summary_base = os.path.join(output_base, "summary")
-    matrix_base = os.path.join(output_base, "matrix")
-    matrixh5_base = os.path.join(output_base, "matrixh5")
-    loomFile_base = os.path.join(output_base, "loomfile")
-
-    # 如果目标文件夹不存在，创建它
-    os.makedirs(summary_base, exist_ok=True)
-    os.makedirs(matrix_base, exist_ok=True)
-    os.makedirs(matrixh5_base, exist_ok=True)
-    os.makedirs(loomFile_base, exist_ok=True)
-
-    for folder in os.listdir(matrices_base):
-        src_folder = os.path.join(matrices_base, folder)
-
-        if os.path.isdir(src_folder):
-            src_file = os.path.join(src_folder, 'outs', 'web_summary.html')
-            src_matrix_folder = os.path.join(
-                src_folder, 'outs', 'filtered_feature_bc_matrix')
-            matrixh5flie = os.path.join(
-                src_folder, 'outs', 'filtered_feature_bc_matrix.h5')
-            loom_file = os.path.join(
-                src_folder, 'velocyto', f'{folder}.loom')
-
-            if os.path.exists(src_file):
-                dst_file = os.path.join(summary_base, folder + '.html')
-                if not os.path.exists(dst_file):
-                    shutil.copy2(src_file, dst_file)
+# from .Utils import tidySummary
+# import os
+# import shutil
+
+
+# matricespath = "/home/data/user/lei/SRAData/GSE/GSE162454/raw//matrices"
+# outputpath = "/home/data/user/lei/SRAData/GSE/GSE162454/raw//output"
+
+
+# def tidySummary(matrices_base, output_base):
+#     summary_base = os.path.join(output_base, "summary")
+#     matrix_base = os.path.join(output_base, "matrix")
+#     matrixh5_base = os.path.join(output_base, "matrixh5")
+#     loomFile_base = os.path.join(output_base, "loomfile")
+
+#     # 如果目标文件夹不存在，创建它
+#     os.makedirs(summary_base, exist_ok=True)
+#     os.makedirs(matrix_base, exist_ok=True)
+#     os.makedirs(matrixh5_base, exist_ok=True)
+#     os.makedirs(loomFile_base, exist_ok=True)
+
+#     for folder in os.listdir(matrices_base):
+#         src_folder = os.path.join(matrices_base, folder)
+
+#         if os.path.isdir(src_folder):
+#             src_file = os.path.join(src_folder, 'outs', 'web_summary.html')
+#             src_matrix_folder = os.path.join(
+#                 src_folder, 'outs', 'filtered_feature_bc_matrix')
+#             matrixh5flie = os.path.join(
+#                 src_folder, 'outs', 'filtered_feature_bc_matrix.h5')
+#             loom_file = os.path.join(
+#                 src_folder, 'velocyto', f'{folder}.loom')
+
+#             if os.path.exists(src_file):
+#                 dst_file = os.path.join(summary_base, folder + '.html')
+#                 if not os.path.exists(dst_file):
+#                     shutil.copy2(src_file, dst_file)
                 
-            if os.path.exists(src_matrix_folder):
-                dst_matrix_folder = os.path.join(matrix_base, folder)
-                if not os.path.exists(dst_matrix_folder):
-                    shutil.copytree(src_matrix_folder, dst_matrix_folder)
+#             if os.path.exists(src_matrix_folder):
+#                 dst_matrix_folder = os.path.join(matrix_base, folder)
+#                 if not os.path.exists(dst_matrix_folder):
+#                     shutil.copytree(src_matrix_folder, dst_matrix_folder)
             
-            if os.path.exists(matrixh5flie):
-                dst_matrixh5_folder = os.path.join(matrixh5_base, folder)
-                if not os.path.exists(dst_matrixh5_folder):
-                    shutil.copy2(matrixh5flie, dst_matrixh5_folder)
+#             if os.path.exists(matrixh5flie):
+#                 dst_matrixh5_folder = os.path.join(matrixh5_base, folder)
+#                 if not os.path.exists(dst_matrixh5_folder):
+#                     shutil.copy2(matrixh5flie, dst_matrixh5_folder)
                     
-            if os.path.exists(matrixh5flie):
-                loomFile_base_folder = os.path.join(loomFile_base, folder)
-                if not os.path.exists(loomFile_base_folder):
-                    shutil.copy2(loom_file, loomFile_base_folder)
+#             if os.path.exists(matrixh5flie):
+#                 loomFile_base_folder = os.path.join(loomFile_base, folder)
+#                 if not os.path.exists(loomFile_base_folder):
+#                     shutil.copy2(loom_file, loomFile_base_folder)
                     
                     
-tidySummary(matricespath, outputpath)
+# tidySummary(matricespath, outputpath)
+
+# outputpath = f"/home/data/groupdata/杨骁老师原始数据/output"
+# os.makedirs(outputpath, exist_ok=True)
+#        # 设置源文件夹和目标文件夹的路径
+# tidySummary("/home/data/groupdata/杨骁老师原始数据/matrices", outputpath)
```

### Comparing `easybio-0.4.0/easybio.egg-info/PKG-INFO` & `easybio-0.4.1/easybio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.4.0
+Version: 0.4.1
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
@@ -12,9 +12,7 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 
 # easyBio_conda
 easyBio_conda
-
-
```

### Comparing `easybio-0.4.0/easybio.egg-info/SOURCES.txt` & `easybio-0.4.1/easybio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easybio-0.4.0/setup.py` & `easybio-0.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 
 setup(
     name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
@@ -30,17 +30,18 @@
             'easyscGSEpipline=easyBio.gsaPipline:main',
         ]
     },
     install_requires=[
         # 'biopython',
         'threadpool',
         'requests',
-        'pandas',
-        'velocyto',
-        'psutil'
+        'pandas'
+        # 'velocyto',
+        # 'psutil',
+        # 'Cython'
         # Add more dependencies here
     ],
     package_data={
         'Utils': ['Utils/*']
     },
     classifiers=[
         'Operating System :: OS Independent',
```

