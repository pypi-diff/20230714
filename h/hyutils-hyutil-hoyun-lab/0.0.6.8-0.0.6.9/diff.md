# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.8.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.8.tar", last modified: Fri Jul 14 03:14:13 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.9.tar", last modified: Fri Jul 14 04:11:50 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:14:13.471311 hyutils-hyutil-hoyun-lab-0.0.6.8/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-07-14 03:14:13.471140 hyutils-hyutil-hoyun-lab-0.0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 03:14:13.471837 hyutils-hyutil-hoyun-lab-0.0.6.8/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-07-14 03:13:47.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:14:13.447307 hyutils-hyutil-hoyun-lab-0.0.6.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 03:14:13.464308 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      449 2023-07-14 03:13:47.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/augmentjob.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    15362 2023-06-28 07:08:39.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     7837 2023-07-14 03:10:12.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:14:13.469814 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-07-14 03:14:13.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-07-14 03:14:13.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:14:13.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 03:14:13.000000 hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.201114 hyutils-hyutil-hoyun-lab-0.0.6.9/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-07-14 04:11:50.200113 hyutils-hyutil-hoyun-lab-0.0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:11:50.201614 hyutils-hyutil-hoyun-lab-0.0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-14 04:11:23.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.150614 hyutils-hyutil-hoyun-lab-0.0.6.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.189613 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      449 2023-07-14 04:11:23.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/augmentjob.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    15362 2023-06-28 07:08:39.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0    10988 2023-07-14 04:09:42.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:11:50.198613 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 04:11:50.000000 hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.8
+Version: 0.0.6.9
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6.8",
+    version="0.0.6.9",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/augmentjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/augmentjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutil_hoyun_lab/xml_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 write_xml
 
 check_xml_and_fix
 
 """
 
+
 def indent(elem, level=0):  # 자료 출처 https://goo.gl/J8VoDK
     i = "\n" + level * " " * 4
     if len(elem):
         if not elem.text or not elem.text.strip():
             elem.text = i + " " * 4
         if not elem.tail or not elem.tail.strip():
             elem.tail = i
@@ -29,14 +30,15 @@
             indent(elem, level + 1)
         if not elem.tail or not elem.tail.strip():
             elem.tail = i
     else:
         if level and (not elem.tail or not elem.tail.strip()):
             elem.tail = i
 
+
 def read_xml(annotation_file_path):
     xml_info = []
     is_ok = False
     if not os.path.exists(annotation_file_path):
         return is_ok, xml_info
 
     tree = ET.parse(annotation_file_path)
@@ -60,14 +62,15 @@
         item.append(bndbox.find('ymax').text) # 7
         xml_info.append(item)
 
     is_ok = True
     # xml_info (class_name, width, height, xmin, ymin, xmax, ymax)
     return is_ok, xml_info
 
+
 def make_xml(class_data, image_filename):
     is_ok = False
 
     if len(class_data) == 0 or image_filename is None:
         print('invalid parameters')
         return is_ok, None
 
@@ -121,14 +124,15 @@
 def write_xml(path, xml_data):
     indent(xml_data, level=0)  # xml 들여쓰기
     b_xml = ET.tostring(xml_data)
     # 주석(xml)기록
     with open(path, 'wb') as f:
         f.write(b_xml)
 
+
 def check_xml_n_fix(xml_path, image_path):
     if os.path.exists(xml_path) and os.path.exists(image_path):
         index = 0
         count = get_entry_count(xml_path, '.xml')
 
         for file in files_ext(xml_path, '.xml'):
             index += 1
@@ -203,7 +207,80 @@
                 if invalid == True: # replace old xml with new xml
                     new_xml_file = xml_file + '.xml'
                     is_ok, data = make_xml(xml_info, image_name)
                     if is_ok == True:
                         write_xml(new_xml_file, data)
                         os.remove(xml_file)
                         shutil.move(new_xml_file, xml_file)
+
+
+def check_csv(image_path, csv_path):
+    if not os.path.exists(image_path)\
+        or not os.path.exists(csv_path):
+        return
+
+    invaild_detected = False
+    idx = 0
+    new_csv_path = csv_path + '.txt'
+    with open(csv_path, 'rt') as f:
+        with open(new_csv_path, 'wt') as new_f:
+            line = f.readline()
+            new_f.write(line)
+            idx += 1
+            print(f'{idx} > {line}')
+            if line:
+                while len(line) > 0:
+                    line = f.readline()
+                    if len(line) == 0:
+                        break
+                    line = line.strip()
+                    if (idx % 1000) == 0:
+                        print(f'{idx}')
+                    idx += 1
+                    # print('{} > {}'.format(idx, line))
+
+                    splited = line.split(',')
+                    if len(splited) != 8:
+                        print(f'invalid item count {splited[0]}')
+                        invaild_detected = True
+                    img_name = splited[0]
+                    img_full_path = os.path.join(image_path, img_name)
+                    img_width = int(splited[1])
+                    img_height = int(splited[2])
+                    img_class = splited[3]
+                    img_xmin = int(splited[4])
+                    img_ymin = int(splited[5])
+                    img_xmax = int(splited[6])
+                    img_ymax = int(splited[7])
+                    # print('{} > {} {} {} {}'
+                    #       .format(img_name, img_xmin / img_width, \
+                    #               img_ymin / img_height, img_xmax / img_width, img_ymax / img_height))
+                    img_mat = cv2.imread(img_full_path)
+                    h, w, c = img_mat.shape
+
+                    if img_height != h or img_width != w:
+                        print(f'not matched width, height {img_name} : {img_height} -> {h} , {img_width} -> {w}')
+                        invaild_detected = True
+
+                    if img_xmin == 0:
+                        img_xmin += 1
+                    if img_ymin == 0:
+                        img_ymin += 1
+                    if img_xmax > w or img_ymax > h:
+                        print(f'xmax or ymax is greater than width or height {img_name} -> {img_xmax} {w} , {img_ymax} {h}  We will fixing')
+                        if (img_xmax - w) == 1:
+                            img_xmax = w
+                        if (img_ymax - h) == 1:
+                            img_ymax = h
+                        invaild_detected = True
+                    if (img_xmax - img_xmin) > img_width or \
+                            (img_ymax - img_ymin) > img_height:
+                        print(f'invalid rectangle {img_name}')
+                        invaild_detected = True
+
+                    new_f.write(f'{img_name},{img_width},{img_height},{img_class},{img_xmin},{img_ymin},{img_xmax},{img_ymax}\n')
+
+
+    if invaild_detected == False:
+        os.remove(new_csv_path)
+    else:
+        print(f'data is invalid. please check the file [{new_csv_path}]')
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.8
+Version: 0.0.6.9
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.8/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.6.9/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

