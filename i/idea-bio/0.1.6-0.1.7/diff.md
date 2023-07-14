# Comparing `tmp/idea_bio-0.1.6.tar.gz` & `tmp/idea_bio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idea_bio-0.1.6.tar", max compression
+gzip compressed data, was "idea_bio-0.1.7.tar", max compression
```

## Comparing `idea_bio-0.1.6.tar` & `idea_bio-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-14 03:15:58.372612 idea_bio-0.1.6/LICENSE
--rw-r--r--   0        0        0     2069 2023-07-14 03:15:58.375945 idea_bio-0.1.6/README.md
--rw-r--r--   0        0        0      201 2023-07-14 03:15:58.392612 idea_bio-0.1.6/idea/__init__.py
--rw-r--r--   0        0        0     1561 2023-07-14 03:15:58.392612 idea_bio-0.1.6/idea/_go.py
--rw-r--r--   0        0        0    13085 2023-07-14 17:32:15.663859 idea_bio-0.1.6/idea/_idea.py
--rw-r--r--   0        0        0      597 2023-07-14 17:32:15.663859 idea_bio-0.1.6/idea/_utils.py
--rw-r--r--   0        0        0      691 2023-07-14 17:32:15.663859 idea_bio-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 idea_bio-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 03:15:58.372612 idea_bio-0.1.7/LICENSE
+-rw-r--r--   0        0        0      850 2023-07-14 20:31:46.845288 idea_bio-0.1.7/README.md
+-rw-r--r--   0        0        0      201 2023-07-14 03:15:58.392612 idea_bio-0.1.7/idea/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-14 03:15:58.392612 idea_bio-0.1.7/idea/_go.py
+-rw-r--r--   0        0        0    13085 2023-07-14 17:32:15.663859 idea_bio-0.1.7/idea/_idea.py
+-rw-r--r--   0        0        0      597 2023-07-14 17:32:15.663859 idea_bio-0.1.7/idea/_utils.py
+-rw-r--r--   0        0        0      975 2023-07-14 20:29:37.227561 idea_bio-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 idea_bio-0.1.7/PKG-INFO
```

### Comparing `idea_bio-0.1.6/LICENSE` & `idea_bio-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.6/idea/_go.py` & `idea_bio-0.1.7/idea/_go.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.6/idea/_idea.py` & `idea_bio-0.1.7/idea/_idea.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.6/idea/_utils.py` & `idea_bio-0.1.7/idea/_utils.py`

 * *Files identical despite different names*

