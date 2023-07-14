# Comparing `tmp/fun_sentence_splitter-0.1.344.post1.tar.gz` & `tmp/fun_sentence_splitter-0.2.344.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_sentence_splitter-0.1.344.post1.tar", max compression
+gzip compressed data, was "fun_sentence_splitter-0.2.344.tar", max compression
```

## Comparing `fun_sentence_splitter-0.1.344.post1.tar` & `fun_sentence_splitter-0.2.344.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-07-06 14:05:01.586905 fun_sentence_splitter-0.1.344.post1/LICENSE
--rw-r--r--   0        0        0      376 2023-07-06 14:05:01.586905 fun_sentence_splitter-0.1.344.post1/README.md
--rw-r--r--   0        0        0       57 2023-07-06 14:05:01.586905 fun_sentence_splitter-0.1.344.post1/fun_sentence_splitter/__init__.py
--rw-r--r--   0        0        0     2405 2023-07-06 14:05:01.586905 fun_sentence_splitter-0.1.344.post1/fun_sentence_splitter/sentence_splitter.py
--rw-r--r--   0        0        0     1151 2023-07-06 14:05:01.590905 fun_sentence_splitter-0.1.344.post1/pyproject.toml
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 fun_sentence_splitter-0.1.344.post1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/LICENSE
+-rw-r--r--   0        0        0     1247 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/README.md
+-rw-r--r--   0        0        0       57 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/fun_sentence_splitter/__init__.py
+-rw-r--r--   0        0        0     3383 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/fun_sentence_splitter/sentence_splitter.py
+-rw-r--r--   0        0        0     1423 2023-07-14 08:44:10.055927 fun_sentence_splitter-0.2.344/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 fun_sentence_splitter-0.2.344/PKG-INFO
```

### Comparing `fun_sentence_splitter-0.1.344.post1/LICENSE` & `fun_sentence_splitter-0.2.344/LICENSE`

 * *Files identical despite different names*

### Comparing `fun_sentence_splitter-0.1.344.post1/pyproject.toml` & `fun_sentence_splitter-0.2.344/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "fun-sentence-splitter"
-version = "0.1.344.post1"
+version = "0.2.344"
 description = "A fundamental sentence splitter based on spacy."
 authors = ["Medical AI Engineering <engineering@m-ai.rhenus.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "fun_sentence_splitter" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 spacy = "3.4.4"
 
-
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.277"
 mypy = "^1.4.1"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
+typer = "~0.7"  # used for evaluation, version restricted by spacy
+types-tqdm = "^4.65.0.1"
 
 [tool.mypy]
 pretty = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 
@@ -41,15 +42,23 @@
     "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI",
     "RET", "RSE", "RUF", "SIM", "SLF",
     "TCH", "TID", "TRY",
     "UP",
     "YTT",
 ]
 
+ignore = [
+    "EM101",  # string literals in exceptions
+    "TRY003",  # custom messages for internal exceptions
+]
+
 [tool.ruff.per-file-ignores]
 "tests/*" = [
     "S101", # allow assertions
 ]
+"tests/evaluate_sentence_splitter.py" = [
+    "T201", # allow print
+]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

