# Comparing `tmp/kaar_gpt_tools-0.1.0.tar.gz` & `tmp/kaar_gpt_tools-0.2.0.tar.gz`

## Comparing `kaar_gpt_tools-0.1.0.tar` & `kaar_gpt_tools-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/Makefile
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/Pipfile
--rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/src/gpt_tools/__init__.py
--rwxr-xr-x   0        0        0     4029 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/src/gpt_tools/chat.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/.gitignore
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/README.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/Makefile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/src/gpt_tools/__init__.py
+-rwxr-xr-x   0        0        0     4029 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/src/gpt_tools/chat.py
+-rwxr-xr-x   0        0        0     5257 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/src/gpt_tools/git.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/.gitignore
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/README.md
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.2.0/PKG-INFO
```

### Comparing `kaar_gpt_tools-0.1.0/src/gpt_tools/chat.py` & `kaar_gpt_tools-0.2.0/src/gpt_tools/chat.py`

 * *Files identical despite different names*

### Comparing `kaar_gpt_tools-0.1.0/pyproject.toml` & `kaar_gpt_tools-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 [project.urls]
 Documentation = "https://github.com/kaar/gpt-tools#readme"
 Issues = "https://github.com/kaar/gpt-tools/issues"
 Source = "https://github.com/kaar/gpt-tools"
 
 [project.scripts]
 gpt-chat = "gpt_tools.chat:main"
+gpt-git = "gpt_tools.git:main"
 
 [tool.hatch.version]
 path = "src/gpt_tools/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
```

### Comparing `kaar_gpt_tools-0.1.0/PKG-INFO` & `kaar_gpt_tools-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaar-gpt-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: GPT Tools
 Project-URL: Documentation, https://github.com/kaar/gpt-tools#readme
 Project-URL: Issues, https://github.com/kaar/gpt-tools/issues
 Project-URL: Source, https://github.com/kaar/gpt-tools
 Author-email: Caspar Nettelbladt <caspar.n@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
```

