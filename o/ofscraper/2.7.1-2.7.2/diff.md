# Comparing `tmp/ofscraper-2.7.1.tar.gz` & `tmp/ofscraper-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.7.1.tar", max compression
+gzip compressed data, was "ofscraper-2.7.2.tar", max compression
```

## Comparing `ofscraper-2.7.1.tar` & `ofscraper-2.7.2.tar`

### file list

```diff
@@ -1,57 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-07-09 23:45:40.296797 ofscraper-2.7.1/LICENSE
--rw-r--r--   0        0        0     2862 2023-07-09 23:45:40.296797 ofscraper-2.7.1/README.md
--rw-r--r--   0        0        0      607 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/__init__.py
--rw-r--r--   0        0        0     1016 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     9002 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9866 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1067 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     8238 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2859 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     9763 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0    10276 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     6012 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     3999 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3408 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9480 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0        0 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/classes/__init__.py
--rw-r--r--   0        0        0      804 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8861 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/classes/media.py
--rw-r--r--   0        0        0     7274 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3603 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/classes/posts.py
--rw-r--r--   0        0        0    14535 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/commands/check.py
--rw-r--r--   0        0        0     4946 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    14111 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6818 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10059 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     5037 2023-07-09 23:45:40.304797 ofscraper-2.7.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      696 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7683 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    29826 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1583 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    12152 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9703 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    13073 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    24710 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5435 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     7193 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0    10696 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7013 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1211 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0    29248 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/table.py
--rw-r--r--   0        0        0     5818 2023-07-09 23:45:40.308797 ofscraper-2.7.1/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1940 2023-07-09 23:46:13.453368 ofscraper-2.7.1/pyproject.toml
--rw-r--r--   0        0        0     4548 1970-01-01 00:00:00.000000 ofscraper-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-14 06:52:24.005885 ofscraper-2.7.2/LICENSE
+-rw-r--r--   0        0        0     2859 2023-07-14 06:52:24.005885 ofscraper-2.7.2/README.md
+-rw-r--r--   0        0        0      607 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/__init__.py
+-rw-r--r--   0        0        0     1016 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8591 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9690 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1060 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7357 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     3246 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9415 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9499 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5113 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4393 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3294 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9139 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/__init__.py
+-rw-r--r--   0        0        0      804 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8491 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     7278 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3737 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4655 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29810 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14593 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5353 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    14111 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6917 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10059 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     5033 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      709 2023-07-14 06:52:24.013884 ofscraper-2.7.2/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     1803 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      696 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7683 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    29766 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1583 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    12396 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9552 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    13552 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    24542 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5564 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     7300 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0    10769 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7013 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1211 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5785 2023-07-14 06:52:24.017885 ofscraper-2.7.2/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1940 2023-07-14 06:52:55.942082 ofscraper-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 ofscraper-2.7.2/PKG-INFO
```

### Comparing `ofscraper-2.7.1/LICENSE` & `ofscraper-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/README.md` & `ofscraper-2.7.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -37,16 +37,15 @@
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
-
-https://discord.gg/wN7uxEVHRK
+https://discord.gg/DV3aBeMu
     
 # Feature Requests
 
 https://ofscraper.clearflask.com/feedback
     
 Or the discord
```

### Comparing `ofscraper-2.7.1/ofscraper/__init__.py` & `ofscraper-2.7.2/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/__version__.py` & `ofscraper-2.7.2/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/__version__.pye` & `ofscraper-2.7.2/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/api/archive.py` & `ofscraper-2.7.2/ofscraper/api/archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,15 @@
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
-import ssl
-import certifi
 import math
-import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -27,16 +24,17 @@
 from rich.live import Live
 from rich.style import Style
 import arrow
 import ofscraper.constants as constants
 from ..utils import auth
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
-import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.AlT_SEM)
@@ -55,20 +53,18 @@
     else:
         ep=constants.archivedEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-        headers=auth.make_headers(auth.read_auth())
-        headers=auth.create_sign(url, headers)
-        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:  
+        async with c.requests(url)() as r:  
             if r.ok:
                 progress.remove_task(task)
-                posts =( await r.json())['list']
+                posts =(await r.json_())['list']
                 log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
                 if not posts:
                     posts= []
                 if len(posts)==0:
                     log.debug(f" {log_id} -> number of post found 0")
                 elif len(posts)>0:
                     log.debug(f"{log_id} -> number of archived post found {len(posts)}")
@@ -91,15 +87,15 @@
                             tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
 
                         elif len(required_ids)>0:
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_archived_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
             else:
                     log.debug(f"[bold]archived request status code:[/bold]{r.status}")
-                    log.debug(f"[bold]archived response:[/bold] {await r.text()}")
+                    log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
                     log.debug(f"[bold]archived headers:[/bold] {r.headers}")
                     progress.remove_task(task)
                     r.raise_for_status()
     return posts
 
 async def get_archived_post(model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting archived media...\n{task.description}"))
@@ -110,16 +106,15 @@
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
         
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                            sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.AlT_SEM)) as c: 
+        async with sessionbuilder.sessionBuilder()  as c: 
 
             oldarchived=cache.get(f"archived_{model_id}",default=[])
             log.trace("oldarchive {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldarchive: {str(x)}",oldarchived)))))
             oldtimeset=set(map(lambda x:x.get("id"),oldarchived))
             log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
             oldarchived=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldarchived))
             postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldarchived)))
@@ -154,15 +149,15 @@
     log.debug(f"[bold]Archived Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
-    log.trace(f"archive dupeset {dupeSet}")
+    log.trace(f"archive dupeset postids {dupeSet}")
     log.trace("archived raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo archive: {str(x)}",unduped)))))
     log.debug(f"[bold]Archived Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"archived_{model_id}",list(map(lambda x:{"id":x.get("id"),"postedAtPrecise":x.get("postedAtPrecise")},unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"archived_check_{model_id}{model_id}",unduped,expire=constants.CHECK_EXPIRY)
 
         cache.close()
```

### Comparing `ofscraper-2.7.1/ofscraper/api/highlights.py` & `ofscraper-2.7.2/ofscraper/api/paid.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,252 +3,229 @@
         _____                                               
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
-
-import asyncio
 import logging
+import asyncio
 import contextvars
-import aiohttp
-import ssl
-import certifi
-from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
+from tenacity import retry,stop_after_attempt,wait_random
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from rich.style import Style
-import ofscraper.constants as c
 import ofscraper.constants as constants
+from ..utils import auth
+from ..utils.paths import getcachepath
+import ofscraper.utils.console as console
 import ofscraper.utils.auth as auth
+import ofscraper.constants as constants
+import ofscraper.api.profile as profile
+from diskcache import Cache
+from ..utils.paths import getcachepath
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
-import ofscraper.utils.console as console
+import ofscraper.utils.args as args_ 
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
+cache = Cache(getcachepath())
+
+paid_content_list_name = 'list'
 log=logging.getLogger(__package__)
-sem = semaphoreDelayed(1)
+
+sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
+
 attempt = contextvars.ContextVar("attempt")
 
-async def get_stories_post(model_id):
-    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting story media...\n{task.description}"))
+
+
+
+
+
+
+
+
+async def get_paid_posts(username,model_id):
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting paid media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
-    page_count=0
     global tasks
     tasks=[]
+    page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=1)) as c: 
-            tasks.append(asyncio.create_task(scrape_stories(c,model_id,job_progress)))
+        async with sessionbuilder.sessionBuilder() as c:
+ 
+            tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress)))
+
+            
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
                     page_count=page_count+1
                     overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
                     output.extend(result)
                 tasks=list(filter(lambda x:x.done()==False,tasks))
             overall_progress.remove_task(page_task)  
-    log.trace("stories raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo stories: {str(x)}",output)))))
-    log.debug(f"[bold]stories+highlight Count without Dupes[/bold] {len(output)} found")
+    log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(output)} found")
+    # set purchash check values during scan
+    log.trace("paid raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo paid: {str(x)}",output)))))
+
+    cache.set(f"purchased_check_{model_id}",output,expire=constants.CHECK_EXPIRY)
+    cache.close()
     return output
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_stories( c,user_id,job_progress) -> list:
+async def scrape_paid(c,username,job_progress,offset=0):
+    """Takes headers to access onlyfans as an argument and then checks the purchased content
+    url to look for any purchased content. If it finds some it will return it as a list."""
     global sem
     global tasks
+    media = None
     attempt.set(attempt.get(0) + 1)
-    stories=None
     await sem.acquire()
     task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-  
-
-    url= constants.highlightsWithAStoryEP.format(user_id)
-    r=await c.request("get",url ,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.create_sign(url, headers))
-    
-    sem.release()
-    if  r.ok:
-        attempt.set(0)
-        stories =await r.json()
-        log.debug(f"stories: -> found stories ids {list(map(lambda x:x.get('id'),stories))}") 
-        log.trace("stories: -> stories raw {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo stories: {str(x)}",stories)))))
-        job_progress.remove_task(task)
-
-    else:
-        job_progress.remove_task(task)
-        r.raise_for_status()
-    return   stories 
+    async with c.requests(url=constants.purchased_contentEP.format(offset,username))() as r:
+        sem.release()
+        if r.ok:
+            data=await r.json_()
+            log.trace("paid raw {posts}".format(posts=  data))
+            attempt.set(0)
+            media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
+            log.debug(f"offset:{offset} -> media found {len(media)}")
+            log.debug(f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }")
+            log.debug(f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
+            if  data.get("hasMore"):
+                offset += len(media)
+                tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress,offset=offset)))
+            job_progress.remove_task(task)
+
+        else:
+            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
+            log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
+            log.debug(f"[bold]paid headers:[/bold] {r.headers}")
+            job_progress.remove_task(task)
+            r.raise_for_status()
+    return media
 
 
 
 
 
+async def get_all_paid_posts():
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting paid media...\n{task.description}"))
+    job_progress=Progress("{task.description}")
+    progress_group = Group(
+    overall_progress,
+    Panel(Group(job_progress)))
 
-async def get_highlight_post(model_id):
-
-    async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=1)) as c: 
-        overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting highlight list...\n{task.description}"))
-        job_progress=Progress("{task.description}")
-        progress_group = Group(
-        overall_progress,
-        Panel(Group(job_progress)))
-
-        output=[]
-
-        page_count=0
-        global tasks
-        tasks=[]    
-        with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+    output=[]
+    min_posts=100
+    global tasks
+    tasks=[]
+    page_count=0
+    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+        async with sessionbuilder.sessionBuilder() as c:
+            allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
+            log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
+            
         
-                tasks.append(asyncio.create_task(scrape_highlight_list(c,model_id,job_progress)))
-                page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
-                while len(tasks)!=0:
-                    for coro in asyncio.as_completed(tasks):
-                        result=await coro or []
-                        page_count=page_count+1
-                        overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                        output.extend(result)
-                    tasks=list(filter(lambda x:x.done()==False,tasks))
+            if len(allpaid)>min_posts:
+                splitArrays=[i for i in range(0, len(allpaid), min_posts)]
+                #use the previous split for timesamp
+                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=0,count=0,required=0)))
+                [ tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,count=0,required=0,offset=splitArrays[i])))
+                for i in range(1,len(splitArrays))]
+                # keeping grabbing until nothign left
+                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=len(allpaid))))
+            else:
+                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress)))
                 
-          
-        overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting highlight...\n{task.description}"))
-        job_progress=Progress("{task.description}")
-        progress_group = Group(
-        overall_progress,
-        Panel(Group(job_progress)))
-        with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-
-
-            output2=[]
-            page_count=0
-            tasks=[]
-                
-            [tasks.append(asyncio.create_task(scrape_highlights(c,i,job_progress))) for i in output]
+            
+            
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
                     page_count=page_count+1
                     overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                    output2.extend(result)
+                    output.extend(result)
                 tasks=list(filter(lambda x:x.done()==False,tasks))
-
-    # log.trace("stories+highlight raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo stories+highlight: {str(x)}",output)))))
-    # log.debug(f"[bold]stories+highlight Count without Dupes[/bold] {len(output)} found")
-    return output2
-
-
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_highlight_list( c,user_id,job_progress,offset=0) -> list:
-    global sem
-    global tasks
-    attempt.set(attempt.get(0) + 1)
-    await sem.acquire()
-    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-  
-
-    url= constants.highlightsWithStoriesEP.format(user_id,offset)
-
-    r=await c.request("get",url ,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.create_sign(url , headers))
-    
-    # highlights_, stories
-    sem.release()
-    if  r.ok:
-        attempt.set(0)
-        resp_data=(await r.json())
-        log.trace(f"highlights list: -> found highlights list data {resp_data}")
-        data=get_highlightList(resp_data)
-        log.debug(f"highlights list: -> found list ids {data}")
-    
-        job_progress.remove_task(task)
-        if resp_data.get("hasMore"):
-            tasks.append(asyncio.create_task(scrape_highlight_list(c,user_id,job_progress,offset+len(data))))
-
-
-
-    else:
-        job_progress.remove_task(task)
-        r.raise_for_status()
-    return  data
-
+            overall_progress.remove_task(page_task)  
+    unduped=[]
+    dupeSet=set()
+    log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
+    for post in output:
+        if post["id"] in dupeSet:
+            continue
+        dupeSet.add(post["id"])
+        unduped.append(post)
+    log.debug(f"[bold]Paid Post count[/bold] {len(unduped)} found")
+    cache.set(f"purchased_all",list(map(lambda x:x.get("id"),unduped)),expire=constants.RESPONSE_EXPIRY)
+    cache.close()
+    return unduped
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_highlights( c,id,job_progress) -> list:
+async def scrape_all_paid(c,job_progress,offset=0,count=0,required=0):
+    """Takes headers to access onlyfans as an argument and then checks the purchased content
+    url to look for any purchased content. If it finds some it will return it as a list."""
     global sem
     global tasks
+    media = None
     attempt.set(attempt.get(0) + 1)
     await sem.acquire()
-    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-  
-
-    url= constants.storyEP.format(id)
-
-    r=await c.request("get",url ,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=auth.create_sign(url , headers))
-    
-    # highlights_, stories
-    sem.release()
-    if  r.ok:
-        attempt.set(0)
-        resp_data=(await r.json())
-        log.trace(f"highlights: -> found highlights data {resp_data}")
-        log.debug(f"highlights: -> found ids {list(map(lambda x:x.get('id'),resp_data['stories']))}")
-        job_progress.remove_task(task)
-    else:
-        job_progress.remove_task(task)
-        r.raise_for_status()
-    return resp_data['stories']
-
-
-
-
-def get_highlightList(data):
-    for ele in list(filter(lambda x:isinstance(x,list),data.values())):
-        if len(list(filter(lambda x:isinstance(x.get("id"),int) and data.get("hasMore")!=None,ele)))>0:
-               return list(map(lambda x:x.get("id"),ele))
-    return []
-
-
-    
-
-
+    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} offset={offset}",visible=True)
+    async with c.requests(url= constants.purchased_contentALL.format(offset))() as r:
+        sem.release()
+        if r.ok:
+            attempt.set(0) 
+            log_id=f"offset {offset or 0}:"
+            data=await r.json_()   
+            job_progress.remove_task(task)
+            media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
+            if not data.get("hasMore"):
+                media=[]
+            if not media:
+                media=[]
+            if len(media)==0:
+                log.debug(f"{log_id} -> number of post found 0")
+            elif len(media)>0:
+                log.debug(f"{log_id} -> number of post found {len(media)}")
+                log.debug(f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}")
+                log.debug(f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}")
+                log.debug(f"{log_id} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
+
+                if required==0:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media))))
+
+                elif len(count)<len(required):
+                    tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media),required=required,count=count+len(media))))
+
+
+            
+
+        else:
+            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
+            log.debug(f"[bold]paid response:[/bold] {await r.text_()}")
+            log.debug(f"[bold]paid headers:[/bold] {r.headers}")
+            job_progress.remove_task(task)
+            r.raise_for_status()
+    return media
 
