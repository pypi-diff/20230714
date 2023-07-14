# Comparing `tmp/ramjam-0.3.0.tar.gz` & `tmp/ramjam-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramjam-0.3.0.tar", last modified: Thu Jul 13 14:29:08 2023, max compression
+gzip compressed data, was "ramjam-0.4.0.tar", last modified: Fri Jul 14 11:32:51 2023, max compression
```

## Comparing `ramjam-0.3.0.tar` & `ramjam-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:29:08.083892 ramjam-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-13 14:29:08.079892 ramjam-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-13 14:29:06.000000 ramjam-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-13 14:29:06.000000 ramjam-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:29:08.079892 ramjam-0.3.0/ramjam/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 14:29:06.000000 ramjam-0.3.0/ramjam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 14:28:40.000000 ramjam-0.3.0/ramjam/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-13 14:28:40.000000 ramjam-0.3.0/ramjam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:29:08.079892 ramjam-0.3.0/ramjam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-13 14:29:08.000000 ramjam-0.3.0/ramjam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 14:29:08.000000 ramjam-0.3.0/ramjam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:29:08.000000 ramjam-0.3.0/ramjam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 14:29:08.000000 ramjam-0.3.0/ramjam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 14:29:08.000000 ramjam-0.3.0/ramjam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:29:08.083892 ramjam-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 14:28:40.000000 ramjam-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:29:08.079892 ramjam-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-13 14:28:40.000000 ramjam-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 14:28:40.000000 ramjam-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:51.124346 ramjam-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 11:32:51.124346 ramjam-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 11:32:49.000000 ramjam-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-14 11:32:49.000000 ramjam-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:51.124346 ramjam-0.4.0/ramjam/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 11:32:49.000000 ramjam-0.4.0/ramjam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-14 11:32:23.000000 ramjam-0.4.0/ramjam/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-14 11:32:23.000000 ramjam-0.4.0/ramjam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:51.124346 ramjam-0.4.0/ramjam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 11:32:51.000000 ramjam-0.4.0/ramjam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 11:32:51.000000 ramjam-0.4.0/ramjam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:32:51.000000 ramjam-0.4.0/ramjam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 11:32:51.000000 ramjam-0.4.0/ramjam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 11:32:51.000000 ramjam-0.4.0/ramjam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:32:51.124346 ramjam-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 11:32:23.000000 ramjam-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:51.124346 ramjam-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-14 11:32:23.000000 ramjam-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 11:32:23.000000 ramjam-0.4.0/tests/test_utils.py
```

### Comparing `ramjam-0.3.0/pyproject.toml` & `ramjam-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramjam"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `ramjam-0.3.0/ramjam/utils.py` & `ramjam-0.4.0/ramjam/utils.py`

 * *Files identical despite different names*

### Comparing `ramjam-0.3.0/tests/test_cli.py` & `ramjam-0.4.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     assert MyCommand.method() == "mycommand"
 
 
 def test_call():
     class MyCommand(Command):
         pass
 
-    with pytest.raises(TypeError):
-        MyCommand(Namespace())  # Cannot instantiate abstract class
+    command_instance = MyCommand(Namespace())
+
+    with pytest.raises(NotImplementedError):
+        command_instance()  # Call the command instance, it should raise NotImplementedError
 
 
 def test_args():
     class MyCommand(Command):
         args = {"--foo": {"help": "Foo help"}}
 
     assert MyCommand.args == {"--foo": {"help": "Foo help"}}
@@ -28,14 +30,24 @@
 def test_help():
     class MyCommand(Command):
         help = "Some help"
 
     assert MyCommand.help == "Some help"
 
 
+def test_multiple_inheritance():
+    class MyCommand(Command):
+        args = {"--foo": {"help": "Foo help"}}
+
+    class MyOtherCommand(MyCommand):
+        args = {"--bar": {"help": "Bar help"}}
+
+    assert MyOtherCommand.args == {"--foo": {"help": "Foo help"}, "--bar": {"help": "Bar help"}}
+
+
 def test_cli():
     class MyCommand(Command):
         args = {"--foo": {"help": "Foo help"}}
         help = "Some help"
 
         def __call__(self) -> None:
             pass
```

