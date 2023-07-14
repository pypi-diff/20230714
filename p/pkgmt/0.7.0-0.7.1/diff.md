# Comparing `tmp/pkgmt-0.7.0.tar.gz` & `tmp/pkgmt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgmt-0.7.0.tar", last modified: Tue Jul 11 18:27:35 2023, max compression
+gzip compressed data, was "pkgmt-0.7.1.tar", last modified: Fri Jul 14 14:44:54 2023, max compression
```

## Comparing `pkgmt-0.7.0.tar` & `pkgmt-0.7.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-11 18:27:17.000000 pkgmt-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-11 18:27:17.000000 pkgmt-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-11 18:27:17.000000 pkgmt-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 18:27:35.757430 pkgmt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-11 18:27:17.000000 pkgmt-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-11 18:27:17.000000 pkgmt-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 18:27:35.757430 pkgmt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-11 18:27:17.000000 pkgmt-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.749429 pkgmt-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/assets/template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt/assets/template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/assets/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.749429 pkgmt-0.7.0/src/pkgmt/assets/template/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/assets/template/src/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/src/package_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/assets/template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/assets/template/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/fail_if_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/fail_if_not_modified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.757430 pkgmt-0.7.0/src/pkgmt/versioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioner/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-11 18:27:17.000000 pkgmt-0.7.0/src/pkgmt/versioner/versioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:27:35.753430 pkgmt-0.7.0/src/pkgmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 18:27:35.000000 pkgmt-0.7.0/src/pkgmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-07-14 14:44:38.000000 pkgmt-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 14:44:38.000000 pkgmt-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-14 14:44:38.000000 pkgmt-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-14 14:44:54.720089 pkgmt-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 14:44:38.000000 pkgmt-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 14:44:38.000000 pkgmt-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 14:44:54.720089 pkgmt-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-14 14:44:38.000000 pkgmt-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.712089 pkgmt-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.716089 pkgmt-0.7.1/src/pkgmt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.716089 pkgmt-0.7.1/src/pkgmt/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.712089 pkgmt-0.7.1/src/pkgmt/assets/template/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/src/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/src/package_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/assets/template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/assets/template/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/fail_if_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/fail_if_not_modified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.720089 pkgmt-0.7.1/src/pkgmt/versioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioner/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-14 14:44:38.000000 pkgmt-0.7.1/src/pkgmt/versioner/versioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:44:54.716089 pkgmt-0.7.1/src/pkgmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 14:44:54.000000 pkgmt-0.7.1/src/pkgmt.egg-info/top_level.txt
```

### Comparing `pkgmt-0.7.0/CHANGELOG.md` & `pkgmt-0.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # CHANGELOG
 
