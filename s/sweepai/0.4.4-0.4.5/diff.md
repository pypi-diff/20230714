# Comparing `tmp/sweepai-0.4.4.tar.gz` & `tmp/sweepai-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.4.tar", max compression
+gzip compressed data, was "sweepai-0.4.5.tar", max compression
```

## Comparing `sweepai-0.4.4.tar` & `sweepai-0.4.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    20850 2023-06-14 19:09:46.074723 sweepai-0.4.4/LICENSE
--rw-r--r--   0        0        0     6847 2023-07-13 18:59:01.830686 sweepai-0.4.4/README.md
--rw-r--r--   0        0        0     1411 2023-07-13 23:41:42.574605 sweepai-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.418346 sweepai-0.4.4/sweepai/__init__.py
--rw-r--r--   0        0        0    12345 2023-07-13 18:59:01.833466 sweepai-0.4.4/sweepai/api.py
--rw-r--r--   0        0        0     6651 2023-07-13 23:38:12.894410 sweepai-0.4.4/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10697 2023-07-13 23:27:42.917993 sweepai-0.4.4/sweepai/app/backend.py
--rw-r--r--   0        0        0     1167 2023-07-13 18:59:01.834993 sweepai-0.4.4/sweepai/app/cli.py
--rw-r--r--   0        0        0     3615 2023-07-13 23:13:30.928829 sweepai-0.4.4/sweepai/app/config.py
--rw-r--r--   0        0        0    15383 2023-07-13 22:49:37.300901 sweepai-0.4.4/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.419148 sweepai-0.4.4/sweepai/core/__init__.py
--rw-r--r--   0        0        0    18015 2023-07-13 23:25:51.402683 sweepai-0.4.4/sweepai/core/chat.py
--rw-r--r--   0        0        0     2880 2023-07-13 18:59:01.836485 sweepai-0.4.4/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8273 2023-07-13 18:59:01.836657 sweepai-0.4.4/sweepai/core/entities.py
--rw-r--r--   0        0        0      535 2023-07-13 18:59:01.837093 sweepai-0.4.4/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16873 2023-07-13 21:52:24.490410 sweepai-0.4.4/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3489 2023-07-13 18:59:01.837629 sweepai-0.4.4/sweepai/core/react.py
--rw-r--r--   0        0        0    20835 2023-07-13 19:24:27.610154 sweepai-0.4.4/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    13594 2023-07-13 18:59:01.837980 sweepai-0.4.4/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3191 2023-07-13 18:59:01.838139 sweepai-0.4.4/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.420325 sweepai-0.4.4/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     7146 2023-07-13 23:28:07.436121 sweepai-0.4.4/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2613 2023-07-13 21:42:18.752139 sweepai-0.4.4/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9748 2023-07-13 19:26:08.750222 sweepai-0.4.4/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4042 2023-07-13 18:59:01.840830 sweepai-0.4.4/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    19986 2023-07-13 22:06:11.061049 sweepai-0.4.4/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841069 sweepai-0.4.4/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.421045 sweepai-0.4.4/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3822 2023-07-13 23:26:07.719104 sweepai-0.4.4/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841626 sweepai-0.4.4/sweepai/utils/config/__init__.py
--rw-r--r--   0        0        0     2761 2023-07-13 23:21:47.583779 sweepai-0.4.4/sweepai/utils/config/client.py
--rw-r--r--   0        0        0     3460 2023-07-13 23:38:41.531570 sweepai-0.4.4/sweepai/utils/config/server.py
--rw-r--r--   0        0        0     6524 2023-07-13 18:59:01.842462 sweepai-0.4.4/sweepai/utils/diff.py
--rw-r--r--   0        0        0      675 2023-07-13 18:59:01.842660 sweepai-0.4.4/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5256 2023-07-13 18:59:01.842775 sweepai-0.4.4/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8431 2023-07-13 18:59:01.843177 sweepai-0.4.4/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0      100 2023-07-13 18:59:01.843270 sweepai-0.4.4/sweepai/utils/hash.py
--rw-r--r--   0        0        0     5585 2023-07-13 18:59:01.843383 sweepai-0.4.4/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      849 2023-07-13 18:59:01.843512 sweepai-0.4.4/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1528 2023-07-13 18:59:01.843616 sweepai-0.4.4/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11648 2023-07-13 18:59:01.843761 sweepai-0.4.4/sweepai/utils/utils.py
--rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 sweepai-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 19:09:46.074723 sweepai-0.4.5/LICENSE
+-rw-r--r--   0        0        0     6847 2023-07-13 18:59:01.830686 sweepai-0.4.5/README.md
+-rw-r--r--   0        0        0     1411 2023-07-13 23:44:40.215808 sweepai-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.418346 sweepai-0.4.5/sweepai/__init__.py
+-rw-r--r--   0        0        0    12345 2023-07-13 18:59:01.833466 sweepai-0.4.5/sweepai/api.py
+-rw-r--r--   0        0        0     6656 2023-07-13 23:44:30.002584 sweepai-0.4.5/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10697 2023-07-13 23:27:42.917993 sweepai-0.4.5/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1167 2023-07-13 18:59:01.834993 sweepai-0.4.5/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3615 2023-07-13 23:13:30.928829 sweepai-0.4.5/sweepai/app/config.py
+-rw-r--r--   0        0        0    15383 2023-07-13 22:49:37.300901 sweepai-0.4.5/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.419148 sweepai-0.4.5/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    18015 2023-07-13 23:25:51.402683 sweepai-0.4.5/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 18:59:01.836485 sweepai-0.4.5/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8273 2023-07-13 18:59:01.836657 sweepai-0.4.5/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 18:59:01.837093 sweepai-0.4.5/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16873 2023-07-13 21:52:24.490410 sweepai-0.4.5/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 18:59:01.837629 sweepai-0.4.5/sweepai/core/react.py
+-rw-r--r--   0        0        0    20835 2023-07-13 19:24:27.610154 sweepai-0.4.5/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 18:59:01.837980 sweepai-0.4.5/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3191 2023-07-13 18:59:01.838139 sweepai-0.4.5/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.420325 sweepai-0.4.5/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     7146 2023-07-13 23:28:07.436121 sweepai-0.4.5/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 21:42:18.752139 sweepai-0.4.5/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9748 2023-07-13 19:26:08.750222 sweepai-0.4.5/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 18:59:01.840830 sweepai-0.4.5/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19986 2023-07-13 22:06:11.061049 sweepai-0.4.5/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841069 sweepai-0.4.5/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.421045 sweepai-0.4.5/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-13 23:26:07.719104 sweepai-0.4.5/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841626 sweepai-0.4.5/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2761 2023-07-13 23:21:47.583779 sweepai-0.4.5/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3460 2023-07-13 23:38:41.531570 sweepai-0.4.5/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     6524 2023-07-13 18:59:01.842462 sweepai-0.4.5/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 18:59:01.842660 sweepai-0.4.5/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 18:59:01.842775 sweepai-0.4.5/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8431 2023-07-13 18:59:01.843177 sweepai-0.4.5/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 18:59:01.843270 sweepai-0.4.5/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 18:59:01.843383 sweepai-0.4.5/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 18:59:01.843512 sweepai-0.4.5/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 18:59:01.843616 sweepai-0.4.5/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 18:59:01.843761 sweepai-0.4.5/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 sweepai-0.4.5/PKG-INFO
```

### Comparing `sweepai-0.4.4/LICENSE` & `sweepai-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/README.md` & `sweepai-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/pyproject.toml` & `sweepai-0.4.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.4"
+version = "0.4.5"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.4/sweepai/api.py` & `sweepai-0.4.5/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/app/api_client.py` & `sweepai-0.4.5/sweepai/app/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 break
             except json.JSONDecodeError:
                 pass
 
 
 class APIClient(BaseModel):
     config: SweepChatConfig
