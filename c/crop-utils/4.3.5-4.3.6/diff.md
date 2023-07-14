# Comparing `tmp/crop_utils-4.3.5.tar.gz` & `tmp/crop_utils-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.5.tar", last modified: Thu Jul  6 09:27:45 2023, max compression
+gzip compressed data, was "crop_utils-4.3.6.tar", last modified: Fri Jul 14 09:05:53 2023, max compression
```

## Comparing `crop_utils-4.3.5.tar` & `crop_utils-4.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.061596 crop_utils-4.3.5/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.5/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2016 2023-07-06 09:27:45.060595 crop_utils-4.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-06-12 03:15:02.000000 crop_utils-4.3.5/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 09:27:45.061596 crop_utils-4.3.5/setup.cfg
--rw-rw-rw-   0        0        0      913 2023-07-06 09:27:35.000000 crop_utils-4.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.032605 crop_utils-4.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.049594 crop_utils-4.3.5/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.5/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.5/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    63534 2023-06-07 06:16:06.000000 crop_utils-4.3.5/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    43480 2023-07-06 08:56:09.000000 crop_utils-4.3.5/src/crop_utils/img_crop.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:27:45.059599 crop_utils-4.3.5/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     2016 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 09:27:44.000000 crop_utils-4.3.5/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.595008 crop_utils-4.3.6/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.6/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1997 2023-07-14 09:05:53.595008 crop_utils-4.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-07-14 09:05:50.000000 crop_utils-4.3.6/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 09:05:53.596012 crop_utils-4.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-07-14 09:05:50.000000 crop_utils-4.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.572012 crop_utils-4.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.586007 crop_utils-4.3.6/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.6/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.6/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    62960 2023-07-14 08:06:39.000000 crop_utils-4.3.6/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43480 2023-07-06 08:56:09.000000 crop_utils-4.3.6/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.593006 crop_utils-4.3.6/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.5/LICENSE` & `crop_utils-4.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.5/PKG-INFO` & `crop_utils-4.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.5
-Summary: 鞋类ai识别;裁剪边距计算
+Version: 4.3.6
+Summary: 鞋类ai识别
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.4 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.6 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.5/README.md` & `crop_utils-4.3.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==4.3.4 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.6 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.5/setup.py` & `crop_utils-4.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.5",  # 版本号
+    version="4.3.6",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
-    description="鞋类ai识别;裁剪边距计算",
+    description="鞋类ai识别",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
```

### Comparing `crop_utils-4.3.5/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.6/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.5/src/crop_utils/image.py` & `crop_utils-4.3.6/src/crop_utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,15 @@
                 ['模特图', '模特胸像图', '模特胸像正面'], ['模特图', '模特胸像图', '模特胸像侧面'], ['模特图', '模特胸像图', '模特胸像背面'],
                 ['模特图', '模特下身图', '模特下身正面'], ['模特图', '模特下身图', '模特下身侧面'], ['模特图', '模特下身图', '模特下身背面'],
                 ['模特图', '模特全身图', '模特全身正面'], ['模特图', '模特全身图', '模特全身侧面'], ['模特图', '模特全身图', '模特全身背面'],
                 ['细节图', '面料'], ['细节图', '领部'], ['细节图', '肩部'], ['细节图', '腰部'], ['细节图', '衣袖'], ['细节图', '下摆'],
                 ['细节图', '口袋'], ['细节图', '门襟'], ['细节图', '内衬'], ['细节图', '图案'], ['细节图', '裤脚'],
                 ['细节图-鞋子', '鞋头'], ['细节图-鞋子', '鞋跟/鞋帮'], ['细节图-鞋子', '鞋口'], ['细节图-鞋子', '鞋底'], ['细节图-鞋子', '鞋标'],
                 ['平铺图', '平铺图背面'], ['平铺图', '平铺图正面'], ['平铺图', '平铺图侧面'],
