# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.9.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.9.tar", last modified: Fri Jul 14 04:11:50 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.7.0.tar", last modified: Fri Jul 14 05:52:58 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9.tar` & `hyutils-hyutil-hoyun-lab-0.0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.201114 hyutils-hyutil-hoyun-lab-0.0.6.9/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-07-14 04:11:50.200113 hyutils-hyutil-hoyun-lab-0.0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 04:11:50.201614 hyutils-hyutil-hoyun-lab-0.0.6.9/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-07-14 04:11:23.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.150614 hyutils-hyutil-hoyun-lab-0.0.6.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.189613 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      449 2023-07-14 04:11:23.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/augmentjob.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    15362 2023-06-28 07:08:39.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0    10988 2023-07-14 04:09:42.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.198613 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:58.288539 hyutils-hyutil-hoyun-lab-0.0.7.0/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-07-14 05:52:58.287932 hyutils-hyutil-hoyun-lab-0.0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:52:58.288666 hyutils-hyutil-hoyun-lab-0.0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-14 05:50:11.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:58.263039 hyutils-hyutil-hoyun-lab-0.0.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:58.280538 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      449 2023-07-14 05:50:11.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/augmentjob.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    15735 2023-07-14 05:41:00.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0    10988 2023-07-14 04:09:42.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:58.286538 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-07-14 05:52:58.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-07-14 05:52:58.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:52:58.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 05:52:58.000000 hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.9
+Version: 0.0.7.0
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6.9",
+    version="0.0.7.0",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/augmentjob.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/augmentjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-import xml.etree.ElementTree as ET
+import xml.etree.ElementTree as Et
 from tqdm import tqdm
 import os
 import io
 import random
 import pandas as pd
 import tensorflow as tf
 import numpy as np
 from PIL import Image
 from object_detection.utils import dataset_util
-from collections import namedtuple, OrderedDict
+from collections import namedtuple
 import glob
 import shutil
 import cv2
 
+
 def xml_to_dataframe(path, include_string):
     classes_names = []
 
     classes_names.clear()
     if not os.path.exists(path) or len(include_string) == 0:
         print(f'invalid parameters: {path} {include_string}')
         return
     xml_list = []
     xml_target = os.path.join(path, include_string)
     file_list = glob.glob(xml_target)
     for xml_file in tqdm(file_list, desc=include_string):
         # sprint('---> ', xml_file)
