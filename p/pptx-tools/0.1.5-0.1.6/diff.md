# Comparing `tmp/pptx-tools-0.1.5.tar.gz` & `tmp/pptx-tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx-tools-0.1.5.tar", last modified: Thu Jul 13 04:47:10 2023, max compression
+gzip compressed data, was "pptx-tools-0.1.6.tar", last modified: Fri Jul 14 07:08:32 2023, max compression
```

## Comparing `pptx-tools-0.1.5.tar` & `pptx-tools-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 04:47:10.209297 pptx-tools-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/apps/slide_add_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/audio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/data/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/data/hello.pptx
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/data/transparent.png
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/slide_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/slide_transition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools/tts/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/azure_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/google_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/tts/google_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/pptx_tools/video_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/pptx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      846 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-13 04:47:10.000000 pptx-tools-0.1.5/pptx_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-13 04:47:10.209297 pptx-tools-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:47:10.205297 pptx-tools-0.1.5/tests/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/tests/pptx_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-13 04:46:56.000000 pptx-tools-0.1.5/tests/pptx_tools/test_slide_add_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.294606 pptx-tools-0.1.6/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/pptx_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2216 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/apps/slide_add_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      650 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/apps/slide_delete_notes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/audio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/pptx_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/data/hello.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/data/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/slide_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/slide_transition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/pptx_tools/tts/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/azure_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/azure_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/google_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/tts/google_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4956 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/pptx_tools/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.294606 pptx-tools-0.1.6/pptx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      884 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-14 07:08:32.000000 pptx-tools-0.1.6/pptx_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2472 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:32.298606 pptx-tools-0.1.6/tests/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/tests/pptx_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-14 07:08:24.000000 pptx-tools-0.1.6/tests/pptx_tools/test_slide_add_voice.py
```

### Comparing `pptx-tools-0.1.5/LICENSE` & `pptx-tools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/PKG-INFO` & `pptx-tools-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -51,7 +51,13 @@
 You can change the synthesized voice by specifying the `--voice-name` as shown below.
 
 ```
 slide-add-voice pptx_tools/data/hello.pptx --voice-name en-US-Wavenet-C
 ```
 
 In addition, you can listen to the voice samples available for use with Google Text-to-Speech at the following URL: https://cloud.google.com/text-to-speech/docs/voices
+
+## Q & A
+
+Q: What happens to the slide transition time when both a video file and a synthesized voice are present on the slide?
+
+A: The transition time for the slide will be based on whichever is longer between the duration of the synthesized voice and the duration of the video.
```

### Comparing `pptx-tools-0.1.5/README.md` & `pptx-tools-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,7 +29,13 @@
 You can change the synthesized voice by specifying the `--voice-name` as shown below.
 
 ```
 slide-add-voice pptx_tools/data/hello.pptx --voice-name en-US-Wavenet-C
 ```
 
 In addition, you can listen to the voice samples available for use with Google Text-to-Speech at the following URL: https://cloud.google.com/text-to-speech/docs/voices
