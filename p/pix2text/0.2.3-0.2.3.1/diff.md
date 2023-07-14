# Comparing `tmp/pix2text-0.2.3.tar.gz` & `tmp/pix2text-0.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2text-0.2.3.tar", last modified: Mon Jul  3 10:12:44 2023, max compression
+gzip compressed data, was "pix2text-0.2.3.1.tar", last modified: Fri Jul 14 06:03:02 2023, max compression
```

## Comparing `pix2text-0.2.3.tar` & `pix2text-0.2.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.363506 pix2text-0.2.3/
--rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-0.2.3/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    24094 2023-07-03 10:12:44.362534 pix2text-0.2.3/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    23013 2023-07-03 10:03:16.000000 pix2text-0.2.3/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.339966 pix2text-0.2.3/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      210 2023-07-03 02:18:23.000000 pix2text-0.2.3/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      108 2023-06-30 06:16:40.000000 pix2text-0.2.3/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-0.2.3/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-0.2.3/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)     4947 2023-07-03 06:25:56.000000 pix2text-0.2.3/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)      929 2023-07-01 16:05:56.000000 pix2text-0.2.3/pix2text/consts.py
--rw-r--r--   0 king       (501) staff       (20)      862 2022-07-13 13:10:07.000000 pix2text-0.2.3/pix2text/latex_config.yaml
--rw-r--r--   0 king       (501) staff       (20)    12842 2023-07-03 09:34:16.000000 pix2text-0.2.3/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-0.2.3/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)    20490 2023-07-03 09:30:59.000000 pix2text-0.2.3/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5300 2023-02-03 11:26:24.000000 pix2text-0.2.3/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-0.2.3/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     2026 2023-07-02 13:12:54.000000 pix2text-0.2.3/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)    14209 2023-07-03 03:07:25.000000 pix2text-0.2.3/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.345337 pix2text-0.2.3/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    24094 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)      904 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       41 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-0.2.3/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      172 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2023-07-03 10:12:44.000000 pix2text-0.2.3/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.358879 pix2text-0.2.3/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-0.2.3/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-0.2.3/scripts/convert_label_studio_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-0.2.3/scripts/gen_label_studio_json.py
--rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-0.2.3/scripts/gen_pure_formula_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-0.2.3/scripts/merge_label_studio_anno_pred_json.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-0.2.3/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-0.2.3/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-0.2.3/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      554 2023-02-03 09:49:06.000000 pix2text-0.2.3/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)       38 2023-07-03 10:12:44.363697 pix2text-0.2.3/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2185 2023-07-02 12:56:12.000000 pix2text-0.2.3/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-03 10:12:44.361000 pix2text-0.2.3/tests/
--rw-r--r--   0 king       (501) staff       (20)     1372 2023-02-14 10:16:51.000000 pix2text-0.2.3/tests/test_pix2text.py
--rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-0.2.3/tests/test_sort_boxes.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-14 06:03:02.896563 pix2text-0.2.3.1/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-0.2.3.1/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    24086 2023-07-14 06:03:02.895912 pix2text-0.2.3.1/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    23003 2023-07-03 10:20:43.000000 pix2text-0.2.3.1/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-14 06:03:02.855066 pix2text-0.2.3.1/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      210 2023-07-03 02:18:23.000000 pix2text-0.2.3.1/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      110 2023-07-13 15:31:08.000000 pix2text-0.2.3.1/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-0.2.3.1/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-0.2.3.1/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)     4947 2023-07-03 06:25:56.000000 pix2text-0.2.3.1/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)      929 2023-07-01 16:05:56.000000 pix2text-0.2.3.1/pix2text/consts.py
+-rw-r--r--   0 king       (501) staff       (20)      862 2022-07-13 13:10:07.000000 pix2text-0.2.3.1/pix2text/latex_config.yaml
+-rw-r--r--   0 king       (501) staff       (20)    12842 2023-07-03 09:34:16.000000 pix2text-0.2.3.1/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-0.2.3.1/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)    20490 2023-07-03 09:30:59.000000 pix2text-0.2.3.1/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5300 2023-02-03 11:26:24.000000 pix2text-0.2.3.1/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-0.2.3.1/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2026 2023-07-02 13:12:54.000000 pix2text-0.2.3.1/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    14220 2023-07-13 15:37:09.000000 pix2text-0.2.3.1/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-14 06:03:02.861021 pix2text-0.2.3.1/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    24086 2023-07-14 06:03:02.000000 pix2text-0.2.3.1/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)      904 2023-07-14 06:03:02.000000 pix2text-0.2.3.1/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2023-07-14 06:03:02.000000 pix2text-0.2.3.1/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       41 2023-07-14 06:03:02.000000 pix2text-0.2.3.1/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-0.2.3.1/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      172 2023-07-14 06:03:02.000000 pix2text-0.2.3.1/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2023-07-14 06:03:02.000000 pix2text-0.2.3.1/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-14 06:03:02.891740 pix2text-0.2.3.1/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-0.2.3.1/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-0.2.3.1/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-0.2.3.1/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-0.2.3.1/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-0.2.3.1/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-0.2.3.1/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-0.2.3.1/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-0.2.3.1/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      554 2023-07-14 06:02:42.000000 pix2text-0.2.3.1/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2023-07-14 06:03:02.896789 pix2text-0.2.3.1/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2185 2023-07-02 12:56:12.000000 pix2text-0.2.3.1/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-14 06:03:02.894448 pix2text-0.2.3.1/tests/
+-rw-r--r--   0 king       (501) staff       (20)     1372 2023-02-14 10:16:51.000000 pix2text-0.2.3.1/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-0.2.3.1/tests/test_sort_boxes.py
```

### Comparing `pix2text-0.2.3/LICENSE` & `pix2text-0.2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/PKG-INFO` & `pix2text-0.2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: An open-source Python3 tool for Optical Character Recognition (OCR) and LaTeX expression extraction from images, a Free Alternative to Mathpix
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
@@ -379,15 +379,15 @@
   ```
 
 * `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```python
   {
       'config': LATEX_CONFIG_FP,
-      'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
+      'model_fp': Path(data_dir()) / 'formula' / 'weights.pth',
       'no_resize': False
   }
   ```
 
 * `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```py
