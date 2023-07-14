# Comparing `tmp/inpython-package-1.0.1.tar.gz` & `tmp/inpython-package-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpython-package-1.0.1.tar", last modified: Fri Jul 14 13:00:04 2023, max compression
+gzip compressed data, was "inpython-package-1.0.2.tar", last modified: Fri Jul 14 14:17:18 2023, max compression
```

## Comparing `inpython-package-1.0.1.tar` & `inpython-package-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:00:04.080948 inpython-package-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-07-14 11:17:43.000000 inpython-package-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1095 2023-07-14 13:00:04.077896 inpython-package-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      765 2023-07-14 10:04:54.000000 inpython-package-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 13:00:03.833905 inpython-package-1.0.1/inpython/
--rw-rw-rw-   0        0        0       47 2023-07-14 10:00:44.000000 inpython-package-1.0.1/inpython/__init__.py
--rw-rw-rw-   0        0        0       30 2023-07-14 10:01:04.000000 inpython-package-1.0.1/inpython/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:00:03.939894 inpython-package-1.0.1/inpython/ingraph/
--rw-rw-rw-   0        0        0      162 2023-07-14 11:05:33.000000 inpython-package-1.0.1/inpython/ingraph/__init__.py
--rw-rw-rw-   0        0        0     2263 2023-07-14 09:55:45.000000 inpython-package-1.0.1/inpython/ingraph/ingraph.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:00:04.074892 inpython-package-1.0.1/inpython_package.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-07-14 13:00:03.000000 inpython-package-1.0.1/inpython_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-07-14 13:00:03.000000 inpython-package-1.0.1/inpython_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:00:03.000000 inpython-package-1.0.1/inpython_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 13:00:03.000000 inpython-package-1.0.1/inpython_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 13:00:03.000000 inpython-package-1.0.1/inpython_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 13:00:04.080948 inpython-package-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      670 2023-07-14 12:59:34.000000 inpython-package-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:17:18.791944 inpython-package-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-14 11:17:43.000000 inpython-package-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1095 2023-07-14 14:17:18.789937 inpython-package-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2023-07-14 10:04:54.000000 inpython-package-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 14:17:18.463933 inpython-package-1.0.2/inpython/
+-rw-rw-rw-   0        0        0       47 2023-07-14 10:00:44.000000 inpython-package-1.0.2/inpython/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-07-14 10:01:04.000000 inpython-package-1.0.2/inpython/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:17:18.756946 inpython-package-1.0.2/inpython/ingraph/
+-rw-rw-rw-   0        0        0      162 2023-07-14 11:05:33.000000 inpython-package-1.0.2/inpython/ingraph/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-07-14 14:16:24.000000 inpython-package-1.0.2/inpython/ingraph/ingraph.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:17:18.786953 inpython-package-1.0.2/inpython_package.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-07-14 14:17:18.000000 inpython-package-1.0.2/inpython_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-07-14 14:17:18.000000 inpython-package-1.0.2/inpython_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:17:18.000000 inpython-package-1.0.2/inpython_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 14:17:18.000000 inpython-package-1.0.2/inpython_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 14:17:18.000000 inpython-package-1.0.2/inpython_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 14:17:18.791944 inpython-package-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      670 2023-07-14 14:17:04.000000 inpython-package-1.0.2/setup.py
```

### Comparing `inpython-package-1.0.1/LICENSE.txt` & `inpython-package-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inpython-package-1.0.1/PKG-INFO` & `inpython-package-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpython-package
-Version: 1.0.1
+Version: 1.0.2
 Summary: # Infodata's IN-Tools U2Python Package
 Home-page: https://bitbucket.org/infodata-dev/inpython
 Author: infodata
 Author-email: info@infodata.lu
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `inpython-package-1.0.1/README.md` & `inpython-package-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `inpython-package-1.0.1/inpython/ingraph/ingraph.py` & `inpython-package-1.0.2/inpython/ingraph/ingraph.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json 
 import msal 
 
 def helloWorld():
      print("hellp from inpython")
 
 
+
 def getGraphTokenFromCertificate(path): 
 # fonctions pour générer un token Graph avec un certificat
 # retourne un objet string json 
 # 
 # c.f. 
 # https://github.com/Azure-Samples/ms-identity-python-daemon/tree/master/2-Call-MsGraph-WithCertificate
 
@@ -19,41 +20,46 @@
      #   "authority": "https://login.microsoftonline.com/infodata.lu",
      #   "tenant_id": "e2a26e34-3...",
      #   "client_id": "15855fc2-...",
      #   "scope": [ "https://graph.microsoft.com/.default" ],
      #   "thumbprint": "9615472D8...",
      #   "private_key_file": "...//9615472D8...//9615472D8....privatekey"
      # }
-
+     
      try:
-          config = json.load(path)
+          f = open(path)
+          config = json.load(f)
      except: # catch *all* exceptions
-          result = {"errorCode":"1",
-                    "errorFrom":"json.load({0})".format(path), 
-                    "error":sys.exc_info()[0]}
+          result = {"errorCode" : "1",
+                    "errorFrom" : "json.load({0})".format(path), 
+                    "error"     : "{0}".format(sys.exc_info()[0])
+                    }
+          print(result)
           return json.dumps(result)
      
      # try to connect
      try:
           app = msal.ConfidentialClientApplication(
                config["client_id"], 
                authority=config["authority"],
                client_credential={"thumbprint": config["thumbprint"], 
                               "private_key": open(config['private_key_file']).read()},
                )
      except:
-          result = {"errorCode":"2",
-                    "errorFrom":"msal.ConfidentialClientApplication(authority={authority}, client_credentials=thumbprint={thumbprint}, privatekey={privatekey})".format(authority=config["authority"], thumbprint=config["thumbprint"], privatekey=config['private_key_file']), 
-                    "error":sys.exc_info()[0] }
+          result = {"errorCode" : "2",
+                    "errorFrom" : "msal.ConfidentialClientApplication(authority={authority}, client_credentials=thumbprint={thumbprint}, privatekey={privatekey})".format(authority=config["authority"], thumbprint=config["thumbprint"], privatekey=config['private_key_file']), 
+                    "error" : "{0}".format(sys.exc_info()[0])
+                    }
           return json.dumps(result)
-     
+
      # try to get a token
      result = None
      try:
           result = app.acquire_token_for_client(scopes=config["scope"])
      except:
-          result = {"errorCode":"3",
-                    "errorFrom":"app.acquire_token_for_client {scopes}=".format(scopes=config["scope"]) , 
-                    "error":sys.exc_info()[0]}
+          result = {"errorCode" : "3",
+                    "errorFrom" : "app.acquire_token_for_client {scopes}=".format(scopes=config["scope"]) , 
+                    "error" : "{0}".format(sys.exc_info()[0])
+                    }
           return json.dumps(result)
 
      return json.dumps(result)
```

### Comparing `inpython-package-1.0.1/inpython_package.egg-info/PKG-INFO` & `inpython-package-1.0.2/inpython_package.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpython-package
-Version: 1.0.1
+Version: 1.0.2
 Summary: # Infodata's IN-Tools U2Python Package
 Home-page: https://bitbucket.org/infodata-dev/inpython
 Author: infodata
 Author-email: info@infodata.lu
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `inpython-package-1.0.1/setup.py` & `inpython-package-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="inpython-package",
-    version="1.0.1",
+    version="1.0.2",
     author="infodata",
     author_email="info@infodata.lu",
     packages=find_packages(),
     description="# Infodata's IN-Tools U2Python Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/infodata-dev/inpython",
```