+
+## Q & A
+
+Q: What happens to the slide transition time when both a video file and a synthesized voice are present on the slide?
+
+A: The transition time for the slide will be based on whichever is longer between the duration of the synthesized voice and the duration of the video.
```

### Comparing `pptx-tools-0.1.5/pptx_tools/apps/slide_add_voice.py` & `pptx-tools-0.1.6/pptx_tools/apps/slide_add_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/data/hello.pptx` & `pptx-tools-0.1.6/pptx_tools/data/hello.pptx`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/slide_info.py` & `pptx-tools-0.1.6/pptx_tools/slide_info.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/slide_transition.py` & `pptx-tools-0.1.6/pptx_tools/slide_transition.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/tts/azure_tts.py` & `pptx-tools-0.1.6/pptx_tools/tts/azure_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/tts/azure_tts_voice.py` & `pptx-tools-0.1.6/pptx_tools/tts/azure_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/tts/google_tts.py` & `pptx-tools-0.1.6/pptx_tools/tts/google_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/tts/google_tts_voice.py` & `pptx-tools-0.1.6/pptx_tools/tts/google_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools/utils.py` & `pptx-tools-0.1.6/pptx_tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,28 @@
         media.element.getparent().getparent().getparent(),
         './/p:timing//p:video//p:spTgt[@spid="%s"]' % el_id,
     )[0]
     cond = xpath(el_cnt.getparent().getparent(), './/p:cond')[0]
     cond.set('delay', '0')
 
 
+def delete_slide_notes_text(slide_path, logger=None):
+    if logger is None:
+        logger = base_logger
+    coloredlogs.install(level='DEBUG', logger=logger)
+
+    presentation = Presentation(slide_path)
+
+    for page, slide in tqdm(enumerate(presentation.slides, start=1),
+                            total=len(presentation.slides)):
+        if slide.has_notes_slide and slide.notes_slide.notes_text_frame.text:
+            slide.notes_slide.notes_text_frame.text = ''
+    return presentation
+
+
 def add_synthesize_audio(slide_path, outdir, logger=None,
                          voice_name=None,
                          tts='google',
                          slide_duration_offset=1.0):
     """Synthesizes speech from the pptx."""
 
     if logger is None:
```

### Comparing `pptx-tools-0.1.5/pptx_tools/video_utils.py` & `pptx-tools-0.1.6/pptx_tools/video_utils.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.5/pptx_tools.egg-info/PKG-INFO` & `pptx-tools-0.1.6/pptx_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -51,7 +51,13 @@
 You can change the synthesized voice by specifying the `--voice-name` as shown below.
 
 ```
 slide-add-voice pptx_tools/data/hello.pptx --voice-name en-US-Wavenet-C
 ```
 
 In addition, you can listen to the voice samples available for use with Google Text-to-Speech at the following URL: https://cloud.google.com/text-to-speech/docs/voices
+
+## Q & A
+
+Q: What happens to the slide transition time when both a video file and a synthesized voice are present on the slide?
+
+A: The transition time for the slide will be based on whichever is longer between the duration of the synthesized voice and the duration of the video.
```

### Comparing `pptx-tools-0.1.5/pptx_tools.egg-info/SOURCES.txt` & `pptx-tools-0.1.6/pptx_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pptx_tools.egg-info/dependency_links.txt
 pptx_tools.egg-info/entry_points.txt
 pptx_tools.egg-info/not-zip-safe
 pptx_tools.egg-info/requires.txt
 pptx_tools.egg-info/top_level.txt
 pptx_tools/apps/__init__.py
 pptx_tools/apps/slide_add_voice.py
+pptx_tools/apps/slide_delete_notes.py
 pptx_tools/data/__init__.py
 pptx_tools/data/hello.pptx
 pptx_tools/data/transparent.png
 pptx_tools/tts/__init__.py
 pptx_tools/tts/azure_tts.py
 pptx_tools/tts/azure_tts_voice.py
 pptx_tools/tts/google_tts.py
```

### Comparing `pptx-tools-0.1.5/setup.py` & `pptx-tools-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.5"
+version = "0.1.6"
 
 
 if sys.argv[-1] == "release":
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
@@ -80,10 +80,11 @@
         'azure': azure_install_requires,
         'all': (install_requires
                 + azure_install_requires),
     },
     entry_points={
         "console_scripts": [
             "slide-add-voice=pptx_tools.apps.slide_add_voice:main",
+            "slide-delete-notes=pptx_tools.apps.slide_delete_notes:main",
         ]
     },
 )
```

### Comparing `pptx-tools-0.1.5/tests/pptx_tools/test_slide_add_voice.py` & `pptx-tools-0.1.6/tests/pptx_tools/test_slide_add_voice.py`

 * *Files identical despite different names*