-def get_individual_highlight(id,client=None):
-    headers = auth.make_headers(auth.read_auth())
-    url=constants.highlightSPECIFIC.format(id)
-    auth.add_cookies(client)
-    client.headers.update(auth.create_sign(url, headers))
-    r=client.get(url)
-    if not r.is_error:
-        return r.json()
-    log.debug(f"{r.status_code}")
-    log.debug(f"{r.content.decode()}")
-
-def get_individual_stories(id,client=None):
-    headers = auth.make_headers(auth.read_auth())
-    url=constants.storiesSPECIFIC.format(id)
-    auth.add_cookies(client)
-    client.headers.update(auth.create_sign(url, headers))
-    r=client.get(url)
-    if not r.is_error:
-        return r.json()
-    log.debug(f"{r.status_code}")
-    log.debug(f"{r.content.decode()}")
```

### Comparing `ofscraper-2.7.1/ofscraper/api/init.py` & `ofscraper-2.7.2/ofscraper/api/init.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,13 +25,13 @@
             print('Status - \033[32mUP\033[0m')
         else:
             print('Status - \033[31mDOWN\033[0m')
 
 
 def getstatus(headers):
     try:
-        resp = me.scrape_user(headers)
+        me.scrape_user(headers)
         return "UP"
     except Exception as e:
         log.traceback(e)
         log.traceback(traceback.format_exc())
         return "DOWN"
```

### Comparing `ofscraper-2.7.1/ofscraper/api/labels.py` & `ofscraper-2.7.2/ofscraper/api/labels.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,39 +4,31 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
-import aiohttp
 import logging
 import contextvars
-import certifi
-import ssl
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from rich.style import Style
-import arrow
-import arrow
 import ofscraper.constants as constants
-import ofscraper.utils.auth as auth
-import ofscraper.utils.paths as paths
-from ..utils import auth
 import ofscraper.utils.console as console
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
-import ofscraper.utils.args as args_
+import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
 
@@ -48,16 +40,15 @@
     Panel(Group(job_progress)))
 
     output=[]
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
+       async with sessionbuilder.sessionBuilder() as c: 
 
             tasks.append(asyncio.create_task(scrape_labels(c,model_id,job_progress)))
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
@@ -72,38 +63,36 @@
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_labels(c,model_id,job_progress,offset=0):
     global sem
     global tasks
     labels = None
     attempt.set(attempt.get(0) + 1)
-    url = constants.labelsEP.format(model_id, offset)
+    
     await sem.acquire()
-    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-    headers=auth.create_sign(url, headers)
-    async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:  
+    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} {offset}",visible=True)
+    async with c.requests(url=constants.labelsEP.format(model_id, offset))() as r:
         sem.release()
         if r.ok:
-            data=await r.json()
+            data=await r.json_()
             attempt.set(0)
             labels=list(filter(lambda x:isinstance(x,list),data.values()))[0]
             log.debug(f"offset:{offset} -> labels names found {len(labels)}")
             log.debug(f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }")
             log.trace("offset:{offset} -> label names raw: {posts}".format(offset=offset,posts=data))  
 
             if data.get("hasMore"):
                 offset = data.get("nextOffset")
                 tasks.append(asyncio.create_task(scrape_labels(c, model_id,job_progress,offset=offset)))
             job_progress.remove_task(task)
             return data.get("list")
 
         else:
             log.debug(f"[bold]labels request status code:[/bold]{r.status}")
-            log.debug(f"[bold]labels response:[/bold] {await r.text()}")
+            log.debug(f"[bold]labels response:[/bold] {await r.text_()}")
             log.debug(f"[bold]labels headers:[/bold] {r.headers}")
             job_progress.remove_task(task)
             r.raise_for_status()
 
 
 async def get_labelled_posts(labels, username):
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting labels...\n{task.description}"))
@@ -113,16 +102,15 @@
     Panel(Group(job_progress)))
 
     output={}
     global tasks
     tasks=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
+        async with sessionbuilder.sessionBuilder() as c:
 
             [tasks.append(asyncio.create_task(scrape_labelled_posts(c,label,username,job_progress)))
                 for label in labels]
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
@@ -147,33 +135,30 @@
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_labelled_posts(c,label,model_id,job_progress,offset=0):
     global sem
     global tasks
     posts = None
     attempt.set(attempt.get(0) + 1)
-    url = constants.labelledPostsEP.format(model_id, offset, label['id'])
-    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-    headers=auth.create_sign(url, headers)
-    async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:  
+    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} : offset -> {offset} + label -> {label.get('name')}",visible=True)
+    async with c.requests(url=constants.labelledPostsEP.format(model_id, offset, label['id']))() as r:
         if r.ok:
-            data=await r.json()
+            data=await r.json_()
             attempt.set(0)
             posts=list(filter(lambda x:isinstance(x,list),data.values()))[0]
             log.debug(f"offset:{offset} -> labelled posts found {len(posts)}")
             log.debug(f"offset:{offset} -> hasMore value in json {data.get('hasMore','undefined') }")
             log.trace("{offset} -> {posts}".format(offset=offset,posts= "\n\n".join(list(map(lambda x:f"scrapeinfo label {str(x)}",posts)))))  
             if data.get("hasMore"):
                 offset += len(posts)
                 tasks.append(asyncio.create_task(scrape_labelled_posts(c, label, model_id,job_progress,offset=offset)))
             job_progress.remove_task(task)
  
         else:
             log.debug(f"[bold]labelled posts request status code:[/bold]{r.status}")
-            log.debug(f"[bold]labelled posts response:[/bold] {await r.text()}")
+            log.debug(f"[bold]labelled posts response:[/bold] {await r.text_()}")
             log.debug(f"[bold]labelled posts headers:[/bold] {r.headers}")
 
             job_progress.remove_task(task)
             r.raise_for_status()
 
     return label, posts
```

### Comparing `ofscraper-2.7.1/ofscraper/api/me.py` & `ofscraper-2.7.2/ofscraper/api/me.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,70 +7,73 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import logging
 from functools import lru_cache
 import json
-import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
 import ofscraper.constants as constants
-import ofscraper.utils.auth as auth
 import ofscraper.utils.encoding as encoding
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.logger as logger
 import ofscraper.constants as constants
 import ofscraper.utils.paths as paths
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 log=logging.getLogger(__package__)
 console=Console()
 
 from diskcache import Cache
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Trying to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
 def scrape_user(headers):
-    return _scraper_user_helper(json.dumps(headers))
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
+        return _scraper_user_helper(c,json.dumps(headers))
 
 
 @lru_cache(maxsize=None)
-def _scraper_user_helper(headers):
+@retry(stop=stop_after_attempt(0),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Trying to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
+def _scraper_user_helper(c,headers):
     headers = json.loads(headers)
     cache = Cache(paths.getcachepath())
     data=cache.get(f"myinfo_{headers['user-id']}",None)
     if not data:
-        with httpx.Client(http2=True, headers=headers) as c:
-            url = constants.meEP
-            auth.add_cookies(c)
-            c.headers.update(auth.create_sign(url, headers))
-            r = c.get(url, timeout=None)
-            if not r.is_error:
-                data=r.json()
-            r.raise_for_status()
-    cache.set(f"myinfo_{headers['user-id']}",data,constants.HOURLY_EXPIRY)
-    cache.close()
-    logger.updateSenstiveDict(data["id"],"userid")
-    logger.updateSenstiveDict(data["username"],"username")
-    logger.updateSenstiveDict(data["name"],"name")
+            with c.requests(constants.meEP)() as r:
+                if r.ok:
+                    data=r.json_()
+                    cache.set(f"myinfo_{headers['user-id']}",data,constants.HOURLY_EXPIRY)
+                    cache.close()
+                    logger.updateSenstiveDict(data["id"],"userid")
+                    logger.updateSenstiveDict(data["username"],"username")
+                    logger.updateSenstiveDict(data["name"],"name")
+                else:
+                    log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+                    log.debug(f"[bold]archived response:[/bold] {r.text_()}")
+                    log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+                    r.raise_for_status()
+                
+           
     return data
 
 def parse_user(profile):
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
 
     return (name, username)
 
 
 def print_user(name, username):
     with stdout.lowstdout():
         console.print(f'Welcome, {name} | {username}')
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-def parse_subscriber_count(headers):
-    with httpx.Client(http2=True, headers=headers) as c:
-        url = constants.subscribeCountEP
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-        r = c.get(url, timeout=None)
-        if not r.is_error:
-            data=r.json()
-            return data["subscriptions"]["all"]
-        r.raise_for_status()
+@retry(stop=stop_after_attempt(constants.MAX_SEMAPHORE),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+def parse_subscriber_count():
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
+        with c.requests(constants.subscribeCountEP)() as r:
+            if r.ok:
+                data=r.json_()
+                return data["subscriptions"]["all"]
+            else:
+                log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+                log.debug(f"[bold]archived response:[/bold] {r.text_()}")
+                log.debug(f"[bold]archived headers:[/bold] {r.headers}")
```

### Comparing `ofscraper-2.7.1/ofscraper/api/messages.py` & `ofscraper-2.7.2/ofscraper/api/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,16 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import asyncio
-import aiohttp
 import logging
 import ssl
-import certifi
 import contextvars
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
@@ -29,14 +27,16 @@
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 import ofscraper.utils.paths as paths
 from ..utils import auth
 import ofscraper.utils.console as console
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.utils.args as args_
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
 
 from diskcache import Cache
 cache = Cache(paths.getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
@@ -57,16 +57,15 @@
 
     tasks=[]
     responseArray=[]
     page_count=0
     #require a min num of posts to be returned
     min_posts=50
     with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
+        async with sessionbuilder.sessionBuilder() as c: 
             oldmessages=cache.get(f"messages_{model_id}",default=[]) if not args_.getargs().no_cache else []
             log.trace("oldamessage {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldtimeline: {str(x)}",oldmessages)))))
 
             oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
             log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
             oldmessages=list(filter(lambda x:(x.get("createdAt") or x.get("postedAt"))!=None,oldmessages))
             startdex=0 if len(oldmessages)==0 else \
@@ -109,15 +108,15 @@
     log.debug(f"[bold]Messages Count with Dupes[/bold] {len(responseArray)} found")
     for message in responseArray:
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
         oldmsgset.discard(message["id"])       
         unduped.append(message)
-    log.trace(f"messages dupeset {dupeSet}")
+    log.trace(f"messages dupeset messageids {dupeSet}")
     log.trace("messages raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo message: {str(x)}",unduped)))))
     if len(oldmsgset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"messages_{model_id}",list(map(lambda x:{"id":x.get("id"),"createdAt":x.get("createdAt") or x.get("postedAt") },unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"message_check_{model_id}",oldmessages,expire=constants.CHECK_EXPIRY)
 
         cache.close()
     elif len(oldmsgset)>0 and not (args_.getargs().before or args_.getargs().after):
@@ -134,24 +133,19 @@
     global tasks
     messages=None
     attempt.set(attempt.get(0) + 1)
     ep = constants.messagesNextEP if message_id else constants.messagesEP
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'}{url}")
 
-
     async with sem:
-        headers=auth.make_headers(auth.read_auth())
-        headers=auth.create_sign(url, headers)
-        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.requests(url=url)() as r:
             task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
-            
             if r.ok:
-
-                messages = (await r.json())['list']
+                messages = (await r.json_())['list']
                 log_id=f"offset messageid:{message_id if message_id else 'init id'}"
                 if not messages:
                     messages=[]
                 if len(messages)==0:
                     log.debug(f"{log_id} -> number of messages found 0")
                 elif len(messages)>0:
                     log.debug(f"{log_id} -> number of messages found {len(messages)}")
@@ -176,30 +170,25 @@
                         elif len(required_ids)>0:
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_messages(c, model_id,progress,message_id=messages[-1]['id'],required_ids=required_ids)))
                 progress.remove_task(task)
 
             else:
                 log.debug(f"[bold]message request status code:[/bold]{r.status}")
-                log.debug(f"[bold]message response:[/bold] {await r.text()}")
+                log.debug(f"[bold]message response:[/bold] {await r.text_()}")
                 log.debug(f"[bold]message headers:[/bold] {r.headers}")
 
                 progress.remove_task(task)
                 r.raise_for_status()
 
     return messages
 
-def get_individual_post(model_id,postid,client=None):
-    headers = auth.make_headers(auth.read_auth())
-    url=constants.messageSPECIFIC.format(model_id,postid)
-
-    auth.add_cookies(client)
-    client.headers.update(auth.create_sign(url, headers))
-    r=client.get(url)
-    if not r.is_error:
-        log.trace(f"message raw individual {r.json()}")
-        return r.json()['list'][0]
-    log.debug(f"{r.status_code}")
-    log.debug(f"{r.content.decode()}")
-
-
+def get_individual_post(model_id,postid,c=None):
+    with c.requests(url=constants.messageSPECIFIC.format(model_id,postid))() as r:
+        if r.ok:
+            log.trace(f"message raw individual {r.json()}")
+            return r.json()['list'][0]
+        else:
+            log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+            log.debug(f"[bold]archived response:[/bold] {r.text_()}")
+            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
```

### Comparing `ofscraper-2.7.1/ofscraper/api/paid.py` & `ofscraper-2.7.2/ofscraper/api/highlights.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,238 +3,237 @@
         _____                                               
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
+
 import asyncio
-import ssl
-import certifi
-import aiohttp
 import logging
 import contextvars
+from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
-from tenacity import retry,stop_after_attempt,wait_random
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from rich.style import Style
+import ofscraper.constants as c
 import ofscraper.constants as constants
-from ..utils import auth
-from ..utils.paths import getcachepath
-import ofscraper.utils.console as console
 import ofscraper.utils.auth as auth
-import ofscraper.constants as constants
-import ofscraper.api.profile as profile
-from diskcache import Cache
-from ..utils.paths import getcachepath
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
-import ofscraper.utils.args as args_
-
-cache = Cache(getcachepath())
+import ofscraper.utils.console as console
+import ofscraper.classes.sessionbuilder as sessionbuilder
 
-paid_content_list_name = 'list'
 log=logging.getLogger(__package__)
-
-sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
-
+sem = semaphoreDelayed(1)
 attempt = contextvars.ContextVar("attempt")
 
-
-
-
-
-
-
-
-
-async def get_paid_posts(username,model_id):
-    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting paid media...\n{task.description}"))
+async def get_stories_post(model_id):
+    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting story media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     output=[]
+    page_count=0
     global tasks
     tasks=[]
-    page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
-
-            tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress)))
-
-            
-            page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
-            while len(tasks)!=0:
-                for coro in asyncio.as_completed(tasks):
-                    result=await coro or []
-                    page_count=page_count+1
-                    overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                    output.extend(result)
-                tasks=list(filter(lambda x:x.done()==False,tasks))
-            overall_progress.remove_task(page_task)  
-    log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(output)} found")
-    # set purchash check values during scan
-    log.trace("paid raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo paid: {str(x)}",output)))))
-
-    cache.set(f"purchased_check_{model_id}",output,expire=constants.CHECK_EXPIRY)
-    cache.close()
+            async with sessionbuilder.sessionBuilder() as c:
+                tasks.append(asyncio.create_task(scrape_stories(c,model_id,job_progress)))
+                page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
+                while len(tasks)!=0:
+                    for coro in asyncio.as_completed(tasks):
+                        result=await coro or []
+                        page_count=page_count+1
+                        overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                        output.extend(result)
+                    tasks=list(filter(lambda x:x.done()==False,tasks))
+                overall_progress.remove_task(page_task)  
+    log.trace("stories raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo stories: {str(x)}",output)))))
+    log.debug(f"[bold]stories+highlight Count without Dupes[/bold] {len(output)} found")
     return output
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_paid(c,username,job_progress,offset=0):
-    """Takes headers to access onlyfans as an argument and then checks the purchased content
-    url to look for any purchased content. If it finds some it will return it as a list."""
+async def scrape_stories( c,user_id,job_progress) -> list:
     global sem
     global tasks
