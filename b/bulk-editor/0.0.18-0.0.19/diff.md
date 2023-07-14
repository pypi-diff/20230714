# Comparing `tmp/bulk_editor-0.0.18.tar.gz` & `tmp/bulk_editor-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bulk_editor-0.0.18.tar", last modified: Fri Jul 14 18:04:15 2023, max compression
+gzip compressed data, was "dist/bulk_editor-0.0.19.tar", last modified: Fri Jul 14 18:08:58 2023, max compression
```

## Comparing `bulk_editor-0.0.18.tar` & `bulk_editor-0.0.19.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/PKG-INFO
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulkeditor/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     3558 2023-07-14 18:03:20.000000 bulk_editor-0.0.18/bulkeditor/__init__.py
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulk_editor.egg-info/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulk_editor.egg-info/PKG-INFO
--rw-r--r--   0 harinikeshr   (501) admin       (80)      215 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulk_editor.egg-info/SOURCES.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulk_editor.egg-info/requires.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulk_editor.egg-info/top_level.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/bulk_editor.egg-info/dependency_links.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.18/README.md
--rw-r--r--   0 harinikeshr   (501) admin       (80)     4858 2023-07-14 18:04:09.000000 bulk_editor-0.0.18/setup.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 18:04:15.000000 bulk_editor-0.0.18/setup.cfg
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/PKG-INFO
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulkeditor/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     3558 2023-07-14 18:03:20.000000 bulk_editor-0.0.19/bulkeditor/__init__.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       10 2023-07-14 17:16:25.000000 bulk_editor-0.0.19/bulkeditor/Certificate.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)    20953 2023-07-14 08:02:23.000000 bulk_editor-0.0.19/bulkeditor/logo.png
+-rw-r--r--   0 harinikeshr   (501) admin       (80)   167336 2023-07-14 08:02:23.000000 bulk_editor-0.0.19/bulkeditor/Roboto-Bold.ttf
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     1070 2023-07-11 07:16:48.000000 bulk_editor-0.0.19/LICENSE
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulk_editor.egg-info/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulk_editor.egg-info/PKG-INFO
+-rw-r--r--   0 harinikeshr   (501) admin       (80)      297 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulk_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulk_editor.egg-info/requires.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulk_editor.egg-info/top_level.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/bulk_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.19/README.md
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     4821 2023-07-14 18:08:47.000000 bulk_editor-0.0.19/setup.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 18:08:58.000000 bulk_editor-0.0.19/setup.cfg
```

### Comparing `bulk_editor-0.0.18/PKG-INFO` & `bulk_editor-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk_editor
-Version: 0.0.18
+Version: 0.0.19
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.18/bulkeditor/__init__.py` & `bulk_editor-0.0.19/bulkeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.0.18/bulk_editor.egg-info/PKG-INFO` & `bulk_editor-0.0.19/bulk_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-editor
-Version: 0.0.18
+Version: 0.0.19
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.18/README.md` & `bulk_editor-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.0.18/setup.py` & `bulk_editor-0.0.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 #     long_description = fh.read()
 
 # long_description = ""
 # with open("README.md", 'r') as f:
 #   long_description = f.read()
 #   print(long_description)
 
-VERSION = '0.0.18'
+VERSION = '0.0.19'
 DESCRIPTION = 'Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.'
 LONG_DESCRIPTION = 'Batch Processing: Our Image Bulk Editor allows you to process multiple certificates or images simultaneously. No need to edit each file individually; simply upload your entire collection, and the tool will automatically apply your customizations to all the files. Custom Text Fields: Effortlessly insert names, dates, or any other custom text onto your certificates or images. Our editor provides intuitive text fields that can be easily filled with the desired information. You can choose from various fonts, sizes, and colors to match your preferences. Dynamic Variables: To further enhance personalization, we offer dynamic variables that automatically populate data across multiple files. For example, if you have a list of names, our tool can dynamically fill in each name in the designated areas, ensuring accuracy and consistency throughout the batch. Easy Alignment and Positioning: Achieve precise placement of text or custom elements on your certificates or images using our user-friendly alignment and positioning tools. You can adjust the position, rotation, and size of the elements to fit your design perfectly. Preview and Quality Control: Before finalizing your edits, our Image Bulk Editor enables you to preview each modified file. This allows you to ensure that the personalized text or customizations are accurately applied to every certificate or image. Additionally, you can compare the original and edited versions side by side to verify the changes. Export Options: Once you are satisfied with the edits, the Image Bulk Editor provides flexible export options. You can choose to save each edited file individually or merge them into a single document or image, making it convenient for distribution or archiving purposes. Time-Saving Efficiency: Image Bulk Editor is designed to streamline your workflow, significantly reducing the time and effort required for editing multiple certificates or images. Whether you are managing a large event, running an educational program, or organizing corporate achievements, our tool empowers you to process bulk customization quickly and accurately.'
 
 # Setting up
 setup(
     include_package_data=True,
     name="bulk_editor",
     version=VERSION,
     url="https://github.com/Hari-Nikesh-R/Bulk-Image-Editor",
     author="Hari Nikesh R",
     author_email="hari.nikesh.r.cce@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description="# Image Bulk Editor Python Package\n\nThe Image Bulk Editor Python Package provides a convenient and efficient way to customize multiple certificates and images with personalized text or custom elements. This package simplifies the process of batch editing by automating the application of changes across multiple files, saving you valuable time and effort.\n\n# Installation\n\nTo install the Image Bulk Editor Python Package, use the following command:\n```bash\npip install BulkImageEditor\n```\n\n# Usage\n\nTo use the Image Bulk Editor Python Package, follow these steps:\n\n- Import the necessary modules:\n\n```python\nfrom BulkImageEditor import BulkEditor\n```\n\n- Create an instance and start of the bulk editor:\n```python\nBulkEditor()\n```\n\n# Example\n```python\nfrom BulkImageEditor import BulkEditor\nBulkEditor()\n```\n\n# Conclusion\n\nThe Image Bulk Editor Python Package simplifies the task of customizing multiple certificates and images by automating the batch editing process. With its intuitive usage and comprehensive features, this package allows you to achieve consistent and professional results efficiently.\n\n# License\n\nThis is under MIT License.",
-    packages=find_packages(include=['bulkeditor','bulkeditor.*']),
+    packages=find_packages(),
     package_data={'bulkeditor': ['Certificate.txt', 'logo.png', 'Roboto-Bold.ttf']},
     install_requires=['opencv-python', 'Pillow'],
     keywords=['python','editor', 'bulk editor', 'certificate editor', 'image writer'],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: Unix",
```