-        tree = ET.parse(xml_file)
+        tree = Et.parse(xml_file)
         root = tree.getroot()
         for member in root.findall('object'):
             classes_names.append(member.find('name').text)
             bndbox = member.find('bndbox')
             value = (root.find('filename').text,
                      int(root.find('size').find('width').text),
                      int(root.find('size').find('height').text),
@@ -42,26 +43,29 @@
             xml_list.append(value)
     column_name = ['filename', 'width', 'height', 'class', 'xmin', 'ymin', 'xmax', 'ymax']
     xml_df = pd.DataFrame(xml_list, columns=column_name)
     classes_names = list(set(classes_names))
     classes_names.sort()
     return xml_df, classes_names
 
+
 """
 설명: 특정 경로와 확장자 정보(*.xml 등)를 입력받아서 입력된 경로의 모든 파일을 대상으로
      coco xml 파일 형식을 가정하고 읽어서 특정 경로 위 폴더에 csv 파일을 생성하고, 
      입력된 label map 파일명으로 입력되었던 특정 경로 바로 위 폴더에 라벨맵을 생성한다.
      
 사용예:
   python 5_xml_to_csv_in_divided_data.py 
     --xml_path=D:\python_work\tf-train-data\faces\new_face_train_label 
     --include_string=01*.xml 
     --output_file=D:\python_work\tf-train-data\faces\new_face_train_label01.csv 
     --labelmap_name=new_face_labelmap_01.pbtxt 
 """
+
+
 def convert_to_csv(xml_path, include_string, output_file, labelmap_path):
 
     xml_df, classes_names = xml_to_dataframe(xml_path, include_string)
 
     # label map 생성
     # labelmap_dir = os.path.dirname(output_file)
     # label_map_path = os.path.join(labelmap_dir, labelmap_name)
@@ -81,19 +85,21 @@
     # csv 파일 생성.
     output_path = os.path.dirname(output_file)
     if not os.path.exists(output_path):
         os.makedirs(output_path, exist_ok=True)
 
     xml_df.to_csv(output_file, index=None)
 
+
 def __split(df, group):
     data = namedtuple('data', ['filename', 'object'])
     gb = df.groupby(group)
     return [data(filename, gb.get_group(x)) for filename, x in zip(gb.groups.keys(), gb.groups)]
 
+
 def create_one_tf_example(group, path, class_dict):
     with tf.io.gfile.GFile(os.path.join(path, '{}'.format(group.filename)), 'rb') as fid:
         encoded_jpg = fid.read()
     encoded_jpg_io = io.BytesIO(encoded_jpg)
     image = Image.open(encoded_jpg_io)
     width, height = image.size
 
@@ -103,25 +109,26 @@
     xmaxs = []
     ymins = []
     ymaxs = []
     classes_text = []
     classes = []
 
     for index, row in group.object.iterrows():
-        if set(['xmin_rel', 'xmax_rel', 'ymin_rel', 'ymax_rel']).issubset(set(row.index)):
+        if {'xmin_rel', 'xmax_rel', 'ymin_rel', 'ymax_rel'}.issubset(set(row.index)):
+        # if set(['xmin_rel', 'xmax_rel', 'ymin_rel', 'ymax_rel']).issubset(set(row.index)):
             xmin = row['xmin_rel']
             xmax = row['xmax_rel']
             ymin = row['ymin_rel']
             ymax = row['ymax_rel']
             xmins.append(xmin)
             xmaxs.append(xmax)
             ymins.append(ymin)
             ymaxs.append(ymax)
-
-        elif set(['xmin', 'xmax', 'ymin', 'ymax']).issubset(set(row.index)):
+        elif {'xmin', 'xmax', 'ymin', 'ymax'}.issubset(set(row.index)):
+        # elif set(['xmin', 'xmax', 'ymin', 'ymax']).issubset(set(row.index)):
             xmn = row['xmin'] / width
             if xmn < 0.0:
                 xmn = 0.0
             elif xmn > 1.0:
                 xmn = 1.0
             xmins.append(xmn)
 
@@ -165,14 +172,15 @@
             'image/object/bbox/xmax': dataset_util.float_list_feature(xmaxs),
             'image/object/bbox/ymin': dataset_util.float_list_feature(ymins),
             'image/object/bbox/ymax': dataset_util.float_list_feature(ymaxs),
             'image/object/class/text': dataset_util.bytes_list_feature(classes_text),
             'image/object/class/label': dataset_util.int64_list_feature(classes), }))
     return tf_example
 
+
 def class_dict_from_pbtxt(pbtxt_path):
     # open file, strip \n, trim lines and keep only
     # lines beginning with id or display_name
 
     with open(pbtxt_path, 'r', encoding='utf-8-sig') as f:
         data = f.readlines()
 
@@ -180,31 +188,33 @@
     if any('display_name:' in s for s in data):
         name_key = 'display_name:'
     elif any('name:' in s for s in data):
         name_key = 'name:'
 
     if name_key is None:
         raise ValueError(
-            "label map does not have class names, provided by values with the 'display_name' or 'name' keys in the contents of the file"
+            "label map does not have class names, provided by values with the 'display_name' \
+            or 'name' keys in the contents of the file"
         )
 
-    data = [l.rstrip('\n').strip() for l in data if 'id:' in l or name_key in l]
+    data = [item.rstrip('\n').strip() for item in data if 'id:' in item or name_key in item]
 
