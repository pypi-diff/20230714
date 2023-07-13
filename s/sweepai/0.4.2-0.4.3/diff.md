# Comparing `tmp/sweepai-0.4.2.tar.gz` & `tmp/sweepai-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.2.tar", max compression
+gzip compressed data, was "sweepai-0.4.3.tar", max compression
```

## Comparing `sweepai-0.4.2.tar` & `sweepai-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.2/LICENSE
--rw-r--r--   0        0        0     6847 2023-07-13 00:07:11.929593 sweepai-0.4.2/README.md
--rw-r--r--   0        0        0     1395 2023-07-13 00:08:34.469618 sweepai-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/__init__.py
--rw-r--r--   0        0        0    12248 2023-07-11 20:05:05.034619 sweepai-0.4.2/sweepai/api.py
--rw-r--r--   0        0        0     6020 2023-07-11 09:20:00.556075 sweepai-0.4.2/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10421 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/app/backend.py
--rw-r--r--   0        0        0     1166 2023-07-09 08:40:46.465379 sweepai-0.4.2/sweepai/app/cli.py
--rw-r--r--   0        0        0     3563 2023-07-13 00:08:02.099608 sweepai-0.4.2/sweepai/app/config.py
--rw-r--r--   0        0        0    14559 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17835 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/core/chat.py
--rw-r--r--   0        0        0     2867 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8306 2023-07-11 20:16:30.901906 sweepai-0.4.2/sweepai/core/entities.py
--rw-r--r--   0        0        0      561 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16809 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/core/react.py
--rw-r--r--   0        0        0    20567 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12695 2023-07-09 08:40:46.468712 sweepai-0.4.2/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3176 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     6715 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2571 2023-07-11 09:19:39.419375 sweepai-0.4.2/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9645 2023-07-13 00:07:11.929593 sweepai-0.4.2/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.4.2/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    19731 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3786 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0     2269 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/config.py
--rw-r--r--   0        0        0     1131 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/constants.py
--rw-r--r--   0        0        0     6525 2023-07-13 00:07:11.932927 sweepai-0.4.2/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.4.2/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8225 2023-07-09 08:40:46.468712 sweepai-0.4.2/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.4.2/sweepai/utils/utils.py
--rw-r--r--   0        0        0     8021 2023-07-13 00:10:09.537208 sweepai-0.4.2/setup.py
--rw-r--r--   0        0        0     7799 2023-07-13 00:10:09.537661 sweepai-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6847 2023-07-13 00:29:33.520020 sweepai-0.4.3/README.md
+-rw-r--r--   0        0        0     1411 2023-07-13 22:31:22.984130 sweepai-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/__init__.py
+-rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/api.py
+-rw-r--r--   0        0        0     6417 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10697 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/app/config.py
+-rw-r--r--   0        0        0    15368 2023-07-13 22:30:25.187445 sweepai-0.4.3/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17965 2023-07-13 22:20:26.747256 sweepai-0.4.3/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.3/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/react.py
+-rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.3/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     6839 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19986 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.3/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.3/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2759 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3460 2023-07-13 07:19:30.090833 sweepai-0.4.3/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.3/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8431 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.3/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     8063 2023-07-13 22:31:57.446699 sweepai-0.4.3/setup.py
+-rw-r--r--   0        0        0     7826 2023-07-13 22:31:57.447146 sweepai-0.4.3/PKG-INFO
```

### Comparing `sweepai-0.4.2/LICENSE` & `sweepai-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.2/README.md` & `sweepai-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.2/pyproject.toml` & `sweepai-0.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.2"
+version = "0.4.3"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -15,20 +15,21 @@
 "Bug Tracker" = "https://github.com/sweepai/sweep/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyGithub = "1.58.2"
 loguru = "^0.6.0"
 requests = "^2.28.2"
-urllib3 = "^2.0.3"
+urllib3 = "<2.0.0"
 gradio = "^3.35.2"
 config-path = "^1.0.3"
 typer = "^0.9.0"
 tabulate = "^0.9.0"
 GitPython = "^3.1.31"
+pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 commit5 = "^0.1.1"
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 build = "^0.10.0"
```

### Comparing `sweepai-0.4.2/sweepai/api.py` & `sweepai-0.4.3/sweepai/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-import time
-from loguru import logger
 import modal
+from fastapi import HTTPException, Request
+from loguru import logger
 from pydantic import ValidationError
-from sweepai.handlers.create_pr import create_pr
-from sweepai.handlers.on_check_suite import on_check_suite  # type: ignore
 
-from sweepai.handlers.on_ticket import on_ticket
-from sweepai.handlers.on_comment import on_comment
-from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, LABEL_COLOR, LABEL_DESCRIPTION, LABEL_NAME, SWEEP_LOGIN
 from sweepai.events import (
     CheckRunCompleted,
     CommentCreatedRequest,
     InstallationCreatedRequest,
     IssueCommentRequest,
     IssueRequest,
     PRRequest,
     ReposAddedRequest,
 )
+from sweepai.handlers.create_pr import create_pr  # type: ignore
+from sweepai.handlers.on_check_suite import on_check_suite  # type: ignore
+from sweepai.handlers.on_comment import on_comment
+from sweepai.handlers.on_ticket import on_ticket
+from sweepai.utils.config.server import DB_MODAL_INST_NAME, API_MODAL_INST_NAME, GITHUB_BOT_USERNAME, \
+    GITHUB_LABEL_NAME, GITHUB_LABEL_COLOR, GITHUB_LABEL_DESCRIPTION, BOT_TOKEN_NAME
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, index_full_repository
-from fastapi import HTTPException, Request
-
-from pymongo import MongoClient
 
-stub = modal.Stub(API_NAME)
+stub = modal.Stub(API_MODAL_INST_NAME)
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
     .pip_install(
         "openai",
         "anthropic",
         "PyGithub",
@@ -42,34 +40,35 @@
         "pyyaml",
         "pymongo",
         "tabulate"
     )
 )
 secrets = [
     modal.Secret.from_name(BOT_TOKEN_NAME),
+    modal.Secret.from_name("github"),
     modal.Secret.from_name("openai-secret"),
     modal.Secret.from_name("anthropic"),
     modal.Secret.from_name("posthog"),
     modal.Secret.from_name("highlight"),
     modal.Secret.from_name("mongodb"),
     modal.Secret.from_name("discord")
 ]
 
 FUNCTION_SETTINGS = {
     "image": image,
     "secrets": secrets,
     "timeout": 30 * 60,
 }
 
-
 handle_ticket = stub.function(**FUNCTION_SETTINGS)(on_ticket)
 handle_comment = stub.function(**FUNCTION_SETTINGS)(on_comment)
 handle_pr = stub.function(**FUNCTION_SETTINGS)(create_pr)
+update_index = modal.Function.lookup(DB_MODAL_INST_NAME, "update_index")
 handle_check_suite = stub.function(**FUNCTION_SETTINGS)(on_check_suite)
-update_index = modal.Function.lookup(DB_NAME, "update_index")
+
 
 @stub.function(**FUNCTION_SETTINGS)
 @modal.web_endpoint(method="POST")
 async def webhook(raw_request: Request):
     """Handle a webhook request from GitHub."""
     try:
         request_dict = await raw_request.json()
@@ -83,37 +82,37 @@
                 if issue_title_lower.startswith("sweep") or "sweep:" in issue_title_lower:
                     g = get_github_client(request.installation.id)
                     repo = g.get_repo(request.repository.full_name)
 
                     labels = repo.get_labels()
                     label_names = [label.name for label in labels]
 
-                    if LABEL_NAME not in label_names:
+                    if GITHUB_LABEL_NAME not in label_names:
                         repo.create_label(
-                            name=LABEL_NAME,
-                            color=LABEL_COLOR,
-                            description=LABEL_DESCRIPTION,
+                            name=GITHUB_LABEL_NAME,
+                            color=GITHUB_LABEL_COLOR,
+                            description=GITHUB_LABEL_DESCRIPTION,
                         )
                     # TODO(sweep): figure out why this is breaking
                     # else:
                     #     label = repo.get_label(LABEL_NAME)
                     #     label.edit(
                     #         name=LABEL_NAME,
                     #         color=LABEL_COLOR, 
                     #         description=LABEL_DESCRIPTION
                     #     )
-                    
+
                     current_issue = repo.get_issue(number=request.issue.number)
-                    current_issue.add_to_labels(LABEL_NAME)
+                    current_issue.add_to_labels(GITHUB_LABEL_NAME)
             case "issues", "labeled":
                 request = IssueRequest(**request_dict)
-                if 'label' in request_dict and str.lower(request_dict['label']['name']) == LABEL_NAME:
+                if 'label' in request_dict and str.lower(request_dict['label']['name']) == GITHUB_LABEL_NAME:
                     request.issue.body = request.issue.body or ""
                     request.repository.description = (
-                        request.repository.description or ""
+                            request.repository.description or ""
                     )
                     # Update before we handle the ticket to make sure index is up to date
                     # other ways suboptimal
                     handle_ticket.spawn(
                         request.issue.title,
                         request.issue.body,
                         request.issue.number,
@@ -124,22 +123,22 @@
                         request.installation.id,
                         None
                     )
             case "issue_comment", "created":
                 request = IssueCommentRequest(**request_dict)
                 # if replying to an issue with sweep label
                 if request.issue is not None \
-                    and "sweep" in [label.name.lower() for label in request.issue.labels] \
-                    and request.comment.user.type == "User":
+                        and GITHUB_LABEL_NAME in [label.name.lower() for label in request.issue.labels] \
+                        and request.comment.user.type == "User":
                     request.issue.body = request.issue.body or ""
                     request.repository.description = (
-                        request.repository.description or ""
+                            request.repository.description or ""
                     )
 
-                    if not request.comment.body.lower().startswith("sweep"):
+                    if not request.comment.body.lower().startswith(GITHUB_LABEL_NAME):
                         return {"success": True, "reason": "Comment does not start with 'Sweep', passing"}
 
                     # Update before we handle the ticket to make sure index is up to date
                     # other ways suboptimal
                     handle_ticket.spawn(
                         request.issue.title,
                         request.issue.body,
@@ -147,16 +146,15 @@
                         request.issue.html_url,
                         request.issue.user.login,
                         request.repository.full_name,
                         request.repository.description,
                         request.installation.id,
                         request.comment.id
                     )
-                # if replying to a pr created by Sweep
-                elif request.issue.pull_request and request.issue.user.login == SWEEP_LOGIN and request.comment.user.type == "User": # TODO(sweep): set a limit                    
+                elif request.issue.pull_request and request.issue.user.login == GITHUB_BOT_USERNAME and request.comment.user.type == "User":  # TODO(sweep): set a limit
                     logger.info(f"Handling comment on PR: {request.issue.pull_request}")
                     handle_comment.spawn(
                         repo_full_name=request.repository.full_name,
                         repo_description=request.repository.description,
                         comment=request.comment.body,
                         pr_path=None,
                         pr_line_position=None,
@@ -179,18 +177,18 @@
                     )
                 # Todo: update index on comments
             case "pull_request_review", "submitted":
                 # request = ReviewSubmittedRequest(**request_dict)
                 pass
             case "check_run", "completed":
                 request = CheckRunCompleted(**request_dict)
-                    # handle_check_suite
+                # handle_check_suite
                 logs = None
                 # Must be Sweep firing the PR and it must fail
-                if request.sender.login == SWEEP_LOGIN and request.check_run.conclusion == "failure": 
+                if request.sender.login == GITHUB_BOT_USERNAME and request.check_run.conclusion == "failure":
                     logs = handle_check_suite.call(request)
                 if len(request.check_run.pull_requests) > 0 and logs:
                     handle_comment.spawn(
                         repo_full_name=request.repository.full_name,
                         repo_description=request.repository.description,
                         comment="Sweep: " + logs,
                         pr_path=None,
@@ -234,24 +232,24 @@
                         installation_id=repos_added_request.installation.id,
                     )
             case ("pull_request", "closed"):
                 pr_request = PRRequest(**request_dict)
                 organization, repo_name = pr_request.repository.full_name.split("/")
                 commit_author = pr_request.pull_request.user.login
                 merged_by = pr_request.pull_request.merged_by.login
