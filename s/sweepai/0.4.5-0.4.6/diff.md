# Comparing `tmp/sweepai-0.4.5.tar.gz` & `tmp/sweepai-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.5.tar", max compression
+gzip compressed data, was "sweepai-0.4.6.tar", max compression
```

## Comparing `sweepai-0.4.5.tar` & `sweepai-0.4.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    20850 2023-06-14 19:09:46.074723 sweepai-0.4.5/LICENSE
--rw-r--r--   0        0        0     6847 2023-07-13 18:59:01.830686 sweepai-0.4.5/README.md
--rw-r--r--   0        0        0     1411 2023-07-13 23:44:40.215808 sweepai-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.418346 sweepai-0.4.5/sweepai/__init__.py
--rw-r--r--   0        0        0    12345 2023-07-13 18:59:01.833466 sweepai-0.4.5/sweepai/api.py
--rw-r--r--   0        0        0     6656 2023-07-13 23:44:30.002584 sweepai-0.4.5/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10697 2023-07-13 23:27:42.917993 sweepai-0.4.5/sweepai/app/backend.py
--rw-r--r--   0        0        0     1167 2023-07-13 18:59:01.834993 sweepai-0.4.5/sweepai/app/cli.py
--rw-r--r--   0        0        0     3615 2023-07-13 23:13:30.928829 sweepai-0.4.5/sweepai/app/config.py
--rw-r--r--   0        0        0    15383 2023-07-13 22:49:37.300901 sweepai-0.4.5/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.419148 sweepai-0.4.5/sweepai/core/__init__.py
--rw-r--r--   0        0        0    18015 2023-07-13 23:25:51.402683 sweepai-0.4.5/sweepai/core/chat.py
--rw-r--r--   0        0        0     2880 2023-07-13 18:59:01.836485 sweepai-0.4.5/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8273 2023-07-13 18:59:01.836657 sweepai-0.4.5/sweepai/core/entities.py
--rw-r--r--   0        0        0      535 2023-07-13 18:59:01.837093 sweepai-0.4.5/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16873 2023-07-13 21:52:24.490410 sweepai-0.4.5/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3489 2023-07-13 18:59:01.837629 sweepai-0.4.5/sweepai/core/react.py
--rw-r--r--   0        0        0    20835 2023-07-13 19:24:27.610154 sweepai-0.4.5/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    13594 2023-07-13 18:59:01.837980 sweepai-0.4.5/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3191 2023-07-13 18:59:01.838139 sweepai-0.4.5/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.420325 sweepai-0.4.5/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     7146 2023-07-13 23:28:07.436121 sweepai-0.4.5/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2613 2023-07-13 21:42:18.752139 sweepai-0.4.5/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9748 2023-07-13 19:26:08.750222 sweepai-0.4.5/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4042 2023-07-13 18:59:01.840830 sweepai-0.4.5/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    19986 2023-07-13 22:06:11.061049 sweepai-0.4.5/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841069 sweepai-0.4.5/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 21:27:38.421045 sweepai-0.4.5/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3822 2023-07-13 23:26:07.719104 sweepai-0.4.5/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0        0 2023-07-13 18:59:01.841626 sweepai-0.4.5/sweepai/utils/config/__init__.py
--rw-r--r--   0        0        0     2761 2023-07-13 23:21:47.583779 sweepai-0.4.5/sweepai/utils/config/client.py
--rw-r--r--   0        0        0     3460 2023-07-13 23:38:41.531570 sweepai-0.4.5/sweepai/utils/config/server.py
--rw-r--r--   0        0        0     6524 2023-07-13 18:59:01.842462 sweepai-0.4.5/sweepai/utils/diff.py
--rw-r--r--   0        0        0      675 2023-07-13 18:59:01.842660 sweepai-0.4.5/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5256 2023-07-13 18:59:01.842775 sweepai-0.4.5/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8431 2023-07-13 18:59:01.843177 sweepai-0.4.5/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0      100 2023-07-13 18:59:01.843270 sweepai-0.4.5/sweepai/utils/hash.py
--rw-r--r--   0        0        0     5585 2023-07-13 18:59:01.843383 sweepai-0.4.5/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      849 2023-07-13 18:59:01.843512 sweepai-0.4.5/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1528 2023-07-13 18:59:01.843616 sweepai-0.4.5/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11648 2023-07-13 18:59:01.843761 sweepai-0.4.5/sweepai/utils/utils.py
--rw-r--r--   0        0        0     7826 1970-01-01 00:00:00.000000 sweepai-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.6/LICENSE
+-rw-r--r--   0        0        0     7019 2023-07-13 23:38:51.881474 sweepai-0.4.6/README.md
+-rw-r--r--   0        0        0     1411 2023-07-13 23:57:55.285751 sweepai-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.6/sweepai/__init__.py
+-rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/api.py
+-rw-r--r--   0        0        0     6656 2023-07-13 23:57:23.352400 sweepai-0.4.6/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10697 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/app/config.py
+-rw-r--r--   0        0        0    15383 2023-07-13 23:57:23.352400 sweepai-0.4.6/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.6/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    18015 2023-07-13 23:57:23.352400 sweepai-0.4.6/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.6/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/core/react.py
+-rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.6/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.6/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     7146 2023-07-13 23:57:23.352400 sweepai-0.4.6/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.6/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.6/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19991 2023-07-13 23:38:31.094765 sweepai-0.4.6/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.6/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.6/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2761 2023-07-13 23:57:23.355733 sweepai-0.4.6/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3460 2023-07-13 07:19:30.090833 sweepai-0.4.6/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.6/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8431 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.6/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     8239 2023-07-13 23:58:22.938111 sweepai-0.4.6/setup.py
+-rw-r--r--   0        0        0     7998 2023-07-13 23:58:22.938579 sweepai-0.4.6/PKG-INFO
```

### Comparing `sweepai-0.4.5/LICENSE` & `sweepai-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/README.md` & `sweepai-0.4.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
 2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
