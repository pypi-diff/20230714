# Comparing `tmp/flashcam-1.5.6.tar.gz` & `tmp/flashcam-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.6.tar", last modified: Fri Jul 14 16:20:04 2023, max compression
+gzip compressed data, was "flashcam-1.5.7.tar", last modified: Fri Jul 14 16:50:44 2023, max compression
```

## Comparing `flashcam-1.5.6.tar` & `flashcam-1.5.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.072691 flashcam-1.5.6/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:20:04.072691 flashcam-1.5.6/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 16:19:59.000000 flashcam-1.5.6/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.068691 flashcam-1.5.6/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 16:20:01.000000 flashcam-1.5.6/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.5.6/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.5.6/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.5.6/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.068691 flashcam-1.5.6/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.5.6/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.5.6/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-14 08:38:46.000000 flashcam-1.5.6/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.072691 flashcam-1.5.6/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/c120.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/c270_orig.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/cameras.org
--rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/cameras.pdf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/cameras.tex
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.5.6/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/f100.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/f100_orig.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.5.6/flashcam/data/vf0770.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.5.6/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.5.6/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.5.6/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.5.6/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    43323 2023-07-14 16:16:55.000000 flashcam-1.5.6/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 14:10:30.000000 flashcam-1.5.6/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   104477 2023-07-14 09:57:07.000000 flashcam-1.5.6/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.5.6/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34128 2023-07-14 16:11:55.000000 flashcam-1.5.6/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 16:20:03.000000 flashcam-1.5.6/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:26:31.000000 flashcam-1.5.6/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:20:04.068691 flashcam-1.5.6/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1025 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 16:20:04.000000 flashcam-1.5.6/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 16:20:04.072691 flashcam-1.5.6/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 07:00:29.000000 flashcam-1.5.6/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.876933 flashcam-1.5.7/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:50:44.876933 flashcam-1.5.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 16:50:42.000000 flashcam-1.5.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.868933 flashcam-1.5.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 16:20:01.000000 flashcam-1.5.7/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.5.7/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.5.7/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.5.7/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.872933 flashcam-1.5.7/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.5.7/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.5.7/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-14 08:38:46.000000 flashcam-1.5.7/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.876933 flashcam-1.5.7/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/c120.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/c270_orig.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/cameras.org
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/cameras.pdf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/cameras.tex
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.5.7/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/f100.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/f100_orig.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/vf0770.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.5.7/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.5.7/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.5.7/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.5.7/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    44585 2023-07-14 16:50:08.000000 flashcam-1.5.7/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   105949 2023-07-14 16:33:22.000000 flashcam-1.5.7/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.5.7/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34532 2023-07-14 16:42:47.000000 flashcam-1.5.7/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:26:31.000000 flashcam-1.5.7/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.872933 flashcam-1.5.7/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1025 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 16:50:44.876933 flashcam-1.5.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 07:00:29.000000 flashcam-1.5.7/setup.py
```

### Comparing `flashcam-1.5.6/PKG-INFO` & `flashcam-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.6
+Version: 1.5.7
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.6/README.md` & `flashcam-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/bin/flashcam` & `flashcam-1.5.7/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/bin/flashcamg` & `flashcam-1.5.7/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/base_camera2.py` & `flashcam-1.5.7/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/config.py` & `flashcam-1.5.7/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.7/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.7/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.7/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.7/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/c120.jpg` & `flashcam-1.5.7/flashcam/data/c120.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/c270_orig.png` & `flashcam-1.5.7/flashcam/data/c270_orig.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/cameras.org` & `flashcam-1.5.7/flashcam/data/cameras.org`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/cameras.pdf` & `flashcam-1.5.7/flashcam/data/cameras.pdf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/cameras.tex` & `flashcam-1.5.7/flashcam/data/cameras.tex`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.7/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/f100.jpg` & `flashcam-1.5.7/flashcam/data/f100.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/f100_orig.jpg` & `flashcam-1.5.7/flashcam/data/f100_orig.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/monoskop.jpg` & `flashcam-1.5.7/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/vf0770.jpg` & `flashcam-1.5.7/flashcam/data/vf0770.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/win_rain.jpg` & `flashcam-1.5.7/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/win_skull.jpg` & `flashcam-1.5.7/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/win_storm.jpg` & `flashcam-1.5.7/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/win_winter.jpg` & `flashcam-1.5.7/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/data/windows.jpg` & `flashcam-1.5.7/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/direct.py` & `flashcam-1.5.7/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/izmq_receiver.py` & `flashcam-1.5.7/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/mmapwr.py` & `flashcam-1.5.7/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/real_camera.py` & `flashcam-1.5.7/flashcam/real_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,15 +393,34 @@
                         config.CONFIG['expo'],
                         config.CONFIG['mmaga'])
 
 
             #--- INITIATION...... collecting???
 
             exposuredef = True