-                if SWEEP_LOGIN == commit_author:
+                if GITHUB_BOT_USERNAME == commit_author:
                     posthog.capture(
-                        merged_by, 
-                        "merged_sweep_pr", 
+                        merged_by,
+                        "merged_sweep_pr",
                         properties={
                             "repo_name": repo_name,
                             "organization": organization,
                             "repo_full_name": pr_request.repository.full_name,
                             "username": merged_by
-                    })
+                        })
                 update_index.spawn(
                     request_dict["repository"]["full_name"],
                     installation_id=request_dict["installation"]["id"],
                 )
             case ("push", None):
                 if event != "pull_request" or request_dict["base"]["merged"] == True:
                     update_index.spawn(
```

### Comparing `sweepai-0.4.2/sweepai/app/api_client.py` & `sweepai-0.4.3/sweepai/app/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Any
+import json
 import webbrowser
+from typing import Any
+
 import httpx
-from pydantic import BaseModel
 import requests
-import json
 from loguru import logger
+from pydantic import BaseModel
 
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.entities import Function, PullRequest, Snippet
-from sweepai.utils.constants import PREFIX
+from sweepai.utils.config.client import GITHUB_APP_CLIENT_ID, SWEEP_API_ENDPOINT
 
 create_pr_function = Function(
     name="create_pr",
     description="Creates a PR.",
     parameters={
         "properties": {
             "plan": {
@@ -23,15 +24,15 @@
                         "file_path": {
                             "type": "string",
                             "description": "The file path to change."
                         },
                         "instructions": {
                             "type": "string",
                             "description": "Concise NATURAL LANGUAGE summary of what to change in each file. There should be absolutely NO code, only English.",
-                            "example":  [
+                            "example": [
                                 "Refactor the algorithm by moving the main function to the top of the file.",
                                 "Change the implementation to recursion"
                             ]
                         },
                     },
                     "required": ["file_path", "instructions"]
                 },
@@ -52,14 +53,15 @@
         },
         "required": ["plan", "title", "summary", "branch"]
     }
 )
 
 create_pr_function_call = {"name": "create_pr"}
 
+
 def break_json(raw_json: str):
     # turns something like {"function_call": {"arguments": " \""}}{"function_call": {"arguments": "summary"}} into two objects
     try:
         yield json.loads(raw_json)
     except json.JSONDecodeError:
         for i in range(1, len(raw_json)):
             try:
@@ -67,107 +69,115 @@
                 yield obj
                 for item in break_json(raw_json[i:]):
                     yield item
                 break
             except json.JSONDecodeError:
                 pass
 
+
 class APIClient(BaseModel):
     config: SweepChatConfig
-    api_endpoint: str = f"https://sweepai--{PREFIX}-ui.modal.run"
+    api_endpoint = SWEEP_API_ENDPOINT
+
+    def __init__(self, config: SweepChatConfig):
+        super().__init__(config=config)
+        self.config = config
+        logger.info(f"Initializing API client")
+        logger.info(f"API endpoint: {self.api_endpoint}")
+        logger.info(f"Github APP Client ID: {GITHUB_APP_CLIENT_ID}")
 
     def get_installation_id(self):
         results = requests.post(
             self.api_endpoint + "/installation_id",
-            json= self.config.dict(),
+            json=self.config.dict(),
         )
         if results.status_code == 401:
             print("Installation ID not found! Please install sweep first.")
             webbrowser.open_new_tab("https://github.com/apps/sweep-ai")
             raise Exception(results.json()["detail"])
         if results.status_code != 200:
             raise Exception(results.json()["detail"])
         obj = results.json()
         return obj["installation_id"]
 
     def search(
-        self,
-        query: str,
-        n_results: int = 5,
+            self,
+            query: str,
+            n_results: int = 5,
     ):
         results = requests.post(
             self.api_endpoint + "/search",
             json={
                 "query": query,
                 "n_results": n_results,
                 "config": self.config.dict(),
             }
         )
         if results.status_code != 200:
             raise Exception(results.text)
         snippets = [Snippet(**item) for item in results.json()]
         return snippets
-    
+
     def create_pr(
-        self,
-        file_change_requests: list[tuple[str, str]],
-        pull_request: PullRequest,
-        messages: list[tuple[str | None, str | None]],
+            self,
+            file_change_requests: list[tuple[str, str]],
+            pull_request: PullRequest,
+            messages: list[tuple[str | None, str | None]],
     ):
         results = requests.post(
             self.api_endpoint + "/create_pr",
             json={
                 "file_change_requests": file_change_requests,
                 "pull_request": pull_request,
                 "messages": messages,
                 "config": self.config.dict(),
             },
             timeout=10 * 60
         )
         return results.json()
-    
+
     def chat(
-        self, 
-        messages: list[tuple[str | None, str | None]],
-        snippets: list[Snippet] = [],
-        model: str = "gpt-4-0613",
+            self,
+            messages: list[tuple[str | None, str | None]],
+            snippets: list[Snippet] = [],
+            model: str = "gpt-4-0613",
     ) -> str:
         results = requests.post(
             self.api_endpoint + "/chat",
             json={
                 "messages": messages,
                 "snippets": [snippet.dict() for snippet in snippets],
                 "config": self.config.dict()
             }
         )
         return results.json()
-    
+
     def stream_chat(
-        self, 
-        messages: list[tuple[str | None, str | None]], 
-        snippets: list[Snippet] = [],
-        functions: list[Function] = [],
-        function_call: Any = "auto",
-        model: str = "gpt-4-0613"
+            self,
+            messages: list[tuple[str | None, str | None]],
+            snippets: list[Snippet] = [],
+            functions: list[Function] = [],
+            function_call: Any = "auto",
+            model: str = "gpt-4-0613"
     ):
-        with httpx.Client(timeout=30) as client: # sometimes this step is slow
+        with httpx.Client(timeout=30) as client:  # sometimes this step is slow
             with client.stream(
-                'POST', 
-                self.api_endpoint + '/chat_stream',
-                json={
-                    "messages": messages,
-                    "snippets": [snippet.dict() for snippet in snippets],
-                    "do_add_plan": True,
-                    "functions": [func.dict() for func in functions],
-                    "function_call": function_call,
-                    "config": self.config.dict()
-                }
+                    'POST',
+                    self.api_endpoint + '/chat_stream',
+                    json={
+                        "messages": messages,
+                        "snippets": [snippet.dict() for snippet in snippets],
+                        "do_add_plan": True,
+                        "functions": [func.dict() for func in functions],
+                        "function_call": function_call,
+                        "config": self.config.dict()
+                    }
             ) as response:
                 for delta_chunk in response.iter_text():
                     if not delta_chunk:
                         break
                     try:
                         for item in break_json(delta_chunk):
                             yield item
-                    except json.decoder.JSONDecodeError as e: 
+                    except json.decoder.JSONDecodeError as e:
                         logger.error(delta_chunk)
                         raise e
```

### Comparing `sweepai-0.4.2/sweepai/app/backend.py` & `sweepai-0.4.3/sweepai/app/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Proxy for the UI.
 """
 
 import json
 from typing import Any
+
 import fastapi
-from github import Github
 import modal
-from loguru import logger
 from fastapi import FastAPI
 from fastapi.responses import StreamingResponse
+from github import Github
+from loguru import logger
 from pydantic import BaseModel
 
 from sweepai.app.config import SweepChatConfig
-from sweepai.utils.config import SweepConfig
-from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, PREFIX
-from sweepai.utils.github_utils import get_github_client, get_installation_id
-from sweepai.utils.event_logger import posthog
 from sweepai.core.chat import ChatGPT
 from sweepai.core.entities import FileChangeRequest, Function, Message, PullRequest, Snippet
-from sweepai.core.sweep_bot import SweepBot
 from sweepai.core.prompts import gradio_system_message_prompt, gradio_user_prompt
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.utils.config.client import SweepConfig
+from sweepai.utils.config.server import PREFIX, DB_MODAL_INST_NAME, API_MODAL_INST_NAME, BOT_TOKEN_NAME
+from sweepai.utils.event_logger import posthog
+from sweepai.utils.github_utils import get_github_client, get_installation_id
 
-get_relevant_snippets = modal.Function.from_name(DB_NAME, "get_relevant_snippets")
+get_relevant_snippets = modal.Function.from_name(DB_MODAL_INST_NAME, "get_relevant_snippets")
 
 stub = modal.Stub(PREFIX + "-ui")
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
     .pip_install(
         "loguru",
@@ -40,26 +41,28 @@
         "config-path",
         "pyyaml",
         "pymongo",
     )
 )
 secrets = [
     modal.Secret.from_name(BOT_TOKEN_NAME),
+    modal.Secret.from_name("github"),
     modal.Secret.from_name("openai-secret"),
     modal.Secret.from_name("posthog"),
     modal.Secret.from_name("highlight")
 ]
 
 FUNCTION_SETTINGS = {
     "image": image,
     "secrets": secrets,
     "timeout": 15 * 60,
     "keep_warm": 1
 }
 
+
 @stub.function(**FUNCTION_SETTINGS)
 @modal.asgi_app(label=PREFIX + "-ui")
 def _asgi_app():
     app = FastAPI()
 
     def verify_config(request: SweepChatConfig) -> bool:
         try:
@@ -90,29 +93,30 @@
         try:
             organization, _repo_name = request.repo_full_name.split("/")
             installation_id = get_installation_id(organization)
             assert installation_id
         except Exception as e:
             logger.warning(e)
             posthog.capture(request.github_username, "failed", properties={"error": str(e), **metadata})
-            raise fastapi.HTTPException(status_code=403, detail="Sweep app is not installed on this repo. To install it, go to https://github.com/apps/sweep-ai")
+            raise fastapi.HTTPException(status_code=403,
+                                        detail="Sweep app is not installed on this repo. To install it, go to https://github.com/apps/sweep-ai")
 
         posthog.capture(request.github_username, "success", properties=metadata)
 
         return {"installation_id": installation_id}
 
     class SearchRequest(BaseModel):
         query: str
         config: SweepChatConfig
         n_results: int = 5
 
     @app.post("/search")
     def search(request: SearchRequest) -> list[Snippet]:
         logger.info("Searching for snippets...")
-        get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
+        get_relevant_snippets = modal.Function.lookup(DB_MODAL_INST_NAME, "get_relevant_snippets")
 
         assert verify_config(request.config)
 
         metadata = {
             "function": "ui_search",
             "repo_full_name": request.config.repo_full_name,
             "organization": request.config.repo_full_name.split("/")[0],
@@ -130,35 +134,36 @@
                 n_results=request.n_results,
                 installation_id=request.config.installation_id
             )
             g = get_github_client(request.config.installation_id)
             repo = g.get_repo(request.config.repo_full_name)
             for snippet in snippets:
                 try:
-                    snippet.content = repo.get_contents(snippet.file_path, SweepConfig.get_branch(repo)).decoded_content.decode("utf-8")
+                    snippet.content = repo.get_contents(snippet.file_path,
+                                                        SweepConfig.get_branch(repo)).decoded_content.decode("utf-8")
                 except Exception:
                     logger.error(snippet)
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
 
         posthog.capture(request.config.github_username, "success", properties=metadata)
         return snippets
 
     class CreatePRRequest(BaseModel):
         # proposed PR information
         file_change_requests: list[tuple[str, str]]
-        pull_request: PullRequest 
+        pull_request: PullRequest
 
         # state information
         messages: list[tuple[str | None, str | None]]
         snippets: list[Snippet] = []
 
         config: SweepChatConfig
-    
+
     @app.post("/create_pr")
     def create_pr(request: CreatePRRequest):
         assert verify_config(request.config)
 
         g = get_github_client(request.config.installation_id)
         repo = g.get_repo(request.config.repo_full_name)
 
@@ -170,77 +175,78 @@
             "installation_id": request.config.installation_id,
             "mode": PREFIX,
         }
 
         posthog.capture(request.config.github_username, "started", properties=metadata)
 
         try:
-            create_pr_func = modal.Function.lookup(API_NAME, "create_pr")
+            create_pr_func = modal.Function.lookup(API_MODAL_INST_NAME, "create_pr")
             system_message = gradio_system_message_prompt.format(
-                snippets="\n".join([snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
+                snippets="\n".join(
+                    [snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
                 repo_name=request.config.repo_full_name,
                 repo_description=repo.description
             )
 
             def file_exists(file_path: str) -> bool:
                 try:
                     repo.get_contents(file_path, SweepConfig.get_branch(repo))
                     return True
                 except Exception:
                     return False
 
             results = create_pr_func.call(
                 [FileChangeRequest(
-                    filename = item[0],
-                    instructions = item[1],
-                    change_type = "modify" if file_exists(item[0]) else "create", # TODO update this
+                    filename=item[0],
+                    instructions=item[1],
+                    change_type="modify" if file_exists(item[0]) else "create",  # TODO update this
                 ) for item in request.file_change_requests],
                 request.pull_request,
                 SweepBot(
-                    repo = repo,
-                    messages = [Message(role="system", content=system_message, key="system")] +
-                        [Message.from_tuple(message) for message in request.messages],
+                    repo=repo,
+                    messages=[Message(role="system", content=system_message, key="system")] +
+                             [Message.from_tuple(message) for message in request.messages],
                 ),
                 request.config.github_username,
-                installation_id = request.config.installation_id,
-                issue_number = None,
+                installation_id=request.config.installation_id,
+                issue_number=None,
             )
             generated_pull_request = results["pull_request"]
             print(generated_pull_request)
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={
                 "error": str(e),
                 **metadata
             })
             raise e
 
         posthog.capture(request.config.github_username, "success", properties=metadata)
         return {
             "html_url": generated_pull_request.html_url,
         }
-    
+
     class ChatRequest(BaseModel):
         messages: list[tuple[str | None, str | None]]
         snippets: list[Snippet]
         config: SweepChatConfig
         do_add_plan: bool = False
         functions: list[Function] = []
         function_call: Any = "auto"
 
     @app.post("/chat")
     def chat(
-        request: ChatRequest,
+            request: ChatRequest,
     ) -> str:
         assert verify_config(request.config)
 
         messages = [Message.from_tuple(message) for message in request.messages]
         chatgpt = ChatGPT(messages=messages[:-1])
         result = chatgpt.chat(messages[-1].content, model="gpt-4-0613")
         return result
-    
+
     @app.post("/chat_stream")
     def chat_stream(request: ChatRequest):
         assert verify_config(request.config)
         metadata = {
             "function": "ui_chat_stream",
             "repo_full_name": request.config.repo_full_name,
             "organization": request.config.repo_full_name.split("/")[0],
@@ -249,26 +255,31 @@
             "mode": PREFIX,
         }
 
         posthog.capture(request.config.github_username, "started", properties=metadata)
         try:
             messages = [Message.from_tuple(message) for message in request.messages]
             system_message = gradio_system_message_prompt.format(
-                snippets="\n".join([snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
+                snippets="\n".join(
+                    [snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
                 repo_name=request.config.repo_full_name,
-                repo_description="" # TODO: fill this
+                repo_description=""  # TODO: fill this
             )
             chatgpt = ChatGPT(messages=[Message(role="system", content=system_message, key="system")] + messages[:-1])
             if request.do_add_plan:
                 chatgpt.messages[-1].content += gradio_user_prompt
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
+
         def stream_chat():
-            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions, function_call=request.function_call):
+            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions,
+                                             function_call=request.function_call):
                 yield json.dumps(chunk)
             posthog.capture(request.config.github_username, "success", properties=metadata)
+
         return StreamingResponse(
             stream_chat(),
             media_type="text/event-stream"
         )
+
     return app
```

### Comparing `sweepai-0.4.2/sweepai/app/cli.py` & `sweepai-0.4.3/sweepai/app/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 
 from sweepai.app.config import SweepChatConfig
 
 epilog = "Sweep is a AI junior developer. Docs at https://docs.sweep.dev, install at https://github.com/apps/sweep-ai and support at https://discord.gg/sweep-ai."
 
 typer_app = typer.Typer(epilog=epilog)
 
+
 # @app.callback()
 @typer_app.command()
 def start():
     """
     Launch Sweep Chat in the browser
     """
     SweepChatConfig.load()
     from sweepai.app.ui import demo
     print("\033[93m⭐ Remember to star our repo at https://github.com/sweepai/sweep! \033[0m")
     demo.queue()
     demo.launch(inbrowser=True)
-    
+
+
 @typer_app.command()
 def auth():
     """
     Reauthenticate with Github API for Sweep to work (for token expiry)
     """
     SweepChatConfig.load(recreate=True)
     print("Setup completed successfully!")
     print("\033[93m⭐ Remember to star our repo at https://github.com/sweepai/sweep! \033[0m")
 
+
 def app():
     # hacky solution based on https://github.com/tiangolo/typer/issues/18#issuecomment-1577788949
     import sys
     commands = {'start', 'auth'}
     sys.argv.append('start') if sys.argv[-1] not in commands else None
     typer_app()
 
+
 if __name__ == "__main__":
-    app()
+    app()
```

### Comparing `sweepai-0.4.2/sweepai/app/config.py` & `sweepai-0.4.3/sweepai/app/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 from __future__ import annotations
 
 import os
 import time
-import requests
-from urllib.parse import parse_qs, unquote
 import webbrowser
+from urllib.parse import parse_qs, unquote
 
+import requests
+import yaml
 from config_path import ConfigPath
 from pydantic import BaseModel
-import yaml
 
-CLIENT_ID = "Iv1.91fd31586a926a9f"
+from sweepai.utils.config.client import GITHUB_APP_CLIENT_ID
 
 DEVICE_CODE_ENDPOINT = "https://github.com/login/device/code"
 USER_LOGIN_ENDPOINT = "https://github.com/login/device"
 OAUTH_ACCESS_TOKEN_ENDPOINT = "https://github.com/login/oauth/access_token"
 
-config_path = ConfigPath( 'sweep_chat', 'sweep', '.yaml' )
+config_path = ConfigPath('sweep_chat', 'sweep', '.yaml')
 CONFIG_FILE = config_path.saveFilePath()
 
+
 class State(BaseModel):
     file_paths: list[str] = []
     chat_history: list[tuple[str | None, str | None]] = []
     snippets_text: str = "### Relevant Snippets:"
     plan: list[tuple[str, str]] = []
 
+
 class SweepChatConfig(BaseModel):
     github_username: str
-    github_pat: str # secret
+    github_pat: str  # secret
     repo_full_name: str | None = None
     installation_id: int | None = None
     state: State = State()
     version: str = "0.0.2"
 
     @classmethod
     def create(cls):
-        device_code_response = requests.post(DEVICE_CODE_ENDPOINT, json={"client_id": CLIENT_ID})
+        device_code_response = requests.post(DEVICE_CODE_ENDPOINT, json={"client_id": GITHUB_APP_CLIENT_ID})
         parsed_device_code_response = parse_qs(unquote(device_code_response.text))
         print("\033[93m" + f"Open {USER_LOGIN_ENDPOINT} if it doesn't open automatically." + "\033[0m")
         print("\033[93m" + f"Paste the following code (copied to your clipboard) and click authorize:" + "\033[0m")
-        print("\033[94m" + parsed_device_code_response["user_code"][0] + "\033[0m") # prints in blue
-        print("\033[93m" + "Once you've authorized, ** just wait a few seconds **..." + "\033[0m") # prints in yellow
+        print("\033[94m" + parsed_device_code_response["user_code"][0] + "\033[0m")  # prints in blue
+        print("\033[93m" + "Once you've authorized, ** just wait a few seconds **..." + "\033[0m")  # prints in yellow
         time.sleep(3)
         webbrowser.open_new_tab(USER_LOGIN_ENDPOINT)
         for _ in range(10):
             time.sleep(5.5)
             try:
                 oauth_access_token_response = requests.post(
                     OAUTH_ACCESS_TOKEN_ENDPOINT,
                     json={
-                        "client_id": CLIENT_ID,
+                        "client_id": GITHUB_APP_CLIENT_ID,
                         "device_code": parsed_device_code_response["device_code"][0],
                         "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
                     }
                 )
                 oauth_access_token_response = parse_qs(unquote(oauth_access_token_response.text))
                 access_token = oauth_access_token_response["access_token"][0]
                 assert access_token
@@ -66,31 +68,31 @@
             "https://api.github.com/user",
             headers={
                 "Accept": "application/vnd.github+json",
                 "Authorization": f"Bearer {access_token}",
             }
         )
 
-        print("\033[92m" + f"Logged in successfully as {username_response.json()['login']}" + "\033[0m") # prints in green
+        print(
+            "\033[92m" + f"Logged in successfully as {username_response.json()['login']}" + "\033[0m")  # prints in green
 
         return cls(
             github_username=username_response.json()["login"],
             github_pat=access_token
         )
-    
+
     def save(self):
         with open(CONFIG_FILE, "w") as f:
             yaml.dump(self.dict(), f)
-    
+
     @staticmethod
     def is_initialized() -> bool:
         return os.path.exists(CONFIG_FILE)
-    
+
     @classmethod
     def load(cls, recreate=False) -> SweepChatConfig:
         if recreate or not SweepChatConfig.is_initialized():
             config = cls.create()
             config.save()
             return config
         with open(CONFIG_FILE, "r") as f:
             return cls(**yaml.load(f, Loader=yaml.FullLoader))
-
```

### Comparing `sweepai-0.4.2/sweepai/app/ui.py` & `sweepai-0.4.3/sweepai/app/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import os
-import re
+import shutil
 import tempfile
+import re
+
+import gradio as gr
 from git import Repo
 from github import Github
-import gradio as gr
 from loguru import logger
-import shutil
 
 from sweepai.app.api_client import APIClient, create_pr_function, create_pr_function_call
 from sweepai.app.config import State, SweepChatConfig
 from sweepai.core.entities import Snippet
-from sweepai.utils.config import SweepConfig
+from sweepai.utils.config.client import SweepConfig
 
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
 pr_summary_template = '''⏳ I'm creating the following PR...
 
@@ -45,14 +46,15 @@
     overflow-y: scroll;
 }
 #message_box > label > span {
     display: none;
 }
 '''
 
+
 def get_files_recursively(root_path, path=''):
     files = []
     path_to_contents = {}
 
     if path == '.git':
         return files, path_to_contents
 
@@ -74,21 +76,25 @@
         elif os.path.isdir(entry_path):
             subfiles, subpath_to_contents = get_files_recursively(root_path, os.path.join(path, entry))
             files.extend(subfiles)
             path_to_contents.update(subpath_to_contents)
 
     return files, path_to_contents
 
+
 def get_installation_id(repo_full_name):
     config.repo_full_name = repo_full_name
     api_client.config = config
     installation_id = api_client.get_installation_id()
     return installation_id
 
+
 path_to_contents = {}
+
+
 def get_files(repo_full_name):
     global path_to_contents
     global repo
     if repo_full_name is None:
         all_files = []
     else:
         # Make sure repo is added to Sweep before checking all recursive files
@@ -113,42 +119,48 @@
             shutil.rmtree(repo_dir)
             git_repo = Repo.clone_from(repo_url, repo_dir)
             git_repo.git.checkout(branch_name)
             git_repo.remotes.origin.pull()
         all_files, path_to_contents = get_files_recursively(repo_dir)
     return all_files
 
+
 def get_files_update(*args):
     global repo
     if len(args) > 0:
         repo = args[0]
     else:
         repo = config.repo_full_name
     return gr.Dropdown.update(choices=get_files(repo))
 
+
 def parse_response(raw_response: str) -> tuple[str, list[tuple[str, str]]]:
     if "Plan:" not in raw_response:
         response, raw_plan = raw_response, ""
     else:
         response, raw_plan = raw_response.split("Plan:", 1)
     if response.startswith("Response:"):
         response = response[len("Response:"):]
-    plan = [(line[:line.find(":")].strip(), line[line.find(":") + 1:].strip()) for line in raw_plan.split("\n*") if line]
+    plan = [(line[:line.find(":")].strip(), line[line.find(":") + 1:].strip()) for line in raw_plan.split("\n*") if
+            line]
     return response, plan
 
+
 global_state = config.state
 
 with gr.Blocks(theme=gr.themes.Soft(), title="Sweep Chat", css=css) as demo:
     print("Launching gradio!")
     with gr.Row():
         with gr.Column(scale=2):
-            repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=lambda: config.repo_full_name or "")
+            repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name",
+                                         value=lambda: config.repo_full_name or "")
         print("Indexing files...")
         with gr.Column(scale=4):
-            file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files", value=lambda: global_state.file_paths)
+            file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files",
+                                     value=lambda: global_state.file_paths)
         print("Indexed files!")
         repo_full_name.change(get_files_update, repo_full_name, file_names)
         with gr.Column(scale=1):
             restart_button = gr.Button("Restart")
 
     with gr.Row():
         with gr.Column(scale=2):
@@ -156,41 +168,44 @@
         with gr.Column():
             with gr.Row():
                 snippets_text = gr.Markdown(value=lambda: global_state.snippets_text, elem_id="snippets")
 
     with gr.Row():
         plan = gr.List(
             value=[[filename + ": " + instructions] for filename, instructions in global_state.plan],
-            headers=["Proposed Plan"], 
+            headers=["Proposed Plan"],
             interactive=True,
             col_count=(1, "static"),
             wrap=True
         )
-    
+
     with gr.Row():
         with gr.Column(scale=8):
             msg = gr.Textbox(placeholder="Send a message to Sweep", label=None, elem_id="message_box")
         with gr.Column(scale=0.5):
             create_pr_button = gr.Button(value="Create PR", interactive=bool(global_state.chat_history))
 
+
     def clear_inputs():
         global global_state
         global_state = State()
         config.state = global_state
         config.save()
         return [], [], [[""]]
 
+
     restart_button.click(clear_inputs, None, [file_names, chatbot, plan])
 
     file_names.change(get_files_update, repo_full_name, chatbot)
 
     searched = False
     selected_snippets = []
     file_to_str = {}
 
+
     def repo_name_change(repo_full_name):
         global installation_id
         try:
             installation_id = get_installation_id(repo_full_name)
             assert installation_id
             config.installation_id = installation_id
             api_client.config = config
@@ -199,53 +214,65 @@
         except Exception as e:
             config.repo_full_name = None
             config.installation_id = None
             config.save()
             api_client.config = config
             raise e
 
+
     def build_string():
         global selected_snippets
         global file_to_str
         for snippet in selected_snippets:
             file_name = snippet.file_path
             if file_name not in file_to_str:
                 add_file_to_dict(file_name)
-        snippets_text = "### Relevant snippets:\n" + "\n\n".join([file_to_str[snippet.file_path] for snippet in selected_snippets])
+        snippets_text = "### Relevant snippets:\n" + "\n\n".join(
+            [file_to_str[snippet.file_path] for snippet in selected_snippets])
         return snippets_text
 
+
     repo_full_name.change(repo_name_change, [repo_full_name], [msg])
 
+
     def add_file_to_dict(file_name):
         global file_to_str
         global path_to_contents
         global repo
         if file_name in path_to_contents:
             file_contents = path_to_contents[file_name]
         else:
-            file_contents = repo.get_contents(file_name, ref=SweepConfig.get_branch(repo)).decoded_content.decode('utf-8')
+            file_contents = repo.get_contents(file_name, ref=SweepConfig.get_branch(repo)).decoded_content.decode(
+                'utf-8')
         file_contents_split = file_contents.split("\n")
         length = len(file_contents_split)
         backtick, escaped_backtick = "`", "\\`"
         preview = "\n".join(file_contents_split[:3]).replace(backtick, escaped_backtick)
         file_to_str[file_name] = f'{file_name}:0:{length}\n```\n{preview}\n...\n```'
-    
+
+
     def file_names_change(file_names):
         global selected_snippets
         global file_to_str
         global path_to_contents
-        selected_snippets = [Snippet(content=path_to_contents[file_name], start=0, end=path_to_contents[file_name].count('\n'), file_path=file_name) for file_name in file_names]
+        selected_snippets = [
+            Snippet(content=path_to_contents[file_name], start=0, end=path_to_contents[file_name].count('\n'),
+                    file_path=file_name) for file_name in file_names]
         return file_names, build_string()
-    
+
+
     file_names.change(file_names_change, [file_names], [file_names, snippets_text])
-    
+
+
     def handle_message_submit(repo_full_name: str, user_message: str, history: list[tuple[str | None, str | None]]):
         if not repo_full_name:
             raise Exception("Set the repository name first")
-        return gr.update(value="", interactive=False), history + [[user_message, None]], gr.Button.update(interactive=True)
+        return gr.update(value="", interactive=False), history + [[user_message, None]], gr.Button.update(
+            interactive=True)
+
 
     def _handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_names, plan):
         global selected_snippets
         global searched
         if plan is None or plan == [[]] or plan == [[""]] or plan == [["", ""]]:
             plan = [["", ""]]
         message = chat_history[-1][0]
@@ -262,24 +289,24 @@
             file_names = [snippet.file_path for snippet in selected_snippets]
             yield chat_history, snippets_text, file_names, plan
             logger.info("Fetched relevant snippets.")
             chat_history[-1][1] = "Found relevant snippets."
             # Update using chat_history
             snippets_text = build_string()
             yield chat_history, snippets_text, file_names, plan
-        
+
         # Generate response
         logger.info("...")
         chat_history.append([None, "..."])
         yield chat_history, snippets_text, file_names, plan
         chat_history[-1][1] = ""
         logger.info("Starting to generate response...")
         if len(chat_history) > 1 and "create pr" in message.lower():
             stream = api_client.stream_chat(
-                chat_history, 
+                chat_history,
                 selected_snippets,
                 functions=[create_pr_function],
                 function_call=create_pr_function_call,
             )
         else:
             stream = api_client.stream_chat(chat_history, selected_snippets)
         function_name = ""
@@ -313,50 +340,66 @@
                     plan="\n".join([f"* `{item['file_path']}`: {item['instructions']}" for item in arguments["plan"]])
                 )
                 yield chat_history, snippets_text, file_names, plan
                 plan = [(item["file_path"], item["instructions"]) for item in arguments["plan"]]
                 yield chat_history, snippets_text, file_names, plan
             else:
                 raise NotImplementedError
-    
+
+
     def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_paths, plan):
         global global_state
-        for chat_history, snippets_text, file_paths, plan in _handle_message_stream(chat_history, snippets_text, file_paths, plan):
+        for chat_history, snippets_text, file_paths, plan in _handle_message_stream(chat_history, snippets_text,
+                                                                                    file_paths, plan):
             if plan is None or plan == [[]] or plan == [[""]] or plan == [["", ""]]:
                 plan = [["", ""]]
+            if plan and isinstance(plan[0], list):
+                plan = [item.split(":") for item in plan]
             global_state = State(
                 chat_history=chat_history,
                 snippets_text=snippets_text,
                 file_paths=file_paths,
                 plan=plan,
             )
             config.state = global_state
             config.save()
-            yield chat_history, snippets_text, file_paths, [(file_path + ": " + instructions,) for file_path, instructions in plan]
+            yield chat_history, snippets_text, file_paths, [(file_path + ": " + instructions,) for
+                                                            file_path, instructions in plan]
+
 
     response = msg \
         .submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot, create_pr_button], queue=False) \
-        .then(handle_message_stream, [chatbot, snippets_text, file_names, plan], [chatbot, snippets_text, file_names, plan]) \
+        .then(handle_message_stream, [chatbot, snippets_text, file_names, plan],
+              [chatbot, snippets_text, file_names, plan]) \
         .then(lambda: gr.update(interactive=True), None, [msg], queue=False)
 
+
+    def validate_branch_name(branch_name):
+        # Replace any characters that are not alphanumeric or '-' or '_' with '_'
+        valid_branch_name = re.sub('[^0-9a-zA-Z_-]', '_', branch_name)
+        return valid_branch_name
+
     def on_create_pr_button_click(chat_history: list[tuple[str | None, str | None]], plan: list[tuple[str]]):
         chat_history.append((None, "⌛ Creating PR..."))
         yield chat_history
         title = chat_history[0][0]
         content = chat_history[-1][1]
+        # Validate the branch name before it's used in the create_pr function
+        valid_branch_name = validate_branch_name(title.lower().replace(" ", "_").replace("-", "_")[:50])
         pull_request = api_client.create_pr(
             file_change_requests=[(item[:item.find(":")], item[item.find(":") + 1:]) for item, *_ in plan],
             pull_request={
                 "title": title,
                 "content": content,
-                "branch_name": title.lower().replace(" ", "_").replace("-", "_")[:50]
+                "branch_name": valid_branch_name
             },
             messages=chat_history,
         )
         chat_history.append((None, f"✅ PR created at {pull_request['html_url']}"))
         yield chat_history
 
+
     create_pr_button.click(on_create_pr_button_click, [chatbot, plan], chatbot)
 
 if __name__ == "__main__":
     demo.queue()
     demo.launch()
```

### Comparing `sweepai-0.4.2/sweepai/core/chat.py` & `sweepai-0.4.3/sweepai/core/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-from copy import deepcopy
 import json
-import os
+from copy import deepcopy
 from typing import Iterator, Literal, Self
 
+import anthropic
+import backoff
 import modal
 import openai
-import anthropic
 from loguru import logger
 from pydantic import BaseModel
-import backoff
 
-from sweepai.core.entities import (
-    Function,
-    Message,
-)
+from sweepai.core.entities import Message, Function
 from sweepai.core.prompts import (
     system_message_prompt,
     system_message_issue_comment_prompt,
 )
-from sweepai.utils.constants import UTILS_NAME
-from sweepai.utils.prompt_constructor import HumanMessagePrompt
-from sweepai.core.entities import Message, Function
 from sweepai.utils.chat_logger import ChatLogger
+from sweepai.utils.config.server import UTILS_MODAL_INST_NAME, ANTHROPIC_API_KEY, OPENAI_DO_HAVE_32K_MODEL_ACCESS
+from sweepai.utils.prompt_constructor import HumanMessagePrompt
 
 # TODO: combine anthropic and openai
 
 AnthropicModel = (
-    Literal["claude-v1"]
-    | Literal["claude-v1.3-100k"]
-    | Literal["claude-instant-v1.1-100k"]
+        Literal["claude-v1"]
+        | Literal["claude-v1.3-100k"]
+        | Literal["claude-instant-v1.1-100k"]
 )
-OpenAIModel = Literal["gpt-3.5-turbo"] | Literal["gpt-4"] | Literal["gpt-4-32k"] | Literal["gpt-4-0613"] | Literal["gpt-4-32k-0613"] | Literal["gpt-3.5-turbo-16k-0613"]
+OpenAIModel = Literal["gpt-3.5-turbo"] | Literal["gpt-4"] | Literal["gpt-4-0613"] | Literal["gpt-3.5-turbo-16k-0613"] | Literal["gpt-4-32k"] | Literal["gpt-4-32k-0613"]
+
 ChatModel = OpenAIModel | AnthropicModel
 model_to_max_tokens = {
     "gpt-3.5-turbo": 4096,
     "gpt-4": 8192,
     "gpt-4-0613": 8192,
-    "gpt-4-32k": 32000,
-    "gpt-4-32k-0613": 32000,
     "claude-v1": 9000,
     "claude-v1.3-100k": 100000,
     "claude-instant-v1.3-100k": 100000,
     "gpt-3.5-turbo-16k-0613": 16000,
+    "gpt-4-32k-0613": 32000,
+    "gpt-4-32k": 32000,
+
 }
 temperature = 0.1
 
 def format_for_anthropic(messages: list[Message]) -> str:
     if len(messages) > 1:
         new_messages: list[Message] = [Message(role="system", content=messages[0].content + "\n" + messages[1].content)]
         messages = messages[2:] if len(messages) >= 3 else []
@@ -63,51 +60,51 @@
     messages: list[Message] = [
         Message(
             role="system",
             content=system_message_prompt,
         )
     ]
     prev_message_states: list[list[Message]] = []
-    model: ChatModel = "gpt-4-32k-0613"
+    model: ChatModel = "gpt-4-32k-0613" if OPENAI_DO_HAVE_32K_MODEL_ACCESS else "gpt-4-0613"
     human_message: HumanMessagePrompt | None = None
     file_change_paths = []
     chat_logger: ChatLogger | None = None
 
     @classmethod
     def from_system_message_content(
-        cls, human_message: HumanMessagePrompt, is_reply: bool = False, **kwargs
+            cls, human_message: HumanMessagePrompt, is_reply: bool = False, **kwargs
     ) -> Self:
         if is_reply:
             system_message_content = system_message_issue_comment_prompt
 
         # Todo: This moves prompts away from unified system message prompt
         # system_message_prompt + "\n\n" + human_message.construct_prompt()
         messages = [
-           Message(role="system", content=system_message_prompt, key="system")
-       ]
+            Message(role="system", content=system_message_prompt, key="system")
+        ]
 
-        added_messages = human_message.construct_prompt() # [ { role, content }, ... ]
+        added_messages = human_message.construct_prompt()  # [ { role, content }, ... ]
         for msg in added_messages:
             messages.append(Message(**msg))
 
         return cls(
-            messages = messages,
+            messages=messages,
             human_message=human_message,
             **kwargs,
         )
 
     @classmethod
     def from_system_message_string(cls, prompt_string, **kwargs) -> Self:
         return cls(
             messages=[Message(role="system", content=prompt_string, key="system")],
             **kwargs,
         )
 
     def select_message_from_message_key(
-        self, message_key: str, message_role: str = None
+            self, message_key: str, message_role: str = None
     ):
         if message_role:
             return [
                 message
                 for message in self.messages
                 if message.key == message_key and message.role == message_role
             ][0]
@@ -118,34 +115,34 @@
             message for message in self.messages if key_to_delete not in (message.key or '')
         ]
 
     def delete_file_from_system_message(self, file_path: str):
         self.human_message.delete_file(file_path)
 
     def get_message_content_from_message_key(
-        self, message_key: str, message_role: str = None
+            self, message_key: str, message_role: str = None
     ):
         return self.select_message_from_message_key(
             message_key, message_role=message_role
         ).content
 
     def update_message_content_from_message_key(
-        self, message_key: str, new_content: str, message_role: str = None
+            self, message_key: str, new_content: str, message_role: str = None
     ):
         self.select_message_from_message_key(
             message_key, message_role=message_role
         ).content = new_content
 
     def chat(
-        self,
-        content: str,
-        model: ChatModel | None = None,
-        message_key: str | None = None,
-        functions: list[Function] = [],
-        function_name: dict | None = None,
+            self,
+            content: str,
+            model: ChatModel | None = None,
+            message_key: str | None = None,
+            functions: list[Function] = [],
+            function_name: dict | None = None,
     ):
         if self.messages[-1].function_call is None:
             self.messages.append(Message(role="user", content=content, key=message_key))
         else:
             name = self.messages[-1].function_call["name"]
             self.messages.append(Message(role="function", content=content, key=message_key, name=name))
         model = model or self.model
@@ -173,37 +170,37 @@
         else:
             response = self.call_anthropic(model=model)
             self.messages.append(
                 Message(role="assistant", content=response, key=message_key)
             )
         self.prev_message_states.append(self.messages)
         return self.messages[-1].content
-    
+
     def call_openai(
-        self, 
-        model: ChatModel | None = None,
-        functions: list[Function] = [],
-        function_name: dict | None = None,
+            self,
+            model: ChatModel | None = None,
+            functions: list[Function] = [],
+            function_name: dict | None = None,
     ):
         if self.chat_logger:
             tickets_allocated = 60 if self.chat_logger.is_paying_user() else 3
             tickets_count = self.chat_logger.get_ticket_count()
             if tickets_count < tickets_allocated:
                 model = model or self.model
                 logger.warning(f"{tickets_count} tickets found in MongoDB, using {model}")
             else:
                 model = "gpt-3.5-turbo-16k-0613"
         else:
             model = "gpt-3.5-turbo-16k-0613"
-        
-        count_tokens = modal.Function.lookup(UTILS_NAME, "Tiktoken.count")
+
+        count_tokens = modal.Function.lookup(UTILS_MODAL_INST_NAME, "Tiktoken.count")
         messages_length = sum(
             [count_tokens.call(message.content or "") for message in self.messages]
         )
-        max_tokens = model_to_max_tokens[model] - int(messages_length) - 400 # this is for the function tokens
+        max_tokens = model_to_max_tokens[model] - int(messages_length) - 400  # this is for the function tokens
         # TODO: Add a check to see if the message is too long
         logger.info("file_change_paths" + str(self.file_change_paths))
         if len(self.file_change_paths) > 0:
             self.file_change_paths.remove(self.file_change_paths[0])
         if max_tokens < 0:
             if len(self.file_change_paths) > 0:
                 pass
@@ -211,15 +208,16 @@
                 raise ValueError(f"Message is too long, max tokens is {max_tokens}")
         messages_raw = "\n".join([(message.content or "") for message in self.messages])
         logger.info(f"Input to call openai:\n{messages_raw}")
 
         gpt_4_buffer = 800
         if int(messages_length) + gpt_4_buffer < 6000 and model == "gpt-4-32k-0613":
             model = "gpt-4-0613"
-            max_tokens = model_to_max_tokens[model] - int(messages_length) - gpt_4_buffer # this is for the function tokens
+            max_tokens = model_to_max_tokens[model] - int(
+                messages_length) - gpt_4_buffer  # this is for the function tokens
         if "gpt-4" in model:
             max_tokens = min(max_tokens, 5000)
         logger.info(f"Using the model {model}, with {max_tokens} tokens remaining")
         global retry_counter
         retry_counter = 0
         if functions:
             @backoff.on_exception(
@@ -267,14 +265,15 @@
                         'function_call': function_name,
                         'output': output,
                     })
                     return output
                 except Exception as e:
                     logger.warning(e)
                     raise e
+
             result = fetch()
             if "function_call" in result:
                 result = dict(result["function_call"]), True
             else:
                 result = result["content"], False
             logger.info(f"Output to call openai:\n{result}")
             return result
@@ -288,50 +287,51 @@
             )
             def fetch():
                 global retry_counter
                 retry_counter += 1
                 token_sub = retry_counter * 200
                 try:
                     output = openai.ChatCompletion.create(
-                            model=model,
-                            messages=self.messages_dicts,
-                            max_tokens=max_tokens - token_sub,
-                            temperature=temperature,
-                        ) \
+                        model=model,
+                        messages=self.messages_dicts,
+                        max_tokens=max_tokens - token_sub,
+                        temperature=temperature,
+                    ) \
                         .choices[0] \
                         .message["content"]
                     if self.chat_logger is not None: self.chat_logger.add_chat({
                         'model': model,
                         'messages': self.messages_dicts,
                         'max_tokens': max_tokens - token_sub,
                         'temperature': temperature,
                         'output': output
                     })
                     return output
                 except Exception as e:
                     logger.warning(e)
                     raise e
+
             result = fetch()
             logger.info(f"Output to call openai:\n{result}")
             return result
-    
+
     def call_anthropic(self, model: ChatModel | None = None) -> str:
         if model is None:
             model = self.model
-        count_tokens = modal.Function.lookup(UTILS_NAME, "Tiktoken.count")
+        count_tokens = modal.Function.lookup(UTILS_MODAL_INST_NAME, "Tiktoken.count")
         messages_length = sum(
             [int(count_tokens.call(message.content) * 1.1) for message in self.messages]
         )
         max_tokens = model_to_max_tokens[model] - int(messages_length) - 1000
         logger.info(f"Number of tokens: {max_tokens}")
         messages_raw = format_for_anthropic(self.messages)
         logger.info(f"Input to call anthropic:\n{messages_raw}")
 
-        assert os.environ.get("ANTHROPIC_API_KEY"), "Please set ANTHROPIC_API_KEY"
-        client = anthropic.Client(api_key=os.environ.get("ANTHROPIC_API_KEY"))
+        assert ANTHROPIC_API_KEY is not None
+        client = anthropic.Client(api_key=ANTHROPIC_API_KEY)
 
         @backoff.on_exception(
             backoff.expo,
             Exception,
             max_tries=12,
             jitter=backoff.random_jitter,
         )
@@ -354,46 +354,46 @@
             _self = deepcopy(self)
             _self.messages.append(Message(role="assistant", content=result, key=""))
             extension = _self.call_anthropic(model=model)
             print(len(result), len(extension), len(result + extension))
             return result + extension
         logger.info(f"Output to call anthropic:\n{result}")
         return result
-    
+
     def chat_stream(
-        self,
-        content: str,
-        model: ChatModel | None = None,
-        message_key: str | None = None,
-        functions: list[Function] = [],
-        function_call: dict | None = None,
+            self,
+            content: str,
+            model: ChatModel | None = None,
+            message_key: str | None = None,
+            functions: list[Function] = [],
+            function_call: dict | None = None,
     ) -> Iterator[dict]:
         if self.messages[-1].function_call is None:
             self.messages.append(Message(role="user", content=content, key=message_key))
         else:
             name = self.messages[-1].function_call["name"]
             self.messages.append(Message(role="function", content=content, key=message_key, name=name))
         model = model or self.model
         is_function_call = False
         # might be a bug here in all of this
         # return self.stream_openai(model=model, functions=functions, function_name=function_name)
         return self.stream_openai(model=model, functions=functions, function_call=function_call)
-    
+
     def stream_openai(
-        self,
-        model: ChatModel | None = None,
-        functions: list[Function] = [],
-        function_call: dict | None = None,
+            self,
+            model: ChatModel | None = None,
+            functions: list[Function] = [],
+            function_call: dict | None = None,
     ) -> Iterator[dict]:
         model = model or self.model
-        count_tokens = modal.Function.lookup(UTILS_NAME, "Tiktoken.count")
+        count_tokens = modal.Function.lookup(UTILS_MODAL_INST_NAME, "Tiktoken.count")
         messages_length = sum(
             [count_tokens.call(message.content or "") for message in self.messages]
         )
-        max_tokens = model_to_max_tokens[model] - int(messages_length) - 400 # this is for the function tokens
+        max_tokens = model_to_max_tokens[model] - int(messages_length) - 400  # this is for the function tokens
         # TODO: Add a check to see if the message is too long
         logger.info("file_change_paths" + str(self.file_change_paths))
         if len(self.file_change_paths) > 0:
             self.file_change_paths.remove(self.file_change_paths[0])
         if max_tokens < 0:
             if len(self.file_change_paths) > 0:
                 pass
@@ -401,17 +401,19 @@
                 raise ValueError(f"Message is too long, max tokens is {max_tokens}")
         messages_raw = "\n".join([(message.content or "") for message in self.messages])
         logger.info(f"Input to call openai:\n{messages_raw}")
 
         gpt_4_buffer = 800
         if int(messages_length) + gpt_4_buffer < 6000 and model == "gpt-4-32k-0613":
             model = "gpt-4-0613"
-            max_tokens = model_to_max_tokens[model] - int(messages_length) - gpt_4_buffer # this is for the function tokens
+            max_tokens = model_to_max_tokens[model] - int(
+                messages_length) - gpt_4_buffer  # this is for the function tokens
 
         logger.info(f"Using the model {model}, with {max_tokens} tokens remaining")
+
         def generator() -> Iterator[str]:
             stream = openai.ChatCompletion.create(
                 model=model,
                 messages=self.messages_dicts,
                 temperature=temperature,
                 functions=[json.loads(function.json()) for function in functions],
                 function_call=function_call or "auto",
@@ -421,14 +423,15 @@
                 messages=self.messages_dicts,
                 temperature=temperature,
                 stream=True
             )
             for data in stream:
                 chunk = data.choices[0].delta
                 yield chunk
+
         return generator()
 
     @property
     def messages_dicts(self):
         # Remove the key from the message object before sending to OpenAI
         cleaned_messages = [
             message.to_openai()
```

### Comparing `sweepai-0.4.2/sweepai/core/code_repair.py` & `sweepai-0.4.3/sweepai/core/code_repair.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import re
 import subprocess
+
 from sweepai.core.chat import ChatGPT
 from sweepai.core.entities import Message
 from sweepai.core.prompts import code_repair_system_prompt, code_repair_prompt
 
 response_regex = r"```[^\n]*(?P<response>.+)```"
 
 
@@ -39,23 +39,23 @@
         # Else, there was a syntax error.
         if result.returncode == 0:
             return True
         else:
             print(result.stderr)
             return False
 
-
-    def repair_code(self, diff: str, user_code: str, feature:str, retries=3) -> str:
+    def repair_code(self, diff: str, user_code: str, feature: str, retries=3) -> str:
         self.messages = [Message(role="system", content=code_repair_system_prompt.format(feature=feature))]
-        self.model = "gpt-3.5-turbo-16k-0613" # can be optimized
+        self.model = "gpt-3.5-turbo-16k-0613"  # can be optimized
         retry_count = 0
         while retry_count < retries:
             response = self.chat(code_repair_prompt.format(diff=diff, user_code=user_code), message_key='code_repair')
             # Check if the length of the response does not differ by more than 15% from the input
-            if len(user_code.splitlines()) > 50 and abs(len(response.splitlines()) - len(user_code.splitlines())) / len(user_code.splitlines()) > 0.15:
+            if len(user_code.splitlines()) > 50 and abs(len(response.splitlines()) - len(user_code.splitlines())) / len(
+                    user_code.splitlines()) > 0.15:
                 self.delete_messages_from_chat(key_to_delete='code_repair')
                 retry_count += 1
                 if retry_count == retries:
                     return user_code
             else:
                 break
         return response.strip() + "\n"
```

### Comparing `sweepai-0.4.2/sweepai/core/entities.py` & `sweepai-0.4.3/sweepai/core/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import string
 from typing import ClassVar, Literal, Type, TypeVar
+
 from loguru import logger
 from pydantic import BaseModel
 
 Self = TypeVar("Self", bound="RegexMatchableBaseModel")
 
 
 class Message(BaseModel):
@@ -29,22 +30,25 @@
         }
         if self.function_call:
             obj["function_call"] = self.function_call
         if self.role == "function":
             obj["name"] = self.name
         return obj
 
+
 class Function(BaseModel):
     class Parameters(BaseModel):
         type: str = "object"
         properties: dict
+
     name: str
     description: str
     parameters: Parameters
 
+
 class RegexMatchError(ValueError):
     pass
 
 
 class RegexMatchableBaseModel(BaseModel):
     _regex: ClassVar[str]
 
@@ -71,71 +75,75 @@
 # tab supremacy
 def clean_filename(file_name: str):
     valid_chars = "-_./[]%s%s" % (string.ascii_letters, string.digits)
     file_name = ''.join(c for c in file_name if c in valid_chars)
     file_name = file_name.replace(' ', '')
     return os.path.normpath(file_name)
 
+
 def clean_instructions(instructions: str):
     return instructions.strip()
 
+
 class FileChangeRequest(RegexMatchableBaseModel):
     filename: str
     instructions: str
     change_type: Literal["modify"] | Literal["create"]
 
     @classmethod
     def from_string(cls: Type[Self], string: str, **kwargs) -> Self:
         colon_idx = string.find(':')
         file_name = string[:colon_idx]
         instructions = string[colon_idx + 1:]
         file_name = clean_filename(file_name)
         instructions = clean_instructions(instructions)
-        res = FileChangeRequest(filename=file_name, 
+        res = FileChangeRequest(filename=file_name,
                                 instructions=instructions,
                                 change_type="modify")
         return res
 
 
 class FileCreation(RegexMatchableBaseModel):
     commit_message: str
     code: str
     _regex = r'''commit_message\s+=\s+"(?P<commit_message>.*?)".*?<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)<\/new_file>'''
-    #_regex = r"""Commit Message:(?P<commit_message>.*)<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)$"""
+
+    # _regex = r"""Commit Message:(?P<commit_message>.*)<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)$"""
     # _regex = r"""Commit Message:(?P<commit_message>.*)(<new_file>|```)(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)($|```)"""
 
     @classmethod
     def from_string(cls: Type[Self], string: str, **kwargs) -> Self:
         result = super().from_string(string, **kwargs)
         result.code = result.code.strip()
         if result.code.endswith("</new_file>"):
             result.code = result.code[: -len("</new_file>")]
         if len(result.code) == 1:
             result.code = result.code.replace("```", "")
             return result.code + "\n"
         if result.code.startswith("```"):
             first_newline = result.code.find("\n")
             last_newline = result.code.rfind("\n")
-            result.code = result.code[first_newline + 1 :]
+            result.code = result.code[first_newline + 1:]
             result.code = result.code[: last_newline]
         result.code += "\n"
         return result
 
 
 class PullRequest(RegexMatchableBaseModel):
     title: str
     branch_name: str
     content: str
-    _regex = r'''title\s+=\s+"(?P<title>.*?)"\n+branch\s+=\s+"(?P<branch_name>.*?)"\n+content\s+=\s+"""(?P<content>.*?)"""'''
+    _regex = r'''pr_title\s+=\s+"(?P<title>.*?)"\n+branch\s+=\s+"(?P<branch_name>.*?)"\n+pr_content\s+=\s+"""(?P<content>.*?)"""'''
+
 
 class Snippet(BaseModel):
     """
     Start and end refer to line numbers
     """
-    
+
     content: str
     start: int
     end: int
     file_path: str
 
     def get_snippet(self):
         snippet = "\n".join(self.content.splitlines()[self.start:self.end])
@@ -150,79 +158,81 @@
         assert self.file_path == other.file_path
         return Snippet(
             content=self.content,
             start=self.start,
             end=other.end,
             file_path=self.file_path
         )
-    
+
     def __xor__(self, other: "Snippet") -> bool:
         """
         Returns True if there is an overlap between two snippets.
         """
         if self.file_path != other.file_path:
             return False
         return self.file_path == other.file_path and (
                 (self.start <= other.start and self.end >= other.start)
                 or (other.start <= self.start and other.end >= self.start)
-            )
-        
+        )
+
     def __or__(self, other: "Snippet") -> "Snippet":
         assert self.file_path == other.file_path
         return Snippet(
             content=self.content,
             start=min(self.start, other.start),
             end=max(self.end, other.end),
             file_path=self.file_path
         )
-    
+
     @property
     def xml(self):
         return f"""<snippet filepath="{self.file_path}" start="{self.start}" end="{self.end}">\n{self.get_snippet()}\n</snippet>"""
-    
+
     def get_url(self, repo_name: str, commit_id: str = "main"):
         num_lines = self.content.count("\n") + 1
         return f"https://github.com/{repo_name}/blob/{commit_id}/{self.file_path}#L{max(self.start, 1)}-L{min(self.end, num_lines)}"
-    
+
     def get_markdown_link(self, repo_name: str, commit_id: str = "main"):
         num_lines = self.content.count("\n") + 1
         base = commit_id + "/" if commit_id != "main" else ""
         return f"[{base}{self.file_path}#L{max(self.start, 1)}-L{min(self.end, num_lines)}]({self.get_url(repo_name, commit_id)})"
-    
+
     def get_slack_link(self, repo_name: str, commit_id: str = "main"):
         num_lines = self.content.count("\n") + 1
         base = commit_id + "/" if commit_id != "main" else ""
         return f"<{self.get_url(repo_name, commit_id)}|{base}{self.file_path}#L{max(self.start, 1)}-L{min(self.end, num_lines)}>"
 
     def get_preview(self, max_lines: int = 5):
         snippet = "\n".join(self.content.splitlines()[self.start:min(self.start + max_lines, self.end)])
         if self.start > 1:
             snippet = '\n' + snippet
         if self.end < self.content.count('\n') + 1 and self.end > max_lines:
             snippet = snippet + '\n'
         return snippet
-    
+
     def expand(self, num_lines: int = 50):
         return Snippet(
             content=self.content,
             start=max(self.start - num_lines, 1),
             end=min(self.end + num_lines, self.content.count("\n") + 1),
             file_path=self.file_path
         )
 
     @property
     def denotation(self):
         return f"{self.file_path}:{self.start}-{self.end}"
-        
+
 
 class DiffSummarization(RegexMatchableBaseModel):
     content: str
     _regex = r"""<file_summarization>(?P<content>.*)<\/file_summarization>"""
 
+
 class PullRequestComment(RegexMatchableBaseModel):
     changes_required: str
     content: str
     _regex = r"""<changes_required>(?P<changes_required>.*)<\/changes_required>(\s+)<review_comment>(?P<content>.*)<\/review_comment>"""
 
+
 class NoFilesException(Exception):
     def __init__(self, message="Sweep could not find any files to modify"):
         super().__init__(message)
```

### Comparing `sweepai-0.4.2/sweepai/core/gha_extraction.py` & `sweepai-0.4.3/sweepai/core/gha_extraction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import re
-import subprocess
 from sweepai.core.chat import ChatGPT
 from sweepai.core.entities import Message
 from sweepai.core.prompts import gha_extraction_system_prompt, gha_extraction_prompt
 
 
 class GHAExtractor(ChatGPT):
     def gha_extract(self, gha_logs: str) -> str:
         self.messages = [Message(role="system", content=gha_extraction_system_prompt)]
-        self.model = "gpt-3.5-turbo-16k-0613" # can be optimized
+        self.model = "gpt-3.5-turbo-16k-0613"  # can be optimized
         response = self.chat(gha_extraction_prompt.format(gha_logs=gha_logs))
         self.undo()
-        return response.strip() + "\n"
+        return response.strip() + "\n"
```

### Comparing `sweepai-0.4.2/sweepai/core/prompts.py` & `sweepai-0.4.3/sweepai/core/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 List of common prompts used across the codebase.
 """
 
 # Following two should be fused
 system_message_prompt = "Your name is Sweep bot. You are a brilliant and thorough engineer assigned to the following Github ticket. You will be helpful and friendly, but informal and concise: get to the point. When you write code to solve tickets, the code works on the first try and is formatted perfectly. You have the utmost care for the user that you write for, so you do not make mistakes."
 system_message_issue_comment_prompt = "Your name is Sweep bot. You are a brilliant and thorough engineer assigned to the following Github ticket, and a user has just responded with feedback. You will be helpful and friendly, but informal and concise: get to the point. When you write code to solve tickets, the code works on the first try and is formatted perfectly. You have the utmost care for the user that you write for, so you do not make mistakes."
 