-    media = None
     attempt.set(attempt.get(0) + 1)
-    url = constants.purchased_contentEP.format(offset,username)
+    stories=None
     await sem.acquire()
-    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-    headers=auth.create_sign(url, headers)
-    async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} : user id -> {user_id}",visible=True)
+    async with c.requests(url=constants.highlightsWithAStoryEP.format(user_id))() as r:
         sem.release()
         if r.ok:
-            data=await r.json()
-            log.trace("paid raw {posts}".format(posts=  data))
             attempt.set(0)
-            media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
-            log.debug(f"offset:{offset} -> media found {len(media)}")
-            log.debug(f"offset:{offset} -> hasmore value in json {data.get('hasMore','undefined') }")
-            log.debug(f"offset:{offset} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
-            if  data.get("hasMore"):
-                offset += len(media)
-                tasks.append(asyncio.create_task(scrape_paid(c,username,job_progress,offset=offset)))
+            stories =await r.json_()
+            log.debug(f"stories: -> found stories ids {list(map(lambda x:x.get('id'),stories))}") 
+            log.trace("stories: -> stories raw {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo stories: {str(x)}",stories)))))
             job_progress.remove_task(task)
-
         else:
-            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
-            log.debug(f"[bold]paid response:[/bold] {await r.text()}")
-            log.debug(f"[bold]paid headers:[/bold] {r.headers}")
-            job_progress.remove_task(task)
+            log.debug(f"[bold]stories request status code:[/bold]{r.status}")
+            log.debug(f"[bold]stories response:[/bold] {await r.text_()}")
+            log.debug(f"[bold]stories headers:[/bold] {r.headers}")
             r.raise_for_status()
-    return media
+        return   stories 
+        
+    
+  
+    r
 
 
 
 
 
-async def get_all_paid_posts():
-    overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting paid media...\n{task.description}"))
-    job_progress=Progress("{task.description}")
-    progress_group = Group(
-    overall_progress,
-    Panel(Group(job_progress)))
 
-    output=[]
-    min_posts=100
-    global tasks
-    tasks=[]
-    page_count=0
-    with Live(progress_group, refresh_per_second=5,console=console.shared_console):
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
-            allpaid=cache.get(f"purchased_all",default=[]) if not args_.getargs().no_cache else []
-            log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
-            
+async def get_highlight_post(model_id):
+
+    async with sessionbuilder.sessionBuilder() as c:
+        overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting highlight list...\n{task.description}"))
+        job_progress=Progress("{task.description}")
+        progress_group = Group(
+        overall_progress,
+        Panel(Group(job_progress)))
+
+        output=[]
+
+        page_count=0
+        global tasks
+        tasks=[]    
+        with Live(progress_group, refresh_per_second=5,console=console.shared_console):
         
-            if len(allpaid)>min_posts:
-                splitArrays=[i for i in range(0, len(allpaid), min_posts)]
-                #use the previous split for timesamp
-                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=0,count=0,required=0)))
-                [ tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,count=0,required=0,offset=splitArrays[i])))
-                for i in range(1,len(splitArrays))]
-                # keeping grabbing until nothign left
-                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=len(allpaid))))
-            else:
-                tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress)))
+                tasks.append(asyncio.create_task(scrape_highlight_list(c,model_id,job_progress)))
+                page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
+                while len(tasks)!=0:
+                    for coro in asyncio.as_completed(tasks):
+                        result=await coro or []
+                        page_count=page_count+1
+                        overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
+                        output.extend(result)
+                    tasks=list(filter(lambda x:x.done()==False,tasks))
                 
-            
-            
+          
+        overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting highlight...\n{task.description}"))
+        job_progress=Progress("{task.description}")
+        progress_group = Group(
+        overall_progress,
+        Panel(Group(job_progress)))
+        with Live(progress_group, refresh_per_second=5,console=console.shared_console):
+
+
+            output2=[]
+            page_count=0
+            tasks=[]
+                
+            [tasks.append(asyncio.create_task(scrape_highlights(c,i,job_progress))) for i in output]
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True) 
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
                     page_count=page_count+1
                     overall_progress.update(page_task,description=f'Pages Progress: {page_count}')
-                    output.extend(result)
+                    output2.extend(result)
                 tasks=list(filter(lambda x:x.done()==False,tasks))
-            overall_progress.remove_task(page_task)  
-    unduped=[]
-    dupeSet=set()
-    log.debug(f"[bold]Paid Post count with Dupes[/bold] {len(output)} found")
-    for post in output:
-        if post["id"] in dupeSet:
-            continue
-        dupeSet.add(post["id"])
-        unduped.append(post)
-    log.debug(f"[bold]Paid Post count[/bold] {len(unduped)} found")
-    cache.set(f"purchased_all",list(map(lambda x:x.get("id"),unduped)),expire=constants.RESPONSE_EXPIRY)
-    cache.close()
-    return unduped
+
+    # log.trace("stories+highlight raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo stories+highlight: {str(x)}",output)))))
+    # log.debug(f"[bold]stories+highlight Count without Dupes[/bold] {len(output)} found")
+    return output2
+
+
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def scrape_highlight_list( c,user_id,job_progress,offset=0) -> list:
+    global sem
+    global tasks
+    attempt.set(attempt.get(0) + 1)
+    await sem.acquire()
+    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}",visible=True)
+    async with c.requests(url=constants.highlightsWithStoriesEP.format(user_id,offset))() as r:
+        sem.release()
+        if r.ok:
+            attempt.set(0)
+            resp_data=(await r.json_())
+            log.trace(f"highlights list: -> found highlights list data {resp_data}")
+            data=get_highlightList(resp_data)
+            log.debug(f"highlights list: -> found list ids {data}")
+    
+        else:
+            log.debug(f"[bold]highlight list request status code:[/bold]{r.status}")
+            log.debug(f"[bold]highlight list response:[/bold] {await r.text_()}")
+            log.debug(f"[bold]highlight list headers:[/bold] {r.headers}")
+    return  data
+
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_all_paid(c,job_progress,offset=0,count=0,required=0):
-    """Takes headers to access onlyfans as an argument and then checks the purchased content
-    url to look for any purchased content. If it finds some it will return it as a list."""
+async def scrape_highlights( c,id,job_progress) -> list:
     global sem
     global tasks
-    media = None
     attempt.set(attempt.get(0) + 1)
     await sem.acquire()
-    url = constants.purchased_contentALL.format(offset)
-    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} offset={offset}",visible=True)
-    headers=auth.make_headers(auth.read_auth())
-    headers=auth.create_sign(url, headers)
-    async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+    task=job_progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES} highlights id -> {id}",visible=True)
+    async with c.requests(url=constants.storyEP.format(id))() as r:
         sem.release()
         if r.ok:
-            attempt.set(0) 
-            log_id=f"offset {offset or 0}:"
-            data=await r.json()   
+            attempt.set(0)
+            resp_data=(await r.json_())
+            log.trace(f"highlights: -> found highlights data {resp_data}")
+            log.debug(f"highlights: -> found ids {list(map(lambda x:x.get('id'),resp_data['stories']))}")
             job_progress.remove_task(task)
-            media=list(filter(lambda x:isinstance(x,list),data.values()))[0]
-            if not data.get("hasMore"):
-                media=[]
-            if not media:
-                media=[]
-            if len(media)==0:
-                log.debug(f"{log_id} -> number of post found 0")
-            elif len(media)>0:
-                log.debug(f"{log_id} -> number of post found {len(media)}")
-                log.debug(f"{log_id} -> first date {media[0].get('createdAt') or media[0].get('postedAt')}")
-                log.debug(f"{log_id} -> last date {media[-1].get('createdAt') or media[-1].get('postedAt')}")
-                log.debug(f"{log_id} -> found paid content ids {list(map(lambda x:x.get('id'),media))}")
-
-                if required==0:
-                    attempt.set(0)
-                    tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media))))
+        else:
+            log.debug(f"[bold]highlight status code:[/bold]{r.status}")
+            log.debug(f"[bold]highlight response:[/bold] {r.text_()}")
+            log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
+    return resp_data['stories']
 
-                elif len(count)<len(required):
-                    tasks.append(asyncio.create_task(scrape_all_paid(c,job_progress,offset=offset+len(media),required=required,count=count+len(media))))
 
 
-            
 
-        else:
-            log.debug(f"[bold]paid request status code:[/bold]{r.status}")
-            log.debug(f"[bold]paid response:[/bold] {await r.text()}")
-            log.debug(f"[bold]paid headers:[/bold] {r.headers}")
-            job_progress.remove_task(task)
-            r.raise_for_status()
-    return media
+def get_highlightList(data):
+    for ele in list(filter(lambda x:isinstance(x,list),data.values())):
+        if len(list(filter(lambda x:isinstance(x.get("id"),int) and data.get("hasMore")!=None,ele)))>0:
+               return list(map(lambda x:x.get("id"),ele))
+    return []
+
+
+    
+
+
+
 
 
 
 
+def get_individual_highlights(id,c=None):
+    return get_individual_stories(id,c)
+    # with c.requests(constants.highlightSPECIFIC.format(id))() as r:
+    #     if r.ok:
+    #         log.trace(f"highlight raw highlight individua; {r.json()}")
+    #         return r.json()
+    #     else:
+    #         log.debug(f"[bold]highlight request status code:[/bold]{r.status}")
+    #         log.debug(f"[bold]highlightresponse:[/bold] {r.text_()}")
+    #         log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
+
+
+
+
+
+
+def get_individual_stories(id,c=None):
+    with c.requests(constants.storiesSPECIFIC.format(id))() as r:
+        if r.ok:
+            log.trace(f"highlight raw highlight individua; {r.json_()}")
+            return r.json()
+        else:
+            log.debug(f"[bold]highlight request status code:[/bold]{r.status}")
+            log.debug(f"[bold]highlightresponse:[/bold] {r.text_()}")
+            log.debug(f"[bold]highlight headers:[/bold] {r.headers}")
+
+
```

### Comparing `ofscraper-2.7.1/ofscraper/api/pinned.py` & `ofscraper-2.7.2/ofscraper/api/pinned.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,18 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import time
 import asyncio
-import ssl
-import certifi
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import logging
 import contextvars
 import math
-import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -27,14 +24,16 @@
 from rich.live import Live
 from rich.style import Style
 import arrow
 import ofscraper.constants as constants
 from ..utils import auth
 import ofscraper.utils.console as console
 import ofscraper.utils.args as args_
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.AlT_SEM)
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_pinned_posts(c, model_id,progress, timestamp=None,required_ids=None) -> list:
@@ -53,58 +52,47 @@
         ep=constants.timelinePinnedEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:         
+        async with c.requests(url=url)() as r:
+    
             if r.ok:
                 progress.remove_task(task)
                 posts =( await r.json())['list']
                 log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
                 if not posts:
                     posts= []
                 if len(posts)==0:
                     log.debug(f"{log_id} -> number of pinned post f found 0")
                 else:
                     log.debug(f"{log_id} -> number of pinned post found {len(posts)}")
                     log.debug(f"{log_id} -> first date {posts[0].get('createdAt') or posts[0].get('postedAt')}")
                     log.debug(f"{log_id} -> last date {posts[-1].get('createdAt') or posts[-1].get('postedAt')}")
                     log.debug(f"{log_id} -> found pinned post IDs {list(map(lambda x:x.get('id'),posts))}")
                     log.trace("{log_id} -> pinned raw {posts}".format(log_id=log_id,posts=  "\n\n".join(list(map(lambda x:f"scrapeinfo pinned: {str(x)}",posts)))))
-
-  
-                #post infinite loops            
-                # elif required_ids==None:
-                #     attempt.set(0)
-                    # tasks.append(asyncio.create_task(scrape_pinned_posts(headers, model_id,progress,timestamp=posts[0]['postedAtPrecise'])))
-            else:
-                    log.debug(f"[bold]pinned request status code:[/bold]{r.status}")
-                    log.debug(f"[bold]pinned response:[/bold] {await r.text()}")
-                    log.debug(f"[bold]pinned headers:[/bold] {r.headers}")
-                    progress.remove_task(task)
-                    r.raise_for_status()
-    return posts
+       
+        return posts
 
 async def get_pinned_post(model_id): 
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting pinned media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
 
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                                    sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
+       async with sessionbuilder.sessionBuilder() as c: 
             tasks.append(asyncio.create_task(scrape_pinned_posts(c,model_id,job_progress,timestamp=args_.getargs().after.float_timestamp if args_.getargs().after else None)))
         
 
             page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
             while len(tasks)!=0:
                 for coro in asyncio.as_completed(tasks):
                     result=await coro or []
@@ -118,11 +106,11 @@
     dupeSet=set()
     log.debug(f"[bold]Pinned Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         unduped.append(post)
-    log.trace(f"pinned dupeset {dupeSet}")
+    log.trace(f"pinned dupeset postids {dupeSet}")
     log.trace("pinned raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo pinned: {str(x)}",unduped)))))
     log.debug(f"[bold]Pinned Count without Dupes[/bold] {len(unduped)} found")
     return unduped
```

### Comparing `ofscraper-2.7.1/ofscraper/api/profile.py` & `ofscraper-2.7.2/ofscraper/api/profile.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,59 +7,66 @@
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import logging
 import contextvars
 
 from typing import Union
-import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import profileEP,NUM_TRIES,HOURLY_EXPIRY,DAILY_EXPIRY
 from ..utils import auth, encoding
 from xxhash import xxh128
 from diskcache import Cache
 from ..utils.paths import getcachepath
 import ofscraper.constants as constants
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 cache = Cache(getcachepath())
 
 
 log=logging.getLogger(__package__)
 console=Console()
 attempt = contextvars.ContextVar("attempt")
 
 
 
+
 # can get profile from username or id
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def scrape_profile(username:Union[int, str]) -> dict:
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
+        return scrape_profile_helper(c,username)
+
+
+  
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+def scrape_profile_helper(c,username:Union[int, str]):
     id=cache.get(f"username_{username}",None)
     log.trace(f"username date: {id}")
     if id:
         return id
     headers = auth.make_headers(auth.read_auth())
-
     attempt.set(attempt.get(0) + 1)
     log.info(f"Attempt {attempt.get()}/{constants.NUM_TRIES} to get profile {username}")
-    with httpx.Client(http2=True, headers=headers) as c:
-        url = profileEP.format(username)
-
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-
-        r = c.get(profileEP.format(username), timeout=None)
-        if not r.is_error:
+    with c.requests(profileEP.format(username))() as r:
+        if r.ok:
             attempt.set(0)
             cache.set(f"username_{username}",r.json(),int(HOURLY_EXPIRY*2))
             cache.close()
             log.trace(f"username date: {r.json()}")
             return r.json()
-        elif r.status_code==404:
+        elif r.status==404:
             return {"username":"modeldeleted"}
-        r.raise_for_status()
+        else:
+              log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+              log.debug(f"[bold]archived response:[/bold] {r.text_()}")
+              log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+              r.raise_for_status()
+
+
 
 
 def parse_profile(profile: dict) -> tuple:
     media = []
     media.append(profile.get('avatar'))
     media.append(profile.get('profile'))
     media=list(filter(lambda x:x!=None,media))