+## 0.7.1 (2023-07-14)
+
+* [Fix] Fixed `black` `--extend-exclude` override in `pyproject.toml`([#66](https://github.com/ploomber/pkgmt/issues/66))
+
 ## 0.7.0 (2023-07-11)
 
 * [API Change] Support for projects containing `version` key in `pyproject.toml`. ([#58](https://github.com/ploomber/pkgmt/issues/58))
 * [Fix] Fix bug when running git hook
+* [Fix] Proper error message when version file is empty, or version string not found. Display version file location when inconsistent version in changelog ([#64](https://github.com/ploomber/pkgmt/issues/64))
 
 ## 0.6.2 (2023-06-30)
 
 * [Feature] Added file path to `pkgmt lint` ([#56](https://github.com/ploomber/pkgmt/issues/56))
 * [Feature] Clearer error when missing `pyproject.toml`
 * [Feature] Added `--exclude` option to pkgmt `lint` and pkgmt `format` ([#55](https://github.com/ploomber/pkgmt/issues/55))
```

### Comparing `pkgmt-0.7.0/LICENSE` & `pkgmt-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/README.md` & `pkgmt-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/setup.py` & `pkgmt-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/.github/pull_request_template.md` & `pkgmt-0.7.1/src/pkgmt/assets/template/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/.github/workflows/ci.yml` & `pkgmt-0.7.1/src/pkgmt/assets/template/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/.gitignore` & `pkgmt-0.7.1/src/pkgmt/assets/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/pyproject.toml` & `pkgmt-0.7.1/src/pkgmt/assets/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/setup.py` & `pkgmt-0.7.1/src/pkgmt/assets/template/setup.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/tasks.py` & `pkgmt-0.7.1/src/pkgmt/assets/template/tasks.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/assets/template/tests/conftest.py` & `pkgmt-0.7.1/src/pkgmt/assets/template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/changelog.py` & `pkgmt-0.7.1/src/pkgmt/changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 
         markdown = mistune.Markdown(
             renderer=None, inline=CustomInlineParser(hard_wrap=False), plugins=None
         )
         self.tree = markdown(text)
 
         versioner = Versioner(project_root=project_root)
+        self.version_file = versioner.get_version_file_path()
         self.current = versioner.current_version()
 
     @classmethod
     def from_path(cls, path, project_root="."):
         return cls(text=Path(path).read_text(), project_root=project_root)
 
     def sort_last_section(self):
@@ -286,15 +287,15 @@
 
         if (date_match and date_match.group(1) != self.current) or (
             date_match is None and subheading != self.current
         ):
             raise ProjectValidationError(
                 "[Inconsistent version] Version in  top section in "
                 f"CHANGELOG is {subheading!r}, "
-                f"but version in __init__.py is {self.current!r}, "
+                f"but version in {self.version_file} is {self.current!r}, "
                 "fix them so they match"
             )
 
     def check(self, *, verbose=False):
         """Runs all checks"""
         errors = []
```

### Comparing `pkgmt-0.7.0/src/pkgmt/cli.py` & `pkgmt-0.7.1/src/pkgmt/cli.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/config.py` & `pkgmt-0.7.1/src/pkgmt/config.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/dependencies.py` & `pkgmt-0.7.1/src/pkgmt/dependencies.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/deprecation.py` & `pkgmt-0.7.1/src/pkgmt/deprecation.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/dev.py` & `pkgmt-0.7.1/src/pkgmt/dev.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/fail_if_modified.py` & `pkgmt-0.7.1/src/pkgmt/fail_if_modified.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/fail_if_not_modified.py` & `pkgmt-0.7.1/src/pkgmt/fail_if_not_modified.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/formatting.py` & `pkgmt-0.7.1/src/pkgmt/formatting.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 
 
 def format(exclude):
     current = find_root()
 
     exclude_str = "|".join(exclude)
 
-    cmd = ["black", ".", "--extend-exclude", exclude_str]
+    if exclude_str:
+        cmd = ["black", ".", "--extend-exclude", exclude_str]
+    else:
+        cmd = ["black", "."]
     click.echo("Running command:" + " ".join(map(quote, cmd)))
     res = subprocess.run(cmd, cwd=current)
 
     error = False
 
     if res.returncode:
         error = True
@@ -56,15 +59,22 @@
     if not jupytext:
         click.echo(
             "jupytext is missing, black won't run on notebooks. "
             "Fix it with: pip install jupytext"
         )
 
     if nbqa and jupytext:
-        cmd = ["nbqa", "black", ".", "--extend-exclude", exclude_str]
+        if exclude_str:
+            cmd = ["nbqa", "black", ".", "--extend-exclude", exclude_str]
+        else:
+            cmd = [
+                "nbqa",
+                "black",
+                ".",
+            ]
         click.echo("Running command:" + " ".join(map(quote, cmd)))
         res_nb = subprocess.run(cmd, cwd=current)
 
         if res_nb.returncode:
             error = True
 
     if error:
```

### Comparing `pkgmt-0.7.0/src/pkgmt/github.py` & `pkgmt-0.7.1/src/pkgmt/github.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/hook.py` & `pkgmt-0.7.1/src/pkgmt/hook.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,16 +67,22 @@
         files = ["."]
     else:
         files = list(files)
 
     exclude_str_flake8 = ",".join(exclude)
     exclude_str_black = "|".join(exclude)
 
-    cmd_black = ["black", "--check"] + files + ["--extend-exclude", exclude_str_black]
-    cmd_flake8 = ["flake8"] + files + ["--extend-exclude", exclude_str_flake8]
+    if exclude_str_flake8 and exclude_str_black:
+        cmd_black = (
+            ["black", "--check"] + files + ["--extend-exclude", exclude_str_black]
+        )
+        cmd_flake8 = ["flake8"] + files + ["--extend-exclude", exclude_str_flake8]
+    else:
+        cmd_black = ["black", "--check"] + files
+        cmd_flake8 = ["flake8"] + files
     runner = Runner(find_root())
     runner.run(cmd_flake8, fix="Run: pkgmt format")
     runner.run(cmd_black, fix="Run: pkgmt format")
 
     if not nbqa:
         click.echo(
             "nbqa is missing, flake8 won't run on notebooks. "
@@ -86,15 +92,19 @@
     if not jupytext:
         click.echo(
             "jupytext is missing, flake8 won't run on notebooks. "
             "Fix it with: pip install jupytext"
         )
 
     if nbqa and jupytext:
-        cmd = ["nbqa", "flake8"] + files + ["--extend-exclude", exclude_str_flake8]
+        if exclude_str_flake8 and exclude_str_black:
+            cmd = ["nbqa", "flake8"] + files + ["--extend-exclude", exclude_str_flake8]
+        else:
+            cmd = ["nbqa", "flake8"] + files
+
         runner.run(
             cmd,
             fix="Install nbqa jupytext and run: pkgmt format",
         )
 
     return runner.check()
```

### Comparing `pkgmt-0.7.0/src/pkgmt/links.py` & `pkgmt-0.7.1/src/pkgmt/links.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/new.py` & `pkgmt-0.7.1/src/pkgmt/new.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/test.py` & `pkgmt-0.7.1/src/pkgmt/test.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/versioneer.py` & `pkgmt-0.7.1/src/pkgmt/versioneer.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/versioner/util.py` & `pkgmt-0.7.1/src/pkgmt/versioner/util.py`

 * *Files identical despite different names*

### Comparing `pkgmt-0.7.0/src/pkgmt/versioner/versioner.py` & `pkgmt-0.7.1/src/pkgmt/versioner/versioner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 import ast
 import datetime
 import subprocess
 
 from pathlib import Path
 
+import click
+
 from pkgmt.versioner.util import complete_version_string, find_package_and_version_file
 
 
 def replace_in_file(path_to_file, original, replacement):
     """Replace string in file"""
     with open(path_to_file, "r+") as f:
         content = f.read()
@@ -47,22 +49,40 @@
             self.path_to_changelog = Path(self.project_root, "CHANGELOG.rst")
         elif Path(self.project_root, "CHANGELOG.md").exists():
             self.path_to_changelog = Path(self.project_root, "CHANGELOG.md")
         else:
             self.path_to_changelog = None
         self.version_file = version_file_name
 
+    def get_version_file_path(self):
+        """Returns the version file path from project root"""
+        return str(self.PACKAGE / self.version_file)
+
     def current_version(self):
         """Returns the current version in version file"""
         _version_re = re.compile(r"__version__\s+=\s+(.*)")
 
         with open(self.PACKAGE / self.version_file, "rb") as f:
-            VERSION = str(
-                ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
-            )
+            try:
+                VERSION = str(
+                    ast.literal_eval(
+                        _version_re.search(f.read().decode("utf-8")).group(1)
+                    )
+                )
+            except AttributeError:
+                raise click.ClickException(
+                    f"Please add version string in "
+                    f"{self.get_version_file_path()}, e.g., __version__ = '0.1dev'"
+                )
+            except SyntaxError:
+                raise click.ClickException(
+                    f"Could not find __version__ value in "
+                    f"{self.get_version_file_path()}. Please add in the format"
+                    f" __version__ = '0.1dev'"
+                )
 
         return VERSION
 
     def release_version(self):
         """
         Returns a release version number
         e.g. 2.4.4dev -> v.2.2.4
```

### Comparing `pkgmt-0.7.0/src/pkgmt.egg-info/SOURCES.txt` & `pkgmt-0.7.1/src/pkgmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