-
 human_message_prompt = [
 {'role': 'assistant', 'content': 'Examining repo...'},
 {'role': 'user', 'content': """<relevant_snippets_in_repo>
 {relevant_snippets}
-</relevant_snippets_in_repo>"""},
+</relevant_snippets_in_repo>""", 'key': 'relevant_snippets'},
 {'role': 'user', 'content': """<relevant_paths_in_repo>
 {relevant_directories}
 </relevant_paths_in_repo>"""},
 {'role': 'user', 'content': """<repo_tree>
 {tree}
 </repo_tree>"""},
 {'role': 'user', 'content':
 """# Repo & Issue Metadata
 Repo: {repo_name}: {repo_description}
 Issue Url: {issue_url}
 Username: {username}
 Issue Title: {title}
 Issue Description: {description}"""}]
 
-
 human_message_review_prompt = [
 {'role': 'assistant', 'content': 'Reviewing my pull request...'},
 {'role': 'user', 'content': """<relevant_snippets_in_repo>
 {relevant_snippets}
 </relevant_snippets_in_repo>"""},
 {'role': 'user', 'content': """<relevant_paths_in_repo>
 {relevant_directories}
@@ -127,15 +125,15 @@
 {'role': 'user', 'content':
 """<relevant_snippets_in_repo>
 {relevant_snippets}
 </relevant_snippets_in_repo>"""},
 {'role': 'user', 'content': """<relevant_paths_in_repo>
 {relevant_directories}
 </relevant_paths_in_repo>"""},
-    {'role': 'user', 'content': """<repo_tree>
+{'role': 'user', 'content': """<repo_tree>
 {tree}
 </repo_tree>"""},
 {'role': 'user', 'content':
 """# Repo, Issue, & PR Metadata
 Repo: {repo_name}: {repo_description}
 Issue Url: {issue_url}
 Username: {username}
@@ -158,25 +156,25 @@
 comment_line_prompt = """\
 The user made the review in this file: {pr_file_path}
 and on this line: {pr_line}
 """
 
 cot_retrieval_prompt = """
 Gather information to solve the problem. Use "finish" when you feel like you have sufficient information.
-""" 
+"""
 
 files_to_change_prompt = """
 Think step-by-step to break down the requested problem or feature, and then figure out what to change in the current codebase.
 Then, provide a list of files you would like to modify, abiding by the following:
-* Including the FULL path, e.g. src/main.py and not just main.py
-* Use a one-line, detailed, natural language instructions on what to modify, with reference to variable names
-* The list of files to create or modify may be empty, but you MUST leave the XML tags with a single list element with "* None"
+* Including the FULL path, e.g. src/main.py and not just main.py, using the repo_tree as the source of truth.
+* Use detailed, natural language instructions on what to modify, with reference to variable names
 * There MUST be both create and modify XML tags
+* The list of files to create or modify may be empty, but you MUST leave the XML tags with a single list element with "* None"
 * Create/modify up to 5 FILES
-* Do not modify non-text files, like images, svgs, binary, etc
+* Do not modify non-text files such as images, svgs, binary, etc
 * You MUST follow the following format:
 
 Step-by-step thoughts with explanations: 
 * Thought 1 - Explanation 1
 * Thought 2 - Explanation 2
 ...
 
@@ -263,17 +261,17 @@
 
 Lines to change in the file:
 * lines a-b
 ...
 
 Only include the line numbers."""
 
-#<snippets>
-#{snippets}
-#</snippets>
+# <snippets>
+# {snippets}
+# </snippets>
 modify_file_prompt = """
 File contains lines {line_numbers}
 
 Generate a new_file based on the given plan, ensuring that you:
 1. It is imperative that we do not leave any work to the user/future readers of this code. So, WRITE FUNCTIONS COMPLETELY THAT WILL WORK.
 2. Do not write the original line numbers with the new code.
 3. Make sure the new code follows the same programming language conventions as the old code.
@@ -281,24 +279,23 @@
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copied>0-25</copied>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copied>0-50</copied>".
 
 Example: If you want to modify lines 51-52 and add line after line 75:
 <new_file>
 <copied>1-50</copied>
 def main():
-     print("hello world")
+    print("hello world")
 <copied>53-75</copied>
 print("debug statement")
 <copied>76-100</copied>
 </new_file>
 
-Do not rewrite entire file. Use <copied> XML tag when possible. Do not include the line numbers in the new file. Write complete implementations.
+Do not rewrite the entire file. Use <copied> XML tag when possible. Do not include the line numbers in the new file. Write complete implementations.
 """
 
-
 modify_file_prompt_2 = """
 File Name: {filename}
 <old_file>
 {code}
 </old_file>
 
 ---
@@ -323,47 +320,42 @@
 Code Generation:
 ```
 Generate a new_file based on the given plan, ensuring that you:
 1. It is imperative that we do not leave any work to the user/future readers of this code. Therefore write functions with complete business logic.
 2. Only write code, do not write line numbers.
 3. Make sure the new code follows the same programming language conventions as the old code.
 
-Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copy_lines A-B>"). Make sure to use this exact format.
-Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copy_lines 1-50>".
+Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copy_lines A-B/>"). Make sure to use this exact format.
+Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copy_lines 1-50/>".
 
 Example: If you want to modify lines 51-52 and add line after line 75:
 <new_file>
-<copy_lines 1-50>
+<copy_lines 1-50/>
 def main():
-     print("hello world")
-<copy_lines 53-75>
+    print("hello world")
+<copy_lines 53-75/>
 print("debug statement")
-<copy_lines 76-100>
+<copy_lines 76-100/>
 </new_file>
 
-Do not rewrite entire file. Use <copy_lines A-B> XML tag when possible. Do not include the line numbers in the new file. Write complete implementations.
+Do not rewrite the entire file. Use <copy_lines A-B/> XML tag when possible. Do not include the line numbers in the new file. Write complete implementations.
 ```
 
 Context: "{instructions}". Limit your changes to the context.
 Instructions:
 - Complete Code Planning step
 - Complete Code Generation step"""
 
-
-
-
-
 pr_code_prompt = ""  # TODO: deprecate this
 
+pull_request_prompt = """Now, create a PR for your changes using GitHub markdown in the following format:
 
-pull_request_prompt = """With your plan in mind, generate one PR for your planned changes using GitHub markdown.
-
-title = "..."
+pr_title = "..."
 branch = "..."
-content = \"\"\"
+pr_content = \"\"\"
 ...
 ...
 \"\"\""""
 
 summarize_system_prompt = """
 Your name is Sweep bot. You are an engineer assigned to helping summarize code instructions and code changes.
 """
```

### Comparing `sweepai-0.4.2/sweepai/core/react.py` & `sweepai-0.4.3/sweepai/core/react.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,64 +38,72 @@
 <output>
 {output}
 </output>
 
 What would you like to do next? Use the same format as above.
 """
 
+
 def dedent(text: str) -> str:
     return re.sub(r'(\n)[ \t]+', r'\n', text.strip())
 
+
 class Tool(BaseModel):
     description: str
     function: Callable[[str], str]
-    example_inputs: str  = ""
+    example_inputs: str = ""
     name: str = ""
 
     @property
     def _name(self):
         return self.__class__.__name__ if self.name == "" else self.name
-    
+
     @property
     def summary(self):
         return dedent(f"""
         {self._name}: {self.description}
         Example usage:
         <tool>{self._name}</tool>
         <inputs>
         {self.example_inputs}
         </inputs>
         """.strip())
-    
+
     def __call__(self, *args, **kwargs):
         return self.function(*args, **kwargs)
-    
+
     @classmethod
     def tool(cls, **kwargs):
         def decorator(function):
             return cls(function=function, **kwargs)
+
         return decorator
 
+
 class CodeSearch(Tool):
     description = "Search in the codebase for relevant snippets of code. Takes natural language search query as input."
     example_inputs = "Modal component on main page."
 
+
 class ReadFiles(Tool):
-    description = "Reads listed files. Takes list of literal file paths as input, separated by newlines. Max 3 files." 
+    description = "Reads listed files. Takes list of literal file paths as input, separated by newlines. Max 3 files."
     example_inputs = "src/main.py\ntests/test_main.py\ntests/test_utils.py:101:200"
 
+
 class Google(Tool):
     description = "Search for code documentation on Google. Takes natural language search query as input."
     example_inputs = "Discord API docs"
 
+
 class Finish(Tool):
     description = "Indicate you have sufficient information to move forward with making changes to the codebase. Return with an empty string."
     example_inputs = ""
     function = lambda _: ""
 
+
 class Toolbox(BaseModel):
     tools: list[Tool] = []
 
     @property
     def prompt(self):
         return REACT_INITIAL_PROMPT.format(tools="\n\n".join([tool.summary for tool in self.tools]))
 
@@ -109,8 +117,7 @@
             match = re.search(cls._regex, results, flags=re.DOTALL)
             return cls(tool_name=match.group("tool").strip(), inputs=match.group("inputs").strip())
 
     def process_results(self, parsed_results: "Toolbox.ParsedResults") -> str:
         # parsed_results = Toolbox.ParsedResults.parse(raw_output)
         tool = next((tool for tool in self.tools if tool._name == parsed_results.tool_name), None)
         return tool(parsed_results.inputs)
-
```

### Comparing `sweepai-0.4.2/sweepai/core/sweep_bot.py` & `sweepai-0.4.3/sweepai/core/sweep_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,97 +1,99 @@
-import json
-from loguru import logger
-import github
-from github.Repository import Repository
+import traceback
+import re
+
+import modal
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException
-import modal
+from github.Repository import Repository
+from loguru import logger
 from pydantic import BaseModel
-from sweepai.core.code_repair import CodeRepairer
-from sweepai.utils.chat_logger import ChatLogger
-import re
-import traceback
 
+from sweepai.core.chat import ChatGPT
+from sweepai.core.code_repair import CodeRepairer
 from sweepai.core.entities import (
     FileCreation,
     FileChangeRequest,
     FilesToChange,
     PullRequest,
     RegexMatchError,
     Function,
     Snippet, NoFilesException
 )
-from sweepai.core.chat import ChatGPT
 from sweepai.core.prompts import (
     files_to_change_prompt,
     pull_request_prompt,
     create_file_prompt,
     modify_file_prompt_2,
-    modify_file_plan_prompt,
 )
-from sweepai.utils.config import SweepConfig
-from sweepai.utils.constants import DB_NAME, SECONDARY_MODEL
-from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown, revert_whitespace_changes
+from sweepai.utils.config.client import SweepConfig
+from sweepai.utils.config.server import DB_MODAL_INST_NAME, SECONDARY_MODEL
+from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown
 
 class MaxTokensExceeded(Exception):
     def __init__(self, filename):
         self.filename = filename
 
 class CodeGenBot(ChatGPT):
 
     def get_files_to_change(self, retries=2):
         file_change_requests: list[FileChangeRequest] = []
         # Todo: put retries into a constants file
         # also, this retries multiple times as the calls for this function are in a for loop
         for count in range(retries):
             try:
                 logger.info(f"Generating for the {count}th time...")
-                files_to_change_response = self.chat(files_to_change_prompt, message_key="files_to_change") # Dedup files to change here
+                files_to_change_response = self.chat(files_to_change_prompt,
+                                                     message_key="files_to_change")  # Dedup files to change here
                 files_to_change = FilesToChange.from_string(files_to_change_response)
                 files_to_create: list[str] = files_to_change.files_to_create.split("\n*")
                 files_to_modify: list[str] = files_to_change.files_to_modify.split("\n*")
                 for file_change_request, change_type in zip(
-                    files_to_create + files_to_modify,
-                    ["create"] * len(files_to_create)
-                    + ["modify"] * len(files_to_modify),
+                        files_to_create + files_to_modify,
+                        ["create"] * len(files_to_create)
+                        + ["modify"] * len(files_to_modify),
                 ):
                     file_change_request = file_change_request.strip()
                     if not file_change_request or file_change_request == "* None":
                         continue
                     logger.debug(file_change_request)
                     logger.debug(change_type)
                     file_change_requests.append(
                         FileChangeRequest.from_string(
                             file_change_request, change_type=change_type
                         )
                     )
                 # Create a dictionary to hold file names and their corresponding instructions
                 file_instructions_dict = {}
                 for file_change_request in file_change_requests:
-                # If the file name is already in the dictionary, append the new instructions
+                    # If the file name is already in the dictionary, append the new instructions
                     if file_change_request.filename in file_instructions_dict:
                         instructions, change_type = file_instructions_dict[file_change_request.filename]
-                        file_instructions_dict[file_change_request.filename] = (instructions + " " + file_change_request.instructions, change_type)
+                        file_instructions_dict[file_change_request.filename] = (
+                            instructions + " " + file_change_request.instructions, change_type)
                     else:
-                        file_instructions_dict[file_change_request.filename] = (file_change_request.instructions, file_change_request.change_type)
-                file_change_requests = [FileChangeRequest(filename=file_name, instructions=instructions, change_type=change_type) for file_name, (instructions, change_type) in file_instructions_dict.items()]
+                        file_instructions_dict[file_change_request.filename] = (
+                            file_change_request.instructions, file_change_request.change_type)
+                file_change_requests = [
+                    FileChangeRequest(filename=file_name, instructions=instructions, change_type=change_type) for
+                    file_name, (instructions, change_type) in file_instructions_dict.items()]
                 if file_change_requests:
                     return file_change_requests
             except RegexMatchError:
                 logger.warning("Failed to parse! Retrying...")
                 self.delete_messages_from_chat("files_to_change")
                 continue
         raise NoFilesException()
 
     def generate_pull_request(self, retries=5) -> PullRequest:
         for count in range(retries):
             too_long = False
             try:
                 logger.info(f"Generating for the {count}th time...")
-                if too_long or count == retries - 2: # if on last try, use gpt4-32k (improved context window)
+                if too_long or count == retries - 2:  # if on last try, use gpt4-32k (improved context window)
                     pr_text_response = self.chat(pull_request_prompt, message_key="pull_request")
                 else:
                     pr_text_response = self.chat(pull_request_prompt, message_key="pull_request", model=SECONDARY_MODEL)
 
                 # Add triple quotes if not present
                 if not pr_text_response.strip().endswith('"""'):
                     pr_text_response += '"""'
@@ -169,50 +171,54 @@
                     except GithubException:
                         pass
             else:
                 new_branch = self.repo.get_branch(branch)
                 if new_branch:
                     return new_branch.name
             raise e
-    
+
     def populate_snippets(self, snippets: list[Snippet]):
         for snippet in snippets:
             try:
-                snippet.content = self.repo.get_contents(snippet.file_path, SweepConfig.get_branch(self.repo)).decoded_content.decode("utf-8")
+                snippet.content = self.repo.get_contents(snippet.file_path,
+                                                         SweepConfig.get_branch(self.repo)).decoded_content.decode(
+                    "utf-8")
             except Exception as e:
                 logger.error(snippet)
-    
+
     def search_snippets(
-        self, 
-        query: str, 
-        installation_id: str,
-        num_snippets: int = 30,
+            self,
+            query: str,
+            installation_id: str,
+            num_snippets: int = 30,
     ) -> list[Snippet]:
-        get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
+        get_relevant_snippets = modal.Function.lookup(DB_MODAL_INST_NAME, "get_relevant_snippets")
         snippets: list[Snippet] = get_relevant_snippets.call(
-            self.repo.full_name, 
+            self.repo.full_name,
             query=query,
             n_results=num_snippets,
             installation_id=installation_id,
         )
         self.populate_snippets(snippets)
         return snippets
-    
+
     def validate_file_change_requests(self, file_change_requests: list[FileChangeRequest], branch: str = ""):
         for file_change_request in file_change_requests:
             try:
-                contents = self.repo.get_contents(file_change_request.filename, branch or SweepConfig.get_branch(self.repo))
+                contents = self.repo.get_contents(file_change_request.filename,
+                                                  branch or SweepConfig.get_branch(self.repo))
                 if contents:
                     file_change_request.change_type = "modify"
                 else:
                     file_change_request.change_type = "create"
             except:
                 file_change_request.change_type = "create"
         return file_change_requests
 
+
 class SweepBot(CodeGenBot, GithubBot):
     def cot_retrieval(self):
         # TODO(sweep): add semantic search using vector db
         # TODO(sweep): add search using webpilot + github
         functions = [
             Function(
                 name="cat",
@@ -220,24 +226,23 @@
                 parameters={
                     "properties": {
                         "filepath": {
                             "type": "string",
                             "description": "Paths to files. One per line."
                         },
                     }
-                } # manage file too large
+                }  # manage file too large
             ),
             Function(
                 name="finish",
                 description="Indicate you have sufficient data to proceed.",
-                parameters={"properties": {}} 
+                parameters={"properties": {}}
             ),
         ]
 
-
         # self.chat(
         #     cot_retrieval_prompt,
         #     message_key="cot_retrieval",
         #     functions=functions,
         # )
         # is_function_call = self.messages[-1].function_call is not None
         # for _retry in range(3):
@@ -296,15 +301,15 @@
                 # Todo: should we undo appending to file_change_paths?
                 logger.warning(f"Failed to parse. Retrying for the {count}th time...")
                 self.delete_messages_from_chat(key)
                 continue
         raise Exception("Failed to parse response after 5 attempts.")
 
     def modify_file(
-        self, file_change_request: FileChangeRequest, contents: str = "", branch = None
+            self, file_change_request: FileChangeRequest, contents: str = "", branch=None
     ) -> tuple[str, str]:
         if not contents:
             contents = self.get_file(
                 file_change_request.filename,
                 branch=branch
             ).decoded_content.decode("utf-8")
         # Add line numbers to the contents; goes in prompts but not github
@@ -363,38 +368,39 @@
 
                 try:
                     logger.info(f"modify_file_response: {modify_file_response}")
                     new_file = generate_new_file(modify_file_response, contents)
                     if not is_markdown(file_change_request.filename):
                         code_repairer = CodeRepairer(chat_logger=self.chat_logger)
                         diff = generate_diff(old_code=contents, new_code=new_file)
-                        new_file = code_repairer.repair_code(diff=diff, user_code=new_file, feature=file_change_request.instructions)
+                        new_file = code_repairer.repair_code(diff=diff, user_code=new_file,
+                                                             feature=file_change_request.instructions)
                     return (new_file, file_change_request.filename)
                 except Exception as e:
                     tb = traceback.format_exc()
                     logger.warning(f"Recieved error {e}\n{tb}")
                     logger.warning(
                         f"Failed to parse. Retrying for the {count}th time..."
                     )
                     self.delete_messages_from_chat(key)
                     continue
         raise Exception("Failed to parse response after 5 attempts.")
- 
+
     def change_file(self, file_change_request: FileChangeRequest):
         if file_change_request.change_type == "create":
             return self.create_file(file_change_request)
         elif file_change_request.change_type == "modify":
             return self.create_file(file_change_request)
         else:
             raise Exception("Not a valid file type")
-        
+
     def change_files_in_github(
-        self,
-        file_change_requests: list[FileChangeRequest],
-        branch: str,
+            self,
+            file_change_requests: list[FileChangeRequest],
+            branch: str,
     ):
         # should check if branch exists, if not, create it
         logger.debug(file_change_requests)
         num_fcr = len(file_change_requests)
         completed = 0
         for file_change_request in file_change_requests:
             try:
```

### Comparing `sweepai-0.4.2/sweepai/core/vector_db.py` & `sweepai-0.4.3/sweepai/core/vector_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,87 @@
+import glob
 import json
 import os
 import re
-import time
 import shutil
-import glob
+import time
 
-from modal import stub
-from loguru import logger
-from redis import Redis
-from tqdm import tqdm
 import modal
-from modal import method
 from deeplake.core.vectorstore.deeplake_vectorstore import DeepLakeVectorStore
+from git.repo import Repo
 from github import Github
-from git import Repo
+from loguru import logger
+from modal import method
+from redis import Redis
+from tqdm import tqdm
 
 from sweepai.core.entities import Snippet
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.hash import hash_sha256
 from sweepai.utils.scorer import compute_score, convert_to_percentiles
-
+from ..utils.config.client import SweepConfig
+from ..utils.config.server import ENV, DB_MODAL_INST_NAME, UTILS_MODAL_INST_NAME, REDIS_URL, BOT_TOKEN_NAME
 from ..utils.github_utils import get_token
-from ..utils.constants import DB_NAME, BOT_TOKEN_NAME, ENV, UTILS_NAME
-from ..utils.config import SweepConfig
-import time
 
 # TODO: Lots of cleanups can be done here with these constants
-stub = modal.Stub(DB_NAME)
-chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
+stub = modal.Stub(DB_MODAL_INST_NAME)
+chunker = modal.Function.lookup(UTILS_MODAL_INST_NAME, "Chunking.chunk")
 model_volume = modal.SharedVolume().persist(f"{ENV}-storage")
 MODEL_DIR = "/root/cache/model"
 DEEPLAKE_DIR = "/root/cache/"
 DISKCACHE_DIR = "/root/cache/diskcache/"
 DEEPLAKE_FOLDER = "deeplake/"
 BATCH_SIZE = 256
 SENTENCE_TRANSFORMERS_MODEL = "sentence-transformers/all-MiniLM-L12-v2"
-timeout = 60 * 30 # 30 minutes
+timeout = 60 * 30  # 30 minutes
 CACHE_VERSION = "v1.0.0"
 MAX_FILES = 3000
 
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
     .pip_install("deeplake==3.6.3", "sentence-transformers")
-    .pip_install("openai", "PyGithub", "loguru", "docarray", "GitPython", "tqdm", "highlight-io", "anthropic", "posthog", "redis", "pyyaml")
+    .pip_install("openai", "PyGithub", "loguru", "docarray", "GitPython", "tqdm", "highlight-io", "anthropic",
+                 "posthog", "redis", "pyyaml")
 )
 secrets = [
     modal.Secret.from_name(BOT_TOKEN_NAME),
+    modal.Secret.from_name("github"),
     modal.Secret.from_name("openai-secret"),
     modal.Secret.from_name("huggingface"),
     modal.Secret.from_name("chroma-endpoint"),
     modal.Secret.from_name("posthog"),
     modal.Secret.from_name("highlight"),
     modal.Secret.from_name("redis_url"),
     modal.Secret.from_dict({"TRANSFORMERS_CACHE": MODEL_DIR}),
 ]
 
