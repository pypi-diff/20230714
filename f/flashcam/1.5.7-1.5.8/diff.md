# Comparing `tmp/flashcam-1.5.7.tar.gz` & `tmp/flashcam-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.7.tar", last modified: Fri Jul 14 16:50:44 2023, max compression
+gzip compressed data, was "flashcam-1.5.8.tar", last modified: Fri Jul 14 19:59:28 2023, max compression
```

## Comparing `flashcam-1.5.7.tar` & `flashcam-1.5.8.tar`

### file list

```diff
@@ -1,50 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.876933 flashcam-1.5.7/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:50:44.876933 flashcam-1.5.7/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 16:50:42.000000 flashcam-1.5.7/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.868933 flashcam-1.5.7/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 16:20:01.000000 flashcam-1.5.7/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2021-11-06 15:40:40.000000 flashcam-1.5.7/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2022-01-21 21:23:45.000000 flashcam-1.5.7/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 11:13:16.000000 flashcam-1.5.7/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.872933 flashcam-1.5.7/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2021-10-01 16:29:02.000000 flashcam-1.5.7/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2022-01-28 21:15:30.000000 flashcam-1.5.7/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-14 08:38:46.000000 flashcam-1.5.7/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.876933 flashcam-1.5.7/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    88835 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/c120.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   533468 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/c270_orig.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1697 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/cameras.org
--rw-rw-r--   0 ojr       (1000) ojr       (1000)  1024874 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/cameras.pdf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1975 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/cameras.tex
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-02-14 15:48:37.000000 flashcam-1.5.7/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   115345 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/f100.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    30371 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/f100_orig.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    82499 2022-11-16 13:28:21.000000 flashcam-1.5.7/flashcam/data/vf0770.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-02-14 15:48:37.000000 flashcam-1.5.7/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2022-04-20 12:50:34.000000 flashcam-1.5.7/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-02-06 11:14:13.000000 flashcam-1.5.7/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-03-06 14:36:24.000000 flashcam-1.5.7/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    44585 2023-07-14 16:50:08.000000 flashcam-1.5.7/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 14:10:30.000000 flashcam-1.5.7/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   105949 2023-07-14 16:33:22.000000 flashcam-1.5.7/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 11:13:16.000000 flashcam-1.5.7/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34532 2023-07-14 16:42:47.000000 flashcam-1.5.7/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:26:31.000000 flashcam-1.5.7/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 16:50:44.872933 flashcam-1.5.7/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1025 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 16:50:44.000000 flashcam-1.5.7/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 16:50:44.876933 flashcam-1.5.7/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 07:00:29.000000 flashcam-1.5.7/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.885467 flashcam-1.5.8/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 19:59:28.885467 flashcam-1.5.8/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-14 19:59:26.000000 flashcam-1.5.8/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24892 2023-07-14 19:16:43.000000 flashcam-1.5.8/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-17 20:01:01.000000 flashcam-1.5.8/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-17 20:01:01.000000 flashcam-1.5.8/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 20:01:01.000000 flashcam-1.5.8/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-13 20:56:38.000000 flashcam-1.5.8/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    45656 2023-07-14 19:50:06.000000 flashcam-1.5.8/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-28 18:56:55.000000 flashcam-1.5.8/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   106457 2023-07-14 19:58:39.000000 flashcam-1.5.8/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 20:01:01.000000 flashcam-1.5.8/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    34595 2023-07-14 19:49:12.000000 flashcam-1.5.8/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-13 20:52:49.000000 flashcam-1.5.8/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-14 19:59:28.881467 flashcam-1.5.8/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-14 19:59:28.000000 flashcam-1.5.8/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-14 19:59:28.885467 flashcam-1.5.8/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-17 20:44:28.000000 flashcam-1.5.8/setup.py
```

### Comparing `flashcam-1.5.7/PKG-INFO` & `flashcam-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.7
+Version: 1.5.8
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.7/README.md` & `flashcam-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/bin/flashcam` & `flashcam-1.5.8/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/bin/flashcamg` & `flashcam-1.5.8/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/base_camera2.py` & `flashcam-1.5.8/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/config.py` & `flashcam-1.5.8/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.8/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.8/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.8/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.8/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.8/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/monoskop.jpg` & `flashcam-1.5.8/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/win_rain.jpg` & `flashcam-1.5.8/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/win_skull.jpg` & `flashcam-1.5.8/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/win_storm.jpg` & `flashcam-1.5.8/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/win_winter.jpg` & `flashcam-1.5.8/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/data/windows.jpg` & `flashcam-1.5.8/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/direct.py` & `flashcam-1.5.8/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/izmq_receiver.py` & `flashcam-1.5.8/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/mmapwr.py` & `flashcam-1.5.8/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/real_camera.py` & `flashcam-1.5.8/flashcam/real_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,14 +663,40 @@
                             gammadefX = True
                             gamma = gammadef
                             if "gamma" in capa:
                                 cc.setdef_gamma( )
                                 gamma = gammadef
 
 
