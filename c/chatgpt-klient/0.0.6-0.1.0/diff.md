# Comparing `tmp/chatgpt-klient-0.0.6.tar.gz` & `tmp/chatgpt-klient-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.0.6.tar", last modified: Wed Jul 12 10:16:16 2023, max compression
+gzip compressed data, was "chatgpt-klient-0.1.0.tar", last modified: Fri Jul 14 09:27:17 2023, max compression
```

## Comparing `chatgpt-klient-0.0.6.tar` & `chatgpt-klient-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.0.6/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-12 10:12:59.000000 chatgpt-klient-0.0.6/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.698738 chatgpt-klient-0.0.6/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.698738 chatgpt-klient-0.0.6/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-12 10:12:48.000000 chatgpt-klient-0.0.6/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     5594 2023-07-12 10:12:26.000000 chatgpt-klient-0.0.6/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1290 2023-06-01 11:37:17.000000 chatgpt-klient-0.0.6/src/chatgpt_klient/consts.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-12 10:16:16.702738 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      322 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-12 10:16:16.000000 chatgpt-klient-0.0.6/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.1.0/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-14 09:21:31.000000 chatgpt-klient-0.1.0/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.177310 chatgpt-klient-0.1.0/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.185310 chatgpt-klient-0.1.0/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-14 09:21:25.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     8322 2023-07-14 09:21:43.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1054 2023-07-14 08:06:02.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/consts.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/exceptions.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      149 2023-07-14 08:09:12.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/utils.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      383 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/top_level.txt
```

