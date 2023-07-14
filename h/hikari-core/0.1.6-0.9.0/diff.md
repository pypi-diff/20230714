# Comparing `tmp/hikari_core-0.1.6.tar.gz` & `tmp/hikari_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.1.6.tar", max compression
+gzip compressed data, was "hikari_core-0.9.0.tar", max compression
```

## Comparing `hikari_core-0.1.6.tar` & `hikari_core-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,49 @@
--rw-r--r--   0        0        0     4536 2023-05-22 02:25:09.664141 hikari_core-0.1.6/hikari_core/__init__.py
--rw-r--r--   0        0        0     6087 2023-06-06 15:48:21.901621 hikari_core-0.1.6/hikari_core/analyze.py
--rw-r--r--   0        0        0     3364 2023-05-17 07:49:16.245089 hikari_core-0.1.6/hikari_core/command_select.py
--rw-r--r--   0        0        0     1468 2023-05-14 15:19:46.161065 hikari_core-0.1.6/hikari_core/config.py
--rw-r--r--   0        0        0    10743 2023-06-06 17:17:33.374770 hikari_core-0.1.6/hikari_core/data_source.py
--rw-r--r--   0        0        0      743 2023-05-14 15:19:45.721315 hikari_core-0.1.6/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2942 2023-05-14 15:19:45.722347 hikari_core-0.1.6/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5462 2023-05-14 15:19:45.723349 hikari_core-0.1.6/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.1.6/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.1.6/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.1.6/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.1.6/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.1.6/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     1968 2023-05-30 20:07:21.287212 hikari_core-0.1.6/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3138 2023-06-06 15:31:07.314957 hikari_core-0.1.6/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.1.6/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    10479 2023-05-16 16:11:32.118354 hikari_core-0.1.6/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0     2392 2023-05-30 20:07:21.289754 hikari_core-0.1.6/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     3190 2023-06-06 16:41:39.549334 hikari_core-0.1.6/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     3874 2023-05-30 20:07:21.290780 hikari_core-0.1.6/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     3792 2023-05-17 07:49:16.247099 hikari_core-0.1.6/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0   173084 2023-05-15 12:36:37.138233 hikari_core-0.1.6/hikari_core/Template/Chart.min.js
--rw-r--r--   0        0        0    13286 2023-05-15 12:36:39.500206 hikari_core-0.1.6/hikari_core/Template/chartjs-plugin-datalabels@1.0.0.js
--rw-r--r--   0        0        0     3780 2023-05-16 16:11:32.110791 hikari_core-0.1.6/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5135 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      225 2023-05-15 12:30:50.607350 hikari_core-0.1.6/hikari_core/Template/text-help.css
--rw-r--r--   0        0        0     7310 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16783 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-05-15 12:30:50.643703 hikari_core-0.1.6/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    25696 2023-06-06 17:10:27.683820 hikari_core-0.1.6/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    24942 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-05-15 12:30:50.750146 hikari_core-0.1.6/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21684 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    20793 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9472 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5810 2023-06-02 14:21:25.824545 hikari_core-0.1.6/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4393 2023-05-16 11:20:41.711193 hikari_core-0.1.6/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.1.6/LICENSE
--rw-r--r--   0        0        0      549 2023-06-06 17:17:25.235690 hikari_core-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.1.6/README.md
--rw-r--r--   0        0        0    11430 1970-01-01 00:00:00.000000 hikari_core-0.1.6/setup.py
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 hikari_core-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5066 2023-07-14 18:13:45.076853 hikari_core-0.9.0/hikari_core/__init__.py
+-rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3498 2023-07-13 10:46:01.317795 hikari_core-0.9.0/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1506 2023-06-09 16:02:41.277675 hikari_core-0.9.0/hikari_core/config.py
+-rw-r--r--   0        0        0    10720 2023-07-14 18:21:52.431027 hikari_core-0.9.0/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2598 2023-07-07 08:04:40.589860 hikari_core-0.9.0/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2324 2023-07-07 09:04:55.774201 hikari_core-0.9.0/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     3659 2023-07-14 08:41:52.994916 hikari_core-0.9.0/hikari_core/game/help.py
+-rw-r--r--   0        0        0     2122 2023-07-10 07:31:07.868469 hikari_core-0.9.0/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2311 2023-07-07 08:58:39.067755 hikari_core-0.9.0/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3152 2023-07-13 08:56:17.527001 hikari_core-0.9.0/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11581 2023-07-14 08:31:13.584765 hikari_core-0.9.0/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10567 2023-07-13 09:41:24.730553 hikari_core-0.9.0/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     2726 2023-07-13 06:28:59.408115 hikari_core-0.9.0/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     3553 2023-07-13 06:29:52.468436 hikari_core-0.9.0/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     4085 2023-07-13 08:58:03.235425 hikari_core-0.9.0/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3998 2023-07-13 08:58:08.113156 hikari_core-0.9.0/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6867 2023-07-13 08:58:13.299011 hikari_core-0.9.0/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2023-07-14 12:03:50.576415 hikari_core-0.9.0/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     3783 2023-07-14 12:03:51.005556 hikari_core-0.9.0/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5166 2023-07-14 12:03:51.031428 hikari_core-0.9.0/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2023-07-14 12:03:51.047079 hikari_core-0.9.0/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7310 2023-07-14 12:03:51.076856 hikari_core-0.9.0/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-07-14 12:03:51.120915 hikari_core-0.9.0/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-07-14 12:03:51.167932 hikari_core-0.9.0/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28156 2023-07-14 13:10:22.607915 hikari_core-0.9.0/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    28082 2023-07-14 13:16:23.660810 hikari_core-0.9.0/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-07-14 12:03:51.349020 hikari_core-0.9.0/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-07-14 12:03:51.375787 hikari_core-0.9.0/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21441 2023-07-14 13:18:45.676515 hikari_core-0.9.0/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-07-14 12:03:51.448109 hikari_core-0.9.0/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-07-14 12:03:51.476400 hikari_core-0.9.0/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4393 2023-06-09 16:04:19.214393 hikari_core-0.9.0/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-07-14 18:20:28.281571 hikari_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0/README.md
+-rw-r--r--   0        0        0     9938 1970-01-01 00:00:00.000000 hikari_core-0.9.0/setup.py
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 hikari_core-0.9.0/PKG-INFO
```

### Comparing `hikari_core-0.1.6/hikari_core/__init__.py` & `hikari_core-0.9.0/hikari_core/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-# fmt: off
-import os
 import time
 import traceback
 
 import jinja2
 from apscheduler.schedulers.background import BackgroundScheduler
 from loguru import logger
 from pydantic import ValidationError
 
 from .analyze import analyze_command
-from .config import hikari_config, set_hikari_config
+from .config import hikari_config, set_hikari_config  # noqa:F401
 from .data_source import set_render_params, template_path
+from .game.help import update_template
 from .Html_Render import html_to_pic
 from .model import Hikari_Model, Input_Model, UserInfo_Model
-from .utils import startup
-
-# fmt: on
 
 env = jinja2.Environment(loader=jinja2.FileSystemLoader(template_path), enable_async=True)
 env.globals.update(
     time=time,
     abs=abs,
     enumerate=enumerate,
     int=int,
@@ -42,99 +38,109 @@
         Hikari_Model: 可通过Hikari.Status和Hikari.Output.Data内数据判断是否输出
     """
     try:
         userinfo = UserInfo_Model(Platform=platform, PlatformId=PlatformId)
         input = Input_Model(Command_Text=command_text)
         hikari = Hikari_Model(UserInfo=userinfo, Input=input)
         hikari = await analyze_command(hikari)
-        if not hikari.Status == "init" or not hikari.Function:
+        if not hikari.Status == 'init' or not hikari.Function:
             return hikari
         hikari: Hikari_Model = await hikari.Function(hikari)
         return await output_hikari(hikari)
     except ValidationError:
         logger.error(traceback.format_exc())
-        return Hikari_Model().error("参数校验错误，请联系开发者确认入参是否符合Model")
+        return Hikari_Model().error('参数校验错误，请联系开发者确认入参是否符合Model')
     except Exception:
         logger.error(traceback.format_exc())
-        return Hikari_Model().error("Hikari-core顶层错误，请检查log")
+        return Hikari_Model().error('Hikari-core顶层错误，请检查log')
 
 
 async def callback_hikari(hikari: Hikari_Model) -> Hikari_Model:
     """回调wait状态的Hikari
 
     Args:
         hikari (Hikari_Model):前置或自行构造的Hikari_Model，可通过from hikari_core import Hikari_Model引入
 
     Returns:
         Hikari_Model: 可通过Hikari.Status和Hikari.Output.Data内数据判断是否输出
     """
     try:
-        if not hikari.Status == "wait":
-            return hikari.error("当前请求状态错误，请确认是否为wait")
+        if not hikari.Status == 'wait':
+            return hikari.error('当前请求状态错误，请确认是否为wait')
         if not hikari.Function:
-            return hikari.error("缺少请求方法")
+            return hikari.error('缺少请求方法')
         hikari: Hikari_Model = await hikari.Function(hikari)
         return await output_hikari(hikari)
 
     except Exception:
         logger.error(traceback.format_exc())
-        return Hikari_Model().error("Hikari-core顶层错误，请检查log")
+        return Hikari_Model().error('Hikari-core顶层错误，请检查log')
 
 
 async def output_hikari(hikari: Hikari_Model) -> Hikari_Model:
     """输出Hikari
 
     Args:
         hikari (Hikari_Model):前置或自行构造的Hikari_Model，可通过from hikari_core import Hikari_Model引入
 
     Returns:
         Hikari_Model: 可通过Hikari.Status和Hikari.Output.Data内数据判断是否输出
     """
     try:
-        if hikari.Status in ["success", "wait"] and hikari_config.auto_rendering:
+        if (
+            hikari.Status in ['success', 'wait']
+            and hikari_config.auto_rendering
+            and hikari.Output.Template
+            and (isinstance(hikari.Output.Data, dict) or isinstance(hikari.Output.Data, list))  # noqa: PLR1701
+        ):
             template = env.get_template(hikari.Output.Template)
-            template_data = await set_render_params(hikari.Output.Data)
+            if hikari.Status == 'success':
+                template_data = await set_render_params(hikari.Output.Data)
+            elif hikari.Status == 'wait':
+                template_data = await set_render_params(hikari.Input.Select_Data)
             content = await template.render_async(template_data)
             hikari.Output.Data = content
+            hikari.Output.Data_Type = type(hikari.Output.Data)
 
             if hikari_config.auto_image:
                 hikari.Output.Data = await html_to_pic(
                     content,
                     wait=0,
-                    viewport={"width": hikari.Output.Width, "height": hikari.Output.Height},
+                    viewport={'width': hikari.Output.Width, 'height': hikari.Output.Height},
                     use_browser=hikari_config.use_broswer,
                 )
+                hikari.Output.Data_Type = type(hikari.Output.Data)
         return hikari
     except Exception:
         logger.error(traceback.format_exc())
-        return Hikari_Model().error("Hikari-core顶层错误，请检查log")
+        return Hikari_Model().error('Hikari-core顶层错误，请检查log')
 
 
-# startup()
-# scheduler = BackgroundScheduler(timezone="Asia/Shanghai")
-# scheduler.add_job(startup, 'cron', hour=4)
-# scheduler.start()
-
-logger.add(
-    "hikari-core-logs/error.log",
-    rotation="00:00",
-    retention="1 week",
-    diagnose=False,
-    level="ERROR",
-    encoding="utf-8",
-)
-logger.add(
-    "hikari-core-logs/info.log",
-    rotation="00:00",
-    retention="1 week",
-    diagnose=False,
-    level="INFO",
-    encoding="utf-8",
-)
-logger.add(
-    "hikari-core-logs/warning.log",
-    rotation="00:00",
-    retention="1 week",
-    diagnose=False,
-    level="WARNING",
-    encoding="utf-8",
-)
+update_template()
+scheduler = BackgroundScheduler(timezone='Asia/Shanghai')
+scheduler.add_job(update_template, 'cron', hour='4,12')
+scheduler.start()
+
+# logger.add(
+#    'hikari-core-logs/error.log',
+#    rotation='00:00',
+#    retention='1 week',
+#    diagnose=False,
+#    level='ERROR',
+#    encoding='utf-8',
+# )
+# logger.add(
+#    'hikari-core-logs/info.log',
+#    rotation='00:00',
+#    retention='1 week',
+#    diagnose=False,
+#    level='INFO',
+#    encoding='utf-8',
+# )
+# logger.add(
+#    'hikari-core-logs/warning.log',
+#    rotation='00:00',
+#    retention='1 week',
+#    diagnose=False,
+#    level='WARNING',
+#    encoding='utf-8',
+# )
```

### Comparing `hikari_core-0.1.6/hikari_core/command_select.py` & `hikari_core-0.9.0/hikari_core/command_select.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# fmt: off
 from dataclasses import dataclass
 from typing import List, Protocol, Tuple, runtime_checkable
 
-# from .game.ban_search import get_BanInfo
-# from .game.box_check import check_christmas_box
+from .game.ban_search import get_BanInfo
+from .game.box_check import check_christmas_box
+from .game.help import check_version, get_help, update_template
+
 # from .game.ocr import get_Random_Ocr_Pic
-# from .game.roll import roll_ship
-# from .game.sx import get_sx_info
-# from .moudle.publicAPI import get_ship_name
-# from .moudle.wws_bind import (change_BindInfo, delete_BindInfo, get_BindInfo,
-#                              set_BindInfo, set_special_BindInfo)
+from .game.roll import roll_ship
+from .game.sx import get_sx_info
+from .moudle.publicAPI import get_ship_name
+from .moudle.wws_bind import change_BindInfo, delete_BindInfo, get_BindInfo, set_BindInfo, set_special_BindInfo
+
 # from .moudle.wws_clan import get_ClanInfo
 from .moudle.wws_info import get_AccountInfo
 from .moudle.wws_recent import get_RecentInfo
+
 # from .moudle.wws_record import get_record
 from .moudle.wws_ship_info import get_ShipInfo
 from .moudle.wws_ship_recent import get_ShipRecent
-
-# from .moudle.wws_shiprank import get_ShipRank
-# fmt: on
+from .moudle.wws_shiprank import get_ShipRank
 
 
 @runtime_checkable
 class Func(Protocol):
     async def __call__(self, **kwargs):
         ...
 
@@ -31,48 +31,51 @@
 class command:
     keywords: Tuple[str, ...]
     func: Func
     default_func: Func = None
 
 
 first_command_list = [  # 同指令中越长的匹配词越靠前
-    # command(("切换绑定", "更换绑定", "更改绑定"), change_BindInfo),
-    # command(("查询绑定", "绑定查询", "绑定列表", "查绑定"), get_BindInfo),
-    # command(("删除绑定",), delete_BindInfo),
-    # command(("特殊绑定",), set_special_BindInfo),
-    # command(("ship.rank", "rank"), get_ShipRank),
-    # command(("bind", "绑定", "set"), set_BindInfo),
-    command(("recent", "近期"), None, get_RecentInfo),
-    command(("ship", "单船"), None, get_ShipInfo),
+    command(('切换绑定', '更换绑定', '更改绑定'), change_BindInfo),
+    command(('查询绑定', '绑定查询', '绑定列表', '查绑定'), get_BindInfo),
+    command(('删除绑定',), delete_BindInfo),
+    command(('特殊绑定',), set_special_BindInfo),
+    command(('ship.rank', 'rank'), get_ShipRank),
+    command(('bind', '绑定', 'set'), set_BindInfo),
+    command(('recent', '近期'), None, get_RecentInfo),
+    command(('ship', '单船'), None, get_ShipInfo),
     # command(("record", "历史记录"), None, get_record),
     # command(("clan", "军团", "公会", "工会"), None, get_ClanInfo),
     # command(("随机表情包",), get_Random_Ocr_Pic),
-    # command(("roll", "随机"), roll_ship),
-    # command(("sx", "扫雪"), get_sx_info),
-    # command(("ban","封号记录"),get_BanInfo),
-    # command(("box", "sd", "圣诞船池"), check_christmas_box),
-    # command(("搜船名", "查船名", "船名"), get_ship_name),
+    command(('roll', '随机'), roll_ship),
+    command(('sx', '扫雪'), get_sx_info),
+    command(('ban', '封号记录'), get_BanInfo),
+    command(('box', 'sd', '圣诞船池'), check_christmas_box),
+    command(('搜船名', '查船名', '船名'), get_ship_name),
+    command(('help', '帮助'), get_help),
+    command(('check_version', '检查更新'), check_version),
+    command(('更新样式',), update_template),
 ]
 
 second_command_list = [
-    command(("recent", "近期"), get_ShipRecent),
-    command(("ship", "单船"), get_ShipRecent),
+    command(('recent', '近期'), get_ShipRecent),
+    command(('ship', '单船'), get_ShipRecent),
     # command(("clan", "军团", "公会", "工会"), get_record),
     # command(("record", "历史记录"), get_record),
 ]
 
 
 async def findFunction_and_replaceKeywords(match_list, command_List, default_func) -> Tuple[command, List]:
     for com in command_List:
         for kw in com.keywords:
             for i, match_kw in enumerate(match_list):
                 if match_kw.find(kw) + 1:
-                    match_list[i] = str(match_kw).replace(kw, "")
-                    if match_list[i] == "":  # 为空时才删除，防止未加空格没有被split切割
-                        match_list.remove("")
+                    match_list[i] = str(match_kw).replace(kw, '')
+                    if not match_list[i]:  # 为空时才删除，防止未加空格没有被split切割
+                        match_list.remove('')
                     return com, match_list
     return command(None, default_func, None), match_list
 
 
 async def select_command(search_list) -> Tuple[Func, List]:
     command, search_list = await findFunction_and_replaceKeywords(search_list, first_command_list, get_AccountInfo)
     if command.func is None:
```

### Comparing `hikari_core-0.1.6/hikari_core/config.py` & `hikari_core-0.9.0/hikari_core/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 from loguru import logger
 from pydantic import BaseModel
 
 
 class Config_Model(BaseModel):
     proxy: Optional[str]
     http2: bool = True
-    token: Optional[str] = "123456:111111111111"
+    token: Optional[str] = '123456:111111111111'
     auto_rendering: bool = True
     auto_image: bool = True
-    use_broswer: Optional[str] = "chromium"
+    use_broswer: Optional[str] = 'chromium'
 
 
 hikari_config = Config_Model()
 
 
-def set_hikari_config(
+def set_hikari_config(  # noqa: PLR0913
     proxy: Optional[str],
     http2: bool = True,
-    token: Optional[str] = "123456:111111111111",
+    token: Optional[str] = '123456:111111111111',
     auto_rendering: bool = True,
     auto_image: bool = True,
-    use_broswer: Optional[str] = "chromium",
+    use_broswer: Optional[str] = 'chromium',
 ):
     """配置Hikari-core
 
     Args:
         proxy (str): 访问WG使用的代理，格式http://localhost:7890
         http2 (bool): 是否开启http2，默认启用
         token (str): #请加群联系雨季获取api_key和token Q群:967546463
         auto_rendering (bool): 自动填充模板，默认启用
         auto_image (bool): 是否自动渲染，默认启用，若auto_rending未启用则该项配置无效
         use_broswer (str): chromium/firefox，默认chromium，性能大约为firefox三倍
 
     """
-    global hikari_config
+    global hikari_config  # noqa: PLW0602
     hikari_config.proxy = proxy
     hikari_config.http2 = http2
     hikari_config.token = token
-    hikari_config.auto_image = auto_rendering
+    hikari_config.auto_rendering = auto_rendering
     hikari_config.auto_image = auto_image
     hikari_config.use_broswer = use_broswer
-    logger.info(f"当前hikari-core配置\n{hikari_config}")
+    logger.info(f'当前hikari-core配置\n{hikari_config}')
```

### Comparing `hikari_core-0.1.6/hikari_core/Html_Render/__init__.py` & `hikari_core-0.9.0/hikari_core/Html_Render/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-# fmt: off
 from loguru import logger
 
-from .browser import get_browser, get_new_page, shutdown_browser
-from .data_source import (capture_element, html_to_pic, template_to_html,
-                          template_to_pic, text_to_pic)
-
-# fmt:on
+from .browser import get_browser, get_new_page, shutdown_browser  # noqa: F401
+from .data_source import capture_element, html_to_pic, template_to_html, template_to_pic, text_to_pic  # noqa: F401
 
 
 async def init(**kwargs):
     """Start Browser
 
     Returns:
         Browser: Browser
     """
     browser = await get_browser(**kwargs)
-    logger.info("Browser Started.")
+    logger.info('Browser Started.')
     return browser
 
 
 async def shutdown():
     await shutdown_browser()
-    logger.info("Browser Stopped.")
+    logger.info('Browser Stopped.')
 
 
 browser_init = init
 
 all = [
-    "browser_init",
-    "text_to_pic",
-    "get_new_page",
-    "template_to_html",
-    "template_to_pic",
-    "html_to_pic",
-    "capture_element",
+    'browser_init',
+    'text_to_pic',
+    'get_new_page',
+    'template_to_html',
+    'template_to_pic',
+    'html_to_pic',
+    'capture_element',
 ]
```

### Comparing `hikari_core-0.1.6/hikari_core/Html_Render/browser.py` & `hikari_core-0.9.0/hikari_core/Html_Render/browser.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 @Author         : yanyongyu
 @Date           : 2021-03-12 13:42:43
 @LastEditors    : yanyongyu
 @LastEditTime   : 2021-11-01 14:05:41
 @Description    : None
 @GitHub         : https://github.com/yanyongyu
 """
-__author__ = "yanyongyu"
-# fmt: off
+__author__ = 'yanyongyu'
 from contextlib import asynccontextmanager
 from typing import AsyncIterator, Optional
 
 from loguru import logger
-from playwright.async_api import (Browser, Error, Page, Playwright,
-                                  async_playwright)
+from playwright.async_api import Browser, Error, Page, Playwright, async_playwright
 
-# fmt:on
 _browser: Optional[Browser] = None
 _playwright: Optional[Playwright] = None
 
 
 async def init(use_browser, **kwargs) -> Browser:
     global _browser
     global _playwright
@@ -31,22 +28,22 @@
     except Error:
         await install_browser(use_browser)
         _browser = await launch_browser(use_browser, **kwargs)
     return _browser
 
 
 async def launch_browser(use_browser, **kwargs) -> Browser:
-    assert _playwright is not None, "Playwright 没有安装"
-    if use_browser == "firefox":
-        logger.info("使用 firefox 启动")
+    assert _playwright is not None, 'Playwright 没有安装'
+    if use_browser == 'firefox':
+        logger.info('使用 firefox 启动')
         return await _playwright.firefox.launch(**kwargs)
 
     else:
         # 默认使用 chromium
-        logger.info("使用 chromium 启动")
+        logger.info('使用 chromium 启动')
         return await _playwright.chromium.launch(**kwargs)
 
 
 async def get_browser(use_browser, **kwargs) -> Browser:
     return _browser if _browser and _browser.is_connected() else await init(use_browser, **kwargs)
 
 
@@ -73,27 +70,27 @@
 
 async def install_browser(use_browser):
     import os
     import sys
 
     from playwright.__main__ import main
 
-    logger.info("使用镜像源进行下载")
-    os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = "https://npmmirror.com/mirrors/playwright/"
+    logger.info('使用镜像源进行下载')
+    os.environ['PLAYWRIGHT_DOWNLOAD_HOST'] = 'https://npmmirror.com/mirrors/playwright/'
     success = False
 
-    if use_browser == "firefox":
-        logger.info("正在安装 firefox")
-        sys.argv = ["", "install", "firefox"]
+    if use_browser == 'firefox':
+        logger.info('正在安装 firefox')
+        sys.argv = ['', 'install', 'firefox']
     else:
         # 默认使用 chromium
-        logger.info("正在安装 chromium")
-        sys.argv = ["", "install", "chromium"]
+        logger.info('正在安装 chromium')
+        sys.argv = ['', 'install', 'chromium']
     try:
-        logger.info("正在安装依赖")
-        os.system("playwright install-deps")
+        logger.info('正在安装依赖')
+        os.system('playwright install-deps')
         main()
     except SystemExit as e:
         if e.code == 0:
             success = True
     if not success:
-        logger.error("浏览器更新失败, 请检查网络连通性")
+        logger.error('浏览器更新失败, 请检查网络连通性')
```

### Comparing `hikari_core-0.1.6/hikari_core/Html_Render/data_source.py` & `hikari_core-0.9.0/hikari_core/Html_Render/data_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 from os import getcwd
 from pathlib import Path
 from typing import Literal, Union
 
 import aiofiles
 import jinja2
-from loguru import logger
 
 from .browser import get_new_page
 
-TEMPLATES_PATH = str(Path(__file__).parent / "templates")
+TEMPLATES_PATH = str(Path(__file__).parent / 'templates')
 
 env = jinja2.Environment(
-    extensions=["jinja2.ext.loopcontrols"],
+    extensions=['jinja2.ext.loopcontrols'],
     loader=jinja2.FileSystemLoader(TEMPLATES_PATH),
     enable_async=True,
 )
 
 
 async def text_to_pic(
     text: str,
-    css_path: str = "",
+    css_path: str = '',
     width: int = 500,
-    type: Literal["jpeg", "png"] = "png",
+    type: Literal['jpeg', 'png'] = 'png',
     quality: Union[int, None] = None,
 ) -> bytes:
     """多行文本转图片
 
     Args:
         text (str): 纯文本, 可多行
         css_path (str, optional): css文件
         width (int, optional): 图片宽度，默认为 500
         type (Literal["jpeg", "png"]): 图片类型, 默认 png
         quality (int, optional): 图片质量 0-100 当为`png`时无效
 
     Returns:
         bytes: 图片, 可直接发送
     """
-    template = env.get_template("text.html")
+    template = env.get_template('text.html')
 
     return await html_to_pic(
-        template_path=f"file://{css_path if css_path else TEMPLATES_PATH}",
+        template_path=f'file://{css_path if css_path else TEMPLATES_PATH}',
         html=await template.render_async(
             text=text,
-            css=await read_file(css_path) if css_path else await read_tpl("text.css"),
+            css=await read_file(css_path) if css_path else await read_tpl('text.css'),
         ),
-        viewport={"width": width, "height": 10},
+        viewport={'width': width, 'height': 10},
         type=type,
         quality=quality,
     )
 
 
 # async def read_md(md_path: str) -> str:
 #     async with aiofiles.open(str(Path(md_path).resolve()), mode="r") as f:
 #         md = await f.read()
 #     return markdown.markdown(md)
 
 
 async def read_file(path: str) -> str:
-    async with aiofiles.open(path, mode="r") as f:
+    async with aiofiles.open(path, mode='r') as f:
         return await f.read()
 
 
 async def read_tpl(path: str) -> str:
-    return await read_file(f"{TEMPLATES_PATH}/{path}")
+    return await read_file(f'{TEMPLATES_PATH}/{path}')
 
 
 async def template_to_html(
     template_path: str,
     template_name: str,
     **kwargs,
 ) -> str:
@@ -86,21 +85,21 @@
         enable_async=True,
     )
     template = template_env.get_template(template_name)
 
     return await template.render_async(**kwargs)
 
 
