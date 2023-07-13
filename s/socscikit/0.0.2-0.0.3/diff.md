# Comparing `tmp/socscikit-0.0.2.tar.gz` & `tmp/socscikit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.2.tar", last modified: Mon Apr 24 07:38:41 2023, max compression
+gzip compressed data, was "socscikit-0.0.3.tar", last modified: Thu Jul 13 23:29:14 2023, max compression
```

## Comparing `socscikit-0.0.2.tar` & `socscikit-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:38:41.963663 socscikit-0.0.2/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      414 2023-04-24 07:38:41.965169 socscikit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 07:38:41.965169 socscikit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-04-24 07:38:07.000000 socscikit-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:38:41.958498 socscikit-0.0.2/socscikit/
--rw-rw-rw-   0        0        0       35 2023-04-24 07:10:10.000000 socscikit-0.0.2/socscikit/__init__.py
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.2/socscikit/socialmedia.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:38:41.963663 socscikit-0.0.2/socscikit.egg-info/
--rw-rw-rw-   0        0        0      414 2023-04-24 07:38:41.000000 socscikit-0.0.2/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-24 07:38:41.000000 socscikit-0.0.2/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:38:41.000000 socscikit-0.0.2/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-24 07:38:41.000000 socscikit-0.0.2/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 07:38:41.000000 socscikit-0.0.2/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 23:29:14.751312 socscikit-0.0.3/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      404 2023-07-13 23:29:14.751312 socscikit-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-13 23:29:14.756312 socscikit-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-07-13 23:20:57.000000 socscikit-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:29:14.681473 socscikit-0.0.3/socscikit/
+-rw-rw-rw-   0        0        0      383 2023-07-13 23:26:49.000000 socscikit-0.0.3/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:18:58.000000 socscikit-0.0.3/socscikit/__init__.py
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.3/socscikit/socialmedia.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:29:14.747016 socscikit-0.0.3/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-07-13 23:29:13.000000 socscikit-0.0.3/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-13 23:29:14.000000 socscikit-0.0.3/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:29:13.000000 socscikit-0.0.3/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-13 23:29:13.000000 socscikit-0.0.3/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 23:29:13.000000 socscikit-0.0.3/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.2/LICENSE.txt` & `socscikit-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.2/setup.py` & `socscikit-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   # Chose the same as "name"
-  version = '0.0.2',      # Start with a small number and increase it with every change you make
+  version = '0.0.3',      # Start with a small number and increase it with every change you make
   license='Apache-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Nick S.H Oh',                   # Type in your name
   author_email = 'nick.sh.oh@socialscience.ai',      # Type in your E-Mail
-  url = 'https://github.com/SOCIALSCIENCEai/socscikit',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/SOCIALSCIENCEai/socscikit/archive/refs/tags/0.0.2.tar.gz',    # I explain this later on
+  url = 'https://github.com/nick-sh-oh/socscikit',   # Provide either the link to your github or to your website
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.3.tar.gz',    # I explain this later on
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'tweepy',
           'plotly',
           'conlp'
       ]
-)
+)
+
```

### Comparing `socscikit-0.0.2/socscikit/socialmedia.py` & `socscikit-0.0.3/socscikit/socialmedia.py`

 * *Files identical despite different names*