+            gammadefX = True
+            gaindefX = True
+
             cc.autoexpo_on("autoexpo")
+            if "gain" in capa:
+                gain = cc.get_gain()
+                gaindef = cc.getdef_gain()
+                if gaindef == gain:
+                    gaindefX = True
+                else:
+                    gaindefX = False
+
+            if "gamma" in capa:
+                gamma = cc.get_gamma()
+                gammadef = cc.getdef_gamma()
+                if gammadef == gamma:
+                    gammadefX = True
+                else:
+                    gammadefX = False
+
             aea,aex,aga,agm = get_gem(cc, capa)
             if aex!=None: ex,exd,mine,maxe,ex10 = aex
             if agm!=None: gm,gmd,minm,maxm,gm10 = agm
             if aga!=None: ga,gad,ming,maxg,ga10 = aga
 
             # very stupid camera    ZC0303 Webcam
             if "exposure" in capa:
@@ -417,21 +436,14 @@
             #     expo_autodef = cc.getdef_auto_exposure()
             #     print(f"i... EXPOAUTO (TOP) == {expo_auto} vs def={expo_autodef}; ")
 
             # if "exposure_time_absolute" in capa:
             #     exposure_time_absolute = cc.get_exposure_time_absolute()
             #     exposuredef = cc.getdef_exposure_time_absolute() # i think all cams
 
-            if "gain" in capa:
-                gain = cc.get_gain()
-                gaindef = cc.getdef_gain()
-
-            if "gamma" in capa:
-                gamma = cc.get_gamma()
-                gammadef = cc.getdef_gamma()
 
 
             nfrm = 0
             if config.CONFIG["product"]:
                 wname = "none "
             else:
                 wname = config.CONFIG["product"]
@@ -539,29 +551,29 @@
                         if is_int(value):
                             print("i... ",value, 'can be safely converted to an integer.')
                             value = int(float(value)) # 1.0 => int crashes
                         elif is_float(value):
                             print("i... ",value, 'is a float with non-zero digit(s) in the fractional-part.')
                             value = float(value)
                         elif is_bool(value):
-                            print("i... ",value, 'is true or false.')
+                            #print("i... ",value, 'is true or false.')
                             if value=="True":
                                 value = True
                             else:
                                 value = False
                         else:
                             print(f"i... /{value}/ is string. It remains a string, without quotes though.")
                             value = str(value) # i dont care anyway
                             value = value.strip('"').strip("'")
 
                         try:
                             # eval makes float float and int int
                             #print("o... evaluating")
                             globals()[expression] = value  #was  eval(value)
-                            print("i... evaluated")
+                            print("i...                                       expression evaluated")
                         except:
                             print("X... globals expression FAIL",expression,value)
 
                         # I need a crosscheck here on terminal screen
                         if expression=="pausedMOTION":
                             if value is True:
                                 print("===================== DM RUNNING ====================")
@@ -616,29 +628,44 @@
                     # print("i.... timelaps", timelaps)
 
                     #print("i... GAMMAS ", gamma, gammadef )
 
                     if ccoi1 == "camera":
                         if gamma_divide:
                             gamma_divide = False
-                            if "gamma" in capa:
-                                newgamma =  int(gamma/2)
-                                cc.set_gamma( newgamma )
-                                gamma = newgamma
+                            gammadefX = False
+                            gamma = cc.gamma_get("gamma")
+                            gamma-=0.1
+                            cc.gamma(gamma  )
+                            gamma = cc.gamma_get("gamma")
+                            v4lc.mk_table(cc)
+                            #cc.gamma()
+                            #if "gamma" in capa:
+                            #    newgamma =  int(gamma/2)
+                            #    cc.set_gamma( newgamma )
+                            #    gamma = newgamma
                         if gamma_multiply:
                             gamma_multiply = False
-                            if "gamma" in capa:
-                                if gamma!=0:
-                                    newgamma =  int(gamma*2)
-                                else:
-                                    newgamma =  int(1)
-                                cc.set_gamma( newgamma )
-                                gamma = newgamma
+                            gammadefX = False
+                            #if "gamma" in capa:
+                            gamma = cc.gamma_get("gamma")
+                            gamma+=0.1
+                            cc.gamma( gamma )
+                            gamma = cc.gamma_get("gamma")
+                            v4lc.mk_table(cc)
+                            # if gamma!=0:
+                            #     newgamma =  int(gamma*2)
+                            # else:
+                            #     newgamma =  int(1)
+                            # cc.set_gamma( newgamma )
+                            # gamma = newgamma
                         if gamma_setdef:
                             gamma_setdef = False