-    ids = [int(l.replace('id:', '')) for l in data if l.startswith('id')]
+    ids = [int(item.replace('id:', '')) for item in data if item.startswith('id')]
     names = [
-        l.replace(name_key, '').replace('"', '').replace("'", '').strip() for l in data
-        if l.startswith(name_key)]
+        item.replace(name_key, '').replace('"', '').replace("'", '').strip() for item in data
+        if item.startswith(name_key)]
 
     # join ids and display_names into a single dictionary
     class_dict = {}
     for i in range(len(ids)):
         class_dict[names[i]] = ids[i]
 
     return class_dict
 
+
 # convert_to_csv(d:\python_work\tf-train-data\faces,
 #                 "new_face_train_label01.csv,new_face_train_label02.csv",
 #                 d:\python_work\tf-train-data\faces\face_label_map.pbtxt,
 #                 d:\python_work\tf-train-data\faces\new_face_images,
 #                 d:\python_work\tf-train-data\faces\new_face_train.tfrecord)
 def convert_to_tfrecord(csv_path, csv_list, pbtxt_path, image_path, output_path):
     image_path = os.path.join(image_path)
@@ -225,20 +235,23 @@
 
         print(f'{csv_input} was processed')
         writer.flush()
 
     writer.close()
     print('Successfully created the TFRecords: {}'.format(output_path))
 
+
 """
 주석이 들어있는 폴더를 입력받아서 xml 파일들을 랜덤으로 섞어서, 훈련 주석 0.8, 테스트 주석 0.2 비율로 나눈후,
 test용 폴더에 test용 xml을, train 폴더에 train용 xml을 복사해준다.
 
 python divide_annotation.py -a .\ANNOTATION_PATH -t1 .\train -t2 .\test
 """
+
+
 def divide_annotation(annotation_path, train_label, test_label):
     if not os.path.exists(annotation_path):
         print('Not Found: {}'.format(annotation_path))
         return
 
     if not os.path.exists(train_label):
         os.makedirs(train_label, exist_ok=True)
@@ -257,15 +270,15 @@
     test_count = total_size - train_count
     print('train:{} test:{}'.format(train_count, test_count))
 
     # progress = tqdm(total_size)
     # idx = 0
     list_range = np.arange(0, total_size)
     for idx in tqdm(list_range, desc='dividing annotations to train & test set'):
-    # while idx < total_size:
+        # while idx < total_size:
         # print(idx, '-', all_anno_list[idx])
         xml_fullpath = all_anno_list[idx]
         if not os.path.exists(xml_fullpath):
             print('Not Found: {}'.format(xml_fullpath))
             # progress.update()
             continue
         if idx < train_count:
@@ -273,52 +286,55 @@
         else:
             target_path = os.path.join(test_label, os.path.basename(all_anno_list[idx]))
 
         if os.path.exists(target_path):
             os.remove(target_path)
         shutil.copy(xml_fullpath, target_path)
 
+
 """
 설명: 입력된 이미지 저장 경로와 csv 파일 경로를 입력받아서, 
   csv의 1라인씩 읽어 width, height, xmin, ymin, xmax, ymax 값을 출력하고,
   대응하는 이미지를 읽어서 width, height를 읽어서 각 값들의 유효성을 체크하여,
   이후 tfrecord로 변환할 데이터의 유효성을 검증하고,
   이미지에 관심영역 box를 그려서 보여준다.
 
 사용예:
   python temp_check_csv.py --image_path=.\images --csv_path=.\data.csv
 """
 
