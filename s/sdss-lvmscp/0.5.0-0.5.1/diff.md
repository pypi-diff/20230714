# Comparing `tmp/sdss_lvmscp-0.5.0.tar.gz` & `tmp/sdss_lvmscp-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.5.0.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.5.1.tar", max compression
```

## Comparing `sdss_lvmscp-0.5.0.tar` & `sdss_lvmscp-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2023-07-10 05:47:11.766281 sdss_lvmscp-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-10 05:47:11.766723 sdss_lvmscp-0.5.0/README.md
--rw-r--r--   0        0        0     2714 2023-07-10 05:47:11.810868 sdss_lvmscp-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-10 05:47:11.811326 sdss_lvmscp-0.5.0/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-10 05:47:11.811631 sdss_lvmscp-0.5.0/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-10 05:47:11.812037 sdss_lvmscp-0.5.0/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-10 05:47:11.812308 sdss_lvmscp-0.5.0/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-10 05:47:11.812630 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-10 05:47:11.812852 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-07-10 05:47:11.813100 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-10 05:47:11.813395 sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-10 05:47:11.813673 sdss_lvmscp-0.5.0/python/lvmscp/controller.py
--rw-r--r--   0        0        0    13581 2023-07-10 05:47:11.814001 sdss_lvmscp-0.5.0/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40775 2023-07-10 05:47:11.814476 sdss_lvmscp-0.5.0/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5466 2023-07-10 05:47:11.814738 sdss_lvmscp-0.5.0/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-10 05:47:11.814918 sdss_lvmscp-0.5.0/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-10 05:47:11.815206 sdss_lvmscp-0.5.0/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 sdss_lvmscp-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-13 23:26:28.638223 sdss_lvmscp-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-13 23:26:28.638685 sdss_lvmscp-0.5.1/README.md
+-rw-r--r--   0        0        0     2715 2023-07-13 23:26:28.702215 sdss_lvmscp-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-13 23:26:28.703298 sdss_lvmscp-0.5.1/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-13 23:26:28.703789 sdss_lvmscp-0.5.1/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-13 23:26:28.704155 sdss_lvmscp-0.5.1/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-13 23:26:28.704512 sdss_lvmscp-0.5.1/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-13 23:26:28.705060 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-13 23:26:28.705354 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/expose.py
+-rw-r--r--   0        0        0     3827 2023-07-13 23:26:28.705730 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-13 23:26:28.706014 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-13 23:26:28.706314 sdss_lvmscp-0.5.1/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    13581 2023-07-13 23:26:28.706624 sdss_lvmscp-0.5.1/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40775 2023-07-13 23:26:28.707229 sdss_lvmscp-0.5.1/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5466 2023-07-13 23:26:28.707967 sdss_lvmscp-0.5.1/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-13 23:26:28.708248 sdss_lvmscp-0.5.1/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-13 23:26:28.708730 sdss_lvmscp-0.5.1/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.5.1/PKG-INFO
```

### Comparing `sdss_lvmscp-0.5.0/LICENSE.md` & `sdss_lvmscp-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/README.md` & `sdss_lvmscp-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/pyproject.toml` & `sdss_lvmscp-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.5.0"
+version = "0.5.1"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
@@ -28,15 +28,15 @@
 [tool.poetry.scripts]
 lvmscp = "lvmscp.__main__:main"
 ln2fill = "lvmscp.ln2:ln2fill"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click-default-group = "^1.2.2"
-sdss-archon = "^0.9.0"
+sdss-archon = "^0.10.0"
 httpx = ">=0.18.1"
 Authlib = ">=1.0.0rc1"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
```

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/__main__.py` & `sdss_lvmscp-0.5.1/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.5.1/python/lvmscp/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/expose.py` & `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/controller.py` & `sdss_lvmscp-0.5.1/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/delegate.py` & `sdss_lvmscp-0.5.1/python/lvmscp/delegate.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.5.1/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.5.1/python/lvmscp/etc/lvmscp.yml`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/python/lvmscp/ln2.py` & `sdss_lvmscp-0.5.1/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.0/PKG-INFO` & `sdss_lvmscp-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.5.0
+Version: 0.5.1
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Authlib (>=1.0.0rc1)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: httpx (>=0.18.1)
-Requires-Dist: sdss-archon (>=0.9.0,<0.10.0)
+Requires-Dist: sdss-archon (>=0.10.0,<0.11.0)
 Project-URL: Documentation, https://sdss-lvmscp.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmscp
 Description-Content-Type: text/markdown
 
 # lvmscp
 
 ![Versions](https://img.shields.io/badge/python->3.8-blue)
```

