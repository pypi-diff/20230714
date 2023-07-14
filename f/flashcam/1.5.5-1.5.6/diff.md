# Comparing `tmp/flashcam-1.5.5.tar.gz` & `tmp/flashcam-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.5.tar", last modified: Fri Jul 14 08:39:01 2023, max compression
+gzip compressed data, was "flashcam-1.5.6.tar", last modified: Fri Jul 14 16:20:04 2023, max compression
```

## Comparing `flashcam-1.5.5.tar` & `flashcam-1.5.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.513224 flashcam-1.5.5/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 08:39:01.513224 flashcam-1.5.5/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 08:38:59.000000 flashcam-1.5.5/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.509224 flashcam-1.5.5/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24865 2023-07-14 08:38:46.000000 flashcam-1.5.5/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.5.5/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.5.5/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.5.5/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.509224 flashcam-1.5.5/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.5.5/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.5.5/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.513224 flashcam-1.5.5/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/c120.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/c270_orig.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/cameras.org
--rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/cameras.pdf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/cameras.tex
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.5.5/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/f100.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/f100_orig.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/vf0770.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.5.5/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.5.5/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.5.5/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.5.5/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40604 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   102717 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.5.5/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27704 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:26:31.000000 flashcam-1.5.5/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.509224 flashcam-1.5.5/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1025 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 08:39:01.513224 flashcam-1.5.5/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 07:00:29.000000 flashcam-1.5.5/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.072691 flashcam-1.5.6/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:20:04.072691 flashcam-1.5.6/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 16:19:59.000000 flashcam-1.5.6/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.068691 flashcam-1.5.6/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 16:20:01.000000 flashcam-1.5.6/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.5.6/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.5.6/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.5.6/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.068691 flashcam-1.5.6/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.5.6/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.5.6/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-14 08:38:46.000000 flashcam-1.5.6/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.072691 flashcam-1.5.6/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/c120.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/c270_orig.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/cameras.org
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/cameras.pdf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/cameras.tex
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.5.6/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/f100.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/f100_orig.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/vf0770.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.5.6/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.5.6/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.5.6/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.5.6/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    43323 2023-07-14 16:16:55.000000 flashcam-1.5.6/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   104477 2023-07-14 09:57:07.000000 flashcam-1.5.6/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.5.6/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34128 2023-07-14 16:11:55.000000 flashcam-1.5.6/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 16:20:03.000000 flashcam-1.5.6/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:26:31.000000 flashcam-1.5.6/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.068691 flashcam-1.5.6/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1025 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 16:20:04.072691 flashcam-1.5.6/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 07:00:29.000000 flashcam-1.5.6/setup.py
```

### Comparing `flashcam-1.5.5/PKG-INFO` & `flashcam-1.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.5
+Version: 1.5.6
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.5/README.md` & `flashcam-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/bin/flashcam` & `flashcam-1.5.6/bin/flashcam`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 import atexit
 
 import flashcam.config as config
 
 try:
     import flashcam.uniwrec as uniwrec
 except:
-    print("X... cannot import uniwrec ... ?problem with pynput and Xserver")
-    print(" ... i go on... anyway")
+    #print("X... cannot import uniwrec ... ?problem with pynput and Xserver")
+    print("X ... cannot import uniwrec ...i go on... anyway")
 
 import os #  for exit
 
 import numpy as np
 
 import datetime as dt
```

### Comparing `flashcam-1.5.5/bin/flashcamg` & `flashcam-1.5.6/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/base_camera2.py` & `flashcam-1.5.6/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/config.py` & `flashcam-1.5.6/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.6/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.6/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.6/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.6/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/c120.jpg` & `flashcam-1.5.6/flashcam/data/c120.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/c270_orig.png` & `flashcam-1.5.6/flashcam/data/c270_orig.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/cameras.org` & `flashcam-1.5.6/flashcam/data/cameras.org`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/cameras.pdf` & `flashcam-1.5.6/flashcam/data/cameras.pdf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/cameras.tex` & `flashcam-1.5.6/flashcam/data/cameras.tex`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.6/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/f100.jpg` & `flashcam-1.5.6/flashcam/data/f100.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/f100_orig.jpg` & `flashcam-1.5.6/flashcam/data/f100_orig.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/monoskop.jpg` & `flashcam-1.5.6/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/vf0770.jpg` & `flashcam-1.5.6/flashcam/data/vf0770.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/win_rain.jpg` & `flashcam-1.5.6/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/win_skull.jpg` & `flashcam-1.5.6/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/win_storm.jpg` & `flashcam-1.5.6/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/win_winter.jpg` & `flashcam-1.5.6/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/data/windows.jpg` & `flashcam-1.5.6/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/direct.py` & `flashcam-1.5.6/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/izmq_receiver.py` & `flashcam-1.5.6/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/mmapwr.py` & `flashcam-1.5.6/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/real_camera.py` & `flashcam-1.5.6/flashcam/real_camera.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # FOR CONNECTION TO FLASHCAM AND NOTIFATOR - SEE FLASHCAM README.org
 
+import random
 import cv2
 from flashcam.base_camera2 import BaseCamera
 
 from flashcam.usbcheck import recommend_video
 # import base_camera  #  Switches: slowrate....
 
 import datetime as dt
@@ -388,36 +389,41 @@
                     set_gem(cc, "def","auto","def") # exp 'def' is different from auto
             else:
                 # I CALL SET_GAM from
                 set_gem(cc, config.CONFIG['gain'],
                         config.CONFIG['expo'],
                         config.CONFIG['mmaga'])
 
