# Comparing `tmp/sweepai-0.4.3.tar.gz` & `tmp/sweepai-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.3.tar", max compression
+gzip compressed data, was "sweepai-0.4.4.tar", max compression
```

## Comparing `sweepai-0.4.3.tar` & `sweepai-0.4.4.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.3/LICENSE
--rw-r--r--   0        0        0     6847 2023-07-13 00:29:33.520020 sweepai-0.4.3/README.md
--rw-r--r--   0        0        0     1411 2023-07-13 22:31:22.984130 sweepai-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/__init__.py
--rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/api.py
--rw-r--r--   0        0        0     6417 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10697 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/backend.py
--rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/cli.py
--rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/config.py
--rw-r--r--   0        0        0    15368 2023-07-13 22:30:25.187445 sweepai-0.4.3/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17965 2023-07-13 22:20:26.747256 sweepai-0.4.3/sweepai/core/chat.py
--rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/entities.py
--rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.3/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/react.py
--rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.3/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     6839 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    19986 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3822 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/utils/config/__init__.py
--rw-r--r--   0        0        0     2759 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/utils/config/client.py
--rw-r--r--   0        0        0     3460 2023-07-13 07:19:30.090833 sweepai-0.4.3/sweepai/utils/config/server.py
--rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/utils/diff.py
--rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8431 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/hash.py
--rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/utils.py
--rw-r--r--   0        0        0     8063 2023-07-13 22:31:57.446699 sweepai-0.4.3/setup.py
--rw-r--r--   0        0        0     7826 2023-07-13 22:31:57.447146 sweepai-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 19:09:46.074723 sweepai-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6847 2023-07-13 18:59:01.830686 sweepai-0.4.4/README.md
+-rw-r--r--   0        0        0     1411 2023-07-13 23:41:42.574605 sweepai-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.418346 sweepai-0.4.4/sweepai/__init__.py
+-rw-r--r--   0        0        0    12345 2023-07-13 18:59:01.833466 sweepai-0.4.4/sweepai/api.py
+-rw-r--r--   0        0        0     6651 2023-07-13 23:38:12.894410 sweepai-0.4.4/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10697 2023-07-13 23:27:42.917993 sweepai-0.4.4/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1167 2023-07-13 18:59:01.834993 sweepai-0.4.4/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3615 2023-07-13 23:13:30.928829 sweepai-0.4.4/sweepai/app/config.py
+-rw-r--r--   0        0        0    15383 2023-07-13 22:49:37.300901 sweepai-0.4.4/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.419148 sweepai-0.4.4/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    18015 2023-07-13 23:25:51.402683 sweepai-0.4.4/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 18:59:01.836485 sweepai-0.4.4/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8273 2023-07-13 18:59:01.836657 sweepai-0.4.4/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 18:59:01.837093 sweepai-0.4.4/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16873 2023-07-13 21:52:24.490410 sweepai-0.4.4/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 18:59:01.837629 sweepai-0.4.4/sweepai/core/react.py
+-rw-r--r--   0        0        0    20835 2023-07-13 19:24:27.610154 sweepai-0.4.4/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 18:59:01.837980 sweepai-0.4.4/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3191 2023-07-13 18:59:01.838139 sweepai-0.4.4/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.420325 sweepai-0.4.4/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     7146 2023-07-13 23:28:07.436121 sweepai-0.4.4/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 21:42:18.752139 sweepai-0.4.4/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9748 2023-07-13 19:26:08.750222 sweepai-0.4.4/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 18:59:01.840830 sweepai-0.4.4/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19986 2023-07-13 22:06:11.061049 sweepai-0.4.4/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841069 sweepai-0.4.4/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:27:38.421045 sweepai-0.4.4/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-13 23:26:07.719104 sweepai-0.4.4/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841626 sweepai-0.4.4/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2761 2023-07-13 23:21:47.583779 sweepai-0.4.4/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3460 2023-07-13 23:38:41.531570 sweepai-0.4.4/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     6524 2023-07-13 18:59:01.842462 sweepai-0.4.4/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 18:59:01.842660 sweepai-0.4.4/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 18:59:01.842775 sweepai-0.4.4/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8431 2023-07-13 18:59:01.843177 sweepai-0.4.4/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 18:59:01.843270 sweepai-0.4.4/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 18:59:01.843383 sweepai-0.4.4/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 18:59:01.843512 sweepai-0.4.4/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 18:59:01.843616 sweepai-0.4.4/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 18:59:01.843761 sweepai-0.4.4/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 sweepai-0.4.4/PKG-INFO
```

### Comparing `sweepai-0.4.3/LICENSE` & `sweepai-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/README.md` & `sweepai-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/pyproject.toml` & `sweepai-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.3"
+version = "0.4.4"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.3/sweepai/api.py` & `sweepai-0.4.4/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/app/api_client.py` & `sweepai-0.4.4/sweepai/app/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,15 +129,18 @@
                 "file_change_requests": file_change_requests,
                 "pull_request": pull_request,
                 "messages": messages,
                 "config": self.config.dict(),
             },
             timeout=10 * 60
         )