-    api_endpoint = SWEEP_API_ENDPOINT
+    api_endpoint: str = SWEEP_API_ENDPOINT
 
     def __init__(self, config: SweepChatConfig):
         super().__init__(config=config)
         self.config = config
         logger.info(f"Initializing API client")
         logger.info(f"API endpoint: {self.api_endpoint}")
         logger.info(f"Github APP Client ID: {GITHUB_APP_CLIENT_ID}")
```

### Comparing `sweepai-0.4.4/sweepai/app/backend.py` & `sweepai-0.4.5/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/app/cli.py` & `sweepai-0.4.5/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/app/config.py` & `sweepai-0.4.5/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/app/ui.py` & `sweepai-0.4.5/sweepai/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/chat.py` & `sweepai-0.4.5/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/code_repair.py` & `sweepai-0.4.5/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/entities.py` & `sweepai-0.4.5/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/gha_extraction.py` & `sweepai-0.4.5/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/prompts.py` & `sweepai-0.4.5/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/react.py` & `sweepai-0.4.5/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/sweep_bot.py` & `sweepai-0.4.5/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/core/vector_db.py` & `sweepai-0.4.5/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/events.py` & `sweepai-0.4.5/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/handlers/create_pr.py` & `sweepai-0.4.5/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.5/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/handlers/on_comment.py` & `sweepai-0.4.5/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/handlers/on_review.py` & `sweepai-0.4.5/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/handlers/on_ticket.py` & `sweepai-0.4.5/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/chat_logger.py` & `sweepai-0.4.5/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/config/client.py` & `sweepai-0.4.5/sweepai/utils/config/client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/config/server.py` & `sweepai-0.4.5/sweepai/utils/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/diff.py` & `sweepai-0.4.5/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/event_logger.py` & `sweepai-0.4.5/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/file_change_functions.py` & `sweepai-0.4.5/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/github_utils.py` & `sweepai-0.4.5/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.5/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/scorer.py` & `sweepai-0.4.5/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/snippets.py` & `sweepai-0.4.5/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/sweepai/utils/utils.py` & `sweepai-0.4.5/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.4/PKG-INFO` & `sweepai-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.4
+Version: 0.4.5
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.4 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.5 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
```