+
+            #--- INITIATION...... collecting???
+
+            exposuredef = True
+            cc.autoexpo_on("autoexpo")
             aea,aex,aga,agm = get_gem(cc, capa)
             if aex!=None: ex,exd,mine,maxe,ex10 = aex
             if agm!=None: gm,gmd,minm,maxm,gm10 = agm
             if aga!=None: ga,gad,ming,maxg,ga10 = aga
 
             # very stupid camera    ZC0303 Webcam
             if "exposure" in capa:
                 exposure = cc.get_exposure()
                 exposuredef = cc.getdef_exposure()
                 #?????
                 #auto_exposuredef = cc.getdef_exposure()
                 print(f"i... EXPOAUTO (top) == {exposure} vs def={exposuredef}; ")
 
 
-            if "auto_exposure" in capa:
-                expo_auto = cc.get_auto_exposure()
-                expo_autodef = cc.getdef_auto_exposure()
-                print(f"i... EXPOAUTO (TOP) == {expo_auto} vs def={expo_autodef}; ")
-
-            if "exposure_time_absolute" in capa:
-                exposure_time_absolute = cc.get_exposure_time_absolute()
-                exposuredef = cc.getdef_exposure_time_absolute() # i think all cams
+            # if "auto_exposure" in capa:
+            #     expo_auto = cc.get_auto_exposure()
+            #     expo_autodef = cc.getdef_auto_exposure()
+            #     print(f"i... EXPOAUTO (TOP) == {expo_auto} vs def={expo_autodef}; ")
+
+            # if "exposure_time_absolute" in capa:
+            #     exposure_time_absolute = cc.get_exposure_time_absolute()
+            #     exposuredef = cc.getdef_exposure_time_absolute() # i think all cams
 
             if "gain" in capa:
                 gain = cc.get_gain()
                 gaindef = cc.getdef_gain()
 
             if "gamma" in capa:
                 gamma = cc.get_gamma()
@@ -675,121 +681,166 @@
                                 gainvalue = -999
 
                             if  'gain' in locals() and gain != gaindef:
                                 senh.setbox(f"g {(gain-ming)/(maxg-ming):.4f}",  senh.gain)
                         #-----------------gain in capa
 
                         # Sony Chip v2
-                        if  "exposure_time_absolute" in capa:
-                            if expo_divide:
-                                expo_divide = False
-                                #if "exposure_time_absolute" in capa:
-                                cc.set_auto_exposure(1) #hardcoded 1
-                                exposure_time_absolute = cc.get_exposure_time_absolute()
-                                newexposure =  int(exposure_time_absolute/2)
-                                if newexposure<mine: newexposure = mine
-                                print("i... ex:", exposure_time_absolute, newexposure)
-                                cc.set_exposure_time_absolute( newexposure)
-                                exposure = newexposure # SENH
+                        # if  "exposure_time_absolute" in capa:
+                        #     if expo_divide:
+                        #         expo_divide = False
+                        #         #if "exposure_time_absolute" in capa:
+                        #         cc.set_auto_exposure(1) #hardcoded 1
+                        #         exposure_time_absolute = cc.get_exposure_time_absolute()
+                        #         newexposure =  int(exposure_time_absolute/2)
+                        #         if newexposure<mine: newexposure = mine
+                        #         print("i... ex:", exposure_time_absolute, newexposure)
+                        #         cc.set_exposure_time_absolute( newexposure)
+                        #         exposure = newexposure # SENH
+
+                        #     if expo_multiply:
+                        #         expo_multiply = False
+                        #         #if "exposure_time_absolute" in capa:
+                        #         cc.set_auto_exposure(1) #harcoded 1
+                        #         exposure_time_absolute = cc.get_exposure_time_absolute()
+                        #         e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                        #         print("i... e10===", e10)
+                        #         if (e10>=0.0001) and (e10<=0.5):
+                        #             newexposure = int(exposure_time_absolute*2)
+                        #         elif (e10>0.5):
+                        #             newexposure = int(maxe)
+                        #         elif (e10<=0.0001):
+                        #             newexposure = int(mine+1)
+                        #         else:
+                        #             newexposure =  int(mine+1)
+                        #         cc.set_exposure_time_absolute( newexposure )
+                        #         exposure = newexposure # SENH
+
+                        #     if expo_setdef:
+                        #         expo_setdef = False
+                        #         #if "auto_exposure" in capa:
+                        #         # cc.setdef_auto_exposure() # Sony v2 prob
+                        #         # HARDCODE-frm ubu22
+                        #         cc.set_auto_exposure(3)
+                        #         cc.setdef_exposure_time_absolute( )
+                        #         exposure = exposuredef #
+                        #         print("i... exposure to def: ",exposure)
+
+                        #     # HIDDEN CAPABILITY ??? Sony Chipv2
+                        #     if expovalue>=0 and expovalue<=1:
+                        #         cc.set_auto_exposure(1) #harcoded 1
+                        #         #exposure_time_absolute = cc.get_exposure_time_absolute()
+                        #         #e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                        #         newexposure = int( (maxe-mine)*expovalue ) + mine
+                        #         print(f"NEW: expoHidCapSony {newexposure} from {expovalue}")
+                        #         cc.set_exposure_time_absolute( newexposure )
+                        #         exposure = newexposure # SENH
+                        #         expovalue = -999
 