@@ -90,29 +97,31 @@
 def print_profile_info(info):
     header_fmt = 'Name: {} | Username: {} | ID: {} | Joined: {}\n'
     info_fmt = '- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts'
     final_fmt = header_fmt + info_fmt
     log.info(final_fmt.format(*info))
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def get_id( username):
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
+        return get_id_helper(c,username)
+
     
-    headers = auth.make_headers(auth.read_auth())
-    with httpx.Client(http2=True, headers=headers) as c:
-        url = profileEP.format(username)
-        id=cache.get(f"model_id_{username}",None)
-        if id:
-            return id
-        auth.add_cookies(c)
-        c.headers.update(auth.create_sign(url, headers))
-        r = c.get(url, timeout=None)
-        if not r.is_error:
+        
+        
+
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+def get_id_helper(c,username):
+    id=cache.get(f"model_id_{username}",None)
+    if id:
+        return id
+    with c.requests(profileEP.format(username))() as r:
+        if r.ok:
             id=r.json()['id']
             cache.set(f"model_id_{username}",id,DAILY_EXPIRY)
             cache.close()
             return id
-        
-        r.raise_for_status()
-
-
-        
+        else:
+            log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+            log.debug(f"[bold]archived response:[/bold] {r.text_()}")
+            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+            r.raise_for_status()
```

### Comparing `ofscraper-2.7.1/ofscraper/api/subscriptions.py` & `ofscraper-2.7.2/ofscraper/api/subscriptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,47 +6,48 @@
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 import asyncio
 from itertools import chain
-import ssl
-import certifi
 import logging
-import aiohttp
 from rich.console import Console
 import arrow
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import subscriptionsEP,NUM_TRIES
-from ..utils import auth, dates
 import ofscraper.constants as constants
 log=logging.getLogger(__package__)
+import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
-async def get_subscriptions(headers, subscribe_count):
+async def get_subscriptions(subscribe_count):
     offsets = range(0, subscribe_count, 10)