-                ['静物图-鞋子', '前面'], ['静物图-鞋子', '后面'], ['静物图-鞋子', '鞋顶面'], ['静物图-鞋子', '鞋底面'],
-                ['静物图-鞋子', '侧面45度'], ['静物图-鞋子', '侧面90度'], ['静物图-鞋子', '侧面135度'], ['静物图-鞋子', '侧面225度'],
-                ['静物图-鞋子', '侧面270度'], ['静物图-鞋子', '侧面315度'],
+                ['静物图-鞋子', '鞋子'],
                 ['资质图', '吊牌图'], ['资质图', '洗水唛'],
                 ['动图']
                 ]
 
 CROP_TYPE = {
     'm_t': ['模特上身正面', '模特上身侧面', '模特上身背面'],
     'm_bu': ['模特胸像正面', '模特胸像侧面', '模特胸像背面'],
@@ -93,14 +91,17 @@
         self.shoes = Shoes(image_analysis)
 
         self.image_analysis = image_analysis
         # 获取主商品
         self.crop_point = self.deal_crop_key_point()
         # 获取图片背景图
         self.image_background = self.deal_image_background()
+        self.shoe_toe_cap = data.get("shoe_toe_cap", "其他")
+        self.shoe_topline = data.get("shoe_topline", "其他")
+        self.shoe_number = data.get("shoe_number", "其他")
 
         self.image_detail = ImageDetail()
         self.detail_point = {}  # {'裁剪模特帽子':{},}
 
         if self.img_crop_type == 'b':
             self.brand = Brand(image_analysis)
             self.brand_crop_point = self.brand.deal_brand_crop_point()
@@ -312,18 +313,15 @@
         #                "gif": "动图",
         #                }
         storage_to_slot = {'model-top_positive': '模特上身正面', 'model-top_side': '模特上身侧面', 'model-top_back': '模特上身背面',
                            'model-up_positive': '模特胸像正面', 'model-up_side': '模特胸像侧面', 'model-up_back': '模特胸像背面',
                            'model-down_positive': '模特下身正面', 'model-down_side': '模特下身侧面', 'model-down_back': '模特下身背面',
                            'model-all_positive': '模特全身正面', 'model-all_side': '模特全身侧面', 'model-all_back': '模特全身背面',
                            'tile_positive': '平铺图正面', 'tile_back': '平铺图背面', 'tile_side': '平铺图侧面',
-                           'tile-shoes_front': '前面', 'tile-shoes_back': '后面', 'tile-shoes_side45': '侧面45度',
-                           'tile-shoes_side90': '侧面90度', 'tile-shoes_side135': '侧面135度', 'tile-shoes_side225': '侧面225度',
-                           'tile-shoes_side270': '侧面270度', 'tile-shoes_side315': '侧面315度',
-                           'tile-shoes_bottom': '鞋底面', 'tile-shoes_top': '鞋顶面',
+                           'tile-shoes_shoes': '鞋子',
                            'detail_sweep': '下摆', 'detail_lining': '内衬', 'detail_pocket': '口袋',
                            'detail_pattern': '图案', 'detail_shoulder': '肩部', 'detail_waist': '腰部', 'detail_sleeve': '衣袖',
                            'detail_leg': '裤脚', 'detail_stay': '门襟', 'detail_fabric': '面料', 'detail_collar': '领部',
                            'detail_other': '其他',
                            'detail-shoes_toe': '鞋头', 'detail-shoes_heel': '鞋跟/鞋帮',
                            'detail-shoes_soles': '鞋底', 'detail-shoes_mouth': '鞋口', 'detail-shoes_label': '鞋标',
                            'intelligence_drop': '吊牌图', 'intelligence_tag': '洗水唛', 'gif': '动图',
```

### Comparing `crop_utils-4.3.5/src/crop_utils/img_crop.py` & `crop_utils-4.3.6/src/crop_utils/img_crop.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.5/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.6/src/crop_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.5
-Summary: 鞋类ai识别;裁剪边距计算
+Version: 4.3.6
+Summary: 鞋类ai识别
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.4 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.6 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

