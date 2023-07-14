# Comparing `tmp/qalita-1.0.1.tar.gz` & `tmp/qalita-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.1.tar", max compression
+gzip compressed data, was "qalita-1.0.3.tar", max compression
```

## Comparing `qalita-1.0.1.tar` & `qalita-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-13 21:38:07.871172 qalita-1.0.1/LICENSE
--rw-r--r--   0        0        0      416 2023-07-13 21:38:07.871172 qalita-1.0.1/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-13 21:38:19.649227 qalita-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 21:38:07.895172 qalita-1.0.1/qalita/__init__.py
--rw-r--r--   0        0        0     4660 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-13 21:38:07.895172 qalita-1.0.1/qalita/commands/__init__.py
--rw-r--r--   0        0        0    18014 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/commands/agent.py
--rw-r--r--   0        0        0    14225 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/commands/pack.py
--rw-r--r--   0        0        0     9429 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-13 21:38:07.895172 qalita-1.0.1/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-13 21:38:07.872172 qalita-1.0.1/qalita/internal/utils.py
--rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 qalita-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-13 21:53:15.774850 qalita-1.0.3/LICENSE
+-rw-r--r--   0        0        0      416 2023-07-13 21:53:15.774850 qalita-1.0.3/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-13 21:53:26.294807 qalita-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 21:53:15.799849 qalita-1.0.3/qalita/__init__.py
+-rw-r--r--   0        0        0     4149 2023-07-13 21:53:26.295807 qalita-1.0.3/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:53:15.799849 qalita-1.0.3/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    18014 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14225 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9429 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:53:15.799849 qalita-1.0.3/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/internal/utils.py
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 qalita-1.0.3/PKG-INFO
```

### Comparing `qalita-1.0.1/LICENSE` & `qalita-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.1/pyproject.toml` & `qalita-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.1"
+version = "1.0.3"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `qalita-1.0.1/qalita/cli.py` & `qalita-1.0.3/qalita/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -100,40 +100,22 @@
     ----------------------------------------------------------------------------\n\r
     Please, Help us improve our service by reporting any bug by filing a bug report, Thanks ! \n\r
     mail : contact-project+qalita-platform-toolset-cli-bug@incoming.gitlab.com \n\r
     ----------------------------------------------------------------------------"""
     pass
 
 
-def fetch_package_version(filename):
-    """
-    Fetch the version from the package.
-    """
-    # Open the file
-    with open(filename, 'r') as f:
-        data = json.load(f)
-
-    # Retrieve the version
-    version = data.get('version', 'Version not found')
-
-    return version
-
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @pass_config
 def version(config):
     """
     Display the version of the cli
     """
     logger.info("------------- QALITA CLI Version -------------")
-
-    # Assuming that your json file is named 'version.json' and located in the same directory as this file
-    file_path = os.path.join(os.path.dirname(__file__), 'version.json')
-    version = fetch_package_version(file_path)
-
-    logger.info(f"Version : {version}")
+    logger.info(f"Version : 1.0.3")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.1/qalita/commands/agent.py` & `qalita-1.0.3/qalita/commands/agent.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.1/qalita/commands/pack.py` & `qalita-1.0.3/qalita/commands/pack.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.1/qalita/commands/source.py` & `qalita-1.0.3/qalita/commands/source.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.1/qalita/internal/logger.py` & `qalita-1.0.3/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.1/qalita/internal/utils.py` & `qalita-1.0.3/qalita/internal/utils.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.1/PKG-INFO` & `qalita-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qalita
-Version: 1.0.1
+Version: 1.0.3
 Summary: Qalita Command Line Interface
 Author: Armand LEOPOLD
 Author-email: armand.leopold@qalita.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