+
 def init_deeplake_vs(repo_name):
     deeplake_repo_path = f"mem://{DEEPLAKE_FOLDER}{repo_name}"
-    deeplake_vector_store = DeepLakeVectorStore(path = deeplake_repo_path)
+    deeplake_vector_store = DeepLakeVectorStore(path=deeplake_repo_path)
     return deeplake_vector_store
 
+
 def parse_collection_name(name: str) -> str:
     # Replace any non-alphanumeric characters with hyphens
     name = re.sub(r"[^\w-]", "--", name)
     # Ensure the name is between 3 and 63 characters and starts/ends with alphanumeric
     name = re.sub(r"^(-*\w{0,61}\w)-*$", r"\1", name[:63].ljust(3, "x"))
     return name
 
+
 @stub.cls(
     image=image,
     secrets=secrets,
     shared_volumes={MODEL_DIR: model_volume},
     keep_warm=1 if ENV == "prod" else 0,
     gpu="T4",
-    retries=modal.Retries(max_retries=5, backoff_coefficient=2, initial_delay=5),
+    retries=modal.Retries(
+        max_retries=5, backoff_coefficient=2, initial_delay=5),
 )
 class Embedding:
     def __enter__(self):
         from sentence_transformers import SentenceTransformer
 
         self.model = SentenceTransformer(
             SENTENCE_TRANSFORMERS_MODEL, cache_folder=MODEL_DIR
@@ -88,77 +91,97 @@
     def compute(self, texts: list[str]):
         return self.model.encode(texts, batch_size=BATCH_SIZE).tolist()
 
     @method()
     def ping(self):
         return "pong"
 
+
 class ModalEmbeddingFunction():
     def __init__(self):
         pass
 
     def __call__(self, texts):
         return Embedding.compute.call(texts)
 
+
 embedding_function = ModalEmbeddingFunction()
 
+
 def get_deeplake_vs_from_repo(
-    repo_name: str,
-    sweep_config: SweepConfig = SweepConfig(),
-    installation_id: int = None,
-    branch_name: str = None,
+        repo_name: str,
+        installation_id: int,
+        branch_name: str | None = None,
+        sweep_config: SweepConfig = SweepConfig(),
 ):
     token = get_token(installation_id)
     g = Github(token)
     repo = g.get_repo(repo_name)
     commits = repo.get_commits()
     commit_hash = commits[0].sha
-    cache_success = True
-    try:
-        cache = Redis.from_url(os.environ.get("redis_url"))
-        logger.info(f"Succesfully got cache for {repo_name}")
-    except:
-        cache_success = False
-        logger.info(f"Failed to get cache for {repo_name}")
-    if cache_success:
+
+    cache_success = False
+    cache_inst = None
+
+    if REDIS_URL is not None:
+        try:
+            # todo: initialize once
+            cache_inst = Redis.from_url(REDIS_URL)
+            logger.info(f"Successfully connected to redis cache")
+            cache_success = True
+        except:
+            cache_success = False
+            logger.error(f"Failed to connect to redis cache")
+    else:
+        logger.warning(f"REDIS_URL is None, skipping cache")
+
+    if cache_inst and cache_success:
+
         try:
             github_cache_key = f"github-{commit_hash}{CACHE_VERSION}"
-            deeplake_items = json.loads(cache.get(github_cache_key))
+            cache_hit = cache_inst.get(github_cache_key)
+            if cache_hit:
+                deeplake_items = json.loads(cache_hit)
+                logger.info(f"Cache hit for {repo_name}")
+            else:
+                deeplake_items = None
+                logger.info(f"Cache miss for {repo_name}")
+
             if deeplake_items:
                 deeplake_vs = init_deeplake_vs(repo_name)
                 deeplake_vs.add(
-                    text = deeplake_items['ids'],
-                    embedding = deeplake_items['embeddings'],
-                    metadata = deeplake_items['metadatas']
+                    text=deeplake_items['ids'],
+                    embedding=deeplake_items['embeddings'],
+                    metadata=deeplake_items['metadatas']
                 )
                 logger.info(f"Returning deeplake vs for {repo_name}")
                 return deeplake_vs
             else:
                 logger.info(f"Cache for {repo_name} is empty")
         except:
             logger.info(f"Failed to get cache for {repo_name}")
     logger.info(f"Downloading repository and indexing for {repo_name}...")
     start = time.time()
     logger.info("Recursively getting list of files...")
 
     repo_url = f"https://x-access-token:{token}@github.com/{repo_name}.git"
     shutil.rmtree("repo", ignore_errors=True)
-    
+
     branch_name = SweepConfig.get_branch(repo)
 
     git_repo = Repo.clone_from(repo_url, "repo")
     git_repo.git.checkout(branch_name)
 
     file_list = glob.iglob("repo/**", recursive=True)
     file_list = [
         file
         for file in tqdm(file_list)
         if os.path.isfile(file)
-        and all(not file.endswith(ext) for ext in sweep_config.exclude_exts)
-        and all(not file[len("repo/"):].startswith(dir_name) for dir_name in sweep_config.exclude_dirs)
+           and all(not file.endswith(ext) for ext in sweep_config.exclude_exts)
+           and all(not file[len("repo/"):].startswith(dir_name) for dir_name in sweep_config.exclude_dirs)
     ]
 
     file_paths = []
     file_contents = []
     scores = []
 
     for file in tqdm(file_list):
@@ -167,132 +190,142 @@
             for block in iter(lambda: f.read(1024), b''):
                 if b'\0' in block:
                     is_binary = True
                     break
             if is_binary:
                 logger.debug("Skipping binary file...")
                 continue
-        
+
         with open(file, "rb") as f:
             if len(f.read()) > sweep_config.max_file_limit:
                 logger.debug("Skipping large file...")
                 continue
 
         with open(file, "r") as f:
             # Can parallelize this
             try:
                 contents = f.read()
                 contents = file + contents
             except UnicodeDecodeError as e:
                 logger.warning(f"Received warning {e}, skipping...")
                 continue
-            file_path = file[len("repo/") :]
+            file_path = file[len("repo/"):]
             file_paths.append(file_path)
             file_contents.append(contents)
             if len(file_list) > MAX_FILES:
                 scores.append(1)
                 continue
             try:
                 cache_key = f"{repo_name}-{file_path}-{CACHE_VERSION}"
-                if cache_success:
-                    cached_value = cache.get(cache_key)
+                if cache_inst and cache_success:
+                    cached_value = cache_inst.get(cache_key)
                     if cached_value:
                         score = json.loads(cached_value)
                         scores.append(score)
                         continue
-                commits = list(repo.get_commits(path=file_path, sha=branch_name))
+                commits = list(repo.get_commits(
+                    path=file_path, sha=branch_name))
                 score = compute_score(contents, commits)
-                if cache_success:
-                    cache.set(cache_key, json.dumps(score), ex=60 * 60 * 2)
+                if cache_inst and cache_success:
+                    cache_inst.set(cache_key, json.dumps(score), ex=60 * 60 * 2)
                 scores.append(score)
             except Exception as e:
                 logger.warning(f"Received warning during scoring {e}, skipping...")
                 scores.append(1)
                 continue
     scores = convert_to_percentiles(scores)
-        
+
     chunked_results = chunker.map(file_contents, file_paths, scores, kwargs={
         "additional_metadata": {"repo_name": repo_name, "branch_name": branch_name}
     })
 
     documents, metadatas, ids = zip(*chunked_results)
     documents = [item for sublist in documents for item in sublist]
     metadatas = [item for sublist in metadatas for item in sublist]
     ids = [item for sublist in ids for item in sublist]
-    
+
     logger.info(f"Used {len(file_paths)} files...")
 
     shutil.rmtree("repo", ignore_errors=True)
-    logger.info(f"Getting list of all files took {time.time() -start}")
-    logger.info(f"Received {len(documents)} documents from repository {repo_name}")
+    logger.info(f"Getting list of all files took {time.time() - start}")
+    logger.info(
+        f"Received {len(documents)} documents from repository {repo_name}")
     collection_name = parse_collection_name(repo_name)
-    return compute_deeplake_vs(collection_name, documents, cache_success, cache, ids, metadatas, commit_hash)
-    
-def compute_deeplake_vs(collection_name, 
-                        documents, 
-                        cache_success, 
-                        cache, 
-                        ids, 
+    return compute_deeplake_vs(collection_name, documents, cache_success, cache_inst, ids, metadatas, commit_hash)
+
+
+def compute_deeplake_vs(collection_name,
+                        documents,
+                        cache_success,
+                        cache_inst,
+                        ids,
                         metadatas,
                         sha):
     deeplake_vs = init_deeplake_vs(collection_name)
     if len(documents) > 0:
         logger.info("Computing embeddings...")
         # Check cache here for all documents
         embeddings = [None] * len(documents)
-        if cache_success:
-            cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + CACHE_VERSION for doc in documents]
-            cache_values = cache.mget(cache_keys)
+        if cache_inst and cache_success:
+            cache_keys = [hash_sha256(
+                doc) + SENTENCE_TRANSFORMERS_MODEL + CACHE_VERSION for doc in documents]
+            cache_values = cache_inst.mget(cache_keys)
             for idx, value in enumerate(cache_values):
                 if value is not None:
                     embeddings[idx] = json.loads(value)
-        logger.info(f"Found {len([x for x in embeddings if x is not None])} embeddings in cache")
-        indices_to_compute = [idx for idx, x in enumerate(embeddings) if x is None]
+        logger.info(
+            f"Found {len([x for x in embeddings if x is not None])} embeddings in cache")
+        indices_to_compute = [idx for idx,
+        x in enumerate(embeddings) if x is None]
         documents_to_compute = [documents[idx] for idx in indices_to_compute]
 
         computed_embeddings = embedding_function(documents_to_compute)
 
         for idx, embedding in zip(indices_to_compute, computed_embeddings):
             embeddings[idx] = embedding
         deeplake_vs.add(
-            text = ids,
-            embedding = embeddings,
-            metadata = metadatas
+            text=ids,
+            embedding=embeddings,
+            metadata=metadatas
         )
-        if cache_success: cache.set(f"github-{sha}{CACHE_VERSION}", json.dumps({"metadatas": metadatas, "ids": ids, "embeddings": embeddings}))
-        if cache_success and len(documents_to_compute) > 0:
-            logger.info(f"Updating cache with {len(computed_embeddings)} embeddings")
-            cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + CACHE_VERSION for doc in documents_to_compute]
-            cache.mset({key: json.dumps(value) for key, value in zip(cache_keys, computed_embeddings)})
+        if cache_inst and cache_success:
+            cache_inst.set(f"github-{sha}{CACHE_VERSION}", json.dumps(
+                {"metadatas": metadatas, "ids": ids, "embeddings": embeddings}))
+        if cache_inst and cache_success and len(documents_to_compute) > 0:
+            logger.info(
+                f"Updating cache with {len(computed_embeddings)} embeddings")
+            cache_keys = [hash_sha256(
+                doc) + SENTENCE_TRANSFORMERS_MODEL + CACHE_VERSION for doc in documents_to_compute]
+            cache_inst.mset({key: json.dumps(value)
+                             for key, value in zip(cache_keys, computed_embeddings)})
         return deeplake_vs
     else:
         logger.error("No documents found in repository")
         return deeplake_vs
 
 
 @stub.function(image=image, secrets=secrets, shared_volumes={DISKCACHE_DIR: model_volume}, timeout=timeout)
 def update_index(
-    repo_name,
-    installation_id: int,
-    sweep_config: SweepConfig = SweepConfig(),
-) -> int:    
-    get_deeplake_vs_from_repo(
-    repo_name,
-    sweep_config,
-    installation_id)
+        repo_name,
+        installation_id: int,
+        sweep_config: SweepConfig = SweepConfig(),
+) -> int:
+    get_deeplake_vs_from_repo(repo_name, installation_id, branch_name=None, sweep_config=sweep_config)
+    # todo: ?
+    return 0
 
 
 @stub.function(image=image, secrets=secrets, shared_volumes={DEEPLAKE_DIR: model_volume}, timeout=timeout, keep_warm=1)
 def get_relevant_snippets(
-    repo_name: str,
-    query: str,
-    n_results: int,
-    installation_id: int,
-    username: str = None,
-    sweep_config: SweepConfig = SweepConfig(),
+        repo_name: str,
+        query: str,
+        n_results: int,
+        installation_id: int,
+        username: str | None = None,
+        sweep_config: SweepConfig = SweepConfig(),
 ):
     deeplake_vs = get_deeplake_vs_from_repo(
         repo_name=repo_name, installation_id=installation_id, sweep_config=sweep_config
     )
     results = {"metadata": [], "text": []}
     for n_result in range(n_results, 0, -1):
         try:
