# Comparing `tmp/ffmpeg_media_type-0.0.4.tar.gz` & `tmp/ffmpeg_media_type-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_media_type-0.0.4.tar", max compression
+gzip compressed data, was "ffmpeg_media_type-0.0.5.tar", max compression
```

## Comparing `ffmpeg_media_type-0.0.4.tar` & `ffmpeg_media_type-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1066 2023-07-13 15:50:52.894261 ffmpeg_media_type-0.0.4/LICENSE
--rw-r--r--   0        0        0     4026 2023-07-13 15:50:52.894261 ffmpeg_media_type-0.0.4/README.md
--rw-r--r--   0        0        0      869 2023-07-13 15:51:17.946539 ffmpeg_media_type-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/__init__.py
--rw-r--r--   0        0        0    89367 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.2.json
--rw-r--r--   0        0        0    91003 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.3.json
--rw-r--r--   0        0        0    92339 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.4.json
--rw-r--r--   0        0        0    94852 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.0.json
--rw-r--r--   0        0        0    95951 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.1.json
--rw-r--r--   0        0        0    97292 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.2.json
--rw-r--r--   0        0        0   100111 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.3.json
--rw-r--r--   0        0        0   106316 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.4.json
--rw-r--r--   0        0        0   107177 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.0.json
--rw-r--r--   0        0        0   109161 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.1.json
--rw-r--r--   0        0        0   120284 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-6.0.json
--rw-r--r--   0        0        0     3780 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/info.py
--rw-r--r--   0        0        0      378 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/main.py
--rw-r--r--   0        0        0        0 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/py.typed
--rw-r--r--   0        0        0        0 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/__init__.py
--rw-r--r--   0        0        0     5956 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/ffmpeg.py
--rw-r--r--   0        0        0     2977 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/table.py
--rw-r--r--   0        0        0     1790 2023-07-13 15:50:53.022262 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/wiki_ext.py
--rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4904 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/README.md
+-rw-r--r--   0        0        0     1589 2023-07-14 21:03:14.467695 ffmpeg_media_type-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      186 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/__init__.py
+-rw-r--r--   0        0        0    89367 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.2.json
+-rw-r--r--   0        0        0    91003 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.3.json
+-rw-r--r--   0        0        0    92339 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.4.json
+-rw-r--r--   0        0        0    94852 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.0.json
+-rw-r--r--   0        0        0    95951 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.1.json
+-rw-r--r--   0        0        0    97292 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.2.json
+-rw-r--r--   0        0        0   100111 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.3.json
+-rw-r--r--   0        0        0   106316 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.4.json
+-rw-r--r--   0        0        0   107177 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.0.json
+-rw-r--r--   0        0        0   109161 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.1.json
+-rw-r--r--   0        0        0   120284 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-6.0.json
+-rw-r--r--   0        0        0     3778 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/info.py
+-rw-r--r--   0        0        0      378 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/py.typed
+-rw-r--r--   0        0        0        0 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/__init__.py
+-rw-r--r--   0        0        0     5951 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/ffmpeg.py
+-rw-r--r--   0        0        0     2977 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/table.py
+-rw-r--r--   0        0        0     1790 2023-07-14 21:02:53.807174 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/wiki_ext.py
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.5/PKG-INFO
```

### Comparing `ffmpeg_media_type-0.0.4/LICENSE` & `ffmpeg_media_type-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/README.md` & `ffmpeg_media_type-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```
 
 ### Detecting Media File Information
 
 To detect media file information, use the `detect` function, providing the path to the media file as a parameter:
 
 ```python
-media_info = ffmpeg_media_type.info.detect('/path/to/media/file.mp4')
+media_info = ffmpeg_media_type.detect('/path/to/media/file.mp4')
 ```
 
 The `detect` function returns a model containing the following information:
 
 - `type`: The type of media file (e.g. `video`, `audio`, `image`, etc.).
 - `duration`: The duration of the media file in seconds.
 - `width`: The width of the media file in pixels.
@@ -62,27 +62,44 @@
 ```python
 import ffmpeg_media_type
 
 # Specify the path to the media file
 file_path = '/path/to/media/file.mp4'
 
 # Detect media file information
-media_info = ffmpeg_media_type.info.detect(file_path)
+media_info = ffmpeg_media_type.detect(file_path)
 
 # Extract information from the media_info dictionary
 duration = media_info.duration
 width = media_info.width
 height = media_info.height
 
 # Print the extracted information
 print(f"Duration: {duration} seconds")
 print(f"Width: {width} pixels")
 print(f"Height: {height} pixels")
 ```
 
+### Enhancing Accuracy in Guessing Media File Extensions with FFmpeg
+
+- Typically, the media file's extension is utilized to determine its file type. Nevertheless, this approach may not always yield accurate results. For instance, a file bearing the `.mp4` extension could, in reality, be an audio file.
+- The `ffmpeg-media-type` tool enhances the precision of media file extension guessing by leveraging the built-in format functionality of FFmpeg through the command `ffmpeg -formats`.
+
+check [data](https://github.com/livingbio/ffmpeg-media-type/tree/main/src/ffmpeg_media_type/data) for details.
+
+### Access ffprobe output
+
+If you need to access the raw ffprobe output, you can use the `ffprobe` function:
+
+```python
+ffprobe_output = ffmpeg_media_type.ffprobe('/path/to/media/file.mp4')
+
+duration = ffprobe_output.format.duration
+codec_type = ffprobe_output.streams[0].codec_type
+```
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/livingbio/ffmpeg-media-type/issues). If you would like to contribute code, please fork the repository and submit a pull request.
 
 Before submitting a pull request, make sure to run the tests using the following command:
 
 ```bash
