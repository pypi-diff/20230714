# Comparing `tmp/fire_opal-5.3.1.tar.gz` & `tmp/fire_opal-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-5.3.1.tar", max compression
+gzip compressed data, was "fire_opal-5.3.2.tar", max compression
```

## Comparing `fire_opal-5.3.1.tar` & `fire_opal-5.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    36653 2023-07-12 16:47:11.839560 fire_opal-5.3.1/LICENSE
--rw-r--r--   0        0        0      532 2023-07-12 16:47:11.839560 fire_opal-5.3.1/README.md
--rw-r--r--   0        0        0      884 2023-07-12 16:47:31.987769 fire_opal-5.3.1/fireopal/__init__.py
--rw-r--r--   0        0        0     2995 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/_utils.py
--rw-r--r--   0        0        0      697 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/admin.py
--rw-r--r--   0        0        0     3298 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/config.py
--rw-r--r--   0        0        0      869 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/constants.py
--rw-r--r--   0        0        0      835 2023-07-12 16:47:31.987769 fire_opal-5.3.1/fireopal/credentials/__init__.py
--rw-r--r--   0        0        0     3345 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/credentials/_credentials.py
--rw-r--r--   0        0        0      891 2023-07-12 16:47:31.991769 fire_opal-5.3.1/fireopal/functions/__init__.py
--rw-r--r--   0        0        0      818 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/base.py
--rw-r--r--   0        0        0     1478 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     2711 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0     1435 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     2029 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/execute.py
--rw-r--r--   0        0        0     1140 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/read_data.py
--rw-r--r--   0        0        0     1276 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     2315 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1702 2023-07-12 16:47:11.839560 fire_opal-5.3.1/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2771 2023-07-12 16:47:31.975769 fire_opal-5.3.1/pyproject.toml
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 fire_opal-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-14 01:51:37.075036 fire_opal-5.3.2/LICENSE
+-rw-r--r--   0        0        0      532 2023-07-14 01:51:37.075036 fire_opal-5.3.2/README.md
+-rw-r--r--   0        0        0      884 2023-07-14 01:51:56.471372 fire_opal-5.3.2/fireopal/__init__.py
+-rw-r--r--   0        0        0     2995 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/_utils.py
+-rw-r--r--   0        0        0      697 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/admin.py
+-rw-r--r--   0        0        0     3298 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/config.py
+-rw-r--r--   0        0        0      869 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/constants.py
+-rw-r--r--   0        0        0      835 2023-07-14 01:51:56.471372 fire_opal-5.3.2/fireopal/credentials/__init__.py
+-rw-r--r--   0        0        0     3345 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/credentials/_credentials.py
+-rw-r--r--   0        0        0      891 2023-07-14 01:51:56.475371 fire_opal-5.3.2/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0      818 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/base.py
+-rw-r--r--   0        0        0     1478 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/benchmark.py
+-rw-r--r--   0        0        0     2711 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/create_calibration_data.py
+-rw-r--r--   0        0        0     1435 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/create_mitigation_data.py
+-rw-r--r--   0        0        0     2029 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     1140 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1276 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     2315 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1702 2023-07-14 01:51:37.075036 fire_opal-5.3.2/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2771 2023-07-14 01:51:56.459371 fire_opal-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 fire_opal-5.3.2/PKG-INFO
```

### Comparing `fire_opal-5.3.1/LICENSE` & `fire_opal-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/README.md` & `fire_opal-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/__init__.py` & `fire_opal-5.3.2/fireopal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "5.3.1"
+__version__ = "5.3.2"
 
 from . import credentials
 from ._utils import print_package_versions
 from .functions import (
     execute,
     show_supported_devices,
     solve_qaoa,
```

### Comparing `fire_opal-5.3.1/fireopal/_utils.py` & `fire_opal-5.3.2/fireopal/_utils.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/admin.py` & `fire_opal-5.3.2/fireopal/admin.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/config.py` & `fire_opal-5.3.2/fireopal/config.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/constants.py` & `fire_opal-5.3.2/fireopal/constants.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/credentials/__init__.py` & `fire_opal-5.3.2/fireopal/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/credentials/_credentials.py` & `fire_opal-5.3.2/fireopal/credentials/_credentials.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/__init__.py` & `fire_opal-5.3.2/fireopal/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/base.py` & `fire_opal-5.3.2/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/benchmark.py` & `fire_opal-5.3.2/fireopal/functions/benchmark.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/create_calibration_data.py` & `fire_opal-5.3.2/fireopal/functions/create_calibration_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/create_mitigation_data.py` & `fire_opal-5.3.2/fireopal/functions/create_mitigation_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/execute.py` & `fire_opal-5.3.2/fireopal/functions/execute.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/read_data.py` & `fire_opal-5.3.2/fireopal/functions/read_data.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/show_supported_devices.py` & `fire_opal-5.3.2/fireopal/functions/show_supported_devices.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/solve_qaoa.py` & `fire_opal-5.3.2/fireopal/functions/solve_qaoa.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/fireopal/functions/validate.py` & `fire_opal-5.3.2/fireopal/functions/validate.py`

 * *Files identical despite different names*

### Comparing `fire_opal-5.3.1/pyproject.toml` & `fire_opal-5.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "5.3.1"
+version = "5.3.2"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -73,15 +73,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 tomli = "^2.0.1"
 importlib-metadata = "^4.13.0"
 qctrl-client = "^7.0.0"
 click = "^8.1.0"
-qctrl-commons = "^18.0.0"
+qctrl-commons = "^19.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
 pylint = "^2.17.4"
```

### Comparing `fire_opal-5.3.1/PKG-INFO` & `fire_opal-5.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 5.3.1
+Version: 5.3.2
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -30,15 +30,15 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: importlib-metadata (>=4.13.0,<5.0.0)
 Requires-Dist: qctrl-client (>=7.0.0,<8.0.0)
-Requires-Dist: qctrl-commons (>=18.0.0,<19.0.0)
+Requires-Dist: qctrl-commons (>=19.1.0,<20.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
```

