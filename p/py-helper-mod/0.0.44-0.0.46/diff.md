# Comparing `tmp/py-helper-mod-0.0.44.tar.gz` & `tmp/py-helper-mod-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-helper-mod-0.0.44.tar", last modified: Thu Jul 13 18:14:27 2023, max compression
+gzip compressed data, was "py-helper-mod-0.0.46.tar", last modified: Fri Jul 14 15:40:02 2023, max compression
```

## Comparing `py-helper-mod-0.0.44.tar` & `py-helper-mod-0.0.46.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 18:14:27.756018 py-helper-mod-0.0.44/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.44/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-13 18:14:27.760018 py-helper-mod-0.0.44/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.44/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91099 2023-07-13 18:11:33.000000 py-helper-mod-0.0.44/py_helper.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 18:14:27.756018 py-helper-mod-0.0.44/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-13 18:14:27.000000 py-helper-mod-0.0.44/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-13 18:14:27.000000 py-helper-mod-0.0.44/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-13 18:14:27.000000 py-helper-mod-0.0.44/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-13 18:14:27.000000 py-helper-mod-0.0.44/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.44/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-13 18:14:27.760018 py-helper-mod-0.0.44/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.44/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-14 15:40:02.834390 py-helper-mod-0.0.46/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.46/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-14 15:40:02.838390 py-helper-mod-0.0.46/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.46/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    91200 2023-07-14 15:38:25.000000 py-helper-mod-0.0.46/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-14 15:40:02.834390 py-helper-mod-0.0.46/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      644 2023-07-14 15:40:02.000000 py-helper-mod-0.0.46/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-07-14 15:40:02.000000 py-helper-mod-0.0.46/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-14 15:40:02.000000 py-helper-mod-0.0.46/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-07-14 15:40:02.000000 py-helper-mod-0.0.46/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.46/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-07-14 15:40:02.838390 py-helper-mod-0.0.46/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.46/setup.py
```

### Comparing `py-helper-mod-0.0.44/LICENSE` & `py-helper-mod-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.44/PKG-INFO` & `py-helper-mod-0.0.46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.44
+Version: 0.0.46
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.44/py_helper.py` & `py-helper-mod-0.0.46/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,15 +1181,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,43)
+VERSION=(0,0,45)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1439,32 +1439,38 @@
 def IsDebugLabelEnabled(dbglabel):
 	"""Check if Debug Label is Enabled"""
 
 	global DebugLabels, DebugLabelExists
 
 	enabled = not DebugLabelExists
 
+	dbglb = None
+
 	if DebugLabels is not None and dbglabel is not None:
 		if type(dbglabel) is str and dbglabel in DebugLabels:
 			enabled = DebugLabels[dbglabel]
+			dbglb = dbglabel
 		elif type(dbglabel) is list:
 			for lbl in dbglabel:
 				if lbl in DebugLabels:
 					enabled = DebugLabels[lbl]
 
+					if enabled:
+						dbglb = lbl
+
 					# only break when enabled. This allows the full list of labels to be checked. Slower, but who cares, we're
 					# Debugging...
 					if enabled: break
 
-	return enabled
+	return enabled,dbglb
 
 def Breakpoint(dbglabel,test_flag=True):
 	"""Check if Debug Label is Enabled AND We Are In DebugMode"""
 
-	enabled = IsDebugLabelEnabled(dbglabel)
+	enabled,dbglb = IsDebugLabelEnabled(dbglabel)
 
 	return (DebugMode() and enabled and test_flag)
 
 
 # A Centrally Controlled Debug Messaging System
 # msg : Message to print
 # func : A simple function to pass the message to (optional)
@@ -1474,15 +1480,17 @@
 	Messaging function that only prints when in DebugMode.
 	Ignores CmdLineMode/ModuleMode.
 	"""
 
 	global __DebugMode__
 
 	if __DebugMode__:
-		if not IsDebugLabelEnabled(dbglabel):
+		flag,dbglb = IsDebugEnabled(dbglabel)
+
+		if not flag:
 			return False
 
 		delta = None
 
 		int_stamp = DbgMsg.__annotations__.get("interval_stamp",None)
 
 		if int_stamp != None:
@@ -1511,15 +1519,15 @@
 			prefix = f"{prefix} {datetime.now()}"
 
 		if delta != None:
 			msg = f"{msg} - Delta from last call {delta}"
 
 		# Just because I don't like putting null pointers into string functions... I know python None is not a null pointer, but it rubs
 		# me the wrong way allowing this anyway.
-		dbglbl = "None" if dbglabel is None else dbglabel
+		dbglbl = "None" if dbglb is None else dbglb
 
 		adjusted = f"{prefix} {caller_str}/{dbglbl} : {msg}" if caller_str != "" else f"{prefix} : {msg}"
 
 		Msg(adjusted,func,ignoreModuleMode=True,end=end,file=file,flush=flush)
 
 		# If True, tells caller to break
 		return break_point
@@ -1529,23 +1537,23 @@
 
 # Block Enter Debug Messages
 def DbgEnter(msg,func=None,prefix="-->",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""DbgMsg Helper Function Output a message when entering a code block"""
 
 	message = f"Entering {msg}"
 
-	return DbgMsg(msg,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
+	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
 
 # Block Exit Debug Messages
 def DbgExit(msg,func=None,prefix="<--",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""DbgMsg Helper Function Output a message when exitting a code block"""
 
 	message = f"Exitting {msg}"
 
-	return DbgMsg(msg,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
+	return DbgMsg(message,func=func,prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,interval_stamp=interval_stamp,dbglabel=dbglabel)
 
 # DbgAuto Messages
 def DbgAuto(msg="Auto Dbg",prefix="[* DbgAuto *]",callerframe=None,timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,dbglabel=None):
 	"""
 	Generate an Automated DbgMsg With File-Line number and optional msg
 
 	Generally the purpose here is generate temporary debug scaffolding messages for
```

### Comparing `py-helper-mod-0.0.44/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.46/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.44
+Version: 0.0.46
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-helper-mod-0.0.44/setup.cfg` & `py-helper-mod-0.0.46/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.44
+version = 0.0.46
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