+                            gammadefX = True
+                            gamma = gammadef
                             if "gamma" in capa:
                                 cc.setdef_gamma( )
                                 gamma = gammadef
 
 
 
                         if "gain" in capa:
@@ -830,15 +857,17 @@
                             #     print(f"NEW  HidCap: {newexposure} from {expovalue}")
                             #     cc.set_exposure_time_absolute( newexposure )
                             #     exposure = newexposure # SENH
                             #     expovalue = -999
 
 
 
-                            if not exposuredef: senh.setbox(f"expo {exposure:.4f}",  senh.expo)
+                            if not exposuredef: senh.setbox(f"exp {exposure:.3f}",  senh.expo)
+                            if not gaindefX: senh.setbox(f"gai {gain:.3f}",  senh.gain)
+                            if not gammadefX: senh.setbox(f"gam {gamma:.3f}",  senh.gamma)
                             #if  'exposure' in locals() and exposure != exposuredef:
                             #senh.setbox(f"expo {exposure:.4f}",  senh.expo)
                         #-----------exposure in capa
                     # ______________________ section with capa for camera _____________________
 
 
                     #--------------- now apply labels ------i cannot get rid in DETM---
```

### Comparing `flashcam-1.5.6/flashcam/stream_enhancer.py` & `flashcam-1.5.7/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/uniwrec.py` & `flashcam-1.5.7/flashcam/uniwrec.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,16 @@
  n/N ... inc/decrease distance
  f/F ... inc/dec Field Of View (-v FOV,dist)
 
  v/V* ... green cross ON/OFF
  b/f* ... substract BG, mix FG
  B/F* ... SAVE BG/ SAVE FG
 
