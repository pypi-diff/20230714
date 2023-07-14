# Comparing `tmp/together-0.0.1.tar.gz` & `tmp/together-0.0.6.tar.gz`

## Comparing `together-0.0.1.tar` & `together-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,19 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.1/src/together/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.1/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 together-0.0.1/README.md
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 together-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 together-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.0.6/.github/workflows/check_code_quality.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 together-0.0.6/src/together/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 together-0.0.6/src/together/api.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 together-0.0.6/src/together/files.py
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 together-0.0.6/src/together/finetune.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 together-0.0.6/src/together/inference.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 together-0.0.6/src/together/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.6/src/together/cli/__init__.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 together-0.0.6/src/together/cli/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/api.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/files.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/finetune.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/inference.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.6/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 together-0.0.6/README.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 together-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 together-0.0.6/PKG-INFO
```

### Comparing `together-0.0.1/.gitignore` & `together-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `together-0.0.1/LICENSE` & `together-0.0.6/LICENSE`

 * *Files identical despite different names*

