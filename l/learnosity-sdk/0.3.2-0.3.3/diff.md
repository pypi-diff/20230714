# Comparing `tmp/learnosity_sdk-0.3.2.tar.gz` & `tmp/learnosity_sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/learnosity_sdk-0.3.2.tar", last modified: Wed Jan  8 06:16:50 2020, max compression
+gzip compressed data, was "learnosity_sdk-0.3.3.tar", last modified: Fri Jul 14 01:17:40 2023, max compression
```

## Comparing `learnosity_sdk-0.3.2.tar` & `learnosity_sdk-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk/
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk/request/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      110 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/request/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5212 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/request/dataapi.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     8740 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/request/init.py
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk/utils/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       64 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/utils/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       96 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/utils/lrnuuid.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      220 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       23 2020-01-08 06:10:36.000000 learnosity_sdk-0.3.2/learnosity_sdk/_version.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      135 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/learnosity_sdk/exceptions.py
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      305 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      680 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      123 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       21 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/learnosity_sdk.egg-info/top_level.txt
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/tests/
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/tests/integration/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/integration/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3765 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/integration/test_dataapi.py
-drwxrwsr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/tests/unit/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/unit/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2843 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/unit/test_dataapi.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6301 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/unit/test_init.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1336 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/unit/test_sdk.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      453 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/unit/test_uuid.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/tests/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       54 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/MANIFEST.in
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7324 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       67 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/setup.cfg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1000 2019-11-25 07:09:32.000000 learnosity_sdk-0.3.2/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      305 2020-01-08 06:16:50.000000 learnosity_sdk-0.3.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.278022 learnosity_sdk-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)     9235 2023-07-13 04:49:15.000000 learnosity_sdk-0.3.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-13 04:49:15.000000 learnosity_sdk-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19064 2023-07-14 01:17:40.279224 learnosity_sdk-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18645 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.140633 learnosity_sdk-0.3.3/docs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/docs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.149047 learnosity_sdk-0.3.3/docs/quickstart/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/docs/quickstart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/docs/quickstart/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.162191 learnosity_sdk-0.3.3/learnosity_sdk/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/learnosity_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/learnosity_sdk/_version.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-13 04:49:15.000000 learnosity_sdk-0.3.3/learnosity_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.211919 learnosity_sdk-0.3.3/learnosity_sdk/request/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-13 04:49:15.000000 learnosity_sdk-0.3.3/learnosity_sdk/request/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/learnosity_sdk/request/dataapi.py
+-rw-r--r--   0 root         (0) root         (0)     9051 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/learnosity_sdk/request/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.221044 learnosity_sdk-0.3.3/learnosity_sdk/utils/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/learnosity_sdk/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-13 04:49:15.000000 learnosity_sdk-0.3.3/learnosity_sdk/utils/lrnuuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.196635 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19064 2023-07-14 01:17:39.000000 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-14 01:17:40.000000 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 01:17:39.000000 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-14 01:17:39.000000 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-14 01:17:39.000000 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-14 01:17:40.000000 learnosity_sdk-0.3.3/learnosity_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-14 01:17:40.281287 learnosity_sdk-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.225726 learnosity_sdk-0.3.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 04:49:15.000000 learnosity_sdk-0.3.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.247500 learnosity_sdk-0.3.3/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4689 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/tests/integration/test_dataapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:17:40.275443 learnosity_sdk-0.3.3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/tests/unit/test_dataapi.py
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-07-13 06:11:15.000000 learnosity_sdk-0.3.3/tests/unit/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/tests/unit/test_sdk.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-13 05:27:20.000000 learnosity_sdk-0.3.3/tests/unit/test_uuid.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `learnosity_sdk-0.3.2/learnosity_sdk/request/dataapi.py` & `learnosity_sdk-0.3.3/learnosity_sdk/request/dataapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             DataApiException: Raised if there was a problem fetching
             data or if the server returns an invalid response.
         """
         for response in self.request_iter(endpoint, security_packet,
                                           secret, request_packet,
                                           action):
             if type(response['data']) == dict:
-                for key, value in self.__iteritems(response['data']):
+                for key, value in response['data'].iteritems():
                     yield {key: value}
             else:
                 for result in response['data']:
                     yield result
 
     def request_iter(self, endpoint, security_packet,
                      secret, request_packet={},
@@ -124,28 +124,7 @@
                 data_end = True
 
             if not data['meta']['status']:
                 raise DataApiException(
                     'server returned unsuccessful status: ' + res.text)
             else:
                 yield data
-
-    """
-    This helper method allows the .items method of Python 3
-    to be wrapped to the equivalent .iteritems method
-    of Python 2.7
-
-    The code for this method was sourced from Python Future:
-    https://python-future.org/
-
-    Python Future is licenced under the MIT Licence. Full licence details
-    and credits can be found here:
-    https://python-future.org/credits.html
-    """
-    @staticmethod
-    def __iteritems(obj, **kwargs):
-        func = getattr(obj, "iteritems", None)
-
-        if not func:
-            func = obj.items
-
-        return func(**kwargs)
```