-    tasks = [scrape_subscriptions(headers, offset) for offset in offsets]
-    subscriptions = await asyncio.gather(*tasks)
-    return list(chain.from_iterable(subscriptions))
+    async with sessionbuilder.sessionBuilder() as c: 
+        tasks = [scrape_subscriptions(c,offset) for offset in offsets]
+        subscriptions = await asyncio.gather(*tasks)
+        return list(chain.from_iterable(subscriptions))
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
-async def scrape_subscriptions(headers, offset=0) -> list:
-    async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,sock_connect=None, sock_read=None)) as c: 
-        url = subscriptionsEP.format(offset)
-        headers=auth.make_headers(auth.read_auth())
-        headers=auth.create_sign(url, headers)
-        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+
+
+
+@retry(stop=stop_after_attempt(constants.MAX_SEMAPHORE),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def scrape_subscriptions(c,offset=0) -> list:
+
+        async with c.requests( subscriptionsEP.format(offset))() as r:
             if r.ok:
-                subscriptions = await r.json()
+                subscriptions = await r.json_()
                 log.debug(f"usernames offset {offset}: usernames retrived -> {list(map(lambda x:x.get('username'),subscriptions))}")      
                 return subscriptions
-            r.raise_for_status()
+            else:
+                log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+                log.debug(f"[bold]archived response:[/bold] {await r.text_()}")
+                log.debug(f"[bold]archived headers:[/bold] {r.headers}")
 
 def parse_subscriptions(subscriptions: list) -> list:
     datenow=arrow.now()
     data = [
         {"name":profile['username']
          ,"id":profile['id'],
          "sub-price":profile.get("currentSubscribePrice",{}),
```

### Comparing `ofscraper-2.7.1/ofscraper/api/timeline.py` & `ofscraper-2.7.2/ofscraper/api/timeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import time
 import asyncio
 import logging
 import ssl
 import certifi
 import contextvars
 import math
-import aiohttp
 from tenacity import retry,stop_after_attempt,wait_random
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TextColumn,
     SpinnerColumn
 )
@@ -28,14 +27,16 @@
 import arrow
 import ofscraper.constants as constants
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 from ..utils import auth
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
 import ofscraper.utils.args as args_
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
 
 sem = semaphoreDelayed(constants.MAX_SEMAPHORE)
@@ -54,20 +55,18 @@
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelineEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-        headers=auth.make_headers(auth.read_auth())
-        headers=auth.create_sign(url, headers)
-        async with c.request("get",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with  c.requests(url=url)() as r:
             if r.ok:
                 progress.remove_task(task)
-                posts = (await r.json())['list']
+                posts = (await r.json_())['list']
                 log_id=f"timestamp:{arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}"
                 if not posts:
                     posts= []
                 if len(posts)==0:
                     log.debug(f"{log_id} -> number of post found 0")
 
 
@@ -89,15 +88,15 @@
                             tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
 
                         elif len(required_ids)>0:
                             attempt.set(0)
                             tasks.append(asyncio.create_task(scrape_timeline_posts(c, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
             else:
                     log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
-                    log.debug(f"[bold]timeline response:[/bold] {await r.text()}")
+                    log.debug(f"[bold]timeline response:[/bold] {await r.text_()}")
                     log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
 
                     progress.remove_task(task)
                     r.raise_for_status()
     return posts
 
 async def get_timeline_post(model_id): 
@@ -110,16 +109,15 @@
     global tasks
     tasks=[]
     min_posts=50
     responseArray=[]
     page_count=0
     
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                      sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as c: 
+        async with sessionbuilder.sessionBuilder() as c:
 
             oldtimeline=cache.get(f"timeline_{model_id}",default=[]) if not args_.getargs().no_cache else []
             log.trace("oldtimeline {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"oldtimeline: {str(x)}",oldtimeline)))))
 
             oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
             log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
             oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
@@ -155,15 +153,15 @@
     log.debug(f"[bold]Timeline Count with Dupes[/bold] {len(responseArray)} found")
     for post in responseArray:
         if post["id"] in dupeSet:
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
-    log.trace(f"timeline dupeset {dupeSet}")
+    log.trace(f"timeline dupeset postids {dupeSet}")
     log.trace("post raw unduped {posts}".format(posts=  "\n\n".join(list(map(lambda x:f"undupedinfo timeline: {str(x)}",unduped)))))
     log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0 and not (args_.getargs().before or args_.getargs().after):
         cache.set(f"timeline_{model_id}",list(map(lambda x:{"id":x.get("id"),"postedAtPrecise":x.get("postedAtPrecise")},unduped)),expire=constants.RESPONSE_EXPIRY)
         cache.set(f"timeline_check_{model_id}",unduped,expire=constants.CHECK_EXPIRY)
         cache.close()
     elif len(oldtimeset)>0 and not (args_.getargs().before or args_.getargs().after):
@@ -171,20 +169,18 @@
         cache.set(f"timeline_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
 
         cache.close()
         log.debug("Some post where not retrived resetting cache")
     return unduped                                
 
 
-def get_individual_post(id,client=None):
-    headers = auth.make_headers(auth.read_auth())
-    url=f"https://onlyfans.com/api2/v2/posts/{id}?skip_users=all"
-    auth.add_cookies(client)
-    client.headers.update(auth.create_sign(url, headers))
-    r=client.get(url)
-    if not r.is_error:
-        log.trace(f"post raw individual {r.json()}")
-        return r.json()
-    log.debug(f"{r.status_code}")
-    log.debug(f"{r.content.decode()}")
-    
+def get_individual_post(id,c=None):
+    with c.requests(constants.INDVIDUAL_TIMELINE.format(id))() as r:
+        if r.ok:
+            log.trace(f"message raw individual {r.json()}")
+            return r.json()
+        else:
+            log.debug(f"[bold]archived request status code:[/bold]{r.status}")
+            log.debug(f"[bold]archived response:[/bold] {r.text_()}")
+            log.debug(f"[bold]archived headers:[/bold] {r.headers}")
+
```

### Comparing `ofscraper-2.7.1/ofscraper/classes/labels.py` & `ofscraper-2.7.2/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/classes/media.py` & `ofscraper-2.7.2/ofscraper/classes/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import re
-import aiohttp
 import arrow
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
 import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
 import ofscraper.constants as constants
 import ofscraper.utils.config as config
 import certifi
 import ssl
 import logging
 import traceback
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
 log=logging.getLogger(__package__)
 class Media():
     def __init__(self, media, count, post):
         self._media = media
         self._count = count
         self._post = post
@@ -255,22 +256,19 @@
     @property
     @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
     async def parse_mpd(self): 
         if not self.mpd:
             return
         try:
             params={"Policy":self.policy,"Key-Pair-Id":self.keypair,"Signature":self.signature}
-            async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=constants.API_REEQUEST_TIMEOUT, connect=None,
-                                        sock_connect=None, sock_read=None),connector = aiohttp.TCPConnector(limit=constants.MAX_SEMAPHORE)) as session:
-                headers=auth.make_headers(auth.read_auth())
-                headers=auth.create_sign(self.mpd, headers) 
-                async with session.request("get",self.mpd,headers=headers,params=params,ssl=ssl.create_default_context(cafile=certifi.where())) as r:
+            async with sessionbuilder.sessionBuilder() as c:
+                async with c.requests(url=self.mpd,params=params)() as r:
                     if not r.ok:
                         return None
-                    return MPEGDASHParser.parse(await r.text())
+                    return MPEGDASHParser.parse(await r.text_())
         except Exception as E:
             log.traceback(traceback.format_exc())
             log.traceback(E)
             raise E
  
     
     @property
```

### Comparing `ofscraper-2.7.1/ofscraper/classes/placeholder.py` & `ofscraper-2.7.2/ofscraper/classes/placeholder.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
     @wrapper
     def getmediadir(self,ele,username,model_id):
         self._variables.update({"username":username})
         self._variables.update({"model_id":model_id})
         user_name=username;self._variables.update({"user_name":username})
         modelid=model_id;self._variables.update({"modelid":modelid})
-        post_id=ele.postid;self._variables.update({"post_id":post_id})
-        postid=ele.postid;self._variables.update({"postid":postid})
+        post_id=ele.postid_;self._variables.update({"post_id":post_id})
+        postid=ele.postid_;self._variables.update({"postid":postid})
         media_id=ele.id;self._variables.update({"media_id":media_id})
         mediaid=ele.id;self._variables.update({"mediaid":mediaid})
         first_letter=username[0].capitalize();self._variables.update({"first_letter":first_letter})
         firstletter=username[0].capitalize();self._variables.update({"firstletter":firstletter})
         mediatype=ele.mediatype.capitalize();self._variables.update({"mediatype":mediatype})
         media_type=ele.mediatype.capitalize();self._variables.update({"media_type":media_type})
         value=ele.value.capitalize();self._variables.update({"value":value})
@@ -102,16 +102,16 @@
             return f"{filename}.{ext}"
         self._variables.update({"username":username})
         self._variables.update({"model_id":model_id})
         self._variables.update({"ext":ext})
 
         user_name=username;self._variables.update({"user_name":username})
         modelid=model_id;self._variables.update({"modelid":modelid})
-        post_id=ele.postid;self._variables.update({"post_id":post_id})
-        postid=ele.postid;self._variables.update({"postid":postid})
+        post_id=ele.postid_;self._variables.update({"post_id":post_id})
+        postid=ele.postid_;self._variables.update({"postid":postid})
         media_id=ele.id;self._variables.update({"media_id":media_id})
         mediaid=ele.id;self._variables.update({"mediaid":mediaid})
         first_letter=username[0].capitalize();self._variables.update({"first_letter":first_letter})
         firstletter=username[0].capitalize();self._variables.update({"firstletter":firstletter})
         mediatype=ele.mediatype.capitalize();self._variables.update({"mediatype":mediatype})
         media_type=ele.mediatype.capitalize();self._variables.update({"media_type":media_type})
         value=ele.value.capitalize();self._variables.update({"value":value})
```

### Comparing `ofscraper-2.7.1/ofscraper/classes/posts.py` & `ofscraper-2.7.2/ofscraper/classes/posts.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,19 +60,23 @@
     def responsetype(self):
         if self.archived:
             if config.get_archived_responsetype(config.read_config()) == "":
                 return "archived"
             return config.get_archived_responsetype(config.read_config())
 
         else:
-            response=config.read_config().get("responsetype", {}).get(self._responsetype_) 
+            responseType=self._responsetype_
+            #remap some values
+            responseType="timeline" if responseType=="post" else responseType
+            response=config.read_config().get("responsetype", {}).get(responseType) 
+
             if  response == "":
-                return self._responsetype_.capitalize()
+                return responseType.capitalize()
             elif  response == None:
-                return self._responsetype_.capitalize()
+                return responseType.capitalize()
             elif  response != "":
                 return  response.capitalize()
 
     @property
     def id(self):
         return self._post["id"]
```

### Comparing `ofscraper-2.7.1/ofscraper/commands/check.py` & `ofscraper-2.7.2/ofscraper/commands/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
 import re
 import time
 import asyncio
 import threading
 import queue
 import textwrap
-import httpx
 import arrow
 import ofscraper.utils.args as args_
 import ofscraper.db.operations as operations
 import ofscraper.api.profile as profile
 import ofscraper.utils.auth as auth
 import ofscraper.api.timeline as timeline
 import ofscraper.api.messages as messages_
 import ofscraper.classes.posts as posts_
 import ofscraper.constants as constants
 import ofscraper.api.paid as paid_
 import ofscraper.api.archive as archive
-import ofscraper.api.pinned as pinned
-import ofscraper.api.highlights as highlights_
+import ofscraper.api.highlights as highlights
 import ofscraper.utils.console as console_
-import ofscraper.utils.table as table
+import ofscraper.classes.table as table
 import ofscraper.commands.manual as manual
 import ofscraper.utils.download as download
 import ofscraper.db.operations as operations
 import ofscraper.constants as constants
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 
 from diskcache import Cache
 from ..utils.paths import getcachepath
 cache = Cache(getcachepath())
 
 log = logging.getLogger(__package__)
 args = args_.getargs()
@@ -51,26 +51,26 @@
                     media_id=app.row_names.index('Media_ID')
                     url=None
                     if row[restype].plain=="message":
                         url=constants.messagesNextEP.format(row[username].plain,row[post_id].plain)
                     elif row[restype].plain=="post":
                         url=f"{row[post_id]}"
                     elif row[restype].plain=="highlights":
-                        url=constants.highlightsWithStoriesEP.format(row[post_id].plain)
+                        url=constants.storyEP.format(row[post_id].plain)
                     elif row[restype].plain=="stories":
                         url=constants.highlightsWithAStoryEP.format(row[post_id].plain)
                     else:
                         log.info("URL not supported")
                         continue
                     log.info(f"Added url {url}")
                     log.info("Sending URLs to OF-Scraper")
                     media_dict= manual.get_media_from_urls(urls=[url])
                     # None for stories and highlights
                     medialist=list(filter(lambda x: x.id==(int(row[media_id].plain) if x.id else None) ,list(media_dict.values())[0]))
-                    media=medialist[0]
+                    media=medialist[0] if len(medialist)>0 else []
                     model_id =media.post.model_id
                     username=media.post.username
                     log.info(f"Downloading Invidual media for {username} {media.filename}")
                     operations.create_tables(model_id,username)
                     operations.write_profile_table(model_id,username)
                     values=asyncio.run(download.process_dicts(
                     username,
@@ -94,15 +94,15 @@
 
 
 
 
 
 def post_checker():
     user_dict = {}
-    with httpx.Client(http2=True, headers=  auth.make_headers(auth.read_auth())) as c:
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
         links = list(url_helper())
         for ele in links:
             name_match = re.search(f"onlyfans.com/({constants.USERNAME_REGEX}+$)", ele)
             name_match2 = re.search(f"^{constants.USERNAME_REGEX}+$", ele)
 
             if name_match:
                 user_name = name_match.group(1)
@@ -269,25 +269,26 @@
 def stories_checker():
     user_dict = {}
     ROWS=[]
     for user_name in args.username:
         user_name=profile.scrape_profile(user_name)["username"]
         user_dict[user_name] = user_dict.get(user_name, [])
         model_id = profile.get_id( user_name)    
-        highlights, stories = asyncio.run(highlights_.get_highlight_post( model_id))
-        highlights=list(map(lambda x:posts_.Post(
-        x, model_id, user_name,"highlights"), highlights))
+        stories = asyncio.run(highlights.get_stories_post( model_id))
+        highlights_=asyncio.run(highlights.get_highlight_post( model_id))
+        highlights_=list(map(lambda x:posts_.Post(
+        x, model_id, user_name,"highlights"), highlights_))
         stories=list(map(lambda x:posts_.Post(
         x, model_id, user_name,"stories"), stories))
             
 
      
         downloaded = get_downloaded(user_name, model_id)
         media=[]
-        [media.extend(ele.all_media) for ele in stories+highlights]
+        [media.extend(ele.all_media) for ele in stories+highlights_]
         ROWS.extend(row_gather(media, downloaded, user_name))
     reset_url()
     set_count(ROWS)
     thread_starters(ROWS)
```

### Comparing `ofscraper-2.7.1/ofscraper/commands/manual.py` & `ofscraper-2.7.2/ofscraper/commands/manual.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 import logging
 import asyncio
-import httpx
 import ofscraper.utils.args as args_
 import ofscraper.api.timeline as timeline
 import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
-import ofscraper.utils.auth as auth
 import ofscraper.classes.posts as posts_
 import ofscraper.db.operations as operations
 import ofscraper.utils.download as download
 import ofscraper.api.messages as messages_
 import ofscraper.api.highlights as highlights_
 import ofscraper.constants as constants
+import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.utils.of as of
 
 
 log = logging.getLogger(__package__)
 
 
 def manual_download(urls=None):
     media_dict=get_media_from_urls(urls)
@@ -38,36 +38,37 @@
 
 def get_media_from_urls(urls):
     args = args_.getargs()
     args.dupe=True
     args_.changeargs(args)
     user_name_dict={}
     id_dict={}
-    with httpx.Client(http2=True) as c:
+    with sessionbuilder.sessionBuilder(backend="httpx") as c:
+
         for url in url_helper(urls):
             response=get_info(url)
             model=response[0]
             postid=response[1]
             type=response[2]
             if type=="post":
                 model_id=user_name_dict.get(model) or profile.get_id( model)
                 user_name_dict[model]=model_id
-                id_dict[model_id]=id_dict.get(model_id,[])+[timeline.get_individual_post(postid,client=c)]
+                id_dict[model_id]=id_dict.get(model_id,[])+[timeline.get_individual_post(postid,c=c)]
             elif type=="msg":
                 model_id=model
-                id_dict[model_id]=id_dict.get(model_id,[])+[messages_.get_individual_post(model_id,postid,client=c)]
+                id_dict[model_id]=id_dict.get(model_id,[])+[messages_.get_individual_post(model_id,postid,c=c)]
             elif type=="msg2":
                 model_id=user_name_dict.get(model) or profile.get_id( model)
-                id_dict[model_id]=id_dict.get(model_id,[])+[messages_.get_individual_post(model_id,postid,client=c)]
+                id_dict[model_id]=id_dict.get(model_id,[])+[messages_.get_individual_post(model_id,postid,c=c)]
             elif type=="unknown":
                 data=unknown_type_helper(postid,c) or {}
                 model_id=data.get("author",{}).get("id")
                 id_dict[model_id]=id_dict.get(model_id,[])+[data]
             elif type=="highlights":
-                data=highlights_.get_individual_highlight(postid,c) or {}
+                data=highlights_.get_individual_highlights(postid,c) or {}
                 model_id=data.get("userId")
                 id_dict[model_id]=id_dict.get(model_id,[])+[data]
                 #special case
                 return get_all_media(id_dict,"highlights")
             elif type=="stories":
                 data=highlights_.get_individual_stories(postid,c) or {}
                 model_id=data.get("userId")
@@ -96,45 +97,56 @@
         if model_id==None:
             continue
         temp = []
         user_name = profile.scrape_profile( model_id)['username']
         posts_array=list(map(lambda x:posts_.Post(
         x, model_id, user_name,responsetype=inputtype), value))
         [temp.extend(ele.media) for ele in posts_array]
-        media_dict[model_id]=temp
-   
-   
+        if len(temp)==0:
+            temp.extend(paid_failback(model_id,user_name))
+        media_dict[model_id]=temp   
     return media_dict
 
+def paid_failback(id,username):
+    log.debug("Using failback search because query return 0 media")
+    return of.process_paid_post(id,username) 
+    
+
+
+
+
     
 
 def get_info(url):
     search1=re.search(f"chats/chat/({constants.NUMBER_REGEX}+)/.*?({constants.NUMBER_REGEX}+)",url)
     search2=re.search(f"/({constants.NUMBER_REGEX}+)/stories/highlights",url)
-    search3=re.search(f"/({constants.NUMBER_REGEX}+)/stories",url)
-    search4=re.search(f"chats/({constants.USERNAME_REGEX}+)/.*?id=({constants.NUMBER_REGEX}+)",url)
-    search5=re.search(f"/({constants.NUMBER_REGEX}+)/({constants.USERNAME_REGEX}+)",url)
-    search6=re.search(f"^{constants.NUMBER_REGEX}+$",url)
+    search3=re.search(f"/stories/highlights/({constants.NUMBER_REGEX}+)",url)
+
+    search4=re.search(f"/({constants.NUMBER_REGEX}+)/stories",url)
+    search5=re.search(f"chats/({constants.USERNAME_REGEX}+)/.*?id=({constants.NUMBER_REGEX}+)",url)
+    search6=re.search(f"/({constants.NUMBER_REGEX}+)/({constants.USERNAME_REGEX}+)",url)
+    search7=re.search(f"^{constants.NUMBER_REGEX}+$",url)
   #model,postid,type
 
     if search1:
         return search1.group(1),search1.group(2),"msg"
-    elif search2:
-        return None,search2.group(1),"highlights"
-    elif search3:
-        return None,search3.group(1),"stories"
-
-
+    elif search2 or search3:
+        search=search2 or search3
+        return None,search.group(1),"highlights"
     elif search4:
-        return search4.group(1),search4.group(2),"msg2"
+        return None,search4.group(1),"stories"
+
 
     elif search5:
-        return search5.group(2),search5.group(1),"post"
+        return search5.group(1),search5.group(2),"msg2"
+
     elif search6:
-        return None,search6.group(0),"unknown"
+        return search6.group(2),search6.group(1),"post"
+    elif search7:
+        return None,search7.group(0),"unknown"
 
 
     return None,None,None
 
 
 def url_helper(urls):
     args = args_.getargs()
```

### Comparing `ofscraper-2.7.1/ofscraper/commands/scraper.py` & `ofscraper-2.7.2/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/constants.py` & `ofscraper-2.7.2/ofscraper/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # LIST NAMES (IF HARDCODED, MOST WILL BE AUTOMATIC
 
 of_posts_list_name = 'list'
 
 
 initEP = 'https://onlyfans.com/api2/v2/init'
 
+INDVIDUAL_TIMELINE="https://onlyfans.com/api2/v2/posts/{}?skip_users=all"
 meEP = 'https://onlyfans.com/api2/v2/users/me'
 
 subscriptionsEP = 'https://onlyfans.com/api2/v2/subscriptions/subscribes?offset={}&type=all&sort=asc&field=expire_date&limit=10'
 subscribeCountEP='https://onlyfans.com/api2/v2/subscriptions/count/all'
 profileEP = 'https://onlyfans.com/api2/v2/users/{}'
 
 timelineEP = 'https://onlyfans.com/api2/v2/users/{}/posts?limit=100&order=publish_date_asc&skip_users=all&skip_users_dups=1&pinned=0&format=infinite'
@@ -102,16 +103,19 @@
 SAVE_PATH_DEFAULT=str(pathlib.Path.home()/'Data/ofscraper')
 DATE_DEFAULT="MM-DD-YYYY"
 PROFILE_DEFAULT="main_profile"
 PREMIUM_DEFAULT="Premium"
 MP4DECRYPT_DEFAULT=""
 FFMPEG_DEFAULT =""
 DISCORD_DEFAULT =""
+BACKEND_DEFAULT ="aio"
+
 DYNAMIC_DEFAULT="deviint"
 SUPPRESS_LOG_LEVEL=21
+
 RESPONSE_TYPE_DEFAULT= {
             "message":"Messages",
             "timeline":"Posts",
             "archived":"Archived",
             "paid":"Messages",
             "stories":"Stories",
             "highlights":"Stories",
```

### Comparing `ofscraper-2.7.1/ofscraper/db/operations.py` & `ofscraper-2.7.2/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/db/queries.py` & `ofscraper-2.7.2/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/interaction/like.py` & `ofscraper-2.7.2/ofscraper/interaction/like.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def _like_request(c,id,model_id):
     async with sem:
         url = favoriteEP.format(id, model_id)
         headers=auth.make_headers(auth.read_auth())
         headers=auth.create_sign(url, headers)
-        async with c.request("post",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.request("post",url,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies(),headers=headers) as r:
             if r.ok:
                 return id                  
             log.debug(f"[bold]timeline request status code:[/bold]{r.status}")
             log.debug(f"[bold]timeline response:[/bold] {await r.text()}")
             log.debug(f"[bold]timeline headers:[/bold] {r.headers}")
             r.raise_for_status()
```

### Comparing `ofscraper-2.7.1/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.7.2/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.7.2/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/prompts/prompts.py` & `ofscraper-2.7.2/ofscraper/prompts/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,57 +9,39 @@
 """
 import sys
 from rich.console import Console
 import pathlib
 import re
 import arrow
 from InquirerPy.resolver import prompt
-from InquirerPy import inquirer
 from InquirerPy.separator import Separator
 from InquirerPy.base import Choice
 from InquirerPy import get_style
 from InquirerPy.validator import EmptyInputValidator,PathValidator
 import ofscraper.constants as constants
 import ofscraper.prompts.prompt_strings as prompt_strings
 import ofscraper.prompts.prompt_validators as prompt_validators
 import ofscraper.utils.config as config
 import ofscraper.utils.args as args_
-
+import ofscraper.prompts.promptConvert as promptClasses
 console=Console()
 def main_prompt() -> int:
     main_prompt_choices = [*constants.mainPromptChoices]
     main_prompt_choices.insert(3, Separator())
+    answer=promptClasses.getMultiSection(           
+            message= 'What would you like to do?',
+            choices = [*main_prompt_choices]
 
-    name = 'action'
-
-    questions = [
-        {
-            'type': 'list',
-            'name': name,
-            'message': 'What would you like to do?',
-            'choices': [*main_prompt_choices],
-        }
-    ]
-
-    answer = prompt(questions)
-    return constants.mainPromptChoices[answer[name]]
-
-
-
-
-
-
-
-
-
+    
+    ).execute()
+    return constants.mainPromptChoices[answer]
 
 def areas_prompt() -> list:
-    name = 'areas'
-
-    questions = [
+    name="value"
+    answers=promptClasses.batchConverter(* [
         {
             'type': 'checkbox',
             'qmark': '[?]',
             'name': name,
             'message': 'Which area(s) would you like to scrape? (Press ENTER to continue)',
              "validate":prompt_validators.emptyListValidator(),
             'choices': [
@@ -72,59 +54,59 @@
                 Choice('Messages'),
                 Choice("Purchased"),
                 Choice("Labels")
             ]
             ,"instruction":prompt_strings.CHECKLISTINSTRUCTIONS,
 
         }
-    ]
-    answers = prompt(questions)
+    ])
     return answers[name]
 
 
 def like_areas_prompt() -> list:
     name = 'areas'
 
-    questions = [
+    answers=promptClasses.batchConverter(*[
         {
             'type': 'checkbox',
             'qmark': '[?]',
             'name': name,
             'message': 'Which area(s) would you to perform like/unlike actions on',
              "validate":prompt_validators.emptyListValidator(),
             'choices': [
                 Choice('Timeline'),
                 Choice('Pinned'),
                 Choice('Archived'),
             ]
             ,"instruction":prompt_strings.CHECKLISTINSTRUCTIONS,
 
         }
-    ]
-    answers = prompt(questions)
+    ])
     return answers[name]
 
 def scrape_paid_prompt():
-    questions = [
+    name="value"
+    answer=promptClasses.batchConverter(*[
+      
         {
             'type': 'list',
+            "name":name,
             'message': "Scrape entire paid page [WARNING ONLY USE IF NEEDED i.e for DELETED MODELS]",
             'choices':[Choice(True,"True"),Choice(False,"False",enabled=True)],
             'long_instruction': prompt_strings.SCRAPE_PAID,
             "default":False
 
         },
 
-    ]
+    ])
 
-    answer = prompt(questions)
-    return answer[0]
+    return answer[name]
 
 def auth_prompt(auth) -> dict:
-    questions = [
+    answers = promptClasses.batchConverter(*[
         {
             'type': 'input',
             'name': 'sess',
             'message': 'Enter your sess cookie:',
             'default': auth['sess']
             ,'validate':EmptyInputValidator()
 
@@ -152,141 +134,146 @@
         {
             'type': 'input',
             'name': 'x-bc',
             'message': 'Enter your `x-bc` token:',
             'default': auth['x-bc']
             ,'validate':EmptyInputValidator()
         }
-    ]
+    ])
 
-    answers = prompt(questions)
     return answers
 
 
 def ask_make_auth_prompt() -> bool:
     name = 'make_auth'
 
-    questions = [
+    questions = promptClasses.batchConverter(*[
         {
             'type': 'confirm',
             'name': name,
             'message': "You don't seem to have an `auth.json` file. Would you like to make one?",
         }
-    ]
+    ])
 
-    answer = prompt(questions)
-    return answer[name]
+    return questions[name]
 
 def browser_prompt()->str:
     pythonver=float(f"{sys.version_info[0]}.{sys.version_info[1]}")
-    msg="Select how to retrive auth information"
+    name="browser"
+    answer=None
 
     if pythonver<3.9 or pythonver>=3.11:
+        msg="Select how to retrive auth information"
         console.print("\nNote: Browser Extractions only works with default browser profile\n\n")
-        questions = [
+        answer=promptClasses.batchConverter(*[
             {
                 'type': 'list',
                 'message':msg ,
+                "name":name,
                 'choices':["Enter Each Field Manually","Paste From M-rcus\' OnlyFans-Cookie-Helper", Separator(line="-----------\nBrowser Extractions"),"Chrome","Chromium","Firefox","Opera","Opera GX","Edge","Chromium","Brave","Vivaldi","Safari"],
                 "default":"Enter Each Field Manually",
 
             }
-        ]
+        ])
         
 
     else:
         console.print("\nNote:To enable automatic extraction install ofscraper with python 3.9 or 3.10\n\n")
         msg="Select how to retrive auth information"
-        questions = [
+        answer= promptClasses.batchConverter(*[
         {
             'type': 'list',
             'message': msg,
             'choices':["Enter Each Field Manually","Paste From Cookie Helper"],
             "default":"Enter Each Field Manually"
 
         }
-    ]  
+    ]  )
       
-    return prompt(questions)[0]
+    return answer[name]
 def user_agent_prompt(current):
-    questions = [
+    name="input"
+    questions = promptClasses.batchConverter(*[
         {
             'type': 'input',
+            "name":name,
             'message':'Enter User_Agent from browser',
             'default':current,
             'validate':EmptyInputValidator(),
             'filter':lambda x:prompt_validators.cleanTextInput(x)
         }
-    ]
-    return  prompt(questions)[0]
+    ])
+    return  questions[name]
 
 def xbc_prompt():
-    questions = [
+    name="input"
+    questions = promptClasses.batchConverter(*[
         {
             'type': 'input',
+            "name":name,
             'message':'Enter x-bc request header',
             'instruction':f"\nGo to browser network tools to view\nFor more instructions visit https://github.com/datawhores/ofscraper\n\n"
             ,'validate':EmptyInputValidator(),
             'filter':lambda x:prompt_validators.cleanTextInput(x)
         }
-    ]
-    return  prompt(questions)[0]
+    ])
+    return questions[name]
 
 
 
 
 def auth_full_paste():
-    questions = [
+    name="input"
+    questions = promptClasses.batchConverter(*[
         {
             'type': 'input',
+            "name":name,
             'message':'Paste Text from Extension',
             "validate": prompt_validators.jsonValidator(),
             "filter":prompt_validators.jsonloader,
              "instruction":\
 """
 Cookie Helper Repo:https://github.com/M-rcus/OnlyFans-Cookie-Helper
 """
              
 
         }
-    ]
-    return prompt(questions)[0]
+    ])
+    return questions[name]
     
 def profiles_prompt() -> int:
     name = 'profile'
 
-    questions = [
+    questions = promptClasses.batchConverter(*[
         {
             'type': 'list',
             'name': name,
             'message': 'Select one of the following:',
             'choices': [*constants.profilesPromptChoices]
         }
-    ]
+    ])
 
-    answer = prompt(questions)
-    return constants.profilesPromptChoices[answer[name]]
+    return constants.profilesPromptChoices.get(questions[name])
 
 
 def edit_profiles_prompt(profiles) -> str:
     name = 'edit'
 
     profile_names = [profile.stem for profile in profiles]
 
-    questions = [
+    questions =promptClasses.batchConverter(* [
         {
             'type': 'list',
             'name': name,
             'message': 'Which profile would you like to edit?',
             'choices': [*profile_names]
         }
-    ]
+    ])
 
-    answer = prompt(questions)
-    return answer[name]
+    return questions[name]
 
 
 def new_name_edit_profiles_prompt(old_profile_name) -> str:
     name = 'new_name'
 
     questions = [
         {
@@ -360,22 +347,27 @@
         },
 
         {
             'type': 'filepath',
             'name': 'client-id',
             'message': 'Enter path to client id file',
             'default': config.get_client_id(config_) or "",
-            "validate":prompt_validators.MultiValidator(EmptyInputValidator(),PathValidator(is_file=True)),
         },
          {
             'type': 'filepath',
             'name': 'private-key',
             'message': 'Enter path to private-key',
             'default': config.get_private_key(config_)  or "",
-            "validate":prompt_validators.MultiValidator(EmptyInputValidator(),PathValidator(is_file=True)),
+        },
+        {
+            'type': 'list',
+            'name': 'backend',
+            'choices':[Choice("aio","aiohttp"),Choice("httpx","httpx")],
+            'message': 'Select Which Backend you want:\n',
+            'default': config.get_backend(config_) or "",
         },
         {
             'type': 'list',
             'name': 'partfileclean',
             'message': 'auto clean .part files',
             "long_instruction":"You won't be able to resume downloads if you select 'Yes'",
             'default': config.get_part_file_clean(config_),
@@ -757,44 +749,38 @@
     "fuzzy_info": "#abb2bf",
     "fuzzy_border": "#4b5263",
     "fuzzy_match": "#c678dd bold",
     "spinner_pattern": "#e5c07b",
     "spinner_text": "",
 })
 
-    p=inquirer.fuzzy(
-        long_instruction=prompt_strings.FUZZY_INSTRUCTION.format(sort=args_.getargs().sort.capitalize(),
+    p=promptClasses.getMultiSection(fuzzy=True,
+                                    long_instruction=prompt_strings.FUZZY_INSTRUCTION.format(sort=args_.getargs().sort.capitalize(),
                                                                  desc=args_.getargs().desc,
                                                                  type=(args_.getargs().account_type or "All").capitalize(),
                                                                 status=(args_.getargs().sub_status or "Both").capitalize(),
                                                                 renewal=(args_.getargs().renewal or "Both").capitalize()
 
                                                                 
                                                                 ),
 
                                                                  
         choices=choices,
         transformer=lambda result:",".join(map(lambda x:x.split(" ")[1],result)),
         multiselect=True,
         validate=prompt_validators.emptyListValidator(),
         prompt='Filter: ',
-        marker="\u25c9 ",
-        marker_pl="\u25cb ",
         message= "Which models do you want to scrape\n:",
         mandatory=False,
-        style=style,
-        keybindings=  {
-                                "toggle": [{"key": "s-right"},{"key": ["pagedown","right"]},{"key": ["home","right"]}],
-
-                                
-                        }
-                            
+        style=style,)
+    
+    
+    
+    
     
-    )
-        
     answers=p.execute()
     return list(map(lambda x:x["name"],answers or [])),p
         
 
 def model_selectorHelper(count,x):
     format='YYYY-MM-DD'
     expired=arrow.get(x['expired']).format(format) if x['expired'] else None
@@ -911,19 +897,15 @@
     
     questions = [
         
      
         
         
         {
-               "keybindings":{
-                             "answer": [{"key": ["pagedown","enter"]},{"key": ["home","enter"]}],
-
-                              
-                         },
+              
             'type': 'input',
             'multiline':True,
             'default':configText,
             'message': "Edit config text",
             "instruction":"\nKeyBindings\nSubmit: esc+Enter or Home+Enter or pageDown +Enter",
         }
     ]
```

### Comparing `ofscraper-2.7.1/ofscraper/start.py` & `ofscraper-2.7.2/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/args.py` & `ofscraper-2.7.2/ofscraper/utils/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,20 @@
     post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
     post.add_argument(
         '-o', '--posts', help = 'Download content from a model',default=[],required=False,type = posttype_helper,action='extend'
     )
 
     post.add_argument("-sk","--skip-timed",default=None,help="skip promotional or temporary post",action="store_true")
     post.add_argument(
-        '-ft', '--filter', help = 'Filter post by provide regex\nNote if you include any uppercase characters the search will be case-sensitive',default=".*",required=False,type = str
+        '-ft', '--filter', help = 'Filter post to where the provided regex True\nNote if you include any uppercase characters the search will be case-sensitive',default=".*",required=False,type = str
+    )
+
+
+    post.add_argument(
+        '-nf', '--neg-filter', help = 'Filter post by provide regex is False\nNote if you include any uppercase characters the search will be case-sensitive',default=None,required=False,type = str
     )
     post.add_argument(
         '-sp', '--scrape-paid', help = 'scrape the entire paid page for content. This can take a very long time',default=False,required=False,action="store_true"
     )
 
     post.add_argument(
         '-dt', '--download-type', help = 'Filter to what type of download you want None==Both, protected=Files that need mp4decrpyt',default=None,required=False,type=str.lower,choices=["protected","normal"]
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/auth.py` & `ofscraper-2.7.2/ofscraper/utils/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 import hashlib
 import json
 import time
 import logging
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
-import httpx
+
 import browser_cookie3
 from .profiles import get_active_profile
 from ..prompts.prompts import *
 from ..constants import configPath, DIGITALCRIMINALS, requestAuth,DEVIINT
 import ofscraper.utils.paths as paths
+import ofscraper.classes.sessionbuilder as sessionbuilder
 
 
 console=Console()
 log=logging.getLogger(__package__)
 
 def read_auth():
-    make_request_auth()
-
     authFile=paths.get_auth_file()
    
     while True:
         try:
             with open(authFile, 'r') as f:
                 authText=f.read()
                 auth = json.loads(authText)
@@ -151,28 +150,16 @@
         'x-bc': auth['auth']['x-bc'],
         'referer': 'https://onlyfans.com',
         'user-agent': auth['auth']['user_agent'],
     }
     return headers
 
 
-def add_cookies(client):
-    authFile=paths.get_auth_file()
-    with open(authFile, 'r') as f:
-        auth = json.load(f)
-
-    domain = 'onlyfans.com'
-
-    auth_uid = 'auth_uid_{}'.format(auth['auth']['auth_id'])
 
-    client.cookies.set('sess', auth['auth']['sess'], domain=domain)
-    client.cookies.set('auth_id', auth['auth']['auth_id'], domain=domain)
-    if auth['auth']['auth_uid_']:
-        client.cookies.set(auth_uid, auth['auth']['auth_uid_'], domain=domain)
-def add_cookies_aio():
+def add_cookies():
 
     authFile=paths.get_auth_file()
     with open(authFile, 'r') as f:
         auth = json.load(f)
 
     cookies={}
     cookies.update({"sess": auth['auth']['sess']})
@@ -268,31 +255,31 @@
 def get_request_auth():
     if (args_.getargs().dynamic_rules or config.get_dynamic(config.read_config()) or "deviint")=="deviint":
         return get_request_auth_deviint()
     else:
         return get_request_digitalcriminals()
 
 def get_request_auth_deviint():
-    with httpx.Client(http2=True) as c:
-        r = c.get(DEVIINT)
-    if not r.is_error:
-        content = r.json()
-        static_param = content['static_param']
-        fmt = f"{content['start']}:{{}}:{{:x}}:{content['end']}" 
-        checksum_indexes = content['checksum_indexes']
-        checksum_constant = content['checksum_constant']
-        return (static_param, fmt, checksum_indexes, checksum_constant)
-    else:
-        return []
-    
+    with sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False) as c:
+        with c.requests(DEVIINT)() as r:
+            if r.ok:
+                content = r.json_()
+                static_param = content['static_param']
+                fmt = f"{content['start']}:{{}}:{{:x}}:{content['end']}" 
+                checksum_indexes = content['checksum_indexes']
+                checksum_constant = content['checksum_constant']
+                return (static_param, fmt, checksum_indexes, checksum_constant)
+            else:
+                return []
+        
 def get_request_digitalcriminals():
-    with httpx.Client(http2=True) as c:
-        r = c.get(DIGITALCRIMINALS)
-    if not r.is_error:
-        content = r.json()
-        static_param = content['static_param']
-        fmt = content['format']
-        checksum_indexes = content['checksum_indexes']
-        checksum_constant = content['checksum_constant']
-        return (static_param, fmt, checksum_indexes, checksum_constant)
-    else:
-        return []
+   with sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False) as c:
+        with c.requests(DIGITALCRIMINALS)() as r:
+            if r.ok:
+                content = r.json_()
+                static_param = content['static_param']
+                fmt = content['format']
+                checksum_indexes = content['checksum_indexes']
+                checksum_constant = content['checksum_constant']
+                return (static_param, fmt, checksum_indexes, checksum_constant)
+            else:
+                return []
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/binaries.py` & `ofscraper-2.7.2/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/config.py` & `ofscraper-2.7.2/ofscraper/utils/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,16 @@
             "ffmpeg":get_ffmpeg(config),
              "discord":get_discord(config),
              "private-key":get_private_key(config),
              "client-id":get_client_id(config),
             "key-mode-default":get_key_mode(config),
             "dynamic-mode-default":get_dynamic(config),
             "partfileclean":get_part_file_clean(config),
+            "backend":get_backend(config),
+
             "responsetype":{
            "timeline":get_timeline_responsetype(config),
          "message":get_messages_responsetype(config),
             "archived":get_archived_responsetype(config),
             "paid":get_paid_responsetype(config),
             "stories":get_stories_responsetype(config),
             "highlights":get_highlights_responsetype(config),
@@ -300,14 +302,21 @@
     else:
         constants.FILTER_DEFAULT
 def get_timeline_responsetype(config=None):
     if config==None:
         return constants.RESPONSE_TYPE_DEFAULT["timeline"]
     return config.get('responsetype',{}).get("timeline") or config.get('responsetype',{}).get("post") or constants.RESPONSE_TYPE_DEFAULT["timeline"]
 
+def get_post_responsetype(config=None):
+    if config==None:
+        return constants.RESPONSE_TYPE_DEFAULT["timeline"]
+    return  config.get('responsetype',{}).get("post") or config.get('responsetype',{}).get("timeline") or constants.RESPONSE_TYPE_DEFAULT["timeline"]
+
+
+
 def get_archived_responsetype(config=None):
     if config==None:
         return constants.RESPONSE_TYPE_DEFAULT["archived"]
     return config.get('responsetype',{}).get("archived") or constants.RESPONSE_TYPE_DEFAULT["archived"]
 
 def get_stories_responsetype(config=None):
     if config==None:
@@ -370,7 +379,13 @@
         return constants.DYNAMIC_DEFAULT
     value=config.get("dynamic-mode-default")
     return value.lower() if value and value.lower() in set(["deviint","dc"]) else "deviint"
 def get_part_file_clean(config=None):
     if config==None:
         return False
     return config.get("partfileclean",False) or False
+
+
+def get_backend(config=None):
+    if config==None:
+        return "aio"
+    return config.get("backend",constants.BACKEND_DEFAULT) or constants.BACKEND_DEFAULT
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/dates.py` & `ofscraper-2.7.2/ofscraper/utils/dates.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,7 +24,10 @@
 
 def convert_date_to_timestamp(date: str):
     datetime_obj = datetime.fromisoformat(date)
     return datetime_obj.timestamp()
 def convert_local_time(date:str):
     return arrow.get(date,tzinfo='UTC').to('local').float_timestamp
 
+
+def get_current_time():
+    return arrow.get(tzinfo='UTC').to('local').float_timestamp
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/download.py` & `ofscraper-2.7.2/ofscraper/utils/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,20 +8,17 @@
                  \/     \/           \/            \/         
 """
 import asyncio
 import math
 import pathlib
 import platform
 import shutil
-import ssl
-import certifi
 import traceback
 import re
 import logging
-import aiohttp
 import contextvars
 import json
 import subprocess
 from rich.progress import Progress
 from rich.progress import (
     Progress,
     TimeElapsedColumn,
@@ -57,44 +54,52 @@
 import ofscraper.utils.logger as logger
 import ofscraper.utils.console as console
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args_
 from ofscraper.utils.semaphoreDelayed import semaphoreDelayed
 import ofscraper.classes.placeholder as placeholder
+import ofscraper.classes.sessionbuilder as sessionbuilder
+
 from diskcache import Cache
 cache = Cache(paths.getcachepath())
 attempt = contextvars.ContextVar("attempt")
 log=logging.getLogger(__package__)
 log_trace=True if "TRACE" in set([args_.getargs().log,args_.getargs().output,args_.getargs().discord]) else False
 
 
 
+
+
 async def process_dicts(username, model_id, medialist):
     with stdout.lowstdout():
         overall_progress=Progress(  TextColumn("{task.description}"),
         BarColumn(),TaskProgressColumn(),TimeElapsedColumn())
         job_progress=Progress(TextColumn("{task.description}",table_column=Column(ratio=2)),BarColumn(),
         TaskProgressColumn(),TimeRemainingColumn(),TransferSpeedColumn(),DownloadColumn())
         progress_group = Group(
         overall_progress
         , Panel(Group(job_progress,fit=True)))
         # This need to be here: https://stackoverflow.com/questions/73599594/asyncio-works-in-python-3-10-but-not-in-python-3-8
         global sem
         sem = semaphoreDelayed(config_.get_threads(config_.read_config()))
+
+        global dirSet
+        dirSet=set()
      
 
         with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console):    
                 if not args_.getargs().dupe:
                     media_ids = set(operations.get_media_ids(model_id,username))
                     log.debug(f"number of unique media ids in database for {username}: {len(media_ids)}")
                     medialist = seperate.separate_by_id(medialist, media_ids)
-                    log.debug(f"Number of new mediaids to download: {len(medialist)}")  
+                    log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")  
                     medialist=seperate.seperate_avatars(medialist)
-                    log.debug(f"Remove avatar and return final number of new mediaids to download: {len(medialist)}")
+                    log.debug(f"Remove avatar")
+                    log.debug(f"Final Number of media to downlaod {len(medialist)}")
 
                 else:
                     log.info(f"forcing all downloads media count {len(medialist)}")
                 file_size_limit = config_.get_filesize()
                   
                 aws=[]
                 photo_count = 0
@@ -102,16 +107,15 @@
                 audio_count=0
                 skipped = 0
                 total_bytes_downloaded = 0
                 data = 0
                 desc = 'Progress: ({p_count} photos, {v_count} videos, {a_count} audios,  {skipped} skipped || {sumcount}/{mediacount}||{data})'    
 
               
-                async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None, connect=None,
-                      sock_connect=None, sock_read=None)) as c: 
+                async with sessionbuilder.sessionBuilder() as c:
                     i=0
                     for ele in medialist:
                         aws.append(asyncio.create_task(download(c,ele ,model_id, username,file_size_limit,job_progress)))
                     task1 = overall_progress.add_task(desc.format(p_count=photo_count, v_count=video_count,a_count=audio_count, skipped=skipped,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped,data=data), total=len(aws),visible=True)
                     # progress_group.renderables[1].height=max(15,console.shared_console.size[1]-2)
                     for coro in asyncio.as_completed(aws):
                             try:
@@ -132,14 +136,15 @@
                             elif media_type == 'audios':
                                 audio_count += 1
                             elif media_type == 'skipped':
                                 skipped += 1
                             overall_progress.update(task1,description=desc.format(
                                         p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
         overall_progress.remove_task(task1)
+    setDirectoriesDate()
     log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
     return photo_count+video_count+audio_count,skipped
 def retry_required(value):
     return value == ('skipped', 1)
 
 async def download(c,ele,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)  
@@ -167,14 +172,15 @@
     elif abs(total-pathlib.Path(temp).absolute().stat().st_size)>500:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size mixmatch target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         return "skipped",1 
     else:
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {ele.filename_} size match target: {total} vs actual: {pathlib.Path(temp).absolute().stat().st_size}")   
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(temp).absolute()} -> {path_to_file}")   
         shutil.move(temp,path_to_file)
+        addGlobalDir(path)
         if ele.postdate:
             newDate=dates.convert_local_time(ele.postdate)
             log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
             set_time(path_to_file,newDate )
             log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
 
         if ele.id:
@@ -183,48 +189,46 @@
         return ele.mediatype,total
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def main_download_downloader(c,ele,path,file_size_limit,username,model_id,progress):
     try:
         url=ele.url
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {ele.filename_} with {url}")
         await sem.acquire()
-        pathlib.Path(temp).unlink(missing_ok=True) if (args_.getargs().part_cleanup or config_.get_part_file_clean(config_.read_config()) or False) else None
         temp=paths.truncate(pathlib.Path(path,f"{ele.filename}_{ele.id}.part"))
+        pathlib.Path(temp).unlink(missing_ok=True) if (args_.getargs().part_cleanup or config_.get_part_file_clean(config_.read_config()) or False) else None
         resume_size=0 if not pathlib.Path(temp).exists() else pathlib.Path(temp).absolute().stat().st_size
         cache.close()
         headers=None
-        total=None
+        
         path_to_file=None
        
 
-      
-        async with c.request("get",url,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=None,headers=None) as r:
+        async with c.requests(url=url)() as r:
                 if r.ok:
                     rheaders=r.headers
                     total = int(rheaders['Content-Length'])
                     if file_size_limit>0 and total > int(file_size_limit): 
                             return total ,"skipped",None 
                        
                     content_type = rheaders.get("content-type").split('/')[-1]
                     filename=placeholder.Placeholders().createfilename(ele,username,model_id,content_type)
                     path_to_file = paths.truncate(pathlib.Path(path,f"{filename}")) 
                 else:
                     r.raise_for_status()          
                                    
         if total!=resume_size:
-            headers={"Range":f"bytes={resume_size}-{total}"}
-            async with c.request("get",url,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=None,headers=headers) as r:
+            async with c.requests(url=url,headers={"Range":f"bytes={resume_size}-{total}"})() as r:
                 if r.ok:
                     pathstr=str(path_to_file)
                     if not total or (resume_size!=total):
                         task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
                         size=0
                         with open(temp, 'ab') as f: 
                             progress.update(task1,visible=True )
-                            async for chunk in r.content.iter_chunked(1024):
+                            async for chunk in r.iter_chunked(1024):
                                 size=size+len(chunk) if log_trace else size
                                 log.trace(f"Media:{ele.id} Post:{ele.postid} Download:{size}/{total}")
                                 f.write(chunk)
                                 progress.update(task1, advance=len(chunk))
                             progress.remove_task(task1)  
                 else:
                     r.raise_for_status() 
@@ -288,14 +292,15 @@
         log.debug(f"Media:{ele.id} Post:{ele.postid} ffmpeg {t.stderr.decode()}")
         log.debug(f"Media:{ele.id} Post:{ele.postid} ffmpeg {t.stdout.decode()}")
 
     video["path"].unlink(missing_ok=True)
     audio["path"].unlink(missing_ok=True)
     log.debug(f"Moving intermediate path {temp_path} to {path_to_file}")
     shutil.move(temp_path,path_to_file)
+    addGlobalDir(path_to_file)
     if ele.postdate:
         newDate=dates.convert_local_time(ele.postdate)
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}")  
         set_time(path_to_file,newDate )
         log.debug(f"Media:{ele.id} Post:{ele.postid} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}")  
     if ele.id:
         await operations.write_media_table(ele,path_to_file,model_id,username)
@@ -333,37 +338,35 @@
     try:
         base_url=re.sub("[0-9a-z]*\.mpd$","",ele.mpd,re.IGNORECASE)
         url=f"{base_url}{item['origname']}"
         log.debug(f"Media:{ele.id} Post:{ele.postid} Attempting to download media {item['origname']} with {url}")
         await sem.acquire()
         params={"Policy":ele.policy,"Key-Pair-Id":ele.keypair,"Signature":ele.signature}   
         temp= paths.truncate(pathlib.Path(path,f"{item['name']}.part"))
-        headers=auth.make_headers(auth.read_auth())
         pathlib.Path(temp).unlink(missing_ok=True) if (args_.getargs().part_cleanup or config_.get_part_file_clean(config_.read_config()) or False) else None
         resume_size=0 if not pathlib.Path(temp).exists() else pathlib.Path(temp).absolute().stat().st_size
         total=None
-        
-        async with c.request("get",url,params=params,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as r:
+        async with c.requests(url=url,params=params)() as r:
             if r.ok:
                 rheaders=r.headers
                 total = int(rheaders['Content-Length'])
                 if file_size_limit>0 and total > int(file_size_limit): 
                         return total ,None,None 
                 r.raise_for_status()  
         if total!=resume_size:
             headers={"Range":f"bytes={resume_size}-{total}"}  
-            async with c.request("get",url,params=params,allow_redirects=True,ssl=ssl.create_default_context(cafile=certifi.where()),cookies=auth.add_cookies_aio(),headers=headers) as l:
+            async with c.requests(url=url,headers=headers,params=params)() as l:                
                 if l.ok:
                     pathstr=str(temp)
                     task1 = progress.add_task(f"{(pathstr[:constants.PATH_STR_MAX] + '....') if len(pathstr) > constants.PATH_STR_MAX else pathstr}\n", total=total,visible=True)
                     progress.update(task1, advance=resume_size)
                     with open(temp, 'ab') as f:                           
                         progress.update(task1,visible=True )
                         size=0
-                        async for chunk in l.content.iter_chunked(1024):
+                        async for chunk in l.iter_chunked(1024):
                             size=size+len(chunk) if log_trace else size
                             log.trace(f"Media:{ele.id} Post:{ele.postid} Download:{size}/{total}")
                             f.write(chunk)
                             progress.update(task1, advance=len(chunk))
                         progress.remove_task(task1)
                 else:
                     l.raise_for_status()
@@ -379,51 +382,52 @@
     finally:
         sem.release()
 
 
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def key_helper(c,pssh,licence_url,id):
-    log.debug("using auto key helper")
+    log.debug(f"ID:{id} using auto key helper")
     try:
         out=cache.get(licence_url)
         log.debug(f"ID:{id} pssh: {pssh!=None}")
         log.debug(f"ID:{id} licence: {licence_url}")
-        if not out:
-            headers=auth.make_headers(auth.read_auth())
-            headers["cookie"]=auth.get_cookies()
-            auth.create_sign(licence_url,headers)
-            json_data = {
-                'license': licence_url,
-                'headers': json.dumps(headers),
-                'pssh': pssh,
-                'buildInfo': '',
-                'proxy': '',
-                'cache': True,
-            }
-
-
-            async with c.request("post",'https://cdrm-project.com/wv',json=json_data,ssl=ssl.create_default_context(cafile=certifi.where()),allow_redirects=True,cookies=None) as r:
-                httpcontent=await r.text()
-                log.debug(f"ID:{id} key_response: {httpcontent}")
-                soup = BeautifulSoup(httpcontent, 'html.parser')
-                out=soup.find("li").contents[0]
-                cache.set(licence_url,out, expire=constants.KEY_EXPIRY)
-                cache.close()
+        if out!=None:
+            log.debug(f"ID:{id} auto key helper got key from cache")
+            return out
+        headers=auth.make_headers(auth.read_auth())
+        headers["cookie"]=auth.get_cookies()
+        auth.create_sign(licence_url,headers)
+        json_data = {
+            'license': licence_url,
+            'headers': json.dumps(headers),
+            'pssh': pssh,
+            'buildInfo': '',
+            'proxy': '',
+            'cache': True,
+        }
+        async with c.requests(url='https://cdrm-project.com/wv',method="post",json=json_data)() as r:
+            httpcontent=await r.text_()
+            log.debug(f"ID:{id} key_response: {httpcontent}")
+            soup = BeautifulSoup(httpcontent, 'html.parser')
+            out=soup.find("li").contents[0]
+            cache.set(licence_url,out, expire=constants.KEY_EXPIRY)
+            cache.close()
         return out
     except Exception as E:
         log.traceback(E)
         log.traceback(traceback.format_exc())
         raise E
         
 
 async def key_helper_manual(c,pssh,licence_url,id):
-    log.debug("using manual keyhelper")
+    log.debug(f"ID:{id} using manual key helper")
     out=cache.get(licence_url)
     if out!=None:
+        log.debug(f"ID:{id} manual key helper got key from cache")
         return out
     log.debug(f"ID:{id} pssh: {pssh!=None}")
     log.debug(f"ID:{id} licence: {licence_url}")
 
     # prepare pssh
     pssh = PSSH(pssh)
 
@@ -437,23 +441,18 @@
     # load cdm
     cdm = Cdm.from_device(device)
 
     # open cdm session
     session_id = cdm.open()
 
     
-    
-    
-    # get license challenge
-    challenge = cdm.get_license_challenge(session_id, pssh)
-    headers=auth.make_headers(auth.read_auth())
-    headers=auth.create_sign(licence_url, headers)
     keys=None
-    async with c.request("post",licence_url,data=challenge,ssl=ssl.create_default_context(cafile=certifi.where()),allow_redirects=True, headers=headers,cookies=auth.add_cookies_aio()) as r:
-        cdm.parse_license(session_id, await r.content.read())
+    challenge = cdm.get_license_challenge(session_id, pssh)
+    async with c.requests(url=licence_url,method="post",data=challenge)() as r:
+        cdm.parse_license(session_id, (await r.content.read()))
         keys = cdm.get_keys(session_id)
         cdm.close(session_id)
     keyobject=list(filter(lambda x:x.type=="CONTENT",keys))[0]
     key="{}:{}".format(keyobject.kid.hex,keyobject.key.hex())
     cache.set(licence_url,key, expire=constants.KEY_EXPIRY)
     return key
 
@@ -488,7 +487,23 @@
 
 def set_cache_helper(ele):
     if  ele.postid and ele.responsetype_=="profile":
         cache.set(ele.postid ,True)
         cache.close()
 
 
+def addGlobalDir(path):
+    dirSet.add(path.parent)
+
+
+def setDirectoriesDate():
+    log.info("Setting Date for modified directories")
+    output=set()
+    rootDir=pathlib.Path(config_.get_save_location(config_.read_config()))
+    for ele in dirSet:
+        output.add(ele)
+        while ele!=rootDir and ele.parent!=rootDir:
+            output.add(ele.parent)
+            ele=ele.parent
+    log.debug(f"Directories list {rootDir}")
+    for ele in output:
+        set_time(ele,dates.get_current_time())
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/encoding.py` & `ofscraper-2.7.2/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/exit.py` & `ofscraper-2.7.2/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/filters.py` & `ofscraper-2.7.2/ofscraper/utils/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 import arrow
 import ofscraper.utils.config as config
 import ofscraper.utils.args as args_
 
 args=args_.getargs()
 log=logging.getLogger(__package__)
 def filterMedia(media):
-    logformater="data: {} id: {} postid: {}"
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 1-> all media no filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    logformater="{} data: {} id: {} postid: {}"
+    []
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 1-> all media no filter:",x.media,x.id,x.postid),media))))
     log.debug(f"filter 1-> all media no filter count: {len(media)}")
     media=dupefilter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f" filter 2-> all media dupe filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 2-> all media dupe filter: ",x.media,x.id,x.postid),media))))
+
     log.debug(f"filter 2-> all media dupe filter count: {len(media)}")
     media=post_datesorter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 3-> all media datesort: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 3-> all media datesort: ",x.media,x.id,x.postid),media))))
     log.debug(f"filter 3-> all media datesort count: {len(media)}")
     media=posts_type_filter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 4-> all media post media type filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 4-> all media post media type filter: ",x.media,x.id,x.postid),media))))
+
     log.debug(f"filter 4-> all media post media type filter count: {len(media)}")
     media=posts_date_filter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 5-> all media post date filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 5-> all media post date filter: ",x.media,x.id,x.postid),media))))
     log.debug(f"filter 5-> all media post date filter: {len(media)}")
-
     media=post_timed_filter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 6->  all media post timed post filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 6->  all media post timed post filter: ",x.media,x.id,x.postid),media))))
     log.debug(f"filter 6->  all media post timed post filter count: {len(media)}")
     media=post_user_filter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 7-> all media post text filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 7-> all media post text filter: ",x.media,x.id,x.postid),media))))
     log.debug(f"filter 7->  all media post text filter count: {len(media)}")
     media=download_type_filter(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 8->  all download type filter: {logformater.format(x.media,x.id,x.postid)}",media)))))
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 8->  all download type filter: ",x.media,x.id,x.postid),media))))
     log.debug(f"filter 8->  all download type filter count: {len(media)}")
     media=sort_media(media)
-    log.trace("{posts}".format(posts=  "\n\n".join(list(map(lambda x:f"filter 9-> final media  from retrived post: {logformater.format(x.media,x.id,x.postid)}",media)))))
-    log.debug(f"filter 0->  final media count from retrived post: {len(media)}")
+    log.trace("\n\n\n".join(list(map(lambda x: logformater.format("filter 9-> final media  from retrived post: ",x.media,x.id,x.postid),media))))
+    log.debug(f"filter 9->  final media count from retrived post: {len(media)}")
     return media
 
 def sort_media(media):
     return sorted(media,key=lambda x:x.date)
 
 def post_manual_filter():
     None
@@ -101,14 +103,23 @@
 def post_user_filter(media):
     userfilter=args.filter
     if not userfilter.islower():
         return list(filter(lambda x:re.search(userfilter,x.text or "")!=None,media))
     else:
         return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)!=None,media))
 
+def anti_post_user_filter(media):
+    userfilter=args.neg_filter
+    if not userfilter.islower():
+        return list(filter(lambda x:re.search(userfilter,x.text or "")==None,media)) if userfilter else media
+    else:
+        return list(filter(lambda x:re.search(userfilter,x.text or "",re.IGNORECASE)==None,media)) if userfilter else media
+
+
+
 def download_type_filter(media):
     if args_.getargs().download_type==None:
         return media
     elif args_.getargs().download_type=="protected":
         return list(filter(lambda x:x.mpd!=None,media))  
     elif args_.getargs().download_type=="normal":
         return list(filter(lambda x:x.url!=None,media))
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/logger.py` & `ofscraper-2.7.2/ofscraper/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 import re
-import httpx
 import logging
 import threading
 import time
 import queue
 from rich.logging import RichHandler
 
 from tenacity import retry,stop_after_attempt,wait_fixed
 
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
 import ofscraper.utils.console as console
 import ofscraper.constants as constants
+import ofscraper.classes.sessionbuilder as sessionbuilder
 senstiveDict={}
 discord_queue=queue.Queue()
 
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
 
@@ -68,38 +68,38 @@
         return self._widget
     @widget.setter
     def widget(self,widget):
         self._widget=widget
 
 
 def discord_messenger():
-    with httpx.Client() as c:
+    with sessionbuilder.sessionBuilder(backend="httpx",set_header=False,set_cookies=False,set_sign=False) as c:
         while True:
             url,message=discord_queue.get()   
             if url=="exit":
                 return
             try:
                 discord_pusher(url,message,c)
-            except httpx.HTTPError as E:
+            except Exception as E:
                 console.shared_console.print("Discord Error")
 
 @retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(constants.DISCORDWAIT),reraise=True) 
 def discord_pusher(url,message,c):
-    c.post(url, headers={"Content-type": "application/json"},json={"content":message})
+    with c.requests(url,"post",headers={"Content-type": "application/json"},json={"content":message})() as r:
+        None
 
 
 
 def discord_cleanup():
     logging.getLogger("ofscraper").info("Pushing Discord Queue")
-    with httpx.Client() as c:
-        while True:
-            if discord_queue.empty:
-                discord_queue.put(("exit",None))
-                break
-            time.sleep(.5)
+    while True:
+        if discord_queue.empty:
+            discord_queue.put(("exit",None))
+            break
+        time.sleep(.5)
              
 def start_discord_queue():
     worker_thread = threading.Thread(target=discord_messenger)
     worker_thread.start()
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/of.py` & `ofscraper-2.7.2/ofscraper/utils/of.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         
 
 
 
 
 
 
-def process_timeline_posts(model_id,username):
+def process_timeline_posts(model_id,username,individual=False):
     with stdout.lowstdout():
-        timeline_posts = asyncio.run(timeline.get_timeline_post( model_id))
+        timeline_posts = asyncio.run(timeline.get_timeline_post( model_id)) if not individual else timeline.get_individual_post(id)
         timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
         log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}")
         log.debug("Removing locked timeline media")
         for post in timeline_posts:
             operations.write_post_table(post,model_id,username)
         output=[]
         [output.extend(post.media) for post in  timeline_posts ]
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/paths.py` & `ofscraper-2.7.2/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/profiles.py` & `ofscraper-2.7.2/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/separate.py` & `ofscraper-2.7.2/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/stdout.py` & `ofscraper-2.7.2/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.1/ofscraper/utils/table.py` & `ofscraper-2.7.2/ofscraper/classes/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 
 
 
 
 
-console=console_.shared_console
+# console=console_.shared_console
 class OutConsole(TextLog):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
 class StyledButton(Button):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
