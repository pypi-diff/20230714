# Comparing `tmp/sweepai-0.4.7.tar.gz` & `tmp/sweepai-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.7.tar", max compression
+gzip compressed data, was "sweepai-0.4.8.tar", max compression
```

## Comparing `sweepai-0.4.7.tar` & `sweepai-0.4.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.7/LICENSE
--rw-r--r--   0        0        0     7019 2023-07-13 23:38:51.881474 sweepai-0.4.7/README.md
--rw-r--r--   0        0        0     1411 2023-07-14 04:50:07.711330 sweepai-0.4.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.7/sweepai/__init__.py
--rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/api.py
--rw-r--r--   0        0        0     6977 2023-07-14 04:12:55.561425 sweepai-0.4.7/sweepai/app/api_client.py
--rw-r--r--   0        0        0    12755 2023-07-14 03:56:57.223048 sweepai-0.4.7/sweepai/app/backend.py
--rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/app/cli.py
--rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/app/config.py
--rw-r--r--   0        0        0    16697 2023-07-14 04:26:38.459296 sweepai-0.4.7/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.7/sweepai/core/__init__.py
--rw-r--r--   0        0        0    18015 2023-07-13 23:57:23.352400 sweepai-0.4.7/sweepai/core/chat.py
--rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/core/entities.py
--rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.7/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/core/react.py
--rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.7/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.7/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     7146 2023-07-13 23:57:23.352400 sweepai-0.4.7/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.7/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.7/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    19991 2023-07-13 23:38:31.094765 sweepai-0.4.7/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.7/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3822 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.7/sweepai/utils/config/__init__.py
--rw-r--r--   0        0        0     2765 2023-07-14 03:23:31.899309 sweepai-0.4.7/sweepai/utils/config/client.py
--rw-r--r--   0        0        0     3460 2023-07-14 04:49:15.051252 sweepai-0.4.7/sweepai/utils/config/server.py
--rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.7/sweepai/utils/diff.py
--rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8431 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/hash.py
--rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.7/sweepai/utils/utils.py
--rw-r--r--   0        0        0     8239 2023-07-14 04:50:30.235421 sweepai-0.4.7/setup.py
--rw-r--r--   0        0        0     7998 2023-07-14 04:50:30.235885 sweepai-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.8/LICENSE
+-rw-r--r--   0        0        0     7019 2023-07-13 23:38:51.881474 sweepai-0.4.8/README.md
+-rw-r--r--   0        0        0     1411 2023-07-14 17:55:12.308118 sweepai-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/__init__.py
+-rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/api.py
+-rw-r--r--   0        0        0     6977 2023-07-14 04:12:55.561425 sweepai-0.4.8/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    12755 2023-07-14 03:56:57.223048 sweepai-0.4.8/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/app/config.py
+-rw-r--r--   0        0        0    16697 2023-07-14 04:26:38.459296 sweepai-0.4.8/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    18015 2023-07-13 23:57:23.352400 sweepai-0.4.8/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.8/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/react.py
+-rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.8/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     7146 2023-07-13 23:57:23.352400 sweepai-0.4.8/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.8/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.8/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19991 2023-07-13 23:38:31.094765 sweepai-0.4.8/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2761 2023-07-14 17:53:38.131398 sweepai-0.4.8/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3460 2023-07-14 04:49:15.051252 sweepai-0.4.8/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.8/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8431 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     8239 2023-07-14 17:55:15.414130 sweepai-0.4.8/setup.py
+-rw-r--r--   0        0        0     7998 2023-07-14 17:55:15.414584 sweepai-0.4.8/PKG-INFO
```

### Comparing `sweepai-0.4.7/LICENSE` & `sweepai-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/README.md` & `sweepai-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/pyproject.toml` & `sweepai-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.7"
+version = "0.4.8"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.7/sweepai/api.py` & `sweepai-0.4.8/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/app/api_client.py` & `sweepai-0.4.8/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/app/backend.py` & `sweepai-0.4.8/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/app/cli.py` & `sweepai-0.4.8/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/app/config.py` & `sweepai-0.4.8/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/app/ui.py` & `sweepai-0.4.8/sweepai/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/chat.py` & `sweepai-0.4.8/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/code_repair.py` & `sweepai-0.4.8/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/entities.py` & `sweepai-0.4.8/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/gha_extraction.py` & `sweepai-0.4.8/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/prompts.py` & `sweepai-0.4.8/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/react.py` & `sweepai-0.4.8/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/sweep_bot.py` & `sweepai-0.4.8/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/core/vector_db.py` & `sweepai-0.4.8/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/events.py` & `sweepai-0.4.8/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/handlers/create_pr.py` & `sweepai-0.4.8/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.8/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/handlers/on_comment.py` & `sweepai-0.4.8/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/handlers/on_review.py` & `sweepai-0.4.8/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/handlers/on_ticket.py` & `sweepai-0.4.8/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/chat_logger.py` & `sweepai-0.4.8/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/config/client.py` & `sweepai-0.4.8/sweepai/utils/config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,8 +64,8 @@
                 logger.warning(f"Error when getting gha enabled: {e}, falling back to False")
                 return False
         gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8")).get("gha_enabled", False)
         return gha_enabled
 
 # optional, can leave env var blank
 GITHUB_APP_CLIENT_ID = os.environ.get('GITHUB_APP_CLIENT_ID', 'Iv1.91fd31586a926a9f')
-SWEEP_API_ENDPOINT = os.environ.get('SWEEP_API_ENDPOINT', f"https://sweepai--{PREFIX}-ui-dev.modal.run")
+SWEEP_API_ENDPOINT = os.environ.get('SWEEP_API_ENDPOINT', f"https://sweepai--{PREFIX}-ui.modal.run")
```

### Comparing `sweepai-0.4.7/sweepai/utils/config/server.py` & `sweepai-0.4.8/sweepai/utils/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/diff.py` & `sweepai-0.4.8/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/event_logger.py` & `sweepai-0.4.8/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/file_change_functions.py` & `sweepai-0.4.8/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/github_utils.py` & `sweepai-0.4.8/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.8/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/scorer.py` & `sweepai-0.4.8/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/snippets.py` & `sweepai-0.4.8/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/sweepai/utils/utils.py` & `sweepai-0.4.8/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.7/setup.py` & `sweepai-0.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.4.7',
+    'version': '0.4.8',
     'description': 'Sweep software chores',
     'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep\'s limitations(for now):\n- Try to change less than 200 lines of code\n- Try to modify less than 3 files\n- Do not include files with more than 1500 lines of code\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 💰 Pricing\n* We charge $120/month for 60 GPT4 tickets per month.\n* For unpaid users, we offer 3 free GPT4 tickets per month.\n* We also offer unlimited GPT3.5 tickets.\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils',
 'sweepai.utils.config'] package_data = \ {'': ['*']} install_requires = \
 ['GitPython>=3.1.31,<4.0.0', 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0',
 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'pyyaml>=6.0,<7.0',
 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
 'urllib3<2.0.0'] entry_points = \ {'console_scripts': ['sweep =
 sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.4.7', 'description': 'Sweep software
+{ 'name': 'sweepai', 'version': '0.4.8', 'description': 'Sweep software
 chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
```

### Comparing `sweepai-0.4.7/PKG-INFO` & `sweepai-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.7
+Version: 0.4.8
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
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.7 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.8 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
```