-                            if expo_multiply:
-                                expo_multiply = False
-                                #if "exposure_time_absolute" in capa:
-                                cc.set_auto_exposure(1) #harcoded 1
-                                exposure_time_absolute = cc.get_exposure_time_absolute()
-                                e10 = (exposure_time_absolute-mine)/(maxe-mine)
-                                print("i... e10===", e10)
-                                if (e10>=0.0001) and (e10<=0.5):
-                                    newexposure = int(exposure_time_absolute*2)
-                                elif (e10>0.5):
-                                    newexposure = int(maxe)
-                                elif (e10<=0.0001):
-                                    newexposure = int(mine+1)
-                                else:
-                                    newexposure =  int(mine+1)
-                                cc.set_exposure_time_absolute( newexposure )
-                                exposure = newexposure # SENH
+                        #     if  'exposure' in locals() and exposure != exposuredef:
+                        #         senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
 
-                            if expo_setdef:
-                                expo_setdef = False
-                                #if "auto_exposure" in capa:
-                                # cc.setdef_auto_exposure() # Sony v2 prob
-                                # HARDCODE-frm ubu22
-                                cc.set_auto_exposure(3)
-                                cc.setdef_exposure_time_absolute( )
-                                exposure = exposuredef #
-                                print("i... exposure to def: ",exposure)
-
-                            # HIDDEN CAPABILITY ??? Sony Chipv2
-                            if expovalue>=0 and expovalue<=1:
-                                cc.set_auto_exposure(1) #harcoded 1
-                                #exposure_time_absolute = cc.get_exposure_time_absolute()
-                                #e10 = (exposure_time_absolute-mine)/(maxe-mine)
-                                newexposure = int( (maxe-mine)*expovalue ) + mine
-                                print(f"NEW: expoHidCapSony {newexposure} from {expovalue}")
-                                cc.set_exposure_time_absolute( newexposure )
-                                exposure = newexposure # SENH
-                                expovalue = -999
+                        if "exposure_time_absolute" in capa or "exposure_absolute" in capa:
 
-                            if  'exposure' in locals() and exposure != exposuredef:
-                                senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
 
-                        if "exposure_time_absolute" in capa:
                             if expo_divide:
                                 expo_divide = False
-                                #if "exposure_time_absolute" in capa:
-                                cc.set_auto_exposure(1) #hardcoded 1
-                                exposure_time_absolute = cc.get_exposure_time_absolute()
-                                newexposure =  int(exposure_time_absolute/2)
-                                if newexposure<mine: newexposure = mine
-                                print("i... ex:", exposure_time_absolute, newexposure)
-                                cc.set_exposure_time_absolute( newexposure)
-                                exposure = newexposure # SENH
+                                v4lc.mk_table(cc)
+                                exposuredef = False
+
+                                cc.autoexpo_off( "autoexpo")
+
+                                exposure = cc.expo_get("expo_get")
+                                #print(f"i ... exposure- = {exposure} ")
+                                exposure = -0.1 + exposure
+                                cc.expo( exposure ,'expo')     # 0-1 log
+                                #exposure = cc.expo_get("expo_get")
+                                #print(f"i ... exposure- = {exposure} ")
+                                #senh.setbox(f"expo {exposure:.4f}",  senh.expo)
+                                v4lc.mk_table(cc)
+                                # #if "exposure_time_absolute" in capa:
+                                # cc.set_auto_exposure(1) #hardcoded 1
+                                # exposure_time_absolute = cc.get_exposure_time_absolute()
+                                # newexposure =  int(exposure_time_absolute/2)
+                                # if newexposure<mine: newexposure = mine
+                                # print("i... ex:", exposure_time_absolute, newexposure)
+                                # cc.set_exposure_time_absolute( newexposure)
+                                # exposure = newexposure # SENH
 
                             if expo_multiply:
                                 expo_multiply = False
-                                #if "exposure_time_absolute" in capa:
-                                cc.set_auto_exposure(1) #harcoded 1
-                                exposure_time_absolute = cc.get_exposure_time_absolute()
-                                e10 = (exposure_time_absolute-mine)/(maxe-mine)
-                                print("i... e10===", e10)
-                                if (e10>=0.0001) and (e10<=0.5):
-                                    newexposure = int(exposure_time_absolute*2)
-                                elif (e10>0.5):
-                                    newexposure = int(maxe)
-                                elif (e10<=0.0001):
-                                    newexposure = int(mine+1)
-                                else:
-                                    newexposure =  int(mine+1)
-                                cc.set_exposure_time_absolute( newexposure )
-                                exposure = newexposure # SENH
+                                v4lc.mk_table(cc)
+
+                                exposuredef = False
+
+                                # ra = random.uniform(0,1)
+                                # print("\n\n", round(ra,3) )
+                                cc.autoexpo_off( "autoexpo")
+                                exposure = cc.expo_get( 'expo_get')     # 0-1 log
+                                #print(" I found exposure === ", exposure)
+                                cc.expo( exposure + 0.1 ,'expo')     # 0-1 log
+
+                                # cc.autoexpo_off( "autoexpo")
+                                # time.sleep(0.1)
+                                # exposure = cc.expo_get("expo_get")
+                                # print(f"i ... exposure+ = {exposure} ")
+                                # exposure = exposure + 0.1
+                                # cc.expo( exposure ,'expo')     # 0-1 log
+                                # exposure = cc.expo_get("expo_get")
+                                # print(f"i ... exposure+ = {exposure} ")
+                                v4lc.mk_table(cc)
+                                # #if "exposure_time_absolute" in capa:
+                                # cc.set_auto_exposure(1) #harcoded 1
+                                # exposure_time_absolute = cc.get_exposure_time_absolute()
+                                # e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                                # print("i... e10===", e10)
+                                # if (e10>=0.0001) and (e10<=0.5):
+                                #     newexposure = int(exposure_time_absolute*2)
+                                # elif (e10>0.5):
+                                #     newexposure = int(maxe)
+                                # elif (e10<=0.0001):
+                                #     newexposure = int(mine+1)
+                                # else:
+                                #     newexposure =  int(mine+1)
+                                # cc.set_exposure_time_absolute( newexposure )
+                                # exposure = newexposure # SENH
 
                             if expo_setdef:
                                 expo_setdef = False