@@ -66,15 +66,15 @@
 
 class NumField(Horizontal):
     def __init__(self, name: str) -> None:
         super().__init__(id=name)
         self.filter_name = name
 
     def compose(self):
-        yield self.IntegerInput(placeholder=self.filter_name.capitalize(), id=f"{self.filter_name}_search")
+        yield self.IntegerInput(placeholder=self.filter_name.capitalize().replace("_"," "), id=f"{self.filter_name}_search")
 
     def on_mount(self):
         self.styles.height = "auto"
         self.styles.width = "1fr"
 
     def empty(self):
         return self.query_one(self.IntegerInput).value == ""
@@ -433,17 +433,17 @@
             return ""
         return match.group(0)
 
 class InputApp(App):
 
     # Events
     def on_data_table_header_selected(self, event):
-        added= self.get_current_added_rows()
+        self._current_added= self.get_current_added_rows()
         self.sort_helper(event.label.plain)
-        self.restore_added_rows(added)
+        self.restore_added_rows()
       
         # set reverse
         # use native python sorting until textual has key support
 
     def on_data_table_cell_selected(self, event):
         table = self.query_one(DataTable) 
         cursor_coordinate = table.cursor_coordinate
@@ -456,19 +456,19 @@
         # use native python sorting until textual has key support
 
 
 
    
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "submit":
-            added=self.get_current_added_rows()
+            self._current_added=self.get_current_added_rows()
             self.set_filtered_rows()
             self.sort_helper()
             self.make_table()
