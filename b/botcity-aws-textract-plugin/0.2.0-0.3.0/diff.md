# Comparing `tmp/botcity-aws-textract-plugin-0.2.0.tar.gz` & `tmp/botcity-aws-textract-plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/bot-aws-textract-plugin-python/bot-aws-textract-plugin-python/dist/.tmp-4bf89c72/botcity-aws-textract-plugin-", last modified: Tue Mar 28 22:40:13 2023, max compression
+gzip compressed data, was "/home/runner/work/bot-aws-textract-plugin-python/bot-aws-textract-plugin-python/dist/.tmp-ij48y9d_/botcity-aws-textract-plugin-", last modified: Fri Jul 14 00:30:18 2023, max compression
```

## Comparing `botcity-aws-textract-plugin-0.2.0.tar` & `botcity-aws-textract-plugin-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/pdfhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 22:40:13.000000 botcity-aws-textract-plugin-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    80053 2023-03-28 22:40:04.000000 botcity-aws-textract-plugin-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/pdfhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:30:18.000000 botcity-aws-textract-plugin-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80053 2023-07-14 00:30:05.000000 botcity-aws-textract-plugin-0.3.0/versioneer.py
```

### Comparing `botcity-aws-textract-plugin-0.2.0/PKG-INFO` & `botcity-aws-textract-plugin-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-aws-textract-plugin
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://github.com/botcity-dev/bot-aws-textract-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity AWS Textract Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-aws-textract-plugin-0.2.0/README.md` & `botcity-aws-textract-plugin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/pdfhandler.py` & `botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/pdfhandler.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import pypdfium2
 
 
 def pdf_to_image(filepath: str, resolution: int = 72, **kwargs) -> List:
     """
     Convert a PDF to a list PIL Image objects.
+
     Args:
         filepath (str): The PDF file path.
         resolution (int, optional): The resolution to use when converting the PDF to image.
             Defaults to 72.
+
     Returns:
         List: List of Image objects being one for each page of the PDF.
     """
     pages = []
-    with pypdfium2.PdfDocument(input_data=filepath) as pdf:
-        for page_num in range(len(pdf)):
-            page = pdf.get_page(page_num)
-            pil_image = page.render_topil(scale=resolution / 72, **kwargs)
-            pages.append(pil_image)
+
+    pdf = pypdfium2.PdfDocument(filepath)
+
+    for page_num in range(len(pdf)):
+        page = pdf.get_page(page_num)
+        pil_image = page.render(scale=resolution / 72, **kwargs).to_pil()
+        pages.append(pil_image)
     return pages
```

### Comparing `botcity-aws-textract-plugin-0.2.0/botcity/plugins/aws/textract/plugin.py` & `botcity-aws-textract-plugin-0.3.0/botcity/plugins/aws/textract/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,44 +109,48 @@
         if "/pdf" in file_type:
             images.extend(pdf_to_image(filepath, resolution=self._render_rate))
         elif "image/" in file_type:
             images.append(Image.open(filepath))
         else:
             raise ValueError("Invalid file type. Only images and PDFs are accepted.")
 
+        page_heights = []
         for page_idx, page in enumerate(images, start=1):
             buffer = io.BytesIO()
             page.save(buffer, format='PNG')
 
             response = self._client.analyze_document(
                 Document={'Bytes': buffer.getvalue()},
                 FeatureTypes=['FORMS'],
                 **kwargs
             )
 
             page_width, page_height = page.size
+            page_heights.append(page_height)
+
+            page_offset = 0 if page_idx == 1 else page_heights[page_idx - 2]
             for block in response["Blocks"]:
                 if block["BlockType"] == "WORD":
                     self._full_text += block["Text"] + os.linesep
                     bb = block["Geometry"]["BoundingBox"]
 
                     # bb.left * page_width
                     x1 = bb["Left"] * page_width
 
                     # bb.top * page_height
-                    y1 = bb["Top"] * page_height
+                    y1 = (bb["Top"] * page_height) + page_offset
 
                     # bb.width * page_width + (bb.left * page_width)
-                    x4 = (bb["Width"] * page_width) + x1
+                    x3 = (bb["Width"] * page_width) + x1
 
                     # bb.height * page_height + (bb.top * page_height)
-                    y4 = ((bb["Height"] * page_height) + y1)
+                    y3 = ((bb["Height"] * page_height) + y1 + page_offset)
 
                     self._entries.append([
                         block["Text"],
                         x1, y1,
-                        x4, y1,
-                        x1, y4,
-                        x4, y4,
+                        x3, y1,
+                        x3, y3,
+                        x1, y3,
                         page_idx
                     ])
         return self
```

### Comparing `botcity-aws-textract-plugin-0.2.0/botcity_aws_textract_plugin.egg-info/PKG-INFO` & `botcity-aws-textract-plugin-0.3.0/botcity_aws_textract_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botcity-aws-textract-plugin
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://github.com/botcity-dev/bot-aws-textract-plugin-python.git
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # BotCity AWS Textract Plugin - Python
 
 ## 🤖 Computer-vision based UI Automation
```

### Comparing `botcity-aws-textract-plugin-0.2.0/setup.py` & `botcity-aws-textract-plugin-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `botcity-aws-textract-plugin-0.2.0/versioneer.py` & `botcity-aws-textract-plugin-0.3.0/versioneer.py`

 * *Files identical despite different names*

