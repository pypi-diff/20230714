# Comparing `tmp/skelly_synchronize-2023.6.1021.tar.gz` & `tmp/skelly_synchronize-2023.7.1022.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.6.1021.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_synchronize-2023.7.1022.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_synchronize-2023.6.1021.tar` & `skelly_synchronize-2023.7.1022.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0       65 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.gitattributes
--rw-r--r--   0        0        0      146 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1010 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/.gitignore
--rw-r--r--   0        0        0    34523 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/LICENSE
--rw-r--r--   0        0        0     3030 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/README.md
--rw-r--r--   0        0        0     1646 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/setup.py
--rw-r--r--   0        0        0     1056 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     3401 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      616 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_output.py
--rw-r--r--   0        0        0     3015 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_plots.py
--rw-r--r--   0        0        0     1558 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     3438 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     5993 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1873 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     5488 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      646 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1487 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0     1593 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_all_files_created.py
--rw-r--r--   0        0        0      656 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      522 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_number_of_videos_is_preserved.py
--rw-r--r--   0        0        0      847 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      712 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_videos_are_same_length.py
--rw-r--r--   0        0        0      577 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-06-21 19:45:06.650786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1044 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     1853 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1348 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1103 2023-06-21 19:45:06.654786 skelly_synchronize-2023.6.1021/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3980 1970-01-01 00:00:00.000000 skelly_synchronize-2023.6.1021/PKG-INFO
+-rw-r--r--   0        0        0      504 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/.flake8
+-rw-r--r--   0        0        0       65 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/.gitattributes
+-rw-r--r--   0        0        0      146 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1010 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/.gitignore
+-rw-r--r--   0        0        0    34523 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/LICENSE
+-rw-r--r--   0        0        0     3030 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/README.md
+-rw-r--r--   0        0        0     1698 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/setup.py
+-rw-r--r--   0        0        0     1064 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     3401 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      616 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/debugging/debug_output.py
+-rw-r--r--   0        0        0     3003 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/debugging/debug_plots.py
+-rw-r--r--   0        0        0     1557 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     3414 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     5993 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1873 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     5488 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      646 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1486 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0     1593 2023-07-13 21:59:53.002742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_all_files_created.py
+-rw-r--r--   0        0        0      656 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      522 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_number_of_videos_is_preserved.py
+-rw-r--r--   0        0        0      847 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      712 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_videos_are_same_length.py
+-rw-r--r--   0        0        0      577 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1062 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     1853 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1348 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1078 2023-07-13 21:59:53.006742 skelly_synchronize-2023.7.1022/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 skelly_synchronize-2023.7.1022/PKG-INFO
```

### Comparing `skelly_synchronize-2023.6.1021/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.7.1022/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.7.1022/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/.gitignore` & `skelly_synchronize-2023.7.1022/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/LICENSE` & `skelly_synchronize-2023.7.1022/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/README.md` & `skelly_synchronize-2023.7.1022/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/pyproject.toml` & `skelly_synchronize-2023.7.1022/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -40,18 +40,27 @@
 ] #add additional dependencies here - try to pin versions as minimally as possible
 
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+dev = [
+"black",
+"bumpver", 
+"isort", 
+"pip-tools", 
+"pytest", 
+"flake8",
+"flake8-bandit",
+"flake8-bugbear",
+]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.06.1021"
+current_version = "v2023.07.1022"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.06.1021"
+__version__ = "v2023.07.1022"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
@@ -20,11 +20,11 @@
 
 base_package_path = Path(__file__).parent
 print(f"adding base_package_path: {base_package_path} : to sys.path")
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from skelly_synchronize.system.default_paths import get_log_file_path
 from skelly_synchronize.system.logging_configuration import configure_logging
-from skelly_synchronize.skelly_synchronize import synchronize_videos_from_audio
+from skelly_synchronize.skelly_synchronize import synchronize_videos_from_audio  # noqa
 
 
 configure_logging(log_file_path=get_log_file_path())
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_output.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/debugging/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/debugging/debug_plots.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/debugging/debug_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import librosa
-import toml
 import numpy as np
 import plotly.graph_objects as go
 import plotly.subplots as sp
 import plotly.colors as colors
 from pathlib import Path
 from typing import List
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     output_video_pathstring: str,
 ):
     vertical_video_bool = check_if_video_has_reversed_metadata(
         video_pathstring=input_video_pathstring
     )
 
     if vertical_video_bool:
-        logging.info(f"Video has reversed metadata, changing FFmpeg transpose argument")
+        logging.info("Video has reversed metadata, changing FFmpeg transpose argument")
         ffparams = {"-ffprefixes": ["-noautorotate"], "-vf": "transpose=1"}
     else:
         ffparams = {}
 
     decoder = FFdecoder(
         str(input_video_pathstring),
         frame_format="bgr24",
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     input_video_pathstring: str,
     start_time: float,
     desired_duration: float,
     output_video_pathstring: str,
 ):
     """Run a subprocess call to trim a video from start time to last as long as the desired duration"""
 
