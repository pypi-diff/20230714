# Comparing `tmp/flashcam-1.5.4.tar.gz` & `tmp/flashcam-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.4.tar", last modified: Thu Jul 13 20:59:03 2023, max compression
+gzip compressed data, was "flashcam-1.5.5.tar", last modified: Fri Jul 14 08:39:01 2023, max compression
```

## Comparing `flashcam-1.5.4.tar` & `flashcam-1.5.5.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-13 20:59:03.689931 flashcam-1.5.4/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-13 20:58:58.000000 flashcam-1.5.4/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.685931 flashcam-1.5.4/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24865 2023-07-13 20:59:00.000000 flashcam-1.5.4/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-17 20:01:01.000000 flashcam-1.5.4/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-17 20:01:01.000000 flashcam-1.5.4/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 20:01:01.000000 flashcam-1.5.4/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-13 20:56:38.000000 flashcam-1.5.4/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40421 2023-07-11 20:11:58.000000 flashcam-1.5.4/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   102717 2023-07-13 20:54:51.000000 flashcam-1.5.4/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27692 2023-07-11 20:09:40.000000 flashcam-1.5.4/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-13 20:52:49.000000 flashcam-1.5.4/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-13 20:59:03.689931 flashcam-1.5.4/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-17 20:44:28.000000 flashcam-1.5.4/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.513224 flashcam-1.5.5/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 08:39:01.513224 flashcam-1.5.5/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 08:38:59.000000 flashcam-1.5.5/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.509224 flashcam-1.5.5/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24865 2023-07-14 08:38:46.000000 flashcam-1.5.5/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.5.5/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.5.5/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.5.5/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.509224 flashcam-1.5.5/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.5.5/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.5.5/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.513224 flashcam-1.5.5/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/c120.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/c270_orig.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/cameras.org
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/cameras.pdf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/cameras.tex
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.5.5/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/f100.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/f100_orig.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.5.5/flashcam/data/vf0770.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.5.5/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.5.5/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.5.5/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.5.5/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40604 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 14:10:30.000000 flashcam-1.5.5/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   102717 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.5.5/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27704 2023-07-14 08:38:46.000000 flashcam-1.5.5/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:26:31.000000 flashcam-1.5.5/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 08:39:01.509224 flashcam-1.5.5/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1025 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 08:39:01.000000 flashcam-1.5.5/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 08:39:01.513224 flashcam-1.5.5/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 07:00:29.000000 flashcam-1.5.5/setup.py
```

### Comparing `flashcam-1.5.4/PKG-INFO` & `flashcam-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.4
+Version: 1.5.5
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.4/README.md` & `flashcam-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/bin/flashcam` & `flashcam-1.5.5/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/bin/flashcamg` & `flashcam-1.5.5/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/base_camera2.py` & `flashcam-1.5.5/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/config.py` & `flashcam-1.5.5/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.5/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.5/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.5/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.5/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.5/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/monoskop.jpg` & `flashcam-1.5.5/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/win_rain.jpg` & `flashcam-1.5.5/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/win_skull.jpg` & `flashcam-1.5.5/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/win_storm.jpg` & `flashcam-1.5.5/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/win_winter.jpg` & `flashcam-1.5.5/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/data/windows.jpg` & `flashcam-1.5.5/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/direct.py` & `flashcam-1.5.5/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/izmq_receiver.py` & `flashcam-1.5.5/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/mmapwr.py` & `flashcam-1.5.5/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/real_camera.py` & `flashcam-1.5.5/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -708,26 +708,28 @@
                                     newexposure =  int(mine+1)
                                 cc.set_exposure_time_absolute( newexposure )
                                 exposure = newexposure # SENH
 
                             if expo_setdef:
                                 expo_setdef = False
                                 #if "auto_exposure" in capa:
-                                cc.setdef_auto_exposure()
+                                # cc.setdef_auto_exposure() # Sony v2 prob
+                                # HARDCODE-frm ubu22
+                                cc.set_auto_exposure(3)
                                 cc.setdef_exposure_time_absolute( )
