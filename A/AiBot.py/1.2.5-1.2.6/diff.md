# Comparing `tmp/AiBot.py-1.2.5.tar.gz` & `tmp/AiBot.py-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AiBot.py-1.2.5.tar", last modified: Mon Mar 20 09:05:39 2023, max compression
+gzip compressed data, was "AiBot.py-1.2.6.tar", last modified: Fri Jul 14 01:15:52 2023, max compression
```

## Comparing `AiBot.py-1.2.5.tar` & `AiBot.py-1.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-03-20 09:05:39.521922 AiBot.py-1.2.5/
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-03-20 09:05:39.516522 AiBot.py-1.2.5/AiBot/
--rw-r--r--   0 chenxun    (501) staff       (20)    53758 2023-03-20 08:54:28.000000 AiBot.py-1.2.5/AiBot/_AndroidBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)    21135 2023-03-13 02:59:10.000000 AiBot.py-1.2.5/AiBot/_WebBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)    35769 2023-03-13 02:59:10.000000 AiBot.py-1.2.5/AiBot/_WinBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)      162 2022-12-11 09:17:44.000000 AiBot.py-1.2.5/AiBot/__init__.py
--rw-r--r--   0 chenxun    (501) staff       (20)     5044 2022-08-31 16:13:27.000000 AiBot.py-1.2.5/AiBot/_loguru_format.py
--rw-r--r--   0 chenxun    (501) staff       (20)     1712 2023-03-13 02:59:10.000000 AiBot.py-1.2.5/AiBot/_utils.py
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-03-20 09:05:39.518272 AiBot.py-1.2.5/AiBot.py.egg-info/
--rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-03-20 09:05:39.000000 AiBot.py-1.2.5/AiBot.py.egg-info/PKG-INFO
--rw-r--r--   0 chenxun    (501) staff       (20)      368 2023-03-20 09:05:39.000000 AiBot.py-1.2.5/AiBot.py.egg-info/SOURCES.txt
--rw-r--r--   0 chenxun    (501) staff       (20)        1 2023-03-20 09:05:39.000000 AiBot.py-1.2.5/AiBot.py.egg-info/dependency_links.txt
--rw-r--r--   0 chenxun    (501) staff       (20)       14 2023-03-20 09:05:39.000000 AiBot.py-1.2.5/AiBot.py.egg-info/requires.txt
--rw-r--r--   0 chenxun    (501) staff       (20)        6 2023-03-20 09:05:39.000000 AiBot.py-1.2.5/AiBot.py.egg-info/top_level.txt
--rw-r--r--   0 chenxun    (501) staff       (20)     1056 2022-08-31 16:13:27.000000 AiBot.py-1.2.5/LICENSE
--rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-03-20 09:05:39.521447 AiBot.py-1.2.5/PKG-INFO
--rw-r--r--   0 chenxun    (501) staff       (20)     5253 2022-12-16 13:41:49.000000 AiBot.py-1.2.5/README.md
--rw-r--r--   0 chenxun    (501) staff       (20)      104 2022-08-31 16:13:27.000000 AiBot.py-1.2.5/pyproject.toml
--rw-r--r--   0 chenxun    (501) staff       (20)       38 2023-03-20 09:05:39.522047 AiBot.py-1.2.5/setup.cfg
--rw-r--r--   0 chenxun    (501) staff       (20)      622 2023-03-20 09:01:08.000000 AiBot.py-1.2.5/setup.py
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-03-20 09:05:39.520615 AiBot.py-1.2.5/test/
--rw-r--r--   0 chenxun    (501) staff       (20)     1534 2023-03-07 01:28:50.000000 AiBot.py-1.2.5/test/test_android.py
--rw-r--r--   0 chenxun    (501) staff       (20)      796 2023-02-16 09:55:43.000000 AiBot.py-1.2.5/test/test_web.py
--rw-r--r--   0 chenxun    (501) staff       (20)      370 2022-12-11 09:17:44.000000 AiBot.py-1.2.5/test/test_win.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.693468 AiBot.py-1.2.6/
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.688877 AiBot.py-1.2.6/AiBot/
+-rw-r--r--   0 chenxun    (501) staff       (20)    54124 2023-07-14 01:10:01.000000 AiBot.py-1.2.6/AiBot/_AndroidBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)    21135 2023-03-13 02:59:10.000000 AiBot.py-1.2.6/AiBot/_WebBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)    35796 2023-07-14 01:14:57.000000 AiBot.py-1.2.6/AiBot/_WinBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      162 2022-12-11 09:17:44.000000 AiBot.py-1.2.6/AiBot/__init__.py
+-rw-r--r--   0 chenxun    (501) staff       (20)     5044 2022-08-31 16:13:27.000000 AiBot.py-1.2.6/AiBot/_loguru_format.py
+-rw-r--r--   0 chenxun    (501) staff       (20)     1712 2023-03-22 01:46:17.000000 AiBot.py-1.2.6/AiBot/_utils.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.691084 AiBot.py-1.2.6/AiBot.py.egg-info/
+-rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/PKG-INFO
+-rw-r--r--   0 chenxun    (501) staff       (20)      368 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)        1 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)       14 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/requires.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)        6 2023-07-14 01:15:52.000000 AiBot.py-1.2.6/AiBot.py.egg-info/top_level.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)     1056 2022-08-31 16:13:27.000000 AiBot.py-1.2.6/LICENSE
+-rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-07-14 01:15:52.692932 AiBot.py-1.2.6/PKG-INFO
+-rw-r--r--   0 chenxun    (501) staff       (20)     5253 2022-12-16 13:41:49.000000 AiBot.py-1.2.6/README.md
+-rw-r--r--   0 chenxun    (501) staff       (20)      104 2022-08-31 16:13:27.000000 AiBot.py-1.2.6/pyproject.toml
+-rw-r--r--   0 chenxun    (501) staff       (20)       38 2023-07-14 01:15:52.693606 AiBot.py-1.2.6/setup.cfg
+-rw-r--r--   0 chenxun    (501) staff       (20)      622 2023-07-14 01:12:34.000000 AiBot.py-1.2.6/setup.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-07-14 01:15:52.692439 AiBot.py-1.2.6/test/
+-rw-r--r--   0 chenxun    (501) staff       (20)     1534 2023-07-14 01:10:12.000000 AiBot.py-1.2.6/test/test_android.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      796 2023-02-16 09:55:43.000000 AiBot.py-1.2.6/test/test_web.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      370 2022-12-11 09:17:44.000000 AiBot.py-1.2.6/test/test_win.py
```

### Comparing `AiBot.py-1.2.5/AiBot/_AndroidBot.py` & `AiBot.py-1.2.6/AiBot/_AndroidBot.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,24 +658,26 @@
     def __parse_ocr(text: str) -> list:
         """
         解析 OCR 识别出出来的信息
 
         :param text:
         :return:
         """