```

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.2.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.3.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.4.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.0.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.1.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.2.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.3.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.4.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.0.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.1.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-6.0.json` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-6.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/info.py` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 from typing import Literal
 from urllib.parse import urlparse
 
 from pydantic import BaseModel
 
-from .utils.ffmpeg import FFProbeInfo, ffprobe_file, load_cache
+from .utils.ffmpeg import FFProbeInfo, ffprobe, load_cache
 
 
 class MediaInfo(BaseModel):
     type: Literal["image", "video", "audio"]
 
     width: int | None = None
     height: int | None = None
@@ -47,15 +47,15 @@
 
 
 def _extract_file_extension(uri: str) -> str:
     parsed_uri = urlparse(uri)
     path = parsed_uri.path
     filename = os.path.basename(path)
     _, extension = os.path.splitext(filename)
-    return extension[1:]
+    return extension[1:].lower()
 
 
 _KNOWN_CODEC_EXTS = {
     "png_pipe": ["png"],
     "svg_pipe": ["svg"],
     "tiff_pipe": ["tiff", "tif"],
     "bmp_pipe": ["bmp"],
@@ -131,9 +131,9 @@
         format=format_name,
         size=info.format.size,
         suggest_ext=suggest_ext,
     )
 
 
 def detect(uri: str) -> MediaInfo:
-    probe_info = ffprobe_file(uri)
+    probe_info = ffprobe(uri)
     return _guess_media_info(uri, probe_info)
```

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/ffmpeg.py` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,25 +172,25 @@
         version_line = output_lines[0].strip()
         version = version_line.split(" ")[2]
         return version
     except FileNotFoundError as e:
         raise FileNotFoundError("FFmpeg not found") from e
 
 
-def ffprobe_file(file_path: str) -> FFProbeInfo:
+def ffprobe(input_url: str) -> FFProbeInfo:
     # Construct the FFprobe command with JSON output format
     ffprobe_cmd = [
         "ffprobe",
         "-v",
         "error",
         "-show_format",
         "-show_streams",
         "-of",
         "json",
-        file_path,
+        input_url,
     ]
 
     try:
         # Execute the FFprobe command and capture the output
         output = subprocess.check_output(ffprobe_cmd, stderr=subprocess.STDOUT)
         output_str = output.decode("utf-8")  # Convert bytes to string
         return FFProbeInfo(**json.loads(output_str))
```

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/table.py` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/table.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/wiki_ext.py` & `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/wiki_ext.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.4/PKG-INFO` & `ffmpeg_media_type-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: ffmpeg-media-type
-Version: 0.0.4
-Summary: 
+Version: 0.0.5
+Summary: ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information.
+Keywords: ffmpeg,ffprobe,video,image,audio,media,mimetype,mp4,mp3,mov,webm
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # ffmpeg-media-type
@@ -45,15 +51,15 @@
 ```
 
 ### Detecting Media File Information
 
 To detect media file information, use the `detect` function, providing the path to the media file as a parameter:
 
 ```python
-media_info = ffmpeg_media_type.info.detect('/path/to/media/file.mp4')
+media_info = ffmpeg_media_type.detect('/path/to/media/file.mp4')
 ```
 
 The `detect` function returns a model containing the following information:
 
 - `type`: The type of media file (e.g. `video`, `audio`, `image`, etc.).
 - `duration`: The duration of the media file in seconds.
 - `width`: The width of the media file in pixels.
@@ -75,27 +81,44 @@
 ```python
 import ffmpeg_media_type
 
 # Specify the path to the media file
 file_path = '/path/to/media/file.mp4'
 
 # Detect media file information
-media_info = ffmpeg_media_type.info.detect(file_path)
+media_info = ffmpeg_media_type.detect(file_path)
 
 # Extract information from the media_info dictionary
 duration = media_info.duration
 width = media_info.width
 height = media_info.height
 
 # Print the extracted information
 print(f"Duration: {duration} seconds")
 print(f"Width: {width} pixels")
 print(f"Height: {height} pixels")
 ```
 
+### Enhancing Accuracy in Guessing Media File Extensions with FFmpeg
+
+- Typically, the media file's extension is utilized to determine its file type. Nevertheless, this approach may not always yield accurate results. For instance, a file bearing the `.mp4` extension could, in reality, be an audio file.
+- The `ffmpeg-media-type` tool enhances the precision of media file extension guessing by leveraging the built-in format functionality of FFmpeg through the command `ffmpeg -formats`.
+
+check [data](https://github.com/livingbio/ffmpeg-media-type/tree/main/src/ffmpeg_media_type/data) for details.
+
+### Access ffprobe output
+
+If you need to access the raw ffprobe output, you can use the `ffprobe` function:
+
+```python
+ffprobe_output = ffmpeg_media_type.ffprobe('/path/to/media/file.mp4')
+
+duration = ffprobe_output.format.duration
+codec_type = ffprobe_output.streams[0].codec_type
+```
 ## Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/livingbio/ffmpeg-media-type/issues). If you would like to contribute code, please fork the repository and submit a pull request.
 
 Before submitting a pull request, make sure to run the tests using the following command:
 
 ```bash
```

