# Comparing `tmp/btconfig-4.4.5.tar.gz` & `tmp/btconfig-4.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btconfig-4.4.5.tar", last modified: Fri Jun  9 20:14:34 2023, max compression
+gzip compressed data, was "btconfig-4.4.6.tar", last modified: Thu Jul 13 22:16:23 2023, max compression
```

## Comparing `btconfig-4.4.5.tar` & `btconfig-4.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:14:34.206710 btconfig-4.4.5/
--rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.4.5/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.4.5/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.4.5/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.4.5/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-06-09 20:14:34.206936 btconfig-4.4.5/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.4.5/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:14:34.199441 btconfig-4.4.5/btconfig/
--rw-r--r--   0 etejeda    (501) staff       (20)     1267 2023-05-11 11:55:36.000000 btconfig-4.4.5/btconfig/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3788 2023-05-14 18:16:20.000000 btconfig-4.4.5/btconfig/configloader.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-05-11 11:53:07.000000 btconfig-4.4.5/btconfig/configutils.py
--rw-r--r--   0 etejeda    (501) staff       (20)      897 2023-06-09 20:13:17.000000 btconfig-4.4.5/btconfig/logger.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4576 2023-05-11 11:53:09.000000 btconfig-4.4.5/btconfig/superconf.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:14:34.201763 btconfig-4.4.5/btconfig.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-06-09 20:14:34.000000 btconfig-4.4.5/btconfig.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-06-09 20:14:34.000000 btconfig-4.4.5/btconfig.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-09 20:14:34.000000 btconfig-4.4.5/btconfig.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 01:07:02.000000 btconfig-4.4.5/btconfig.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       78 2023-06-09 20:14:34.000000 btconfig-4.4.5/btconfig.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-06-09 20:14:34.000000 btconfig-4.4.5/btconfig.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-09 20:14:34.206307 btconfig-4.4.5/examples/
--rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.4.5/examples/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.4.5/examples/example1.py
--rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.4.5/examples/example2.py
--rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.4.5/examples/example3.py
--rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.4.5/examples/example4.py
--rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.4.5/examples/myconfig1.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.4.5/examples/myconfig2.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.4.5/examples/myconfig3.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.4.5/examples/myconfig4.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.4.5/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1074 2023-06-09 20:14:34.207767 btconfig-4.4.5/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.4.5/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.4.5/test.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.4.5/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 22:16:23.461198 btconfig-4.4.6/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1311 2023-01-09 20:02:16.000000 btconfig-4.4.6/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-01-09 20:02:16.000000 btconfig-4.4.6/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-01-09 20:02:16.000000 btconfig-4.4.6/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      344 2023-01-09 20:02:16.000000 btconfig-4.4.6/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-07-13 22:16:23.461450 btconfig-4.4.6/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     3132 2023-05-11 11:53:49.000000 btconfig-4.4.6/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 22:16:23.447666 btconfig-4.4.6/btconfig/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1267 2023-05-11 11:55:36.000000 btconfig-4.4.6/btconfig/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3788 2023-05-14 18:16:20.000000 btconfig-4.4.6/btconfig/configloader.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3217 2023-05-11 11:53:07.000000 btconfig-4.4.6/btconfig/configutils.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      897 2023-06-09 20:13:17.000000 btconfig-4.4.6/btconfig/logger.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4608 2023-07-13 22:13:24.000000 btconfig-4.4.6/btconfig/superconf.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 22:16:23.452877 btconfig-4.4.6/btconfig.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3796 2023-07-13 22:16:23.000000 btconfig-4.4.6/btconfig.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      604 2023-07-13 22:16:23.000000 btconfig-4.4.6/btconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-13 22:16:23.000000 btconfig-4.4.6/btconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 01:07:02.000000 btconfig-4.4.6/btconfig.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       88 2023-07-13 22:16:23.000000 btconfig-4.4.6/btconfig.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        9 2023-07-13 22:16:23.000000 btconfig-4.4.6/btconfig.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-13 22:16:23.460636 btconfig-4.4.6/examples/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3045 2023-05-11 11:53:23.000000 btconfig-4.4.6/examples/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)      157 2023-05-11 11:53:25.000000 btconfig-4.4.6/examples/example1.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      170 2023-05-11 11:53:22.000000 btconfig-4.4.6/examples/example2.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      160 2023-05-11 11:53:23.000000 btconfig-4.4.6/examples/example3.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      189 2023-05-11 11:53:24.000000 btconfig-4.4.6/examples/example4.py
+-rw-r--r--   0 etejeda    (501) staff       (20)       54 2023-01-09 20:02:16.000000 btconfig-4.4.6/examples/myconfig1.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      234 2023-01-09 20:02:16.000000 btconfig-4.4.6/examples/myconfig2.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      435 2023-01-09 20:02:16.000000 btconfig-4.4.6/examples/myconfig3.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)      208 2023-01-09 20:02:16.000000 btconfig-4.4.6/examples/myconfig4.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-01-09 20:02:16.000000 btconfig-4.4.6/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1085 2023-07-13 22:16:23.462815 btconfig-4.4.6/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-01-09 20:02:16.000000 btconfig-4.4.6/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      248 2023-05-11 11:54:41.000000 btconfig-4.4.6/test.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-01-09 20:02:16.000000 btconfig-4.4.6/tox.ini
```

### Comparing `btconfig-4.4.5/.gitignore` & `btconfig-4.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/LICENSE` & `btconfig-4.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/PKG-INFO` & `btconfig-4.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.4.5
+Version: 4.4.6
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.4.5/README.md` & `btconfig-4.4.6/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/btconfig/__init__.py` & `btconfig-4.4.6/btconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/btconfig/configloader.py` & `btconfig-4.4.6/btconfig/configloader.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/btconfig/configutils.py` & `btconfig-4.4.6/btconfig/configutils.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/btconfig/logger.py` & `btconfig-4.4.6/btconfig/logger.py`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/btconfig/superconf.py` & `btconfig-4.4.6/btconfig/superconf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from btconfig.logger import Logger
 from btconfig.configutils import AttrDict
 from btconfig.configloader import ConfigLoader
 import sys
 from jinja2 import Template
 import yaml
+from pyaml_env import parse_config
 
 # Setup Logging
 logger = Logger().init_logger(__name__)
 
 class SuperDuperConfig(ConfigLoader):
 
   def render(self, **kwargs):
@@ -16,17 +17,17 @@
     config_file_uri = kwargs.get('uri')
     config_dict = {}
     config_is_valid = False
     invalid_keys = []
 
     try:
       if not config_content:
-        ymlfile_content = open(config_file_uri).read()
+        ymlfile_content = parse_config(config_file_uri)
       else:
-        ymlfile_content = config_content
+        ymlfile_content = parse_config(data=config_content)
       if self.templatized:
         try:
           ymlfile_template = Template(ymlfile_content)
           ymlfile_data = ymlfile_template.render(
             session=self.initial_data
           )
         except Exception as e:
@@ -36,16 +37,15 @@
           )
           if self.failfast:
             sys.exit(1)
           else:
             ymlfile_data = ymlfile_content
       else:
         ymlfile_data = ymlfile_content
-      cfg = yaml.safe_load(ymlfile_data)
-      config_dict = cfg[self.data_key] if self.data_key is not None else cfg
+      config_dict = ymlfile_data[self.data_key] if self.data_key is not None else ymlfile_data
       if isinstance(config_dict, dict):
         config_dict['config_file_uri'] = config_file_uri
       else:
         _config_dict = [e for e in config_dict if isinstance(e, dict)]
         if len(_config_dict) >= 0:
           config_dict = config_dict[0]
           config_dict['config_file_uri'] = config_file_uri
```

### Comparing `btconfig-4.4.5/btconfig.egg-info/PKG-INFO` & `btconfig-4.4.6/btconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btconfig
-Version: 4.4.5
+Version: 4.4.6
 Summary: Module for reading configuration files
 Home-page: https://github.com/berttejeda/bert.config
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btconfig-4.4.5/btconfig.egg-info/SOURCES.txt` & `btconfig-4.4.6/btconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/examples/README.md` & `btconfig-4.4.6/examples/README.md`

 * *Files identical despite different names*

### Comparing `btconfig-4.4.5/setup.cfg` & `btconfig-4.4.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btconfig
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Module for reading configuration files
-version = 4.4.5
+version = 4.4.6
 url = https://github.com/berttejeda/bert.config
 keywords = 
 	yaml
 	configuration
 	config
 	file
 	python
@@ -37,14 +37,15 @@
 zip_safe = False
 scripts = 
 install_requires = 
 	jinja2
 	PyYAML
 	requests
 	btweb
+	pyaml-env
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-cov
 	coveralls
 	flake8
```