+                        if gain_divide:
+                            gain_divide = False
+                            gaindefX = False
+                            gain = cc.gain_get("gain")
+                            gain-=0.1
+                            cc.gain(gain)
+                            gamma = cc.gain_get("gain")
+                            v4lc.mk_table(cc)
+
+
+                        if gain_multiply:
+                            gain_multiply = False
+                            gaindefX = False
+                            gain = cc.gain_get("gain")
+                            gain+=0.1
+                            cc.gain(gain)
+                            gamma = cc.gain_get("gain")
+                            v4lc.mk_table(cc)
+
+                        if gain_setdef:
+                            gain_setdef = False
+                            gaindefX = True
+                            gain = gaindef
+                            if "gain" in capa:
+                                cc.setdef_gain( )
+                                gamma = gammadef
 
                         if "gain" in capa:
                             if gain_divide:
                                 gain_divide = False
                                 if "gain" in capa:
                                     newgain =  int(gain/2)
                                     if newgain<ming: newgain = ming
@@ -703,16 +729,16 @@
                                 #exposure_time_absolute = cc.get_exposure_time_absolute()
                                 #e10 = (exposure_time_absolute-mine)/(maxe-mine)
                                 newgain = (maxg-ming)*gainvalue + ming
                                 cc.set_gain( newgain )
                                 gain = newgain # SENH
                                 gainvalue = -999
 
-                            if  'gain' in locals() and gain != gaindef:
-                                senh.setbox(f"g {(gain-ming)/(maxg-ming):.4f}",  senh.gain)
+                            #if  'gain' in locals() and gain != gaindef:
+                            #    senh.setbox(f"g {(gain-ming)/(maxg-ming):.4f}",  senh.gain)
                         #-----------------gain in capa
 
                         # Sony Chip v2
                         # if  "exposure_time_absolute" in capa:
                         #     if expo_divide:
                         #         expo_divide = False
                         #         #if "exposure_time_absolute" in capa:
@@ -835,15 +861,15 @@
                                 expo_setdef = False
                                 exposuredef = True
                                 v4lc.mk_table(cc)
                                 exposure = cc.expo_get("expo_get")
                                 cc.autoexpo_on()
                                 print(f"i ... AUTO ;   exposure = {exposure} ")
                                 exposure = 0
-                                senh.setbox(f"expo {exposure:.4f}",  senh.expo)
+                                #senh.setbox(f"expo {exposure:.4f}",  senh.expo)
                                 v4lc.mk_table(cc)
 
                                 # #if "auto_exposure" in capa:
                                 # cc.setdef_exposure_time_absolute( ) # changed the order
                                 # cc.setdef_auto_exposure() # the order
                                 # exposure = exposuredef
                                 # print("i... exposure to def: ",exposure)
```

### Comparing `flashcam-1.5.7/flashcam/stream_enhancer.py` & `flashcam-1.5.8/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/uniwrec.py` & `flashcam-1.5.8/flashcam/uniwrec.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,22 +172,17 @@
     """
     Problem - THIS TABLE WORKS ON  gigajm
         , while zen : 65505
     """
     global CTRL
     CTRL=False
     print(f" ... remap_keys()  KEY==/{key}/", CTRL)
-    if key==1310821: CTRL=True # ctrl e
-    if key==1310834: CTRL=True #  ctrl r
-    if key==1310817: CTRL=True # ctrl a
-    if key==1310823: CTRL=True # ctrl g
-    if key==1310841: CTRL=True # ctrl y
-    if key==1310836: CTRL=True # ctrl t
-    # zen:
     if key>=262241 and key<=262266:CTRL=True  # zen