-                                #if "auto_exposure" in capa:
-                                cc.setdef_exposure_time_absolute( ) # changed the order
-                                cc.setdef_auto_exposure() # the order
-                                exposure = exposuredef
-                                print("i... exposure to def: ",exposure)
-
-                            # HIDDEN CAPABILITY
-                            if expovalue>=0 and expovalue<=1:
-                                cc.set_auto_exposure(1) #harcoded 1
-                                #exposure_time_absolute = cc.get_exposure_time_absolute()
-                                #e10 = (exposure_time_absolute-mine)/(maxe-mine)
-                                newexposure = int( (maxe-mine)*expovalue ) + mine
-                                print(f"NEW  HidCap: {newexposure} from {expovalue}")
-                                cc.set_exposure_time_absolute( newexposure )
-                                exposure = newexposure # SENH
-                                expovalue = -999
+                                exposuredef = True
+                                v4lc.mk_table(cc)
+                                exposure = cc.expo_get("expo_get")
+                                cc.autoexpo_on()
+                                print(f"i ... AUTO ;   exposure = {exposure} ")
+                                exposure = 0
+                                senh.setbox(f"expo {exposure:.4f}",  senh.expo)
+                                v4lc.mk_table(cc)
+
+                                # #if "auto_exposure" in capa:
+                                # cc.setdef_exposure_time_absolute( ) # changed the order
+                                # cc.setdef_auto_exposure() # the order
+                                # exposure = exposuredef
+                                # print("i... exposure to def: ",exposure)
+
+                            # # HIDDEN CAPABILITY
+                            # if expovalue>=0 and expovalue<=1:
+                            #     cc.set_auto_exposure(1) #harcoded 1
+                            #     #exposure_time_absolute = cc.get_exposure_time_absolute()
+                            #     #e10 = (exposure_time_absolute-mine)/(maxe-mine)
+                            #     newexposure = int( (maxe-mine)*expovalue ) + mine
+                            #     print(f"NEW  HidCap: {newexposure} from {expovalue}")
+                            #     cc.set_exposure_time_absolute( newexposure )
+                            #     exposure = newexposure # SENH
+                            #     expovalue = -999
 
 
 
-                            if  'exposure' in locals() and exposure != exposuredef:
-                                senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
+                            if not exposuredef: senh.setbox(f"expo {exposure:.4f}",  senh.expo)
+                            #if  'exposure' in locals() and exposure != exposuredef:
+                            #senh.setbox(f"expo {exposure:.4f}",  senh.expo)
                         #-----------exposure in capa
                     # ______________________ section with capa for camera _____________________
 
 
                     #--------------- now apply labels ------i cannot get rid in DETM---
                     #--------- all this will be on all rames histo,detect,direct,delta
                     senh.setbox(" ", senh.TIME)
```

### Comparing `flashcam-1.5.5/flashcam/stream_enhancer.py` & `flashcam-1.5.6/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/uniwrec.py` & `flashcam-1.5.6/flashcam/uniwrec.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 import webbrowser
 
 import math
 
 import requests  # crosson=CROSSON
 
 # ------------------problem with SHIFT
-from pynput.keyboard import Key, Listener
+# from pynput.keyboard import Key, Listener
 
 
 global SHIFT, CTRL
 SHIFT = CTRL = False
 
 global centerX1, centerY1
 global FILE_USERPASS
@@ -169,24 +169,55 @@
 
 
 def remap_keys(key):
     """
     Problem - THIS TABLE WORKS ON  gigajm
         , while zen : 65505
     """
-    # print(f" KEY==/{key}/")
     global CTRL
     CTRL=False
+    print(f" ... remap_keys()  KEY==/{key}/", CTRL)
     if key==1310821: CTRL=True # ctrl e
     if key==1310834: CTRL=True #  ctrl r
     if key==1310817: CTRL=True # ctrl a
     if key==1310823: CTRL=True # ctrl g
     if key==1310841: CTRL=True # ctrl y
     if key==1310836: CTRL=True # ctrl t
