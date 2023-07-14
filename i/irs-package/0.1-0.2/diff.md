# Comparing `tmp/irs_package-0.1.tar.gz` & `tmp/irs_package-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irs_package-0.1.tar", last modified: Fri Jul 14 18:41:04 2023, max compression
+gzip compressed data, was "irs_package-0.2.tar", last modified: Fri Jul 14 18:50:46 2023, max compression
```

## Comparing `irs_package-0.1.tar` & `irs_package-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-14 18:41:04.491420 irs_package-0.1/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-14 18:26:42.000000 irs_package-0.1/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)      745 2023-07-14 18:41:04.491550 irs_package-0.1/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-14 18:25:06.000000 irs_package-0.1/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-14 18:41:04.488317 irs_package-0.1/irs_data_functions/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     2021 2023-07-14 18:33:10.000000 irs_package-0.1/irs_data_functions/read_data.py
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-14 18:41:04.491130 irs_package-0.1/irs_package.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)      745 2023-07-14 18:41:04.000000 irs_package-0.1/irs_package.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      246 2023-07-14 18:41:04.000000 irs_package-0.1/irs_package.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-14 18:41:04.000000 irs_package-0.1/irs_package.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       53 2023-07-14 18:41:04.000000 irs_package-0.1/irs_package.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       19 2023-07-14 18:41:04.000000 irs_package-0.1/irs_package.egg-info/top_level.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-14 18:41:04.492161 irs_package-0.1/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1647 2023-07-14 18:36:53.000000 irs_package-0.1/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-14 18:50:46.560416 irs_package-0.2/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-14 18:26:42.000000 irs_package-0.2/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      745 2023-07-14 18:50:46.560608 irs_package-0.2/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       25 2023-07-14 18:25:06.000000 irs_package-0.2/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-14 18:50:46.556733 irs_package-0.2/irs_data_functions/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     2021 2023-07-14 18:33:10.000000 irs_package-0.2/irs_data_functions/read_data.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-14 18:50:46.560050 irs_package-0.2/irs_package.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      745 2023-07-14 18:50:45.000000 irs_package-0.2/irs_package.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      246 2023-07-14 18:50:46.000000 irs_package-0.2/irs_package.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-14 18:50:45.000000 irs_package-0.2/irs_package.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       50 2023-07-14 18:50:45.000000 irs_package-0.2/irs_package.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       19 2023-07-14 18:50:45.000000 irs_package-0.2/irs_package.egg-info/top_level.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-14 18:50:46.562326 irs_package-0.2/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1637 2023-07-14 18:48:46.000000 irs_package-0.2/setup.py
```

### Comparing `irs_package-0.1/LICENSE.txt` & `irs_package-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irs_package-0.1/PKG-INFO` & `irs_package-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: irs_package
-Version: 0.1
+Version: 0.2
 Summary: sample package
 Home-page: https://github.com/vrathi101/irs_package.git
-Download-URL: https://github.com/vrathi101/irs_package/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/vrathi101/irs_package/archive/refs/tags/v_02.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `irs_package-0.1/irs_data_functions/read_data.py` & `irs_package-0.2/irs_data_functions/read_data.py`

 * *Files identical despite different names*

### Comparing `irs_package-0.1/irs_package.egg-info/PKG-INFO` & `irs_package-0.2/irs_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: irs-package
-Version: 0.1
+Version: 0.2
 Summary: sample package
 Home-page: https://github.com/vrathi101/irs_package.git
-Download-URL: https://github.com/vrathi101/irs_package/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/vrathi101/irs_package/archive/refs/tags/v_02.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `irs_package-0.1/setup.py` & `irs_package-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import setuptools
 setuptools.setup(
   name = 'irs_package',         # How you named your package 
   packages = ['irs_data_functions'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'sample package',   # Give a short description about your library
   author = 'VEDANT RATHI',                   # Type in your name
   author_email = 'vedrathi10@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/vrathi101/irs_package.git',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/vrathi101/irs_package/archive/refs/tags/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/vrathi101/irs_package/archive/refs/tags/v_02.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[
     'numpy',
     'pandas',
     'google-api-python-client',
-    'google-auth',
-    'io'
+    'google-auth'
 ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3.7',      #Specify which pyhton versions that you want to support
```