+    if key>=1310817 and key<=1310842:CTRL=True # zaba
+
     print(f" ... remap_keys()  KEY==/{key}/ ", CTRL)
     table = {
         262241: "a", # zen ctrl
         262242: "b", # zen ctrl
         262243: "c", # zen ctrl
         262244: "d", # zen ctrl
         262245: "e", # zen ctrl
@@ -210,38 +205,61 @@
         262262: "v", # zen ctrl
         262263: "w", # zen ctrl
         262264: "x", # zen ctrl
         262265: "y", # zen ctrl
         262266: "z", # zen ctrl
 
 
+        1310817: "a", #ctrl zaba
+        1310818: "b", #ctrl zaba
+        1310819: "c", #ctrl zaba
+        1310820: "d", #ctrl
+        1310821: "e", #ctrl
+        1310822: "f", #ctrl zaba
+        1310823: "g", #ctrl zaba
+        1310824: "h", #ctrl zaba
+        1310825: "i", #ctrl zaba
+        1310826: "j", #ctrl zaba
+        1310827: "k", #ctrl zaba
+        1310828: "l", #ctrl zaba
+        1310829: "m", #ctrl zaba
+        1310830: "n", #ctrl zaba
+        1310831: "o", #ctrl zaba
+        1310832: "p", #ctrl zaba
+        1310833: "q", #ctrl zaba
+        1310834: "r", #ctrl zaba
+        1310835: "s", #ctrl zaba
+        1310836: "t", # ctrl
+        1310837: "u", # ctrl
+        1310838: "v", # ctrl
+        1310839: "w", # ctrl
+        1310840: "x", # ctrl
+        1310841: "y", # ctrl
+        1310842: "z", # ctrl
+
         1048673: "a",
-        1310817: "a", #ctrl
         1048674: "b",
         1048675: "c",
         1048676: "d",
-        1310821: "e", #ctrl
         1048677: "e",
         1048678: "f",
         1048679: "g",
-        1310823: "g", # ctrl g
         1048680: "h",
         1048681: "i",
         1048682: "j",
         1048683: "k",
         1048684: "l",
         1048685: "m",
         1048686: "n",
         1048687: "o",
         1048688: "p",
         1048689: "q",
         1048690: "r",
         1048691: "s",
         1048692: "t",
-        1310836: "t", # ctrl
         1048693: "u",
         1048694: "v",
         1048695: "w",
         1048696: "x",
         1048697: "y",
         1310841: "y", #ctrl
         1048698: "z",
```

### Comparing `flashcam-1.5.7/flashcam/usbcheck.py` & `flashcam-1.5.8/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam/v4lc.py` & `flashcam-1.5.8/flashcam/v4lc.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,15 @@
                 setattr(self, "gamma_get", control.get_value01)
                 GM = True
 
             # here I want to extract 4 MAIN controls: *************************
             # gain -
             if control.name.find("gain")>=0:
                 setattr(self, "gain", control.change_value01)
+                setattr(self, "gain_get", control.get_value01)
                 GA = True
 
         #------------------------------------------------------------- end for all contr
 
         empty = V4L2_Control(
                     "empty_control",
                     "w0",
```

### Comparing `flashcam-1.5.7/flashcam/web.py` & `flashcam-1.5.8/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.7/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.8/flashcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.7
+Version: 1.5.8
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `flashcam-1.5.7/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.8/flashcam.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,22 +22,14 @@
 flashcam.egg-info/dependency_links.txt
 flashcam.egg-info/requires.txt
 flashcam.egg-info/top_level.txt
 flashcam/data/BEAM_OFF.jpg
 flashcam/data/BEAM_ON_.jpg
 flashcam/data/DET_NRDY.jpg
 flashcam/data/DET_RDY_.jpg
-flashcam/data/c120.jpg
-flashcam/data/c270_orig.png
-flashcam/data/cameras.org
-flashcam/data/cameras.pdf
-flashcam/data/cameras.tex
 flashcam/data/digital-7.mono.ttf
-flashcam/data/f100.jpg
-flashcam/data/f100_orig.jpg
 flashcam/data/monoskop.jpg
-flashcam/data/vf0770.jpg
 flashcam/data/win_rain.jpg
 flashcam/data/win_skull.jpg
 flashcam/data/win_storm.jpg
 flashcam/data/win_winter.jpg
 flashcam/data/windows.jpg
```

### Comparing `flashcam-1.5.7/setup.py` & `flashcam-1.5.8/setup.py`

 * *Files identical despite different names*