-async def html_to_pic(
+async def html_to_pic(  # noqa: PLR0913
     html: str,
     wait: int = 0,
-    template_path: str = f"file://{getcwd()}",
-    type: Literal["jpeg", "png"] = "png",
+    template_path: str = f'file://{getcwd()}',  # noqa: B008
+    type: Literal['jpeg', 'png'] = 'png',
     quality: Union[int, None] = None,
-    use_browser: str = "chromium",
+    use_browser: str = 'chromium',
     **kwargs,
 ) -> bytes:
     """html转图片
 
     Args:
         html (str): html文本
         wait (int, optional): 等待时间. Defaults to 0.
@@ -109,38 +108,38 @@
         quality (int, optional): 图片质量 0-100 当为`png`时无效
         **kwargs: 传入 page 的参数
 
     Returns:
         bytes: 图片, 可直接发送
     """
     # logger.debug(f"html:\n{html}")
-    if "file:" not in template_path:
-        raise Exception("template_path 应该为 file:///path/to/template")
-    async with get_new_page(use_browser,**kwargs) as page:
+    if 'file:' not in template_path:
+        raise Exception('template_path 应该为 file:///path/to/template')
+    async with get_new_page(use_browser, **kwargs) as page:
         await page.goto(template_path)
-        await page.set_content(html, wait_until="networkidle")
+        await page.set_content(html, wait_until='networkidle')
         await page.wait_for_timeout(wait)
         img_raw = await page.screenshot(
             full_page=True,
             type=type,
             quality=quality,
         )
     return img_raw
 
 
-async def template_to_pic(
+async def template_to_pic(  # noqa: PLR0913
     template_path: str,
     template_name: str,
     templates: dict,
-    pages: dict = {
-        "viewport": {"width": 500, "height": 10},
-        "base_url": f"file://{getcwd()}",
+    pages: dict = {  # noqa: B006
+        'viewport': {'width': 500, 'height': 10},
+        'base_url': f'file://{getcwd()}',  # noqa: B008
     },
     wait: int = 0,
-    type: Literal["jpeg", "png"] = "png",
+    type: Literal['jpeg', 'png'] = 'png',
     quality: Union[int, None] = None,
 ) -> bytes:
     """使用jinja2模板引擎通过html生成图片
 
     Args:
         template_path (str): 模板路径
         template_name (str): 模板名
@@ -158,28 +157,28 @@
     template_env = jinja2.Environment(
         loader=jinja2.FileSystemLoader(template_path),
         enable_async=True,
     )
     template = template_env.get_template(template_name)
 
     return await html_to_pic(
-        template_path=f"file://{template_path}",
+        template_path=f'file://{template_path}',
         html=await template.render_async(**templates),
         wait=wait,
         type=type,
         quality=quality,
         **pages,
     )
 
 
 async def capture_element(
     url: str,
     element: str,
     timeout: float = 0,
-    type: Literal["jpeg", "png"] = "png",
+    type: Literal['jpeg', 'png'] = 'png',
     quality: Union[int, None] = None,
     **kwargs,
 ) -> bytes:
     async with get_new_page(**kwargs) as page:
         await page.goto(url, timeout=timeout)
         img_raw = await page.locator(element).screenshot(
             type=type,
```

### Comparing `hikari_core-0.1.6/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.9.0/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.9.0/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.9.0/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/HttpClient_Pool.py` & `hikari_core-0.9.0/hikari_core/HttpClient_Pool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,93 @@
-from typing import Optional
-
 import httpx
 from httpx import AsyncClient, Request, Response
 from loguru import logger
 
 from .config import hikari_config
 from .data_source import __version__
 
 
 async def before_request(request: Request):
-    logger.info(f"{request.method} {request.url}")
+    logger.info(f'{request.method} {request.url}')
 
 
 async def after_response(response: Response):
-    logger.info(f"本次响应的状态码:{response.status_code} {response.http_version} {response.request}")
+    logger.info(f'本次响应的状态码:{response.status_code} {response.http_version} {response.request}')
 
 
 _client_yuyuko: AsyncClient = None
 _client_wg: AsyncClient = None
 _client_default: AsyncClient = None
 
 
 async def create_client_yuyuko() -> AsyncClient:
     global _client_yuyuko
     _client_yuyuko = httpx.AsyncClient(
         headers={
             'Authorization': hikari_config.token,
-            "accept": "application/json",
-            "Content-Type": "application/json",
-            "Yuyuko-Client-Type": f"BOT;{__version__}",
+            'accept': 'application/json',
+            'Content-Type': 'application/json',
+            'Yuyuko-Client-Type': f'BOT;{__version__}',
         },
         event_hooks={
-            "request": [
+            'request': [
                 before_request,
             ],
-            "response": [
+            'response': [
                 after_response,
             ],
         },
         http2=hikari_config.http2,
     )
+    logger.info('创建client_yuyuko')
     return _client_yuyuko
 
 
 async def create_client_wg() -> AsyncClient:
     if hikari_config.proxy:
-        proxy = {"https://": hikari_config.proxy}
+        proxy = {'https://': hikari_config.proxy}
     else:
         proxy = {}
-    global client_wg
+    global _client_wg
     _client_wg = httpx.AsyncClient(proxies=proxy)
+    logger.info('创建client_wg')
     return _client_wg
 
 
 async def create_client_default() -> AsyncClient:
     global _client_default
     _client_default = httpx.AsyncClient()
+    logger.info('创建client_default')
     return _client_default
 
 
 async def get_client_yuyuko() -> AsyncClient:
     return _client_yuyuko if _client_yuyuko else await create_client_yuyuko()
 
 
 async def get_client_wg() -> AsyncClient:
     return _client_wg if _client_wg else await create_client_wg()
 
 
 async def get_client_default() -> AsyncClient:
     return _client_default if _client_default else await create_client_default()
+
+
+async def recreate_client_yuyuko():
+    _client_yuyuko = await get_client_yuyuko()
+    logger.info('重新创建yuyuko连接池')
+    await _client_yuyuko.aclose()
+    _client_yuyuko = await create_client_yuyuko()
+
+
+async def recreate_client_wg():
+    _client_wg = await get_client_wg()
+    logger.info('重新创建wg连接池')
+    await _client_wg.aclose()
+    _client_wg = await create_client_wg()
+
+
+async def recreate_client_default():
+    _client_default = await get_client_default()
+    logger.info('重新创建default连接池')
+    await _client_default.aclose()
+    _client_default = await create_client_default()
```

### Comparing `hikari_core-0.1.6/hikari_core/model.py` & `hikari_core-0.9.0/hikari_core/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 import time
-from datetime import date
 from typing import List, Optional, Protocol, Union, runtime_checkable
 
 from pydantic import BaseModel, Field
 
 
 @runtime_checkable
 class Func(Protocol):
     async def __call__(self, **kwargs):
         ...
 
 
 class UserInfo_Model(BaseModel):
-    Platform: str = "QQ"
-    PlatformId: str = "1119809439"
+    Platform: str = 'QQ'
+    PlatformId: str = '1119809439'
 
 
 class Ship_Model(BaseModel):
     Ship_Nation: Optional[str]
     Ship_Tier: Optional[int]
     Ship_Type: Optional[str]
-    Ship_Name: Optional[str]
+    Ship_Name_Cn: Optional[str]
+    Ship_Name_English: Optional[str]
     ship_Name_Numbers: Optional[str]
     Ship_Id: Optional[int]
 
 
 class Input_Model(BaseModel):
-    Command_Text: Optional[str] = ""  # 输入的指令,请提前去除wws
+    Command_Text: Optional[str] = ''  # 输入的指令,请提前去除wws
     Command_List: Optional[List]
     Search_Type: Optional[int] = 3  # 1:me  2:@  3:server+name or default
     Platform: Optional[str]
     PlatformId: Optional[str]
     Server: Optional[str]
     AccountName: Optional[str]
     AccountId: Optional[int]
     ClanName: Optional[str]
     Recent_Day: Optional[int] = 0
-    Recent_Date: Optional[str] = time.strftime("%Y-%m-%d", time.localtime())
+    Recent_Date: Optional[str] = time.strftime('%Y-%m-%d', time.localtime())
     Select_Index: Optional[int]
     Select_Data: Optional[List]
     ShipInfo: Ship_Model = Ship_Model()
 
 
 class Output_Model(BaseModel):
     Yuyuko_Code: Optional[int]
-    Data_Type: str = Field("str", description="返回的类型")
-    Data: Union[str, int, bytes] = Field("初始化", description="返回的数据")
+    Data_Type: str = Field('str', description='返回的类型')
+    Data: Union[str, int, bytes] = Field('初始化', description='返回的数据')
     Template: Optional[str]
     Width: Optional[int]
     Height: Optional[int]
 
 
 class Hikari_Model(BaseModel):
-    Status: str = "init"  # init:初始化 success:请求成功  failed:请求成功但API有错误或空返回  error:异常及本地错误
+    Status: str = 'init'  # init:初始化 success:请求成功  failed:请求成功但API有错误或空返回  error:异常及本地错误
     UserInfo: UserInfo_Model = UserInfo_Model()
     Function: Func = None
     Input: Input_Model = Input_Model()
     Output: Output_Model = Output_Model()
 
     class Config:
         arbitrary_types_allowed = True
 
     def error(self, error_data):
-        self.Status = "error"
+        self.Status = 'error'
         self.Output.Data = error_data
         self.Output.Data_Type = str(type(error_data))
         return self
 
     def success(self, success_data):
-        self.Status = "success"
+        self.Status = 'success'
         self.Output.Data = success_data
         self.Output.Data_Type = str(type(success_data))
         return self
 
     def failed(self, failed_data):
-        self.Status = "failed"
+        self.Status = 'failed'
         self.Output.Data = failed_data
         self.Output.Data_Type = str(type(failed_data))
         return self
 
     def wait(self, select_data: List):
-        self.Status = "wait"
+        self.Status = 'wait'
         self.Input.Select_Data = select_data
         self.Output.Data = select_data
         self.Output.Data_Type = str(type(self.Output.Data))
         return self
 
     def set_template_info(self, template_name: str, width: int, height: int):
         """配置模板解析参数
```

### Comparing `hikari_core-0.1.6/hikari_core/moudle/publicAPI.py` & `hikari_core-0.9.0/hikari_core/moudle/publicAPI.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,269 +1,302 @@
-# fmt: off
 import asyncio
 import gzip
 import traceback
 from asyncio.exceptions import TimeoutError
 from base64 import b64encode
-from typing import List, Tuple
+from typing import List
 
 import orjson
 from bs4 import BeautifulSoup
-from httpx import ConnectTimeout
+from httpx import ConnectTimeout, PoolTimeout
 from loguru import logger
 
-from ..data_source import levels, nations, number_url_homes, shiptypes
-from ..HttpClient_Pool import (get_client_default, get_client_wg,
-                               get_client_yuyuko)
-from ..model import Ship_Model
-from ..utils import match_keywords
-
-# fmt: on
+from ..data_source import number_url_homes
+from ..HttpClient_Pool import (
+    get_client_default,
+    get_client_wg,
+    get_client_yuyuko,
+    recreate_client_default,
+    recreate_client_wg,
+    recreate_client_yuyuko,
+)
+from ..model import Hikari_Model, Ship_Model
 
 
 async def get_nation_list():
     try:
-        msg = ""
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/nation/list"
+        msg = ''
+        url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/nation/list'
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, timeout=None)
         result = orjson.loads(resp.content)
-        for nation in result["data"]:
+        for nation in result['data']:
             msg: str = msg + f"{nation['cn']}：{nation['nation']}\n"
         return msg
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         logger.error(traceback.format_exc())
 
 
-async def get_ship_name(server_type, infolist: List, bot, ev):
-    msg = ""
+async def get_ship_name(hikari: Hikari_Model):
+    msg = ''
     try:
-        param_nation, infolist = await match_keywords(infolist, nations)
-        if not param_nation:
-            return "请检查国家名是否正确"
-
-        param_shiptype, infolist = await match_keywords(infolist, shiptypes)
-        if not param_shiptype:
-            return "请检查船只类别是否正确"
-
-        param_level, infolist = await match_keywords(infolist, levels)
-        if not param_level:
-            return "请检查船只等级是否正确"
         params = {
-            "county": param_nation,
-            "level": param_level,
-            "shipName": "",
-            "shipType": param_shiptype,
+            'country': hikari.Input.ShipInfo.Ship_Nation,
+            'level': hikari.Input.ShipInfo.Ship_Tier,
+            'shipName': '',
+            'shipType': hikari.Input.ShipInfo.Ship_Type,
+            'groupType': 'default',
         }
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
+        url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/ship/search'
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        if result["data"]:
-            for ship in result["data"]:
-                msg += f"{ship['shipNameCn']}：{ship['shipNameNumbers']}\n"
+        if result['data']:
+            for ship in result['data']:
+                msg += f"{ship['nameCn']}：{ship['nameEnglish']}\n"
+            return hikari.success(msg)
         else:
-            msg = "没有符合的船只"
-        return msg
+            return hikari.failed('没有符合的船只')
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
+        return hikari.error('请求超时了，请过会儿再尝试哦~')
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return hikari.error('连接池异常，请尝试重新查询~')
     except Exception:
         logger.error(traceback.format_exc())
-        return "wuwuwu出了点问题，请联系麻麻解决"
+        return hikari.error('wuwuwu出了点问题，请联系麻麻解决')
 
 
 async def get_ship_byName(shipname: str) -> List:
     try:
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
-        params = {"county": "", "level": "", "shipName": shipname, "shipType": ""}
+        shipname_select_index = None
+        result = shipname.split('.')
+        if len(result) == 2 and result[1].isdigit():
+            shipname = result[0]
+            shipname_select_index = int(result[1])
+        url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/ship/search'
+        params = {'country': '', 'level': '', 'shipName': shipname, 'shipType': '', 'groupType': 'default'}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        List = []
-        if result["code"] == 200 and result["data"]:
-            for each in result["data"]:
+        List, select_List = [], []
+        if result['code'] == 200 and result['data']:
+            for each in result['data']:
                 List.append(
                     Ship_Model(
-                        Ship_Nation=each["country"],
-                        Ship_Tier=each["tier"],
-                        Ship_Type=each["shipType"],
-                        Ship_Name=each["shipNameCn"],
-                        ship_Name_Numbers=each["shipNameNumbers"],
-                        Ship_Id=each["id"],
+                        Ship_Nation=each['country'],
+                        Ship_Tier=each['level'],
+                        Ship_Type=each['shipType'],
+                        Ship_Name_Cn=each['nameCn'],
+                        Ship_Name_English=each['nameEnglish'],
+                        ship_Name_Numbers=each['nameEnglish'],
+                        Ship_Id=each['shipId'],
                     )
                 )
-            return List
+            if shipname_select_index and shipname_select_index <= len(List):
+                select_List.append(List[shipname_select_index - 1])
+                return select_List
+            else:
+                return List
         else:
             return None
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def get_all_shipList():
     try:
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
-        params = {"county": "", "level": "", "shipName": "", "shipType": ""}
+        url = 'https://v3-api.wows.shinoaki.com/public/wows/encyclopedia/ship/search'
+        params = {'country': '', 'level': '', 'shipName': '', 'shipType': '', 'groupType': 'default'}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        if result["code"] == 200 and result["data"]:
-            return result["data"]
+        if result['code'] == 200 and result['data']:
+            return result['data']
         else:
             return None
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         return None
 
 
 async def get_AccountIdByName(server: str, name: str) -> str:
     try:
-        url = "https://api.wows.shinoaki.com/public/wows/account/search/user"
-        params = {"server": server, "userName": name}
+        url = 'https://api.wows.shinoaki.com/public/wows/account/search/user'
+        params = {'server': server, 'userName': name}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        if result["code"] == 200 and result["data"]:
-            return int(result["data"]["accountId"])
+        if result['code'] == 200 and result['data']:
+            return int(result['data']['accountId'])
         else:
-            return result["message"]
+            return result['message']
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
-        return "请求超时了，请过一会儿重试哦~"
+        return '请求超时了，请过一会儿重试哦~'
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         logger.error(traceback.format_exc())
-        return "好像出了点问题呢，可能是网络问题，如果重试几次还不行的话，请联系麻麻解决"
+        return '好像出了点问题呢，可能是网络问题，如果重试几次还不行的话，请联系麻麻解决'
 
 
 async def get_ClanIdByName(server: str, tag: str):
     try:
-        url = "https://api.wows.shinoaki.com/public/wows/clan/search"
-        params = {"server": server, "tag": tag, "type": 1}
+        url = 'https://api.wows.shinoaki.com/public/wows/clan/search'
+        params = {'server': server, 'tag': tag, 'type': 1}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        List = []
-        if result["code"] == 200 and result["data"]:
+        if result['code'] == 200 and result['data']:
             # for each in result['data']:
             #    List.append([each['clanId'],each['name'],each['serverName'],each['tag']])
-            return result["data"]
+            return result['data']
         else:
             return None
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def check_yuyuko_cache(server, id):
     try:
-        yuyuko_cache_url = "https://api.wows.shinoaki.com/api/wows/cache/check"
-        params = {"accountId": id, "server": server}
+        yuyuko_cache_url = 'https://api.wows.shinoaki.com/api/wows/cache/check'
+        params = {'accountId': id, 'server': server}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.post(yuyuko_cache_url, json=params, timeout=5)
         result = orjson.loads(resp.content)
         cache_data = {}
-        if result["code"] == 201:
-            if "DEV" in result["data"]:
-                await get_wg_info(cache_data, "DEV", result["data"]["DEV"])
-            elif "pvp" in result["data"]:
+        if result['code'] == 201:
+            if 'DEV' in result['data']:
+                await get_wg_info(cache_data, 'DEV', result['data']['DEV'])
+            elif 'pvp' in result['data']:
                 tasks = []
-                for key in result["data"]:
-                    tasks.append(asyncio.ensure_future(get_wg_info(cache_data, key, result["data"][key])))
+                for key in result['data']:
+                    tasks.append(asyncio.ensure_future(get_wg_info(cache_data, key, result['data'][key])))
                 await asyncio.gather(*tasks)
             if not cache_data:
                 return False
             data_base64 = b64encode(gzip.compress(orjson.dumps(cache_data))).decode()
-            params["data"] = data_base64
+            params['data'] = data_base64
             resp = await client_yuyuko.post(yuyuko_cache_url, json=params, timeout=5)
             result = orjson.loads(resp.content)
             logger.success(result)
-            if result["code"] == 200:
+            if result['code'] == 200:
                 return True
             else:
                 return False
         return False
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         logger.error(traceback.format_exc())
         return False
 
 
 async def get_wg_info(params, key, url):
     try:
         client_wg = await get_client_wg()
         resp = await client_wg.get(url, timeout=5, follow_redirects=True)
         wg_result = orjson.loads(resp.content)
-        if resp.status_code == 200 and wg_result["status"] == "ok":
+        if resp.status_code == 200 and wg_result['status'] == 'ok':
             params[key] = resp.text
+    except PoolTimeout:
+        await recreate_client_wg()
+        return
     except Exception:
         logger.error(traceback.format_exc())
-        logger.error(f"上报url：{url}")
+        logger.error(f'上报url：{url}')
         return
 
 
 async def get_MyShipRank_yuyuko(params) -> int:
     try:
-        url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
+        url = 'https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank'
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        if result["code"] == 200 and result["data"]:
-            if result["data"]["ranking"]:
-                return result["data"]["ranking"]
-            elif not result["data"]["ranking"] and not result["data"]["serverId"] == "cn":
-                ranking = await get_MyShipRank_Numbers(result["data"]["httpUrl"], result["data"]["serverId"])
+        if result['code'] == 200 and result['data']:
+            if result['data']['ranking']:
+                return result['data']['ranking']
+            elif not result['data']['ranking'] and not result['data']['serverId'] == 'cn':
+                ranking = await get_MyShipRank_Numbers(result['data']['httpUrl'], result['data']['serverId'])
                 if ranking:
                     await post_MyShipRank_yuyuko(
-                        result["data"]["accountId"],
+                        result['data']['accountId'],
                         ranking,
-                        result["data"]["serverId"],
-                        result["data"]["shipId"],
+                        result['data']['serverId'],
+                        result['data']['shipId'],
                     )
                 return ranking
             else:
                 return None
         else:
             return None
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def get_MyShipRank_Numbers(url, server) -> int:
     try:
         data = None
         client_default = await get_client_default()
-        client_default = await get_client_default()
         resp = await client_default.get(url, timeout=10)
         if resp.content:
             result = orjson.loads(resp.content)
-            page_url = str(result["url"]).replace("\\", "")
-            nickname = str(result["nickname"])
-            my_rank_url = f"{number_url_homes[server]}{page_url}"
+            page_url = str(result['url']).replace('\\', '')
+            nickname = str(result['nickname'])
+            my_rank_url = f'{number_url_homes[server]}{page_url}'
             resp = await client_default.get(my_rank_url, timeout=10)
-            soup = BeautifulSoup(resp.content, "html.parser")
-            data = soup.select_one(f'tr[data-nickname="{nickname}"]').select_one("td").string
+            soup = BeautifulSoup(resp.content, 'html.parser')
+            data = soup.select_one(f'tr[data-nickname="{nickname}"]').select_one('td').string
         if data and data.isdigit():
             return data
         else:
             return None
+    except PoolTimeout:
+        await recreate_client_default()
+        return
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def post_MyShipRank_yuyuko(accountId, ranking, serverId, shipId):
     try:
-        url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
+        url = 'https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank'
         post_data = {
-            "accountId": int(accountId),
-            "ranking": int(ranking),
-            "serverId": serverId,
-            "shipId": int(shipId),
+            'accountId': int(accountId),
+            'ranking': int(ranking),
+            'serverId': serverId,
+            'shipId': int(shipId),
         }
         client_yuyuko = await get_client_yuyuko()
-        resp = await client_yuyuko.post(url, json=post_data, timeout=None)
-        result = orjson.loads(resp.content)
+        await client_yuyuko.post(url, json=post_data, timeout=None)
+        return
+    except PoolTimeout:
+        await recreate_client_yuyuko()
         return
     except Exception:
         logger.error(traceback.format_exc())
         return
```

### Comparing `hikari_core-0.1.6/hikari_core/moudle/wws_info.py` & `hikari_core-0.9.0/hikari_core/game/box_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 import traceback
 from asyncio.exceptions import TimeoutError
 
 import orjson
-from httpx import ConnectTimeout
+from httpx import ConnectTimeout, PoolTimeout
 from loguru import logger
 
-from ..HttpClient_Pool import get_client_yuyuko
+from ..HttpClient_Pool import get_client_yuyuko, recreate_client_yuyuko
 from ..model import Hikari_Model
-from .publicAPI import check_yuyuko_cache, get_AccountIdByName
+from ..moudle.publicAPI import get_AccountIdByName
 
 
-async def get_AccountInfo(hikari: Hikari_Model) -> Hikari_Model:
+async def check_christmas_box(hikari: Hikari_Model) -> Hikari_Model:
     try:
-        if hikari.Status == "init":
+        if hikari.Status == 'init':
             if hikari.Input.Search_Type == 3:
                 hikari.Input.AccountId = await get_AccountIdByName(hikari.Input.Server, hikari.Input.AccountName)
                 if not isinstance(hikari.Input.AccountId, int):
-                    return hikari.error(f"{hikari.Input.AccountId}")
+                    return hikari.error(f'{hikari.Input.AccountId}')
         else:
-            return hikari.error("当前请求状态错误")
-        is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
-        if is_cache:
-            logger.success("上报数据成功")
-        else:
-            logger.success("跳过上报数据，直接请求")
-        url = "https://v3-api.wows.shinoaki.com/public/wows/account/user/info"
+            return hikari.error('当前请求状态错误')
+        url = 'https://api.wows.shinoaki.com/public/wows/christmas/ship/box'
         if hikari.Input.Search_Type == 3:
-            params = {"server": hikari.Input.Server, "accountId": hikari.Input.AccountId}
+            params = {'server': hikari.Input.Server, 'accountId': hikari.Input.AccountId}
         else:
-            params = {"server": hikari.Input.Platform, "accountId": hikari.Input.PlatformId}
+            params = {'server': hikari.Input.Platform, 'accountId': hikari.Input.PlatformId}
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        hikari.Output.Yuyuko_Code = result["code"]
-        if result["code"] == 200 and result["data"]:
-            hikari = hikari.set_template_info("wws-info.html", 920, 1000)
-            return hikari.success(result["data"])
-        elif result["code"] == 403:
+        hikari.Output.Yuyuko_Code = result['code']
+        if result['code'] == 200 and result['data']:
+            hikari = hikari.set_template_info('wws-box-christmas.html', 920, 1000)
+            return hikari.success(result['data'])
+        elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
-        elif result["code"] == 500:
+        elif result['code'] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
         else:
             return hikari.failed(f"{result['message']}")
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
-        return hikari.erroe("请求超时了，请过会儿再尝试哦~")
+        return hikari.error('请求超时了，请过会儿再尝试哦~')
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return hikari.error('连接池异常，请尝试重新查询~')
     except Exception:
         logger.error(traceback.format_exc())
-        return hikari.error("wuwuwu出了点问题，请联系麻麻解决")
+        return hikari.error('wuwuwu出了点问题，请联系麻麻解决')
```

### Comparing `hikari_core-0.1.6/hikari_core/moudle/wws_recent.py` & `hikari_core-0.9.0/hikari_core/moudle/wws_recent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 import traceback
 from asyncio.exceptions import TimeoutError
-from datetime import datetime
 
 import orjson
-from httpx import ConnectTimeout
+from httpx import ConnectTimeout, PoolTimeout
 from loguru import logger
 
-from ..HttpClient_Pool import get_client_yuyuko
+from ..HttpClient_Pool import get_client_yuyuko, recreate_client_yuyuko
 from ..model import Hikari_Model
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName
 
 # from nonebot_plugin_htmlrender import html_to_pic
 
 
 async def get_RecentInfo(hikari: Hikari_Model) -> Hikari_Model:
     try:
-        if hikari.Status == "init":
+        if hikari.Status == 'init':
             if hikari.Input.Search_Type == 3:
                 hikari.Input.AccountId = await get_AccountIdByName(hikari.Input.Server, hikari.Input.AccountName)
                 if not isinstance(hikari.Input.AccountId, int):
-                    return hikari.error(f"{hikari.Input.AccountId}")
+                    return hikari.error(f'{hikari.Input.AccountId}')
         else:
-            return hikari.error("当前请求状态错误")
-        is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
+            return hikari.error('当前请求状态错误')
+        if hikari.Input.Search_Type == 3:
+            is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
+        else:
+            is_cache = await check_yuyuko_cache(hikari.Input.Platform, hikari.Input.PlatformId)
         if is_cache:
-            logger.success("上报数据成功")
+            logger.success('上报数据成功')
         else:
-            logger.success("跳过上报数据，直接请求")
-        url = "https://recent.wows.shinoaki.com:8890/api/wows/recent/day/info"
+            logger.success('跳过上报数据，直接请求')
+        url = 'https://recent.wows.shinoaki.com:8890/api/wows/recent/day/info'
         if hikari.Input.Search_Type == 3:
             params = {
-                "server": hikari.Input.Server,
-                "accountId": hikari.Input.AccountId,
-                "dateTime": hikari.Input.Recent_Date,
-                "day": hikari.Input.Recent_Day,
+                'server': hikari.Input.Server,
+                'accountId': hikari.Input.AccountId,
+                'dateTime': hikari.Input.Recent_Date,
+                'day': hikari.Input.Recent_Day,
+                'shipId': 0,
             }
         else:
             params = {
-                "server": hikari.Input.Platform,
-                "accountId": hikari.Input.PlatformId,
-                "dateTime": hikari.Input.Recent_Date,
-                "day": hikari.Input.Recent_Day,
+                'server': hikari.Input.Platform,
+                'accountId': hikari.Input.PlatformId,
+                'dateTime': hikari.Input.Recent_Date,
+                'day': hikari.Input.Recent_Day,
+                'shipId': 0,
             }
         print(params)
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        hikari.Output.Yuyuko_Code = result["code"]
-        if result["code"] == 200:
-            if result["data"]["battleTypeInfo"]['PVP']['battle'] or result["data"]["battleTypeInfo"]['RANK_SOLO']['battle']:
-                hikari = hikari.set_template_info("wws-info-recent.html", 1200, 100)
-                return hikari.success(result["data"])
+        hikari.Output.Yuyuko_Code = result['code']
+        if result['code'] == 200:
+            if result['data']['battleTypeInfo']['PVP']['battle'] or result['data']['battleTypeInfo']['RANK_SOLO']['battle']:
+                hikari = hikari.set_template_info('wws-info-recent.html', 1200, 100)
+                return hikari.success(result['data'])
             else:
-                return hikari.failed("该日期数据记录不存在")
-        elif result["code"] == 403:
+                return hikari.failed('该日期数据记录不存在')
+        elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
-        elif result["code"] == 404 or result["code"] == 405:
+        elif result['code'] == 404 or result['code'] == 405:
             return hikari.failed(f"{result['message']}\n您可以发送wws help查看recent相关说明")
-        elif result["code"] == 500:
+        elif result['code'] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
         else:
             return hikari.failed(f"{result['message']}")
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
-        return hikari.erroe("请求超时了，请过会儿再尝试哦~")
+        return hikari.error('请求超时了，请过会儿再尝试哦~')
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return hikari.error('连接池异常，请尝试重新查询~')
     except Exception:
         logger.error(traceback.format_exc())
-        return hikari.error("wuwuwu出了点问题，请联系麻麻解决")
+        return hikari.error('wuwuwu出了点问题，请联系麻麻解决')
```

### Comparing `hikari_core-0.1.6/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-0.9.0/hikari_core/moudle/wws_ship_recent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,89 @@
 # fmt: off
 import traceback
 from asyncio.exceptions import TimeoutError
 
 import orjson
-from httpx import ConnectTimeout
+from httpx import ConnectTimeout, PoolTimeout
 from loguru import logger
 
-from ..HttpClient_Pool import get_client_yuyuko
+from ..HttpClient_Pool import get_client_yuyuko, recreate_client_yuyuko
 from ..model import Hikari_Model
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName, get_ship_byName
 
 # fmt: on
 
 
 async def get_ShipRecent(hikari: Hikari_Model) -> Hikari_Model:
     try:
-        if hikari.Status == "init":
-            shipList = await get_ship_byName(hikari.Input.ShipInfo.Ship_Name)
+        if hikari.Status == 'init':
+            shipList = await get_ship_byName(hikari.Input.ShipInfo.Ship_Name_Cn)
             if shipList:
                 if len(shipList) < 2:
                     hikari.Input.ShipInfo = shipList[0]
                 else:
                     hikari.Input.Select_Data = shipList
-                    hikari.set_template_info("select-ship.html", 360, 100)
+                    hikari.set_template_info('select-ship.html', 360, 100)
                     return hikari.wait(shipList)
             else:
-                return hikari.failed("找不到船，请确认船名是否正确，可以使用【wws 查船名】查询船只中英文")
-        elif hikari.Status == "wait":
+                return hikari.failed('找不到船，请确认船名是否正确，可以使用【wws 查船名】查询船只中英文')
+        elif hikari.Status == 'wait':
             if hikari.Input.Select_Data and hikari.Input.Select_Index and hikari.Input.Select_Index <= len(hikari.Input.Select_Data):
                 hikari.Input.ShipInfo = hikari.Input.Select_Data[hikari.Input.Select_Index - 1]
             else:
-                return hikari.error("请选择有效的序号")
+                return hikari.error('请选择有效的序号')
         else:
-            return hikari.error("当前请求状态错误")
+            return hikari.error('当前请求状态错误')
 
         if hikari.Input.Search_Type == 3:
             hikari.Input.AccountId = await get_AccountIdByName(hikari.Input.Server, hikari.Input.AccountName)
             if not isinstance(hikari.Input.AccountId, int):
-                return hikari.error(f"{hikari.Input.AccountId}")
+                return hikari.error(f'{hikari.Input.AccountId}')
 
-        is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
+        if hikari.Input.Search_Type == 3:
+            is_cache = await check_yuyuko_cache(hikari.Input.Server, hikari.Input.AccountId)
+        else:
+            is_cache = await check_yuyuko_cache(hikari.Input.Platform, hikari.Input.PlatformId)
         if is_cache:
-            logger.success("上报数据成功")
+            logger.success('上报数据成功')
         else:
-            logger.success("跳过上报数据，直接请求")
+            logger.success('跳过上报数据，直接请求')
 
-        url = "https://api.wows.shinoaki.com/api/wows/recent/v2/recent/info/ship"
+        url = 'https://api.wows.shinoaki.com/api/wows/recent/v2/recent/info/ship'
         if hikari.Input.Search_Type == 3:
             params = {
-                "server": hikari.Input.Server,
-                "accountId": hikari.Input.AccountId,
-                "shipId": hikari.Input.ShipInfo.Ship_Id,
-                "day": hikari.Input.Recent_Day,
+                'server': hikari.Input.Server,
+                'accountId': hikari.Input.AccountId,
+                'shipId': hikari.Input.ShipInfo.Ship_Id,
+                'day': hikari.Input.Recent_Day,
             }
         else:
             params = {
-                "server": hikari.Input.Platform,
-                "accountId": hikari.Input.PlatformId,
-                "shipId": hikari.Input.ShipInfo.Ship_Id,
-                "day": hikari.Input.Recent_Day,
+                'server': hikari.Input.Platform,
+                'accountId': hikari.Input.PlatformId,
+                'shipId': hikari.Input.ShipInfo.Ship_Id,
+                'day': hikari.Input.Recent_Day,
             }
 
         client_yuyuko = await get_client_yuyuko()
         resp = await client_yuyuko.get(url, params=params, timeout=None)
         result = orjson.loads(resp.content)
-        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
-        hikari.Output.Yuyuko_Code = result["code"]
+        hikari.Output.Yuyuko_Code = result['code']
 
-        if result["code"] == 200 and result["data"]:
-            hikari.set_template_info("wws-ship-recent.html", 800, 100)
-            return hikari.success(result["data"])
-        elif result["code"] == 403:
+        if result['code'] == 200 and result['data']:
+            hikari.set_template_info('wws-ship-recent.html', 800, 100)
+            return hikari.success(result['data'])
+        elif result['code'] == 403:
             return hikari.failed(f"{result['message']}\n请先绑定账号")
-        elif result["code"] == 500:
+        elif result['code'] == 500:
             return hikari.failed(f"{result['message']}\n这是服务器问题，请联系雨季麻麻")
         else:
             return hikari.failed(f"{result['message']}")
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
-        return hikari.erroe("请求超时了，请过会儿再尝试哦~")
+        return hikari.error('请求超时了，请过会儿再尝试哦~')
+    except PoolTimeout:
+        await recreate_client_yuyuko()
+        return hikari.error('连接池异常，请尝试重新查询~')
     except Exception:
         logger.error(traceback.format_exc())
-        return hikari.error("wuwuwu出了点问题，请联系麻麻解决")
+        return hikari.error('wuwuwu出了点问题，请联系麻麻解决')
```

### Comparing `hikari_core-0.1.6/hikari_core/Template/select-ship.html` & `hikari_core-0.9.0/hikari_core/Template/select-ship.html`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png">
 							{% elif ship['Ship_Type'] == 'AirCarrier' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png">
 							{% elif ship['Ship_Type'] == 'Submarine' %}
 							<img src="https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png">
 							{% endif %}
 						</div>
-						<div class="ship-name">{{ ship['Ship_Name'] }}</div>
+						<div class="ship-name">{{ ship['Ship_Name_Cn'] }}</div>
 					</div>
 				</div>
 				{% endfor %}
 			</div>
 		</div>
 	</body>
```

#### html2text {}

```diff
@@ -9,9 +9,9 @@
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png] {% elif ship
 ['Ship_Type'] == 'Battleship' %} [https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png] {% elif ship
 ['Ship_Type'] == 'AirCarrier' %} [https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png] {% elif ship
 ['Ship_Type'] == 'Submarine' %} [https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png] {% endif %}
-{{ ship['Ship_Name'] }}
+{{ ship['Ship_Name_Cn'] }}
 {% endfor %}
```

### Comparing `hikari_core-0.1.6/hikari_core/Template/ship-rank.html` & `hikari_core-0.9.0/hikari_core/Template/ship-rank.html`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,18 @@
 		}
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
 				<div class="page-header">
 					<div class="ship-level">
-						{{ shipInfo['tier'] }}
+						{{ data['shipInfo']['Ship_Tier'] }}
 					</div>
 					<div class="ship-name">
-						{{ shipInfo['shipNameCn'] }}
+						{{ data['shipInfo']['Ship_Name_Cn'] }}
 					</div>
 				</div>
 				<div class="rank-header">
 					<div class="ranks flex-2 col">排名</div>
 					<div class="player-name flex-10 col">ID</div>
 					<div class="battles flex-2 col">场次</div>
 					<div class="pr flex-3 col">PR</div>
@@ -119,15 +119,15 @@
 					<div class="avg-dmg flex-5 col">场均</div>
 					<div class="max-dmg flex-5 col">最大伤害</div>
 					<div class="xp flex-3 col">经验</div>
 					<div class="max-xp flex-3 col">最大经验</div>
 					<div class="ar-frag flex-2 col">击落飞机</div>
 					<div class="max-ar-frag flex-2 col">最大击落</div>
 				</div>
-				{% for rank in data %}
+				{% for rank in data['data'] %}
 				<div class="rank-item">
 					{% if rank['index'] %}
 					<div class="ranks flex-2 col">{{ rank['index'] }}</div>
 					{% else %}
 					<div class="ranks flex-2 col">{{ rank['sortValue'] }}</div>
 					{% endif %}
 					{% if rank['tag'] != null %}
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-{{ shipInfo['tier'] }}
-{{ shipInfo['shipNameCn'] }}
+{{ data['shipInfo']['Ship_Tier'] }}
+{{ data['shipInfo']['Ship_Name_Cn'] }}
 æå
 ID
 åºæ¬¡
 PR
 èç
 å»æ
 æå¤å»æ
 åºå
 æå¤§ä¼¤å®³
 ç»éª
 æå¤§ç»éª
 å»è½é£æº
 æå¤§å»è½
-{% for rank in data %}
+{% for rank in data['data'] %}
 {% if rank['index'] %}
 {{ rank['index'] }}
 {% else %}
 {{ rank['sortValue'] }}
 {% endif %} {% if rank['tag'] != null %}
 [{{ rank['tag'] }}]{{ rank['userName'] }}
 {% else %}
```

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-ban.html` & `hikari_core-0.9.0/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.9.0/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-clan.html` & `hikari_core-0.9.0/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.9.0/hikari_core/Template/wws-info-recent.html`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,46 @@
 			margin-bottom: 20px;
 		}
 		
 		.rank-data-col {
 			display: flex;
 			height: 90px;
 		}
