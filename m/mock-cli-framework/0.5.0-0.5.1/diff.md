# Comparing `tmp/mock-cli-framework-0.5.0.tar.gz` & `tmp/mock-cli-framework-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock-cli-framework-0.5.0.tar", last modified: Mon Jul 10 22:51:27 2023, max compression
+gzip compressed data, was "mock-cli-framework-0.5.1.tar", last modified: Fri Jul 14 02:07:03 2023, max compression
```

## Comparing `mock-cli-framework-0.5.0.tar` & `mock-cli-framework-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.909373 mock-cli-framework-0.5.0/
--rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.5.0/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     9890 2023-07-10 22:51:27.909436 mock-cli-framework-0.5.0/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     9452 2023-07-10 22:44:06.000000 mock-cli-framework-0.5.0/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.908559 mock-cli-framework-0.5.0/mock_cli/
--rw-r--r--   0 zach       (502) staff       (20)      541 2023-07-10 22:50:10.000000 mock-cli-framework-0.5.0/mock_cli/__about__.py
--rw-r--r--   0 zach       (502) staff       (20)      513 2023-07-01 05:01:04.000000 mock-cli-framework-0.5.0/mock_cli/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.5.0/mock_cli/about.py
--rw-r--r--   0 zach       (502) staff       (20)      791 2023-06-16 22:37:28.000000 mock-cli-framework-0.5.0/mock_cli/argv_conversion.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.908712 mock-cli-framework-0.5.0/mock_cli/data/
--rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.5.0/mock_cli/data/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.5.0/mock_cli/hashing.py
--rw-r--r--   0 zach       (502) staff       (20)     2507 2023-06-21 02:46:51.000000 mock-cli-framework-0.5.0/mock_cli/mock_cmd.py
--rw-r--r--   0 zach       (502) staff       (20)     6872 2023-07-01 05:01:04.000000 mock-cli-framework-0.5.0/mock_cli/mock_cmd_state.py
--rw-r--r--   0 zach       (502) staff       (20)     1013 2021-02-03 00:37:32.000000 mock-cli-framework-0.5.0/mock_cli/path.py
--rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.5.0/mock_cli/pkg_resources.py
--rw-r--r--   0 zach       (502) staff       (20)     8928 2023-03-14 03:44:06.000000 mock-cli-framework-0.5.0/mock_cli/responses.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-10 22:51:27.909256 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     9890 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      452 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        9 2023-07-10 22:51:27.000000 mock-cli-framework-0.5.0/mock_cli_framework.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)      156 2023-07-10 22:51:27.909660 mock-cli-framework-0.5.0/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)      708 2021-02-05 23:19:45.000000 mock-cli-framework-0.5.0/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-14 02:07:03.650325 mock-cli-framework-0.5.1/
+-rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.5.1/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     9890 2023-07-14 02:07:03.650398 mock-cli-framework-0.5.1/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     9452 2023-07-10 22:44:06.000000 mock-cli-framework-0.5.1/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-14 02:07:03.649345 mock-cli-framework-0.5.1/mock_cli/
+-rw-r--r--   0 zach       (502) staff       (20)      541 2023-07-14 02:06:14.000000 mock-cli-framework-0.5.1/mock_cli/__about__.py
+-rw-r--r--   0 zach       (502) staff       (20)      513 2023-07-01 05:01:04.000000 mock-cli-framework-0.5.1/mock_cli/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.5.1/mock_cli/about.py
+-rw-r--r--   0 zach       (502) staff       (20)      791 2023-06-16 22:37:28.000000 mock-cli-framework-0.5.1/mock_cli/argv_conversion.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-14 02:07:03.649590 mock-cli-framework-0.5.1/mock_cli/data/
+-rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.5.1/mock_cli/data/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.5.1/mock_cli/hashing.py
+-rw-r--r--   0 zach       (502) staff       (20)     2507 2023-06-21 02:46:51.000000 mock-cli-framework-0.5.1/mock_cli/mock_cmd.py
+-rw-r--r--   0 zach       (502) staff       (20)     6984 2023-07-14 02:06:01.000000 mock-cli-framework-0.5.1/mock_cli/mock_cmd_state.py
+-rw-r--r--   0 zach       (502) staff       (20)     1013 2021-02-03 00:37:32.000000 mock-cli-framework-0.5.1/mock_cli/path.py
+-rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.5.1/mock_cli/pkg_resources.py
+-rw-r--r--   0 zach       (502) staff       (20)     8928 2023-03-14 03:44:06.000000 mock-cli-framework-0.5.1/mock_cli/responses.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-07-14 02:07:03.650220 mock-cli-framework-0.5.1/mock_cli_framework.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     9890 2023-07-14 02:07:03.000000 mock-cli-framework-0.5.1/mock_cli_framework.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      452 2023-07-14 02:07:03.000000 mock-cli-framework-0.5.1/mock_cli_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-07-14 02:07:03.000000 mock-cli-framework-0.5.1/mock_cli_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        9 2023-07-14 02:07:03.000000 mock-cli-framework-0.5.1/mock_cli_framework.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)      156 2023-07-14 02:07:03.650609 mock-cli-framework-0.5.1/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)      708 2021-02-05 23:19:45.000000 mock-cli-framework-0.5.1/setup.py
```

### Comparing `mock-cli-framework-0.5.0/LICENSE` & `mock-cli-framework-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/PKG-INFO` & `mock-cli-framework-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.5.0
+Version: 0.5.1
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mock-cli-framework-0.5.0/README.md` & `mock-cli-framework-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/mock_cli/__about__.py` & `mock-cli-framework-0.5.1/mock_cli/__about__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = "Mock CLI Framework"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 __summary__ = """A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests."""
 
 """
 See PEP 440 for version scheme
 https://www.python.org/dev/peps/pep-0440/#examples-of-compliant-version-schemes
 Examples:
```

### Comparing `mock-cli-framework-0.5.0/mock_cli/__init__.py` & `mock-cli-framework-0.5.1/mock_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/mock_cli/argv_conversion.py` & `mock-cli-framework-0.5.1/mock_cli/argv_conversion.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/mock_cli/mock_cmd.py` & `mock-cli-framework-0.5.1/mock_cli/mock_cmd.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/mock_cli/mock_cmd_state.py` & `mock-cli-framework-0.5.1/mock_cli/mock_cmd_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,19 +215,23 @@
             state_dir = os.environ.get(STATE_DIR_ENV_NAME)
 
         if state_dir is None:
             raise MockCMDStateNoDirectoryException(
                 "No state directory path provided")
 
         state_dir = Path(state_dir)
-        if not state_dir.is_dir():
+
+        if not state_dir.exists():
             raise MockCMDStateDirException(
                 f"Invalid state directory: {state_dir}")
-        self._state_dir = state_dir
-        self._config = MockCMDStateConfig(
-            Path(self._state_dir, self.CONFIG_FILE_NAME))
+        if state_dir.is_dir():
+            state_path = Path(state_dir, self.CONFIG_FILE_NAME)
+        else:
+            state_path = state_dir
+        self._state_path = state_path
+        self._config = MockCMDStateConfig(Path(self._state_path))
 
     def response_directory_path(self) -> str:
         return self._config.response_directory
 
     def iterate_config(self):
         self._config.iterate()
```

### Comparing `mock-cli-framework-0.5.0/mock_cli/path.py` & `mock-cli-framework-0.5.1/mock_cli/path.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/mock_cli/responses.py` & `mock-cli-framework-0.5.1/mock_cli/responses.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.5.0/mock_cli_framework.egg-info/PKG-INFO` & `mock-cli-framework-0.5.1/mock_cli_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.5.0
+Version: 0.5.1
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mock-cli-framework-0.5.0/setup.py` & `mock-cli-framework-0.5.1/setup.py`

 * *Files identical despite different names*