+    # zen:
+    if key>=262241 and key<=262266:CTRL=True  # zen
+    print(f" ... remap_keys()  KEY==/{key}/ ", CTRL)
     table = {
+        262241: "a", # zen ctrl
+        262242: "b", # zen ctrl
+        262243: "c", # zen ctrl
+        262244: "d", # zen ctrl
+        262245: "e", # zen ctrl
+        262246: "f", # zen ctrl
+        262247: "g", # zen ctrl
+        262248: "h", # zen ctrl
+        262249: "i", # zen ctrl
+        262250: "j", # zen ctrl
+        262251: "k", # zen ctrl
+        262252: "l", # zen ctrl
+        262253: "m", # zen ctrl
+        262254: "n", # zen ctrl
+        262255: "o", # zen ctrl
+        262256: "p", # zen ctrl
+        262257: "q", # zen ctrl
+        262258: "r", # zen ctrl
+        262259: "s", # zen ctrl
+        262260: "t", # zen ctrl
+        262261: "u", # zen ctrl
+        262262: "v", # zen ctrl
+        262263: "w", # zen ctrl
+        262264: "x", # zen ctrl
+        262265: "y", # zen ctrl
+        262266: "z", # zen ctrl
+
+
         1048673: "a",
         1310817: "a", #ctrl
         1048674: "b",
         1048675: "c",
         1048676: "d",
         1310821: "e", #ctrl
         1048677: "e",
@@ -216,14 +247,42 @@
         1048698: "z",
         1114177: "A",
         1114178: "B",
         1114179: "C",
         1114180: "D",
         1114181: "E",
         1114182: "F",
+
+        65601: "A", # zen
+        65602: "B", #zen
+        65603: "C", # zen
+        65604: "D",
+        65605: "E",
+        65606: "F", # zen
+        65607: "G",
+        65608: "H",
+        65609: "I",
+        65610: "J",
+        65611: "K",
+        65612: "L",
+        65613: "M",
+        65614: "N",
+        65615: "O",
+        65616: "P",
+        65617: "Q",
+        65618: "R",
+        65619: "S",
+        65620: "T",
+        65621: "U",
+        65622: "V",
+        65623: "W",
+        65624: "X",
+        65625: "Y",
+        65626: "Z",
+
         1114183: "G",
         1114184: "H",
         1114185: "I",
         1114186: "J",
         1114187: "K",
         1114188: "L",
         1114189: "M",
@@ -1607,18 +1666,18 @@
                 #if SHIFT: s = "SHIFT"
                 # print(f" {c} x {s} ...      ", end = "       \n")
 
                 #
                 # UBUNTU 22 - ctrl and alt give 227 and 233 resp
                 #
                 if key != -1:
-                    print(f" key== {key}   /{chr(0xFF&key)}/  .. {c} : {s}  >>>.      ")
+                    print(f" *key== {key}   /{chr(0xFF&key)}/  .. {c} : {s}  >>>.      ")
                     key = remap_keys(key) # make compatible with waitKey()
                     print(f" ... --------------------------------------------- remapped {key}")
-                    if SHIFT: key = ord(chr(key).upper())
+                    # if SHIFT: key = ord(chr(key).upper())
 
                 # i will not use the translation,,
                 # key = remap_keys(key) # make compatible with waitKey()
                 # print(f"remapped {key}")
 
                 # print(f"{centerX1} {centerY1}")
                 if (cross is None) and not greencross:
@@ -2357,14 +2416,22 @@
                 ):
                     print("Y PRESSED! - ")
                     local_gamma = local_gamma / 1.4
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
+                    and (key == ord("Y") and not CTRL)
+                ):
+                    print("ctrl - Y PRESSED! -  no action")
+
+
+                if (
+                    (frame is not None)
+                    and (rpi_name != "")
                     and (key == ord("y"))
                     and (CTRL)
                 ):  # and  (key == 1310841): #ctrly
                     print("ctl-y PRESSED! - ")
                     local_gamma = 1
 
                 if (frame is not None) and (rpi_name != "") and (key == ord("p")):
```

### Comparing `flashcam-1.5.5/flashcam/usbcheck.py` & `flashcam-1.5.6/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam/v4lc.py` & `flashcam-1.5.6/flashcam/v4lc.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,98 +23,172 @@
 
 
 import time # tuning has a delay from camera chip.... oscilates...
 
 import random # i need to skip some tune frames
 
 
+import math
+
 class V4L2_Control:
     """docstring for V4L2_CTL"""
 
-    def __init__(self, control_group, name, addr, type, min=-99, max=-99, step=-99, default=-99, value=-99, flags="none", access="local", device="/dev/video0", callback=None):
+    def is_int(self,n):
+        if n is None:return False
+        try:
+            float_n = float(n)
+            int_n = int(float_n)
+        except ValueError:
+            return False
+        else:
+            return float_n == int_n
+
+
+    def is_float(self,n):
+        if n is None:return False
+        try:
+            float_n = float(n)
+        except ValueError:
+            return False
+        else:
+            return True
+
+
+    def __init__(self, control_group, name, addr, type, min=None, max=None, step=None, default=None, value=None, flags="none", access="local", device="/dev/video0", callback=None):
         super(V4L2_Control, self).__init__()
         self.control_group = control_group
 
         self.name = name
         self.addr = addr
         self.type = type
         self.min = min
         self.max = max
         self.step = step
+        self.default = None # was not here...
 
-
+        # RECOVER  DEFAULTS... SOLVE BOUNDS
         # the cheap sonix camera problem
-        if (default>max) or (default<min):
-            self.default = self.min
-        else:
+        if self.is_int(max) and self.is_int(min) and self.is_int(default):
+            if (default>max) or (default<min):
+                print(f"X... camera default parameter /{name}/ is out of min-max")
+                self.default = self.min
+            else:
+                self.default = default
+        elif self.is_int(default):
             self.default = default
 
+
         self.value = value
         self.flags = flags
 
         self.access = access
         self.device = device
         self.callback = callback
 
         self.server = None
 
 
     def setServer(self, server):
         self.server = server
 
-    def get_value(self):
+    def get_value(self, a2 = None):
         return self.value
 
