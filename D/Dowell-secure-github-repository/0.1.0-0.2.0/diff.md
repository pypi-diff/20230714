# Comparing `tmp/Dowell secure github repository-0.1.0.tar.gz` & `tmp/Dowell secure github repository-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dowell secure github repository-0.1.0.tar", last modified: Fri Jul 14 15:57:11 2023, max compression
+gzip compressed data, was "Dowell secure github repository-0.2.0.tar", last modified: Fri Jul 14 16:32:03 2023, max compression
```

## Comparing `Dowell secure github repository-0.1.0.tar` & `Dowell secure github repository-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:57:11.489343 Dowell secure github repository-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-14 15:57:11.480069 Dowell secure github repository-0.1.0/Dowell_secure_github_repository.egg-info/
--rw-rw-rw-   0        0        0      182 2023-07-14 15:57:11.000000 Dowell secure github repository-0.1.0/Dowell_secure_github_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-14 15:57:11.000000 Dowell secure github repository-0.1.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:57:11.000000 Dowell secure github repository-0.1.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 15:57:11.000000 Dowell secure github repository-0.1.0/Dowell_secure_github_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 15:57:11.000000 Dowell secure github repository-0.1.0/Dowell_secure_github_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      182 2023-07-14 15:57:11.486851 Dowell secure github repository-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5062 2023-07-14 15:56:02.000000 Dowell secure github repository-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:57:11.484579 Dowell secure github repository-0.1.0/doWell_secure_github_repository/
--rw-rw-rw-   0        0        0       64 2023-07-14 15:53:03.000000 Dowell secure github repository-0.1.0/doWell_secure_github_repository/__init__.py
--rw-rw-rw-   0        0        0     3299 2023-07-14 15:53:20.000000 Dowell secure github repository-0.1.0/doWell_secure_github_repository/doWell_secure_github_repository.py
--rw-rw-rw-   0        0        0       42 2023-07-14 15:57:11.489343 Dowell secure github repository-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-07-14 15:55:41.000000 Dowell secure github repository-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:32:03.975653 Dowell secure github repository-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:32:03.969438 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/
+-rw-rw-rw-   0        0        0     5379 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 16:32:03.000000 Dowell secure github repository-0.2.0/Dowell_secure_github_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5379 2023-07-14 16:32:03.974231 Dowell secure github repository-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5062 2023-07-14 15:56:02.000000 Dowell secure github repository-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 16:32:03.971453 Dowell secure github repository-0.2.0/doWell_secure_github_repository/
+-rw-rw-rw-   0        0        0       64 2023-07-14 15:53:03.000000 Dowell secure github repository-0.2.0/doWell_secure_github_repository/__init__.py
+-rw-rw-rw-   0        0        0     3299 2023-07-14 15:53:20.000000 Dowell secure github repository-0.2.0/doWell_secure_github_repository/doWell_secure_github_repository.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:32:03.975653 Dowell secure github repository-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      756 2023-07-14 16:30:08.000000 Dowell secure github repository-0.2.0/setup.py
```

### Comparing `Dowell secure github repository-0.1.0/README.md` & `Dowell secure github repository-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Dowell secure github repository-0.1.0/doWell_secure_github_repository/doWell_secure_github_repository.py` & `Dowell secure github repository-0.2.0/doWell_secure_github_repository/doWell_secure_github_repository.py`

 * *Files identical despite different names*

### Comparing `Dowell secure github repository-0.1.0/setup.py` & `Dowell secure github repository-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name="Dowell secure github repository",
-    version="0.1.0",
+    version="0.2.0",
     description="Dowell secure github repository from DoWell",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='uxlivinglab',
     license="Apache License 2.0",
     packages=["doWell_secure_github_repository"],
     include_package_data=True,
     install_requires=["requests"]
 )
```

