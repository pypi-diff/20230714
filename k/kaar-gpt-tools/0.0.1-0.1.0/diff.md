# Comparing `tmp/kaar_gpt_tools-0.0.1.tar.gz` & `tmp/kaar_gpt_tools-0.1.0.tar.gz`

## Comparing `kaar_gpt_tools-0.0.1.tar` & `kaar_gpt_tools-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/Makefile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/src/gpt_tools/__init__.py
--rwxr-xr-x   0        0        0     4034 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/src/gpt_tools/chat.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/.gitignore
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/README.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/Makefile
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/Pipfile
+-rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/Pipfile.lock
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/src/gpt_tools/__init__.py
+-rwxr-xr-x   0        0        0     4029 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/src/gpt_tools/chat.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/.gitignore
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/README.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 kaar_gpt_tools-0.1.0/PKG-INFO
```

### Comparing `kaar_gpt_tools-0.0.1/src/gpt_tools/chat.py` & `kaar_gpt_tools-0.1.0/src/gpt_tools/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import argparse
 import logging
 import os
 import sys
 
-from llm_base.openai import ChatCompletion, ChatCompletionRequest, ChatMessage
+from gpt.openai import ChatCompletion, ChatCompletionRequest, ChatMessage
 
 LOG = logging.getLogger(__name__)
 DEFAULT_LOG_LEVEL = logging.INFO
 
 DEFAULT_USER = "gpt-cli"
 OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY")
 MODELS = ["gpt-3.5-turbo", "gpt-4"]
```

### Comparing `kaar_gpt_tools-0.0.1/pyproject.toml` & `kaar_gpt_tools-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   { name="Caspar Nettelbladt", email="caspar.n@gmail.com" },
 ]
 description = "GPT Tools"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 dependencies=[
-  "llm_base",
+  "kaar-gpt",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
```

### Comparing `kaar_gpt_tools-0.0.1/PKG-INFO` & `kaar_gpt_tools-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: kaar-gpt-tools
-Version: 0.0.1
+Version: 0.1.0
 Summary: GPT Tools
 Project-URL: Documentation, https://github.com/kaar/gpt-tools#readme
 Project-URL: Issues, https://github.com/kaar/gpt-tools/issues
 Project-URL: Source, https://github.com/kaar/gpt-tools
 Author-email: Caspar Nettelbladt <caspar.n@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: llm-base
+Requires-Dist: kaar-gpt
 Description-Content-Type: text/markdown
 
 # GPT Tools
```