+    def get_value01log(self, a2 = None):
+        res =  (self.value - self.min)/(self.max- self.min)
+        # res = 0-1
+        # val2 = (math.exp(mul*value)-1)/math.exp(1*mul)
+        mul = 5
+        res = math.log( res* math.exp(mul)  +1 )/mul
+
+        return res
+
     def getmin_value(self):
         return self.min
 
     def getmax_value(self):
         return self.max
 
     def setdef_value(self):
         return self.change_value(self.default)
 
     # uuuuuiiiiiiiiii ---works
     def getdef_value(self):
         return self.default
 
+    # hard way with autoexp
+    def set3(self, a2 = None):
+        return self.change_value(3)
+
+    def set1(self, a2 = None):
+        return self.change_value(1)
+
+    def nonpres(self, a1=None, a2=None):
+        print(f" ... ... /{a2}/ control not available")
+        return False# elf.change_value(1)
+
+    def change_value01log(self,value, a2 = None):
+        #print("D... in value01log", value)
+        if self.is_float(value):
+            vv = value
+            if vv<0: vv =0
+            if vv>1: vv= 1
+            mul=5 #2.71 # EMPIRICALLY ============5
+            val2 = (math.exp(mul*vv)-1)/math.exp(1*mul)
+            val2 = val2*(self.max-self.min)+self.min
+            #print(" ... ... translates to ", self.name, round(val2,4))
+            self.change_value(val2)
+
+    def change_value01(self,value, a2 = None):
+        print("D... in value01", value)
+        if self.is_float(value):
+            vv = value
+            if value<0: vv=0
+            if value>1: vv=1
+            val2 = vv*(self.max-self.min)+self.min
+            #print(" ... ... ", self.name, round(val2,4))
+            self.change_value(val2)
+
+
     def change_value(self, value):
         if value> self.max:
             value = self.max
         if value< self.min:
             value = self.min
         try:
             value = int(value)
+            #print(" ... ... ... ... ",value)
         except Exception as e:
             print("change_value: Invalid input -> " + str(e))
             return -1
 
-        if self.step != -99 and value < self.min:
+        if self.step is not None and value < self.min:
             print("change_value: Value too little", value," x ",self.min)
             return -1
 
-        if self.step != -99 and value > self.max:
+        if self.step is not None and value > self.max:
             print("change_value: Value too big", value," x ",self.max)
             return -1
 
-        if self.step != -99 and value % self.step != 0:
+        if self.step is not None and value % self.step != 0:
             print("change_value: Invalid step number (Steps per " + str(self.step) + ")")
             return -1
 
         if self.type == "custom":
             if self.callback is not None:
                 return self.callback(value)
 
         if self.access == "local":
             #print("Executing: " + ' '.join(['v4l2-ctl', '-d', self.device, '--set-ctrl=' + self.name + '=' + str(value)]))
             try:
                 sp.check_output(['v4l2-ctl', '-d', self.device, '--set-ctrl=' + self.name + '=' + str(value)]).decode("utf-8")
                 self.value = value
                 time.sleep(0.1) # i want to see a blink ??
                 return 0
+
             except sp.CalledProcessError as e:
                 print(
                     "Failed to execute command" +
                     ' '.join(['v4l2-ctl', '-d', self.device, '--set-ctrl=' + self.name + '=' + str(value)]) +
                     " -> "+str(e)
                 )
                 print("!... you may need apt install v4l-utils")
@@ -139,102 +213,164 @@
             "step": self.step,
             "default": self.default,
             "value": self.value,
             "flags": self.flags
         }
     def __repr__(self):
         return str(self)
+
     def __str__(self):
         out = "V4L2_Control() -> " + self.name + " " + self.addr + " (" + self.type + ")  :  "
-        out += "min=" + str(self.min) + " " if self.min != -99 else ""
-        out += "max=" + str(self.max) + " " if self.max != -99 else ""
-        out += "step=" + str(self.step) + " " if self.step != -99 else ""
-        out += "default=" + str(self.default) + " " if self.default != -99 else ""
-        out += "value=" + str(self.value) + " " if self.value != -99 else ""
-        out += "flags=" + self.flags + " " if self.flags != "none" else ""
+        # out += "min=" + str(self.min) + " " if self.min != -99 else ""
+        # out += "max=" + str(self.max) + " " if self.max != -99 else ""
+        # out += "step=" + str(self.step) + " " if self.step != -99 else ""
+        # out += "default=" + str(self.default) + " " if self.default != -99 else ""
+        # out += "value=" + str(self.value) + " " if self.value != -99 else ""
+        # out += "flags=" + self.flags + " " if self.flags != "none" else ""
         return out
 
 
 
+
+
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+# ---------------------------------------------------------------------------------
+
+
+
 class V4L2_CTL():
-    """docstring for V4L2_CTL"""
+    """docstring for V4L2_CTL... this is what I call from real_camera"""
+    def is_int(self,n):
+        if n is None:return False
+        try:
+            float_n = float(n)
+            int_n = int(float_n)
+        except ValueError:
+            return False
+        else:
+            return float_n == int_n
+
+    def int_or_none(self, ii ):
+        if ii is None: return None
+        if self.is_int(ii): return int(ii)
+        return None
+
+
 
     def __init__(self, device="/dev/video0"):
         super(V4L2_CTL, self).__init__()
         self.device = device
         self.controls = self._list_controls()
         self.capabilities = []
         self.update_capabilities()
 
