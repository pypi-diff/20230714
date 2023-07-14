# Comparing `tmp/gitprprod-0.0.2.tar.gz` & `tmp/gitprprod-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitprprod-0.0.2.tar", last modified: Fri Jul 14 09:11:51 2023, max compression
+gzip compressed data, was "gitprprod-0.0.3.tar", last modified: Fri Jul 14 09:41:29 2023, max compression
```

## Comparing `gitprprod-0.0.2.tar` & `gitprprod-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 09:11:51.420889 gitprprod-0.0.2/
--rw-rw-rw-   0        0        0      865 2023-07-14 09:11:51.419479 gitprprod-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-12 07:12:52.000000 gitprprod-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 09:11:51.388975 gitprprod-0.0.2/git_pr/
--rw-rw-rw-   0        0        0        0 2023-07-11 10:47:17.000000 gitprprod-0.0.2/git_pr/__init__.py
--rw-rw-rw-   0        0        0     2485 2023-07-13 06:56:32.000000 gitprprod-0.0.2/git_pr/git_pr.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:11:51.414853 gitprprod-0.0.2/gitprprod.egg-info/
--rw-rw-rw-   0        0        0      865 2023-07-14 09:11:51.000000 gitprprod-0.0.2/gitprprod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-14 09:11:51.000000 gitprprod-0.0.2/gitprprod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 09:11:51.000000 gitprprod-0.0.2/gitprprod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-14 09:11:51.000000 gitprprod-0.0.2/gitprprod.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-07-14 09:11:51.000000 gitprprod-0.0.2/gitprprod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 09:11:51.000000 gitprprod-0.0.2/gitprprod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5347 2023-07-14 09:11:06.000000 gitprprod-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 09:11:51.421446 gitprprod-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:29.912637 gitprprod-0.0.3/
+-rw-rw-rw-   0        0        0      865 2023-07-14 09:41:29.912637 gitprprod-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:12:52.000000 gitprprod-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:29.892428 gitprprod-0.0.3/git_pr/
+-rw-rw-rw-   0        0        0        0 2023-07-11 10:47:17.000000 gitprprod-0.0.3/git_pr/__init__.py
+-rw-rw-rw-   0        0        0     2485 2023-07-13 06:56:32.000000 gitprprod-0.0.3/git_pr/git_pr.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:29.912637 gitprprod-0.0.3/gitprprod.egg-info/
+-rw-rw-rw-   0        0        0      865 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 09:41:29.000000 gitprprod-0.0.3/gitprprod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5319 2023-07-14 09:41:12.000000 gitprprod-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 09:41:29.912637 gitprprod-0.0.3/setup.cfg
```

### Comparing `gitprprod-0.0.2/PKG-INFO` & `gitprprod-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitprprod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Project for git pr
 Author-email: Abhinandan <abhinandan.x@nxp.com>
 Maintainer-email: Abhinandan <abhinandan.x@nxp.com>
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `gitprprod-0.0.2/git_pr/git_pr.py` & `gitprprod-0.0.3/git_pr/git_pr.py`

 * *Files identical despite different names*

### Comparing `gitprprod-0.0.2/gitprprod.egg-info/PKG-INFO` & `gitprprod-0.0.3/gitprprod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitprprod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Project for git pr
 Author-email: Abhinandan <abhinandan.x@nxp.com>
 Maintainer-email: Abhinandan <abhinandan.x@nxp.com>
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `gitprprod-0.0.2/pyproject.toml` & `gitprprod-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "gitprprod"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.2"  # Required
+version = "0.0.3"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A Python Project for git pr"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -99,16 +99,15 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ 
-  "boto3==1.4.0",
-  "botocore<1.5.0,>=1.4.1"
+  "boto3>=1.28.0"
 
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
```

