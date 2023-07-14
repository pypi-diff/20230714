# Comparing `tmp/install-auto-1.1.tar.gz` & `tmp/install-auto-1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\install-auto-1.1.tar", last modified: Thu Jul 13 23:52:19 2023, max compression
+gzip compressed data, was "dist\install-auto-1.11.tar", last modified: Fri Jul 14 00:00:08 2023, max compression
```

## Comparing `install-auto-1.1.tar` & `install-auto-1.11.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:52:19.000000 install-auto-1.1/
--rw-rw-rw-   0        0        0      194 2023-07-13 23:52:19.000000 install-auto-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/
--rw-rw-rw-   0        0        0      194 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      251 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:52:19.000000 install-auto-1.1/install_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 23:52:19.000000 install-auto-1.1/setup.cfg
--rw-rw-rw-   0        0        0      635 2023-07-13 23:52:10.000000 install-auto-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:00:08.000000 install-auto-1.11/
+-rw-rw-rw-   0        0        0      195 2023-07-14 00:00:08.000000 install-auto-1.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/
+-rw-rw-rw-   0        0        0      195 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      251 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:00:08.000000 install-auto-1.11/install_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 00:00:08.000000 install-auto-1.11/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-07-13 23:59:53.000000 install-auto-1.11/setup.py
```

### Comparing `install-auto-1.1/setup.py` & `install-auto-1.11/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="install-auto",
-    version='1.1',
+    version='1.11',
     packages=find_packages(),
     package_data={'utils': ['*']},
     install_requires=[
     'click==8.1.4',
     'colorama==0.4.6',
     'importlib-metadata==6.7.0',
     'pip==23.1.2',
@@ -21,10 +21,10 @@
     'typing_extensions==4.7.1',
     'wcwidth==0.2.6',
     'zipp==3.15.0',
 ],
 
     entry_points='''
     [console_scripts]
-    gen=main
+    gen=main:app
 ''',
 )
```

