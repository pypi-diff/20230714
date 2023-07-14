# Comparing `tmp/scrab_img_from_ligthshot-2.1.0.tar.gz` & `tmp/scrab_img_from_ligthshot-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrab_img_from_ligthshot-2.1.0.tar", max compression
+gzip compressed data, was "scrab_img_from_ligthshot-2.2.0.tar", max compression
```

## Comparing `scrab_img_from_ligthshot-2.1.0.tar` & `scrab_img_from_ligthshot-2.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10173 2023-06-07 15:41:05.465902 scrab_img_from_ligthshot-2.1.0/LICENSE
--rw-r--r--   0        0        0     2098 2023-07-12 21:20:22.812262 scrab_img_from_ligthshot-2.1.0/README.md
--rw-r--r--   0        0        0      530 2023-07-14 02:17:15.888282 scrab_img_from_ligthshot-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-14 02:08:42.347699 scrab_img_from_ligthshot-2.1.0/silf/__init__.py
--rw-r--r--   0        0        0      518 2023-07-14 02:17:45.200351 scrab_img_from_ligthshot-2.1.0/silf/cli.py
--rwxr-xr-x   0        0        0     2945 2023-07-14 02:17:45.212350 scrab_img_from_ligthshot-2.1.0/silf/main.py
--rw-r--r--   0        0        0     3873 2023-07-14 02:08:42.355698 scrab_img_from_ligthshot-2.1.0/silf/scrab_img_from_lightshot.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 scrab_img_from_ligthshot-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-07 15:41:05.465902 scrab_img_from_ligthshot-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2122 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/README.md
+-rw-r--r--   0        0        0      640 2023-07-14 17:28:50.230603 scrab_img_from_ligthshot-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/cli.py
+-rwxr-xr-x   0        0        0     2977 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/main.py
+-rw-r--r--   0        0        0     3873 2023-07-14 17:22:58.126647 scrab_img_from_ligthshot-2.2.0/src/silf/scrab_img_from_lightshot.py
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 scrab_img_from_ligthshot-2.2.0/PKG-INFO
```

### Comparing `scrab_img_from_ligthshot-2.1.0/LICENSE` & `scrab_img_from_ligthshot-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrab_img_from_ligthshot-2.1.0/README.md` & `scrab_img_from_ligthshot-2.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,75 +13,81 @@
 but changing it manually is uncomfortable. To automatic this uncomfortable process, I created this project.
 
 Script will download certain count(that you indicate) of images
 ___
 
 ## Installing
 
-### With Poetry
+### Poetry
 You have to have installed poetry 1.4 or higher.
 
-Install packages:
+Spawn virtual environment:
 ```
-poetry install
+poetry shell 
 ```
 
-Activate virtual environment:
+Install requirements
 ```
-poetry shell
+poetry install
 ```
 
-### With Pip
+### PyPi
 You have to have installed python 3.7 or higher. 
 
 Create virtual environment: 
 ```
-python -m venv venv 
+python3 -m venv env 
 ```
-If didn't work:
+
+Then activate(launch) virtual environment: 
+- **Linux**: `source env/bin/activate`
+
 ```
-python3 -m venv venv 
+pip3 install scrab-img-from-ligthshot
 ```
 
-Then activate(launch) virtual environmen: 
-- **Linux**: `source venv/bin/activate`
 
-Then launch this command in the ***root***(scrab-img-from-lightshot/) project's folder:
+### Source
+Clone repository:
 ```
-pip install -r requirements.txt
+git clone git@github.com:Transparency010101/scrab-img-from-ligthshot.git
 ```
-That command will install needed libraries.
 
+```
+cd scrab-img-from-ligthshot/
+```
 
-## Usage
-See more in help: `python3 src/main.py -h`
+Create virtual environment: 
+```
+python3 -m venv env 
+```
 
-### Launch program:
+Then activate(launch) virtual environment: 
+- **Linux**: `source env/bin/activate`
 
-Python:
 ```
-python3 src/main.py 10 
+python3 setup.py install
 ```
-
+If occurred permision denied error:
 ```
-python3 src/main.py 3 -D
+sudo python3 setup.py install
 ```
+## Usage
 
-Poetry:
+PyPi or Source:
 ```
-poetry run python3 src/main.py 7 
+silf -h
 ```
-or
+
+Poetry:
 ```
-poetry run python3 src/main.py 2 -D
+poetry run silf -h
 ```