+
+		.frag-data {
+			display: flex;
+			margin: 30px 90px;
+		}
+		
+		.frag-data-col {
+			display: flex;
+			flex: 1;
+			margin-bottom: 20px;
+		}
+		.frag-item {
+			flex: 1;
+			text-align: center;
+			background-color: #F2F2F2;
+			border-radius: 16px;
+			margin: 0 10px;
+        }
+		
+		.frag-key,.frag-value {
+			height: 100px;
+			font-size: 35px;
+		}
+		
+		.frag-key {
+			color: #606266;
+			font-weight: normal;
+			line-height: 120px;
+		}
+		.frag-value {
+			line-height: 80px;
+		}
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
 				
 				<div class="page-header">
 					<div class="clan-user-server">
@@ -465,15 +497,15 @@
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['frags']) }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 					</div>
 					{% endif %}
 					
 					{% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
-					<<div class="information-col">
+					<div class="information-col">
 						<div class="information-col-item information-type">排位</div>
 						<div class="information-col-item">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}</div>
 						<div class="information-col-item" style="color: {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
 						<div class="information-col-item">{{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
@@ -533,24 +565,56 @@
 					</div>
 					{% for ship in data['shipInfoBattleList'] %}
 						{% if ship['typeInfo']['RANK_SOLO']['battle'] %}
 						<div class="rank-data-col">
 							<div class="random-col-item flex-3 ship-level">{{ ship['shipInfo']['level'] }}</div>
 							<div class="random-col-item flex-8">{{ ship['shipInfo']['nameCn'] }}</div>
 							<div class="random-col-item flex-3">{{ ship['typeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
-							<div class="random-col-item flex-3" style="color: {{ ship['typeInfo']['RANK_SOLO']['prInfo']['color'] }};">{{ ship['typeInfo']['PVP']['prInfo']['value'] }}</div>
-							<div class="random-col-item flex-3" style="color: {{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ ship['typeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%</div>
-							<div class="random-col-item flex-4" style="color: {{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ ship['typeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="random-col-item flex-3" style="color: {{ ship['typeInfo']['RANK_SOLO']['prInfo']['color'] }};">{{ ship['typeInfo']['RANK_SOLO']['prInfo']['value'] }}</div>
+							<div class="random-col-item flex-3" style="color: {{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">{{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="random-col-item flex-4" style="color: {{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">{{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
 							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
 							<div class="random-col-item flex-3">{{ '%.2f' | format(ship['typeInfo']['RANK_SOLO']['battleInfo']['hitRatioInfo']['ratioMain']) }}%</div>
 						</div>
 						{% endif %}
 					{% endfor %}
 				</div>
 				{% endif %}
+
+				<div class="information-header">击沉数据</div>
+				<div class="frag-data">
+					<div class="frag-data-col">
+						<div class="frag-item">
+							<div class="frag-key">主炮击沉</div>
+							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByMain'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByMain'] }}</div>
+						</div>
+						<div class="frag-item">
+							<div class="frag-key">副炮击沉</div>
+							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByAtba'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByAtba'] }}</div>
+						</div>
+						<div class="frag-item">
+							<div class="frag-key">舰载机击沉</div>
+							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByPlanes'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByPlanes'] }}</div>
+						</div>
+					</div>
+					<div class="frag-data-col">
+						<div class="frag-item">
+							<div class="frag-key">鱼雷击沉</div>
+							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByTpd'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByTpd'] }}</div>
+						</div>
+						<div class="frag-item">
+							<div class="frag-key">撞击击沉</div>
+							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByRam'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByRam'] }}</div>
+						</div>
+						<div class="frag-item">
+							<div class="frag-key">深弹击沉</div>
+							<div class="frag-value">{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByDbomb'] + data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByDbomb'] }}</div>
+						</div>
+					</div>
+				</div>
 				
 				<div class="footer">
 					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
 					<p>https://github.com/benx1n/HikariBot</p>
 					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
 					<p>Design By 冷眠 H5 Converted By C1ystal</p>
 					<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
