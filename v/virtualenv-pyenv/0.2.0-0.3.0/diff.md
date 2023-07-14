# Comparing `tmp/virtualenv-pyenv-0.2.0.tar.gz` & `tmp/virtualenv_pyenv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualenv-pyenv-0.2.0.tar", max compression
+gzip compressed data, was "virtualenv_pyenv-0.3.0.tar", max compression
```

## Comparing `virtualenv-pyenv-0.2.0.tar` & `virtualenv_pyenv-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1093 2022-04-06 09:44:57.674622 virtualenv-pyenv-0.2.0/LICENSE
--rw-r--r--   0        0        0     1022 2021-12-09 12:39:11.284056 virtualenv-pyenv-0.2.0/README.md
--rw-r--r--   0        0        0     1524 2022-04-06 09:44:30.794382 virtualenv-pyenv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-04-06 09:44:23.306316 virtualenv-pyenv-0.2.0/src/_virtualenv_pyenv/__init__.py
--rw-r--r--   0        0        0     1977 2022-04-06 09:31:48.354475 virtualenv-pyenv-0.2.0/src/_virtualenv_pyenv/discovery.py
--rw-r--r--   0        0        0     1948 2022-04-06 09:45:44.915578 virtualenv-pyenv-0.2.0/setup.py
--rw-r--r--   0        0        0     2007 2022-04-06 09:45:44.915732 virtualenv-pyenv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-14 09:50:32.674448 virtualenv_pyenv-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3964 2023-07-13 14:26:07.450787 virtualenv_pyenv-0.3.0/README.md
+-rw-r--r--   0        0        0     1555 2023-07-13 14:58:13.210574 virtualenv_pyenv-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-13 14:58:20.454688 virtualenv_pyenv-0.3.0/src/_virtualenv_pyenv/__init__.py
+-rw-r--r--   0        0        0     4669 2023-07-10 10:33:32.312416 virtualenv_pyenv-0.3.0/src/_virtualenv_pyenv/discovery.py
+-rw-r--r--   0        0        0     5021 1970-01-01 00:00:00.000000 virtualenv_pyenv-0.3.0/PKG-INFO
```

### Comparing `virtualenv-pyenv-0.2.0/LICENSE` & `virtualenv_pyenv-0.3.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021, 2022 un.def <me@undef.im>
+Copyright (c) 2021, 2022, 2023 un.def <me@undef.im>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `virtualenv-pyenv-0.2.0/pyproject.toml` & `virtualenv_pyenv-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'virtualenv-pyenv'
-version = '0.2.0'
-description = 'A virtualenv Python discovery plugin using pyenv'
+version = '0.3.0'
+description = 'A virtualenv Python discovery plugin for pyenv-installed interpreters'
 license = 'MIT'
 authors = ['un.def <me@undef.im>']
 readme = 'README.md'
 homepage = 'https://github.com/un-def/virtualenv-pyenv'
 repository = 'https://github.com/un-def/virtualenv-pyenv'
 keywords = ['virtualenv', 'pyenv']
 classifiers = [
@@ -23,15 +23,15 @@
 
 [tool.poetry.plugins.'virtualenv.discovery']
 pyenv = '_virtualenv_pyenv.discovery:Pyenv'
 
 [tool.poetry.dependencies]
 python = '^3.7'
 virtualenv = '*'
-pyenv-inspect = '~0.2'
+pyenv-inspect = '^0.2'
 
 [tool.isort]
 lines_after_imports = 2
 multi_line_output = 5
 include_trailing_comma = true
 use_parentheses = true
 known_first_party = ['_virtualenv_pyenv']
@@ -45,14 +45,15 @@
 legacy_tox_ini = '''
 [tox]
 envlist =
     py37
     py38
     py39
     py310
+    py311
     flake8
     isort
 isolated_build = true
 
 [testenv]
 deps =
     pytest
```