-When program finished, open the project's folder `scrab-img-from-lightshot/img/`, and there will be images.
+When program finished, open the project's folder `img/`, and there will be images.
 
 ## Notes
 Idea for the project I got [there](https://www.youtube.com/watch?v=OUki27mlwOw) 4:30.
 
 I'm developing this project only for my practise, maybe there is fools ideas,
 controversial points regarding the development, not serious thing, attitude towards whole development
 
 P.S. Не бейте за англиский.
-
-
```

### Comparing `scrab_img_from_ligthshot-2.1.0/silf/main.py` & `scrab_img_from_ligthshot-2.2.0/src/silf/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,26 +18,25 @@
 Foreword:
     I'm trying to observe standards of code writing on Python(PEP8)
 
 Usage:
     See in README file
 
 Functions:
-    create_img_folder_if_not_exist()
+    create_img_folder_if_not_exist
     delete_all_images
+    start_downloading
     main
 """
 
 import time
 import os
-import sys
-
 
-from silf.scrab_img_from_lightshot import ScrabImgFromLightShot
-from silf.cli import cli
+from .scrab_img_from_lightshot import ScrabImgFromLightShot
+from .cli import cli
 
 
 def create_img_folder_if_not_exist():
     """Create folder img/ if it doesn't exist.
 
     If folder img/ doesn't exist will be an error, so need to check this every
     time when program starts.
@@ -78,15 +77,14 @@
     Arguments:
         number_of_images (int): number of images, that need to download
         debug_mod (bool): turn on/off debug mod
 
     Returns:
         None
     """
-
     # While this code executing, sometimes errors occur and that stop program
     # that's why code wrapped in try/except, but there is nuance, bugs that I
     # accidentally made while developing, are not shown, so there is debug mod
     # in function
     while number_of_images != len(os.listdir("img/")):
         try:
             ScrabImgFromLightShot.download_img()
@@ -94,14 +92,15 @@
             if debug_mod:
                 print("SOMETHING WENT WRONG!:")
                 print(error)
             pass
 
 
 def main():
+    """Enter point in program"""
     start_program_time = time.time()
 
     cli_args = cli()
     create_img_folder_if_not_exist()
     delete_all_images(cli_args.delete_images)
     start_downloading(cli_args.count_of_images)
```

### Comparing `scrab_img_from_ligthshot-2.1.0/silf/scrab_img_from_lightshot.py` & `scrab_img_from_ligthshot-2.2.0/src/silf/scrab_img_from_lightshot.py`

 * *Files identical despite different names*

### Comparing `scrab_img_from_ligthshot-2.1.0/PKG-INFO` & `scrab_img_from_ligthshot-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: scrab-img-from-ligthshot
-Version: 2.1.0
+Version: 2.2.0
 Summary: scrab images from ligthshot (i don't know is this legal)
+Home-page: https://github.com/Transparency010101/scrab-img-from-ligthshot
+License: Apache-2.0
 Author: ossys
 Author-email: ossys1010110@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
+Project-URL: Repository, https://github.com/Transparency010101/scrab-img-from-ligthshot
 Description-Content-Type: text/markdown
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry)
 ![Static Badge](https://img.shields.io/badge/poetry-1.4%2B-green)
 ![Static Badge](https://img.shields.io/badge/only_linux_support-green)
 ![Static Badge](https://img.shields.io/badge/pass_tests-none-red)
 ![GitHub issues](https://img.shields.io/github/issues-raw/Transparency010101/scrab-img-from-ligthshot)
@@ -29,76 +33,82 @@
 but changing it manually is uncomfortable. To automatic this uncomfortable process, I created this project.
 
 Script will download certain count(that you indicate) of images
 ___
 
 ## Installing
 
-### With Poetry
+### Poetry
 You have to have installed poetry 1.4 or higher.
 
-Install packages:
+Spawn virtual environment:
 ```
-poetry install
+poetry shell 
 ```
 
-Activate virtual environment:
+Install requirements
 ```
-poetry shell
+poetry install
 ```
 
-### With Pip
+### PyPi
 You have to have installed python 3.7 or higher. 
 
 Create virtual environment: 
 ```
-python -m venv venv 
+python3 -m venv env 
 ```
-If didn't work:
+
+Then activate(launch) virtual environment: 
+- **Linux**: `source env/bin/activate`
+
 ```
-python3 -m venv venv 
+pip3 install scrab-img-from-ligthshot
 ```
 
-Then activate(launch) virtual environmen: 
-- **Linux**: `source venv/bin/activate`
 
-Then launch this command in the ***root***(scrab-img-from-lightshot/) project's folder:
+### Source
+Clone repository:
 ```
-pip install -r requirements.txt
+git clone git@github.com:Transparency010101/scrab-img-from-ligthshot.git
 ```
-That command will install needed libraries.
 
+```
+cd scrab-img-from-ligthshot/
+```
 
-## Usage
-See more in help: `python3 src/main.py -h`
+Create virtual environment: 
+```
+python3 -m venv env 
+```
 
-### Launch program:
+Then activate(launch) virtual environment: 
+- **Linux**: `source env/bin/activate`
 
-Python:
 ```
-python3 src/main.py 10 
+python3 setup.py install
 ```
-
+If occurred permision denied error:
 ```
-python3 src/main.py 3 -D
+sudo python3 setup.py install
 ```
+## Usage
 
-Poetry:
+PyPi or Source:
 ```
-poetry run python3 src/main.py 7 
+silf -h
 ```
-or
+
+Poetry:
 ```
-poetry run python3 src/main.py 2 -D
+poetry run silf -h
 ```
-When program finished, open the project's folder `scrab-img-from-lightshot/img/`, and there will be images.
+When program finished, open the project's folder `img/`, and there will be images.
 
 ## Notes
 Idea for the project I got [there](https://www.youtube.com/watch?v=OUki27mlwOw) 4:30.
 
 I'm developing this project only for my practise, maybe there is fools ideas,
 controversial points regarding the development, not serious thing, attitude towards whole development
 
 P.S. Не бейте за англиский.
 
-
-
```

