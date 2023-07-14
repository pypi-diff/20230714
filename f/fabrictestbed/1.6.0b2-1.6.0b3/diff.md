# Comparing `tmp/fabrictestbed-1.6.0b2.tar.gz` & `tmp/fabrictestbed-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.6.0b2.tar", last modified: Fri Jul 14 15:20:17 2023, max compression
+gzip compressed data, was "fabrictestbed-1.6.0b3.tar", last modified: Fri Jul 14 16:28:50 2023, max compression
```

## Comparing `fabrictestbed-1.6.0b2.tar` & `fabrictestbed-1.6.0b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b2/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b2/LICENSE
--rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b2/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b2/README.md
--rw-r--r--   0        0        0       24 2023-07-14 15:18:36.298265 fabrictestbed-1.6.0b2/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b2/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b2/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b2/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b2/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b2/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    19929 2023-07-14 15:19:59.556056 fabrictestbed-1.6.0b2/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b2/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b2/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0     1071 2023-07-13 18:48:30.199529 fabrictestbed-1.6.0b2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b2/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b2/test/test_cli.py
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-07-13 18:40:33.774250 fabrictestbed-1.6.0b3/.gitignore
+-rw-r--r--   0        0        0     1071 2023-07-13 18:40:33.774483 fabrictestbed-1.6.0b3/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-13 18:40:33.774598 fabrictestbed-1.6.0b3/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-07-13 18:40:33.774750 fabrictestbed-1.6.0b3/README.md
+-rw-r--r--   0        0        0       24 2023-07-14 16:28:28.781860 fabrictestbed-1.6.0b3/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.775067 fabrictestbed-1.6.0b3/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-07-13 18:40:33.775336 fabrictestbed-1.6.0b3/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.775647 fabrictestbed-1.6.0b3/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-07-13 18:40:33.775918 fabrictestbed-1.6.0b3/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-07-13 18:40:33.776101 fabrictestbed-1.6.0b3/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    20091 2023-07-14 15:30:33.271468 fabrictestbed-1.6.0b3/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.776619 fabrictestbed-1.6.0b3/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-07-13 18:40:33.776762 fabrictestbed-1.6.0b3/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1071 2023-07-13 18:48:30.199529 fabrictestbed-1.6.0b3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 18:40:33.777184 fabrictestbed-1.6.0b3/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-13 18:40:33.777415 fabrictestbed-1.6.0b3/test/test_cli.py
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 fabrictestbed-1.6.0b3/PKG-INFO
```

### Comparing `fabrictestbed-1.6.0b2/.gitignore` & `fabrictestbed-1.6.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/LICENSE` & `fabrictestbed-1.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/README.md` & `fabrictestbed-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/fabrictestbed/cli/cli.py` & `fabrictestbed-1.6.0b3/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.6.0b3/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.6.0b3/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.6.0b3/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import json
+import logging
 import os
 from datetime import datetime, timedelta, timezone
 from typing import Tuple, Union, List, Any, Dict
 
 import paramiko
 from fabric_cf.orchestrator.swagger_client import Sliver, Slice
 from fabric_cf.orchestrator.swagger_client.models import PoaData
@@ -43,14 +44,15 @@
 
 class SliceManager:
     """
     Implements User facing Control Framework API interface
     """
     def __init__(self, *, cm_host: str = None, oc_host: str = None, token_location: str = None,
                  project_id: str = None, scope: str = "all", initialize: bool = True):
+        self.logger = logging.getLogger()
         if cm_host is None:
             cm_host = os.environ.get(Constants.FABRIC_CREDMGR_HOST)
         if oc_host is None:
             oc_host = os.environ.get(Constants.FABRIC_ORCHESTRATOR_HOST)
         self.cm_proxy = CredmgrProxy(credmgr_host=cm_host)
         self.oc_proxy = OrchestratorProxy(orchestrator_host=oc_host)
         self.token_location = token_location
@@ -119,15 +121,17 @@
             with open(self.token_location, 'r') as stream:
                 self.tokens = json.loads(stream.read())
             refresh_token = self.get_refresh_token()
         else:
             # First time login, use environment variable to load the tokens
             refresh_token = os.environ.get(Constants.CILOGON_REFRESH_TOKEN)
         if refresh_token is None:
-            raise SliceManagerException(f"Unable to refresh tokens: no refresh token found!")
+            #raise SliceManagerException(f"Unable to refresh tokens: no refresh token found!")
+            self.logger.warning("Unable to refresh tokens: no refresh token found!")
+            return
         # Renew the tokens to ensure any project_id changes are taken into account
         self.refresh_tokens(refresh_token=refresh_token)
 
     def get_refresh_token(self) -> str:
         """
         Get Refresh Token
         @return refresh token
```

### Comparing `fabrictestbed-1.6.0b2/fabrictestbed/util/constants.py` & `fabrictestbed-1.6.0b3/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/pyproject.toml` & `fabrictestbed-1.6.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/test/test_cli.py` & `fabrictestbed-1.6.0b3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.6.0b2/PKG-INFO` & `fabrictestbed-1.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