-                                exposure = exposuredef
+                                exposure = exposuredef #
                                 print("i... exposure to def: ",exposure)
 
                             # HIDDEN CAPABILITY ??? Sony Chipv2
                             if expovalue>=0 and expovalue<=1:
                                 cc.set_auto_exposure(1) #harcoded 1
                                 #exposure_time_absolute = cc.get_exposure_time_absolute()
                                 #e10 = (exposure_time_absolute-mine)/(maxe-mine)
                                 newexposure = int( (maxe-mine)*expovalue ) + mine
-                                print(f"NEW: {newexposure} from {expovalue}")
+                                print(f"NEW: expoHidCapSony {newexposure} from {expovalue}")
                                 cc.set_exposure_time_absolute( newexposure )
                                 exposure = newexposure # SENH
                                 expovalue = -999
 
                             if  'exposure' in locals() and exposure != exposuredef:
                                 senh.setbox(f"expo {(exposure-mine)/(maxe-mine):.4f}",  senh.expo)
 
@@ -760,26 +762,26 @@
                                     newexposure =  int(mine+1)
                                 cc.set_exposure_time_absolute( newexposure )
                                 exposure = newexposure # SENH
 
                             if expo_setdef:
                                 expo_setdef = False
                                 #if "auto_exposure" in capa:
-                                cc.setdef_auto_exposure()
-                                cc.setdef_exposure_time_absolute( )
+                                cc.setdef_exposure_time_absolute( ) # changed the order
+                                cc.setdef_auto_exposure() # the order
                                 exposure = exposuredef
                                 print("i... exposure to def: ",exposure)
 
                             # HIDDEN CAPABILITY
                             if expovalue>=0 and expovalue<=1:
                                 cc.set_auto_exposure(1) #harcoded 1
                                 #exposure_time_absolute = cc.get_exposure_time_absolute()
                                 #e10 = (exposure_time_absolute-mine)/(maxe-mine)
                                 newexposure = int( (maxe-mine)*expovalue ) + mine
-                                print(f"NEW: {newexposure} from {expovalue}")
+                                print(f"NEW  HidCap: {newexposure} from {expovalue}")
                                 cc.set_exposure_time_absolute( newexposure )
                                 exposure = newexposure # SENH
                                 expovalue = -999
 
 
 
                             if  'exposure' in locals() and exposure != exposuredef:
```

### Comparing `flashcam-1.5.4/flashcam/stream_enhancer.py` & `flashcam-1.5.5/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/uniwrec.py` & `flashcam-1.5.5/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/usbcheck.py` & `flashcam-1.5.5/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam/v4lc.py` & `flashcam-1.5.5/flashcam/v4lc.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
     initme = True
     gain = 100
     capa = cc.get_capbilities()
 
     if "auto_exposure" in capa:
         print("D... AUTO EXPOSURE OFF")
         cc.setdef_auto_exposure() # doesnt do default 3
-        print("ex def",cc.get_auto_exposure())
+        print("i... v4l... ex def",cc.get_auto_exposure())
         cc.set_auto_exposure(1)
 
     #print("ex 3",cc.get_auto_exposure())
     if "gain" in capa:
         cc.setdef_gain()
         gg = cc.get_gain()
         print("defgain ",gg)
```

### Comparing `flashcam-1.5.4/flashcam/web.py` & `flashcam-1.5.5/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.4/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.5/flashcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.4
+Version: 1.5.5
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.4/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.5/flashcam.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 flashcam.egg-info/dependency_links.txt
 flashcam.egg-info/requires.txt
 flashcam.egg-info/top_level.txt
 flashcam/data/BEAM_OFF.jpg
 flashcam/data/BEAM_ON_.jpg
 flashcam/data/DET_NRDY.jpg
 flashcam/data/DET_RDY_.jpg
+flashcam/data/c120.jpg
+flashcam/data/c270_orig.png
+flashcam/data/cameras.org
+flashcam/data/cameras.pdf
+flashcam/data/cameras.tex
 flashcam/data/digital-7.mono.ttf
+flashcam/data/f100.jpg
+flashcam/data/f100_orig.jpg
 flashcam/data/monoskop.jpg
+flashcam/data/vf0770.jpg
 flashcam/data/win_rain.jpg
 flashcam/data/win_skull.jpg
 flashcam/data/win_storm.jpg
 flashcam/data/win_winter.jpg
 flashcam/data/windows.jpg
```

### Comparing `flashcam-1.5.4/setup.py` & `flashcam-1.5.5/setup.py`

 * *Files identical despite different names*

