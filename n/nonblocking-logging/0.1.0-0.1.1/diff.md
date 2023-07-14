# Comparing `tmp/nonblocking_logging-0.1.0.tar.gz` & `tmp/nonblocking_logging-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonblocking_logging-0.1.0.tar", max compression
+gzip compressed data, was "nonblocking_logging-0.1.1.tar", max compression
```

## Comparing `nonblocking_logging-0.1.0.tar` & `nonblocking_logging-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-07-13 11:49:25.507351 nonblocking_logging-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-13 05:57:41.647426 nonblocking_logging-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 05:57:41.647426 nonblocking_logging-0.1.0/nonblocking_logging/__init__.py
--rw-r--r--   0        0        0       68 2023-07-13 11:53:32.527350 nonblocking_logging-0.1.0/nonblocking_logging/handlers/__init__.py
--rw-r--r--   0        0        0     1527 2023-07-13 11:25:07.151356 nonblocking_logging-0.1.0/nonblocking_logging/handlers/telegram.py
--rw-r--r--   0        0        0        0 2023-07-13 11:54:13.571350 nonblocking_logging-0.1.0/nonblocking_logging/integrations/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 10:43:47.367365 nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/__init__.py
--rw-r--r--   0        0        0      373 2023-07-13 11:25:07.159356 nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/apps.py
--rw-r--r--   0        0        0     1991 2023-07-13 10:47:04.959364 nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/conf.py
--rw-r--r--   0        0        0       68 2023-07-13 11:56:35.055349 nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/handlers/__init__.py
--rw-r--r--   0        0        0     1264 2023-07-13 11:56:35.051349 nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/handlers/telegram.py
--rw-r--r--   0        0        0      154 2023-07-13 10:47:04.955364 nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/startup.py
--rw-r--r--   0        0        0      330 2023-07-13 11:51:19.487351 nonblocking_logging-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 nonblocking_logging-0.1.0/setup.py
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 nonblocking_logging-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-13 11:49:25.507351 nonblocking_logging-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-13 05:57:41.647426 nonblocking_logging-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 05:57:41.647426 nonblocking_logging-0.1.1/nonblocking_logging/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-13 11:53:32.527350 nonblocking_logging-0.1.1/nonblocking_logging/handlers/__init__.py
+-rw-r--r--   0        0        0     1527 2023-07-13 11:25:07.151356 nonblocking_logging-0.1.1/nonblocking_logging/handlers/telegram.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:54:13.571350 nonblocking_logging-0.1.1/nonblocking_logging/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 10:43:47.367365 nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-14 11:01:54.703779 nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/apps.py
+-rw-r--r--   0        0        0     1991 2023-07-13 10:47:04.959364 nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/conf.py
+-rw-r--r--   0        0        0       68 2023-07-13 11:56:35.055349 nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/handlers/__init__.py
+-rw-r--r--   0        0        0     1264 2023-07-13 11:56:35.051349 nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/handlers/telegram.py
+-rw-r--r--   0        0        0      154 2023-07-13 10:47:04.955364 nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/startup.py
+-rw-r--r--   0        0        0      330 2023-07-14 11:12:19.059788 nonblocking_logging-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 nonblocking_logging-0.1.1/PKG-INFO
```

### Comparing `nonblocking_logging-0.1.0/LICENSE` & `nonblocking_logging-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonblocking_logging-0.1.0/nonblocking_logging/handlers/telegram.py` & `nonblocking_logging-0.1.1/nonblocking_logging/handlers/telegram.py`

 * *Files identical despite different names*

### Comparing `nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/conf.py` & `nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/conf.py`

 * *Files identical despite different names*

### Comparing `nonblocking_logging-0.1.0/nonblocking_logging/integrations/django/handlers/telegram.py` & `nonblocking_logging-0.1.1/nonblocking_logging/integrations/django/handlers/telegram.py`

 * *Files identical despite different names*

