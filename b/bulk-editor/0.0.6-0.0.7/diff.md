# Comparing `tmp/bulk_editor-0.0.6.tar.gz` & `tmp/bulk_editor-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bulk_editor-0.0.6.tar", last modified: Fri Jul 14 16:54:58 2023, max compression
+gzip compressed data, was "dist/bulk_editor-0.0.7.tar", last modified: Fri Jul 14 17:18:32 2023, max compression
```

## Comparing `bulk_editor-0.0.6.tar` & `bulk_editor-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/PKG-INFO
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/bulk_editor.egg-info/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/bulk_editor.egg-info/PKG-INFO
--rw-r--r--   0 harinikeshr   (501) admin       (80)      192 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/bulk_editor.egg-info/SOURCES.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/bulk_editor.egg-info/requires.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/bulk_editor.egg-info/top_level.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/bulk_editor.egg-info/dependency_links.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.6/README.md
--rw-r--r--   0 harinikeshr   (501) admin       (80)     4704 2023-07-14 16:54:45.000000 bulk_editor-0.0.6/setup.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 16:54:58.000000 bulk_editor-0.0.6/setup.cfg
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/PKG-INFO
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulkeditor/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     3476 2023-07-14 17:16:08.000000 bulk_editor-0.0.7/bulkeditor/bulk_editor.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       35 2023-07-14 17:17:44.000000 bulk_editor-0.0.7/bulkeditor/__init__.py
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulk_editor.egg-info/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulk_editor.egg-info/PKG-INFO
+-rw-r--r--   0 harinikeshr   (501) admin       (80)      241 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulk_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulk_editor.egg-info/requires.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulk_editor.egg-info/top_level.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/bulk_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.7/README.md
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     4704 2023-07-14 17:18:20.000000 bulk_editor-0.0.7/setup.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 17:18:32.000000 bulk_editor-0.0.7/setup.cfg
```

### Comparing `bulk_editor-0.0.6/PKG-INFO` & `bulk_editor-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk_editor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.6/bulk_editor.egg-info/PKG-INFO` & `bulk_editor-0.0.7/bulk_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-editor
-Version: 0.0.6
+Version: 0.0.7
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.6/README.md` & `bulk_editor-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.0.6/setup.py` & `bulk_editor-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     long_description = fh.read()
 
 # long_description = ""
 # with open("README.md", 'r') as f:
 #   long_description = f.read()
 #   print(long_description)
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.'
 LONG_DESCRIPTION = 'Batch Processing: Our Image Bulk Editor allows you to process multiple certificates or images simultaneously. No need to edit each file individually; simply upload your entire collection, and the tool will automatically apply your customizations to all the files. Custom Text Fields: Effortlessly insert names, dates, or any other custom text onto your certificates or images. Our editor provides intuitive text fields that can be easily filled with the desired information. You can choose from various fonts, sizes, and colors to match your preferences. Dynamic Variables: To further enhance personalization, we offer dynamic variables that automatically populate data across multiple files. For example, if you have a list of names, our tool can dynamically fill in each name in the designated areas, ensuring accuracy and consistency throughout the batch. Easy Alignment and Positioning: Achieve precise placement of text or custom elements on your certificates or images using our user-friendly alignment and positioning tools. You can adjust the position, rotation, and size of the elements to fit your design perfectly. Preview and Quality Control: Before finalizing your edits, our Image Bulk Editor enables you to preview each modified file. This allows you to ensure that the personalized text or customizations are accurately applied to every certificate or image. Additionally, you can compare the original and edited versions side by side to verify the changes. Export Options: Once you are satisfied with the edits, the Image Bulk Editor provides flexible export options. You can choose to save each edited file individually or merge them into a single document or image, making it convenient for distribution or archiving purposes. Time-Saving Efficiency: Image Bulk Editor is designed to streamline your workflow, significantly reducing the time and effort required for editing multiple certificates or images. Whether you are managing a large event, running an educational program, or organizing corporate achievements, our tool empowers you to process bulk customization quickly and accurately.'
 
 # Setting up
 setup(
     name="bulk_editor",
     version=VERSION,
```

