# Comparing `tmp/py-helper-mod-0.0.47.tar.gz` & `tmp/py-helper-mod-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.47.tar", last modified: Fri Jul 14 17:24:04 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.48.tar", last modified: Fri Jul 14 18:02:08 2023, max compression
```

## Comparing `py-helper-mod-0.0.47.tar` & `py-helper-mod-0.0.48.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-14 17:24:04.862555 py-helper-mod-0.0.47/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.47/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-14 17:24:04.862555 py-helper-mod-0.0.47/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.47/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91205 2023-07-14 17:23:25.000000 py-helper-mod-0.0.47/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-14 17:24:04.862555 py-helper-mod-0.0.47/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-14 17:24:04.000000 py-helper-mod-0.0.47/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-14 17:24:04.000000 py-helper-mod-0.0.47/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-14 17:24:04.000000 py-helper-mod-0.0.47/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-14 17:24:04.000000 py-helper-mod-0.0.47/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.47/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-14 17:24:04.862555 py-helper-mod-0.0.47/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.47/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-14 18:02:08.522834 py-helper-mod-0.0.48/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.48/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-14 18:02:08.522834 py-helper-mod-0.0.48/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.48/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91349 2023-07-14 18:01:10.000000 py-helper-mod-0.0.48/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-14 18:02:08.522834 py-helper-mod-0.0.48/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-14 18:02:08.000000 py-helper-mod-0.0.48/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-14 18:02:08.000000 py-helper-mod-0.0.48/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-14 18:02:08.000000 py-helper-mod-0.0.48/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-14 18:02:08.000000 py-helper-mod-0.0.48/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.48/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-14 18:02:08.522834 py-helper-mod-0.0.48/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.48/setup.py
```

### Comparing `py-helper-mod-0.0.47/LICENSE` & `py-helper-mod-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.47/PKG-INFO` & `py-helper-mod-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.47
+Version: 0.0.48
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.47/py_helper.py` & `py-helper-mod-0.0.48/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,46)
+VERSION=(0,0,47)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1537,22 +1537,28 @@
 
 # Block Enter Debug Messages
 def DbgEnter(msg,func=None,prefix="-->",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""DbgMsg Helper Function Output a message when entering a code block"""
 
 	message = f"Entering {msg}"
 
+	if callerframe == None:
+		callerframe = inspect.currentframe().f_back
+
 	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
 
 # Block Exit Debug Messages
 def DbgExit(msg,func=None,prefix="<--",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""DbgMsg Helper Function Output a message when exitting a code block"""
 
 	message = f"Exitting {msg}"
 
+	if callerframe == None:
+		callerframe = inspect.currentframe().f_back
+
 	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
 
 # DbgAuto Messages
 def DbgAuto(msg="Auto Dbg",prefix="[* DbgAuto *]",callerframe=None,timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,dbglabel=None):
 	"""
 	Generate an Automated DbgMsg With File-Line number and optional msg
```

### Comparing `py-helper-mod-0.0.47/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.48/py_helper_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.47
+Version: 0.0.48
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.47/setup.cfg` & `py-helper-mod-0.0.48/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.47
+version = 0.0.48
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