```

#### html2text {}

```diff
@@ -71,15 +71,15 @@
 {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%
 {{ data['battleTypeInfo']['PVP_DIV3']['prInfo']['value'] }}
 {{ data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}
 {{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']['avgInfo']
 ['frags']) }}
 {{ '%.2f' | format(data['battleTypeInfo']['PVP_DIV3']['battleInfo']
 ['hitRatioInfo']['ratioMain']) }}%
-{% endif %} {% if data['battleTypeInfo']['RANK_SOLO']['battle'] %} <
+{% endif %} {% if data['battleTypeInfo']['RANK_SOLO']['battle'] %}
 æä½
 {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}
 {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%
 {{ data['battleTypeInfo']['RANK_SOLO']['prInfo']['value'] }}
 {{ data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}
 {{ '%.2f' | format(data['battleTypeInfo']['RANK_SOLO']['battleInfo']['avgInfo']
 ['frags']) }}
@@ -122,21 +122,44 @@
 å»æ
 å½ä¸­
 {% for ship in data['shipInfoBattleList'] %} {% if ship['typeInfo']
 ['RANK_SOLO']['battle'] %}
 {{ ship['shipInfo']['level'] }}
 {{ ship['shipInfo']['nameCn'] }}
 {{ ship['typeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}
-{{ ship['typeInfo']['PVP']['prInfo']['value'] }}
-{{ ship['typeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%
-{{ ship['typeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}
+{{ ship['typeInfo']['RANK_SOLO']['prInfo']['value'] }}
+{{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%
+{{ ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}
 {{ '%.2f' | format(ship['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']
 ['frags']) }}
 {{ '%.2f' | format(ship['typeInfo']['RANK_SOLO']['battleInfo']['hitRatioInfo']
 ['ratioMain']) }}%
 {% endif %} {% endfor %}
 {% endif %}
+å»æ²æ°æ®
+ä¸»ç®å»æ²
+{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByMain'] +
+data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByMain']
+}}
+å¯ç®å»æ²
+{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByAtba'] +
+data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByAtba']
+}}
+è°è½½æºå»æ²
+{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByPlanes'] +
+data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByPlanes']
+}}
+é±¼é·å»æ²
+{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByTpd'] +
+data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByTpd'] }}
+æå»å»æ²
+{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByRam'] +
+data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByRam'] }}
+æ·±å¼¹å»æ²
+{{ data['battleTypeInfo']['PVP']['battleInfo']['fragsInfo']['fragsByDbomb'] +
+data['battleTypeInfo']['RANK_SOLO']['battleInfo']['fragsInfo']['fragsByDbomb']
+}}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
 èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-info.html` & `hikari_core-0.9.0/hikari_core/Template/wws-ship-recent.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,825 +1,686 @@
 <!DOCTYPE html>
 <html>
+	<head>
+		<meta charset="utf-8">
+		<title></title>
+	</head>
+	<style>
+		* {
+			padding: 0;
+			margin: 0;
+		}
 
-<head>
-	<meta charset="utf-8">
-	<title></title>
-</head>
-<style>
-	* {
-		margin: 0;
-		padding: 0;
-	}
-
-	.main-content {
-		width: 1200px;
-		font-size: 30px;
-		font-family: "Microsoft YaHei";
-		font-weight: bold;
-	}
-
-	.page-box {
-		width: 1200px;
-		display: flex;
-		flex-direction: column;
-	}
-
-	.page-header {
-		display: flex;
-		flex-direction: column;
-		margin-top: 30px;
-	}
-
-	.clan-user-server {
-		height: 120px;
-		text-align: center;
-		font-size: 45px;
-		line-height: 120px;
-	}
-
-	.clan {
-		display: inline-block;
-		padding-right: 10px;
-		height: 120px;
-	}
-
-	.user {
-		display: inline-block;
-		height: 120px;
-	}
-
-	.server {
-		display: inline-block;
-		padding-left: 10px;
-	}
-
-	.server-border {
-		width: 200px;
-		height: 50px;
-		line-height: 50px;
-		text-align: center;
-		background-color: #F2F2F2;
-		border-radius: 25px;
-		font-size: 35px;
-	}
-
-	.image-box {
-		width: 100px;
-		height: 100px;
-		position: fixed;
-		left: 50px;
-		top: 40px;
-	}
-
-	.image-box img {
-		width: 100px;
-		height: 100px;
-		border-radius: 50px;
-	}
-
-	.pr {
-		display: flex;
-		height: 100px;
-		font-weight: bold;
-		line-height: 60px;
-		padding: 0 80px;
-	}
-
-	.pr-bar-bg {
-		position: relative;
-		flex: 1;
-		line-height: 80px;
-		background-color: #A6A6A6;
-		height: 80px;
-		border-radius: 40px;
-		margin-top: 10px;
-		text-align: center;
-		color: #FFFFFF;
-	}
-
-	.pr-bar {
-		position: absolute;
-		top: 0;
-		left: 0;
-		height: 80px;
-		z-index: 1;
-		border-radius: 40px;
-	}
-
-	.pr-number {
-		z-index: 99;
-		position: absolute;
-		left: 0px;
-		right: 0px;
-		font-size: 35px;
-		font-weight: bold;
-	}
-
-	.recnet-time {
-		text-align: center;
-		font-weight: normal;
-	}
-
-	.overview-change {
-		display: flex;
-		margin-top: 30px;
-		padding: 0 50px;
-		height: 300px;
-	}
-
-	.overview-change-item {
-		flex: 1;
-		display: flex;
-		flex-direction: column;
-		margin: 0 20px;
-
-	}
-
-	.item-top {
-		flex: 5;
-		background-color: #F2F2F2;
-		border-radius: 16px;
-	}
-
-	.item-bottom {
-		display: flex;
-		flex: 4;
-		margin-top: 20px;
-	}
-
-	.left-item-bottom {
-		background-color: #F2F2F2;
-		border-radius: 16px;
-	}
-
-	.bottom-mini-item-left {
-		flex: 1;
-		margin-right: 10px;
-		background-color: #F2F2F2;
-		border-radius: 16px;
-	}
-
-	.bottom-mini-item-right {
-		flex: 1;
-		margin-left: 10px;
-		background-color: #F2F2F2;
-		border-radius: 16px;
-	}
-
-	.item-top {
-		display: flex;
-		flex-direction: column;
-	}
-
-	.item-top div {
-		height: 80px;
-		text-align: center;
-		font-size: 40px;
-	}
-
-	.item-top-top {
-		color: #606266;
-		font-weight: normal;
-		line-height: 100px;
-	}
-
-	.item-top-bottom {
-		line-height: 60px;
-	}
-
-	.left-item-bottom {
-		display: flex;
-		flex-direction: column;
-	}
-
-	.change-pr-title {
-		color: #606266;
-		height: 60px;
-		display: flex;
-		font-weight: normal;
-		line-height: 70px;
-	}
-
-	.change-pr {
-		height: 60px;
-		line-height: 50px;
-		text-align: center;
-		font-size: 30px;
-	}
-
-	.change-pr-title-left {
-		flex: 1;
-		font-size: 35px;
-		text-align: right;
-		margin-right: 30px;
-	}
-
-	.change-pr-title-right {
-		flex: 1;
-		font-size: 20px;
-	}
-
-	.bottom-mini-item-left,
-	.bottom-mini-item-right {
-		display: flex;
-		flex-direction: column;
-	}
-
-	.mini-item-top {
-		color: #606266;
-		font-weight: normal;
-		line-height: 70px;
-	}
-
-	.mini-item-bottom {
-		line-height: 45px;
-		font-size: 27px;
-	}
-
-	.bottom-mini-item-left div,
-	.bottom-mini-item-right div {
-		height: 60px;
-		text-align: center;
-	}
-
-	.information-header,
-	.ship-data-header {
-		margin: 0 200px;
-		margin-top: 30px;
-		height: 60px;
-		line-height: 60px;
-		border-radius: 16px;
-		background-color: #D9D9D9;
-		text-align: center;
-	}
-
-	.information-body,
-	.ship-data-body {
-		margin: 0 80px;
-		margin-top: 30px;
-		display: flex;
-		flex-direction: column;
-		background-color: #F2F2F2;
-		border-radius: 16px;
-	}
-
-	.information-col,
-	.ship-data-col {
-		height: 60px;
-		display: flex;
-		line-height: 60px;
-	}
-
-	.information-col-item,
-	.ship-data-col-item {
-		flex: 1;
-		text-align: center;
-	}
-
-	.information-table-header,
-	.ship-data-table-header {
-		color: #606266;
-	}
-
-	.information-type,
-	.ship-data-type {
-		color: #909399;
-	}
-
-	.chart-box {
-		margin: 0 80px;
-		margin-top: 30px;
-		background-color: #F2F2F2;
-		height: 400px;
-		display: flex;
-		border-radius: 16px;
-	}
-
-	.chart-bar {
-		flex: 6;
-	}
-
-	.chart-pie {
-		flex: 4;
-	}
-
-	.footer {
-		margin-top: 30px;
-		text-align: center;
-		font-weight: bold;
-		font-size: 24px;
-		color: #909399;
-		margin-bottom: 20px;
-	}
-</style>
-
-<body>
-	<div class="main-content">
-		<div class="page-box">
-			<div class="page-header">
-
-				<!-- 					<div class="image-box">
-						<img src="IMG_20220607_224103.jpg" />
-					</div> -->
-
-				<div class="clan-user-server">
-					{% if data['userInfo']['clanInfo']['tag'] %}
-					<div class="clan" style="color: {{ data['userInfo']['clanInfo']['color'] }};">[{{
-						data['userInfo']['clanInfo']['tag'] }}]</div>
-					{% endif %}
-					<div class="user">{{ data['userInfo']['userName'] }}</div>
-					<div class="server">
-						<div class="server-border">
-							{{ data['userInfo']['server'] }}
+		.flex-2 {
+			flex: 2;
+		}
+
+		.flex-3 {
+			flex: 3;
+		}
+
+		.flex-4 {
+			flex: 4;
+		}
+
+		.flex-8 {
+			flex: 8;
+		}
+
+		.flex-10 {
+			flex: 10;
+		}
+
+		.main-content {
+			width: 1000px;
+			font-size: 30px;
+			font-family: "Microsoft YaHei";
+			font-weight: bold;
+		}
+
+		.page-box {
+			width: 1000px;
+			display: flex;
+			flex-direction: column;
+		}
+
+		.page-header {
+			display: flex;
+			flex-direction: column;
+		}
+
+		.clan-user-server {
+			height: 120px;
+			text-align: center;
+			font-size: 45px;
+			line-height: 120px;
+		}
+
+		.clan {
+			display: inline-block;
+			padding-right: 10px;
+			height: 120px;
+		}
+
+		.user {
+			display: inline-block;
+			height: 120px;
+		}
+
+		.server {
+			display: inline-block;
+			padding-left: 10px;
+		}
+
+		.server-border {
+			width: 200px;
+			height: 50px;
+			line-height: 50px;
+			text-align: center;
+			background-color: #F2F2F2;
+			border-radius: 25px;
+			font-size: 35px;
+		}
+
+		.ship-bar {
+			height: 80px;
+			font-size: 40px;
+			line-height: 80px;
+			text-align: center;
+			display: flex;
+		}
+
+		.ship-level {
+			flex: 1;
+			text-align: right;
+			margin-right: 30px;
+		}
+
+		.ship-icon {
+			flex: 1;
+			text-align: left;
+			margin-left: 30px;
+		}
+
+		.ship-icon img {
+			width: 80px;
+			height: 80px;
+		}
+
+		.pr {
+			display: flex;
+			height: 100px;
+			font-weight: bold;
+			line-height: 60px;
+			padding: 0 50px;
+		}
+
+		.pr-bar-bg {
+			position: relative;
+			flex: 1;
+			line-height: 80px;
+			background-color: #A6A6A6;
+			height: 80px;
+			border-radius: 40px;
+			margin-top: 10px;
+			text-align: center;
+			color: #FFFFFF;
+		}
+
+		.pr-bar {
+			position: absolute;
+			top: 0;
+			left: 0;
+			height: 80px;
+			z-index: 1;
+			border-radius: 40px;
+		}
+
+		.pr-number {
+			z-index: 99;
+			position: absolute;
+			left: 0px;
+			right: 0px;
+			font-size: 35px;
+			font-weight: bold;
+		}
+
+		.recnet-time {
+			text-align: center;
+			font-weight: normal;
+		}
+
+		.overview-change {
+			display: flex;
+			margin-top: 30px;
+			padding: 0 30px;
+			height: 300px;
+		}
+
+		.overview-change-item {
+			flex: 1;
+			display: flex;
+			flex-direction: column;
+			margin: 0 20px;
+
+		}
+
+		.item-top {
+			flex: 5;
+			background-color: #F2F2F2;
+			border-radius: 16px;
+		}
+
+		.item-bottom {
+			display: flex;
+			flex: 4;
+			margin-top: 20px;
+		}
+
+		.left-item-bottom {
+			background-color: #F2F2F2;
+			border-radius: 16px;
+		}
+
+		.bottom-mini-item-left {
+			flex: 1;
+			margin-right: 10px;
+			background-color: #F2F2F2;
+			border-radius: 16px;
+		}
+
+		.bottom-mini-item-right {
+			flex: 1;
+			margin-left: 10px;
+			background-color: #F2F2F2;
+			border-radius: 16px;
+		}
+
+		.item-top {
+			display: flex;
+			flex-direction: column;
+		}
+
+		.item-top div {
+			height: 80px;
+			text-align: center;
+			font-size: 40px;
+		}
+
+		.item-top-top {
+			color: #606266;
+			font-weight: normal;
+			line-height: 100px;
+		}
+
+		.item-top-bottom {
+			line-height: 60px;
+		}
+
+		.left-item-bottom {
+			display: flex;
+			flex-direction: column;
+		}
+
+		.change-pr-title {
+			color: #606266;
+			height: 60px;
+			display: flex;
+			font-weight: normal;
+			line-height: 70px;
+		}
+
+		.change-pr {
+			height: 60px;
+			line-height: 50px;
+			text-align: center;
+			font-size: 30px;
+		}
+
+		.change-pr-title-left {
+			flex: 1;
+			font-size: 35px;
+			text-align: right;
+			margin-right: 30px;
+		}
+
+		.change-pr-title-right {
+			flex: 1;
+			font-size: 20px;
+		}
+
+		.bottom-mini-item-left,
+		.bottom-mini-item-right {
+			display: flex;
+			flex-direction: column;
+		}
+
+		.mini-item-top {
+			color: #606266;
+			font-weight: normal;
+			line-height: 70px;
+		}
+
+		.mini-item-bottom {
+			line-height: 45px;
+			font-size: 27px;
+		}
+
+		.bottom-mini-item-left div,
+		.bottom-mini-item-right div {
+			height: 60px;
+			text-align: center;
+		}
+
+		.information-header,
+		.day-header {
+			margin: 0 200px;
+			margin-top: 30px;
+			height: 60px;
+			line-height: 60px;
+			border-radius: 16px;
+			background-color: #D9D9D9;
+			text-align: center;
+		}
+
+		.information-body {
+			margin: 0 50px;
+			margin-top: 30px;
+			display: flex;
+			flex-direction: column;
+			background-color: #F2F2F2;
+			border-radius: 16px;
+		}
+
+		.information-col {
+			height: 60px;
+			display: flex;
+			line-height: 60px;
+		}
+
+		.information-col-item,
+		.day-col-item {
+			flex: 1;
+			text-align: center;
+		}
+
+		.information-table-header {
+			color: #606266;
+		}
+
+		.information-type {
+			color: #909399;
+		}
+
+		.day-body {
+			margin: 0 50px;
+			margin-top: 30px;
+		}
+
+		.day-table-header {
+			height: 60px;
+			line-height: 60px;
+			background-color: #D9D9D9;
+			display: flex;
+			border-radius: 16px;
+			color: #606266;
+		}
+
+		.date {
+			background-color: #D9D9D9;
+			width: 300px;
+			height: 40px;
+			line-height: 40px;
+			text-align: center;
+			border-radius: 20px;
+			margin-top: 10px;
+		}
+
+		.day-col {
+			display: flex;
+			height: 60px;
+			line-height: 60px;
+			background-color: #F2F2F2;
+			border-radius: 30px;
+			margin: 10px 0;
+		}
+
+		.footer {
+			margin-top: 30px;
+			text-align: center;
+			font-weight: bold;
+			font-size: 24px;
+			color: #909399;
+			margin-bottom: 20px;
+		}
+	</style>
+	<body>
+		<div class="main-content">
+			<div class="page-box">
+				<div class="page-header">
+					<div class="clan-user-server">
+						
+						{% if data['clanInfo']['tag'] %}
+						<div class="clan" style="color: {{ data['clanInfo']['colorRgb'] }};">[{{ data['clanInfo']['tag'] }}]</div>
+						{% endif %}
+						<div class="user">{{ data['userName'] }}</div>
+						<div class="server">
+							<div class="server-border">
+								{{ data['serverName'] }}
+							</div>
 						</div>
 					</div>
 				</div>
 
+				<div class="ship-bar">
+					{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+					<div class="ship-level">{{ data['shipData'][0]['shipInfo']['shipInfo']['level'] }}</div>
+					{% else %}
+					<div class="ship-level">{{ data['shipData'][0]['rankSolo']['shipInfo']['level'] }}</div>
+					{% endif %}
+					
+					{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+					<div class="ship-name">{{ data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] }}</div>
+					{% else %}
+					<div class="ship-name">{{ data['shipData'][0]['rankSolo']['shipInfo']['nameCn'] }}</div>
+					{% endif %}
+					
+					<div class="ship-icon"><img
+									src={% if data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
+									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
+									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
+									{% elif data['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
+									{% else %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png"
+									{% endif %} />
+					</div>
+				</div>
+
 				<div class="pr">
 					<!-- 动态设置长度及颜色，填写PR即可 -->
 					<div class="pr-bar-bg">
-						<span class="pr-number">{{ data['prInfo']['value'] }}&nbsp;&nbsp;&nbsp;&nbsp;<span
-								class="pr-text"></span></span>
+						{% if data['pvpInfo']['pr']['color'] and data['pvpInfo']['pr']['color'] != '#828282' %}
+						<span class="pr-number">{{ data['pvpInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+						{% else %}
+						<span class="pr-number">{{ data['rankInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span class="pr-text"></span></span>
+						{% endif %}
 						<div class="pr-bar"></div>
 					</div>
 				</div>
 
 				<div class="recnet-time">
-					<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d
-						%H:%M:%S',time.localtime(abs(data['battleTypeInfo'][0]['shipInfo']['lastBattleTime'])))
-						}}</span>
+					<span>记录时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data['shipData'][0]['recordDateTime']/1000)))) }}—{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(time.time())) }}</span>
 				</div>
 
+				{% if data['pvpInfo']['battles'] %}
 				<div class="overview-change">
 					<div class="overview-change-item left-item">
 						<div class="left-item-top item-top">
 							<div class="overview-count-title item-top-top">场次</div>
-							<div class="overview-count item-top-bottom">{{
-								data['battleTypeInfo'][0]['shipInfo']['battleInfo']['battle'] }}</div>
+							<div class="overview-count item-top-bottom">{{ data['pvpInfo']['battles'] }}</div>
 						</div>
 						<div class="left-item-bottom item-bottom">
 							<div class="change-pr-title">
 								<div class="change-pr-title-left">PR</div>
-								<div class="change-pr-title-right">较上次</div>
+								<div class="change-pr-title-right">较上周</div>
 							</div>
-							<div class="change-pr">{{ '%+d' | format(data['dwpDataVO']['pr']) }}</div>
+							<div class="change-pr">暂不可用</div>
 						</div>
 					</div>
 					<div class="overview-change-item mid-item">
 						<div class="mid-item-top item-top">
 							<div class="overview-win-title item-top-top">胜率</div>
-							<div class="overview-win item-top-bottom"
-								style="color: {{ data['pvp']['winsData']['color'] }}">{{ data['pvp']['wins'] }}%</div>
+							<div class="overview-win item-top-bottom" style="color: {{ data['pvpInfo']['winsData']['color'] }}">{{ data['pvpInfo']['wins'] }}%</div>
 						</div>
 						<div class="mid-item-bottom item-bottom">
 							<div class="change-avgdmg-box bottom-mini-item-left">
 								<div class="mini-item-top">场均</div>
-								<div class="mini-item-bottom change-avgdmg">{{ '%+d' |
-									format(data['dwpDataVO']['damage']) }}</div>
+								<div class="mini-item-bottom change-avgdmg">暂不可用</div>
 							</div>
 							<div class="change-win-box bottom-mini-item-right">
 								<div class="mini-item-top">胜率</div>
-								<div class="mini-item-bottom change-win">{{ '%+.2f' | format(data['dwpDataVO']['wins'])
-									}}%</div>
+								<div class="mini-item-bottom change-win">暂不可用</div>
 							</div>
 						</div>
 					</div>
 					<div class="overview-change-item right-item">
 						<div class="right-item-top item-top">
 							<div class="overview-avgdmg-title item-top-top">场均</div>
-							<div class="overview-avgdmg item-top-bottom"
-								style="color: {{ data['pvp']['damageData']['color'] }};">{{ data['pvp']['damage'] }}
-							</div>
+							<div class="overview-avgdmg item-top-bottom" style="color: {{ data['pvpInfo']['damageData']['color'] }};">{{ data['pvpInfo']['damage'] }}</div>
 						</div>
 						<div class="right-item-bottom item-bottom">
 							<div class="overview-kd-box bottom-mini-item-left">
 								<div class="mini-item-top">击杀</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvp']['frags']) }}</div>
+								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvpInfo']['frags']) }}</div>
 							</div>
 							<div class="overview-hit-box bottom-mini-item-right">
 								<div class="mini-item-top">命中</div>
-								<div class="mini-item-bottom">{{ '%.2f' | format(data['pvp']['hit']) }}%</div>
+								<div class="mini-item-bottom">{{ data['pvpInfo']['hit'] }}%</div>
 							</div>
 						</div>
 					</div>
 				</div>
-
-				<div class="ship-data-header">船只数据</div>
-
-				<div class="ship-data-body">
-					<div class="ship-data-col ship-data-table-header">
-						<div class="ship-data-col-item">类型</div>
-						<div class="ship-data-col-item">场次</div>
-						<div class="ship-data-col-item">胜率</div>
-						<div class="ship-data-col-item">PR</div>
-						<div class="ship-data-col-item">场均</div>
-						<div class="ship-data-col-item">命中</div>
-					</div>
-
-					{% if data['type']['Battleship']['battles'] %}
-					<div class="ship-data-col">
-						<div class="ship-data-col-item ship-data-type">战列舰</div>
-						<div class="ship-data-col-item">{{ data['type']['Battleship']['battles'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Battleship']['winsData']['color'] }};">{{
-							data['type']['Battleship']['wins'] }}%</div>
-						<div class="ship-data-col-item" style="color: {{ data['type']['Battleship']['pr']['color'] }};">
-							{{ data['type']['Battleship']['pr']['value'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Battleship']['damageData']['color'] }};">{{
-							data['type']['Battleship']['damage'] }}</div>
-						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Battleship']['hit']) }}%</div>
-					</div>
-					{% endif %}
-
-					{% if data['type']['Cruiser']['battles'] %}
-					<div class="ship-data-col">
-						<div class="ship-data-col-item ship-data-type">巡洋舰</div>
-						<div class="ship-data-col-item">{{ data['type']['Cruiser']['battles'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Cruiser']['winsData']['color'] }};">{{
-							data['type']['Cruiser']['wins'] }}%</div>
-						<div class="ship-data-col-item" style="color: {{ data['type']['Cruiser']['pr']['color'] }};">{{
-							data['type']['Cruiser']['pr']['value'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Cruiser']['damageData']['color'] }};">{{
-							data['type']['Cruiser']['damage'] }}</div>
-						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Cruiser']['hit']) }}%</div>
-					</div>
-					{% endif %}
-
-
-					{% if data['type']['Destroyer']['battles'] %}
-					<div class="ship-data-col">
-						<div class="ship-data-col-item ship-data-type">驱逐舰</div>
-						<div class="ship-data-col-item">{{ data['type']['Destroyer']['battles'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Destroyer']['winsData']['color'] }};">{{
-							data['type']['Destroyer']['wins'] }}%</div>
-						<div class="ship-data-col-item" style="color: {{ data['type']['Destroyer']['pr']['color'] }};">
-							{{ data['type']['Destroyer']['pr']['value'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Destroyer']['damageData']['color'] }};">{{
-							data['type']['Destroyer']['damage'] }}</div>
-						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Destroyer']['hit']) }}%</div>
-					</div>
-					{% endif %}
-
-					{% if data['type']['AirCarrier']['battles'] %}
-					<div class="ship-data-col">
-						<div class="ship-data-col-item ship-data-type">航空母舰</div>
-						<div class="ship-data-col-item">{{ data['type']['AirCarrier']['battles'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['AirCarrier']['winsData']['color'] }};">{{
-							data['type']['AirCarrier']['wins'] }}%</div>
-						<div class="ship-data-col-item" style="color: {{ data['type']['AirCarrier']['pr']['color'] }};">
-							{{ data['type']['AirCarrier']['pr']['value'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['AirCarrier']['damageData']['color'] }};">{{
-							data['type']['AirCarrier']['damage'] }}</div>
-						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['AirCarrier']['hit']) }}%</div>
-					</div>
-					{% endif %}
-
-					{% if data['type']['Submarine']['battles'] %}
-					<div class="ship-data-col">
-						<div class="ship-data-col-item ship-data-type">潜艇</div>
-						<div class="ship-data-col-item">{{ data['type']['Submarine']['battles'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Submarine']['winsData']['color'] }};">{{
-							data['type']['Submarine']['wins'] }}%</div>
-						<div class="ship-data-col-item" style="color: {{ data['type']['Submarine']['pr']['color'] }};">
-							{{ data['type']['Submarine']['pr']['value'] }}</div>
-						<div class="ship-data-col-item"
-							style="color: {{ data['type']['Submarine']['damageData']['color'] }};">{{
-							data['type']['Submarine']['damage'] }}</div>
-						<div class="ship-data-col-item">{{ '%.2f' | format (data['type']['Submarine']['hit']) }}%</div>
-					</div>
-					{% endif %}
-
-				</div>
+				{% endif %}
 
 				<div class="information-header">总体战绩</div>
 
 				<div class="information-body">
 					<div class="information-col information-table-header">
 						<div class="information-col-item">类型</div>
 						<div class="information-col-item">场次</div>
 						<div class="information-col-item">胜率</div>
 						<div class="information-col-item">PR</div>
 						<div class="information-col-item">场均</div>
 						<div class="information-col-item">击杀</div>
 					</div>
-
-					{% if data['pvpSolo']['battles'] %}
+					
+					{% if data['pvpSoloInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">单野</div>
-						<div class="information-col-item">{{ data['pvpSolo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpSolo']['winsData']['color'] }};">{{
-							data['pvpSolo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['pvpSolo']['pr']['color'] }};">{{
-							data['pvpSolo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpSolo']['damageData']['color'] }};">
-							{{ data['pvpSolo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['pvpSolo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['pvpSoloInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['winsData']['color'] }};">{{ data['pvpSoloInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['pr']['color'] }};">{{ data['pvpSoloInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpSoloInfo']['damageData']['color'] }};">{{ data['pvpSoloInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpSoloInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
-					{% if data['pvpTwo']['battles'], %}
+					{% if data['pvpTwoInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">自行车</div>
-						<div class="information-col-item">{{ data['pvpTwo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpTwo']['winsData']['color'] }};">{{
-							data['pvpTwo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['pvpTwo']['pr']['color'] }};">{{
-							data['pvpTwo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpTwo']['damageData']['color'] }};">{{
-							data['pvpTwo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['pvpTwo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['pvpTwoInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['winsData']['color'] }};">{{ data['pvpTwoInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['pr']['color'] }};">{{ data['pvpTwoInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpTwoInfo']['damageData']['color'] }};">{{ data['pvpTwoInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpTwoInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
-					{% if data['pvpThree']['battles'] %}
+
+					{% if data['pvpThreeInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">三轮车</div>
-						<div class="information-col-item">{{ data['pvpThree']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpThree']['winsData']['color'] }};">{{
-							data['pvpThree']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['pvpThree']['pr']['color'] }};">{{
-							data['pvpThree']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['pvpThree']['damageData']['color'] }};">
-							{{ data['pvpThree']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['pvpThree']['frags']) }}</div>
+						<div class="information-col-item">{{ data['pvpThreeInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['winsData']['color'] }};">{{ data['pvpThreeInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['pr']['color'] }};">{{ data['pvpThreeInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['pvpThreeInfo']['damageData']['color'] }};">{{ data['pvpThreeInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['pvpThreeInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
-					{% if data['rankSolo']['battles'] %}
+
+					{% if data['rankInfo']['battles'] %}
 					<div class="information-col">
 						<div class="information-col-item information-type">排位</div>
-						<div class="information-col-item">{{ data['rankSolo']['battles'] }}</div>
-						<div class="information-col-item" style="color: {{ data['rankSolo']['winsData']['color'] }};">{{
-							data['rankSolo']['wins'] }}%</div>
-						<div class="information-col-item" style="color: {{ data['rankSolo']['pr']['color'] }};">{{
-							data['rankSolo']['pr']['value'] }}</div>
-						<div class="information-col-item" style="color: {{ data['rankSolo']['damageData']['color'] }};">
-							{{ data['rankSolo']['damage'] }}</div>
-						<div class="information-col-item">{{ '%.2f' | format(data['rankSolo']['frags']) }}</div>
+						<div class="information-col-item">{{ data['rankInfo']['battles'] }}</div>
+						<div class="information-col-item" style="color: {{ data['rankInfo']['winsData']['color'] }};">{{ data['rankInfo']['wins'] }}%</div>
+						<div class="information-col-item" style="color: {{ data['rankInfo']['pr']['color'] }};">{{ data['rankInfo']['pr']['value'] }}</div>
+						<div class="information-col-item" style="color: {{ data['rankInfo']['damageData']['color'] }};">{{ data['rankInfo']['damage'] }}</div>
+						<div class="information-col-item">{{ '%.2f' | format(data['rankInfo']['frags']) }}</div>
 					</div>
 					{% endif %}
 
 				</div>
 
-				<div class="chart-box">
-					<div class="chart-bar"></div>
-					<div class="chart-pie"></div>
-				</div>
+				<div class="day-header">每日战绩</div>
+
+				<div class="day-body">
+					<div class="day-table-header">
+						<div class="day-col-item">类型</div>
+						<div class="day-col-item">场次</div>
+						<div class="day-col-item">胜率</div>
+						<div class="day-col-item">PR</div>
+						<div class="day-col-item">场均</div>
+						<div class="day-col-item">击杀</div>
+					</div>
+
+
+						<div class="data-item">
+							{% for eachShipData in data['shipData'] %}
+							    {% if eachShipData['shipInfo']['battles'] or eachShipData['rankSolo']['battles'] %}
+								<div class="date">{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData['recordDateTime']/1000)))) }}</div>
+									{% for each in eachShipData %}
+										{% for index,value in enumerate(['shipSolo','shipTwo','shipThree','rankSolo']) %}
+											{% if each|string == value and eachShipData[each]['battles'] %}
+											<div class="day-data">
+												<div class="day-col">
+													<div class="day-col-item" style="color: #606266;;">{{ ['单野','自行车','三轮车','排位'][index] }}</div>
+													<div class="day-col-item">{{ eachShipData[each]['battles'] }}</div>
+													<div class="day-col-item" style="color: {{ eachShipData[each]['winsData']['color'] }};">{{ eachShipData[each]['wins'] }}%</div>
+													<div class="day-col-item" style="color: {{ eachShipData[each]['pr']['color'] }};">{{ eachShipData[each]['pr']['value'] }}</div>
+													<div class="day-col-item" style="color: {{ eachShipData[each]['damageData']['color'] }};">{{ eachShipData[each]['damage'] }}</div>
+													<div class="day-col-item">{{ '%.2f' | format(eachShipData[each]['frags']) }}</div>
+												</div>
+											</div>
+											{% endif %}
+										{% endfor %}
+									{% endfor %}
+								{% endif %}
+							{% endfor %}
+						</div>
+
+					<div class="footer">
+						<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
+						<p>https://github.com/benx1n/HikariBot</p>
+						<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
+						<p>Design By 冷眠 H5 Converted By C1ystal</p>
+						<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
+					</div>
 
-				<div class="footer">
-					<p>©西行寺雨季&nbsp;&nbsp;©本心</p>
-					<p>https://github.com/benx1n/HikariBot</p>
-					<p>QQ频道搜索”yuyuko”即可使用稳定的腾讯官方机器人~</p>
-					<p>Design By 冷眠 H5 Converted By C1ystal</p>
-					<p>赞助鸣谢：科长、男人们的定远号、海上最速暴毙传说</p>
 				</div>
 
+
+
 			</div>
 		</div>
-	</div>
-</body>
-{% if template_path and template_path/"echarts.js" %}
-<script src="file:\\{{template_path}}/echarts.js"></script>
-{% else %}
-<script src="https://cdn.jsdelivr.net/npm/echarts@5.3.3/dist/echarts.js"></script>
-{% endif %}
-<script>
-	window.onload = function () {
-		drawBarChart();
-		drawPieChart();
-	};
-
-	function drawBarChart() {
-		var barChart = echarts.init(document.querySelector('.chart-bar'));
-		var barOption = {
-			animation: false,
-			tooltip: {},
-			label: {
-				position: 'top',
-				show: true,
-				fontSize: '15',
-				color: '#303133',
-			},
-			xAxis: {
-				data: ['I', 'II', 'III', 'IV', 'V', 'VI', 'VII', 'VIII', 'IX', 'X', '★'],
-				axisLabel: {
-					align: 'center',
-					fontSize: '20',
-				}
-			},
-			yAxis: {
-				axisLabel: {
-					align: 'center',
-					fontSize: '20',
-				}
-			},
-			series: [{
-				name: '场次',
-				type: 'bar',
-				data: [
-					{{ data['battleCountAll']['1'] }},
-			{{ data['battleCountAll']['2'] }},
-			{{ data['battleCountAll']['3'] }
-	},
-	{ { data['battleCountAll']['4'] } },
-	{ { data['battleCountAll']['5'] } },
-	{ { data['battleCountAll']['6'] } },
-	{ { data['battleCountAll']['7'] } },
-	{ { data['battleCountAll']['8'] } },
-	{ { data['battleCountAll']['9'] } },
-	{ { data['battleCountAll']['10'] } },
-	{ { data['battleCountAll']['11'] } },
-					],
-	itemStyle: {
-		color: '#D6ECFB40',
-			borderWidth: 1,
-				borderType: 'solid',
-					borderColor: '#9FB8FF',
-						shadowColor: '#9FB8FF',
-							shadowBlur: 3
-	},
-				}]
-			};
-
-	barChart.setOption(barOption);
-		}
-
-	function drawPieChart() {
-		var pieChart = echarts.init(document.querySelector('.chart-pie'));
-		var pieOption = {
-			animation: false,
-			tooltip: {},
-			color: ["#FBE5D6", "#E2F0D9", "#F2E2E2", "#DAE3F3", "#D9FFFF"],
-			series: [
-				{
-					name: this.title,
-					type: 'pie',
-					selectedMode: 'single',
-					radius: ['30%', '80%'],
-					clockwise: false,
-					itemStyle: {
-						borderWidth: 5,
-						borderColor: '#F2F2F2'
-					},
-					label: {
-						position: 'inside',
-						formatter: '{b}\n{d}%',
-						fontSize: 20,
-						fontWeight: 'bold',
-					},
-					data: [
-						{ value: {{ data['type']['Battleship']['battles'] }}, name: 'BB' },
-			{ value: {{ data['type']['Cruiser']['battles'] }
-	}, name: 'CA' },
-	{ value: { { data['type']['Destroyer']['battles'] } }, name: 'DD' },
-	{ value: { { data['type']['AirCarrier']['battles'] } }, name: 'CV' },
-	{ value: { { data['type']['Submarine']['battles'] } }, name: 'SS' }
-			        ]
-			    }],
-	graphic: {
-		elements: [{
-			type: 'text',
-			left: 'center',
-			top: 'center',
-			style: {
-				text: '舰船\n场次',
-				fontSize: 35,
-				textAlign: 'center',
-				width: 30,
-				height: 30,
-				fill: 'darkgray'
-			}
-		}]
-	}
-			};
-
-	pieChart.setOption(pieOption);
-		}
-</script>
-
-<script>
-	// PR条颜色动态变化
-	let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
-	let pr_number = document.querySelector('.pr-number').innerText;
-	pr_number = parseInt(pr_number);
-	if (pr_number == 0) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#828282";
-		document.querySelector(".pr-text").innerText = "暂无数据";
-	} else if (pr_number < 750) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
-		document.querySelector(".pr-text").innerText = "还需努力";
-	} else if (pr_number < 1100) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
-		document.querySelector(".pr-text").innerText = "低于平均";
-	} else if (pr_number < 1350) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
-		document.querySelector(".pr-text").innerText = "平均水平";
-		document.querySelector(".pr-number").style.color = "#303133";
-	} else if (pr_number < 1550) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
-		document.querySelector(".pr-text").innerText = "好";
-	} else if (pr_number < 1750) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
-		document.querySelector(".pr-text").innerText = "很好";
-	} else if (pr_number < 2100) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
-		document.querySelector(".pr-text").innerText = "非常好";
-	} else if (pr_number < 2450) {
-		document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
-		document.querySelector(".pr-text").innerText = "大佬水平";
-	} else {
-		document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
-		document.querySelector(".pr-text").innerText = "神佬水平";
-		pr_number = 2450; //防止pr条溢出
-	}
-
-	if (pr_number < 220 && pr_number > 0) {
-		pr_number = 220; //防止pr过低导致圆角异常
-	}
-	// PR条动态长度
-	let width = bar_bg_width * (pr_number / 2450);
-	document.querySelector('.pr-bar').style.width = width + "px";
-</script>
-
-<script>
-	// 服务器字体颜色自动填充
-	let server_name = document.querySelector(".server").innerText;
-	if (server_name == "亚服") {
-		document.querySelector(".server").style.color = "#92D050";
-	} else if (server_name == "国服") {
-		document.querySelector(".server").style.color = "#BF9000";
-	} else if (server_name == "欧服") {
-		document.querySelector(".server").style.color = "#009664";
-	} else if (server_name == "美服") {
-		document.querySelector(".server").style.color = "#6872C4";
-	} else if (server_name == "俄服") {
-		document.querySelector(".server").style.color = "#FF0000";
-	}
-</script>
-
-<script>
-	// 数据变化动态颜色填充
-	let change_avgdmg = document.querySelector(".change-avgdmg").innerText;
-	change_avgdmg = parseInt(change_avgdmg);
-
-	let change_win = document.querySelector(".change-win").innerText;
-	change_win = change_win.split("%", 1);
-	change_win = parseFloat(change_win);
-
-	let change_pr = document.querySelector(".change-pr").innerText;
-	change_pr = parseInt(change_pr);
-
-	if (change_avgdmg > 0) {
-		document.querySelector(".change-avgdmg").style.color = "#70AD47";
-	} else {
-		document.querySelector(".change-avgdmg").style.color = "#FF0000";
-	}
-
-	if (change_win > 0) {
-		document.querySelector(".change-win").style.color = "#70AD47";
-	} else {
-		document.querySelector(".change-win").style.color = "#FF0000";
-	}
-
-	if (change_pr > 0) {
-		document.querySelector(".change-pr").style.color = "#70AD47";
-	} else {
-		document.querySelector(".change-pr").style.color = "#FF0000";
-	}
-</script>
-
-<script>
-	let arr_ship_data = document.getElementsByClassName('ship-data-col');
-	for (let i = 0; i < arr_ship_data.length; i++) {
-		if (i % 2 != 0 && i == (arr_ship_data.length - 1)) {
-			arr_ship_data[i].style.backgroundColor = "#E4E4E4";
-			arr_ship_data[i].style.borderBottomLeftRadius = "16px";
-			arr_ship_data[i].style.borderBottomRightRadius = "16px";
-		} else if (i % 2 != 0) {
-			arr_ship_data[i].style.backgroundColor = "#E4E4E4";
-		}
-	}
-</script>
-
-<script>
-	let arr_information = document.getElementsByClassName('information-col');
-	for (let i = 0; i < arr_information.length; i++) {
-		if (i % 2 != 0 && i == (arr_information.length - 1)) {
-			arr_information[i].style.backgroundColor = "#E4E4E4";
-			arr_information[i].style.borderBottomLeftRadius = "16px";
-			arr_information[i].style.borderBottomRightRadius = "16px";
-		} else if (i % 2 != 0) {
-			arr_information[i].style.backgroundColor = "#E4E4E4";
+	</body>
+	<script>
+		// PR条颜色动态变化
+		let bar_bg_width = document.querySelector('.pr-bar-bg').clientWidth;
+		let pr_number = document.querySelector('.pr-number').innerText;
+		pr_number = parseInt(pr_number);
+		if (pr_number == 0) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#828282";
+			document.querySelector(".pr-text").innerText = "暂无数据";
+		} else if (pr_number < 750) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#F44336";
+			document.querySelector(".pr-text").innerText = "还需努力";
+		} else if (pr_number < 1100) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#FF9800";
+			document.querySelector(".pr-text").innerText = "低于平均";
+		} else if (pr_number < 1350) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#FFC107";
+			document.querySelector(".pr-text").innerText = "平均水平";
+			document.querySelector(".pr-number").style.color = "#303133";
+		} else if (pr_number < 1550) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#8BC34A";
+			document.querySelector(".pr-text").innerText = "好";
+		} else if (pr_number < 1750) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#4CAF50";
+			document.querySelector(".pr-text").innerText = "很好";
+		} else if (pr_number < 2100) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#00BCD4";
+			document.querySelector(".pr-text").innerText = "非常好";
+		} else if (pr_number < 2450) {
+			document.querySelector(".pr-bar").style.backgroundColor = "#9C27B0";
+			document.querySelector(".pr-text").innerText = "大佬水平";
+		} else {
+			document.querySelector(".pr-bar").style.backgroundColor = "#673AB7";
+			document.querySelector(".pr-text").innerText = "神佬水平";
+			pr_number = 2450; //防止pr条溢出
 		}
-	}
-</script>
 
-</html>
+		if (pr_number < 220 && pr_number > 0) {
+			pr_number = 220; //防止pr过低导致圆角异常
+		}
+		// PR条动态长度
+		let width = bar_bg_width * (pr_number / 2450);
+		document.querySelector('.pr-bar').style.width = width + "px";
+	</script>
+
+	<script>
+		// 服务器字体颜色自动填充
+		let server_name = document.querySelector(".server").innerText;
+		if (server_name == "亚服") {
+			document.querySelector(".server").style.color = "#92D050";
+		} else if (server_name == "国服") {
+			document.querySelector(".server").style.color = "#BF9000";
+		} else if (server_name == "欧服") {
+			document.querySelector(".server").style.color = "#009664";
+		} else if (server_name == "美服") {
+			document.querySelector(".server").style.color = "#6872C4";
+		} else if (server_name == "俄服") {
+			document.querySelector(".server").style.color = "#FF0000";
+		}
+	</script>
+
+	<script>
+		// 数据变化动态颜色填充
+		let change_avgdmg = document.querySelector(".change-avgdmg").innerText;
+		change_avgdmg = parseInt(change_avgdmg);
+
+		let change_win = document.querySelector(".change-win").innerText;
+		change_win = change_win.split("%", 1);
+		change_win = parseFloat(change_win);
+
+		let change_pr = document.querySelector(".change-pr").innerText;
+		change_pr = parseInt(change_pr);
+
+		if (change_avgdmg > 0) {
+			document.querySelector(".change-avgdmg").style.color = "#70AD47";
+		} else {
+			document.querySelector(".change-avgdmg").style.color = "#FF0000";
+		}
+
+		if (change_win > 0) {
+			document.querySelector(".change-win").style.color = "#70AD47";
+		} else {
+			document.querySelector(".change-win").style.color = "#FF0000";
+		}
+
+		if (change_pr > 0) {
+			document.querySelector(".change-pr").style.color = "#70AD47";
+		} else {
+			document.querySelector(".change-pr").style.color = "#FF0000";
+		}
+	</script>
+
+	<script>
+		let ship_level = document.querySelector(".ship-level").innerText;
+		let level_number = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"];
+		let level_roma = ["I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX", "X", "★"];
+		let ship_level_roma = level_roma[level_number.indexOf(ship_level)]
+		document.querySelector(".ship-level").innerText = ship_level_roma;
+	</script>
+
+	<script>
+		let arr_information = document.getElementsByClassName('information-col');
+		for (let i = 0; i < arr_information.length; i++) {
+			if (i % 2 != 0 && i == (arr_information.length - 1)) {
+				arr_information[i].style.backgroundColor = "#E4E4E4";
+				arr_information[i].style.borderBottomLeftRadius = "16px";
+				arr_information[i].style.borderBottomRightRadius = "16px";
+			} else if (i % 2 != 0) {
+				arr_information[i].style.backgroundColor = "#E4E4E4";
+			}
+		}
+	</script>
+</html>
```

#### html2text {}

```diff
@@ -1,112 +1,117 @@
-{% if data['userInfo']['clanInfo']['tag'] %}
-[{{ data['userInfo']['clanInfo']['tag'] }}]
+{% if data['clanInfo']['tag'] %}
+[{{ data['clanInfo']['tag'] }}]
 {% endif %}
-{{ data['userInfo']['userName'] }}
-{{ data['userInfo']['server'] }}
-{{ data['prInfo']['value'] }}    
-æåæææ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs
-(data['battleTypeInfo'][0]['shipInfo']['lastBattleTime']))) }}
+{{ data['userName'] }}
+{{ data['serverName'] }}
+{% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+{{ data['shipData'][0]['shipInfo']['shipInfo']['level'] }}
+{% else %}
+{{ data['shipData'][0]['rankSolo']['shipInfo']['level'] }}
+{% endif %} {% if data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] %}
+{{ data['shipData'][0]['shipInfo']['shipInfo']['nameCn'] }}
+{% else %}
+{{ data['shipData'][0]['rankSolo']['shipInfo']['nameCn'] }}
+{% endif %}
+'shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data
+['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://
+hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_destroyer.png" {% elif data['shipData'][0]['shipInfo']['shipInfo']
+['shipType'] == 'Cruiser' or data['shipData'][0]['rankSolo']['shipInfo']
+['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png" {% elif data
+['shipData'][0]['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data
+['shipData'][0]['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https:/
+/hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_battleship.png" {% elif data['shipData'][0]['shipInfo']['shipInfo']
+['shipType'] == 'AirCarrier' or data['shipData'][0]['rankSolo']['shipInfo']
+['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-
+shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png" {% else %}
+"https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
+icon_sunk_submarine.png" {% endif %} />
+{% if data['pvpInfo']['pr']['color'] and data['pvpInfo']['pr']['color'] !=
+'#828282' %} {{ data['pvpInfo']['pr']['value'] }}      {% else %} {{ data
+['rankInfo']['pr']['value'] }}      {% endif %}
+è®°å½æ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M',time.localtime(int(abs(data
+['shipData'][0]['recordDateTime']/1000)))) }}â{{ time.strftime('%Y-%m-%d %H:
+%M',time.localtime(time.time())) }}
+{% if data['pvpInfo']['battles'] %}
 åºæ¬¡
-{{ data['battleTypeInfo'][0]['shipInfo']['battleInfo']['battle'] }}
+{{ data['pvpInfo']['battles'] }}
 PR
-è¾ä¸æ¬¡
-{{ '%+d' | format(data['dwpDataVO']['pr']) }}
+è¾ä¸å¨
+æä¸å¯ç¨
 èç
-{{ data['pvp']['wins'] }}%
+{{ data['pvpInfo']['wins'] }}%
 åºå
-{{ '%+d' | format(data['dwpDataVO']['damage']) }}
+æä¸å¯ç¨
 èç
-{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}%
+æä¸å¯ç¨
 åºå
-{{ data['pvp']['damage'] }}
+{{ data['pvpInfo']['damage'] }}
 å»æ
-{{ '%.2f' | format(data['pvp']['frags']) }}
-å½ä¸­
-{{ '%.2f' | format(data['pvp']['hit']) }}%
-è¹åªæ°æ®
-ç±»å
-åºæ¬¡
-èç
-PR
-åºå
+{{ '%.2f' | format(data['pvpInfo']['frags']) }}
 å½ä¸­
-{% if data['type']['Battleship']['battles'] %}
-æåè°
-{{ data['type']['Battleship']['battles'] }}
-{{ data['type']['Battleship']['wins'] }}%
-{{ data['type']['Battleship']['pr']['value'] }}
-{{ data['type']['Battleship']['damage'] }}
-{{ '%.2f' | format (data['type']['Battleship']['hit']) }}%
-{% endif %} {% if data['type']['Cruiser']['battles'] %}
-å·¡æ´è°
-{{ data['type']['Cruiser']['battles'] }}
-{{ data['type']['Cruiser']['wins'] }}%
-{{ data['type']['Cruiser']['pr']['value'] }}
-{{ data['type']['Cruiser']['damage'] }}
-{{ '%.2f' | format (data['type']['Cruiser']['hit']) }}%
-{% endif %} {% if data['type']['Destroyer']['battles'] %}
-é©±éè°
-{{ data['type']['Destroyer']['battles'] }}
-{{ data['type']['Destroyer']['wins'] }}%
-{{ data['type']['Destroyer']['pr']['value'] }}
-{{ data['type']['Destroyer']['damage'] }}
-{{ '%.2f' | format (data['type']['Destroyer']['hit']) }}%
-{% endif %} {% if data['type']['AirCarrier']['battles'] %}
-èªç©ºæ¯è°
-{{ data['type']['AirCarrier']['battles'] }}
-{{ data['type']['AirCarrier']['wins'] }}%
-{{ data['type']['AirCarrier']['pr']['value'] }}
-{{ data['type']['AirCarrier']['damage'] }}
-{{ '%.2f' | format (data['type']['AirCarrier']['hit']) }}%
-{% endif %} {% if data['type']['Submarine']['battles'] %}
-æ½è
-{{ data['type']['Submarine']['battles'] }}
-{{ data['type']['Submarine']['wins'] }}%
-{{ data['type']['Submarine']['pr']['value'] }}
-{{ data['type']['Submarine']['damage'] }}
-{{ '%.2f' | format (data['type']['Submarine']['hit']) }}%
+{{ data['pvpInfo']['hit'] }}%
 {% endif %}
 æ»ä½æç»©
 ç±»å
 åºæ¬¡
 èç
 PR
 åºå
 å»æ
-{% if data['pvpSolo']['battles'] %}
+{% if data['pvpSoloInfo']['battles'] %}
 åé
-{{ data['pvpSolo']['battles'] }}
-{{ data['pvpSolo']['wins'] }}%
-{{ data['pvpSolo']['pr']['value'] }}
-{{ data['pvpSolo']['damage'] }}
-{{ '%.2f' | format(data['pvpSolo']['frags']) }}
-{% endif %} {% if data['pvpTwo']['battles'], %}
+{{ data['pvpSoloInfo']['battles'] }}
+{{ data['pvpSoloInfo']['wins'] }}%
+{{ data['pvpSoloInfo']['pr']['value'] }}
+{{ data['pvpSoloInfo']['damage'] }}
+{{ '%.2f' | format(data['pvpSoloInfo']['frags']) }}
+{% endif %} {% if data['pvpTwoInfo']['battles'] %}
 èªè¡è½¦
-{{ data['pvpTwo']['battles'] }}
-{{ data['pvpTwo']['wins'] }}%
-{{ data['pvpTwo']['pr']['value'] }}
-{{ data['pvpTwo']['damage'] }}
-{{ '%.2f' | format(data['pvpTwo']['frags']) }}
-{% endif %} {% if data['pvpThree']['battles'] %}
+{{ data['pvpTwoInfo']['battles'] }}
+{{ data['pvpTwoInfo']['wins'] }}%
+{{ data['pvpTwoInfo']['pr']['value'] }}
+{{ data['pvpTwoInfo']['damage'] }}
+{{ '%.2f' | format(data['pvpTwoInfo']['frags']) }}
+{% endif %} {% if data['pvpThreeInfo']['battles'] %}
 ä¸è½®è½¦
-{{ data['pvpThree']['battles'] }}
-{{ data['pvpThree']['wins'] }}%
-{{ data['pvpThree']['pr']['value'] }}
-{{ data['pvpThree']['damage'] }}
-{{ '%.2f' | format(data['pvpThree']['frags']) }}
-{% endif %} {% if data['rankSolo']['battles'] %}
+{{ data['pvpThreeInfo']['battles'] }}
+{{ data['pvpThreeInfo']['wins'] }}%
+{{ data['pvpThreeInfo']['pr']['value'] }}
+{{ data['pvpThreeInfo']['damage'] }}
+{{ '%.2f' | format(data['pvpThreeInfo']['frags']) }}
+{% endif %} {% if data['rankInfo']['battles'] %}
 æä½
-{{ data['rankSolo']['battles'] }}
-{{ data['rankSolo']['wins'] }}%
-{{ data['rankSolo']['pr']['value'] }}
-{{ data['rankSolo']['damage'] }}
-{{ '%.2f' | format(data['rankSolo']['frags']) }}
+{{ data['rankInfo']['battles'] }}
+{{ data['rankInfo']['wins'] }}%
+{{ data['rankInfo']['pr']['value'] }}
+{{ data['rankInfo']['damage'] }}
+{{ '%.2f' | format(data['rankInfo']['frags']) }}
 {% endif %}
+æ¯æ¥æç»©
+ç±»å
+åºæ¬¡
+èç
+PR
+åºå
+å»æ
+{% for eachShipData in data['shipData'] %} {% if eachShipData['shipInfo']
+['battles'] or eachShipData['rankSolo']['battles'] %}
+{{ time.strftime('%Y-%m-%d',time.localtime(int(abs(eachShipData
+['recordDateTime']/1000)))) }}
+{% for each in eachShipData %} {% for index,value in enumerate(
+['shipSolo','shipTwo','shipThree','rankSolo']) %} {% if each|string == value
+and eachShipData[each]['battles'] %}
+{{ ['åé','èªè¡è½¦','ä¸è½®è½¦','æä½'][index] }}
+{{ eachShipData[each]['battles'] }}
+{{ eachShipData[each]['wins'] }}%
+{{ eachShipData[each]['pr']['value'] }}
+{{ eachShipData[each]['damage'] }}
+{{ '%.2f' | format(eachShipData[each]['frags']) }}
+{% endif %} {% endfor %} {% endfor %} {% endif %} {% endfor %}
 Â©è¥¿è¡å¯ºé¨å­£  Â©æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
 èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
-{% if template_path and template_path/"echarts.js" %}
- {% else %}
- {% endif %}
```

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.9.0/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-ship.html` & `hikari_core-0.9.0/hikari_core/Template/wws-ship.html`

 * *Files 26% similar despite different names*

```diff
@@ -109,16 +109,14 @@
 			height: 40px;
 			border-radius: 28px;
 			padding: 4px 20px;
 			background-color: #F2F2F2;
 		}
 
 		.last-time {
-			height: 60px;
-			line-height: 60px;
 			text-align: center;
 			color: #606266;
 		}
 
 		.pr {
 			display: flex;
 			height: 120px;
@@ -327,126 +325,110 @@
 	</style>
 	<body>
 		<div class="main-content">
 			<div class="page-box">
 				<div class="page-header">
 
 						<div class="clan-user-server">
-					 	{% if data['clanInfo']['tag'] %}
-							<div class="clan" style="color: {{ data['clanInfo']['colorRgb'] }};">
-								[{{ data['clanInfo']['tag'] }}]</div>
+					 	{% if data['userInfo']['clanInfo']['tag'] %}
+							<div class="clan" style="color: {{ data['userInfo']['clanInfo']['color'] }};">
+								[{{ data['userInfo']['clanInfo']['tag'] }}]</div>
 						{% endif %}
-							<div class="username">{{ data['userName'] }}</div>
+							<div class="username">{{ data['userInfo']['userName'] }}</div>
 							<div class="server">
 								<!-- 动态设置服务器字体颜色 -->
-								<div class="server-border">{{ data['serverName'] }}</div>
+								<div class="server-border">{{ data['userInfo']['serverCn'] }}</div>
 							</div>
 						</div>
 
 						<div class="ship-detail">
-							{% if data['shipInfo']['shipInfo']['nameCn'] %}
-							<div class="ship-level">{{ data['shipInfo']['shipInfo']['level'] }}</div>
-							{% else %}
-							<div class="ship-level">{{ data['rankSolo']['shipInfo']['level'] }}</div>
-							{% endif %}
-
-							{% if data['shipInfo']['shipInfo']['nameCn'] %}
-							<div class="ship-name">{{ data['shipInfo']['shipInfo']['nameCn'] }}</div>
-							{% else %}
-							<div class="ship-name">{{ data['rankSolo']['shipInfo']['nameCn'] }}</div>
-							{% endif %}
+							<div class="ship-level">{{ data['shipInfo']['level'] }}</div>
+							<div class="ship-name">{{ data['shipInfo']['nameCn'] }}</div>
 							<div class="ship-icon"><img
-									src={% if data['shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['rankSolo']['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
-									{% elif data['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['rankSolo']['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
-									{% elif data['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['rankSolo']['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
-									{% elif data['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['rankSolo']['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
+									src={% if data['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png"
+									{% elif data['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png"
+									{% elif data['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png"
+									{% elif data['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png"
 									{% else %} "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/icon_sunk_submarine.png"
 									{% endif %} /></div>
 						</div>
 					</div>
 
 					<div class="pr">
 						<!-- 动态设置长度及颜色，填写PR即可 -->
 						<div class="pr-bar-bg">
-							{% if data['shipInfo']['pr']['color'] and data['shipInfo']['pr']['color'] != '#828282' %}
-							<span class="pr-number">{{ data['shipInfo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
+							{% if data['typeInfo']['PVP']['prInfo']['color'] and data['typeInfo']['PVP']['prInfo']['color'] != '#828282' %}
+							<span class="pr-number">{{ data['typeInfo']['PVP']['prInfo']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
 									class="pr-text"></span></span>
 							{% else %}
-							<span class="pr-number">{{ data['rankSolo']['pr']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
+							<span class="pr-number">{{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }} &nbsp;&nbsp;&nbsp;&nbsp;<span
 									class="pr-text"></span></span>
 							{% endif %}
 							<div class="pr-bar"></div>
 						</div>
 					</div>
 					
 					<div class="last-time">
-						<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['shipInfo']['lastBattlesTime']))) }}</span>
+						<span>最后战斗时间：</span><span>{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs(data['typeInfo']['PVP']['battleInfo']['lastBattleTime']))) }}</span>
 					</div>
 					
 					{% if data['shipRank'] %}
 					<div class="ranking">
 						<div class="ranking_border"><span
 								style="color: #606266;">排名</span>&nbsp;&nbsp;<span>{{data['shipRank']}}</span>
 						</div>
 					</div>
 					{% endif %}
-					{% if data['rank'] != -1 %}
-					<div class="ranking">
-						<div class="ranking_border"><span
-								style="color: #606266;">排名</span>&nbsp;&nbsp;<span>{{data['rank']}}</span>
-						</div>
-					</div>
-					{% endif %}
 
 					<div class="data-change">
 						<div class="change-header">
 							<div class="change-header-item">场均</div>
 							<div class="change-header-item">胜率</div>
 							<div class="change-header-item">PR</div>
 						</div>
 						<div class="change-body">
 							<div class="change-body-item change-avgdmg">
-								{{ '%+d' | format(data['dwpDataVO']['damage']) }}</div>
-							<div class="change-body-item change-win">{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}
+								{{ '%+d' | format(data['dwpData']['damage']) }}</div>
+							<div class="change-body-item change-win">{{ '%+.2f' | format(data['dwpData']['wins']) }}
 							</div>
-							<div class="change-body-item change-pr">{{ '%+d' | format(data['dwpDataVO']['pr']) }}</div>
+							<div class="change-body-item change-pr">{{ '%+d' | format(data['dwpData']['pr']) }}</div>
 						</div>
 					</div>
 
 					<div class="ship-overview">
 						<div class="overview-col">
 							<div class="overview-item">
 								<div class="overview-item-title">场次</div>
-								<div class="overview-item-data">{{ data['shipInfo']['battles'] }}</div>
+								<div class="overview-item-data">{{ data['typeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}</div>
 							</div>
 							<div class="overview-item">
 								<div class="overview-item-title">胜率</div>
 								<div class="overview-item-data"
-									style="color: {{ data['shipInfo']['winsData']['color'] }};">
-									{{ data['shipInfo']['wins'] }}%</div>
+									style="color: {{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['winsData']['color'] }};">
+									{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%</div>
 							</div>
 							<div class="overview-item">
 								<div class="overview-item-title">场均</div>
 								<div class="overview-item-data"
-									style="color: {{ data['shipInfo']['damageData']['color'] }};">
-									{{ data['shipInfo']['damage'] }}</div>
+									style="color: {{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['damageData']['color'] }};">
+									{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}</div>
 							</div>
 						</div>
 						<div class="overview-col">
 							<div class="overview-item">
 								<div class="overview-item-title">经验</div>
-								<div class="overview-item-data">{{ data['shipInfo']['xp'] }}</div>
+								<div class="overview-item-data">{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['xp'] }}</div>
 							</div>
 							<div class="overview-item">
 								<div class="overview-item-title">击杀</div>
-								<div class="overview-item-data">{{ '%.2f' | format(data['shipInfo']['frags']) }}</div>
+								<div class="overview-item-data">{{ '%.2f' | format(data['typeInfo']['PVP']['battleInfo']['avgInfo']['frags']) }}</div>
 							</div>
 							<div class="overview-item">
 								<div class="overview-item-title">命中</div>
-								<div class="overview-item-data">{{ data['shipInfo']['hit'] }}%</div>
+								<div class="overview-item-data">{{ data['typeInfo']['PVP']['battleInfo']['hitRatioInfo']['ratioMain'] }}%</div>
 							</div>
 						</div>
 					</div>
 
 					<div class="information-header">
 						总体战绩
 					</div>
@@ -457,108 +439,108 @@
 							<div class="information-item">场次</div>
 							<div class="information-item">胜率</div>
 							<div class="information-item">PR</div>
 							<div class="information-item">场均</div>
 							<div class="information-item">击杀</div>
 						</div>
 
-						{% if data['shipSolo']['battles'] %}
+						{% if data['typeInfo']['PVP_SOLO']['battle'] %}
 						<div class="information-body-data">
 							<div class="information-item" style="color: #909399;">单野</div>
-							<div class="information-item">{{ data['shipSolo']['battles'] }}</div>
-							<div class="information-item" style="color: {{ data['shipSolo']['winsData']['color'] }};">
-								{{ data['shipSolo']['wins'] }}%</div>
-							<div class="information-item" style="color: {{ data['shipSolo']['pr']['color'] }};">
-								{{ data['shipSolo']['pr']['value'] }}</div>
+							<div class="information-item">{{ data['typeInfo']['PVP_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['PVP_SOLO']['prInfo']['color'] }};">
+								{{ data['typeInfo']['PVP_SOLO']['prInfo']['value'] }}</div>
 							<div class="information-item"
-								style="color: {{ data['shipSolo']['damageData']['color'] }};">
-								{{ data['shipSolo']['damage'] }}</div>
-							<div class="information-item">{{ '%.2f' | format(data['shipSolo']['frags']) }}</div>
+								style="color: {{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
 						</div>
 						{% endif %}
-						{% if data['shipTwo']['battles'] %}
+						{% if data['typeInfo']['PVP_DIV2']['battle'] %}
 						<div class="information-body-data">
 							<div class="information-item" style="color: #909399;">自行车</div>
-							<div class="information-item">{{ data['shipTwo']['battles'] }}</div>
-							<div class="information-item" style="color: {{ data['shipTwo']['winsData']['color'] }};">
-								{{ data['shipTwo']['wins'] }}%</div>
-							<div class="information-item" style="color: {{ data['shipTwo']['pr']['color'] }};">
-								{{ data['shipTwo']['pr']['value'] }}</div>
+							<div class="information-item">{{ data['typeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['PVP_DIV2']['prInfo']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV2']['prInfo']['value'] }}</div>
 							<div class="information-item"
-								style="color: {{ data['shipTwo']['damageData']['color'] }};">
-								{{ data['shipTwo']['damage'] }}</div>
-							<div class="information-item">{{ '%.2f' | format(data['shipTwo']['frags']) }}</div>
+								style="color: {{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['frags']) }}</div>
 						</div>
 						{% endif %}
-						{% if data['shipThree']['battles'] %}
+						{% if data['typeInfo']['PVP_DIV3']['battle'] %}
 						<div class="information-body-data">
 							<div class="information-item" style="color: #909399;">三轮车</div>
-							<div class="information-item">{{ data['shipThree']['battles'] }}</div>
-							<div class="information-item" style="color: {{ data['shipThree']['winsData']['color'] }};">
-								{{ data['shipThree']['wins'] }}%</div>
-							<div class="information-item" style="color: {{ data['shipThree']['pr']['color'] }};">
-								{{ data['shipThree']['pr']['value'] }}</div>
+							<div class="information-item">{{ data['typeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['PVP_DIV3']['prInfo']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV3']['prInfo']['value'] }}</div>
 							<div class="information-item"
-								style="color: {{ data['shipThree']['damageData']['color'] }};">
-								{{ data['shipThree']['damage'] }}</div>
-							<div class="information-item">{{ '%.2f' | format(data['shipThree']['frags']) }}</div>
+								style="color: {{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['frags']) }}</div>
 						</div>
 						{% endif %}
-						{% if data['rankSolo']['battles'] %}
+						{% if data['typeInfo']['RANK_SOLO']['battle'] %}
 						<div class="information-body-data">
 							<div class="information-item" style="color: #909399;">排位</div>
-							<div class="information-item">{{ data['rankSolo']['battles'] }}</div>
-							<div class="information-item" style="color: {{ data['rankSolo']['winsData']['color'] }};">
-								{{ data['rankSolo']['wins'] }}%</div>
-							<div class="information-item" style="color: {{ data['rankSolo']['pr']['color'] }};">
-								{{ data['rankSolo']['pr']['value'] }}</div>
+							<div class="information-item">{{ data['typeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}</div>
+							<div class="information-item" style="color: {{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['winsData']['color'] }};">
+								{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%</div>
+							<div class="information-item" style="color: {{  data['typeInfo']['RANK_SOLO']['prInfo']['color'] }};">
+								{{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }}</div>
 							<div class="information-item"
-								style="color: {{ data['rankSolo']['damageData']['color'] }};">
-								{{ data['rankSolo']['damage'] }}</div>
-							<div class="information-item">{{ '%.2f' | format(data['rankSolo']['frags']) }}</div>
+								style="color: {{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damageData']['color'] }};">
+								{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}</div>
+							<div class="information-item">{{ '%.2f' | format(data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['frags']) }}</div>
 						</div>
 						{% endif %}
 					</div>
 
 					<div class="ship-highest-header">
 						最高纪录
 					</div>
 
 					<div class="ship-highest-data">
 						<div class="high-col">
 							<div class="high-item">
 								<div class="high-item-top">最高伤害</div>
-								<div class="high-item-bottom">{{ data['shipInfo']['extensionDataInfo']['maxDamage'] }}
+								<div class="high-item-bottom">{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxDamageDealt']['value'] }}
 								</div>
 							</div>
 							<div class="high-item">
 								<div class="high-item-top">侦察伤害</div>
 								<div class="high-item-bottom">
-									{{ data['shipInfo']['extensionDataInfo']['maxDamageScouting'] }}</div>
+									{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxScoutingDamage']['value'] }}</div>
 							</div>
 							<div class="high-item">
 								<div class="high-item-top">最高潜在</div>
 								<div class="high-item-bottom">
-									{{ data['shipInfo']['extensionDataInfo']['maxTotalAgro'] }}</div>
+									{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxTotalAgro']['value'] }}</div>
 							</div>
 						</div>
 						<div class="high-col">
 							<div class="high-item">
 								<div class="high-item-top">经验</div>
-								<div class="high-item-bottom">{{ data['shipInfo']['extensionDataInfo']['maxXp'] }}</div>
+								<div class="high-item-bottom">{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxXp']['value'] }}</div>
 							</div>
 							<div class="high-item">
 								<div class="high-item-top">击杀</div>
-								<div class="high-item-bottom">{{ data['shipInfo']['extensionDataInfo']['maxFrags'] }}
+								<div class="high-item-bottom">{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxFrags']['value'] }}
 								</div>
 							</div>
 							<div class="high-item">
 								<div class="high-item-top">飞机击落</div>
 								<div class="high-item-bottom">
-									{{ data['shipInfo']['extensionDataInfo']['maxPlanesKilled'] }}</div>
+									{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxPlanesKilled']['value'] }}</div>
 							</div>
 						</div>
 					</div>
 
 					<div class="footer">
 						<p>© 西行寺雨季&nbsp;&nbsp;© 本心</p>
 						<p>https://github.com/benx1n/HikariBot</p>
```

#### html2text {}

```diff
@@ -1,110 +1,106 @@
-{% if data['clanInfo']['tag'] %}
-[{{ data['clanInfo']['tag'] }}]
+{% if data['userInfo']['clanInfo']['tag'] %}
+[{{ data['userInfo']['clanInfo']['tag'] }}]
 {% endif %}
-{{ data['userName'] }}
-{{ data['serverName'] }}
-{% if data['shipInfo']['shipInfo']['nameCn'] %}
-{{ data['shipInfo']['shipInfo']['level'] }}
-{% else %}
-{{ data['rankSolo']['shipInfo']['level'] }}
-{% endif %} {% if data['shipInfo']['shipInfo']['nameCn'] %}
-{{ data['shipInfo']['shipInfo']['nameCn'] }}
-{% else %}
-{{ data['rankSolo']['shipInfo']['nameCn'] }}
-{% endif %}
-'shipInfo']['shipInfo']['shipType'] == 'Destroyer' or data['rankSolo']
-['shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-
+{{ data['userInfo']['userName'] }}
+{{ data['userInfo']['serverCn'] }}
+{{ data['shipInfo']['level'] }}
+{{ data['shipInfo']['nameCn'] }}
+'shipInfo']['shipType'] == 'Destroyer' %} "https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_destroyer.png" {% elif data
-['shipInfo']['shipInfo']['shipType'] == 'Cruiser' or data['rankSolo']
 ['shipInfo']['shipType'] == 'Cruiser' %} "https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_cruiser.png" {% elif data
-['shipInfo']['shipInfo']['shipType'] == 'Battleship' or data['rankSolo']
 ['shipInfo']['shipType'] == 'Battleship' %} "https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_battleship.png" {% elif data
-['shipInfo']['shipInfo']['shipType'] == 'AirCarrier' or data['rankSolo']
 ['shipInfo']['shipType'] == 'AirCarrier' %} "https://hikari-resource.oss-cn-
 shanghai.aliyuncs.com/shipType_Icon/icon_sunk_aircarrier.png" {% else %}
 "https://hikari-resource.oss-cn-shanghai.aliyuncs.com/shipType_Icon/
 icon_sunk_submarine.png" {% endif %} />
-{% if data['shipInfo']['pr']['color'] and data['shipInfo']['pr']['color'] !=
-'#828282' %} {{ data['shipInfo']['pr']['value'] }}      {% else %} {{ data
-['rankSolo']['pr']['value'] }}      {% endif %}
+{% if data['typeInfo']['PVP']['prInfo']['color'] and data['typeInfo']['PVP']
+['prInfo']['color'] != '#828282' %} {{ data['typeInfo']['PVP']['prInfo']
+['value'] }}      {% else %} {{ data['typeInfo']['RANK_SOLO']['prInfo']
+['value'] }}      {% endif %}
 æåæææ¶é´ï¼{{ time.strftime('%Y-%m-%d %H:%M:%S',time.localtime(abs
-(data['shipInfo']['lastBattlesTime']))) }}
+(data['typeInfo']['PVP']['battleInfo']['lastBattleTime']))) }}
 {% if data['shipRank'] %}
 æå  {{data['shipRank']}}
-{% endif %} {% if data['rank'] != -1 %}
-æå  {{data['rank']}}
 {% endif %}
 åºå
 èç
 PR
-{{ '%+d' | format(data['dwpDataVO']['damage']) }}
-{{ '%+.2f' | format(data['dwpDataVO']['wins']) }}
-{{ '%+d' | format(data['dwpDataVO']['pr']) }}
+{{ '%+d' | format(data['dwpData']['damage']) }}
+{{ '%+.2f' | format(data['dwpData']['wins']) }}
+{{ '%+d' | format(data['dwpData']['pr']) }}
 åºæ¬¡
-{{ data['shipInfo']['battles'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['battleInfo']['battle'] }}
 èç
-{{ data['shipInfo']['wins'] }}%
+{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['win'] }}%
 åºå
-{{ data['shipInfo']['damage'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['damage'] }}
 ç»éª
-{{ data['shipInfo']['xp'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['avgInfo']['xp'] }}
 å»æ
-{{ '%.2f' | format(data['shipInfo']['frags']) }}
+{{ '%.2f' | format(data['typeInfo']['PVP']['battleInfo']['avgInfo']['frags'])
+}}
 å½ä¸­
-{{ data['shipInfo']['hit'] }}%
+{{ data['typeInfo']['PVP']['battleInfo']['hitRatioInfo']['ratioMain'] }}%
 æ»ä½æç»©
 ç±»å
 åºæ¬¡
 èç
 PR
 åºå
 å»æ
-{% if data['shipSolo']['battles'] %}
+{% if data['typeInfo']['PVP_SOLO']['battle'] %}
 åé
-{{ data['shipSolo']['battles'] }}
-{{ data['shipSolo']['wins'] }}%
-{{ data['shipSolo']['pr']['value'] }}
-{{ data['shipSolo']['damage'] }}
-{{ '%.2f' | format(data['shipSolo']['frags']) }}
-{% endif %} {% if data['shipTwo']['battles'] %}
+{{ data['typeInfo']['PVP_SOLO']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['PVP_SOLO']['prInfo']['value'] }}
+{{ data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['PVP_SOLO']['battleInfo']['avgInfo']
+['frags']) }}
+{% endif %} {% if data['typeInfo']['PVP_DIV2']['battle'] %}
 èªè¡è½¦
-{{ data['shipTwo']['battles'] }}
-{{ data['shipTwo']['wins'] }}%
-{{ data['shipTwo']['pr']['value'] }}
-{{ data['shipTwo']['damage'] }}
-{{ '%.2f' | format(data['shipTwo']['frags']) }}
-{% endif %} {% if data['shipThree']['battles'] %}
+{{ data['typeInfo']['PVP_DIV2']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['PVP_DIV2']['prInfo']['value'] }}
+{{ data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['PVP_DIV2']['battleInfo']['avgInfo']
+['frags']) }}
+{% endif %} {% if data['typeInfo']['PVP_DIV3']['battle'] %}
 ä¸è½®è½¦
-{{ data['shipThree']['battles'] }}
-{{ data['shipThree']['wins'] }}%
-{{ data['shipThree']['pr']['value'] }}
-{{ data['shipThree']['damage'] }}
-{{ '%.2f' | format(data['shipThree']['frags']) }}
-{% endif %} {% if data['rankSolo']['battles'] %}
+{{ data['typeInfo']['PVP_DIV3']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['PVP_DIV3']['prInfo']['value'] }}
+{{ data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['PVP_DIV3']['battleInfo']['avgInfo']
+['frags']) }}
+{% endif %} {% if data['typeInfo']['RANK_SOLO']['battle'] %}
 æä½
-{{ data['rankSolo']['battles'] }}
-{{ data['rankSolo']['wins'] }}%
-{{ data['rankSolo']['pr']['value'] }}
-{{ data['rankSolo']['damage'] }}
-{{ '%.2f' | format(data['rankSolo']['frags']) }}
+{{ data['typeInfo']['RANK_SOLO']['battleInfo']['battleInfo']['battle'] }}
+{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['win'] }}%
+{{ data['typeInfo']['RANK_SOLO']['prInfo']['value'] }}
+{{ data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']['damage'] }}
+{{ '%.2f' | format(data['typeInfo']['RANK_SOLO']['battleInfo']['avgInfo']
+['frags']) }}
 {% endif %}
 æé«çºªå½
 æé«ä¼¤å®³
-{{ data['shipInfo']['extensionDataInfo']['maxDamage'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxDamageDealt']['value']
+}}
 ä¾¦å¯ä¼¤å®³
-{{ data['shipInfo']['extensionDataInfo']['maxDamageScouting'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxScoutingDamage']
+['value'] }}
 æé«æ½å¨
-{{ data['shipInfo']['extensionDataInfo']['maxTotalAgro'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxTotalAgro']['value'] }}
 ç»éª
-{{ data['shipInfo']['extensionDataInfo']['maxXp'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxXp']['value'] }}
 å»æ
-{{ data['shipInfo']['extensionDataInfo']['maxFrags'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxFrags']['value'] }}
 é£æºå»è½
-{{ data['shipInfo']['extensionDataInfo']['maxPlanesKilled'] }}
+{{ data['typeInfo']['PVP']['battleInfo']['maxInfo']['maxPlanesKilled']['value']
+}}
 Â© è¥¿è¡å¯ºé¨å­£  Â© æ¬å¿
 https://github.com/benx1n/HikariBot
 QQé¢éæç´¢âyuyukoâå³å¯ä½¿ç¨ç¨³å®çè¾è®¯å®æ¹æºå¨äºº~
 Design By å·ç  H5 Converted By C1ystal
 èµå©é¸£è°¢ï¼ç§é¿ãç·äººä»¬çå®è¿å·ãæµ·ä¸æéæ´æ¯ä¼ è¯´
```

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-sx.html` & `hikari_core-0.9.0/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/Template/wws-unban.html` & `hikari_core-0.9.0/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/hikari_core/utils.py` & `hikari_core-0.9.0/hikari_core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,83 +13,83 @@
 from loguru import logger
 
 from .data_source import template_path
 
 
 def startup():
     try:
-        url = "https://benx1n.oss-cn-beijing.aliyuncs.com/template_Hikari_Latest/template.json"
+        url = 'https://benx1n.oss-cn-beijing.aliyuncs.com/template_Hikari_Latest/template.json'
         with httpx.Client() as client:
             resp = client.get(url, timeout=20)
             result = orjson.loads(resp.content)
             for each in result:
                 for name, url in each.items():
                     resp = client.get(url, timeout=20)
-                    with open(template_path / name, "wb+") as file:
+                    with open(template_path / name, 'wb+') as file:
                         file.write(resp.content)
-        print(f"success {time.time()}")
+        print(f'success {time.time()}')
     except Exception:
         logger.error(traceback.format_exc())
         return
 
 
-async def match_keywords(match_list, Lists) -> Tuple[Optional[str], List]:
+async def match_keywords(match_list, lists) -> Tuple[Optional[str], List]:
     """字段列表匹配(仅匹配单个元素)
 
     Args:
         match_list (List): 待匹配列表
-        Lists (List): 匹配字符列表
+        lists (List): 匹配字符列表
 
     Returns:
         match_keywards (str/None):匹配到的字段
         match_list (List): 去除匹配字符后的列表
     """
-    for List in Lists:
-        for kw in List.keywords:
+    for each in lists:
+        for kw in each.keywords:
             for match_kw in match_list:
                 if match_kw == kw or match_kw.upper() == kw.upper() or match_kw.lower() == kw.lower():
                     match_list.remove(match_kw)
-                    return List.match_keywords, match_list
+                    return each.match_keywords, match_list
     return None, match_list
 
 
-async def find_and_replace_keywords(match_list, Lists) -> Tuple[Optional[str], List]:
+async def find_and_replace_keywords(match_list, lists) -> Tuple[Optional[str], List]:
     """字段列表匹配(可匹配同元素内更小长度)
 
     Args:
         match_list (List): 待匹配列表
-        Lists (List): 匹配字符列表
+        lists (List): 匹配字符列表
 
     Returns:
         match_keywards (str/None):匹配到的字段
         match_list (List): 去除匹配字符后的列表
     """
-    for List in Lists:
-        for kw in List.keywords:
+    for each in lists:
+        for kw in each.keywords:
             for i, match_kw in enumerate(match_list):
                 if match_kw.find(kw) + 1:
-                    match_list[i] = str(match_kw).replace(kw, "")
-                    if match_list[i] == "":
-                        match_list.remove("")
-                    return List.match_keywords, match_list
+                    match_list[i] = str(match_kw).replace(kw, '')
+                    if not match_list[i]:
+                        match_list.remove('')
+                    return each.match_keywords, match_list
     return None, match_list
 
 
 def encode_gzip(bytes) -> str:
     """gzip压缩
 
     Args:
         bytes (bytes): 需要压缩的content
 
     Returns:
         str (str): 压缩后数据
     """
     buf = io.BytesIO(bytes)
     gf = gzip.GzipFile(fileobj=buf)
-    return gf.read().decode("utf-8")
+    return gf.read().decode('utf-8')
 
 
 class FreqLimiter:
     def __init__(self, default_cd_seconds):
         self.next_time = defaultdict(float)
         self.default_cd = default_cd_seconds
 
@@ -100,15 +100,15 @@
         self.next_time[key] = time.time() + (cd_time if cd_time > 0 else self.default_cd)
 
     def left_time(self, key) -> float:
         return self.next_time[key] - time.time()
 
 
 class DailyNumberLimiter:
-    tz = pytz.timezone("Asia/Shanghai")
+    tz = pytz.timezone('Asia/Shanghai')
 
     def __init__(self, max_num):
         self.today = -1
         self.count = defaultdict(int)
         self.max = max_num
 
     def check(self, key) -> bool:
@@ -125,20 +125,20 @@
     def increase(self, key, num=1):
         self.count[key] += num
 
     def reset(self, key):
         self.count[key] = 0
 
 
-async def download(url, path, proxy={}):
+async def download(url, path, proxy=None):
     async with httpx.AsyncClient(proxies=proxy) as client:
         resp = await client.get(url, timeout=None)
         content = resp.read()
-        content = content.replace(b"\n", b"\r\n")
-        with open(path, "wb") as f:
+        content = content.replace(b'\n', b'\r\n')
+        with open(path, 'wb') as f:
             f.write(content)
 
 
 async def byte2md5(bytes) -> str:
     """bytes转为md5
 
     Args:
```

### Comparing `hikari_core-0.1.6/LICENSE` & `hikari_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.1.6/setup.py` & `hikari_core-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,74 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['hikari_core', 'hikari_core.Html_Render', 'hikari_core.moudle']
+['hikari_core',
+ 'hikari_core.Html_Render',
+ 'hikari_core.game',
+ 'hikari_core.moudle']
 
 package_data = \
 {'': ['*'],
- 'hikari_core': ['Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/Chart.min.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
-                 'Template/chartjs-plugin-datalabels@1.0.0.js',
+ 'hikari_core': ['Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
+                 'Template/bind-list.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
                  'Template/select-ship.html',
-                 'Template/select-ship.html',
-                 'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
                  'Template/ship-rank.html',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/text-help.css',
-                 'Template/wws-ban.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
+                 'Template/text.html',
                  'Template/wws-ban.html',
                  'Template/wws-ban.html',
                  'Template/wws-ban.html',
                  'Template/wws-ban.html',
                  'Template/wws-ban.html',
                  'Template/wws-ban.html',
                  'Template/wws-ban.html',
@@ -106,16 +89,14 @@
                  'Template/wws-box-christmas.html',
                  'Template/wws-box-christmas.html',
                  'Template/wws-box-christmas.html',
                  'Template/wws-box-christmas.html',
                  'Template/wws-box-christmas.html',
                  'Template/wws-box-christmas.html',
                  'Template/wws-box-christmas.html',
-                 'Template/wws-box-christmas.html',
-                 'Template/wws-clan.html',
                  'Template/wws-clan.html',
                  'Template/wws-clan.html',
                  'Template/wws-clan.html',
                  'Template/wws-clan.html',
                  'Template/wws-clan.html',
                  'Template/wws-clan.html',
                  'Template/wws-clan.html',
@@ -136,31 +117,28 @@
                  'Template/wws-info-recent.html',
                  'Template/wws-info-recent.html',
                  'Template/wws-info-recent.html',
                  'Template/wws-info-recent.html',
                  'Template/wws-info-recent.html',
                  'Template/wws-info-recent.html',
                  'Template/wws-info-recent.html',
-                 'Template/wws-info-recent.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
                  'Template/wws-info.html',
-                 'Template/wws-info.html',
-                 'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
                  'Template/wws-personalRecord.html',
@@ -181,31 +159,28 @@
                  'Template/wws-ship-recent.html',
                  'Template/wws-ship-recent.html',
                  'Template/wws-ship-recent.html',
                  'Template/wws-ship-recent.html',
                  'Template/wws-ship-recent.html',
                  'Template/wws-ship-recent.html',
                  'Template/wws-ship-recent.html',
-                 'Template/wws-ship-recent.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
                  'Template/wws-ship.html',
-                 'Template/wws-ship.html',
-                 'Template/wws-sx.html',
                  'Template/wws-sx.html',
                  'Template/wws-sx.html',
                  'Template/wws-sx.html',
                  'Template/wws-sx.html',
                  'Template/wws-sx.html',
                  'Template/wws-sx.html',
                  'Template/wws-sx.html',
@@ -225,39 +200,39 @@
                  'Template/wws-unban.html',
                  'Template/wws-unban.html',
                  'Template/wws-unban.html',
                  'Template/wws-unban.html',
                  'Template/wws-unban.html',
                  'Template/wws-unban.html',
                  'Template/wws-unban.html',
-                 'Template/wws-unban.html',
                  'Template/wws-unban.html'],
  'hikari_core.Html_Render': ['templates/*']}
 
 install_requires = \
 ['APScheduler>=3.10.1,<4.0.0',
  'aiofiles>=0.8.0',
  'asyncio>=3.4.3,<4.0.0',
- 'beautifulsoup4>=4.11.1,<5.0.0',
+ 'beautifulsoup4>=4.12.2,<5.0.0',
  'httpx[http2]>=0.24.0',
  'jinja2>=3.0.0,<4.0.0',
+ 'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.17.2',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '0.1.6',
-    'description': '',
+    'version': '0.9.0',
+    'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/wows-yuyuko/Hikari-core',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

