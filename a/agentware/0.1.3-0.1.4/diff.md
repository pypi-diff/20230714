# Comparing `tmp/agentware-0.1.3.tar.gz` & `tmp/agentware-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/agentware-0.1.3.tar", last modified: Fri Jul 14 09:19:59 2023, max compression
+gzip compressed data, was "dist/agentware-0.1.4.tar", last modified: Fri Jul 14 09:48:37 2023, max compression
```

## Comparing `agentware-0.1.3.tar` & `agentware-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.301140 agentware-0.1.3/
--rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 09:19:59.299504 agentware-0.1.3/PKG-INFO
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.246660 agentware-0.1.3/agentware/
--rw-r--r--   0 weiduan    (501) staff       (20)      168 2023-07-12 13:20:22.000000 agentware-0.1.3/agentware/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     4439 2023-07-13 10:10:58.000000 agentware-0.1.3/agentware/agent.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1799 2023-07-10 15:16:08.000000 agentware-0.1.3/agentware/agent_logger.py
--rw-r--r--   0 weiduan    (501) staff       (20)    23058 2023-07-13 12:23:05.000000 agentware-0.1.3/agentware/base.py
--rw-r--r--   0 weiduan    (501) staff       (20)      224 2023-07-13 12:26:26.000000 agentware-0.1.3/agentware/error_codes.py
--rw-r--r--   0 weiduan    (501) staff       (20)      250 2023-07-12 14:52:41.000000 agentware-0.1.3/agentware/hub.py
--rw-r--r--   0 weiduan    (501) staff       (20)    13831 2023-07-13 12:05:53.000000 agentware-0.1.3/agentware/memory.py
--rw-r--r--   0 weiduan    (501) staff       (20)      225 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/singleton.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.259697 agentware-0.1.3/agentware/utils/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 05:21:12.000000 agentware-0.1.3/agentware/utils/__init__.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.279448 agentware-0.1.3/agentware/utils/json_fixes/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/utils/json_fixes/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     2268 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/utils/json_fixes/auto_fix.py
--rw-r--r--   0 weiduan    (501) staff       (20)      800 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/utils/json_fixes/bracket_termination.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1052 2023-07-10 15:16:07.000000 agentware-0.1.3/agentware/utils/json_fixes/escaping.py
--rw-r--r--   0 weiduan    (501) staff       (20)      795 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/utils/json_fixes/master_json_fix_method.py
--rw-r--r--   0 weiduan    (501) staff       (20)      674 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/utils/json_fixes/missing_quotes.py
--rw-r--r--   0 weiduan    (501) staff       (20)     6066 2023-07-10 15:16:08.000000 agentware-0.1.3/agentware/utils/json_fixes/parsing.py
--rw-r--r--   0 weiduan    (501) staff       (20)      565 2023-07-10 14:52:15.000000 agentware-0.1.3/agentware/utils/json_fixes/utilities.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.285168 agentware-0.1.3/agentware/utils/json_validation/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 09:17:54.000000 agentware-0.1.3/agentware/utils/json_validation/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1071 2023-07-10 15:16:07.000000 agentware-0.1.3/agentware/utils/json_validation/validate_json.py
--rw-r--r--   0 weiduan    (501) staff       (20)     2255 2023-07-10 15:16:07.000000 agentware-0.1.3/agentware/utils/num_token_utils.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.256543 agentware-0.1.3/agentware.egg-info/
--rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 09:19:58.000000 agentware-0.1.3/agentware.egg-info/PKG-INFO
--rw-r--r--   0 weiduan    (501) staff       (20)      939 2023-07-14 09:19:59.000000 agentware-0.1.3/agentware.egg-info/SOURCES.txt
--rw-r--r--   0 weiduan    (501) staff       (20)        1 2023-07-14 09:19:58.000000 agentware-0.1.3/agentware.egg-info/dependency_links.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       43 2023-07-14 09:19:58.000000 agentware-0.1.3/agentware.egg-info/requires.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       16 2023-07-14 09:19:58.000000 agentware-0.1.3/agentware.egg-info/top_level.txt
--rw-r--r--   0 weiduan    (501) staff       (20)       38 2023-07-14 09:19:59.301696 agentware-0.1.3/setup.cfg
--rw-r--r--   0 weiduan    (501) staff       (20)      467 2023-07-14 09:19:05.000000 agentware-0.1.3/setup.py
-drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:19:59.296457 agentware-0.1.3/tests/
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-12 09:22:40.000000 agentware-0.1.3/tests/__init__.py
--rw-r--r--   0 weiduan    (501) staff       (20)     1819 2023-07-13 10:12:38.000000 agentware-0.1.3/tests/agent_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)      549 2023-07-10 15:16:07.000000 agentware-0.1.3/tests/connector_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.3/tests/memory_test.py
--rw-r--r--   0 weiduan    (501) staff       (20)      281 2023-07-12 14:42:06.000000 agentware-0.1.3/tests/utils.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.269218 agentware-0.1.4/
+-rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 09:48:37.268511 agentware-0.1.4/PKG-INFO
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.252893 agentware-0.1.4/agentware/
+-rw-r--r--   0 weiduan    (501) staff       (20)      168 2023-07-12 13:20:22.000000 agentware-0.1.4/agentware/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     4439 2023-07-13 10:10:58.000000 agentware-0.1.4/agentware/agent.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1799 2023-07-10 15:16:08.000000 agentware-0.1.4/agentware/agent_logger.py
+-rw-r--r--   0 weiduan    (501) staff       (20)    23058 2023-07-13 12:23:05.000000 agentware-0.1.4/agentware/base.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      224 2023-07-13 12:26:26.000000 agentware-0.1.4/agentware/error_codes.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      250 2023-07-12 14:52:41.000000 agentware-0.1.4/agentware/hub.py
+-rw-r--r--   0 weiduan    (501) staff       (20)    13831 2023-07-13 12:05:53.000000 agentware-0.1.4/agentware/memory.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      225 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/singleton.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.256797 agentware-0.1.4/agentware/utils/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 05:21:12.000000 agentware-0.1.4/agentware/utils/__init__.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.262251 agentware-0.1.4/agentware/utils/json_fixes/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     2268 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/auto_fix.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      800 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/bracket_termination.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1052 2023-07-10 15:16:07.000000 agentware-0.1.4/agentware/utils/json_fixes/escaping.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      795 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/master_json_fix_method.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      674 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/missing_quotes.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     6003 2023-07-14 09:47:09.000000 agentware-0.1.4/agentware/utils/json_fixes/parsing.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      565 2023-07-10 14:52:15.000000 agentware-0.1.4/agentware/utils/json_fixes/utilities.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.263733 agentware-0.1.4/agentware/utils/json_validation/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-14 09:17:54.000000 agentware-0.1.4/agentware/utils/json_validation/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1071 2023-07-10 15:16:07.000000 agentware-0.1.4/agentware/utils/json_validation/validate_json.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     2255 2023-07-10 15:16:07.000000 agentware-0.1.4/agentware/utils/num_token_utils.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.255812 agentware-0.1.4/agentware.egg-info/
+-rw-r--r--   0 weiduan    (501) staff       (20)      221 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/PKG-INFO
+-rw-r--r--   0 weiduan    (501) staff       (20)      939 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/SOURCES.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)        1 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/dependency_links.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       43 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/requires.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       16 2023-07-14 09:48:37.000000 agentware-0.1.4/agentware.egg-info/top_level.txt
+-rw-r--r--   0 weiduan    (501) staff       (20)       38 2023-07-14 09:48:37.269381 agentware-0.1.4/setup.cfg
+-rw-r--r--   0 weiduan    (501) staff       (20)      467 2023-07-14 09:48:34.000000 agentware-0.1.4/setup.py
+drwxr-xr-x   0 weiduan    (501) staff       (20)        0 2023-07-14 09:48:37.267492 agentware-0.1.4/tests/
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-12 09:22:40.000000 agentware-0.1.4/tests/__init__.py
+-rw-r--r--   0 weiduan    (501) staff       (20)     1819 2023-07-13 10:12:38.000000 agentware-0.1.4/tests/agent_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      549 2023-07-10 15:16:07.000000 agentware-0.1.4/tests/connector_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)        0 2023-07-10 14:52:15.000000 agentware-0.1.4/tests/memory_test.py
+-rw-r--r--   0 weiduan    (501) staff       (20)      281 2023-07-12 14:42:06.000000 agentware-0.1.4/tests/utils.py
```

### Comparing `agentware-0.1.3/agentware/agent.py` & `agentware-0.1.4/agentware/agent.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/agent_logger.py` & `agentware-0.1.4/agentware/agent_logger.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/base.py` & `agentware-0.1.4/agentware/base.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/memory.py` & `agentware-0.1.4/agentware/memory.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/auto_fix.py` & `agentware-0.1.4/agentware/utils/json_fixes/auto_fix.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/bracket_termination.py` & `agentware-0.1.4/agentware/utils/json_fixes/bracket_termination.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/escaping.py` & `agentware-0.1.4/agentware/utils/json_fixes/escaping.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/master_json_fix_method.py` & `agentware-0.1.4/agentware/utils/json_fixes/master_json_fix_method.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/missing_quotes.py` & `agentware-0.1.4/agentware/utils/json_fixes/missing_quotes.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/parsing.py` & `agentware-0.1.4/agentware/utils/json_fixes/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Fix and parse JSON strings."""
 from __future__ import annotations
 
 import contextlib
 import json
 from typing import Any, Dict, Union
-from colorama import Fore
 from regex import regex
 from agentware.utils.json_fixes.auto_fix import fix_json
 from agentware.utils.json_fixes.bracket_termination import balance_braces
 from agentware.utils.json_fixes.escaping import fix_invalid_escape
 from agentware.utils.json_fixes.missing_quotes import add_quotes_to_property_names
 from logging import Logger
 
@@ -156,16 +155,15 @@
         json_pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
         json_match = json_pattern.search(json_string)
 
         if json_match:
             # Extract the valid JSON object from the string
             json_string = json_match.group(0)
             logger.typewriter_log(
-                title="Apparently json was fixed.", title_color=Fore.GREEN
-            )
+                title="Apparently json was fixed.")
             if CFG.speak_mode and debug_mode:
                 say_text("Apparently json was fixed.")
         else:
             return {}
 
     except (json.JSONDecodeError, ValueError):
         if debug_mode:
```

### Comparing `agentware-0.1.3/agentware/utils/json_fixes/utilities.py` & `agentware-0.1.4/agentware/utils/json_fixes/utilities.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/json_validation/validate_json.py` & `agentware-0.1.4/agentware/utils/json_validation/validate_json.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware/utils/num_token_utils.py` & `agentware-0.1.4/agentware/utils/num_token_utils.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/agentware.egg-info/SOURCES.txt` & `agentware-0.1.4/agentware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/tests/agent_test.py` & `agentware-0.1.4/tests/agent_test.py`

 * *Files identical despite different names*

### Comparing `agentware-0.1.3/tests/connector_test.py` & `agentware-0.1.4/tests/connector_test.py`

 * *Files identical despite different names*