+## 💰 Pricing
+* We charge $120/month for 60 GPT4 tickets per month.
+* For unpaid users, we offer 3 free GPT4 tickets per month.
+* We also offer unlimited GPT3.5 tickets.
 ## 🤝 Contributing
 
 Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
 
 ## 📘 Story
```

#### html2text {}

```diff
@@ -55,28 +55,30 @@
 this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
 gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
 right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
 ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 #### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð¤
-Contributing Contributions are welcome and greatly appreciated! For detailed
-guidelines on how to contribute, please see the [CONTRIBUTING.md]
-(CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/). ## ð Story We were frustrated by small tickets, like
-simple bug fixes, annoying refactors, and small features. Each task required us
-to open our IDE to fix simple bugs. So we decided to leverage the capabilities
-of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
-this can solve entire tickets and can be parallelized + asynchronous:
-developers can spin up 10 tickets and Sweep will address them all at once. ##
-ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
-with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
-Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap](https://
-docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart](https://
-api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð°
+Pricing * We charge $120/month for 60 GPT4 tickets per month. * For unpaid
+users, we offer 3 free GPT4 tickets per month. * We also offer unlimited GPT3.5
+tickets. ## ð¤ Contributing Contributions are welcome and greatly
+appreciated! For detailed guidelines on how to contribute, please see the
+[CONTRIBUTING.md](CONTRIBUTING.md) file. For more detailed docs, see [ð
+Quickstart](https://docs.sweep.dev/). ## ð Story We were frustrated by small
+tickets, like simple bug fixes, annoying refactors, and small features. Each
+task required us to open our IDE to fix simple bugs. So we decided to leverage
+the capabilities of ChatGPT to address this directly in GitHub. Unlike existing
+AI solutions, this can solve entire tickets and can be parallelized +
+asynchronous: developers can spin up 10 tickets and Sweep will address them all
+at once. ## ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for
+Vector DB with MiniLM L12 as our embeddings model - Modal Labs for infra +
+deployment - Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap]
+(https://docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart]
+(https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
 history.com/#sweepai/sweep&Date) Consider starring us if you're using Sweep so
 more people hear about us!
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
                             and, of course, Sweep!
```

### Comparing `sweepai-0.4.5/pyproject.toml` & `sweepai-0.4.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.5"
+version = "0.4.6"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.5/sweepai/api.py` & `sweepai-0.4.6/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/app/api_client.py` & `sweepai-0.4.6/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/app/backend.py` & `sweepai-0.4.6/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/app/cli.py` & `sweepai-0.4.6/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/app/config.py` & `sweepai-0.4.6/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/app/ui.py` & `sweepai-0.4.6/sweepai/app/ui.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -375,20 +375,20 @@
 
     def validate_branch_name(branch_name):
         # Replace any characters that are not alphanumeric or '-' or '_' with '_'
         valid_branch_name = re.sub('[^0-9a-zA-Z_-]', '_', branch_name)
         return valid_branch_name
 
     def on_create_pr_button_click(chat_history: list[tuple[str | None, str | None]], plan: list[tuple[str]]):
-        chat_history.append((None, "⌛ Creating PR..."))
-        yield chat_history
         title = chat_history[0][0]
         content = chat_history[-1][1]
         # Validate the branch name before it's used in the create_pr function
         valid_branch_name = validate_branch_name(title.lower().replace(" ", "_").replace("-", "_")[:50])
+        chat_history.append((None, "⌛ Creating PR..."))
+        yield chat_history
         pull_request = api_client.create_pr(
             file_change_requests=[(item[:item.find(":")], item[item.find(":") + 1:]) for item, *_ in plan],
             pull_request={
                 "title": title,
                 "content": content,
                 "branch_name": valid_branch_name
             },
```

### Comparing `sweepai-0.4.5/sweepai/core/chat.py` & `sweepai-0.4.6/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/code_repair.py` & `sweepai-0.4.6/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/entities.py` & `sweepai-0.4.6/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/gha_extraction.py` & `sweepai-0.4.6/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/prompts.py` & `sweepai-0.4.6/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/react.py` & `sweepai-0.4.6/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/sweep_bot.py` & `sweepai-0.4.6/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/core/vector_db.py` & `sweepai-0.4.6/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/events.py` & `sweepai-0.4.6/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/handlers/create_pr.py` & `sweepai-0.4.6/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.6/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/handlers/on_comment.py` & `sweepai-0.4.6/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/handlers/on_review.py` & `sweepai-0.4.6/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/handlers/on_ticket.py` & `sweepai-0.4.6/sweepai/handlers/on_ticket.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
         logger.info("Max tokens exceeded")
         log_error("Max Tokens Exceeded", str(e) + "\n" + traceback.format_exc())
         if chat_logger.is_paying_user():
             edit_sweep_comment(f"Sorry, I could not edit `{e.filename}` as this file is too long. We are currently working on improved file streaming to address this issue.\n", -1)
         else:
             edit_sweep_comment(f"Sorry, I could not edit `{e.filename}` as this file is too long.\n\nIf this file is incorrect, please describe the desired file in the prompt. However, if you would like to edit longer files, consider upgrading to [Sweep Pro](https://sweep.dev/) for longer context lengths.\n", -1)
         raise e
-    except NoFilesException:
+    except NoFilesException as e:
         logger.info("No files to change.")
         log_error("No Files to Change", str(e) + "\n" + traceback.format_exc())
         edit_sweep_comment("Sorry, I could find any appropriate files to edit to address this issue. If this is a mistake, please provide more context and I will retry!", -1)
         raise e
     except openai.error.InvalidRequestError as e:
         logger.error(traceback.format_exc())
         logger.error(e)
```

### Comparing `sweepai-0.4.5/sweepai/utils/chat_logger.py` & `sweepai-0.4.6/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/config/client.py` & `sweepai-0.4.6/sweepai/utils/config/client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/config/server.py` & `sweepai-0.4.6/sweepai/utils/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/diff.py` & `sweepai-0.4.6/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/event_logger.py` & `sweepai-0.4.6/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/file_change_functions.py` & `sweepai-0.4.6/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/github_utils.py` & `sweepai-0.4.6/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.6/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/scorer.py` & `sweepai-0.4.6/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/snippets.py` & `sweepai-0.4.6/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/sweepai/utils/utils.py` & `sweepai-0.4.6/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.5/PKG-INFO` & `sweepai-0.4.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.5
+Version: 0.4.6
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -125,14 +125,18 @@
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
 2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
+## 💰 Pricing
+* We charge $120/month for 60 GPT4 tickets per month.
+* For unpaid users, we offer 3 free GPT4 tickets per month.
+* We also offer unlimited GPT3.5 tickets.
 ## 🤝 Contributing
 
 Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
 
 ## 📘 Story
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.5 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.6 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
@@ -68,28 +68,30 @@
 this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
 gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
 right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
 ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 #### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð¤
-Contributing Contributions are welcome and greatly appreciated! For detailed
-guidelines on how to contribute, please see the [CONTRIBUTING.md]
-(CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
-docs.sweep.dev/). ## ð Story We were frustrated by small tickets, like
-simple bug fixes, annoying refactors, and small features. Each task required us
-to open our IDE to fix simple bugs. So we decided to leverage the capabilities
-of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
-this can solve entire tickets and can be parallelized + asynchronous:
-developers can spin up 10 tickets and Sweep will address them all at once. ##
-ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
-with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
-Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap](https://
-docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart](https://
-api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð°
+Pricing * We charge $120/month for 60 GPT4 tickets per month. * For unpaid
+users, we offer 3 free GPT4 tickets per month. * We also offer unlimited GPT3.5
+tickets. ## ð¤ Contributing Contributions are welcome and greatly
+appreciated! For detailed guidelines on how to contribute, please see the
+[CONTRIBUTING.md](CONTRIBUTING.md) file. For more detailed docs, see [ð
+Quickstart](https://docs.sweep.dev/). ## ð Story We were frustrated by small
+tickets, like simple bug fixes, annoying refactors, and small features. Each
+task required us to open our IDE to fix simple bugs. So we decided to leverage
+the capabilities of ChatGPT to address this directly in GitHub. Unlike existing
+AI solutions, this can solve entire tickets and can be parallelized +
+asynchronous: developers can spin up 10 tickets and Sweep will address them all
+at once. ## ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for
+Vector DB with MiniLM L12 as our embeddings model - Modal Labs for infra +
+deployment - Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap]
+(https://docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart]
+(https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
 history.com/#sweepai/sweep&Date) Consider starring us if you're using Sweep so
 more people hear about us!
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
                             and, of course, Sweep!
```

