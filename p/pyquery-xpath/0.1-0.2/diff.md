# Comparing `tmp/pyquery_xpath-0.1.tar.gz` & `tmp/pyquery_xpath-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyquery_xpath-0.1.tar", last modified: Fri Jul 14 01:50:19 2023, max compression
+gzip compressed data, was "dist\pyquery_xpath-0.2.tar", last modified: Fri Jul 14 02:07:02 2023, max compression
```

## Comparing `pyquery_xpath-0.1.tar` & `pyquery_xpath-0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 01:50:19.263505 pyquery_xpath-0.1/
--rw-rw-rw-   0        0        0      293 2023-07-14 01:50:19.263505 pyquery_xpath-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 01:50:19.262503 pyquery_xpath-0.1/pyquery_xpath/
--rw-rw-rw-   0        0        0       34 2023-07-13 23:53:17.857000 pyquery_xpath-0.1/pyquery_xpath/__init__.py
--rw-rw-rw-   0        0        0      798 2023-07-14 00:08:57.243000 pyquery_xpath-0.1/pyquery_xpath/pyquery_xpath.py
--rw-rw-rw-   0        0        0      654 2023-07-14 01:09:53.563550 pyquery_xpath-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:07:02.372027 pyquery_xpath-0.2/
+-rw-rw-rw-   0        0        0      293 2023-07-14 02:07:02.372027 pyquery_xpath-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 02:07:02.372027 pyquery_xpath-0.2/pyquery_xpath/
+-rw-rw-rw-   0        0        0       34 2023-07-13 23:53:17.857000 pyquery_xpath-0.2/pyquery_xpath/__init__.py
+-rw-rw-rw-   0        0        0      798 2023-07-14 00:08:57.243000 pyquery_xpath-0.2/pyquery_xpath/pyquery_xpath.py
+-rw-rw-rw-   0        0        0      654 2023-07-14 02:06:50.442801 pyquery_xpath-0.2/setup.py
```

### Comparing `pyquery_xpath-0.1/pyquery_xpath/pyquery_xpath.py` & `pyquery_xpath-0.2/pyquery_xpath/pyquery_xpath.py`

 * *Files identical despite different names*

### Comparing `pyquery_xpath-0.1/setup.py` & `pyquery_xpath-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except:
     long_description = ""
 
 setup(
     name='pyquery_xpath',
-    version='0.1',
+    version='0.2',
     description='Adding XPath support to pyquery',
     author='alleyfrost',
     author_email='alleyfrost@qq.com',
     url='https://github.com/alleyfrost/pyquery_xpath',
     packages=['pyquery_xpath'],
     install_requires=['pyquery'],
     keywords='pyquery xpath',
```