-            self.restore_added_rows(added)
+            self.restore_added_rows()
         elif event.button.id == "reset":
             self.set_filtered_rows(reset=True)
             self.reset_all_inputs()
             self.set_reverse(init=True)
             self.make_table()
         elif event.button.id=="send_downloads":
             log.info("Adding Downloads to queue")
@@ -490,19 +490,19 @@
                 self,
                 table.get_cell_at(cursor_coordinate),
                 coordinate=cursor_coordinate,
                 cell_key=cell_key,
             )
             row_name = self.row_names[event.coordinate[1]]
             if row_name!="Download_Cart":
-                added=self.get_current_added_rows()
+                self._current_added=self.get_current_added_rows()
                 self.update_input(row_name, event.value.plain)
                 self.set_filtered_rows()
                 self.make_table()
-                self.restore_added_rows(added)
+                self.restore_added_rows()
             else:
                 self.change_download_cart(event.coordinate)
     #Main
     def compose(self) -> ComposeResult:
         with Horizontal(id="buttons"):  
             yield Button("DataTable", id="table")  
             yield Button("Console", id="console")
@@ -546,16 +546,14 @@
         self.query_one(VerticalScroll).styles.height = "25vh"
         self.query_one(VerticalScroll).styles.dock = "top"
         self.query_one(DataTable).styles.height = "60vh"
         self.query_one("#send_downloads").styles.content_align=("right", "middle")
         for ele in self.query(Horizontal)[:-1]:
             ele.styles.height = "10vh"
         logger.add_widget(self.query_one("#console_page").query_one(OutConsole))