@@ -306,36 +339,36 @@
             username = "anonymous"
         posthog.capture(
             username,
             "failed",
             {
                 "reason": "Results query was empty",
                 "repo_name": repo_name,
-                "installation_id": installation_id, 
-                "query": query, 
+                "installation_id": installation_id,
+                "query": query,
                 "n_results": n_results
             },
         )
     metadatas = results["metadata"]
     code_scores = [metadata["score"] for metadata in metadatas]
     vector_scores = results["score"]
-    combined_scores = [code_score + vector_score for code_score, vector_score in zip(code_scores, vector_scores)]
+    combined_scores = [code_score + vector_score for code_score,
+    vector_score in zip(code_scores, vector_scores)]
     # Sort by combined scores
     # Combine the three lists into a single list of tuples
     combined_list = list(zip(combined_scores, metadatas))
 
     # Sort the combined list based on the combined scores
     sorted_list = sorted(combined_list, key=lambda x: x[0], reverse=True)
 
     # Extract the sorted metadatas and relevant_paths
     sorted_metadatas = [metadata for _, metadata in sorted_list]
     relevant_paths = [metadata["file_path"] for metadata in sorted_metadatas]
     logger.info("Relevant paths: {}".format(relevant_paths))
     return [
         Snippet(
             content="",
-            start=metadata["start"], 
-            end=metadata["end"], 
+            start=metadata["start"],
+            end=metadata["end"],
             file_path=file_path
         ) for metadata, file_path in zip(sorted_metadatas, relevant_paths)
     ]
-
```

### Comparing `sweepai-0.4.2/sweepai/events.py` & `sweepai-0.4.3/sweepai/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 from typing import Literal
+
 from pydantic import BaseModel
 
 
 class Installation(BaseModel):
     id: str
 
+
 class InstallationCreatedRequest(BaseModel):
     class Repository(BaseModel):
         full_name: str
+
     repositories: list[Repository]
     installation: Installation
 
+
 class ReposAddedRequest(BaseModel):
     class Repository(BaseModel):
         full_name: str
+
     repositories_added: list[Repository]
     installation: Installation
 
+
 class CommentCreatedRequest(BaseModel):
     class Comment(BaseModel):
         class User(BaseModel):
             login: str
+
         body: str | None
         original_line: int
         path: str
         diff_hunk: str
         user: User
 
     class PullRequest(BaseModel):
         class Head(BaseModel):
             ref: str
+
         number: int
         body: str | None
         state: str  # "closed" or "open"
         head: Head
         title: str
 
     class Repository(BaseModel):
@@ -60,15 +68,15 @@
         class Assignee(BaseModel):
             login: str
 
         class Repository(BaseModel):
             # TODO(sweep): Move this out
             full_name: str
             description: str | None
-        
+
         class Label(BaseModel):
             name: str
 
         class PullRequest(BaseModel):
             pass
 
         pull_request: PullRequest | None
@@ -82,50 +90,64 @@
 
     action: str
     issue: Issue
     repository: Issue.Repository
     assignee: Issue.Assignee | None
     installation: Installation
 
+
 class IssueCommentRequest(IssueRequest):
     class Comment(BaseModel):
         class User(BaseModel):
             login: str
             type: Literal["User", "Bot"]
+
         user: User
         id: int
         body: str
+
     comment: Comment
 
+
 class PRRequest(BaseModel):
     class PullRequest(BaseModel):
         class User(BaseModel):
             login: str
+
         class MergedBy(BaseModel):
             login: str
+
         user: User
         merged_by: MergedBy
+
     class Repository(BaseModel):
         full_name: str
+
     pull_request: PullRequest
     repository: Repository
 
+
 class CheckRunCompleted(BaseModel):
     class CheckRun(BaseModel):
         class PullRequest(BaseModel):
             number: int
+
         conclusion: str
         html_url: str
         pull_requests: list[PullRequest]
+
         @property
         def run_id(self):
             # format is like https://github.com/ORG/REPO_NAME/actions/runs/RUN_ID/jobs/JOB_ID
             return self.html_url.split("/")[-3]
+
     class Repository(BaseModel):
         full_name: str
         description: str | None
+
     class Sender(BaseModel):
         login: str
+
     check_run: CheckRun
     installation: Installation
     repository: Repository
-    sender: Sender
+    sender: Sender
```

### Comparing `sweepai-0.4.2/sweepai/handlers/create_pr.py` & `sweepai-0.4.3/sweepai/handlers/create_pr.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-import os
-import openai
-
-from loguru import logger
 import modal
+import openai
 from github.Repository import Repository
+from loguru import logger
 
 from sweepai.core.entities import FileChangeRequest, PullRequest
+from sweepai.utils.config.client import SweepConfig
+from sweepai.utils.config.server import GITHUB_DEFAULT_CONFIG, OPENAI_API_KEY, PREFIX, DB_MODAL_INST_NAME, GITHUB_BOT_TOKEN, \
+    GITHUB_BOT_USERNAME, \
+    GITHUB_CONFIG_BRANCH
 from sweepai.core.sweep_bot import SweepBot, MaxTokensExceeded
-from sweepai.handlers.on_review import review_pr
-from sweepai.utils.config import SweepConfig
 from sweepai.utils.event_logger import posthog
-from sweepai.utils.github_utils import get_github_client
-from sweepai.utils.constants import DB_NAME, PREFIX, DEFAULT_CONFIG, SWEEP_CONFIG_BRANCH, SWEEP_LOGIN
 
-github_access_token = os.environ.get("GITHUB_TOKEN")
-openai.api_key = os.environ.get("OPENAI_API_KEY")
+github_access_token = GITHUB_BOT_TOKEN
+openai.api_key = OPENAI_API_KEY
 
-update_index = modal.Function.lookup(DB_NAME, "update_index")
+update_index = modal.Function.lookup(DB_MODAL_INST_NAME, "update_index")
 
 num_of_snippets_to_query = 10
 max_num_of_snippets = 5
 
+
 def create_pr(
-    file_change_requests: list[FileChangeRequest],
-    pull_request: PullRequest,
-    sweep_bot: SweepBot,
-    username: str,
-    installation_id: int,
-    issue_number: int | None = None
+        file_change_requests: list[FileChangeRequest],
+        pull_request: PullRequest,
+        sweep_bot: SweepBot,
+        username: str,
+        installation_id: int,
+        issue_number: int | None = None
 ):
     # Flow:
     # 1. Get relevant files
     # 2: Get human message
     # 3. Get files to change
     # 4. Get file changes
     # 5. Create PR
@@ -114,53 +113,55 @@
                 **metadata,
             },
         )
         raise e
 
     posthog.capture(username, "success", properties={**metadata})
     logger.info("create_pr success")
-    sweep_bot.chat_logger.add_successful_ticket()
+    if sweep_bot.chat_logger is not None:
+        sweep_bot.chat_logger.add_successful_ticket()
     return {"success": True, "pull_request": pr}
 
+
 def safe_delete_sweep_branch(
-    pr, # Github PullRequest
-    repo: Repository,
+        pr,  # Github PullRequest
+        repo: Repository,
 ) -> bool:
     """
     Safely delete Sweep branch
     1. Only edited by Sweep
     2. Prefixed by sweep/
     """
     pr_commits = pr.get_commits()
     pr_commit_authors = set([commit.author.login for commit in pr_commits])
 
     # Check if only Sweep has edited the PR, and sweep/ prefix
     if len(pr_commit_authors) == 1 \
-            and SWEEP_LOGIN in pr_commit_authors \
+            and GITHUB_BOT_USERNAME in pr_commit_authors \
             and pr.head.ref.startswith("sweep/"):
         branch = repo.get_git_ref(f"heads/{pr.head.ref}")
         # pr.edit(state='closed')
         branch.delete()
         return True
     else:
         # Failed to delete branch as it was edited by someone else
         return False
 
 
 def create_config_pr(
         sweep_bot: SweepBot,
 ):
     title = "Create `sweep.yaml` Config File"
-    branch_name = SWEEP_CONFIG_BRANCH
+    branch_name = GITHUB_CONFIG_BRANCH
     branch_name = sweep_bot.create_branch(branch_name, retry=False)
     try:
         sweep_bot.repo.create_file(
             'sweep.yaml',
             'Create sweep.yaml config file',
-            DEFAULT_CONFIG.format(branch=sweep_bot.repo.default_branch),
+            GITHUB_DEFAULT_CONFIG.format(branch=sweep_bot.repo.default_branch),
             branch=branch_name
         )
     except Exception as e:
         logger.error(e)
 
     # Check if the pull request from this branch to main already exists.
     # If it does, then we don't need to create a new one.