+
 # 각 레코드를 파싱하기 위한 함수 정의
 def parse_record(record):
     # 레코드의 feature 정의
     feature_description = {
         'image/encoded': tf.io.FixedLenFeature([], tf.string),
         'image/object/class/text': tf.io.VarLenFeature(tf.string),
-        'image/object/bbox/xmin' : tf.io.VarLenFeature(tf.float32),
+        'image/object/bbox/xmin': tf.io.VarLenFeature(tf.float32),
         'image/object/bbox/xmax': tf.io.VarLenFeature(tf.float32),
         'image/object/bbox/ymin': tf.io.VarLenFeature(tf.float32),
         'image/object/bbox/ymax': tf.io.VarLenFeature(tf.float32),
-        'image/width' : tf.io.VarLenFeature(tf.int64),
+        'image/width': tf.io.VarLenFeature(tf.int64),
         'image/height': tf.io.VarLenFeature(tf.int64),
-        'image/filename' : tf.io.FixedLenFeature([], tf.string)
+        'image/filename': tf.io.FixedLenFeature([], tf.string)
     }
     # 레코드 파싱
     parsed_record = tf.io.parse_single_example(record, feature_description)
     # 이미지 데이터 디코딩
     image = tf.io.decode_image(parsed_record['image/encoded'])
     # 레이블 추출
     label = parsed_record['image/object/class/text']
     xmin = parsed_record['image/object/bbox/xmin']
     xmax = parsed_record['image/object/bbox/xmax']
     ymin = parsed_record['image/object/bbox/ymin']
     ymax = parsed_record['image/object/bbox/ymax']
     filename = parsed_record['image/filename']
     return image, label, filename, xmin, xmax, ymin, ymax
 
+
 def tfrecord_valid_check(tfrecord_path, mode):
     # for example in tf.io..tf_record_iterator(tfrecord_path):
     #     print(tf.train.Example.FromString(example))
 
     if os.path.exists(tfrecord_path):
         # 지정된 tfrecord 파일에 대한 데이터셋을 만듬.
         dataset = tf.data.TFRecordDataset(tfrecord_path)
@@ -335,30 +351,33 @@
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
             xmin = tf.sparse.to_dense(xmin, default_value=0.0).numpy()
             xmax = tf.sparse.to_dense(xmax, default_value=0.0).numpy()
             ymin = tf.sparse.to_dense(ymin, default_value=0.0).numpy()
             ymax = tf.sparse.to_dense(ymax, default_value=0.0).numpy()
             label = tf.sparse.to_dense(label, default_value='???').numpy()
 
-            if mode == 'print':
+            if mode is not None:
                 for idx in np.arange(0, len(label)):
-                    print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} ymin:{ymin[idx]} ymax:{ymax[idx]}, h:{h} w:{w} c:{c}')
+                    print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} \
+                    ymin:{ymin[idx]} ymax:{ymax[idx]}, h:{h} w:{w} c:{c}')
                 if c != 3:
                     print('---------------------- invalid image\'s channel size ----------------------')
                     cv2.waitKey(0)
             else:
                 # 레이블 출력
                 for idx in np.arange(0, len(label)):
-                    print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} ymin:{ymin[idx]} ymax:{ymax[idx]}')
-                    cv2.rectangle(image, (int(xmin[idx] * w), int(ymin[idx] * h)), (int(xmax[idx] * w), int(ymax[idx] * h)), (255, 255, 0), 2)
+                    print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} \
+                    ymin:{ymin[idx]} ymax:{ymax[idx]}')
+                    cv2.rectangle(image,
+                                  (int(xmin[idx] * w), int(ymin[idx] * h)),
+                                  (int(xmax[idx] * w), int(ymax[idx] * h)),
+                                  (255, 255, 0), 2)
 
                 cv2.imshow('image', image)
 
-
-
         # for d in raw_dataset:
         #     ex = tf.train.Example()
         #     ex.ParseFromString(d.numpy())
         #     m = json.loads(MessageToJson(ex))
         #     print(m['features']['feature'].keys())
 
         # for raw_record in dataset:
@@ -368,8 +387,8 @@
         #     print('-----------------------------------------------------------')
             key = cv2.waitKey(0)
             if key == 27:
                 break
 
 # def merge_multiple_tfrecords(record_list, output_path):
 #     raw_dataset = tf.data.TFRecordDataset(record_list)
-#     merged_dataset = raw_dataset.concatenate(tf.data.TFRecordDataset(output_path))
+#     merged_dataset = raw_dataset.concatenate(tf.data.TFRecordDataset(output_path))
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.9
+Version: 0.0.7.0
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.7.0/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

