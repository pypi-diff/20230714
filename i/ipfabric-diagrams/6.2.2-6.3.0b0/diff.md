# Comparing `tmp/ipfabric_diagrams-6.2.2.tar.gz` & `tmp/ipfabric_diagrams-6.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_diagrams-6.2.2.tar", max compression
+gzip compressed data, was "ipfabric_diagrams-6.3.0b0.tar", max compression
```

## Comparing `ipfabric_diagrams-6.2.2.tar` & `ipfabric_diagrams-6.3.0b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1829 2023-05-25 13:21:36.145925 ipfabric_diagrams-6.2.2/ipfabric/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-25 13:21:36.146926 ipfabric_diagrams-6.2.2/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0     7488 2023-05-25 13:21:36.146926 ipfabric_diagrams-6.2.2/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3625 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.2.2/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      580 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3755 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     7009 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2277 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    10507 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    10534 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0       68 2023-05-25 13:21:36.151765 ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     2608 2023-05-25 13:21:36.151765 ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     1412 2023-05-25 13:21:36.152771 ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     3198 2023-05-25 13:35:46.575244 ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0     1152 2023-05-25 13:21:36.160649 ipfabric_diagrams-6.2.2/ipfabric_diagrams/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 13:21:36.166244 ipfabric_diagrams-6.2.2/ipfabric_diagrams/graphs.py
--rw-r--r--   0        0        0     2910 2023-05-25 13:21:36.173769 ipfabric_diagrams-6.2.2/ipfabric_diagrams/icmp.py
--rw-r--r--   0        0        0     1087 2023-05-25 13:21:36.111751 ipfabric_diagrams-6.2.2/LICENSE
--rw-r--r--   0        0        0     1678 2023-05-25 13:44:01.184190 ipfabric_diagrams-6.2.2/pyproject.toml
--rw-r--r--   0        0        0     2572 2023-05-25 13:21:36.116783 ipfabric_diagrams-6.2.2/README.md
--rw-r--r--   0        0        0     3596 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.2/setup.py
--rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1829 2023-05-25 13:21:36.145925 ipfabric_diagrams-6.3.0b0/ipfabric/__init__.py
+-rw-r--r--   0        0        0     1906 2023-05-25 13:21:36.146926 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0     7488 2023-05-25 13:21:36.146926 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      580 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3755 2023-05-25 13:21:36.148253 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     7009 2023-05-25 13:21:36.149259 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2277 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    10507 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    10534 2023-05-25 13:21:36.150259 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0       68 2023-05-25 13:21:36.151765 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     2608 2023-05-25 13:21:36.151765 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     1412 2023-05-25 13:21:36.152771 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     3198 2023-05-25 13:35:46.575244 ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     1152 2023-05-25 13:21:36.160649 ipfabric_diagrams-6.3.0b0/ipfabric_diagrams/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 13:21:36.166244 ipfabric_diagrams-6.3.0b0/ipfabric_diagrams/graphs.py
+-rw-r--r--   0        0        0     2910 2023-05-25 13:21:36.173769 ipfabric_diagrams-6.3.0b0/ipfabric_diagrams/icmp.py
+-rw-r--r--   0        0        0     1087 2023-05-25 13:21:36.111751 ipfabric_diagrams-6.3.0b0/LICENSE
+-rw-r--r--   0        0        0     1682 2023-07-14 16:37:07.047908 ipfabric_diagrams-6.3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2572 2023-05-25 13:21:36.116783 ipfabric_diagrams-6.3.0b0/README.md
+-rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.3.0b0/setup.py
+-rw-r--r--   0        0        0     3629 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.3.0b0/PKG-INFO
```

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/__init__.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/__init__.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/graphs.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/graphs.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/icmp.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/__init__.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/constants.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/protocols.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/protocols.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric/diagrams/output_models/trace.py` & `ipfabric_diagrams-6.3.0b0/ipfabric/diagrams/output_models/trace.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric_diagrams/__init__.py` & `ipfabric_diagrams-6.3.0b0/ipfabric_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/ipfabric_diagrams/icmp.py` & `ipfabric_diagrams-6.3.0b0/ipfabric_diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/LICENSE` & `ipfabric_diagrams-6.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/pyproject.toml` & `ipfabric_diagrams-6.3.0b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric-diagrams"
-version = "v6.2.2"
+version = "v6.3.0b0"
 description = "Python package for interacting with IP Fabric Diagrams"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,21 +18,21 @@
 
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams/-/blob/develop/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-ipfabric = "~6.2.2"
+ipfabric = "~6.3.0b0"
 typing-extensions = "^4.5"
 rich = {version = "^13.3.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
 flake8 = "^5.0.4"
 black = "^22.12"
 
 [tool.poetry.extras]
 examples = ["rich"]
 
 [build-system]
```

### Comparing `ipfabric_diagrams-6.2.2/README.md` & `ipfabric_diagrams-6.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.2/setup.py` & `ipfabric_diagrams-6.3.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
  'ipfabric.diagrams.output_models',
  'ipfabric_diagrams']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ipfabric>=6.2.2,<6.3.0', 'typing-extensions>=4.5,<5.0']
+['ipfabric>=6.3.0b0,<6.4.0', 'typing-extensions>=4.5,<5.0']
 
 extras_require = \
 {'examples': ['rich>=13.3.0,<14.0.0']}
 
 setup_kwargs = {
     'name': 'ipfabric-diagrams',
-    'version': '6.2.2',
+    'version': '6.3.0b0',
     'description': 'Python package for interacting with IP Fabric Diagrams',
     'long_description': "# IP Fabric\n\nipfabric_diagrams is a Python module for connecting to and graphing topologies against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation.\n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth='TOKEN')`\n  - User/Pass: `IPFClient(auth=('USER', 'PASS'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API's are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK's match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric-diagrams\n```\n\n## Introduction\n\nThis package is used for diagramming via the API for IP Fabric v4.3.0.  \nExamples can be located under [examples](examples/) directory.\n\n## Authentication\nPlease take a look at [python-ipfabric](https://gitlab.com/ip-fabric/integrations/python-ipfabric#authentication) \nfor all authentication options.\n\n```python\nfrom ipfabric.diagrams import IPFDiagram\nipf = IPFDiagram(base_url='https://demo3.ipfabric.io/', auth='token', verify=False, timeout=15)\n```\n\n## Development\n\nIPFabric uses poetry for the python packaging module. Install poetry globally:\n\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo test and build:\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric_diagrams ipfabric\npoetry update\n```\n",
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams',
```

### Comparing `ipfabric_diagrams-6.2.2/PKG-INFO` & `ipfabric_diagrams-6.3.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ipfabric-diagrams
-Version: 6.2.2
+Version: 6.3.0b0
 Summary: Python package for interacting with IP Fabric Diagrams
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: examples
-Requires-Dist: ipfabric (>=6.2.2,<6.3.0)
+Requires-Dist: ipfabric (>=6.3.0b0,<6.4.0)
 Requires-Dist: rich (>=13.3.0,<14.0.0) ; extra == "examples"
 Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams/-/blob/develop/CHANGELOG.md
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 Description-Content-Type: text/markdown
```