-       
-
 
     # Cart
     def change_download_cart(self,coord):
         table=self.query_one(DataTable)
         Download_Cart=table.get_row_at(coord[0])[ self.row_names.index("Download_Cart")]
         if Download_Cart.plain=="Not Unlocked":
             return
@@ -579,18 +577,18 @@
         [self.row_queue.put(ele) for ele in map(lambda x:(table.get_row(x),x),filter_keys)]
     def get_current_added_rows(self):
         table=self.query_one(DataTable)
         keys=[str(ele[0]) for ele in self._filtered_rows]
         index=self.row_names.index("Download_Cart")
         filter_keys=list(filter(lambda x:table.get_row(x)[index].plain=="[added]",keys))
         return filter_keys
-    def restore_added_rows(self,added):
+    def restore_added_rows(self):
         table=self.query_one(DataTable)
         currentkeys=set(map(lambda x:x.value,table.rows.keys()))
-        [table.update_cell(key,"Download_Cart",Text("[added]")) for key in filter(lambda x:x in currentkeys,added)]
+        [table.update_cell(key,"Download_Cart",Text("[added]")) for key in filter(lambda x:x in currentkeys,self._current_added)]
 
 
     def reset_cart(self):
         index=self.row_names.index("Download_Cart")
         self.update_downloadcart_cell(  [str(x[0]) for x in list(filter(lambda x:x[index]=="[added]",self.table_data[1:]))],"[]")
     
     def reset_filtered_cart(self):
@@ -640,90 +638,93 @@
 
     # Table Functions
 
     def sort_helper(self, label=None):
         # to allow sorting after submit
         if label == None:
             return
-        index=self.row_names.index(re.sub(" ","_",label))
-        if label=="Download Cart":
+        
+        elif label=="Download Cart":
+            index=self.row_names.index(re.sub(" ","_",label))
             filtered_status=["[downloading]","Not Unlocked","[downloaded]"]
             table=self.query_one(DataTable)
             self.set_cart_toggle()
             keys=[str(ele[0]) for ele in self._filtered_rows]
             filter_keys=list(filter(lambda x:table.get_row(x)[index].plain not in filtered_status,keys))
+            log.debug(f"set cart toggle to {self.cart_toggle.plain}")
             [table.update_cell(key,"Download_Cart",self.cart_toggle) for key in filter_keys]
-            
 
-           
-           
-            return
-        self.set_reverse(label=label)
-        
-        if label == "Number":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
-            self.make_table()
-        elif label == "UserName":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
-            self.make_table()
-        elif label == "Downloaded":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
-            self.make_table()
+            # [table.update_cell(key,"Download_Cart",self.cart_toggle) for key in filter_keys]
+                    
+        elif label!="Download Cart":
+            index=self.row_names.index(re.sub(" ","_",label))
 
-        elif label == "Unlocked":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
-            self.make_table()
-        elif label == "Times Detected":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
-            self.make_table()
-        elif label == "Length":
-            helperNode = self.query_one("#Length")
-            self._filtered_rows = sorted(self._filtered_rows, key=lambda x: helperNode.convertString(
-                x[index]) if x[index] != "N/A" else 0, reverse=self.reverse)
-            self.make_table()
-        elif label == "Mediatype":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index] , reverse=self.reverse)
-            self.make_table()
-        elif label == "Post Date":
-            helperNode = self.query_one("#Post_Date")
-            self._filtered_rows = sorted(self._filtered_rows, key=lambda x: helperNode.convertString(
-                x[index]) if x[index] != "N/A" else 0, reverse=self.reverse)
-            self.make_table()
-        elif label == "Post Media Count":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
-            self.make_table()
+            self.set_reverse(label=label)
+            
+            if label == "Number":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
+                self.make_table()
+            elif label == "UserName":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
+                self.make_table()
+            elif label == "Downloaded":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
+                self.make_table()
 
-        elif label == "Responsetype":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
-            self.make_table()
-        elif label == "Price":
-            self._filtered_rows = sorted(self._filtered_rows, key=lambda x: int(
-                float(x[index])) if x[index] != "Free" else 0, reverse=self.reverse)
-            self.make_table()
+            elif label == "Unlocked":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
+                self.make_table()
+            elif label == "Times Detected":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: 1 if x[index] == True else 0, reverse=self.reverse)
+                self.make_table()
+            elif label == "Length":
+                helperNode = self.query_one("#Length")
+                self._filtered_rows = sorted(self._filtered_rows, key=lambda x: helperNode.convertString(
+                    x[index]) if x[index] != "N/A" else 0, reverse=self.reverse)
+                self.make_table()
+            elif label == "Mediatype":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index] , reverse=self.reverse)
+                self.make_table()
+            elif label == "Post Date":
+                helperNode = self.query_one("#Post_Date")
+                self._filtered_rows = sorted(self._filtered_rows, key=lambda x: helperNode.convertString(
+                    x[index]) if x[index] != "N/A" else 0, reverse=self.reverse)
+                self.make_table()
+            elif label == "Post Media Count":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
+                self.make_table()
 
-        elif label == "Post ID":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index] if  x[index] else 0, reverse=self.reverse)
-            self.make_table()
-        elif label == "Media ID":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index] if  x[index] else 0, reverse=self.reverse)
-            self.make_table()
-        elif label == "Text":
-            self._filtered_rows = sorted(
-                self._filtered_rows, key=lambda x: x[index] , reverse=self.reverse)
-            self.make_table()
+            elif label == "Responsetype":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index], reverse=self.reverse)
+                self.make_table()
+            elif label == "Price":
+                self._filtered_rows = sorted(self._filtered_rows, key=lambda x: int(
+                    float(x[index])) if x[index] != "Free" else 0, reverse=self.reverse)
+                self.make_table()
+
+            elif label == "Post ID":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index] if  x[index] else 0, reverse=self.reverse)
+                self.make_table()
+            elif label == "Media ID":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index] if  x[index] else 0, reverse=self.reverse)
+                self.make_table()
+            elif label == "Text":
+                self._filtered_rows = sorted(
+                    self._filtered_rows, key=lambda x: x[index] , reverse=self.reverse)
+                self.make_table()
 
     def set_reverse(self, label=None, init=False):
         if init:
             self.reverse = None
             self.label = None
         if not self.label:
             self.label = label
@@ -736,16 +737,17 @@
             self.reverse = True
 
         elif self.label == label and self.reverse:
             self.reverse = False
 
     def set_cart_toggle(self,init=False):
         if init:
-            self.cart_toggle = Text("[added]")
-        if self.cart_toggle.plain == "[added]":
+            self.cart_toggle = Text("[]")
+        elif self.cart_toggle.plain == "[added]":
+            self._current_added=[]
             self.cart_toggle = Text("[]")
         elif self.cart_toggle.plain == "[]":
             self.cart_toggle = Text("[added]")
 
     def set_filtered_rows(self, reset=False):
         if reset == True:
             self._filtered_rows = self.table_data[1:]
```

### Comparing `ofscraper-2.7.1/ofscraper/utils/userselector.py` & `ofscraper-2.7.2/ofscraper/utils/userselector.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     usernameset=set(args.username)
     return list(filter(lambda x:x["name"] in usernameset,parsed_subscriptions)) if "ALL" not in args.username else parsed_subscriptions
     
 def selectuserhelper(): 
     headers = auth.make_headers(auth.read_auth())
     subscribe_count = process_me(headers)
     global parsed_subscriptions
-    all_subs = get_models(headers, subscribe_count)
+    all_subs = get_models( subscribe_count)
     if not args.username: 
         selected=None
         while True:
             parsed_subscriptions=filterNSort( all_subs )
             selectedusers,p= get_model(parsed_subscriptions ,selected)
             if len(selectedusers)!=0:
                 args.username=selectedusers
@@ -132,27 +132,27 @@
         return sorted(models,reverse=reverse, key=lambda x:x.get("price") or 0)
     else:
         return sorted(models,reverse=reverse, key=lambda x:x["name"])
 #check if auth is valid
 def process_me(headers):
     my_profile = me.scrape_user(headers)
     name, username = me.parse_user(my_profile)
-    subscribe_count=me.parse_subscriber_count(headers)
+    subscribe_count=me.parse_subscriber_count()
     me.print_user(name, username)
     return subscribe_count
 
-def get_models(headers, subscribe_count) -> list:
+def get_models(subscribe_count) -> list:
     """
     Get user's subscriptions in form of a list.
     """
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
             task1=progress.add_task('Getting your subscriptions (this may take awhile)...')
             list_subscriptions = asyncio.run(
-                subscriptions.get_subscriptions(headers, subscribe_count))
+                subscriptions.get_subscriptions(subscribe_count))
             parsed_subscriptions = subscriptions.parse_subscriptions(
                 list_subscriptions)
             progress.remove_task(task1)
             return parsed_subscriptions
 
 
 def get_model(parsed_subscriptions: list,selected) -> tuple:
```

### Comparing `ofscraper-2.7.1/pyproject.toml` & `ofscraper-2.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.7.1"
+version = "2.7.2"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.7.1/PKG-INFO` & `ofscraper-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.7.1
+Version: 2.7.2
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -78,16 +78,15 @@
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
-
-https://discord.gg/wN7uxEVHRK
+https://discord.gg/DV3aBeMu
     
 # Feature Requests
 
 https://ofscraper.clearflask.com/feedback
     
 Or the discord
```