- eg* ...  expo/gain (+ shift or ctl)
- y   ...  gamma (local) (+shift or ctl)
+ egy* ...  expo/gain/gm (+ shift or ctl)
+ d   ...  gamma (local) (+shift or ctl)
  o/O ... autotune expo / break tuning
  i/I* ... accumulate images
 
  w ... open web browser
  q ... quit     ctl-t ... some test
        * with remote flashcam server """
 
@@ -2370,74 +2370,98 @@
                     and (CTRL)
                 ):  # (key == 1310821 ): # ctrle
                     print("ctl-e PRESSED! - ")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"expo": "EXPO"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
+
+                # --------------------------gain ----------------------
+
                 if (
                     (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("g") and not CTRL)
                 ):
-                    print("g PRESSED! - ")
+                    print("g PRESSED! -  gain up")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"gain2": "GAIN2"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
                 if (frame is not None) and (rpi_name != "") and (key == ord("G")):
-                    print("G PRESSED! - ")
+                    print("G PRESSED! - gain down")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"gain05": "GAIN05"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("g"))
                     and (CTRL)
                 ):  # and  (key == 1310823): # ctrlg
-                    print("ctl-g PRESSED! - ")
+                    print("ctl-g PRESSED! -  gain reset")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"gain": "GAIN"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
-                if (
-                    (frame is not None)
-                    and (rpi_name != "")
-                    and (key == ord("y") and not CTRL)
-                ):
-                    print("y PRESSED! - ")
-                    local_gamma = local_gamma * 1.4
 
-                if (
-                    (frame is not None)
-                    and (rpi_name != "")
-                    and (key == ord("Y") and not CTRL)
-                ):
-                    print("Y PRESSED! - ")
-                    local_gamma = local_gamma / 1.4
+                # --------------------------gamma ----------------------
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
-                    and (key == ord("Y") and not CTRL)
+                    and (key == ord("y") and not CTRL)
                 ):
-                    print("ctrl - Y PRESSED! -  no action")
+                    print("y PRESSED! -  gamm up")
+                    post_addr = videodev.replace("/video", "/cross")
+                    post_data = {"gamma2": "GAMMA2"}
+                    post_response = requests.post(url=post_addr, data=post_data)
 
+                if (frame is not None) and (rpi_name != "") and (key == ord("Y")):
+                    print("Y PRESSED! - gain down")
+                    post_addr = videodev.replace("/video", "/cross")
+                    post_data = {"gamma05": "GAMMA05"}
+                    post_response = requests.post(url=post_addr, data=post_data)
 
                 if (
                     (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("y"))
                     and (CTRL)
-                ):  # and  (key == 1310841): #ctrly
-                    print("ctl-y PRESSED! - ")
+                ):  # and  (key == 1310823): # ctrlg
+                    print("ctl-y PRESSED! -  gamma reset")
+                    post_addr = videodev.replace("/video", "/cross")
+                    post_data = {"gamma": "GAMMA"}
+                    post_response = requests.post(url=post_addr, data=post_data)
+
+                # ------------------------------local gamma --------------------------
+                if ( (frame is not None)   and (rpi_name != "")
+                    and (key == ord("d") and not CTRL)               ):
+                    print("d PRESSED! - local gamma+")
+                    local_gamma = local_gamma * 1.4
+
+                if (   (frame is not None)  and (rpi_name != "")
+                    and (key == ord("D") and not CTRL)   ):
+                    print("D PRESSED! - local gamma -")
+                    local_gamma = local_gamma / 1.4
+
+                if ( (frame is not None) and (rpi_name != "")
+                    and (key == ord("D") and not CTRL)        ):
+                    print("ctrl - Y PRESSED! -  no action")
+
+                if (     (frame is not None)  and (rpi_name != "")   and (key == ord("d"))
+                    and (CTRL)      ):  # and  (key == 1310841): #ctrly
+                    print("ctl-d PRESSED! - eset local gamma")
                     local_gamma = 1
 
+
+
+                # -------------------------------------------------------- p fixed live ----------pause
+
                 if (frame is not None) and (rpi_name != "") and (key == ord("p")):
                     print("p PRESSED! - ")
                     post_addr = videodev.replace("/video", "/cross")
                     post_data = {"fixed": "FIXED"}
                     post_response = requests.post(url=post_addr, data=post_data)
 
                 if (frame is not None) and (rpi_name != "") and (key == ord("P")):
```

### Comparing `flashcam-1.5.6/flashcam/usbcheck.py` & `flashcam-1.5.7/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam/v4lc.py` & `flashcam-1.5.7/flashcam/v4lc.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,21 +89,28 @@
 
     def setServer(self, server):
         self.server = server
 
     def get_value(self, a2 = None):
         return self.value
 
+    def get_value01(self, a2 = None):
+        res =  (self.value - self.min)/(self.max- self.min)
+        # res = 0-1
+        # val2 = (math.exp(mul*value)-1)/math.exp(1*mul)
+        #mul = 5
+        #res = math.log( res* math.exp(mul)  +1 )/mul
+        return res
+
     def get_value01log(self, a2 = None):
         res =  (self.value - self.min)/(self.max- self.min)
         # res = 0-1
         # val2 = (math.exp(mul*value)-1)/math.exp(1*mul)
         mul = 5
         res = math.log( res* math.exp(mul)  +1 )/mul
-
         return res
 
     def getmin_value(self):
         return self.min
 
     def getmax_value(self):
         return self.max
@@ -300,14 +307,15 @@
                     setattr(self, "expo_get", control.get_value01log)
                     EX = True
 
             # here I want to extract 4 MAIN controls: *************************
             # gamma -
             if control.name.find("gamma")>=0:
                 setattr(self, "gamma", control.change_value01)
+                setattr(self, "gamma_get", control.get_value01)
                 GM = True
 
             # here I want to extract 4 MAIN controls: *************************
             # gain -
             if control.name.find("gain")>=0:
                 setattr(self, "gain", control.change_value01)
                 GA = True
@@ -330,15 +338,17 @@
         # it will not know its name, sinvce the control is not displaye
         if not AE: setattr(self, "autoexpo_on" , empty.nonpres )
         if not AE: setattr(self, "autoexpo_off", empty.nonpres )
         if not EX:
              setattr(self, "expo"  ,       empty.nonpres )
              setattr(self, "expo_get"  ,       empty.nonpres )
         if not GA: setattr(self, "gain"  ,       empty.nonpres )
-        if not GM: setattr(self, "gamma" ,       empty.nonpres )
+        if not GM:
+            setattr(self, "gamma" ,       empty.nonpres )
+            setattr(self, "gamma_get"  ,       empty.nonpres )
 
 
 
     def get_capbilities_as_json(self):
         return json.dumps([x.asdict() for x in self.controls])
 
     def get_capbilities(self):
```

### Comparing `flashcam-1.5.6/flashcam/web.py` & `flashcam-1.5.7/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.7/flashcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.6
+Version: 1.5.7
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.6/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.7/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.6/setup.py` & `flashcam-1.5.7/setup.py`

 * *Files identical despite different names*

