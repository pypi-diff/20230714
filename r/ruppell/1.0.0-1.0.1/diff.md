# Comparing `tmp/ruppell-1.0.0.tar.gz` & `tmp/ruppell-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruppell-1.0.0.tar", last modified: Thu Jul 13 19:14:56 2023, max compression
+gzip compressed data, was "ruppell-1.0.1.tar", last modified: Fri Jul 14 17:00:29 2023, max compression
```

## Comparing `ruppell-1.0.0.tar` & `ruppell-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 19:14:45.000000 ruppell-1.0.0/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 19:14:45.000000 ruppell-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 19:14:45.000000 ruppell-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 19:14:56.807659 ruppell-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-13 19:14:45.000000 ruppell-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:45.000000 ruppell-1.0.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/AbstractReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/DocxReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/ImageReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/PdfReader.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 19:14:45.000000 ruppell-1.0.0/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 19:14:45.000000 ruppell-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/ruppell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:14:56.000000 ruppell-1.0.0/ruppell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-13 19:14:45.000000 ruppell-1.0.0/ruppell.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 19:14:56.807659 ruppell-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 19:14:45.000000 ruppell-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:56.807659 ruppell-1.0.0/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:14:45.000000 ruppell-1.0.0/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 19:14:45.000000 ruppell-1.0.0/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:29.826587 ruppell-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 17:00:16.000000 ruppell-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 17:00:16.000000 ruppell-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 17:00:29.826587 ruppell-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-14 17:00:16.000000 ruppell-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:16.000000 ruppell-1.0.1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:29.826587 ruppell-1.0.1/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-14 17:00:16.000000 ruppell-1.0.1/readers/AbstractReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-14 17:00:16.000000 ruppell-1.0.1/readers/DocxReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-14 17:00:16.000000 ruppell-1.0.1/readers/ImageReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 17:00:16.000000 ruppell-1.0.1/readers/PdfReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 17:00:16.000000 ruppell-1.0.1/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 17:00:16.000000 ruppell-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:29.826587 ruppell-1.0.1/ruppell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 17:00:29.000000 ruppell-1.0.1/ruppell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 17:00:29.000000 ruppell-1.0.1/ruppell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:29.000000 ruppell-1.0.1/ruppell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 17:00:29.000000 ruppell-1.0.1/ruppell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 17:00:29.000000 ruppell-1.0.1/ruppell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-14 17:00:16.000000 ruppell-1.0.1/ruppell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 17:00:29.826587 ruppell-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 17:00:16.000000 ruppell-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:29.826587 ruppell-1.0.1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:16.000000 ruppell-1.0.1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-14 17:00:16.000000 ruppell-1.0.1/utils/utils.py
```

### Comparing `ruppell-1.0.0/LICENSE` & `ruppell-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ruppell-1.0.0/PKG-INFO` & `ruppell-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,86 @@
 Metadata-Version: 2.1
 Name: ruppell
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ruppell is a Python package to help in text extraction from documents.
 Home-page: https://github.com/joorgelm/ruppell
-Download-URL: https://github.com/joorgelm/ruppell/archive/1.0.0.tar.gz
+Download-URL: https://github.com/joorgelm/ruppell/archive/1.0.1.tar.gz
 Author: Jorge Melgarejo
 Author-email: melgarejo.colarte@gmail.com
 License: MIT License
 Keywords: ocr text extractor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ruppell: powerful Python text extractor toolkit
 
 ## What is it?
 
-**Ruppell** is a Python package to help in documents' text extraction.
+**Ruppell** is a Python wrapper to help in documents' text extraction.
+
+![](./assets/ruppell.gif)
 
 ## Main Features
 Here are just a few of the things that ruppell does well:
 
   - Create datasets from multiple files.
   - Extract documents' text (pdf, docx, jpeg, jpg, png).
   - Create Pandas dataframe from documents' folder.
   - Convert documents to .txt files
 
 ## Where to get it
 