-        return results.json()
+        try:
+            return results.json()
+        except json.JSONDecodeError:
+            raise Exception(f"{results.text} is invalid JSON")
 
     def chat(
             self,
             messages: list[tuple[str | None, str | None]],
             snippets: list[Snippet] = [],
             model: str = "gpt-4-0613",
     ) -> str:
@@ -145,15 +148,18 @@
             self.api_endpoint + "/chat",
             json={
                 "messages": messages,
                 "snippets": [snippet.dict() for snippet in snippets],
                 "config": self.config.dict()
             }
         )
-        return results.json()
+        try:
+            return results.json()
+        except json.JSONDecodeError:
+            raise Exception(f"{results.text} is invalid JSON")
 
     def stream_chat(
             self,
             messages: list[tuple[str | None, str | None]],
             snippets: list[Snippet] = [],
             functions: list[Function] = [],
             function_call: Any = "auto",
```

### Comparing `sweepai-0.4.3/sweepai/app/backend.py` & `sweepai-0.4.4/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/app/cli.py` & `sweepai-0.4.4/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/app/config.py` & `sweepai-0.4.4/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/app/ui.py` & `sweepai-0.4.4/sweepai/app/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
     def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_paths, plan):
         global global_state
         for chat_history, snippets_text, file_paths, plan in _handle_message_stream(chat_history, snippets_text,
                                                                                     file_paths, plan):
             if plan is None or plan == [[]] or plan == [[""]] or plan == [["", ""]]:
                 plan = [["", ""]]
             if plan and isinstance(plan[0], list):
-                plan = [item.split(":") for item in plan]
+                plan = [item.split(":") for item in plan if ":" in item]
             global_state = State(
                 chat_history=chat_history,
                 snippets_text=snippets_text,
                 file_paths=file_paths,
                 plan=plan,
             )
             config.state = global_state
```

### Comparing `sweepai-0.4.3/sweepai/core/chat.py` & `sweepai-0.4.4/sweepai/core/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             content=system_message_prompt,
         )
     ]
     prev_message_states: list[list[Message]] = []
     model: ChatModel = "gpt-4-32k-0613" if OPENAI_DO_HAVE_32K_MODEL_ACCESS else "gpt-4-0613"
     human_message: HumanMessagePrompt | None = None
     file_change_paths = []
