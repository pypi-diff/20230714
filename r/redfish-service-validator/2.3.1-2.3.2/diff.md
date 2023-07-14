# Comparing `tmp/redfish_service_validator-2.3.1.tar.gz` & `tmp/redfish_service_validator-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_service_validator-2.3.1.tar", last modified: Fri Apr 21 19:24:05 2023, max compression
+gzip compressed data, was "redfish_service_validator-2.3.2.tar", last modified: Fri Jul 14 20:45:42 2023, max compression
```

## Comparing `redfish_service_validator-2.3.1.tar` & `redfish_service_validator-2.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/redfish_service_validator/
--rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/RedfishLogo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11487 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16495 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidatorGui.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47588 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/schema_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/traverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/validateRedfish.py
--rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:45:42.583528 redfish_service_validator-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-14 20:45:42.583528 redfish_service_validator-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:45:42.583528 redfish_service_validator-2.3.2/redfish_service_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/RedfishLogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11550 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/RedfishServiceValidator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16500 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/RedfishServiceValidatorGui.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47588 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/schema_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/validateRedfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/redfish_service_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:45:42.583528 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-14 20:45:42.000000 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-14 20:45:42.000000 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:45:42.000000 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 20:45:42.000000 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 20:45:42.000000 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 20:45:42.000000 redfish_service_validator-2.3.2/redfish_service_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:45:42.583528 redfish_service_validator-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 20:45:29.000000 redfish_service_validator-2.3.2/setup.py
```

### Comparing `redfish_service_validator-2.3.1/LICENSE.md` & `redfish_service_validator-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/PKG-INFO` & `redfish_service_validator-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.3.1
+Version: 2.3.2
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.3.1/README.md` & `redfish_service_validator-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/RedfishLogo.py` & `redfish_service_validator-2.3.2/redfish_service_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidator.py` & `redfish_service_validator-2.3.2/redfish_service_validator/RedfishServiceValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from redfish_service_validator.config import convert_config_to_args, convert_args_to_config
 from redfish_service_validator.validateResource import validateSingleURI, validateURITree
 import redfish_service_validator.schema as schema
 from redfish_service_validator import tohtml, schema_pack, traverse
 from urllib.parse import urlparse, urlunparse
 from collections import Counter
 
-tool_version = '2.3.1'
+tool_version = '2.3.2'
 
 # Set up the custom debug levels
 VERBOSE1=logging.INFO-1
 VERBOSE2=logging.INFO-2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
@@ -38,15 +38,15 @@
 
 my_logger = logging.getLogger()
 my_logger.setLevel(logging.DEBUG)
 standard_out = logging.StreamHandler(sys.stdout)
 standard_out.setLevel(logging.INFO)
 my_logger.addHandler(standard_out)
 
-def main(argslist=None, configfile=None):
+def validate(argslist=None, configfile=None):
     """Main command
 
     Args:
         argslist ([type], optional): List of arguments in the form of argv. Defaults to None.
     """    
     argget = argparse.ArgumentParser(description='DMTF tool to test a service against a collection of Schema, version {}'.format(tool_version))
 
@@ -238,11 +238,16 @@
         my_logger.error("Validation has failed: {} problems found".format(fails))
     else:
         my_logger.info("Validation has succeeded.")
         status_code = 0
 
     return status_code, lastResultsPage, 'Validation done'
 
+def main():
+    """
+    Entry point for the program.
+    """
+    status_code, _, _ = validate()
+    return status_code
 
 if __name__ == '__main__':
-    status_code, lastResultsPage, exit_string = main()
-    sys.exit(status_code)
+    sys.exit(main())
```

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidatorGui.py` & `redfish_service_validator-2.3.2/redfish_service_validator/RedfishServiceValidatorGui.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         run_button_frame.pack( side = tk.BOTTOM )
         tk.Button( run_button_frame, text = "OK", command = run_window.destroy ).pack( side = tk.LEFT )
         tk.Button( run_button_frame, text = "Copy", command = lambda: self.copy_text( run_text ) ).pack( side = tk.RIGHT )
 
         # Launch the validator
         try:
             rsv_config = self.build_config_parser( False )
-            status_code, last_results_page, exit_string = rsv.main(configfile = rsv_config )
+            status_code, last_results_page, exit_string = rsv.validate( configfile = rsv_config )
             if last_results_page is not None:
                 webbrowser.open_new( last_results_page )
             else:
                 # The validation could not take place (for a controlled reason)
                 notification_window = tk.Toplevel()
                 tk.Label( notification_window, text = "Test aborted: " + exit_string, anchor = "center" ).pack( side = tk.TOP )
                 tk.Button( notification_window, text = "OK", command = notification_window.destroy ).pack( side = tk.BOTTOM )
```

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/catalog.py` & `redfish_service_validator-2.3.2/redfish_service_validator/catalog.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/config.py` & `redfish_service_validator-2.3.2/redfish_service_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/helper.py` & `redfish_service_validator-2.3.2/redfish_service_validator/helper.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/metadata.py` & `redfish_service_validator-2.3.2/redfish_service_validator/metadata.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/schema.py` & `redfish_service_validator-2.3.2/redfish_service_validator/schema.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/schema_pack.py` & `redfish_service_validator-2.3.2/redfish_service_validator/schema_pack.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/tohtml.py` & `redfish_service_validator-2.3.2/redfish_service_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/traverse.py` & `redfish_service_validator-2.3.2/redfish_service_validator/traverse.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/validateRedfish.py` & `redfish_service_validator-2.3.2/redfish_service_validator/validateRedfish.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator/validateResource.py` & `redfish_service_validator-2.3.2/redfish_service_validator/validateResource.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator.egg-info/PKG-INFO` & `redfish_service_validator-2.3.2/redfish_service_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-service-validator
-Version: 2.3.1
+Version: 2.3.2
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.3.1/redfish_service_validator.egg-info/SOURCES.txt` & `redfish_service_validator-2.3.2/redfish_service_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.1/setup.py` & `redfish_service_validator-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_service_validator",
-    version="2.3.1",
+    version="2.3.2",
     description="Redfish Service Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