-Binary installers for the latest released version are available at the [Python
-package index](https://pypi.org/project/ruppell/).
+Binary installers for the latest released version are available at the [Pypi](https://pypi.org/project/ruppell/).
 
 ```sh
 pip install ruppell
 ```
 
-## Dependencies
-- [Pillow](https://github.com/python-pillow/Pillow)
-- [Pytesseract](https://github.com/madmaze/pytesseract)
-- [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)
-- [Docx2txt](https://github.com/ankushshah89/python-docx2txt)
-- [Pandas](https://github.com/pandas-dev/pandas)
+## Requisites
+To run Ruppell you need
+
+- [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 - Python >= 3.6
 
+## How to use
+
+```python
+import ruppell
+
+
+# Configure your documents language, defaults to eng if not specified!
+ruppell.setup_language(language='eng')
+
+
+# Extract text from pdf
+text = ruppell.pdf_to_string(file_path='file_path.pdf')
+
+
+# Extract text from docx
+text = ruppell.docx_to_string(file_path='file_path.docx')
+
+
+# Extract text from image
+text = ruppell.image_to_string(file_path='file_path.jpeg')
+
+
+# Create pandas dataframe from documents folder
+dataframe = ruppell.folder_to_dataframe(folder_path='folder_path')
+
+
+# Create dict from documents folder
+dict_out = ruppell.folder_to_dict(folder_path='folder_path')
+
+
+# Create .txt files from documents folder
+# A folder ./out_{now_in_timestamp} will created in the same path of folder_path
+path_to_out = ruppell.folder_to_txt(folder_path='folder_path')
+
+```
+
 ## Example
 
 ```
 >>> import ruppell
 >>> ruppell.image_to_string('image.png')
 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer id bibendum sapien.'
 ```
```

### Comparing `ruppell-1.0.0/README.md` & `ruppell-1.0.1/ruppell.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,48 @@
+Metadata-Version: 2.1
+Name: ruppell
+Version: 1.0.1
+Summary: Ruppell is a Python package to help in text extraction from documents.
+Home-page: https://github.com/joorgelm/ruppell
+Download-URL: https://github.com/joorgelm/ruppell/archive/1.0.1.tar.gz
+Author: Jorge Melgarejo
+Author-email: melgarejo.colarte@gmail.com
+License: MIT License
+Keywords: ocr text extractor
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Ruppell: powerful Python text extractor toolkit
 
 ## What is it?
 
-**Ruppell** is a Python package to help in documents' text extraction.
+**Ruppell** is a Python wrapper to help in documents' text extraction.
+
+![](./assets/ruppell.gif)
 
 ## Main Features
 Here are just a few of the things that ruppell does well:
 
   - Create datasets from multiple files.
   - Extract documents' text (pdf, docx, jpeg, jpg, png).
   - Create Pandas dataframe from documents' folder.
   - Convert documents to .txt files
 
 ## Where to get it
 
-Binary installers for the latest released version are available at the [Python
-package index](https://pypi.org/project/ruppell/).
+Binary installers for the latest released version are available at the [Pypi](https://pypi.org/project/ruppell/).
 
 ```sh
 pip install ruppell
 ```
 
-## Dependencies
-- [Pillow](https://github.com/python-pillow/Pillow)
-- [Pytesseract](https://github.com/madmaze/pytesseract)
-- [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)
-- [Docx2txt](https://github.com/ankushshah89/python-docx2txt)
-- [Pandas](https://github.com/pandas-dev/pandas)
+## Requisites
+To run Ruppell you need
+
+- [Tesseract OCR](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 - Python >= 3.6
 
 ## How to use
 
 ```python
 import ruppell
```

### Comparing `ruppell-1.0.0/ruppell.py` & `ruppell-1.0.1/ruppell.py`

 * *Files identical despite different names*

### Comparing `ruppell-1.0.0/setup.py` & `ruppell-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
-with open("DESCRIPTION.md", "r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 PACKAGE_NAME = 'ruppell'
 PACKAGES = ['', 'readers', 'utils']
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = "Ruppell is a Python package to help in text extraction from documents."
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     url='https://github.com/joorgelm/ruppell',
     download_url=f'https://github.com/joorgelm/ruppell/archive/{VERSION}.tar.gz',
```