-        pattern = re.compile(r'(\[\[\[).+?(\)])')
-        matches = pattern.finditer(text)
+        # pattern = re.compile(r'(\[\[\[).+?(\)])')
+        # matches = pattern.finditer(text)
+        #
+        # text_info_list = []
+        # for match in matches:
+        #     result_str = match.group()
+        #     text_info = literal_eval(result_str)
+        #     text_info_list.append(text_info)
+        #
+        # return text_info_list
 
-        text_info_list = []
-        for match in matches:
-            result_str = match.group()
-            text_info = literal_eval(result_str)
-            text_info_list.append(text_info)
-
-        return text_info_list
+        return literal_eval(text)
 
     def __ocr_server(self, region: _Region = None, algorithm: _Algorithm = None, scale: float = 1.0) -> list:
         """
         OCR 服务，通过 OCR 识别屏幕中文字
 
         :param region:
         :param algorithm:
@@ -689,19 +691,33 @@
             algorithm_type, threshold, max_val = [0, 0, 0]
         else:
             algorithm_type, threshold, max_val = algorithm
             if algorithm_type in (5, 6):
                 threshold = 127
                 max_val = 255
 
+        # scale 仅支持区域识别
+        if region[2] == 0:
+            scale = 1.0
+
         response = self.__send_data("ocr", *region, algorithm_type, threshold, max_val, scale)
         if response == "null" or response == "":
             return []
         return self.__parse_ocr(response)
 
+    def init_ocr_server(self, ip: str, port: int=9752) -> bool:
+        """
+        初始化 OCR 服务
+
+        :param ip:
+        :param port:
+        :return:
+        """
+        return self.__send_data("initOcr", ip, port) == "true"
+
     def get_text(self, region: _Region = None, algorithm: _Algorithm = None, scale: float = 1.0) -> List[str]:
         """
         通过 OCR 识别屏幕中的文字，返回文字列表
 
         :param region: 识别区域，默认全屏；
         :param algorithm: 处理图片/屏幕所用算法和参数，默认保存原图；
         :param scale: 图片缩放率，默认为 1.0，1.0 以下为缩小，1.0 以上为放大；
