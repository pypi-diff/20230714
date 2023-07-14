# Comparing `tmp/agentware-0.1.0.tar.gz` & `tmp/agentware-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/agentware-0.1.0.tar", last modified: Fri Jul 14 03:50:34 2023, max compression
+gzip compressed data, was "dist/agentware-0.1.1.tar", last modified: Fri Jul 14 05:00:33 2023, max compression
```

## Comparing `agentware-0.1.0.tar` & `agentware-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 03:50:34.739604 agentware-0.1.0/
--rw-r--r--   0 weiduan    (501) staff       (20)      220 2023-07-14 03:50:34.738710 agentware-0.1.0/PKG-INFO
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 03:50:34.727243 agentware-0.1.0/agentware/
--rw-r--r--   0 weiduan    (501) staff       (20)      168 2023-07-12 13:20:22.000000 agentware-0.1.0/agentware/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     4439 2023-07-13 10:10:58.000000 agentware-0.1.0/agentware/agent.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1799 2023-07-10 15:16:08.000000 agentware-0.1.0/agentware/agent_logger.py
--rw-r--r--   0 weiduan    (501) staff       (20)    23058 2023-07-13 12:23:05.000000 agentware-0.1.0/agentware/base.py
--rw-r--r--   0 weiduan    (501) staff       (20)      224 2023-07-13 12:26:26.000000 agentware-0.1.0/agentware/error_codes.py
--rw-r--r--   0 weiduan    (501) staff       (20)      250 2023-07-12 14:52:41.000000 agentware-0.1.0/agentware/hub.py
--rw-r--r--   0 weiduan    (501) staff       (20)    13831 2023-07-13 12:05:53.000000 agentware-0.1.0/agentware/memory.py
--rw-r--r--   0 weiduan    (501) staff       (20)      225 2023-07-10 14:52:15.000000 agentware-0.1.0/agentware/singleton.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 03:50:34.731529 agentware-0.1.0/agentware.egg-info/
--rw-r--r--   0 weiduan    (501) staff       (20)      220 2023-07-14 03:50:34.000000 agentware-0.1.0/agentware.egg-info/PKG-INFO
--rw-r--r--   0 weiduan    (501) staff       (20)      440 2023-07-14 03:50:34.000000 agentware-0.1.0/agentware.egg-info/SOURCES.txt
--rw-r--r--   0 weiduan    (501) staff       (20)        1 2023-07-14 03:50:34.000000 agentware-0.1.0/agentware.egg-info/dependency_links.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       52 2023-07-14 03:50:34.000000 agentware-0.1.0/agentware.egg-info/requires.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       16 2023-07-14 03:50:34.000000 agentware-0.1.0/agentware.egg-info/top_level.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       38 2023-07-14 03:50:34.740040 agentware-0.1.0/setup.cfg
--rw-r--r--   0 weiduan    (501) staff       (20)      486 2023-07-10 15:16:07.000000 agentware-0.1.0/setup.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 03:50:34.736629 agentware-0.1.0/tests/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-12 09:22:40.000000 agentware-0.1.0/tests/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1819 2023-07-13 10:12:38.000000 agentware-0.1.0/tests/agent_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)      549 2023-07-10 15:16:07.000000 agentware-0.1.0/tests/connector_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.0/tests/memory_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)      281 2023-07-12 14:42:06.000000 agentware-0.1.0/tests/utils.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 05:00:33.994608 agentware-0.1.1/
+-rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 05:00:33.994093 agentware-0.1.1/PKG-INFO
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 05:00:33.985673 agentware-0.1.1/agentware/
+-rw-r--r--   0 weiduan    (501) staff       (20)      168 2023-07-12 13:20:22.000000 agentware-0.1.1/agentware/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     4439 2023-07-13 10:10:58.000000 agentware-0.1.1/agentware/agent.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1799 2023-07-10 15:16:08.000000 agentware-0.1.1/agentware/agent_logger.py
+-rw-r--r--   0 weiduan    (501) staff       (20)    23058 2023-07-13 12:23:05.000000 agentware-0.1.1/agentware/base.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      224 2023-07-13 12:26:26.000000 agentware-0.1.1/agentware/error_codes.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      250 2023-07-12 14:52:41.000000 agentware-0.1.1/agentware/hub.py
+-rw-r--r--   0 weiduan    (501) staff       (20)    13831 2023-07-13 12:05:53.000000 agentware-0.1.1/agentware/memory.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      225 2023-07-10 14:52:15.000000 agentware-0.1.1/agentware/singleton.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 05:00:33.989828 agentware-0.1.1/agentware.egg-info/
+-rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 05:00:33.000000 agentware-0.1.1/agentware.egg-info/PKG-INFO
+-rw-r--r--   0 weiduan    (501) staff       (20)      440 2023-07-14 05:00:33.000000 agentware-0.1.1/agentware.egg-info/SOURCES.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)        1 2023-07-14 05:00:33.000000 agentware-0.1.1/agentware.egg-info/dependency_links.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       43 2023-07-14 05:00:33.000000 agentware-0.1.1/agentware.egg-info/requires.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       16 2023-07-14 05:00:33.000000 agentware-0.1.1/agentware.egg-info/top_level.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       38 2023-07-14 05:00:33.994745 agentware-0.1.1/setup.cfg
+-rw-r--r--   0 weiduan    (501) staff       (20)      467 2023-07-14 04:59:19.000000 agentware-0.1.1/setup.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 05:00:33.993318 agentware-0.1.1/tests/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-12 09:22:40.000000 agentware-0.1.1/tests/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1819 2023-07-13 10:12:38.000000 agentware-0.1.1/tests/agent_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      549 2023-07-10 15:16:07.000000 agentware-0.1.1/tests/connector_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.1/tests/memory_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      281 2023-07-12 14:42:06.000000 agentware-0.1.1/tests/utils.py
```

### Comparing `agentware-0.1.0/agentware/agent.py` & `agentware-0.1.1/agentware/agent.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.0/agentware/agent_logger.py` & `agentware-0.1.1/agentware/agent_logger.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.0/agentware/base.py` & `agentware-0.1.1/agentware/base.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.0/agentware/memory.py` & `agentware-0.1.1/agentware/memory.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.0/tests/agent_test.py` & `agentware-0.1.1/tests/agent_test.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.0/tests/connector_test.py` & `agentware-0.1.1/tests/connector_test.py`

 * *Files identical despite different names*