@@ -428,24 +428,22 @@
 
 
 返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
 
 * `type`：识别出的图像类别；
   * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `embedding`（行内的数学公式）；
   
-    >  Warning
-    > 对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
+    >  注意：对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
   * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
   
 * `text`：识别出的文字或Latex表达式；
 * `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`；
 * `line_number`：仅在使用 **MFD Analyzer** 时，才会包含此字段。此字段为 Box 所在的行号（第一行 **`line_number=0`**），值相同的 Box 表示它们在同一行。
 
-  > Warning
-  > 此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
+  > 注意：此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
 
 
 
 `Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
 
 ```python
 from pix2text import Pix2Text, merge_line_texts
```

### Comparing `pix2text-0.2.3/README.md` & `pix2text-0.2.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
   ```
 
 * `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```python
   {
       'config': LATEX_CONFIG_FP,
-      'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
+      'model_fp': Path(data_dir()) / 'formula' / 'weights.pth',
       'no_resize': False
   }
   ```
 
 * `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```py
@@ -400,24 +400,22 @@
 
 
 返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
 
 * `type`：识别出的图像类别；
   * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `embedding`（行内的数学公式）；
   
-    >  Warning
-    > 对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
+    >  注意：对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
   * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
   
 * `text`：识别出的文字或Latex表达式；
 * `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`；
 * `line_number`：仅在使用 **MFD Analyzer** 时，才会包含此字段。此字段为 Box 所在的行号（第一行 **`line_number=0`**），值相同的 Box 表示它们在同一行。
 
-  > Warning
-  > 此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
+  > 注意：此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
 
 
 
 `Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
 
 ```python
 from pix2text import Pix2Text, merge_line_texts
```

### Comparing `pix2text-0.2.3/pix2text/app.py` & `pix2text-0.2.3.1/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/category_mapping.py` & `pix2text-0.2.3.1/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/cli.py` & `pix2text-0.2.3.1/pix2text/cli.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/consts.py` & `pix2text-0.2.3.1/pix2text/consts.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/latex_config.yaml` & `pix2text-0.2.3.1/pix2text/latex_config.yaml`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/latex_ocr.py` & `pix2text-0.2.3.1/pix2text/latex_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/object_detector.py` & `pix2text-0.2.3.1/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/pix_to_text.py` & `pix2text-0.2.3.1/pix2text/pix_to_text.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/render.py` & `pix2text-0.2.3.1/pix2text/render.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/screenshot_daemon_with_server2.py` & `pix2text-0.2.3.1/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/serve.py` & `pix2text-0.2.3.1/pix2text/serve.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/pix2text/utils.py` & `pix2text-0.2.3.1/pix2text/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,27 +416,28 @@
     Returns: 合并后的字符串
 
     """
     out_texts = []
     line_margin_list = []  # 每行的最左边和左右边的x坐标
     isolated_included = []  # 每行是否包含了 `isolated` 类型的数学公式
     for o in out:
-        if len(out_texts) <= o['line_number']:
+        line_number = o.get('line_number', 0)
+        if len(out_texts) <= line_number:
             out_texts.append([])
             line_margin_list.append([0, 0])
             isolated_included.append(False)
-        out_texts[o['line_number']].append(o['text'])
-        line_margin_list[o['line_number']][1] = max(
-            line_margin_list[o['line_number']][1], float(o['position'][2, 0])
+        out_texts[line_number].append(o['text'])
+        line_margin_list[line_number][1] = max(
+            line_margin_list[line_number][1], float(o['position'][2, 0])
         )
-        line_margin_list[o['line_number']][0] = min(
-            line_margin_list[o['line_number']][0], float(o['position'][0, 0])
+        line_margin_list[line_number][0] = min(
+            line_margin_list[line_number][0], float(o['position'][0, 0])
         )
         if o['type'] == 'isolated':
-            isolated_included[o['line_number']] = True
+            isolated_included[line_number] = True
 
     line_text_list = [smart_join(o) for o in out_texts]
 
     if not auto_line_break:
         return line_sep.join(line_text_list)
 
     line_lengths = [rx - lx for lx, rx in line_margin_list]
```

