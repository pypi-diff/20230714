# Comparing `tmp/socscikit-0.0.3.1.tar.gz` & `tmp/socscikit-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.3.1.tar", last modified: Thu Jul 13 23:51:04 2023, max compression
+gzip compressed data, was "socscikit-0.0.3.2.tar", last modified: Thu Jul 13 23:57:45 2023, max compression
```

## Comparing `socscikit-0.0.3.1.tar` & `socscikit-0.0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:51:04.778623 socscikit-0.0.3.1/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0      408 2023-07-13 23:51:04.779720 socscikit-0.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.3.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-13 23:51:04.783244 socscikit-0.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-07-13 23:50:45.000000 socscikit-0.0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:51:04.739246 socscikit-0.0.3.1/socscikit/
--rw-rw-rw-   0        0        0      519 2023-07-13 23:49:09.000000 socscikit-0.0.3.1/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       91 2023-07-13 23:44:07.000000 socscikit-0.0.3.1/socscikit/init.py
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.3.1/socscikit/socialmedia.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:51:04.776618 socscikit-0.0.3.1/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-13 23:51:03.000000 socscikit-0.0.3.1/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-13 23:51:04.000000 socscikit-0.0.3.1/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:51:03.000000 socscikit-0.0.3.1/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-13 23:51:04.000000 socscikit-0.0.3.1/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 23:51:04.000000 socscikit-0.0.3.1/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 23:57:45.264813 socscikit-0.0.3.2/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      408 2023-07-13 23:57:45.264813 socscikit-0.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.3.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-13 23:57:45.278529 socscikit-0.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-07-13 23:57:31.000000 socscikit-0.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:57:45.210213 socscikit-0.0.3.2/socscikit/
+-rw-rw-rw-   0        0        0      486 2023-07-13 23:56:46.000000 socscikit-0.0.3.2/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.3.2/socscikit/__init__.py
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.3.2/socscikit/socialmedia.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:57:45.262722 socscikit-0.0.3.2/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-13 23:57:44.000000 socscikit-0.0.3.2/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-13 23:57:44.000000 socscikit-0.0.3.2/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:57:44.000000 socscikit-0.0.3.2/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-13 23:57:44.000000 socscikit-0.0.3.2/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 23:57:44.000000 socscikit-0.0.3.2/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.3.1/LICENSE.txt` & `socscikit-0.0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.3.1/setup.py` & `socscikit-0.0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   # Chose the same as "name"
-  version = '0.0.3.1',      # Start with a small number and increase it with every change you make
+  version = '0.0.3.2',      # Start with a small number and increase it with every change you make
   license='Apache-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Nick S.H Oh',                   # Type in your name
   author_email = 'nick.sh.oh@socialscience.ai',      # Type in your E-Mail
   url = 'https://github.com/nick-sh-oh/socscikit',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.3.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.3.2.tar.gz',    # I explain this later on
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'tweepy',
           'plotly',
           'conlp'
       ]
 )
```

### Comparing `socscikit-0.0.3.1/socscikit/socialmedia.py` & `socscikit-0.0.3.2/socscikit/socialmedia.py`

 * *Files identical despite different names*