@@ -727,17 +743,16 @@
         :param algorithm: 处理图片/屏幕所用算法和参数，默认保存原图；
         :param scale: 图片缩放率，默认为 1.0，1.0 以下为缩小，1.0 以上为放大；
         :return: 坐标列表（坐标是文本区域中心位置）
 
         .. seealso::
             :meth:`find_image`: ``region`` 和 ``algorithm`` 的参数说明
         """
-        # scale 仅支持区域识别
-        if region[2] == 0:
-            scale = 1.0
+        if not region:
+            region = [0, 0, 0, 0]
 
         text_info_list = self.__ocr_server(region, algorithm, scale)
 
         text_points = []
         for text_info in text_info_list:
             if text in text_info[-1][0]:
                 points, words_tuple = text_info
```

### Comparing `AiBot.py-1.2.5/AiBot/_WebBot.py` & `AiBot.py-1.2.6/AiBot/_WebBot.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.5/AiBot/_WinBot.py` & `AiBot.py-1.2.6/AiBot/_WinBot.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,24 +478,24 @@
     def __parse_ocr(text: str) -> list:
         """
         解析 OCR 识别出出来的信息
 
         :param text:
         :return:
         """
-        pattern = re.compile(r'(\[\[\[).+?(\)])')
-        matches = pattern.finditer(text)
+        # pattern = re.compile(r'(\[\[\[).+?(\)])')
+        # matches = pattern.finditer(text)
+        #
+        # text_info_list = []
+        # for match in matches:
+        #     result_str = match.group()
+        #     text_info = literal_eval(result_str)
+        #     text_info_list.append(text_info)
 
-        text_info_list = []
-        for match in matches:
-            result_str = match.group()
-            text_info = literal_eval(result_str)
-            text_info_list.append(text_info)
-
-        return text_info_list
+        return literal_eval(text)
 
     def __ocr_server(self, hwnd: str, region: _Region = None, algorithm: _Algorithm = None, mode: bool = False) -> list:
         """
         OCR 服务，通过 OCR 识别屏幕中文字
 
         :param hwnd:
         :param region:
```

### Comparing `AiBot.py-1.2.5/AiBot/_loguru_format.py` & `AiBot.py-1.2.6/AiBot/_loguru_format.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.5/AiBot/_utils.py` & `AiBot.py-1.2.6/AiBot/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 _SubColors = List[Tuple[int, int, str]]
 
 
 def _protect(*protected):
     """
     元类工厂，禁止类属性或方法被子类重写
 
-    :param protected: 禁止重新的属性或方法
+    :param protected: 禁止重写的属性或方法
     :return:
     """
 
     class Protect(abc.ABCMeta):
         # 是否父类
         is_parent_class = True
```

### Comparing `AiBot.py-1.2.5/LICENSE` & `AiBot.py-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.5/README.md` & `AiBot.py-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.5/setup.py` & `AiBot.py-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install_requires = [
     "loguru~=0.6.0"
 ]
 
 setup_kwargs = {
     'name': 'AiBot.py',
-    'version': '1.2.5',
+    'version': '1.2.6',
     'description': '...',
     'long_description': '...',
     'long_description_content_type': 'text/markdown',
     'author': 'waitan2018',
     'author_email': None,
     'maintainer': 'waitan2018',
     'maintainer_email': None,
```

### Comparing `AiBot.py-1.2.5/test/test_android.py` & `AiBot.py-1.2.6/test/test_android.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.5/test/test_web.py` & `AiBot.py-1.2.6/test/test_web.py`

 * *Files identical despite different names*

