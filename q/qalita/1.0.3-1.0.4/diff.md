# Comparing `tmp/qalita-1.0.3.tar.gz` & `tmp/qalita-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.3.tar", max compression
+gzip compressed data, was "qalita-1.0.4.tar", max compression
```

## Comparing `qalita-1.0.3.tar` & `qalita-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-13 21:53:15.774850 qalita-1.0.3/LICENSE
--rw-r--r--   0        0        0      416 2023-07-13 21:53:15.774850 qalita-1.0.3/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-13 21:53:26.294807 qalita-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 21:53:15.799849 qalita-1.0.3/qalita/__init__.py
--rw-r--r--   0        0        0     4149 2023-07-13 21:53:26.295807 qalita-1.0.3/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-13 21:53:15.799849 qalita-1.0.3/qalita/commands/__init__.py
--rw-r--r--   0        0        0    18014 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/commands/agent.py
--rw-r--r--   0        0        0    14225 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/commands/pack.py
--rw-r--r--   0        0        0     9429 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-13 21:53:15.799849 qalita-1.0.3/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-13 21:53:15.775849 qalita-1.0.3/qalita/internal/utils.py
--rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 qalita-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-14 13:24:05.512130 qalita-1.0.4/LICENSE
+-rw-r--r--   0        0        0      416 2023-07-14 13:24:05.513130 qalita-1.0.4/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-14 13:24:15.851944 qalita-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 13:24:05.535129 qalita-1.0.4/qalita/__init__.py
+-rw-r--r--   0        0        0     4189 2023-07-14 13:24:15.852944 qalita-1.0.4/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:24:05.536130 qalita-1.0.4/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    18014 2023-07-14 13:24:05.513130 qalita-1.0.4/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14225 2023-07-14 13:24:05.513130 qalita-1.0.4/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9526 2023-07-14 13:24:05.513130 qalita-1.0.4/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:24:05.536130 qalita-1.0.4/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-14 13:24:05.514130 qalita-1.0.4/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-14 13:24:05.514130 qalita-1.0.4/qalita/internal/utils.py
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 qalita-1.0.4/PKG-INFO
```

### Comparing `qalita-1.0.3/LICENSE` & `qalita-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.3/pyproject.toml` & `qalita-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.3"
+version = "1.0.4"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `qalita-1.0.3/qalita/cli.py` & `qalita-1.0.4/qalita/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,18 @@
     def save_source_config(self):
         with open("qalita-conf.yaml", "w") as file:
             yaml.dump(self.config, file)
 
     def load_source_config(self):
         try:
             with open("qalita-conf.yaml", "r") as file:
-                return yaml.safe_load(file)
+                self.config = yaml.safe_load(file)
+                return self.config
         except FileNotFoundError:
-            logger.warning("Configuration file not found, creating a new one.")
+            logger.warning("Configuration file [qalita-conf.yaml] not found, creating a new one.")
             self.config = {"version": 1, "sources": []}
             self.save_source_config()
             return self.config
         except Exception as e:
             logger.warning(
                 f"An unexpected error occurred while loading the configuration: {e}"
             )
@@ -80,15 +81,15 @@
     def __init__(self):
         self.name = ""
         self.mode = ""
         self.token = ""
         self.url = ""
         self.verbose = False
         self.agent_id = None
-        self.config = self.load_source_config()
+        self.config = None
 
         # con = sqlite3.connect("agent.db")
 
 
 pass_config = click.make_pass_decorator(Config, ensure=True)
 
 
@@ -107,15 +108,15 @@
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @pass_config
 def version(config):
     """
     Display the version of the cli
     """
     logger.info("------------- QALITA CLI Version -------------")
-    logger.info(f"Version : 1.0.3")
+    logger.info(f"Version : 1.0.4")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.3/qalita/commands/agent.py` & `qalita-1.0.4/qalita/commands/agent.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.3/qalita/commands/pack.py` & `qalita-1.0.4/qalita/commands/pack.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.3/qalita/commands/source.py` & `qalita-1.0.4/qalita/commands/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     logger.warning("Not Yet Implemented")
 
 
 @source.command()
 @pass_config
 def list(config):
     """List sources that are accessible to the agent"""
+    config.load_source_config()
 
     sources = []
     headers = ["ID", "Name", "Type", "Description", "Validity"]
+
     for source in config.config["sources"]:
         sources.append(
             [
                 source.get("id", ""),
                 source.get("name", ""),
                 source.get("type", ""),
                 source.get("description", ""),
@@ -48,14 +50,15 @@
     print(tabulate(sources, headers, tablefmt="simple"))
 
 
 @pass_config
 def validate_source(config):
     """Validate a source configuration"""
     logger.info("------------- Source Validation -------------")
+    config.load_source_config()
     agent_conf = config.load_agent_config()
 
     total_sources = 0
     error_count = 0
 
     source_names = []
 
@@ -149,14 +152,15 @@
 def push(config):
     """Publish a source to the Qalita Platform"""
     validate_source()
     logger.info("------------- Source Publishing -------------")
     logger.info("Publishing sources to the Qalita Platform...")
     invalid_count = 0  # to count failed publishing sources
     agent_conf = config.load_agent_config()
+    config.load_source_config()
 
     for i, source in enumerate(config.config["sources"]):
         if source["validate"] == "valid":
             owner_id = agent_conf["user"]["id"]
             if "id" in source:
                 # Try to get source info from name, type and owner_id
                 r = send_api_request(
```

### Comparing `qalita-1.0.3/qalita/internal/logger.py` & `qalita-1.0.4/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.3/qalita/internal/utils.py` & `qalita-1.0.4/qalita/internal/utils.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.3/PKG-INFO` & `qalita-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qalita
-Version: 1.0.3
+Version: 1.0.4
 Summary: Qalita Command Line Interface
 Author: Armand LEOPOLD
 Author-email: armand.leopold@qalita.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