+        AE = False
+        EX = False
+        GA = False
+        GM = False
         for control in self.controls:
             #print(control.name)
             setattr(self, "set_" + control.name, control.change_value)
             setattr(self, "getmin_" + control.name, control.getmin_value)
             setattr(self, "getmax_" + control.name, control.getmax_value)
             setattr(self, "setdef_" + control.name, control.setdef_value)
             setattr(self, "get_" + control.name, control.get_value)
             setattr(self, "getdef_" + control.name, control.getdef_value)
 
+
+            # here I want to extract 4 MAIN controls: *************************
+            # autexp - Hard way 3 is always auto
+            if control.name.find("auto")>=0:
+                if control.name.find("exposure")>=0:
+                    setattr(self, "autoexpo_on", control.set3)
+                    setattr(self, "autoexpo_off", control.set1)
+                    AE = True
+
+
+
+            # exposure_absolute -     exposure_time_absolute
+            if control.name.find("absolute")>=0:
+                if control.name.find("exposure")>=0:
+                    setattr(self, "expo", control.change_value01log)
+                    setattr(self, "expo_get", control.get_value01log)
+                    EX = True
+
+            # here I want to extract 4 MAIN controls: *************************
+            # gamma -
+            if control.name.find("gamma")>=0:
+                setattr(self, "gamma", control.change_value01)
+                GM = True
+
+            # here I want to extract 4 MAIN controls: *************************
+            # gain -
+            if control.name.find("gain")>=0:
+                setattr(self, "gain", control.change_value01)
+                GA = True
+
+        #------------------------------------------------------------- end for all contr
+
+        empty = V4L2_Control(
+                    "empty_control",
+                    "w0",
+                    "w1",
+                    "w3",
+                    min=0,
+                    max=1,
+                    step=1,
+                    default=1,
+                    value=1,
+                    flags="none",
+                    device=self.device
+                )
+        # it will not know its name, sinvce the control is not displaye
+        if not AE: setattr(self, "autoexpo_on" , empty.nonpres )
+        if not AE: setattr(self, "autoexpo_off", empty.nonpres )
+        if not EX:
+             setattr(self, "expo"  ,       empty.nonpres )
+             setattr(self, "expo_get"  ,       empty.nonpres )
+        if not GA: setattr(self, "gain"  ,       empty.nonpres )
+        if not GM: setattr(self, "gamma" ,       empty.nonpres )
+
+
+
     def get_capbilities_as_json(self):
         return json.dumps([x.asdict() for x in self.controls])
 
     def get_capbilities(self):
         li = [x.asdict() for x in self.controls]
         ca = []
         for i in li:
             ca.append( i["name"] )
         return ca
 
 
-    # def refresh(self):
-    #     super(V4L2_CTL, self).__init__()
-    #     self.controls = self._list_controls()
-    #     self.capabilities = []
-    #     self.update_capabilities()
-    #     for control in self.controls:
-    #         #print(control.name)
-    #         setattr(self, "set_" + control.name, control.change_value)
-    #         setattr(self, "getmin_" + control.name, control.getmin_value)
-    #         setattr(self, "getmax_" + control.name, control.getmax_value)
-    #         setattr(self, "setdef_" + control.name, control.setdef_value)
-    #         setattr(self, "get_" + control.name, control.get_value)
-    #         setattr(self, "getdef_" + control.name, control.getdef_value)
-
-
     def update_capabilities(self):
         self.capabilities = [x.name for x in self.controls]
 
     def has_capability(self,what):
         return what in self.capabilities
 
     def _list_controls(self):
         controls = []
-        #print("Executing: " + ' '.join(['v4l2-ctl', '-d', self.device, '-l']))
-        #
-        # ---------- i check in bin_flashcam.py-----------------
-        # CMD = ['which','v4l2-ctl']
-        # child = sp.Popen( CMD, stdout = sp.PIPE )
-        # returncode = child.returncode
-        # # print(f"i... v4l2-ctl:", returncode, 'str=',child.communicate()[0] )
-        # if not(returncode is None):
-        #     print("X... install v4l2-ctl:  apt install v4l-utils")
-        #     sys.exit(1)
-
         CMDL = ['v4l2-ctl', '-d', self.device, '-l']
-        #print("i... ", CMDL )
         output = ""
         try:
             output = sp.check_output( CMDL ).decode("utf-8")  # TODO: Check if the output is valid
         except Exception as e:
             print("!... Exception when", CMDL)
             print("!... you may need apt install v4l-utils")
             print("!... you may need apt install v4l-utils")
             print("!... you may need apt install v4l-utils")
 
-    #print(f"i... output = /{output}/")
         if len(output) <2:
             #print("D... no output, returning")
             return []
 
         raw_ctrls = [x for x in output.split('\n') if x]  # TODO: Same
 
         last_control_group = "unknown"
