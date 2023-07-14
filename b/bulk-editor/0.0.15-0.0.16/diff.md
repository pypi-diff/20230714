# Comparing `tmp/bulk_editor-0.0.15.tar.gz` & `tmp/bulk_editor-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bulk_editor-0.0.15.tar", last modified: Fri Jul 14 17:55:34 2023, max compression
+gzip compressed data, was "dist/bulk_editor-0.0.16.tar", last modified: Fri Jul 14 18:00:18 2023, max compression
```

## Comparing `bulk_editor-0.0.15.tar` & `bulk_editor-0.0.16.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/PKG-INFO
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulkeditor/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     3487 2023-07-14 17:36:52.000000 bulk_editor-0.0.15/bulkeditor/__init__.py
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulk_editor.egg-info/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulk_editor.egg-info/PKG-INFO
--rw-r--r--   0 harinikeshr   (501) admin       (80)      215 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulk_editor.egg-info/SOURCES.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulk_editor.egg-info/requires.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulk_editor.egg-info/top_level.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/bulk_editor.egg-info/dependency_links.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.15/README.md
--rw-r--r--   0 harinikeshr   (501) admin       (80)     4858 2023-07-14 17:55:26.000000 bulk_editor-0.0.15/setup.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 17:55:34.000000 bulk_editor-0.0.15/setup.cfg
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/PKG-INFO
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulkeditor/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     3464 2023-07-14 17:59:51.000000 bulk_editor-0.0.16/bulkeditor/__init__.py
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulk_editor.egg-info/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2168 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulk_editor.egg-info/PKG-INFO
+-rw-r--r--   0 harinikeshr   (501) admin       (80)      215 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulk_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulk_editor.egg-info/requires.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulk_editor.egg-info/top_level.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/bulk_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.16/README.md
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     4858 2023-07-14 17:59:49.000000 bulk_editor-0.0.16/setup.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 18:00:18.000000 bulk_editor-0.0.16/setup.cfg
```

### Comparing `bulk_editor-0.0.15/PKG-INFO` & `bulk_editor-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk_editor
-Version: 0.0.15
+Version: 0.0.16
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.15/bulkeditor/__init__.py` & `bulk_editor-0.0.16/bulkeditor/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,23 +93,22 @@
 		path = filedialog.askopenfilename()
 		if len(path) > 0:
 			image = GetImageAxisAndCreateImage(path)
 
 	def __init__(self):
 		root = Tk()
 		root.title("DoSmartie - Bulk edit images")
-		ico =  ImageEdit.open('bulkeditor/logo.png')
+		ico =  ImageEdit.open('logo.png')
 		photo = ImageTk.PhotoImage(ico)
 		root.wm_iconphoto(False, photo)
 		root.geometry("360x360")  
 		heading = Label(text="Enter the data to be added")
 		label = Label(text="Each image will be created from a single line of text.")
 		self.textField = Text(root, height = 24, width = 52)
 		panelA = None
 		panelB = None
 		btn = Button(root, text="Select an image", command=self.select_image)
 		btn.pack(side="bottom", fill="both", expand="no", padx="10", pady="10")
 		heading.pack()
 		label.pack()
 		self.textField.pack()
 		root.mainloop()
-BulkEditor()
```

### Comparing `bulk_editor-0.0.15/bulk_editor.egg-info/PKG-INFO` & `bulk_editor-0.0.16/bulk_editor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-editor
-Version: 0.0.15
+Version: 0.0.16
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.15/README.md` & `bulk_editor-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.0.15/setup.py` & `bulk_editor-0.0.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     long_description = fh.read()
 
 # long_description = ""
 # with open("README.md", 'r') as f:
 #   long_description = f.read()
 #   print(long_description)
 
-VERSION = '0.0.15'
+VERSION = '0.0.16'
 DESCRIPTION = 'Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.'
 LONG_DESCRIPTION = 'Batch Processing: Our Image Bulk Editor allows you to process multiple certificates or images simultaneously. No need to edit each file individually; simply upload your entire collection, and the tool will automatically apply your customizations to all the files. Custom Text Fields: Effortlessly insert names, dates, or any other custom text onto your certificates or images. Our editor provides intuitive text fields that can be easily filled with the desired information. You can choose from various fonts, sizes, and colors to match your preferences. Dynamic Variables: To further enhance personalization, we offer dynamic variables that automatically populate data across multiple files. For example, if you have a list of names, our tool can dynamically fill in each name in the designated areas, ensuring accuracy and consistency throughout the batch. Easy Alignment and Positioning: Achieve precise placement of text or custom elements on your certificates or images using our user-friendly alignment and positioning tools. You can adjust the position, rotation, and size of the elements to fit your design perfectly. Preview and Quality Control: Before finalizing your edits, our Image Bulk Editor enables you to preview each modified file. This allows you to ensure that the personalized text or customizations are accurately applied to every certificate or image. Additionally, you can compare the original and edited versions side by side to verify the changes. Export Options: Once you are satisfied with the edits, the Image Bulk Editor provides flexible export options. You can choose to save each edited file individually or merge them into a single document or image, making it convenient for distribution or archiving purposes. Time-Saving Efficiency: Image Bulk Editor is designed to streamline your workflow, significantly reducing the time and effort required for editing multiple certificates or images. Whether you are managing a large event, running an educational program, or organizing corporate achievements, our tool empowers you to process bulk customization quickly and accurately.'
 
 # Setting up
 setup(
     include_package_data=True,
     name="bulk_editor",
```