-    trim_video_subprocess = subprocess.run(
+    subprocess.run(
         [
             "ffmpeg",
             "-i",
             f"{input_video_pathstring}",
             "-ss",
             f"{start_time}",
             "-t",
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/skelly_synchronize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import time
 import logging
 from pathlib import Path
 from skelly_synchronize.core_processes.debugging.debug_plots import create_debug_plots
 
-logging.basicConfig(level=logging.INFO)
-
 from skelly_synchronize.utils.get_video_files import get_video_file_list
 from skelly_synchronize.core_processes.audio_utilities import (
     extract_audio_files,
     get_audio_sample_rates,
 )
 from skelly_synchronize.core_processes.correlation_functions import find_lags
 from skelly_synchronize.core_processes.video_functions.video_utilities import (
@@ -36,14 +34,16 @@
     LAG_DICTIONARY_NAME,
     RAW_VIDEO_NAME,
     SYNCHRONIZED_VIDEO_NAME,
     SYNCHRONIZED_VIDEOS_FOLDER_NAME,
     AUDIO_FILES_FOLDER_NAME,
 )
 
+logging.basicConfig(level=logging.INFO)
+
 
 def synchronize_videos_from_audio(
     raw_video_folder_path: Path,
     synchronized_video_folder_path: Path = None,
     file_type: str = ".mp4",
     video_handler: str = "deffcode",
     create_debug_plots_bool: bool = True,
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/system/paths_and_file_names.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/system/paths_and_file_names.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import pytest
 from pathlib import Path
 
-print(f"Thank you for using skelly_synchronize!")
+print("Thank you for using skelly_synchronize!")
 print(f"This is printing from: {__file__}")
 
 base_package_path = Path(__file__).parent.parent.parent
 print(f"adding base_package_path: {base_package_path} : to sys.path")
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from skelly_synchronize.skelly_synchronize import synchronize_videos_from_audio
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_all_files_created.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_all_files_created.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_number_of_videos_is_preserved.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_number_of_videos_is_preserved.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/test_videos_are_same_length.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/test_videos_are_same_length.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import sys
 from pathlib import Path
 from typing import Union
 
-logger = logging.getLogger(__name__)
-
 base_package_path = Path(__file__).parent.parent.parent.parent
 print(f"adding base_package_path: {base_package_path} : to sys.path")
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from skelly_synchronize.utils.get_video_files import get_video_file_list
 from skelly_synchronize.tests.utilities.find_frame_count_of_video import (
     find_frame_count_of_video,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def get_number_of_frames_of_videos_in_a_folder(folder_path: Union[str, Path]):
     """
     Get the number of frames in the first video in a folder
     """
 
     list_of_video_paths = get_video_file_list(
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def load_sample_data() -> Path:
     extract_to_path = Path.home()
     extract_to_path.mkdir(exist_ok=True)
 
     figshare_sample_data_path = extract_to_path / FIGSHARE_SAMPLE_DATA_FILE_NAME
 
     if not Path.exists(figshare_sample_data_path):
-        r = requests.get(FIGSHARE_ZIP_FILE_URL)
+        r = requests.get(FIGSHARE_ZIP_FILE_URL, timeout=(10, 60))
         z = zipfile.ZipFile(io.BytesIO(r.content))
         z.extractall(figshare_sample_data_path)
 
     return figshare_sample_data_path
 
 
 def find_raw_videos_folder_path(session_folder_path: Path) -> Path:
```

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.6.1021/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.7.1022/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from pathlib import Path
-from typing import Union
 
 logging.basicConfig(level=logging.INFO)
 
 
 def create_directory(parent_directory: Path, directory_name: str) -> Path:
     """Create a new directory under the specified parent directory."""
     parent_directory = Path(parent_directory)
```

### Comparing `skelly_synchronize-2023.6.1021/PKG-INFO` & `skelly_synchronize-2023.7.1022/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.6.1021
+Version: 2023.7.1022
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
@@ -21,14 +21,17 @@
 Requires-Dist: plotly
 Requires-Dist: kaleido
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: flake8 ; extra == "dev"
+Requires-Dist: flake8-bandit ; extra == "dev"
+Requires-Dist: flake8-bugbear ; extra == "dev"
 Provides-Extra: dev
 
 # Skelly Synchronize
 
 This package synchronizes a set of videos of the same event by cross-correlating their audio files. The videos will be synchronized so that they all start at the earliest shared time, and end at the latest shared time. 
 
 # Install and Run
```