### Comparing `pix2text-0.2.3/pix2text.egg-info/PKG-INFO` & `pix2text-0.2.3.1/pix2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: An open-source Python3 tool for Optical Character Recognition (OCR) and LaTeX expression extraction from images, a Free Alternative to Mathpix
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
@@ -379,15 +379,15 @@
   ```
 
 * `formula_config` (dict): 公式识别模型对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```python
   {
       'config': LATEX_CONFIG_FP,
-      'checkpoint': Path(data_dir()) / 'formula' / 'weights.pth',
+      'model_fp': Path(data_dir()) / 'formula' / 'weights.pth',
       'no_resize': False
   }
   ```
 
 * `thresholds` (dict): 识别阈值对应的配置信息；默认为 `None`，表示使用默认配置：
 
   ```py
@@ -428,24 +428,22 @@
 
 
 返回结果为列表（`list`），列表中的每个元素为`dict`，包含如下 `key`：
 
 * `type`：识别出的图像类别；
   * 当开启Analyzer时（`use_analyzer==True`），取值为 `text`（纯文本）、`isolated`（独立行的数学公式） 或者 `embedding`（行内的数学公式）；
   
-    >  Warning
-    > 对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
+    >  注意：对于 **MFD Analyzer** ，此取值从 P2T **v0.2.3** 开始与之前不同。
   * 当未开启Analyzer时（`use_analyzer==False`），取值为`formula`（纯数学公式）、`english`（纯英文文字）、`general`（纯文字，可能包含中英文）；
   
 * `text`：识别出的文字或Latex表达式；
 * `position`：所在块的位置信息，`np.ndarray`, with shape of `[4, 2]`；
 * `line_number`：仅在使用 **MFD Analyzer** 时，才会包含此字段。此字段为 Box 所在的行号（第一行 **`line_number=0`**），值相同的 Box 表示它们在同一行。
 
-  > Warning
-  > 此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
+  > 注意：此取值从 P2T **v0.2.3** 开始才有，之前版本没有此 `key`。
 
 
 
 `Pix2Text` 类也实现了 `__call__()` 函数，其功能与 `.recognize()` 函数完全相同。所以才会有以下的调用方式：
 
 ```python
 from pix2text import Pix2Text, merge_line_texts
```

### Comparing `pix2text-0.2.3/pix2text.egg-info/SOURCES.txt` & `pix2text-0.2.3.1/pix2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/convert_label_studio_to_yolov7.py` & `pix2text-0.2.3.1/scripts/convert_label_studio_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/gen_label_studio_json.py` & `pix2text-0.2.3.1/scripts/gen_label_studio_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/gen_pure_formula_to_yolov7.py` & `pix2text-0.2.3.1/scripts/gen_pure_formula_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/merge_label_studio_anno_pred_json.py` & `pix2text-0.2.3.1/scripts/merge_label_studio_anno_pred_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/object_detection3.py` & `pix2text-0.2.3.1/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/screenshot_daemon.py` & `pix2text-0.2.3.1/scripts/screenshot_daemon.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/try_layout.py` & `pix2text-0.2.3.1/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/scripts/try_service.py` & `pix2text-0.2.3.1/scripts/try_service.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/setup.py` & `pix2text-0.2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/tests/test_pix2text.py` & `pix2text-0.2.3.1/tests/test_pix2text.py`

 * *Files identical despite different names*

### Comparing `pix2text-0.2.3/tests/test_sort_boxes.py` & `pix2text-0.2.3.1/tests/test_sort_boxes.py`

 * *Files identical despite different names*

