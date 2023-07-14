# Comparing `tmp/zylo-1.0.8.tar.gz` & `tmp/zylo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-1.0.8.tar", last modified: Fri Jul 14 08:26:13 2023, max compression
+gzip compressed data, was "zylo-1.0.9.tar", last modified: Fri Jul 14 10:04:12 2023, max compression
```

## Comparing `zylo-1.0.8.tar` & `zylo-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 08:26:13.691396 zylo-1.0.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 08:26:13.691396 zylo-1.0.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1046 2023-07-14 08:24:50.000000 zylo-1.0.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-14 08:26:13.691396 zylo-1.0.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-07-14 06:14:40.000000 zylo-1.0.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 08:26:13.691396 zylo-1.0.8/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-14 08:14:27.000000 zylo-1.0.8/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-14 06:52:19.000000 zylo-1.0.8/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-07-14 06:36:57.000000 zylo-1.0.8/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-14 06:48:09.000000 zylo-1.0.8/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-1.0.8/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2346 2023-07-14 06:25:13.000000 zylo-1.0.8/zylo/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.8/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.8/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 08:26:13.691396 zylo-1.0.8/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      310 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 10:04:12.013692 zylo-1.0.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 10:04:12.013692 zylo-1.0.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1046 2023-07-14 10:03:34.000000 zylo-1.0.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-14 10:04:12.013692 zylo-1.0.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-07-14 10:00:37.000000 zylo-1.0.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 10:04:12.009692 zylo-1.0.9/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-14 08:14:27.000000 zylo-1.0.9/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-07-14 10:02:42.000000 zylo-1.0.9/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-07-14 06:36:57.000000 zylo-1.0.9/zylo/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-14 06:48:09.000000 zylo-1.0.9/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-1.0.9/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2346 2023-07-14 06:25:13.000000 zylo-1.0.9/zylo/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.9/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.9/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 10:04:12.009692 zylo-1.0.9/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-14 10:04:11.000000 zylo-1.0.9/zylo.egg-info/top_level.txt
```

### Comparing `zylo-1.0.8/PKG-INFO` & `zylo-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.8
+Version: 1.0.9
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,20 +51,20 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 1.0.8
+- Beta version 1.0.9
 - Added Limiter ( from zylo.limiter import Limiter )
 - New init app=(__name__)
 - Function run() update --> run(host, port, debug)
 - JwT updated to vesion --> 1.0.2
-- Bug fixed with update --> 1.0.8
+- Bug fixed with update --> 1.0.9
 - zylo-admin library added, usage will be disclosed soon
 - Improved session management
 
 
 ```python
 
 from zylo.limiter import Limiter, render_template
```

### Comparing `zylo-1.0.8/README.md` & `zylo-1.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 1.0.8
+- Beta version 1.0.9
 - Added Limiter ( from zylo.limiter import Limiter )
 - New init app=(__name__)
 - Function run() update --> run(host, port, debug)
 - JwT updated to vesion --> 1.0.2
-- Bug fixed with update --> 1.0.8
+- Bug fixed with update --> 1.0.9
 - zylo-admin library added, usage will be disclosed soon
 - Improved session management
 
 
 ```python
 
 from zylo.limiter import Limiter, render_template
```

### Comparing `zylo-1.0.8/setup.py` & `zylo-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='1.0.8',
+    version='1.0.9',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
-    install_requires=['werkzeug', 'jinja2', 'cryptography'],  
+    install_requires=['werkzeug', 'jinja2', 'cryptography', 'zylo-admin'],  
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    entry_points={
-        'console_scripts': [
-            'zylo = zylo.app',  
-        ],
-    },
 )
```

### Comparing `zylo-1.0.8/zylo/JwT.py` & `zylo-1.0.9/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo/app.py` & `zylo-1.0.9/zylo/app.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo/blueprint.py` & `zylo-1.0.9/zylo/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo/chiper.py` & `zylo-1.0.9/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo/limiter.py` & `zylo-1.0.9/zylo/limiter.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo/mailer.py` & `zylo-1.0.9/zylo/mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo/sessions.py` & `zylo-1.0.9/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.8/zylo.egg-info/PKG-INFO` & `zylo-1.0.9/zylo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.8
+Version: 1.0.9
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -51,20 +51,20 @@
 if __name__ == '__main__':
     app.run()
  
 ```
 
 ## changelogs
 
-- Beta version 1.0.8
+- Beta version 1.0.9
 - Added Limiter ( from zylo.limiter import Limiter )
 - New init app=(__name__)
 - Function run() update --> run(host, port, debug)
 - JwT updated to vesion --> 1.0.2
-- Bug fixed with update --> 1.0.8
+- Bug fixed with update --> 1.0.9
 - zylo-admin library added, usage will be disclosed soon
 - Improved session management
 
 
 ```python
 
 from zylo.limiter import Limiter, render_template
```