@@ -247,50 +383,54 @@
                 while "  " in raw_ctrl:
                     raw_ctrl = raw_ctrl.replace("  ", " ")
 
                 raw_ctrl_what, raw_ctrl_values = raw_ctrl.split(":")
                 raw_ctrl_what = [x for x in raw_ctrl_what.split(' ') if x and x != ' ']
 
                 values = {
-                    "min": -99,
-                    "max": -99,
-                    "step": -99,
-                    "default": -99,
-                    "value": -99,
+                    "min": None,
+                    "max": None,
+                    "step": None,
+                    "default": None,
+                    "value": None,
                     "flags": "none"
                 }
 
                 for name, value in [name_value_combo.split("=") for name_value_combo in raw_ctrl_values.split(" ") if
                                     "=" in name_value_combo]:
                     values[name] = value
 
                 ctrlr = V4L2_Control(
                     last_control_group,
                     raw_ctrl_what[0],
                     raw_ctrl_what[1],
                     raw_ctrl_what[2].replace("(", "").replace(")", ""),
-                    min=int(values["min"]),
-                    max=int(values["max"]),
-                    step=int(values["step"]),
-                    default=int(values["default"]),
-                    value=int(values["value"]),
+                    min=self.int_or_none(values["min"]),
+                    max=self.int_or_none(values["max"]),
+                    step=self.int_or_none(values["step"]),
+                    default=self.int_or_none(values["default"]),
+                    value=self.int_or_none(values["value"]),
                     flags=values["flags"],
                     device=self.device
                 )
 
                 #print("N..." + str(ctrlr))
                 controls.append(ctrlr)
 
 
         return controls
 
 
 #------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------------------------
+
 
-# print("v... unit 'unitname' loaded, version:",__version__)
 
 
 
 
 def get_gem( cc, capa ):
     # capa = cc.get_capbilities()
 
@@ -487,26 +627,14 @@
 def func(debug = False):
 
     print("D... in unit unitname function func DEBUG may be filtered")
     print("i... in unit unitname function func - info")
     print("X... in unit unitname function func - ALERT")
     return True
 
-# def test_config_save():
-#     config.CONFIG['filename'] = "~/.config/flashcam/cfg.json"
-#     config.show_config()
-#     print( config.get_config_file() )
-#     return config.save_config()
-
-# def test_config_read():
-#     config.CONFIG['filename'] = "~/.config/flashcam/cfg.json"
-#     config.load_config()
-#     config.show_config()
-#     print( config.get_config_file() )
-#     assert config.save_config() == True
 
 def test_func():
     print("i... TESTING function func")
     assert func() == True
 
 
 
@@ -744,15 +872,15 @@
     #     elif h_avg>ghigh:
     #         gg-=2
     #         if "gain" in capa: cc.set_gain(gg)
     #res = cc.set_exposure_time_absolute(ex)
     return gg,ex
 
 
-def main( devid ):
+def old_main( devid ):
     """
     Here it is a test to set exposure and gain by histogram
     """
     #cam = Device.from_id(0)
     #print( cam.info)
     #print()
     #print(cam.video_capture.get_format())
@@ -870,10 +998,90 @@
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
 
     vid.release()
     cv2.destroyAllWindows()
 
 
+def mk_table(cc):
+    # -------------------------------------- NICE TABLE PRINT -----------
+    capa = cc.get_capbilities()
+
+    print("_"*77)
+    for i in capa:
+        if i in ["contrast","saturation","hue","power_line_frequency","sharpness","brightness"]: continue
+        mi = getattr(cc,f"getmin_{i}")()
+        ma = getattr(cc,f"getmax_{i}")()
+        de = getattr(cc,f"getdef_{i}")()
+        va = getattr(cc,f"get_{i}")()
+
+        mi = "    ~" if mi is None else f"{mi:6d}"
+        ma = "    ~" if ma is None else f"{ma:6d}"
+        de = "    ~" if de is None else f"{de:6d}"
+        va = "    ~" if va is None else f"{va:6d}"
+
+        #print( type(mi) )
+        #ma = i.getmax_value()
+        #de = i.getdef_value()
+        print(f"{i:30s} ... {mi:6s}   {va:6s} ({de:6s})    {ma:6s}")
+
+    print("_"*77)
+    # -------------------------------------- NICE TABLE PRINT -----------
+
+
+def main( devid ):
+    """
+    Here it is a test of class
+
+
+    # very stupid camera    ZC0303 Webcam  ... only exposure!
+
+
+    """
+    cc = V4L2_CTL("/dev/video"+str(devid))
+
+    mk_table(cc)
+
+
+    cc.autoexpo_on("autoexpo")
+
+    vid = cv2.VideoCapture(devid)
+    cnt = 0
+    while(True):
+        cnt+=1
+        ret, frame = vid.read()
+
+        if cnt%40 == 0:
+            ra = random.uniform(0,1)
+            print("\n\n", round(ra,3) )
+
+            cc.autoexpo_off( "autoexpo")
+            a = cc.expo_get( 'expo_get')     # 0-1 log
+            print("1I found exposure === ", a)
+            cc.expo( ra ,'expo')     # 0-1 log
+            a = cc.expo_get( 'expo_get')     # 0-1 log
+            print("2I found exposure === ", a)
+            cc.gamma( ra ,'gamma' )     # 0-1 log
+            #print("gain...")
+            cc.gain( ra , 'gain'  )     # 0-1 log
+            mk_table(cc)
+
+        if cnt%200 == 0:
+            cc.autoexpo_on("autoexpo")
+            print("ON")
+
+        if cnt%200 == 100:
+            cc.autoexpo_off("autoexpo")
+            print("OFF")
+
+        cv2.imshow('colorhist',frame)
+        if cv2.waitKey(1) & 0xFF == ord('q'):
+            cc.autoexpo_on("autoexpo")
+            break
+
+    vid.release()
+    cv2.destroyAllWindows()
+
+
 if __name__ == "__main__":
     print("i... in the __main__ of unitname of flashcam")
     Fire(main)
```

### Comparing `flashcam-1.5.5/flashcam/web.py` & `flashcam-1.5.6/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.6/flashcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.5
+Version: 1.5.6
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.5/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.6/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.5/setup.py` & `flashcam-1.5.6/setup.py`

 * *Files identical despite different names*

