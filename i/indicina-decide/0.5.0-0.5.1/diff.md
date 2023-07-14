# Comparing `tmp/indicina-decide-0.5.0.tar.gz` & `tmp/indicina-decide-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indicina-decide-0.5.0.tar", last modified: Thu Mar 30 12:04:18 2023, max compression
+gzip compressed data, was "indicina-decide-0.5.1.tar", last modified: Fri Jul 14 11:10:31 2023, max compression
```

## Comparing `indicina-decide-0.5.0.tar` & `indicina-decide-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:04:18.548600 indicina-decide-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22232 2023-03-30 12:04:18.548600 indicina-decide-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22009 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:04:18.544600 indicina-decide-0.5.0/decide/
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/auth.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/globals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:04:18.544600 indicina-decide-0.5.0/decide/models/
--rw-r--r--   0 root         (0) root         (0)      169 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6370 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/analysis.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/base.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/client.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/enums.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/error.py
--rw-r--r--   0 root         (0) root         (0)    16379 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/rules_engine.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/statement.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/models/tagged_statement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:04:18.544600 indicina-decide-0.5.0/decide/test/
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/test/conftest.py
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/test/helpers.py
--rw-r--r--   0 root         (0) root         (0)    11679 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/test/test_decide.py
--rw-r--r--   0 root         (0) root         (0)    13178 2023-03-30 12:04:14.000000 indicina-decide-0.5.0/decide/test/test_rules_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 12:04:18.548600 indicina-decide-0.5.0/indicina_decide.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22232 2023-03-30 12:04:18.000000 indicina-decide-0.5.0/indicina_decide.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      690 2023-03-30 12:04:18.000000 indicina-decide-0.5.0/indicina_decide.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 12:04:18.000000 indicina-decide-0.5.0/indicina_decide.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-30 12:04:18.000000 indicina-decide-0.5.0/indicina_decide.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-30 12:04:18.000000 indicina-decide-0.5.0/indicina_decide.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      275 2023-03-30 12:04:18.548600 indicina-decide-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      579 2023-03-30 12:04:15.000000 indicina-decide-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:10:31.285668 indicina-decide-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    22232 2023-07-14 11:10:31.285668 indicina-decide-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22009 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:10:31.277668 indicina-decide-0.5.1/decide/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/auth.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:10:31.281668 indicina-decide-0.5.1/decide/models/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/analysis.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/client.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/enums.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/error.py
+-rw-r--r--   0 root         (0) root         (0)    16379 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/rules_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/statement.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/models/tagged_statement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:10:31.281668 indicina-decide-0.5.1/decide/test/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/test/conftest.py
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/test/helpers.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/test/test_decide.py
+-rw-r--r--   0 root         (0) root         (0)    13178 2023-07-14 11:10:27.000000 indicina-decide-0.5.1/decide/test/test_rules_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:10:31.285668 indicina-decide-0.5.1/indicina_decide.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22232 2023-07-14 11:10:31.000000 indicina-decide-0.5.1/indicina_decide.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-14 11:10:31.000000 indicina-decide-0.5.1/indicina_decide.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 11:10:31.000000 indicina-decide-0.5.1/indicina_decide.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-14 11:10:31.000000 indicina-decide-0.5.1/indicina_decide.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 11:10:31.000000 indicina-decide-0.5.1/indicina_decide.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-14 11:10:31.285668 indicina-decide-0.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      579 2023-07-14 11:10:28.000000 indicina-decide-0.5.1/setup.py
```

### Comparing `indicina-decide-0.5.0/LICENSE.txt` & `indicina-decide-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/PKG-INFO` & `indicina-decide-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indicina-decide
-Version: 0.5.0
+Version: 0.5.1
 Author: Indicina Engineering
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ## decide-python-package
```

### Comparing `indicina-decide-0.5.0/README.md` & `indicina-decide-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/analysis.py` & `indicina-decide-0.5.1/decide/models/analysis.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/base.py` & `indicina-decide-0.5.1/decide/models/base.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/client.py` & `indicina-decide-0.5.1/decide/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		url = BASE_URL
 		full_path = urllib.parse.urljoin(url, self.path)
 		response = requests.request(method, full_path, headers=self.headers, **kwargs)
 		if response.status_code == 401:
 			self.auth.refresh()  # refresh token
 			return requests.request(method, full_path, headers=self.headers, **kwargs)
 		if response.status_code != 200:
-			raise DecideException(response_code=response.status_code, message=response.text)
+			raise DecideException(status_code=response.status_code, message=response.text)
 		return response
 
 	@property
 	def headers(self):
 		return {
 			"Authorization": f"Bearer {self.auth.code}"
 		}
```

### Comparing `indicina-decide-0.5.0/decide/models/customer.py` & `indicina-decide-0.5.1/decide/models/customer.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/enums.py` & `indicina-decide-0.5.1/decide/models/enums.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/rules_engine.py` & `indicina-decide-0.5.1/decide/models/rules_engine.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/statement.py` & `indicina-decide-0.5.1/decide/models/statement.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/models/tagged_statement.py` & `indicina-decide-0.5.1/decide/models/tagged_statement.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/decide/test/test_rules_engine.py` & `indicina-decide-0.5.1/decide/test/test_rules_engine.py`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/indicina_decide.egg-info/PKG-INFO` & `indicina-decide-0.5.1/indicina_decide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indicina-decide
-Version: 0.5.0
+Version: 0.5.1
 Author: Indicina Engineering
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ## decide-python-package
```

### Comparing `indicina-decide-0.5.0/indicina_decide.egg-info/SOURCES.txt` & `indicina-decide-0.5.1/indicina_decide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indicina-decide-0.5.0/setup.py` & `indicina-decide-0.5.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
```