@@ -173,22 +174,22 @@
     for pr in pull_requests:
         if pr.title == title:
             return pr
 
     pr = sweep_bot.repo.create_pull(
         title=title,
         body=
-"""🎉 Thank you for installing Sweep! We're thrilled to announce the latest update for Sweep, your trusty AI junior developer on GitHub. This PR creates a `sweep.yaml` config file, allowing you to personalize Sweep's performance according to your project requirements.
-
-## What's new?
-- **Sweep is now configurable**. 
-- To configure Sweep, simply edit the `sweep.yaml` file in the root of your repository.
-- If you need help, check out the [Sweep Default Config](https://github.com/sweepai/sweep/blob/main/sweep.yaml) or [Join Our Discord](https://discord.gg/sweep-ai) for help.
-
-If you would like me to stop creating this PR, go to issues and say "Sweep: create an empty `sweep.yaml` file".
-Thank you for using Sweep! 🧹
-""",
+        """🎉 Thank you for installing Sweep! We're thrilled to announce the latest update for Sweep, your trusty AI junior developer on GitHub. This PR creates a `sweep.yaml` config file, allowing you to personalize Sweep's performance according to your project requirements.
+        
+        ## What's new?
+        - **Sweep is now configurable**. 
+        - To configure Sweep, simply edit the `sweep.yaml` file in the root of your repository.
+        - If you need help, check out the [Sweep Default Config](https://github.com/sweepai/sweep/blob/main/sweep.yaml) or [Join Our Discord](https://discord.gg/sweep-ai) for help.
+        
+        If you would like me to stop creating this PR, go to issues and say "Sweep: create an empty `sweep.yaml` file".
+        Thank you for using Sweep! 🧹
+        """,
         head=branch_name,
         base=SweepConfig.get_branch(sweep_bot.repo),
     )
 
-    return pr
+    return pr
```

### Comparing `sweepai-0.4.2/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.3/sweepai/handlers/on_check_suite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import io
 import os
 import zipfile
-from loguru import logger
+
 import openai
 import requests
-from sweepai.core.gha_extraction import GHAExtractor
+from loguru import logger
 
+from sweepai.core.gha_extraction import GHAExtractor
 from sweepai.events import CheckRunCompleted
-from sweepai.utils.config import SweepConfig
+from sweepai.utils.config.client import SweepConfig, get_gha_enabled
 from sweepai.utils.github_utils import get_github_client, get_token
 
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 
-
 def download_logs(repo_full_name: str, run_id: int, installation_id: int):
