# Comparing `tmp/kaar_gpt-0.0.1.tar.gz` & `tmp/kaar_gpt-0.1.0.tar.gz`

## Comparing `kaar_gpt-0.0.1.tar` & `kaar_gpt-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/Makefile
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/src/gpt/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/src/gpt/openai/__init__.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/src/gpt/openai/chat_completion.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/.gitignore
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/README.md
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 kaar_gpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/Makefile
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/src/gpt/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/src/gpt/openai/__init__.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/src/gpt/openai/chat_completion.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/.gitignore
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/README.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 kaar_gpt-0.1.0/PKG-INFO
```

### Comparing `kaar_gpt-0.0.1/src/gpt/openai/chat_completion.py` & `kaar_gpt-0.1.0/src/gpt/openai/chat_completion.py`

 * *Files identical despite different names*

### Comparing `kaar_gpt-0.0.1/pyproject.toml` & `kaar_gpt-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaar_gpt-0.0.1/PKG-INFO` & `kaar_gpt-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: kaar-gpt
-Version: 0.0.1
+Version: 0.1.0
 Summary: OpenAI API wrapper
 Project-URL: Documentation, https://github.com/kaar/gpt#readme
 Project-URL: Issues, https://github.com/kaar/gpt/issues
 Project-URL: Source, https://github.com/kaar/gpt
 Author-email: Caspar Nettelbladt <caspar.n@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
-# LLM Base
+# GPT
 
-## Install
-```
-pip install llm-base
+## Getting Started
+
+### Installation
+
+Kaar GPT is available as [`kaar-gpt`](https://pypi.org/project/kaar-gpt/) on PyPI:
+```bash
+pip install kaar-gpt
 ```
 
 ## Usage
 ```python
-from llm_base import openai
-from llm_base.openai import ...
+from gpt.openai import ChatCompletion, ChatCompletionRequest, ChatMessage
 ```
```