### Comparing `learnosity_sdk-0.3.2/learnosity_sdk/request/init.py` & `learnosity_sdk-0.3.3/learnosity_sdk/request/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import datetime
 import hashlib
+import hmac
 import json
 import platform
 from learnosity_sdk._version import __version__
 
 from learnosity_sdk.exceptions import ValidationException
 
 
@@ -33,15 +34,17 @@
 
     def __init__(
             self, service, security, secret,
             request=None, action=None):
         self.service = service
         self.security = security.copy()
         self.secret = secret
-        self.request = request.copy()
+        self.request = request
+        if hasattr(request, 'copy'):
+            self.request = request.copy()
         self.action = action
 
         self.validate()
         self.add_telemetry_data()
         self.request_string = self.generate_request_string()
         self.sign_request_data = True
         self.set_service_options()
@@ -94,15 +97,15 @@
 
             if self.request is not None:
                 output['request'] = self.request
 
             if self.action is not None:
                 output['action'] = self.action
 
-        if encode:
+        if encode or self.request_passed_as_string:
             return json.dumps(output)
         else:
             return output
 
     def get_sdk_meta(self):
         return {
             'version': self.get_sdk_version(),
@@ -114,29 +117,26 @@
 
     def get_sdk_version(self):
         return __version__
 
     def generate_request_string(self):
         if self.request is None:
             return None
-        return json.dumps(self.request, separators=(',', ':'))
+        return json.dumps(self.request, separators=(',', ':'), ensure_ascii=False)
 
     def generate_signature(self):
 
         vals = []
 
         # Add each valid security field.
         # The order is signifcant.
         for key in self.security_keys:
             if key in self.security:
                 vals.append(self.security[key])
 
-        # Add the secret.
-        vals.append(self.secret)
-
         # Add the request if necessary
         if self.sign_request_data and self.request_string is not None:
             vals.append(self.request_string)
 
         if self.action is not None:
             vals.append(self.action)
 
@@ -144,25 +144,27 @@
 
     def validate(self):
         # Parse the security packet if the user provided it as a string
         if isinstance(self.security, str):
             self.security = json.loads(self.security)
 
         # Parse the request packet if the user provided it as a string
+        self.request_passed_as_string = False
         if isinstance(self.request, str):
             self.request = json.loads(self.request)
+            self.request_passed_as_string = True
 
         # Validate field lengths and types
         if len(self.service) == 0:
             raise ValidationException(
-                "The \`service\` argument wasn't found or was empty")
+                "The `service` argument wasn't found or was empty")
 
         if len(self.secret) == 0:
             raise ValidationException(
-                "The \`secret\` argument wasn't found or  was empty")
+                "The `secret` argument wasn't found or  was empty")
 
         if self.action is not None and not isinstance(self.action, str):
             raise ValidationException("The action parameter must be a string")
 
         # Check that service is valid
         if self.service not in self.services:
             raise ValidationException(
@@ -231,15 +233,17 @@
                 hashed_users[user] = hashlib.sha256(concat.encode('utf-8')).hexdigest()
 
             if len(hashed_users) > 0:
                 self.security['users'] = hashed_users
 
     def hash_list(self, l):
         "Hash a list by concatenating values with an underscore"
-        return hashlib.sha256("_".join(l).encode('utf-8')).hexdigest()
+        concatValues = "_".join(l)
+        signature =  hmac.new(bytes(str(self.secret),'utf_8'), msg = bytes(str(concatValues) , 'utf-8'), digestmod = hashlib.sha256).hexdigest()
+        return '$02$' + signature
 
     def add_telemetry_data(self):
         if self.__telemetry_enabled:
             if 'meta' in self.request:
                 self.request['meta']['sdk'] = self.get_sdk_meta()
             else:
                 self.request['meta'] = {
```

### Comparing `learnosity_sdk-0.3.2/learnosity_sdk.egg-info/SOURCES.txt` & `learnosity_sdk-0.3.3/learnosity_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+LICENSE.md
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+docs/__init__.py
+docs/quickstart/__init__.py
+docs/quickstart/config.py
 learnosity_sdk/__init__.py
 learnosity_sdk/_version.py
 learnosity_sdk/exceptions.py
 learnosity_sdk.egg-info/PKG-INFO
 learnosity_sdk.egg-info/SOURCES.txt
 learnosity_sdk.egg-info/dependency_links.txt
+learnosity_sdk.egg-info/entry_points.txt
 learnosity_sdk.egg-info/requires.txt
 learnosity_sdk.egg-info/top_level.txt
 learnosity_sdk/request/__init__.py
 learnosity_sdk/request/dataapi.py
 learnosity_sdk/request/init.py
 learnosity_sdk/utils/__init__.py
 learnosity_sdk/utils/lrnuuid.py
```

### Comparing `learnosity_sdk-0.3.2/tests/integration/test_dataapi.py` & `learnosity_sdk-0.3.3/tests/integration/test_dataapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,14 +74,33 @@
         for page in pages:
             if page['data']:
                 results.add(page['data'][0]['reference'])
 
         assert len(results) == 2
         assert results == {'item_2', 'item_3'}
 
+    def test_real_request_with_special_characters(self):
+        """Make a request against Data Api to ensure the SDK works"""
+        client = DataApi()
+
+        # Add a reference containing special characters to ensure
+        # signature creation works with special characters in the request
+        local_items_request = items_request.copy()  # prevent modifying the base fixture
+        local_items_request['references'] = items_request['references'].copy()  # prevent modifying the base fixture's list
+        local_items_request['references'].append('тест')
+
+        res = client.request(self.__build_base_url() + items_endpoint, security, consumer_secret, items_request,
+                             action)
+        returned_json = res.json()
+
+        assert len(returned_json['data']) > 0
+
+        returned_ref = returned_json['data'][0]['reference']
+        assert returned_ref in items_request['references']
+
     def test_real_question_request(self):
         """Make a request against Data Api to ensure the SDK works"""
         client = DataApi()
 
         questions_request['limit'] = 3
         res = client.request(self.__build_base_url() + questions_endpoint, security, consumer_secret, questions_request,
                              action)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `learnosity_sdk-0.3.2/tests/unit/test_dataapi.py` & `learnosity_sdk-0.3.3/tests/unit/test_dataapi.py`

 * *Files identical despite different names*

### Comparing `learnosity_sdk-0.3.2/tests/unit/test_sdk.py` & `learnosity_sdk-0.3.3/tests/unit/test_sdk.py`

 * *Files identical despite different names*

### Comparing `learnosity_sdk-0.3.2/setup.py` & `learnosity_sdk-0.3.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,42 +3,51 @@
 # Loads __version__ using exec as setup.py can't import its own package
 version = {}
 version_file = 'learnosity_sdk/_version.py'
 exec(open(version_file).read(), { '__builtins__': None }, version)
 if '__version__' not in version:
     raise Exception('__version__ not found in file %s' % version_file)
 
-
 INSTALL_REQUIRES = [
     'requests >=2.21.0',
 ]
 
 DEV_REQUIRES = [
     'setuptools',
-    'tox',
     'twine',
     'wheel',
 ]
 
 TEST_REQUIRES = [
-    'pytest >=4.6.6, <6.0',
-    'pytest-cov >=2.8.1, <3.0',
-    'responses >=0.8.1, <1.0',
+    'pytest >=4.6.6',
+    'pytest-cov >=2.8.1',
+    'pytest-subtests',
+    'responses >=0.8.1',
 ]
 
+# Extract the markdown content of the README to be sent to Pypi as the project description page.
+with open("README.md", "r") as f:
+    readmeText = f.read()
 
 setuptools.setup(
     author='Learnosity',
     author_email='sdk@learnosity.com',
     url='https://github.com/Learnosity/learnosity-sdk-python',
     version=version['__version__'],
+    license='Apache 2.0 license. See LICENSE.md for details.',
     name='learnosity_sdk',
     description='Learnosity SDK for Python',
-
+    long_description=readmeText, # Pulled from README.me on line 28
+    long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=('tests')),
-
     install_requires=INSTALL_REQUIRES,
     extras_require={
         'dev': DEV_REQUIRES,
         'test': TEST_REQUIRES,
+        'quickstart': ['jinja2'],
+    },
+    entry_points={
+    'console_scripts': [
+        'learnosity-sdk-assessment-quickstart=docs.quickstart.assessment.standalone_assessment:main [quickstart]',
+    ],
     },
 )
```