-    headers={
+    headers = {
         "Accept": "application/vnd.github+json",
         "Authorization": f"Bearer {get_token(installation_id)}",
         "X-GitHub-Api-Version": "2022-11-28"
     }
-    response = requests.get(f"https://api.github.com/repos/{repo_full_name}/actions/runs/{run_id}/logs", headers=headers)
+    response = requests.get(f"https://api.github.com/repos/{repo_full_name}/actions/runs/{run_id}/logs",
+                            headers=headers)
 
     logs_str = ""
     if response.status_code == 200:
         zip_file = zipfile.ZipFile(io.BytesIO(response.content))
         for file in zip_file.namelist():
             if "/" not in file:
                 with zip_file.open(file) as f:
                     logs_str += f.read().decode("utf-8")
     else:
         logger.warning(f"Failed to download logs for run id: {run_id}")
     return logs_str
 
+
 def clean_logs(logs_str: str):
     log_list = logs_str.split("\n")
     truncated_logs = [log[log.find(" ") + 1:] for log in log_list]
     patterns = [
         # for docker
         "Already exists",
         "Pulling fs layer",
@@ -48,26 +50,27 @@
         "remote: Counting objects",
         "remote: Compressing objects:",
         "Receiving objects:",
         "Resolving deltas:"
     ]
     return "\n".join([log.strip() for log in truncated_logs if not any(pattern in log for pattern in patterns)])
 
+
 def on_check_suite(request: CheckRunCompleted):
     g = get_github_client(request.installation.id)
     repo = g.get_repo(request.repository.full_name)
-    if not SweepConfig.get_gha_enabled(repo):
+    if not get_gha_enabled(repo):
         return None
     pr = repo.get_pull(request.check_run.pull_requests[0].number)
     num_pr_commits = len(list(pr.get_commits()))
     if num_pr_commits > 20:
         return None
-    logger.info(f"Running github action for PR with {num_pr_commits } commits")
+    logger.info(f"Running github action for PR with {num_pr_commits} commits")
     logs = download_logs(
-        request.repository.full_name, 
+        request.repository.full_name,
         request.check_run.run_id,
         request.installation.id
     )
     if not logs:
         return None
     logs = clean_logs(logs)
     extractor = GHAExtractor()
```

### Comparing `sweepai-0.4.2/sweepai/handlers/on_comment.py` & `sweepai-0.4.3/sweepai/handlers/on_comment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
 On Github ticket, get ChatGPT to deal with it
 """
 
 # TODO: Add file validation
 
-import os
-import openai
 import traceback
 
+import openai
 from loguru import logger
 
 from sweepai.core.entities import NoFilesException, Snippet
 from sweepai.core.sweep_bot import SweepBot
 from sweepai.handlers.on_review import get_pr_diffs
+from sweepai.utils.chat_logger import ChatLogger
+from sweepai.utils.config.server import PREFIX, OPENAI_API_KEY, GITHUB_BOT_TOKEN
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import (
     get_github_client,
     search_snippets,
 )
 from sweepai.utils.prompt_constructor import HumanMessageCommentPrompt
-from sweepai.utils.constants import PREFIX
-from sweepai.utils.chat_logger import ChatLogger
 
-github_access_token = os.environ.get("GITHUB_TOKEN")
-openai.api_key = os.environ.get("OPENAI_API_KEY")
+github_access_token = GITHUB_BOT_TOKEN
+openai.api_key = OPENAI_API_KEY
 
 num_of_snippets_to_query = 30
 total_number_of_snippet_tokens = 15_000
 num_full_files = 2
 num_extended_snippets = 2
 
+
 def post_process_snippets(snippets: list[Snippet], max_num_of_snippets: int = 3):
     for snippet in snippets[:num_full_files]:
         snippet = snippet.expand()
 
     # snippet fusing
     i = 0
     while i < len(snippets):
@@ -52,75 +52,78 @@
     for snippet in snippets:
         total_length += len(snippet.get_snippet())
         if total_length > total_number_of_snippet_tokens * 5:
             break
         result_snippets.append(snippet)
     return result_snippets[:max_num_of_snippets]
 
+
 def on_comment(
-    repo_full_name: str,
-    repo_description: str,
-    comment: str,
-    pr_path: str | None,
-    pr_line_position: int | None,
-    username: str,
-    installation_id: int,
-    pr_number: int = None,
+        repo_full_name: str,
+        repo_description: str,
+        comment: str,
+        pr_path: str | None,
+        pr_line_position: int | None,
+        username: str,
+        installation_id: int,
+        pr_number: int = None,
 ):
     # Check if the comment is "REVERT"
     if comment.strip().upper() == "REVERT":
         rollback_file(repo_full_name, pr_path, installation_id, pr_number)
         return {"success": True, "message": "File has been reverted to the previous commit."}
 
     # Flow:
     # 1. Get relevant files
     # 2: Get human message
     # 3. Get files to change
     # 4. Get file changes
     # 5. Create PR
-    logger.info(f"Calling on_comment() with the following arguments: {comment}, {repo_full_name}, {repo_description}, {pr_path}")
+    logger.info(
+        f"Calling on_comment() with the following arguments: {comment}, {repo_full_name}, {repo_description}, {pr_path}")
     organization, repo_name = repo_full_name.split("/")
     metadata = {
         "repo_full_name": repo_full_name,
         "repo_name": repo_name,
         "organization": organization,
         "repo_description": repo_description,
         "installation_id": installation_id,
         "username": username,
         "function": "on_comment",
         "mode": PREFIX,
     }
 
     posthog.capture(username, "started", properties=metadata)
     logger.info(f"Getting repo {repo_full_name}")
+    file_comment = pr_path and pr_line_position
     try:
         g = get_github_client(installation_id)
         repo = g.get_repo(repo_full_name)
         pr = repo.get_pull(pr_number)
         # Check if the PR is closed
         if pr.state == "closed":
             return {"success": True, "message": "PR is closed. No event fired."}
         branch_name = pr.head.ref
         pr_title = pr.title
         pr_body = pr.body
         diffs = get_pr_diffs(repo, pr)
         pr_line = None
         pr_file_path = None
         # This means it's a comment on a file
-        if pr_path and pr_line_position:
+        if file_comment:
             pr_file = repo.get_contents(pr_path, ref=branch_name).decoded_content.decode("utf-8")
             pr_lines = pr_file.splitlines()
             pr_line = pr_lines[min(len(pr_lines), pr_line_position) - 1]
             pr_file_path = pr_path.strip()
         # This means it's a comment on the PR
         else:
             if not comment.strip().lower().startswith("sweep"):
                 logger.info("No event fired because it doesn't start with Sweep.")
                 return {"success": True, "message": "No event fired."}
-            
+
         def fetch_file_contents_with_retry():
             retries = 3
             error = None
             for i in range(retries):
                 try:
                     logger.info(f"Fetching relevant files for the {i}th time...")
                     return search_snippets(
@@ -133,22 +136,22 @@
                 except Exception as e:
                     error = e
                     continue
             posthog.capture(
                 username, "fetching_failed", properties={"error": error, **metadata}
             )
             raise error
+
         snippets, tree = fetch_file_contents_with_retry()
         logger.info("Fetching relevant files...")
         try:
             snippets, tree = fetch_file_contents_with_retry()
             assert len(snippets) > 0
         except Exception as e:
             logger.error(traceback.format_exc())
-            logger.error(e)
             raise e
         chat_logger = ChatLogger({
             'repo_name': repo_name,
             'title': '(Comment) ' + pr_title,
             "issue_url": pr.html_url,
             "pr_file_path": pr_file_path,  # may be None
             "pr_line": pr_line,  # may be None
@@ -158,30 +161,30 @@
             "pr_path": pr_path,
             "pr_line_position": pr_line_position,
             "username": username,
             "installation_id": installation_id,
             "pr_number": pr_number,
             "type": "comment",
         })
-        snippets = post_process_snippets(snippets, max_num_of_snippets=2)
+        snippets = post_process_snippets(snippets, max_num_of_snippets=0 if file_comment else 2)
 
         logger.info("Getting response from ChatGPT...")
         human_message = HumanMessageCommentPrompt(
             comment=comment,
             repo_name=repo_name,
             repo_description=repo_description if repo_description else "",
             diffs=diffs,
             issue_url=pr.html_url,
             username=username,
             title=pr_title,
             tree=tree,
             summary=pr_body,
             snippets=snippets,
-            pr_file_path=pr_file_path, # may be None
-            pr_line=pr_line, # may be None
+            pr_file_path=pr_file_path,  # may be None
+            pr_line=pr_line,  # may be None
         )
         logger.info(f"Human prompt{human_message.construct_prompt()}")
 
         sweep_bot = SweepBot.from_system_message_content(
             # human_message=human_message, model="claude-v1.3-100k", repo=repo
             human_message=human_message, repo=repo, chat_logger=chat_logger, model="gpt-4-32k-0613"
         )
@@ -218,41 +221,43 @@
         })
         raise e
 
     posthog.capture(username, "success", properties={**metadata})
     logger.info("on_comment success")
     return {"success": True}
 
+
 def rollback_file(repo_full_name, pr_path, installation_id, pr_number):
     g = get_github_client(installation_id)
     repo = g.get_repo(repo_full_name)
     pr = repo.get_pull(pr_number)
     branch_name = pr.head.ref
 
     # Get the file's content from the previous commit
     commits = repo.get_commits(sha=branch_name)
     if commits.totalCount < 2:
         current_file = repo.get_contents(pr_path, ref=commits[0].sha)
         current_file_sha = current_file.sha
         previous_content = repo.get_contents(pr_path, ref=repo.default_branch)
         previous_file_content = previous_content.decoded_content.decode("utf-8")
-        repo.update_file(pr_path, "Revert file to previous commit", previous_file_content, current_file_sha, branch=branch_name)
+        repo.update_file(pr_path, "Revert file to previous commit", previous_file_content, current_file_sha,
+                         branch=branch_name)
         return
     previous_commit = commits[1]
-    
+
     # Get current file SHA
     current_file = repo.get_contents(pr_path, ref=commits[0].sha)
     current_file_sha = current_file.sha
 
     # Check if the file exists in the previous commit
     try:
         previous_content = repo.get_contents(pr_path, ref=previous_commit.sha)
         previous_file_content = previous_content.decoded_content.decode("utf-8")
         # Create a new commit with the previous file content
-        repo.update_file(pr_path, "Revert file to previous commit", previous_file_content, current_file_sha, branch=branch_name)
+        repo.update_file(pr_path, "Revert file to previous commit", previous_file_content, current_file_sha,
+                         branch=branch_name)
     except Exception as e:
         logger.error(traceback.format_exc())
         if e.status == 404:
             logger.warning(f"File {pr_path} was not found in previous commit {previous_commit.sha}")
         else:
             raise e
-
```

### Comparing `sweepai-0.4.2/sweepai/handlers/on_review.py` & `sweepai-0.4.3/sweepai/handlers/on_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Take a PR and provide an AI generated review of the PR.
 """
 from loguru import logger
+
 from sweepai.core.entities import DiffSummarization, PullRequestComment
 from sweepai.core.prompts import review_prompt
 from sweepai.core.sweep_bot import SweepBot
-
-from sweepai.utils.github_utils import get_file_contents
-from sweepai.utils.prompt_constructor import HumanMessageFinalPRComment, HumanMessagePromptReview, HumanMessageReviewFollowup
 from sweepai.utils.chat_logger import ChatLogger
+from sweepai.utils.github_utils import get_file_contents
+from sweepai.utils.prompt_constructor import HumanMessageFinalPRComment, HumanMessagePromptReview, \
+    HumanMessageReviewFollowup
+
 
 # Plan:
 # 1. Get PR
 # 2. Get files changed
 # 3. Come up with some comments for the PR
 # 4. Take comments and add them to the PR
 
@@ -26,21 +28,23 @@
     pr_diffs = []
     for file in file_diffs:
         print(file.status)
         diff = file.patch
         if file.status == "added":
             pr_diffs.append((file.filename, get_file_contents(repo, file_path=file.filename, ref=head_sha), "", diff))
         elif file.status == "modified":
-            pr_diffs.append((file.filename, get_file_contents(repo, file_path=file.filename, ref=head_sha), get_file_contents(repo, file_path=file.filename, ref=base_sha), diff))
+            pr_diffs.append((file.filename, get_file_contents(repo, file_path=file.filename, ref=head_sha),
+                             get_file_contents(repo, file_path=file.filename, ref=base_sha), diff))
         elif file.status == "removed":
             pr_diffs.append((file.filename, "", get_file_contents(repo, file_path=file.filename, ref=base_sha), diff))
         else:
-            logger.info(f"File status {file.status} not recognized") #TODO(sweep): We don't handle renamed files
+            logger.info(f"File status {file.status} not recognized")  # TODO(sweep): We don't handle renamed files
     return pr_diffs
 
+
 def review_pr(repo, pr, issue_url, username, repo_description, title, summary, replies_text, tree):
     repo_name = repo.full_name
     logger.info("Getting PR diffs...")
     diffs = get_pr_diffs(repo, pr)
     human_message = HumanMessagePromptReview(
         repo_name=repo_name,
         issue_url=issue_url,
```

### Comparing `sweepai-0.4.2/sweepai/handlers/on_ticket.py` & `sweepai-0.4.3/sweepai/handlers/on_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 '''
 On Github ticket, get ChatGPT to deal with it
 '''
 
 # TODO: Add file validation
 
-import os
-import openai
+import traceback
 
-from loguru import logger
 import modal
+import openai
+from loguru import logger
 from tabulate import tabulate
-import traceback
 
-from sweepai.core.entities import FileChangeRequest, Snippet, NoFilesException
-from sweepai.core.prompts import (
-    reply_prompt,
-)
+from sweepai.core.entities import Snippet, NoFilesException
 from sweepai.core.sweep_bot import SweepBot, MaxTokensExceeded
 from sweepai.core.prompts import issue_comment_prompt
 from sweepai.handlers.create_pr import create_pr, create_config_pr, safe_delete_sweep_branch
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_review import review_pr
+from sweepai.utils.chat_logger import ChatLogger, discord_log_error
+from sweepai.utils.config.client import SweepConfig
+from sweepai.utils.config.server import PREFIX, DB_MODAL_INST_NAME, UTILS_MODAL_INST_NAME, OPENAI_API_KEY, \
+    GITHUB_BOT_TOKEN, \
+    GITHUB_BOT_USERNAME
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, search_snippets
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
-from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME, SWEEP_LOGIN
-from sweepai.utils.chat_logger import ChatLogger, discord_log_error
-from sweepai.utils.config import SweepConfig
 
-github_access_token = os.environ.get("GITHUB_TOKEN")
-openai.api_key = os.environ.get("OPENAI_API_KEY")
+github_access_token = GITHUB_BOT_TOKEN
+openai.api_key = OPENAI_API_KEY
 
-update_index = modal.Function.lookup(DB_NAME, "update_index")
+update_index = modal.Function.lookup(DB_MODAL_INST_NAME, "update_index")
 
 sep = "\n---\n"
 bot_suffix_starring = "⭐ If you are enjoying Sweep, please [star our repo](https://github.com/sweepai/sweep) so more people can hear about us!"
 bot_suffix = f"\n{sep}I'm a bot that handles simple bugs and feature requests but I might make mistakes. Please be kind!"
 discord_suffix = f'\n<sup>[Join Our Discord](https://discord.com/invite/sweep-ai)'
 
 stars_suffix = "⭐ In the meantime, consider [starring our repo](https://github.com/sweepai/sweep) so more people can hear about us!"
@@ -44,21 +42,22 @@
 <details>
   <summary>{summary}</summary>
 
   {body}
 </details>
 '''
 
-chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
+chunker = modal.Function.lookup(UTILS_MODAL_INST_NAME, "Chunking.chunk")
 
 num_of_snippets_to_query = 30
 total_number_of_snippet_tokens = 15_000
 num_full_files = 2
 num_extended_snippets = 2
 
+
 def post_process_snippets(snippets: list[Snippet], max_num_of_snippets: int = 5):
     for snippet in snippets[:num_full_files]:
         snippet = snippet.expand()
 
     # snippet fusing
     i = 0
     while i < len(snippets):
@@ -77,24 +76,25 @@
     for snippet in snippets:
         total_length += len(snippet.get_snippet())
         if total_length > total_number_of_snippet_tokens * 5:
             break
         result_snippets.append(snippet)
     return result_snippets[:max_num_of_snippets]
 
+
 def on_ticket(
-    title: str,
-    summary: str,
-    issue_number: int,
-    issue_url: str,
-    username: str,
-    repo_full_name: str,
-    repo_description: str,
-    installation_id: int,
-    comment_id: int = None
+        title: str,
+        summary: str,
+        issue_number: int,
+        issue_url: str,
+        username: str,
+        repo_full_name: str,
+        repo_description: str,
+        installation_id: int,
+        comment_id: int = None
 ):
     # Check if the title starts with "sweep" or "sweep: " and remove it
     if title.lower().startswith("sweep: "):
         title = title[7:]
     elif title.lower().startswith("sweep "):
         title = title[6:]
 
@@ -125,25 +125,24 @@
     if current_issue.state == 'closed':
         posthog.capture(username, "issue_closed", properties=metadata)
         return {"success": False, "reason": "Issue is closed"}
     item_to_react_to = current_issue.get_comment(comment_id) if comment_id else current_issue
     replies_text = ""
     comments = list(current_issue.get_comments())
     if comment_id:
-        
         logger.info(f"Replying to comment {comment_id}...")
         replies_text = "\nComments:\n" + "\n".join(
             [
                 issue_comment_prompt.format(
                     username=comment.user.login,
                     reply=comment.body,
                 ) for comment in comments if comment.user.type == "User"
             ]
         )
-    
+
     chat_logger = ChatLogger({
         'repo_name': repo_name,
         'title': title,
         'summary': summary + replies_text,
         "issue_number": issue_number,
         "issue_url": issue_url,
         "username": username,
@@ -155,83 +154,89 @@
 
     # Check if branch was already created for this issue
     preexisting_branch = None
     prs = repo.get_pulls(state='open', sort='created', base=SweepConfig.get_branch(repo))
     for pr in prs:
         # Check if this issue is mentioned in the PR, and pr is owned by bot
         # This is done in create_pr, (pr_description = ...)
-        if pr.user.login == SWEEP_LOGIN and f'Fixes #{issue_number}.\n' in pr.body:
+        if pr.user.login == GITHUB_BOT_USERNAME and f'Fixes #{issue_number}.\n' in pr.body:
             success = safe_delete_sweep_branch(pr, repo)
 
     # Add emojis
     eyes_reaction = item_to_react_to.create_reaction("eyes")
     # If SWEEP_BOT reacted to item_to_react_to with "rocket", then remove it.
     reactions = item_to_react_to.get_reactions()
     for reaction in reactions:
-        if reaction.content == "rocket" and reaction.user.login == SWEEP_LOGIN:
+        if reaction.content == "rocket" and reaction.user.login == GITHUB_BOT_USERNAME:
             item_to_react_to.delete_reaction(reaction.id)
 
     # Creates progress bar ASCII for 0-5 states
     progress_headers = [
         None,
         "Step 1: 🔍 Code Search",
         "Step 2: 🧐 Snippet Analysis",
         "Step 3: 📝 Planning",
         "Step 4: ⌨️ Coding",
         "Step 5: 🔁 Code Review"
     ]
 
     config_pr_url = None
+
     def get_comment_header(index, errored=False, pr_message=""):
-        config_pr_message = ("\n" + f"* Install Sweep Configs: [Pull Request]({config_pr_url})" if config_pr_url is not None else "")
+        config_pr_message = (
+            "\n" + f"* Install Sweep Configs: [Pull Request]({config_pr_url})" if config_pr_url is not None else "")
         if index < 0: index = 0
         if index == 5:
             return pr_message + config_pr_message
         index *= 20
         index = min(100, index)
         if errored:
             return f"![{index}%](https://progress-bar.dev/{index}/?&title=Errored&width=600)"
-        return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + ("\n" + stars_suffix + config_pr_message if index != -1 else "")
+        return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + (
+            "\n" + stars_suffix + config_pr_message if index != -1 else "")
 
     # Find the first comment made by the bot
     issue_comment = None
     is_paying_user = chat_logger.is_paying_user()
     tickets_allocated = 60 if is_paying_user else 3
     ticket_count = max(tickets_allocated - chat_logger.get_ticket_count(), 0)
     use_faster_model = chat_logger.use_faster_model()
     payment_message = f"To create this ticket, I used {'gpt-3.5. ' if use_faster_model else 'gpt-4. '}You have {ticket_count} gpt-4 tickets left." + (" For more gpt-4 tickets, visit [our payment portal.](https://buy.stripe.com/fZe03512h99u0AE6os)" if not is_paying_user else "")
     first_comment = f"{get_comment_header(0)}\n{sep}I am currently looking into this ticket!. I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.\n{sep}## {progress_headers[1]}\nWorking on it...{bot_suffix}{discord_suffix}"
     for comment in comments:
-        if comment.user.login == SWEEP_LOGIN:
+        if comment.user.login == GITHUB_BOT_USERNAME:
             issue_comment = comment
             issue_comment.edit(first_comment)
             break
     if issue_comment is None:
         issue_comment = current_issue.create_comment(first_comment)
 
     # Comment edit function
     past_messages = {}
     current_index = {}
-    def edit_sweep_comment(message: str, index: int, pr_message = ""):
+
+    def edit_sweep_comment(message: str, index: int, pr_message=""):
         nonlocal current_index
         # -1 = error, -2 = retry
         # Only update the progress bar if the issue generation errors.
         errored = (index == -1)
         if index >= 0:
             past_messages[index] = message
             current_index = index
 
         agg_message = None
         # Include progress history
         # index = -2 is reserved for
-        for i in range(current_index + 2): # go to next header (for Working on it... text)
-            if i == 0 or i >= len(progress_headers): continue # skip None header
+        for i in range(current_index + 2):  # go to next header (for Working on it... text)
+            if i == 0 or i >= len(progress_headers): continue  # skip None header
             header = progress_headers[i]
-            if header is not None: header = "## " + header + "\n"
-            else: header = "No header\n"
+            if header is not None:
+                header = "## " + header + "\n"
+            else:
+                header = "No header\n"
             msg = header + (past_messages.get(i) or "Working on it...")
             if agg_message is None:
                 agg_message = msg
             else:
                 agg_message = agg_message + f"\n{sep}" + msg
 
         suffix = bot_suffix + discord_suffix
@@ -277,34 +282,35 @@
         logger.error(trace)
         edit_sweep_comment(
             "It looks like an issue has occured around fetching the files. Perhaps the repo has not been initialized: try removing this repo and adding it back. I'll try again in a minute. If this error persists contact team@sweep.dev.",
             -1
         )
         log_error("File Fetch", str(e) + "\n" + traceback.format_exc())
         raise e
-    
-    snippets = post_process_snippets(snippets, 
+
+    snippets = post_process_snippets(snippets)
+
+    snippets = post_process_snippets(snippets,
                                      max_num_of_snippets=2 if use_faster_model else 5)
 
     human_message = HumanMessagePrompt(
         repo_name=repo_name,
         issue_url=issue_url,
         username=username,
         repo_description=repo_description,
         title=title,
         summary=summary + replies_text,
         snippets=snippets,
-        tree=tree, # TODO: Anything in repo tree that has something going through is expanded
+        tree=tree,  # TODO: Anything in repo tree that has something going through is expanded
     )
 
     sweep_bot = SweepBot.from_system_message_content(
         human_message=human_message, repo=repo, is_reply=bool(comments), chat_logger=chat_logger
     )
 
-
     # Check repository for sweep.yml file.
     sweep_yml_exists = False
     for content_file in repo.get_contents(""):
         if content_file.name == "sweep.yaml":
             sweep_yml_exists = True
             break
 
@@ -316,15 +322,14 @@
             config_pr_url = config_pr.html_url
             edit_sweep_comment(message="", index=-2)
         except Exception as e:
             logger.error("Failed to create new branch for sweep.yaml file.\n", e, traceback.format_exc())
     else:
         logger.info("sweep.yaml file already exists.")
 
-
     sweepbot_retries = 3
     try:
         for i in range(sweepbot_retries):
             # ANALYZE SNIPPETS
             if sweep_bot.model == "gpt-4-32k-0613":
                 logger.info("CoT retrieval...")
                 sweep_bot.cot_retrieval()
@@ -349,15 +354,16 @@
 
             # COMMENT ON ISSUE
             # TODO: removed issue commenting here
             logger.info("Fetching files to modify/create...")
             file_change_requests = sweep_bot.get_files_to_change()
             file_change_requests = sweep_bot.validate_file_change_requests(file_change_requests)
             table = tabulate(
-                [[f"`{file_change_request.filename}`", file_change_request.instructions] for file_change_request in file_change_requests],
+                [[f"`{file_change_request.filename}`", file_change_request.instructions] for file_change_request in
+                 file_change_requests],
                 headers=["File Path", "Proposed Changes"],
                 tablefmt="pipe"
             )
             edit_sweep_comment(
                 "From looking through the relevant snippets, I decided to make the following modifications:\n\n" + table + "\n\n",
                 2
             )
@@ -386,26 +392,26 @@
             try:
                 current_issue.delete_reaction(eyes_reaction.id)
             except:
                 pass
             try:
                 # CODE REVIEW
                 changes_required, review_comment = review_pr(repo=repo, pr=pr, issue_url=issue_url, username=username,
-                        repo_description=repo_description, title=title,
-                        summary=summary, replies_text=replies_text, tree=tree)
+                                                             repo_description=repo_description, title=title,
+                                                             summary=summary, replies_text=replies_text, tree=tree)
                 logger.info(f"Addressing review comment {review_comment}")
                 if changes_required:
                     on_comment(repo_full_name=repo_full_name,
-                            repo_description=repo_description,
-                            comment=review_comment,
-                            username=username,
-                            installation_id=installation_id,
-                            pr_path=None,
-                            pr_line_position=None,
-                            pr_number=pr.number)
+                               repo_description=repo_description,
+                               comment=review_comment,
+                               username=username,
+                               installation_id=installation_id,
+                               pr_path=None,
+                               pr_line_position=None,
+                               pr_number=pr.number)
             except Exception as e:
                 logger.error(traceback.format_exc())
                 logger.error(e)
 
             # Completed code review
             edit_sweep_comment(
                 "Success! 🚀",
@@ -465,8 +471,7 @@
         except:
             pass
         item_to_react_to.create_reaction("rocket")
 
     posthog.capture(username, "success", properties={**metadata})
     logger.info("on_ticket success")
     return {"success": True}
-
```

### Comparing `sweepai-0.4.2/sweepai/utils/chat_logger.py` & `sweepai-0.4.3/sweepai/utils/chat_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import os
-import requests
 import json
 from datetime import datetime, timedelta
 from typing import Any
 
-from pymongo import MongoClient
-from pydantic import BaseModel, Field
+from fastapi import requests
 from loguru import logger
+from pydantic import BaseModel, Field
+from pymongo import MongoClient
+
+from sweepai.utils.config.server import MONGODB_URI, DISCORD_WEBHOOK_URL
+
 
 class ChatLogger(BaseModel):
     data: dict = Field(default_factory=dict)
     chat_collection: Any = None
     ticket_collection: Any = None
     expiration: datetime = None
     index: int = 0
     current_month: str = datetime.utcnow().strftime('%m/%Y')
 
     def __init__(self, data: dict = Field(default_factory=dict)):
         super().__init__(data=data)  # Call the BaseModel's __init__ method
-        key = os.environ.get('MONGODB_URI')
+        key = MONGODB_URI
         if key is None:
             logger.warning('Chat history logger has no key')
             return
         try:
             client = MongoClient(key, serverSelectionTimeoutMS=5000, socketTimeoutMS=5000)
             db = client['llm']
             self.chat_collection = db['chat_history']
@@ -73,26 +75,27 @@
     def is_paying_user(self):
         if self.ticket_collection is None:
             logger.error('Ticket Collection Does Not Exist')
             return False
         username = self.data['username']
         result = self.ticket_collection.find_one({'username': username})
         return result.get('is_paying_user', False) if result else False
-    
+
     def use_faster_model(self):
         if self.ticket_collection is None:
             logger.error('Ticket Collection Does Not Exist')
             return True
         if self.is_paying_user():
             return self.get_ticket_count() >= 60
         return self.get_ticket_count() >= 3
 
+
 def discord_log_error(content):
     try:
-        url = os.environ.get('DISCORD_WEBHOOK_URL')
-        data = { 'content': content }
-        headers = { 'Content-Type': 'application/json' }
+        url = DISCORD_WEBHOOK_URL
+        data = {'content': content}
+        headers = {'Content-Type': 'application/json'}
         response = requests.post(url, data=json.dumps(data), headers=headers)
         # Success: response.status_code == 204:
     except Exception as e:
         logger.error(f'Could not log to Discord: {e}')
-        pass
+        pass
```

### Comparing `sweepai-0.4.2/sweepai/utils/config.py` & `sweepai-0.4.3/sweepai/utils/config/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
+import os
 from functools import lru_cache
-from loguru import logger
+
 import yaml
 from github.Repository import Repository
+from loguru import logger
 from pydantic import BaseModel
 
+
 class SweepConfig(BaseModel):
     include_dirs: list[str] = []
     exclude_dirs: list[str] = [".git", "node_modules", "venv"]
     include_exts: list[str] = ['.cs', '.csharp', '.py', '.md', '.txt', '.ts', '.tsx', '.js', '.jsx', '.mjs']
     exclude_exts: list[str] = ['.min.js', '.min.js.map', '.min.css', '.min.css.map']
     max_file_limit: int = 60_000
-    
+
     def to_yaml(self) -> str:
         return yaml.safe_dump(self.dict())
-    
+
     @classmethod
     def from_yaml(cls, yaml_str: str) -> "SweepConfig":
         data = yaml.safe_load(yaml_str)
         return cls.parse_obj(data)
 
     @staticmethod
     @lru_cache(maxsize=None)
@@ -38,20 +41,31 @@
                 logger.warning(f"Error when getting branch: {e}, creating branch")
                 repo.create_git_ref(f"refs/heads/{branch_name}", repo.get_branch(default_branch).commit.sha)
                 return branch_name
         except Exception as e:
             logger.warning(f"Error when getting branch: {e}, falling back to default branch")
             return default_branch
 
-    @staticmethod
-    @lru_cache(maxsize=None)
-    def get_gha_enabled(repo: Repository) -> bool:
+
+@staticmethod
+@lru_cache(maxsize=None)
+def get_gha_enabled(repo: Repository) -> bool:
+    try:
+        contents = repo.get_contents("sweep.yaml")
+        gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8")).get("gha_enabled", False)
+        return gha_enabled
+    except Exception as e:
         try:
-            contents = repo.get_contents("sweep.yaml")
+            contents = repo.get_contents(".github/sweep.yaml")
         except Exception as e:
             try:
                 contents = repo.get_contents(".github/sweep.yaml")
             except Exception as e:
                 logger.warning(f"Error when getting gha enabled: {e}, falling back to False")
                 return False
         gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8")).get("gha_enabled", False)
-        return gha_enabled
+        return gha_enabled
+
+# optional, can leave env var blank
+GITHUB_APP_CLIENT_ID = os.environ.get('GITHUB_APP_CLIENT_ID', 'Iv1.91fd31586a926a9f')
+local_env = os.environ.get('ENV', 'prod')
+SWEEP_API_ENDPOINT = os.environ.get('SWEEP_API_ENDPOINT', f"https://sweepai--{local_env}-ui.modal.run")
```

### Comparing `sweepai-0.4.2/sweepai/utils/diff.py` & `sweepai-0.4.3/sweepai/utils/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import difflib
-import re
+
 
 def generate_diff(old_code, new_code):
     diff = difflib.unified_diff(
         old_code.splitlines(keepends=True),
         new_code.splitlines(keepends=True)
     )
     return ''.join(diff)
 
+
 def revert_whitespace_changes(original_file_str, modified_file_str):
     original_lines = original_file_str.splitlines()
     modified_lines = modified_file_str.splitlines()
 
     diff = difflib.SequenceMatcher(None, original_lines, modified_lines)
 
     final_lines = []
@@ -25,23 +26,24 @@
             # If it's just whitespace changes, ignore them.
             for line in modified_lines[opcode[3]:opcode[4]]:
                 if line.strip() != "":
                     final_lines.append(line)
 
     return '\n'.join(final_lines)
 
+
 def format_contents(file_contents, is_markdown=False):
     """
     Add arbitrary postprocessing here, this affects files and diffs
     """
     lines = file_contents.split('\n')
 
     if is_markdown:
         return '\n'.join(lines)
-    
+
     # Handle small files
     if len(lines) <= 5:
         start_idx = 0
         end_idx = len(lines)
         for idx, line in enumerate(lines):
             if start_idx == 0 and line.strip().startswith('```'):
                 start_idx = idx + 1
@@ -81,37 +83,37 @@
         return new_file
 
     # v5
     result = []
     lines = new_file.split('\n')
     for line_number, line in enumerate(lines):
         # Todo: make it support 1 number only
-        matches = re.finditer(r"<copy_lines\s(\d+-\d+)>", line)
+        matches = re.finditer(r"<copy_lines\s(\d+-\d+)/?>", line)
         copied_lines = False
         for match in matches:
             copied_lines = True
             start, end = match.group(1).split('-')
-            start, end = int(start)-1, int(end)-1
+            start, end = int(start) - 1, int(end) - 1
 
             start = max(0, start)
             end = min(len(old_file_lines) - 1, end)
 
             replacements = old_file_lines[start:end + 1]
             replacements_str = '\n'.join(replacements)
             line = line.replace(match.group(0), replacements_str)
 
         # check if line was incorrectly duplicated
         append = True
-        if not copied_lines: # if bot generated, and line before is not bot generated
+        if not copied_lines:  # if bot generated, and line before is not bot generated
             if len(result) > 0:
                 # Get last line in results
                 last_group = result[-1]
-                #last_line = last_group
+                # last_line = last_group
                 if '\n' in last_group:
-                    last_line = last_group[last_group.rindex('\n')+1:] # if its multiple lines
+                    last_line = last_group[last_group.rindex('\n') + 1:]  # if its multiple lines
                     # if last line is same is current line
                     if last_line == line:
                         append = False
 
         if append:
             result.append(line)
     result = '\n'.join(result)
@@ -148,23 +150,25 @@
         result_file = join_contents_k(result_file, new_file[:next_section_idx], k)
         new_file = new_file[next_section_idx:] # remove the first section from new_file
     
     return result_file + last_section
     """
 
     return result
-    
+
+
 def join_contents_k(first, second, k):
     """
     Join contents together removing k duplicate lines
     """
     first_lines = first.splitlines()
     second_lines = second.splitlines()
     for i in range(k, 0, -1):
         if len(first_lines) < k or len(second_lines) < k:
             continue
         if first_lines[-i:] == second_lines[:i]:
             return "\n".join(first_lines) + "\n" + "\n".join(second_lines[i:])
     return "\n".join(first_lines) + "\n" + "\n".join(second_lines)
 
+
 def is_markdown(filename):
-    return filename.endswith(".md") or filename.endswith(".rst") or filename.endswith(".txt")
+    return filename.endswith(".md") or filename.endswith(".rst") or filename.endswith(".txt")
```

### Comparing `sweepai-0.4.2/sweepai/utils/event_logger.py` & `sweepai-0.4.3/sweepai/utils/event_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-import os
-from loguru import logger
-
 import highlight_io
+from loguru import logger
 from posthog import Posthog
 
-POSTHOG_API_KEY = os.environ.get("POSTHOG_API_KEY")
+from sweepai.utils.config.server import POSTHOG_API_KEY, HIGHLIGHT_API_KEY
+
 if POSTHOG_API_KEY is None:
     posthog = Posthog(project_api_key="none", disabled=True, host='https://app.posthog.com')
     logger.warning("Initialized an empty Posthog instance as POSTHOG_API_KEY is not present.")
 else:
     posthog = Posthog(project_api_key=POSTHOG_API_KEY, host='https://app.posthog.com')
 
-HIGHLIGHT_API_KEY = os.environ.get("HIGHLIGHT_API_KEY")
 if HIGHLIGHT_API_KEY is None:
     H = None
 else:
     H = highlight_io.H(HIGHLIGHT_API_KEY)
     logger.add(
         H.logging_handler,
         format="{message}",
         level="INFO",
         backtrace=True,
     )
-
```

### Comparing `sweepai-0.4.2/sweepai/utils/file_change_functions.py` & `sweepai-0.4.3/sweepai/utils/file_change_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from loguru import logger
+
 from sweepai.core.chat import Function
 from sweepai.utils.diff import format_contents
 
 modify_file_function = Function(
     name="modify_file",
     description="Edits the code in a file. Use start_line and end_line to completely cover the line indexes of code that should be replaced. Indent and format the code in the edits. Output the code in the order it should appear in the file. Make sure start_line and end_line do not overlap between code edits.",
     parameters={
@@ -36,17 +37,18 @@
                     },
                     "required": ["start_line", "end_line", "code", "num_indents"]
                 },
                 "description": "An array of edits. Each `code_edit` represents a slice of the code split by newlines and delimited by `start_line` and `end_line`. Both `start_line` and `end_line` are zero-indexed and inclusive."
             }
         },
         "required": ["file_name", "code_edits"]
-        }
+    }
 )
 
+
 def apply_code_edits(file_contents, code_edits):
     modifications = []
     for edit in code_edits:
         start_line = int(edit['start_line'])
         end_line = int(edit['end_line'])
         new_code = format_contents(edit['inserted_code'])
         # Indentation
@@ -72,28 +74,28 @@
             continue
         if end_line > len(lines) - 1:
             logger.error(f"End line {end_line} is greater than the number of lines in the file {len(lines)}")
             continue
         # Handle duplicate lines between the existing code and new code
         indents = '  ' * indentation
         if start_line > 0 and end_line < len(lines) \
-            and new_code[0] == lines[start_line-1] and new_code[-1] == lines[end_line]:
+                and new_code[0] == lines[start_line - 1] and new_code[-1] == lines[end_line]:
             new_code = new_code[1:-1]
             new_code = [indents + line for line in new_code]
             lines[start_line:end_line] = new_code
             continue
-        elif start_line > 0 and new_code[0] == lines[start_line-1]:
+        elif start_line > 0 and new_code[0] == lines[start_line - 1]:
             new_code = new_code[1:]
             new_code = [indents + line for line in new_code]
-            lines[start_line-1:end_line + 1] = new_code # Exit and merge first line
+            lines[start_line - 1:end_line + 1] = new_code  # Exit and merge first line
             continue
         elif end_line < len(lines) and new_code[-1] == lines[end_line]:
             new_code = new_code[:-1]
             new_code = [indents + line for line in new_code]
-            lines[start_line:end_line] = new_code # Exit and merge last line
+            lines[start_line:end_line] = new_code  # Exit and merge last line
             continue
         # Check index error
         if end_line > len(lines) - 1:
             end_line = len(lines) - 1
         new_code = [indents + line for line in new_code]
-        lines[start_line:end_line + 1] = new_code # Start and end are inclusive
+        lines[start_line:end_line + 1] = new_code  # Start and end are inclusive
     return '\n'.join(lines)
```

### Comparing `sweepai-0.4.2/sweepai/utils/github_utils.py` & `sweepai-0.4.3/sweepai/utils/github_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-import shutil
-import modal
 import os
-import time
 import re
+import shutil
+import time
+
 import github
+import modal
+import requests
 from github import Github
 from github.Repository import Repository
-from loguru import logger
-
 from jwt import encode
-import requests
+from loguru import logger
 from tqdm import tqdm
+
 from sweepai.core.entities import Snippet
-from sweepai.utils.config import SweepConfig
-from sweepai.utils.constants import APP_ID, DB_NAME
+from sweepai.utils.config.client import SweepConfig
+from sweepai.utils.config.server import DB_MODAL_INST_NAME, GITHUB_APP_ID, GITHUB_APP_PEM
 from sweepai.utils.event_logger import posthog
 
+
 def make_valid_string(string: str):
     pattern = r"[^\w./-]+"
     return re.sub(pattern, "_", string)
 
 
 def get_jwt():
-    signing_key = os.environ["GITHUB_APP_PEM"]
-    app_id = APP_ID
+    signing_key = GITHUB_APP_PEM
+    app_id = GITHUB_APP_ID
     payload = {"iat": int(time.time()), "exp": int(time.time()) + 600, "iss": app_id}
 
     return encode(payload, signing_key, algorithm="RS256")
 
 
 def get_token(installation_id: int):
     jwt = get_jwt()
@@ -60,42 +62,44 @@
     )
     obj = response.json()
     try:
         return obj["id"]
     except:
         raise Exception("Could not get installation id, probably not installed")
 
+
 def display_directory_tree(
-    root_path,
-    includes: list[str] = [],
-    excludes: list[str] = [".git"],
+        root_path,
+        includes: list[str] = [],
+        excludes: list[str] = [".git"],
 ):
     def display_directory_tree_helper(
-        current_dir,
-        indent="",
+            current_dir,
+            indent="",
     ) -> str:
         files = os.listdir(current_dir)
         files.sort()
         tree = ""
         for item_name in files:
-            full_path = os.path.join(current_dir, item_name)[len(root_path) + 1 :]
+            full_path = os.path.join(current_dir, item_name)[len(root_path) + 1:]
             if item_name in excludes:
                 continue
             file_path = os.path.join(current_dir, item_name)
             if os.path.isdir(file_path):
                 if full_path in includes:
                     tree += f"{indent}|- {item_name}/\n"
                     tree += display_directory_tree_helper(
                         file_path, indent + "|   "
                     )
                 else:
                     tree += f"{indent}|- {item_name}/...\n"
             else:
                 tree += f"{indent}|- {item_name}\n"
         return tree
+
     tree = display_directory_tree_helper(root_path)
     lines = tree.splitlines()
     return "\n".join([line[3:] for line in lines])
 
 
 def get_file_list(root_directory: str) -> str:
     files = []
@@ -108,29 +112,29 @@
             item_path = os.path.join(directory, item)
             if os.path.isfile(item_path):
                 files.append(item_path)  # Add the file to the list
             elif os.path.isdir(item_path):
                 dfs_helper(item_path)  # Recursive call to explore subdirectory
 
     dfs_helper(root_directory)
-    files = [file[len(root_directory) + 1 :] for file in files]
+    files = [file[len(root_directory) + 1:] for file in files]
     return files
 
 
 # def get_tree(repo_name: str, installation_id: int) -> str:
 #     token = get_token(installation_id)
 #     repo_url = f"https://x-access-token:{token}@github.com/{repo_name}.git"
 #     Repo.clone_from(repo_url, "repo")
 #     tree = display_directory_tree("repo")
 #     shutil.rmtree("repo")
 #     return tree
 def get_tree_and_file_list(
-    repo: Repository, 
-    installation_id: int, 
-    snippet_paths: list[str]
+        repo: Repository,
+        installation_id: int,
+        snippet_paths: list[str]
 ) -> str:
     from git import Repo
     token = get_token(installation_id)
     shutil.rmtree("repo", ignore_errors=True)
     repo_url = f"https://x-access-token:{token}@github.com/{repo.full_name}.git"
     git_repo = Repo.clone_from(repo_url, "repo")
     git_repo.git.checkout(SweepConfig.get_branch(repo))
@@ -141,15 +145,15 @@
         for directory in snippet_path.split("/")[:-1]:
             file_list += directory + "/"
             prefixes.append(file_list.rstrip("/"))
         file_list += snippet_path.split("/")[-1]
         prefixes.append(snippet_path)
 
     tree = display_directory_tree(
-        "repo", 
+        "repo",
         includes=prefixes,
     )
     file_list = get_file_list("repo")
     shutil.rmtree("repo")
     return tree, file_list
 
 
@@ -158,24 +162,24 @@
         ref = repo.default_branch
     file = repo.get_contents(file_path, ref=ref)
     contents = file.decoded_content.decode("utf-8")
     return contents
 
 
 def search_snippets(
-    repo: Repository,
-    query: str,
-    installation_id: int,
-    num_files: int = 5,
-    include_tree: bool = True,
-    branch: str = None,
-    sweep_config: SweepConfig = SweepConfig(),
+        repo: Repository,
+        query: str,
+        installation_id: int,
+        num_files: int = 5,
+        include_tree: bool = True,
+        branch: str = None,
+        sweep_config: SweepConfig = SweepConfig(),
 ) -> tuple[list[Snippet], str]:
     # Initialize the relevant directories string
-    get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
+    get_relevant_snippets = modal.Function.lookup(DB_MODAL_INST_NAME, "get_relevant_snippets")
     snippets: list[Snippet] = get_relevant_snippets.call(
         repo.full_name, query, num_files, installation_id=installation_id
     )
     logger.info(f"Snippets: {snippets}")
     # TODO: We should prioritize the mentioned files
     for snippet in snippets:
         try:
@@ -185,50 +189,50 @@
                 continue
         except github.UnknownObjectException as e:
             logger.warning(f"Error: {e}")
             logger.warning(f"Skipping {snippet.file_path}")
         else:
             snippet.content = file_contents
     tree, file_list = get_tree_and_file_list(
-        repo, 
-        installation_id, 
+        repo,
+        installation_id,
         snippet_paths=[snippet.file_path for snippet in snippets]
     )
     for file_path in tqdm(file_list):
         if file_path in query:
             try:
                 file_contents = get_file_contents(repo, file_path, ref=branch)
                 if len(file_contents) > sweep_config.max_file_limit:  # more than 10000 tokens
                     logger.warning(f"Skipping {file_path}, too many tokens")
                     continue
             except github.UnknownObjectException as e:
                 logger.warning(f"Error: {e}")
                 logger.warning(f"Skipping {file_path}")
             else:
                 snippets = [
-                    Snippet(
-                        content=file_contents,
-                        start=0,
-                        end=file_contents.count("\n") + 1,
-                        file_path=file_path,
-                    )
-                ] + snippets
+                               Snippet(
+                                   content=file_contents,
+                                   start=0,
+                                   end=file_contents.count("\n") + 1,
+                                   file_path=file_path,
+                               )
+                           ] + snippets
     snippets = [snippet.expand() for snippet in snippets]
     if include_tree:
         return snippets, tree
     else:
         return snippets
 
 
 def index_full_repository(
-    repo_name: str,
-    installation_id: int = None,
-    sweep_config: SweepConfig = SweepConfig(),
+        repo_name: str,
+        installation_id: int = None,
+        sweep_config: SweepConfig = SweepConfig(),
 ):
-    update_index = modal.Function.lookup(DB_NAME, "update_index")
+    update_index = modal.Function.lookup(DB_MODAL_INST_NAME, "update_index")
     num_indexed_docs = update_index.spawn(
         repo_name=repo_name,
         installation_id=installation_id,
         sweep_config=sweep_config,
     )
     try:
         repo = get_github_client(installation_id).get_repo(repo_name)
```

### Comparing `sweepai-0.4.2/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.3/sweepai/utils/prompt_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from loguru import logger
 from pydantic import BaseModel
+
 from sweepai.core.prompts import (
     human_message_prompt,
     human_message_prompt_comment,
     human_message_review_prompt,
     diff_section_prompt,
     review_follow_up_prompt,
     final_review_prompt,
     comment_line_prompt
 )
 
-from loguru import logger
 
 class HumanMessagePrompt(BaseModel):
     repo_name: str
     issue_url: str
     username: str
     title: str
     summary: str
@@ -33,29 +34,30 @@
         for snippet in self.snippets:
             if snippet.file_path not in deduped_paths:
                 deduped_paths.append(snippet.file_path)
         return "\n".join(deduped_paths)
 
     def render_snippets(self):
         return "\n".join([snippet.xml for snippet in self.snippets])
-    
+
     def construct_prompt(self):
         human_messages = [{'role': msg['role'], 'content': msg['content'].format(
             repo_name=self.repo_name,
             issue_url=self.issue_url,
             username=self.username,
             repo_description=self.repo_description,
             tree=self.tree,
             title=self.title,
             description=self.summary if self.summary else "No description provided.",
             relevant_snippets=self.render_snippets(),
             relevant_directories=self.get_relevant_directories(),
-        )} for msg in human_message_prompt]
+        ), 'key': msg.get('key')} for msg in human_message_prompt]
         return human_messages
-    
+
+
 class HumanMessagePromptReview(HumanMessagePrompt):
     pr_title: str
     pr_message: str = ""
     diffs: list
 
     def format_diffs(self):
         formatted_diffs = []
@@ -83,26 +85,29 @@
             diffs=self.format_diffs(),
             pr_title=self.pr_title,
             pr_message=self.pr_message,
         )} for msg in human_message_review_prompt]
 
         return human_messages
 
+
 class HumanMessageReviewFollowup(BaseModel):
     diff: tuple
+
     def construct_prompt(self):
         file_name, new_file_contents, old_file_contents, file_patch = self.diff
         format_diff = diff_section_prompt.format(
             diff_file_path=file_name,
             new_file_content=new_file_contents.rstrip("\n"),
             previous_file_content=old_file_contents.rstrip("\n"),
             diffs=file_patch
         )
         return review_follow_up_prompt + format_diff
 
+
 class HumanMessageCommentPrompt(HumanMessagePrompt):
     comment: str
     diffs: list
     pr_file_path: str | None
     pr_line: str | None
 
     def format_diffs(self):
@@ -139,14 +144,15 @@
                 pr_line=self.pr_line
             )})
         else:
             logger.info(f"General Comment {self.comment}")
 
         return human_messages
 
+
 class HumanMessageFinalPRComment(BaseModel):
     summarization_replies: list
 
     def construct_prompt(self):
         final_review = final_review_prompt.format(
             file_summaries="\n".join(self.summarization_replies)
         )
```

### Comparing `sweepai-0.4.2/sweepai/utils/scorer.py` & `sweepai-0.4.3/sweepai/utils/scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-
 from datetime import datetime
 
+
 def compute_score(contents, commits):
-    line_count = contents.count("\n") 
+    line_count = contents.count("\n")
     if line_count > 200:
         line_count_score = 10
     else:
         line_count_score = line_count / 20
     commit_count = len(commits) + 1
     days_since_last_modified = max(((datetime.now() - commits[0].commit.author.date).total_seconds() // 3600), 0) + 1
     return (line_count_score * commit_count / days_since_last_modified)
 
+
 def convert_to_percentiles(values):
     sorted_values = sorted(values)  # Sort the values in ascending order
     n = len(sorted_values)
     max_percentile = .25
     percentile_mapping = {value: (i / (n)) * max_percentile for i, value in enumerate(sorted_values)}
     percentiles = [percentile_mapping[value] for value in values]  # Create the percentiles list based on the mapping
 
-    return percentiles
+    return percentiles
```

### Comparing `sweepai-0.4.2/sweepai/utils/snippets.py` & `sweepai-0.4.3/sweepai/utils/snippets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-
-from loguru import logger
 import modal
+from loguru import logger
+
+from sweepai.core.entities import Snippet
+from sweepai.utils.config.server import UTILS_MODAL_INST_NAME
 
-from sweepai.core.chat import Snippet
-from sweepai.utils.constants import UTILS_NAME
+chunker = modal.Function.lookup(UTILS_MODAL_INST_NAME, "Chunking.chunk")
 
-chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
 
 def format_snippets(snippets: list[Snippet]):
     snippets: list[Snippet] = snippets[::-1]
 
     num_full_files = 3
     num_extended_snippets = 5
 
     most_relevant_snippets = snippets[-num_full_files:]
     snippets = snippets[:-num_full_files]
     logger.info("Expanding snippets...")
     for snippet in most_relevant_snippets:
         current_snippet = snippet
         _chunks, metadatas, _ids = chunker.call(
-            current_snippet.content, 
+            current_snippet.content,
             current_snippet.file_path
         )
         segmented_snippets = [
             Snippet(
                 content=current_snippet.content,
                 start=metadata["start"],
                 end=metadata["end"],
@@ -35,8 +35,8 @@
             index += 1
         index -= 1
         for i in range(index + 1, min(index + num_extended_snippets + 1, len(segmented_snippets))):
             current_snippet += segmented_snippets[i]
         for i in range(index - 1, max(index - num_extended_snippets - 1, 0), -1):
             current_snippet = segmented_snippets[i] + current_snippet
         snippets.append(current_snippet)
-    return snippets
+    return snippets
```

### Comparing `sweepai-0.4.2/sweepai/utils/utils.py` & `sweepai-0.4.3/sweepai/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
+import re
 import subprocess
 from dataclasses import dataclass
-import re
 
 import modal
-from modal import method
 from loguru import logger
+from modal import method
 
-from sweepai.utils.constants import UTILS_NAME
+from sweepai.utils.config.server import UTILS_MODAL_INST_NAME
 
-stub = modal.Stub(UTILS_NAME)
-tiktoken_image = modal.Image.debian_slim().pip_install("tiktoken", "loguru", "anthropic")
+stub = modal.Stub(UTILS_MODAL_INST_NAME)
+tiktoken_image = modal.Image.debian_slim().pip_install("tiktoken", "loguru", "anthropic", "pyyaml", "PyGithub")
 
 TIKTOKEN_CACHE_DIR = "/root/cache/tiktoken"
 tiktoken_volume = modal.SharedVolume().persist("tiktoken-models")
 
+
 @stub.cls(
-    image=tiktoken_image, 
-    shared_volumes={TIKTOKEN_CACHE_DIR: tiktoken_volume}, 
+    image=tiktoken_image,
+    shared_volumes={TIKTOKEN_CACHE_DIR: tiktoken_volume},
     secret=modal.Secret.from_dict({"TIKTOKEN_CACHE_DIR": TIKTOKEN_CACHE_DIR})
 )
 class Tiktoken:
     openai_models = ["gpt-3.5-turbo", "gpt-4", "gpt-4-32k", "gpt-4-32k-0613"]
     anthropic_models = ["claude-v1", "claude-v1.3-100k", "claude-instant-v1.3-100k"]
     models = openai_models + anthropic_models
 
@@ -29,21 +30,23 @@
         import tiktoken
         self.openai_models = {model: tiktoken.encoding_for_model(model) for model in Tiktoken.openai_models}
 
     @method()
     def count(self, text: str, model: str = "gpt-4"):
         return len(self.openai_models[model].encode(text))
 
+
 chunking_image = modal.Image.debian_slim() \
     .apt_install("git") \
-    .pip_install("tree-sitter", "loguru")
+    .pip_install("tree-sitter", "loguru", "pyyaml", "PyGithub")
 
 CHUNKING_CACHE_DIR = "/root/cache/"
 chunking_volume = modal.SharedVolume().persist("chunking-parsers")
 
+
 @dataclass
 class Span:
     start: int
     end: int
 
     def extract(self, s: str) -> str:
         return "\n".join(s.splitlines()[self.start:self.end])
@@ -51,31 +54,33 @@
     def __add__(self, other):
         if isinstance(other, int):
             return Span(self.start + other, self.end + other)
         elif isinstance(other, Span):
             return Span(self.start, other.end)
         else:
             raise NotImplementedError()
-    
+
     def __len__(self):
         return self.end - self.start
 
+
 def get_line_number(index: int, source_code: str) -> int:
     # unoptimized, use binary search
     lines = source_code.splitlines(keepends=True)
     total_chars = 0
     line_number = 0
     while total_chars <= index:
         if line_number == len(lines):
             return line_number
         total_chars += len(lines[line_number])
         line_number += 1
     return line_number - 1
 
-def chunker(tree, source_code_bytes, max_chunk_size = 512 * 3, coalesce = 50):
+
+def chunker(tree, source_code_bytes, max_chunk_size=512 * 3, coalesce=50):
     # Recursively form chunks with a maximum chunk size of max_chunk_size
     def chunker_helper(node, source_code_bytes, start_position=0):
         chunks = []
         current_chunk = Span(start_position, start_position)
         for child in node.children:
             child_span = Span(child.start_byte, child.end_byte)
             if len(child_span) > max_chunk_size:
@@ -86,44 +91,48 @@
                 chunks.append(current_chunk)
                 current_chunk = child_span
             else:
                 current_chunk += child_span
         if len(current_chunk) > 0:
             chunks.append(current_chunk)
         return chunks
+
     chunks = chunker_helper(tree.root_node, source_code_bytes)
 
     # removing gaps
     for prev, curr in zip(chunks[:-1], chunks[1:]):
         prev.end = curr.start
-    
+
     # combining small chunks with bigger ones
     new_chunks = []
     i = 0
     current_chunk = Span(0, 0)
     while i < len(chunks):
         current_chunk += chunks[i]
-        if count_length_without_whitespace(source_code_bytes[current_chunk.start:current_chunk.end].decode("utf-8")) > coalesce \
-            and "\n" in source_code_bytes[current_chunk.start:current_chunk.end].decode("utf-8"):
+        if count_length_without_whitespace(
+                source_code_bytes[current_chunk.start:current_chunk.end].decode("utf-8")) > coalesce \
+                and "\n" in source_code_bytes[current_chunk.start:current_chunk.end].decode("utf-8"):
             new_chunks.append(current_chunk)
             current_chunk = Span(chunks[i].end, chunks[i].end)
         i += 1
     if len(current_chunk) > 0:
         new_chunks.append(current_chunk)
-    
-    line_chunks = [Span(get_line_number(chunk.start, source_code=source_code_bytes), get_line_number(chunk.end, source_code=source_code_bytes)) for chunk in new_chunks]
+
+    line_chunks = [Span(get_line_number(chunk.start, source_code=source_code_bytes),
+                        get_line_number(chunk.end, source_code=source_code_bytes)) for chunk in new_chunks]
     line_chunks = [chunk for chunk in line_chunks if len(chunk) > 0]
-    
+
     return line_chunks
 
 
 def count_length_without_whitespace(s: str):
     string_without_whitespace = re.sub(r'\s', '', s)
     return len(string_without_whitespace)
 
+
 extension_to_language = {
     "js": "tsx",
     "jsx": "tsx",
     "ts": "tsx",
     "tsx": "tsx",
     "mjs": "tsx",
     "py": "python",
@@ -144,67 +153,78 @@
     "erb": "embedded-template",
     "ejs": "embedded-template",
     "html": "embedded-template",
     "vue": "vue",
     "php": "php",
 }
 
+
 @stub.cls(
-    image=chunking_image, 
+    image=chunking_image,
     shared_volumes={CHUNKING_CACHE_DIR: chunking_volume},
 )
 class Chunking:
 
     def __enter__(self):
         from tree_sitter import Language
 
+        logger.debug("Downloading tree-sitter parsers")
+
         LANGUAGE_NAMES = ["python", "java", "cpp", "go", "rust", "ruby", "php"]
         for language in LANGUAGE_NAMES:
-            subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-{language} cache/tree-sitter-{language}", shell=True)
+            subprocess.run(
+                f"git clone https://github.com/tree-sitter/tree-sitter-{language} cache/tree-sitter-{language}",
+                shell=True)
         for language in LANGUAGE_NAMES:
-            Language.build_library(f'cache/build/{language}.so', [f"cache/tree-sitter-{language}"]) 
-            subprocess.run(f"cp cache/build/{language}.so /tmp/{language}.so", shell=True) # copying for executability
+            Language.build_library(f'cache/build/{language}.so', [f"cache/tree-sitter-{language}"])
+            subprocess.run(f"cp cache/build/{language}.so /tmp/{language}.so", shell=True)  # copying for executability
         self.languages = {language: Language(f"/tmp/{language}.so", language) for language in LANGUAGE_NAMES}
 
-        subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-typescript cache/tree-sitter-typescript", shell=True)
-        Language.build_library(f'cache/build/typescript.so', [f"cache/tree-sitter-typescript/tsx"]) 
+        subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-typescript cache/tree-sitter-typescript",
+                       shell=True)
+        Language.build_library(f'cache/build/typescript.so', [f"cache/tree-sitter-typescript/tsx"])
         subprocess.run(f"cp cache/build/typescript.so /tmp/typescript.so", shell=True)
         self.languages["tsx"] = Language("/tmp/typescript.so", "tsx")
 
-        subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-c-sharp cache/tree-sitter-c-sharp", shell=True)
-        Language.build_library(f'cache/build/c-sharp.so', [f"cache/tree-sitter-c-sharp"]) 
+        subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-c-sharp cache/tree-sitter-c-sharp",
+                       shell=True)
+        Language.build_library(f'cache/build/c-sharp.so', [f"cache/tree-sitter-c-sharp"])
         subprocess.run(f"cp cache/build/c-sharp.so /tmp/c-sharp.so", shell=True)
         self.languages["c-sharp"] = Language("/tmp/c-sharp.so", "c_sharp")
 
-        subprocess.run(f"git clone https://github.com/tree-sitter/tree-sitter-embedded-template cache/tree-sitter-embedded-template", shell=True)
-        Language.build_library(f'cache/build/embedded-template.so', [f"cache/tree-sitter-embedded-template"]) 
+        subprocess.run(
+            f"git clone https://github.com/tree-sitter/tree-sitter-embedded-template cache/tree-sitter-embedded-template",
+            shell=True)
+        Language.build_library(f'cache/build/embedded-template.so', [f"cache/tree-sitter-embedded-template"])
         subprocess.run(f"cp cache/build/embedded-template.so /tmp/embedded-template.so", shell=True)
         self.languages["embedded-template"] = Language("/tmp/embedded-template.so", "embedded_template")
-        
-        subprocess.run(f"git clone https://github.com/MDeiml/tree-sitter-markdown cache/tree-sitter-markdown", shell=True)
-        Language.build_library(f'cache/build/markdown.so', [f"cache/tree-sitter-markdown/tree-sitter-markdown"]) 
+
+        subprocess.run(f"git clone https://github.com/MDeiml/tree-sitter-markdown cache/tree-sitter-markdown",
+                       shell=True)
+        Language.build_library(f'cache/build/markdown.so', [f"cache/tree-sitter-markdown/tree-sitter-markdown"])
         subprocess.run(f"cp cache/build/markdown.so /tmp/markdown.so", shell=True)
         self.languages["markdown"] = Language("/tmp/markdown.so", "markdown")
 
         subprocess.run(f"git clone https://github.com/ikatyang/tree-sitter-vue cache/tree-sitter-vue", shell=True)
-        Language.build_library(f'cache/build/vue.so', [f"cache/tree-sitter-vue"]) 
+        Language.build_library(f'cache/build/vue.so', [f"cache/tree-sitter-vue"])
         subprocess.run(f"cp cache/build/vue.so /tmp/vue.so", shell=True)
         self.languages["vue"] = Language("/tmp/vue.so", "vue")
-        
+
+        logger.debug("Finished downloading tree-sitter parsers")
 
     @method()
     def chunk(
-        self,
-        file_content: str, 
-        file_path: str,
-        score: float = 1.0, 
-        additional_metadata: dict[str, str] = {},
-        max_chunk_size: int = 512 * 3,
-        chunk_size: int = 30, 
-        overlap: int = 15
+            self,
+            file_content: str,
+            file_path: str,
+            score: float = 1.0,
+            additional_metadata: dict[str, str] = {},
+            max_chunk_size: int = 512 * 3,
+            chunk_size: int = 30,
+            overlap: int = 15
     ) -> tuple[list[str], list[dict[str, str]]]:
         """This function returns a list of chunks and a list of metadata for each chunk.
         chunks: list of file chunks
         metadata: list of metadata for each chunk example: {"file_path": "python", "start": 0, "end": 10}
         ids: list of ids for each chunk {file_path}:{start}{end}
         """
         # TODO(Sweep): implement a config file for the above
```

### Comparing `sweepai-0.4.2/setup.py` & `sweepai-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['sweepai', 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
+['sweepai',
+ 'sweepai.app',
+ 'sweepai.core',
+ 'sweepai.handlers',
+ 'sweepai.utils',
+ 'sweepai.utils.config']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['GitPython>=3.1.31,<4.0.0',
  'PyGithub==1.58.2',
  'config-path>=1.0.3,<2.0.0',
  'gradio>=3.35.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
+ 'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'typer>=0.9.0,<0.10.0',
- 'urllib3>=2.0.3,<3.0.0']
+ 'urllib3<2.0.0']
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'Sweep software chores',
     'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep\'s limitations(for now):\n- Try to change less than 200 lines of code\n- Try to modify less than 3 files\n- Do not include files with more than 1500 lines of code\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
-'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
-package_data = \ {'': ['*']} install_requires = \ ['GitPython>=3.1.31,<4.0.0',
-'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0',
-'loguru>=0.6.0,<0.7.0', 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0',
-'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0'] entry_points = \
-{'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai = sweepai.app.cli:
-app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.4.2', 'description':
-'Sweep software chores', 'long_description': '
+'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils',
+'sweepai.utils.config'] package_data = \ {'': ['*']} install_requires = \
+['GitPython>=3.1.31,<4.0.0', 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0',
+'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'pyyaml>=6.0,<7.0',
+'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
+'urllib3<2.0.0'] entry_points = \ {'console_scripts': ['sweep =
+sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
+{ 'name': 'sweepai', 'version': '0.4.3', 'description': 'Sweep software
+chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
   sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
```

### Comparing `sweepai-0.4.2/PKG-INFO` & `sweepai-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.2
+Version: 0.4.3
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: config-path (>=1.0.3,<2.0.0)
 Requires-Dist: gradio (>=3.35.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
+Requires-Dist: urllib3 (<2.0.0)
 Project-URL: Bug Tracker, https://github.com/sweepai/sweep/issues
 Project-URL: Community, https://discord.gg/sweep-ai
 Project-URL: documentation, https://docs.sweep.dev
 Project-URL: homepage, https://sweep.dev
 Project-URL: repository, https://github.com/sweepai/sweep
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.2 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.3 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
-tabulate (>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
-Dist: urllib3 (>=2.0.3,<3.0.0) Project-URL: Bug Tracker, https://github.com/
-sweepai/sweep/issues Project-URL: Community, https://discord.gg/sweep-ai
-Project-URL: documentation, https://docs.sweep.dev Project-URL: homepage,
-https://sweep.dev Project-URL: repository, https://github.com/sweepai/sweep
-Description-Content-Type: text/markdown
+(>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
+(>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
+typer (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (<2.0.0) Project-URL: Bug
+Tracker, https://github.com/sweepai/sweep/issues Project-URL: Community, https:
+//discord.gg/sweep-ai Project-URL: documentation, https://docs.sweep.dev
+Project-URL: homepage, https://sweep.dev Project-URL: repository, https://
+github.com/sweepai/sweep Description-Content-Type: text/markdown
   [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                  3e61f57ad233]
                Bug Reports & Feature Requests â¶  Code Changes
       [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
 ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
```

