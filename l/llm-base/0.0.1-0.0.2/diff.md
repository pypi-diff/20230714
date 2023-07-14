# Comparing `tmp/llm-base-0.0.1.tar.gz` & `tmp/llm-base-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-base-0.0.1.tar", last modified: Thu Jul 13 23:17:34 2023, max compression
+gzip compressed data, was "llm-base-0.0.2.tar", last modified: Fri Jul 14 00:15:55 2023, max compression
```

## Comparing `llm-base-0.0.1.tar` & `llm-base-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-13 23:17:34.682342 llm-base-0.0.1/
--rw-r--r--   0 tibber    (1001) tibber    (1002)      540 2023-07-13 23:17:34.682342 llm-base-0.0.1/PKG-INFO
--rw-r--r--   0 tibber    (1001) tibber    (1002)       11 2023-07-13 22:24:26.000000 llm-base-0.0.1/README.md
-drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-13 23:17:34.679008 llm-base-0.0.1/gpt/
--rw-r--r--   0 tibber    (1001) tibber    (1002)        0 2023-07-13 22:37:53.000000 llm-base-0.0.1/gpt/__init__.py
-drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-13 23:17:34.682342 llm-base-0.0.1/gpt/openai/
--rw-r--r--   0 tibber    (1001) tibber    (1002)      304 2023-07-13 21:25:19.000000 llm-base-0.0.1/gpt/openai/__init__.py
--rw-r--r--   0 tibber    (1001) tibber    (1002)     8574 2023-07-13 21:25:19.000000 llm-base-0.0.1/gpt/openai/chat_completion.py
-drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-13 23:17:34.682342 llm-base-0.0.1/llm_base.egg-info/
--rw-r--r--   0 tibber    (1001) tibber    (1002)      540 2023-07-13 23:17:34.000000 llm-base-0.0.1/llm_base.egg-info/PKG-INFO
--rw-r--r--   0 tibber    (1001) tibber    (1002)      221 2023-07-13 23:17:34.000000 llm-base-0.0.1/llm_base.egg-info/SOURCES.txt
--rw-r--r--   0 tibber    (1001) tibber    (1002)        1 2023-07-13 23:17:34.000000 llm-base-0.0.1/llm_base.egg-info/dependency_links.txt
--rw-r--r--   0 tibber    (1001) tibber    (1002)        4 2023-07-13 23:17:34.000000 llm-base-0.0.1/llm_base.egg-info/top_level.txt
--rw-r--r--   0 tibber    (1001) tibber    (1002)      702 2023-07-13 23:17:25.000000 llm-base-0.0.1/pyproject.toml
--rw-r--r--   0 tibber    (1001) tibber    (1002)       38 2023-07-13 23:17:34.682342 llm-base-0.0.1/setup.cfg
+drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-14 00:15:55.871186 llm-base-0.0.2/
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      665 2023-07-14 00:15:55.871186 llm-base-0.0.2/PKG-INFO
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      136 2023-07-13 23:23:29.000000 llm-base-0.0.2/README.md
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      733 2023-07-14 00:14:59.000000 llm-base-0.0.2/pyproject.toml
+-rw-r--r--   0 tibber    (1001) tibber    (1002)       38 2023-07-14 00:15:55.871186 llm-base-0.0.2/setup.cfg
+drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-14 00:15:55.871186 llm-base-0.0.2/src/
+drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-14 00:15:55.871186 llm-base-0.0.2/src/gpt/
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      311 2023-07-14 00:10:40.000000 llm-base-0.0.2/src/gpt/__init__.py
+drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-14 00:15:55.871186 llm-base-0.0.2/src/gpt/openai/
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      304 2023-07-13 21:25:19.000000 llm-base-0.0.2/src/gpt/openai/__init__.py
+-rw-r--r--   0 tibber    (1001) tibber    (1002)     8574 2023-07-13 21:25:19.000000 llm-base-0.0.2/src/gpt/openai/chat_completion.py
+drwxr-xr-x   0 tibber    (1001) tibber    (1002)        0 2023-07-14 00:15:55.871186 llm-base-0.0.2/src/llm_base.egg-info/
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      665 2023-07-14 00:15:55.000000 llm-base-0.0.2/src/llm_base.egg-info/PKG-INFO
+-rw-r--r--   0 tibber    (1001) tibber    (1002)      284 2023-07-14 00:15:55.000000 llm-base-0.0.2/src/llm_base.egg-info/SOURCES.txt
+-rw-r--r--   0 tibber    (1001) tibber    (1002)        1 2023-07-14 00:15:55.000000 llm-base-0.0.2/src/llm_base.egg-info/dependency_links.txt
+-rw-r--r--   0 tibber    (1001) tibber    (1002)        9 2023-07-14 00:15:55.000000 llm-base-0.0.2/src/llm_base.egg-info/requires.txt
+-rw-r--r--   0 tibber    (1001) tibber    (1002)        4 2023-07-14 00:15:55.000000 llm-base-0.0.2/src/llm_base.egg-info/top_level.txt
```

### Comparing `llm-base-0.0.1/gpt/openai/chat_completion.py` & `llm-base-0.0.2/src/gpt/openai/chat_completion.py`

 * *Files identical despite different names*

### Comparing `llm-base-0.0.1/pyproject.toml` & `llm-base-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-base"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Caspar Nettelbladt", email="caspar.n@gmail.com" },
 ]
-description = "GPT Base"
+description = "LLM Base"
 readme = "README.md"
 requires-python = ">=3.7"
+dependencies=[
+  "requests",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 # [project.entry_points]
 # console_scripts = [
 #     "gpt-chat = chat:main",
 # ]
 
 [project.urls]
-"Homepage" = "https://github.com/kaar/gpt-base"
-"Bug Tracker" = "https://github.com/kaar/gpt-base/issues"
+"Homepage" = "https://github.com/kaar/llm-base"
+"Bug Tracker" = "https://github.com/kaar/llm-base/issues"
```

