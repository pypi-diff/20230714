# Comparing `tmp/scPANTHEON-0.3.4.tar.gz` & `tmp/scPANTHEON-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.4.tar", last modified: Fri Jul 14 07:15:41 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.5.tar", last modified: Fri Jul 14 07:18:26 2023, max compression
```

## Comparing `scPANTHEON-0.3.4.tar` & `scPANTHEON-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:15:41.528266 scPANTHEON-0.3.4/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-07-14 07:15:41.527307 scPANTHEON-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:15:41.521680 scPANTHEON-0.3.4/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-14 07:15:41.000000 scPANTHEON-0.3.4/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-14 07:15:41.000000 scPANTHEON-0.3.4/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:15:41.000000 scPANTHEON-0.3.4/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-14 07:15:41.000000 scPANTHEON-0.3.4/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-07-14 07:15:41.000000 scPANTHEON-0.3.4/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 07:15:41.000000 scPANTHEON-0.3.4/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 07:15:41.525434 scPANTHEON-0.3.4/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.4/scpantheon/__init__.py
--rw-rw-rw-   0        0        0     1182 2023-07-12 11:48:35.000000 scPANTHEON-0.3.4/scpantheon/main.py
--rw-rw-rw-   0        0        0    66184 2023-07-13 12:12:07.000000 scPANTHEON-0.3.4/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2023-07-14 07:15:41.528266 scPANTHEON-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-07-14 07:14:05.000000 scPANTHEON-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:18:26.864931 scPANTHEON-0.3.5/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-07-14 07:18:26.863928 scPANTHEON-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:18:26.859043 scPANTHEON-0.3.5/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-14 07:18:26.000000 scPANTHEON-0.3.5/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-14 07:18:26.000000 scPANTHEON-0.3.5/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:18:26.000000 scPANTHEON-0.3.5/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-14 07:18:26.000000 scPANTHEON-0.3.5/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-07-14 07:18:26.000000 scPANTHEON-0.3.5/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 07:18:26.000000 scPANTHEON-0.3.5/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 07:18:26.862530 scPANTHEON-0.3.5/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.5/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     1220 2023-07-14 07:17:42.000000 scPANTHEON-0.3.5/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66195 2023-07-14 07:16:49.000000 scPANTHEON-0.3.5/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:18:26.864931 scPANTHEON-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-07-14 07:16:39.000000 scPANTHEON-0.3.5/setup.py
```

### Comparing `scPANTHEON-0.3.4/scpantheon/main.py` & `scPANTHEON-0.3.5/scpantheon/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''from multiprocessing import freeze_support
 freeze_support()'''
 
 from bokeh.server.server import Server
 import multiprocessing
 import warnings
 
-from app import bokeh_qt
-from front_end import data_qt
+from scpantheon.app import bokeh_qt
+from scpantheon.front_end import data_qt
 
 class ImportWarning(Warning):
     def __init__(self, message):
         self.message = message
     def __str__(self):
         return repr(self.message)
 
 try: 
-    import source # import from online
+    from scpantheon import source # import from online
 except:
     warnings.warn('source import failed',ImportWarning)
 
 def run():
     global server
     print('Opening Bokeh application on http://localhost:5006/')
     server = Server({'/': source.main}, allow_websocket_origin=["localhost:5006"], port=5006, show=False, num_procs=1)
```

### Comparing `scPANTHEON-0.3.4/scpantheon/source.py` & `scPANTHEON-0.3.5/scpantheon/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # from new_func import new_layout
 # from main3 import change_class_color
 
 import os, sys, io
 import importlib
 from PyQt5.QtWidgets import *
 # import mysql.connector
-from front_end import save_qt
+from scpantheon.front_end import save_qt
 from appdirs import AppDirs
 import requests, zipfile, shutil
 
 
 TOOLTIPS = [
         ("(x,y)", "($x, $y)"),
         ("color", "@color"),
```

### Comparing `scPANTHEON-0.3.4/setup.py` & `scPANTHEON-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.4',#版本
+    version='0.3.5',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas==1.4.4','anndata==0.8.0','colorcet==3.0.0','scanpy==1.9.1','numpy==1.21.5','PyQt5==5.15.9','PyQtWebEngine==5.15.6',
                         'appdirs==1.4.4',], # 依赖包,如果没有,可以不要
```

