# Comparing `tmp/scPANTHEON-0.3.6.tar.gz` & `tmp/scPANTHEON-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.3.6.tar", last modified: Fri Jul 14 07:24:03 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.7.tar", last modified: Fri Jul 14 07:29:52 2023, max compression
```

## Comparing `scPANTHEON-0.3.6.tar` & `scPANTHEON-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:24:03.914910 scPANTHEON-0.3.6/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-07-14 07:24:03.914910 scPANTHEON-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:24:03.908839 scPANTHEON-0.3.6/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-14 07:24:03.000000 scPANTHEON-0.3.6/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-14 07:24:03.000000 scPANTHEON-0.3.6/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:24:03.000000 scPANTHEON-0.3.6/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-14 07:24:03.000000 scPANTHEON-0.3.6/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-07-14 07:24:03.000000 scPANTHEON-0.3.6/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 07:24:03.000000 scPANTHEON-0.3.6/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 07:24:03.913100 scPANTHEON-0.3.6/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.6/scpantheon/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-07-14 07:17:42.000000 scPANTHEON-0.3.6/scpantheon/main.py
--rw-rw-rw-   0        0        0    66195 2023-07-14 07:16:49.000000 scPANTHEON-0.3.6/scpantheon/source.py
--rw-rw-rw-   0        0        0       42 2023-07-14 07:24:03.914910 scPANTHEON-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-07-14 07:23:27.000000 scPANTHEON-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:52.157873 scPANTHEON-0.3.7/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-07-14 07:29:52.157873 scPANTHEON-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:52.145506 scPANTHEON-0.3.7/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-14 07:29:51.000000 scPANTHEON-0.3.7/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-07-14 07:29:52.000000 scPANTHEON-0.3.7/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:29:51.000000 scPANTHEON-0.3.7/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-14 07:29:51.000000 scPANTHEON-0.3.7/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-07-14 07:29:51.000000 scPANTHEON-0.3.7/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 07:29:51.000000 scPANTHEON-0.3.7/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:52.149646 scPANTHEON-0.3.7/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.7/scpantheon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:52.152351 scPANTHEON-0.3.7/scpantheon/app/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.7/scpantheon/app/__init__.py
+-rw-rw-rw-   0        0        0     2607 2023-07-05 15:50:04.000000 scPANTHEON-0.3.7/scpantheon/app/bokeh_qt.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:52.155868 scPANTHEON-0.3.7/scpantheon/front_end/
+-rw-rw-rw-   0        0        0        0 2023-07-12 11:30:12.000000 scPANTHEON-0.3.7/scpantheon/front_end/__init__.py
+-rw-rw-rw-   0        0        0     5711 2023-07-13 13:24:16.000000 scPANTHEON-0.3.7/scpantheon/front_end/data_qt.py
+-rw-rw-rw-   0        0        0     3683 2023-07-10 13:33:19.000000 scPANTHEON-0.3.7/scpantheon/front_end/save_qt.py
+-rw-rw-rw-   0        0        0     1220 2023-07-14 07:17:42.000000 scPANTHEON-0.3.7/scpantheon/main.py
+-rw-rw-rw-   0        0        0    66195 2023-07-14 07:16:49.000000 scPANTHEON-0.3.7/scpantheon/source.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:29:52.157873 scPANTHEON-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1179 2023-07-14 07:29:42.000000 scPANTHEON-0.3.7/setup.py
```

### Comparing `scPANTHEON-0.3.6/scpantheon/main.py` & `scPANTHEON-0.3.7/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.6/scpantheon/source.py` & `scPANTHEON-0.3.7/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.3.6/setup.py` & `scPANTHEON-0.3.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.3.6',#版本
+    version='0.3.7',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
-    packages=['scpantheon'],   #  需要打包的模块
+    packages=['scpantheon', 'scpantheon.app', 'scpantheon.front_end'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas==1.4.4','anndata==0.8.0','colorcet==3.0.0','scanpy==1.9.1','numpy==1.21.5','PyQt5==5.15.9','PyQtWebEngine==5.15.6',
                         'appdirs==1.4.4',], # 依赖包,如果没有,可以不要
     extras_require={
         'tomas': ['tomas'],
```

