# Comparing `tmp/pyquery_xpath-0.3.tar.gz` & `tmp/pyquery_xpath-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyquery_xpath-0.3.tar", last modified: Fri Jul 14 02:21:12 2023, max compression
+gzip compressed data, was "dist\pyquery_xpath-0.4.tar", last modified: Fri Jul 14 02:31:47 2023, max compression
```

## Comparing `pyquery_xpath-0.3.tar` & `pyquery_xpath-0.4.tar`

### file list

```diff
@@ -1,7 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 02:21:12.675649 pyquery_xpath-0.3/
--rw-rw-rw-   0        0        0      293 2023-07-14 02:21:12.676651 pyquery_xpath-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 02:21:12.675649 pyquery_xpath-0.3/pyquery_xpath/
--rw-rw-rw-   0        0        0       34 2023-07-13 23:53:17.857000 pyquery_xpath-0.3/pyquery_xpath/__init__.py
--rw-rw-rw-   0        0        0      798 2023-07-14 00:08:57.243000 pyquery_xpath-0.3/pyquery_xpath/pyquery_xpath.py
--rw-rw-rw-   0        0        0       40 2023-07-14 02:19:31.762968 pyquery_xpath-0.3/setup.cfg
--rw-rw-rw-   0        0        0      654 2023-07-14 02:21:05.295089 pyquery_xpath-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:31:47.611817 pyquery_xpath-0.4/
+-rw-rw-rw-   0        0        0     1461 2023-07-14 01:16:37.000000 pyquery_xpath-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1373 2023-07-14 02:31:47.611817 pyquery_xpath-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-07-14 01:49:36.000000 pyquery_xpath-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 02:31:47.609816 pyquery_xpath-0.4/pyquery_xpath.egg-info/
+-rw-rw-rw-   0        0        0     1373 2023-07-14 02:31:47.000000 pyquery_xpath-0.4/pyquery_xpath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-07-14 02:31:47.000000 pyquery_xpath-0.4/pyquery_xpath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 02:31:47.000000 pyquery_xpath-0.4/pyquery_xpath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 02:31:47.000000 pyquery_xpath-0.4/pyquery_xpath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 02:31:47.000000 pyquery_xpath-0.4/pyquery_xpath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 02:31:47.612811 pyquery_xpath-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-07-14 02:28:43.000000 pyquery_xpath-0.4/setup.py
```

### Comparing `pyquery_xpath-0.3/setup.py` & `pyquery_xpath-0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 # coding: utf-8
-from distutils.core import setup
-from os import path
-this_directory = path.abspath(path.dirname(__file__))
+from setuptools import setup, find_packages
 
-try:
-    import pypandoc
-    long_description = pypandoc.convert('README.md', 'rst')
-except:
-    long_description = ""
+with open("README.md", "r", encoding='utf-8') as fh:
+    long_description = fh.read()
 
-setup(
-    name='pyquery_xpath',
-    version='0.3',
-    description='Adding XPath support to pyquery',
-    author='alleyfrost',
-    author_email='alleyfrost@qq.com',
-    url='https://github.com/alleyfrost/pyquery_xpath',
-    packages=['pyquery_xpath'],
-    install_requires=['pyquery'],
-    keywords='pyquery xpath',
-    long_description=long_description,
-    python_requires=">=3.0"
-)
+setup(name='pyquery_xpath',
+      version='0.4',
+      description='Adding XPath support to pyquery',
+      author='alleyfrost',
+      author_email='alleyfrost@qq.com',
+      url='https://github.com/alleyfrost/pyquery_xpath',
+      packages=find_packages('pyquery',),
+      long_description=long_description,
+      long_description_content_type="text/markdown",
+      license="GPLv3",
+      python_requires='>=3.0',
+      install_requires=['pyquery'],
+      )
```

