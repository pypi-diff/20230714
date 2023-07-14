# Comparing `tmp/bulk_editor-0.0.8.tar.gz` & `tmp/bulk_editor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bulk_editor-0.0.8.tar", last modified: Fri Jul 14 17:24:42 2023, max compression
+gzip compressed data, was "dist/bulk_editor-0.0.9.tar", last modified: Fri Jul 14 17:28:02 2023, max compression
```

## Comparing `bulk_editor-0.0.8.tar` & `bulk_editor-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/PKG-INFO
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulkeditor/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     3476 2023-07-14 17:24:25.000000 bulk_editor-0.0.8/bulkeditor/__init__.py
-drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulk_editor.egg-info/
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulk_editor.egg-info/PKG-INFO
--rw-r--r--   0 harinikeshr   (501) admin       (80)      215 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulk_editor.egg-info/SOURCES.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulk_editor.egg-info/requires.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulk_editor.egg-info/top_level.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/bulk_editor.egg-info/dependency_links.txt
--rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.8/README.md
--rw-r--r--   0 harinikeshr   (501) admin       (80)     4704 2023-07-14 17:24:38.000000 bulk_editor-0.0.8/setup.py
--rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 17:24:42.000000 bulk_editor-0.0.8/setup.cfg
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/PKG-INFO
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulkeditor/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     3432 2023-07-14 17:27:38.000000 bulk_editor-0.0.9/bulkeditor/__init__.py
+drwxr-xr-x   0 harinikeshr   (501) admin       (80)        0 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulk_editor.egg-info/
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2167 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulk_editor.egg-info/PKG-INFO
+-rw-r--r--   0 harinikeshr   (501) admin       (80)      215 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulk_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       21 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulk_editor.egg-info/requires.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       11 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulk_editor.egg-info/top_level.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)        1 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/bulk_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     2356 2023-07-14 10:57:13.000000 bulk_editor-0.0.9/README.md
+-rw-r--r--   0 harinikeshr   (501) admin       (80)     4704 2023-07-14 17:27:56.000000 bulk_editor-0.0.9/setup.py
+-rw-r--r--   0 harinikeshr   (501) admin       (80)       38 2023-07-14 17:28:02.000000 bulk_editor-0.0.9/setup.cfg
```

### Comparing `bulk_editor-0.0.8/PKG-INFO` & `bulk_editor-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk_editor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.8/bulkeditor/__init__.py` & `bulk_editor-0.0.9/bulkeditor/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 5. Make it as a Compiler package
 '''
 
 class GetImageAxisAndCreateImage:
 	
 	def createImage(self,path,x,y, fontColor):
 		directory_to_save = filedialog.askdirectory()
-		certificateFont= ImageFont.truetype('bulkeditor/Roboto-Bold.ttf',42)
+		certificateFont= ImageFont.truetype('Roboto-Bold.ttf',42)
 		#certificateFont= ImageFont.truetype(r'C:\\Windows\\Fonts\\Arial',42)
 		nameList=[]
 		certificateName = []
-		file = open("bulkeditor/Certificate.txt","r")
+		file = open("Certificate.txt","r")
 		nameList = file.readlines()
 		file.close
 		for i in nameList:
 			certificateName.append(i.replace("\n","").strip())
 		for i in certificateName:
 			certificateImage = ImageEdit.open(path) 
 			editableImage = ImageDraw.Draw(certificateImage)    
@@ -85,24 +85,24 @@
 		cv2.destroyAllWindows()
 
 class BulkEditor:
 
 	def select_image(self):
 		global windowA, windowB
 		self.text = self.textField.get("1.0", "end-1c")
-		with open("bulkeditor/Certificate.txt", 'w') as file:
+		with open("Certificate.txt", 'w') as file:
 			file.write(self.text)
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
```

### Comparing `bulk_editor-0.0.8/bulk_editor.egg-info/PKG-INFO` & `bulk_editor-0.0.9/bulk_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-editor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.
 Home-page: https://github.com/Hari-Nikesh-R/Bulk-Image-Editor
 Author: Hari Nikesh R
 Author-email: hari.nikesh.r.cce@gmail.com
 License: UNKNOWN
 Description: # Image Bulk Editor Python Package
```

### Comparing `bulk_editor-0.0.8/README.md` & `bulk_editor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bulk_editor-0.0.8/setup.py` & `bulk_editor-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     long_description = fh.read()
 
 # long_description = ""
 # with open("README.md", 'r') as f:
 #   long_description = f.read()
 #   print(long_description)
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Transforming multiple certificates and images with personalized text has never been easier thanks to the all-new Image Bulk Editor.'
 LONG_DESCRIPTION = 'Batch Processing: Our Image Bulk Editor allows you to process multiple certificates or images simultaneously. No need to edit each file individually; simply upload your entire collection, and the tool will automatically apply your customizations to all the files. Custom Text Fields: Effortlessly insert names, dates, or any other custom text onto your certificates or images. Our editor provides intuitive text fields that can be easily filled with the desired information. You can choose from various fonts, sizes, and colors to match your preferences. Dynamic Variables: To further enhance personalization, we offer dynamic variables that automatically populate data across multiple files. For example, if you have a list of names, our tool can dynamically fill in each name in the designated areas, ensuring accuracy and consistency throughout the batch. Easy Alignment and Positioning: Achieve precise placement of text or custom elements on your certificates or images using our user-friendly alignment and positioning tools. You can adjust the position, rotation, and size of the elements to fit your design perfectly. Preview and Quality Control: Before finalizing your edits, our Image Bulk Editor enables you to preview each modified file. This allows you to ensure that the personalized text or customizations are accurately applied to every certificate or image. Additionally, you can compare the original and edited versions side by side to verify the changes. Export Options: Once you are satisfied with the edits, the Image Bulk Editor provides flexible export options. You can choose to save each edited file individually or merge them into a single document or image, making it convenient for distribution or archiving purposes. Time-Saving Efficiency: Image Bulk Editor is designed to streamline your workflow, significantly reducing the time and effort required for editing multiple certificates or images. Whether you are managing a large event, running an educational program, or organizing corporate achievements, our tool empowers you to process bulk customization quickly and accurately.'
 
 # Setting up
 setup(
     name="bulk_editor",
     version=VERSION,
```