-    chat_logger: ChatLogger | None = None
+    chat_logger: ChatLogger | None
 
     @classmethod
     def from_system_message_content(
-            cls, human_message: HumanMessagePrompt, is_reply: bool = False, **kwargs
+            cls, human_message: HumanMessagePrompt, is_reply: bool = False, chat_logger = None, **kwargs
     ) -> Self:
         if is_reply:
             system_message_content = system_message_issue_comment_prompt
 
         # Todo: This moves prompts away from unified system message prompt
         # system_message_prompt + "\n\n" + human_message.construct_prompt()
         messages = [
@@ -85,14 +85,15 @@
         added_messages = human_message.construct_prompt()  # [ { role, content }, ... ]
         for msg in added_messages:
             messages.append(Message(**msg))
 
         return cls(
             messages=messages,
             human_message=human_message,
+            chat_logger=chat_logger,
             **kwargs,
         )
 
     @classmethod
     def from_system_message_string(cls, prompt_string, **kwargs) -> Self:
         return cls(
             messages=[Message(role="system", content=prompt_string, key="system")],
```

### Comparing `sweepai-0.4.3/sweepai/core/code_repair.py` & `sweepai-0.4.4/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/core/entities.py` & `sweepai-0.4.4/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/core/gha_extraction.py` & `sweepai-0.4.4/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/core/prompts.py` & `sweepai-0.4.4/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/core/react.py` & `sweepai-0.4.4/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/core/sweep_bot.py` & `sweepai-0.4.4/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/core/vector_db.py` & `sweepai-0.4.4/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/events.py` & `sweepai-0.4.4/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/handlers/create_pr.py` & `sweepai-0.4.4/sweepai/handlers/create_pr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import modal
 import openai
 from github.Repository import Repository
 from loguru import logger
 
 from sweepai.core.entities import FileChangeRequest, PullRequest
+from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.config.client import SweepConfig
 from sweepai.utils.config.server import GITHUB_DEFAULT_CONFIG, OPENAI_API_KEY, PREFIX, DB_MODAL_INST_NAME, GITHUB_BOT_TOKEN, \
     GITHUB_BOT_USERNAME, \
     GITHUB_CONFIG_BRANCH
 from sweepai.core.sweep_bot import SweepBot, MaxTokensExceeded
 from sweepai.utils.event_logger import posthog
 
@@ -30,15 +31,22 @@
 ):
     # Flow:
     # 1. Get relevant files
     # 2: Get human message
     # 3. Get files to change
     # 4. Get file changes
     # 5. Create PR
-
+    chat_logger = ChatLogger({
+    "username": username,
+    "installation_id": installation_id,
+    "repo_full_name": sweep_bot.repo.full_name,
+    "title": pull_request.title,
+    "summary": "",
+    "issue_url": ""})
+    sweep_bot.chat_logger = chat_logger
     organization, repo_name = sweep_bot.repo.full_name.split("/")
     metadata = {
         "repo_full_name": sweep_bot.repo.full_name,
         "organization": organization,
         "repo_name": repo_name,
         "repo_description": sweep_bot.repo.description,
         "username": username,
```

### Comparing `sweepai-0.4.3/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.4/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/handlers/on_comment.py` & `sweepai-0.4.4/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/handlers/on_review.py` & `sweepai-0.4.4/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/handlers/on_ticket.py` & `sweepai-0.4.4/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/chat_logger.py` & `sweepai-0.4.4/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/config/client.py` & `sweepai-0.4.4/sweepai/utils/config/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from functools import lru_cache
 
 import yaml
 from github.Repository import Repository
 from loguru import logger
 from pydantic import BaseModel
+from sweepai.utils.config.server import PREFIX
 
 
 class SweepConfig(BaseModel):
     include_dirs: list[str] = []
     exclude_dirs: list[str] = [".git", "node_modules", "venv"]
     include_exts: list[str] = ['.cs', '.csharp', '.py', '.md', '.txt', '.ts', '.tsx', '.js', '.jsx', '.mjs']
     exclude_exts: list[str] = ['.min.js', '.min.js.map', '.min.css', '.min.css.map']
@@ -63,9 +64,8 @@
                 logger.warning(f"Error when getting gha enabled: {e}, falling back to False")
                 return False
         gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8")).get("gha_enabled", False)
         return gha_enabled
 
 # optional, can leave env var blank
 GITHUB_APP_CLIENT_ID = os.environ.get('GITHUB_APP_CLIENT_ID', 'Iv1.91fd31586a926a9f')
-local_env = os.environ.get('ENV', 'prod')
-SWEEP_API_ENDPOINT = os.environ.get('SWEEP_API_ENDPOINT', f"https://sweepai--{local_env}-ui.modal.run")
+SWEEP_API_ENDPOINT = os.environ.get('SWEEP_API_ENDPOINT', f"https://sweepai--{PREFIX}-ui.modal.run")
```

### Comparing `sweepai-0.4.3/sweepai/utils/config/server.py` & `sweepai-0.4.4/sweepai/utils/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/diff.py` & `sweepai-0.4.4/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/event_logger.py` & `sweepai-0.4.4/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/file_change_functions.py` & `sweepai-0.4.4/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/github_utils.py` & `sweepai-0.4.4/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.4/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/scorer.py` & `sweepai-0.4.4/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/snippets.py` & `sweepai-0.4.4/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/sweepai/utils/utils.py` & `sweepai-0.4.4/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.3/setup.py` & `sweepai-0.4.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,171 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sweepai
+Version: 0.4.4
+Summary: Sweep software chores
+Author: Kevin Lu
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: GitPython (>=3.1.31,<4.0.0)
+Requires-Dist: PyGithub (==1.58.2)
+Requires-Dist: config-path (>=1.0.3,<2.0.0)
+Requires-Dist: gradio (>=3.35.2,<4.0.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: urllib3 (<2.0.0)
+Project-URL: Bug Tracker, https://github.com/sweepai/sweep/issues
+Project-URL: Community, https://discord.gg/sweep-ai
+Project-URL: documentation, https://docs.sweep.dev
+Project-URL: homepage, https://sweep.dev
+Project-URL: repository, https://github.com/sweepai/sweep
+Description-Content-Type: text/markdown
+
+<p align="center">
+    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
+</p>
+<p align="center">
+    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>
+</p>
+
+<p align="center">
+<a href="https://sweep.dev">
+    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">
+</a>
+<a href="https://docs.sweep.dev/">
+    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">
+</a> 
+<a href="https://discord.gg/sweep-ai">
+    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />
+</a>
+<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">
+<a href="https://pepy.tech/project/sweepai">
+    <img src="https://static.pepy.tech/badge/sweepai/month" />
+</a>
+<a href="https://github.com/sweepai/sweep">
+    <img src="https://img.shields.io/github/stars/sweepai/sweep" />
+</a>
+<a href="https://twitter.com/sweep__ai">
+    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />
+</a>
+</p>
+
+<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.
+
+Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
+1. 🔍 reads your codebase
+2. 📝 plans the changes
+3. ⚡**writes a pull request with code**⚡
+
+See highlights at https://docs.sweep.dev/examples.
+
+[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
+
+## 🌠 Sweep
+* 🔧 Turns issues directly into pull requests (without an IDE)
+* 👀 Addresses developer replies & comments on its PRs
+* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
+* 🎊 New: Fixes PRs based on Github Actions feedback
+* 🎊 New: Sweep Chat, a local interface for Sweep (see below)
+
+## 🚀 Getting Started
+
+### 🍲 Recipes
+#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. 
+For harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.
+
+A good issue might include:
+
+| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there's a bug/we need this feature/there's this dependency]** |
+|-----------|------------|----------------------|
+|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|
+|In `on_comment.py`|we should not fire an event|because it's possible that the comment is on a closed PR|
+|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|
+
+If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
+
+#### Limitations:
+Sweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep's limitations(for now):
+- Try to change less than 200 lines of code
+- Try to modify less than 3 files
+- Do not include files with more than 1500 lines of code
+
+### ✨ Sweep Github App
+Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
+
+1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+
+### 🖥️ Sweep Chat
+Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
+
+**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
+
+1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
+    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
+    - This runs GitHub authentication in your browser.
+
+2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  
+    - Wait a few seconds and Sweep Chat will start. 
+
+3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).
+
+    - ⚡ Start chatting with Sweep Chat! ⚡
+
+<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
+
+Tips:
+* 🔍 Relevant searched files will show up on the right. 
+* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. 
+* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
+
+#### From Source
+If you want the nightly build and or if the latest build has issues.
+
+1. `git clone https://github.com/sweepai/sweep && poetry install`
+2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
+
+## 🤝 Contributing
+
+Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
+
+## 📘 Story
+
+We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
+
+Unlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.
+
+## 📚 The Stack
+- GPT-4 32k 0613 (default)
+- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model
+- Modal Labs for infra + deployment
+- Gradio for Sweep Chat
+
+## 🗺️ Roadmap
+See [🗺️ Roadmap](https://docs.sweep.dev/roadmap)
+
+## ⭐ Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)
+
+Consider starring us if you're using Sweep so more people hear about us!
+<h2 align="center">
+    Contributors
+</h2>
+<p align="center">
+    Thank you for your contribution!
+</p>
+<p align="center">
+    <a href="https://github.com/sweepai/sweep/graphs/contributors">
+      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />
+    </a>
+</p>
+<p align="center">
+    and, of course, Sweep!
+</p>
 
-packages = \
-['sweepai',
- 'sweepai.app',
- 'sweepai.core',
- 'sweepai.handlers',
- 'sweepai.utils',
- 'sweepai.utils.config']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['GitPython>=3.1.31,<4.0.0',
- 'PyGithub==1.58.2',
- 'config-path>=1.0.3,<2.0.0',
- 'gradio>=3.35.2,<4.0.0',
- 'loguru>=0.6.0,<0.7.0',
- 'pyyaml>=6.0,<7.0',
- 'requests>=2.28.2,<3.0.0',
- 'tabulate>=0.9.0,<0.10.0',
- 'typer>=0.9.0,<0.10.0',
- 'urllib3<2.0.0']
-
-entry_points = \
-{'console_scripts': ['sweep = sweepai.app.cli:app',
-                     'sweepai = sweepai.app.cli:app']}
-
-setup_kwargs = {
-    'name': 'sweepai',
-    'version': '0.4.3',
-    'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep\'s limitations(for now):\n- Try to change less than 200 lines of code\n- Try to modify less than 3 files\n- Do not include files with more than 1500 lines of code\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
-    'author': 'Kevin Lu',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,104 +1,95 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
-'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils',
-'sweepai.utils.config'] package_data = \ {'': ['*']} install_requires = \
-['GitPython>=3.1.31,<4.0.0', 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0',
-'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'pyyaml>=6.0,<7.0',
-'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
-'urllib3<2.0.0'] entry_points = \ {'console_scripts': ['sweep =
-sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.4.3', 'description': 'Sweep software
-chores', 'long_description': '
- \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
-                                3e61f57ad233]\n
-\n
-             \n Bug Reports & Feature Requests â¶  Code Changes\n
-\n\n
-\n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
-  sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
-month]\n\n\n_[https://img.shields.io/github/stars/sweepai/sweep]\n\n\n_[https:/
-  /img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]\n\n
-\n\nSweep is an AI junior developer that transforms bug reports & feature
-requests into code changes.\n\nDescribe bugs, small features, and refactors
-like you would to a junior developer, and Sweep:\n1. ð reads your
-codebase\n2. ð plans the changes\n3. â¡**writes a pull request with
-code**â¡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo]
-(https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
-0af02f2b0e47)\n\n## ð  Sweep\n* ð§ Turns issues directly into pull requests
-(without an IDE)\n* ð Addresses developer replies & comments on its PRs\n*
-ðµï¸\u200dâï¸ Uses embedding-based code search, with popularity reranking
-for repository-level code understanding ([ð Rebuilding our Search Engine in
-a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-
-day))\n* ð New: Fixes PRs based on Github Actions feedback\n* ð New:
-Sweep Chat, a local interface for Sweep (see below)\n\n## ð Getting
-Started\n\n### ð² Recipes\n#### To get the best performance from Sweep, we
-recommend the following approach to writing github issues/chats. \nFor harder
-problems, try to provide the same information a human would need. For simpler
-problems, providing a single line and a file name should suffice.\n\nA good
-issue might include:\n\n| Where to look
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.4 Summary: Sweep software
+chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
+(>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
+(>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
+(>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
+(>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
+typer (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (<2.0.0) Project-URL: Bug
+Tracker, https://github.com/sweepai/sweep/issues Project-URL: Community, https:
+//discord.gg/sweep-ai Project-URL: documentation, https://docs.sweep.dev
+Project-URL: homepage, https://sweep.dev Project-URL: repository, https://
+github.com/sweepai/sweep Description-Content-Type: text/markdown
+  [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
+                                 3e61f57ad233]
+               Bug Reports & Feature Requests â¶  Code Changes
+      [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
+ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
+  img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
+                url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
+Sweep is an AI junior developer that transforms bug reports & feature requests
+into code changes. Describe bugs, small features, and refactors like you would
+to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
+changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
+docs.sweep.dev/examples. [Demo](https://github.com/sweepai/sweep/assets/
+44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns
+issues directly into pull requests (without an IDE) * ð Addresses developer
+replies & comments on its PRs * ðµï¸ââï¸ Uses embedding-based code
+search, with popularity reranking for repository-level code understanding (
+[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-
+rebuilt-our-code-search-engine-in-a-day)) * ð New: Fixes PRs based on Github
+Actions feedback * ð New: Sweep Chat, a local interface for Sweep (see
+below) ## ð Getting Started ### ð² Recipes #### To get the best
+performance from Sweep, we recommend the following approach to writing github
+issues/chats. For harder problems, try to provide the same information a human
+would need. For simpler problems, providing a single line and a file name
+should suffice. A good issue might include: | Where to look
 **[file name or function name]**| What to do
 **[change the logic to do this]** | Additional Context (optional)
-**[there\'s a bug/we need this feature/there\'s this dependency]** |\n|--------
----|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-
-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an
-event|because it\'s possible that the comment is on a closed PR|\n|In the
-config loader in `packages/server/src/config.ts`|add a third option called
-"env" to load the config settings from environment variables| At present, there
-are two options: 1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to
-mention the full path. Similarly, to have Sweep use a function, try to mention
-the class method or what it does. Also see [â¨ Tips and tricks for Sweep]
-(https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to
-complete complex issues on the first try, similar to the average junior
-developer. Here are Sweep\'s limitations(for now):\n- Try to change less than
-200 lines of code\n- Try to modify less than 3 files\n- Do not include files
-with more than 1500 lines of code\n\n### â¨ Sweep Github App\nSetting up Sweep
-is as simple as adding the GitHub bot to a repo, then creating an issue for the
-bot to address.\nWe support all languages GPT4 supports, including Python,
-Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https:
-//github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like
-"Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### ð¥ï¸
-Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally.
-Collaborate on the plan with Sweep, then have it create the pull request for
-you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/
-sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note
-that you need **python 3.10+.**\n - Alternatively run `pip3 install --force-
-reinstall sweepai && sweep` if the previous command fails.\n - This runs GitHub
-authentication in your browser.\n\n2. Copy the ðµ blue 8-digit code from your
-terminal into the page. You should only need to do the authentication once. \n
-- Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from
-the dropdown at the top (the Github app must be installed to this
-repository).\n\n - â¡ Start chatting with Sweep Chat! â¡\n\n[https://
+**[there's a bug/we need this feature/there's this dependency]** | |-----------
+|------------|----------------------| |In `sweepai/app/ui.py`|use an os-
+agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
+event|because it's possible that the comment is on a closed PR| |In the config
+loader in `packages/server/src/config.ts`|add a third option called "env" to
+load the config settings from environment variables| At present, there are two
+options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
+full path. Similarly, to have Sweep use a function, try to mention the class
+method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
+docs.sweep.dev/tricks). #### Limitations: Sweep is unlikely to complete complex
+issues on the first try, similar to the average junior developer. Here are
+Sweep's limitations(for now): - Try to change less than 200 lines of code - Try
+to modify less than 3 files - Do not include files with more than 1500 lines of
+code ### â¨ Sweep Github App Setting up Sweep is as simple as adding the
+GitHub bot to a repo, then creating an issue for the bot to address. We support
+all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C#
+and C++. 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to
+desired repos 2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py
+use an os-agnostic temp directory" ### ð¥ï¸ Sweep Chat Sweep Chat allows you
+to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
+then have it create the pull request for you. **Prerequisites:** Install [Sweep
+GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
+install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
+run `pip3 install --force-reinstall sweepai && sweep` if the previous command
+fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
+8-digit code from your terminal into the page. You should only need to do the
+authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
+a repository from the dropdown at the top (the Github app must be installed to
+this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
-gradio-screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on
-the right. \n* ð Sweep Chat creates PRs when the "Create PR" button is
-clicked. \n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
-?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the
-latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep &&
-poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python
-3.10+**.\n\n## ð¤ Contributing\n\nContributions are welcome and greatly
-appreciated! For detailed guidelines on how to contribute, please see the
-[CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [ð
-Quickstart](https://docs.sweep.dev/).\n\n## ð Story\n\nWe were frustrated by
-small tickets, like simple bug fixes, annoying refactors, and small features.
-Each task required us to open our IDE to fix simple bugs. So we decided to
-leverage the capabilities of ChatGPT to address this directly in
-GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can
-be parallelized + asynchronous: developers can spin up 10 tickets and Sweep
-will address them all at once.\n\n## ð The Stack\n- GPT-4 32k 0613
-(default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our
-embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep
-Chat\n\n## ðºï¸ Roadmap\nSee [ðºï¸ Roadmap](https://docs.sweep.dev/
-roadmap)\n\n## â­ Star History\n\n[![Star History Chart](https://api.star-
-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/
-#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more
-people hear about us!\n
-                         ***** \n Contributors\n *****
-\n
-                     \n Thank you for your contribution!\n
-\n
-          \n \n_[https://contrib.rocks/image?repo=sweepai/sweep]\n\n
-\n
-                          \n and, of course, Sweep!\n
-\n', 'author': 'Kevin Lu', 'author_email': None, 'maintainer': None,
-'maintainer_email': None, 'url': None, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
+right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
+ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
+#### From Source If you want the nightly build and or if the latest build has
+issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð¤
+Contributing Contributions are welcome and greatly appreciated! For detailed
+guidelines on how to contribute, please see the [CONTRIBUTING.md]
+(CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
+docs.sweep.dev/). ## ð Story We were frustrated by small tickets, like
+simple bug fixes, annoying refactors, and small features. Each task required us
+to open our IDE to fix simple bugs. So we decided to leverage the capabilities
+of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
+this can solve entire tickets and can be parallelized + asynchronous:
+developers can spin up 10 tickets and Sweep will address them all at once. ##
+ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
+with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
+Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap](https://
+docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart](https://
+api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
+history.com/#sweepai/sweep&Date) Consider starring us if you're using Sweep so
+more people hear about us!
+                           ***** Contributors *****
+                       Thank you for your contribution!
+               [https://contrib.rocks/image?repo=sweepai/sweep]
+                            and, of course, Sweep!
```

