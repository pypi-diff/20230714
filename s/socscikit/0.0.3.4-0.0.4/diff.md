# Comparing `tmp/socscikit-0.0.3.4.tar.gz` & `tmp/socscikit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.3.4.tar", last modified: Fri Jul 14 00:28:03 2023, max compression
+gzip compressed data, was "socscikit-0.0.4.tar", last modified: Fri Jul 14 01:14:50 2023, max compression
```

## Comparing `socscikit-0.0.3.4.tar` & `socscikit-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 00:28:03.325215 socscikit-0.0.3.4/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0       90 2023-07-14 00:27:44.000000 socscikit-0.0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-14 00:28:03.325215 socscikit-0.0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.3.4/README.md
--rw-rw-rw-   0        0        0       86 2023-07-14 00:28:03.328297 socscikit-0.0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1116 2023-07-14 00:23:36.000000 socscikit-0.0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 00:28:03.264242 socscikit-0.0.3.4/socscikit/
--rw-rw-rw-   0        0        0      486 2023-07-13 23:56:46.000000 socscikit-0.0.3.4/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.3.4/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 00:28:03.247820 socscikit-0.0.3.4/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-14 00:28:03.323763 socscikit-0.0.3.4/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.3.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.3.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.3.4/socscikit/socialmedia.py
-drwxrwxrwx   0        0        0        0 2023-07-14 00:28:03.287062 socscikit-0.0.3.4/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-14 00:28:02.000000 socscikit-0.0.3.4/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-07-14 00:28:03.000000 socscikit-0.0.3.4/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 00:28:02.000000 socscikit-0.0.3.4/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-14 00:28:02.000000 socscikit-0.0.3.4/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 00:28:02.000000 socscikit-0.0.3.4/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 01:14:50.210393 socscikit-0.0.4/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      167 2023-07-14 01:11:43.000000 socscikit-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      404 2023-07-14 01:14:50.211401 socscikit-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-14 01:14:50.221481 socscikit-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-07-14 01:14:35.000000 socscikit-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:14:50.103529 socscikit-0.0.4/socscikit/
+-rw-rw-rw-   0        0        0      737 2023-07-14 01:10:54.000000 socscikit-0.0.4/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.4/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:14:50.077041 socscikit-0.0.4/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-14 01:14:50.172664 socscikit-0.0.4/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-14 01:14:50.207017 socscikit-0.0.4/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.4/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153319 2023-07-14 01:03:12.000000 socscikit-0.0.4/socscikit/lexicon_dictionary/VADER/VADER.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.4/socscikit/socialmedia.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:14:50.148594 socscikit-0.0.4/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-07-14 01:14:49.000000 socscikit-0.0.4/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-07-14 01:14:49.000000 socscikit-0.0.4/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 01:14:49.000000 socscikit-0.0.4/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-14 01:14:49.000000 socscikit-0.0.4/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 01:14:49.000000 socscikit-0.0.4/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.3.4/LICENSE.txt` & `socscikit-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.3.4/setup.py` & `socscikit-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   # Chose the same as "name"
-  version = '0.0.3.4',      # Start with a small number and increase it with every change you make
+  version = '0.0.4',      # Start with a small number and increase it with every change you make
   license='Apache-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Nick S.H Oh',                   # Type in your name
   author_email = 'nick.sh.oh@socialscience.ai',      # Type in your E-Mail
   url = 'https://github.com/nick-sh-oh/socscikit',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.3.4.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.4.tar.gz',    # I explain this later on
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'tweepy',
           'plotly',
           'conlp'
       ],
   include_package_data=True
```

### Comparing `socscikit-0.0.3.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.3.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.4/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.3.4/socscikit/socialmedia.py` & `socscikit-0.0.4/socscikit/socialmedia.py`

 * *Files identical despite different names*

