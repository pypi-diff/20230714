# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.tar", last modified: Fri Jul 14 02:29:52 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.1.tar", last modified: Fri Jul 14 07:27:24 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    25588 2023-07-14 02:29:23.939546 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    14048 2023-07-10 03:47:58.215732 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    17924 2023-07-10 13:46:44.820439 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    37733 2023-07-13 16:22:00.918325 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4417 2023-07-10 13:38:19.527767 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7818 2023-07-10 12:44:00.159159 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      726 2023-07-14 02:29:52.555797 nonebot_plugin_stable_diffusion_diao-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.1/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    26051 2023-07-14 06:14:48.823684 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15847 2023-07-14 06:52:57.572497 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    17941 2023-07-14 05:24:38.854386 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    38151 2023-07-14 07:24:58.878281 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4417 2023-07-10 13:38:19.527767 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6326 2023-07-14 06:15:38.350677 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-07-14 07:27:24.444210 nonebot_plugin_stable_diffusion_diao-0.3.9.1/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.1/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,18 @@
             if "_" in tag:
                 org_str.append(tag)
             else:
                 convert_list.append(tag)
         args.tags = "".join(convert_list) + ", " + "".join(org_str)
         fifo = AIDRAW(**vars(args), event=event)
         fifo.extra_info += info_style if info_style else ""
-        await fifo.load_balance_init()
+        if fifo.backend_index:
+            fifo.backend_name = config.backend_name_list[fifo.backend_index]
+        else:
+            await fifo.load_balance_init()
         if args.model:
             
             index = fifo.backend_index if (
                 fifo.backend_index is not None and isinstance(fifo.backend_index, int)
                 ) else "0"
             
             await change_model(event, bot, args.model, index)
@@ -229,16 +232,21 @@
                             if re.search(tag, emb, re.IGNORECASE):
                                 new_tags_list.append(emb)
                                 info_ = f"自动找到的嵌入式模型: {emb}, "
                                 fifo.extra_info += f"{info_}\n"
                                 logger.info(info_)
                                 tags_list.pop(org_tag_list.index(tag))
                                 break
+                    if len(new_tags_list) >2:
+                        new_tags_list = []
+                        tags_list = org_tag_list
+                        fifo.extra_info += "↑以上模型未生效↑\n"
+                        raise RuntimeError("匹配到很多lora")
             except Exception as e:
-                logger.warning(f"tag自动匹配失效,出现问题的: {tag}")
+                logger.warning(f"tag自动匹配失效,出现问题的: {tag}\n或者是prompt里自动匹配到的模型过多")
         # 检测是否有18+词条
         try:  # 检查翻译API是否失效
             tags_list: str = await prepocess_tags(tags_list)
         except Exception as e:
             logger.debug(str(e))
             await aidraw.finish("tag处理失败!可能是翻译API错误, 请稍后重试, 或者使用英文重试")
         fifo.ntags = await prepocess_tags(fifo.ntags)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import base64
 import random
 import time
 from io import BytesIO
 import aiofiles
 import json
 import hashlib
+import traceback
+import os
+import ast
 
 import aiohttp
 from nonebot import get_driver
 from nonebot.log import logger
 from PIL import Image
 from nonebot.adapters.onebot.v11 import MessageEvent, PrivateMessageEvent
-
+from datetime import datetime
 from ..config import config, redis_client
 from ..utils import png2jpg, unload_and_reload
 from ..utils.data import shapemap
 from ..utils.load_balance import sd_LoadBalance
-history_list = []
 
 
 class AIDRAW_BASE:
     max_resolution: int = 16
     sampler: str
 
     def __init__(
@@ -251,15 +253,14 @@
         :header: 请求头
         :post_api: 请求地址
         :json: 请求体
         """
         # 请求交互      
         async with aiohttp.ClientSession(headers=header, timeout=aiohttp.ClientTimeout(total=1800)) as session:
             # 向服务器发送请求
-            global history_list
             async with session.post(post_api, json=payload) as resp:
                 if resp.status not in [200, 201]:
                     resp_dict = json.loads(await resp.text())
                     logger.error(resp_dict)
                     if resp_dict["error"] == "OutOfMemoryError":
                         logger.info("检测到爆显存，执行自动模型释放并加载")
                         await unload_and_reload(backend_site=self.backend_site)
@@ -269,14 +270,48 @@
                 logger.debug(f"获取到返回图片，正在处理")
                 # 将图片转化为jpg
                 if config.novelai_save == 1:
                     image_new = await png2jpg(img)
                 else:
                     image_new = base64.b64decode(img)
                 self.img_hash = f"图片id:{hashlib.md5(image_new).hexdigest()}"
+        current_date = datetime.now().date()
+        day: str = str(int(datetime.combine(current_date, datetime.min.time()).timestamp()))
+        try:
+            if redis_client:
+                r = redis_client[2]
+                if r.exists(day):
+                    backend_info = r.get(day)
+                    backend_info = backend_info.decode("utf-8")
+                    backend_info = ast.literal_eval(backend_info)
+                    if backend_info.get("gpu"):
+                        backend_dict = backend_info.get("gpu")
+                        backend_dict[self.backend_name] = backend_dict[self.backend_name] + 1
+                        backend_info["gpu"] = backend_dict
+                    else:
+                        backend_dict = {}
+                        backend_info["gpu"] = {}
+                        for i in list(config.novelai_backend_url_dict.keys()):
+                            backend_dict[i] = 1
+                            backend_info["gpu"] = backend_dict
+                    r.set(day, str(backend_info))
+            else:
+                filename = "data/novelai/day_limit_data.json"
+                if os.path.exists(filename):
+                    async with aiofiles.open(filename, "r") as f:
+                        json_ = await f.read()
+                        json_ = json.loads(json_)
+                    json_[day]["gpu"][self.backend_name] = json_[day]["gpu"][self.backend_name] + 1
+                    async with aiofiles.open(filename, "w") as f:
+                        await f.write(json.dumps(json_))
+                else:
+                    pass
+        except Exception:
+            logger.warning("记录后端工作数量出错")
+            logger.warning(str(traceback.print_exc()))
         self.result.append(image_new)
         return image_new
 
     async def fromresp(self, resp):
         """
         处理请求的返回内容，不要直接调用，请使用post函数
         """
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 import aiohttp
 import ast
 import asyncio
 import traceback
+from tqdm import tqdm
 
 import aiofiles
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseSettings, validator
 from pydantic.fields import ModelField
 
@@ -90,30 +91,30 @@
     novelai_ControlNet_payload: list = [
         {
             "alwayson_scripts": {
             "controlnet": {
             "args": [
                 {
                 "input_image": "",
-                "module": "scribble_hed",
-                "model": "control_v11p_sd15_scribble [d4ba51ff]",
+                "module": "lineart_anime",
+                "model": "control_v11p_sd15s2_lineart_anime [3825e83e]",
                 "weight": 1,
                 "lowvram": "false",
                 "processor_res": novelai_size*1.5,
                 "threshold_a": 100,
                 "threshold_b": 250,
                 }
             ]
                 }
             }
         }, 
         {"controlnet_units": 
                 [{"input_image": "", 
-                "module": "scribble_hed", 
-                "model": "control_v11p_sd15_scribble [d4ba51ff]", 
+                "module": "lineart_anime", 
+                "model": "control_v11p_sd15s2_lineart_anime [3825e83e]", 
                 "weight": 1, 
                 "lowvram": "false", 
                 "processor_res": novelai_size*1.5, 
                 "threshold_a": 100,
                 "threshold_b": 250}]
         }
     ]
@@ -296,15 +297,14 @@
             r3 = redis.Redis(host='localhost', port=6379, db=9)
             redis_client = [r1, r2, r3]
             resp = r1.ping()
             try:
                 if resp:
                     logger.info("redis连接成功")
                     logger.info("开始读取webui的预设")
-                    
                     all_style_list, all_emb_list, all_lora_list = [], [], []
                     backend_emb, backend_lora = {}, {}
                     all_resp_style = await this_is_a_func(0)
                     for backend_style in all_resp_style:
                         if backend_style is not None:
                             for style in backend_style:
                                 all_style_list.append(json.dumps(style))
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,19 +677,26 @@
     await risk_control(bot=bot, event=event, message=[en])
 
 
 @random_tags.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     if redis_client:
         r = redis_client[0]
+        all_tags_list = []
         all_tags_list_str = [] 
-        all_tags_list = r.lrange("prompt", 0, -1)
-        for byte_tag in all_tags_list:
-            all_tags_list_str.append(ast.literal_eval(byte_tag.decode("utf-8")))
-        all_tags_list = all_tags_list_str
+        byte_tags_list = r.lrange("prompts", 0, -1)
+        for byte_tag in byte_tags_list:
+            all_tags_list.append(ast.literal_eval(byte_tag.decode("utf-8")))
+        for list_ in all_tags_list:
+            all_tags_list_str += list_
+        unique_strings = []
+        for string in all_tags_list_str:
+            if string not in unique_strings and string != "":
+                unique_strings.append(string)
+        all_tags_list = unique_strings
     else:
         all_tags_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list)
     chose_tags_list = random.sample(all_tags_list, 12)
     chose_tags = ', '.join(chose_tags_list)
 
     fifo = AIDRAW(user_id=event.user_id, 
                   tags=chose_tags, 
@@ -756,19 +763,22 @@
 
 
 @word_frequency_count.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
     msg_list = []
     if redis_client:
         r = redis_client[0]
-        if r.exists("prompt"):
+        if r.exists("prompts"):
             word_list_str = []
-            word_list = r.lrange("prompt", 0, -1)
-            for byte_word in word_list:
-                word_list_str.append(ast.literal_eval(byte_word.decode("utf-8")))
+            word_list = []
+            byte_word_list = r.lrange("prompts", 0, -1)
+            for byte_tag in byte_word_list:
+                word_list.append(ast.literal_eval(byte_tag.decode("utf-8")))
+            for list_ in word_list:
+                word_list_str += list_
             word_list = word_list_str
         else:
             await word_frequency_count.finish("画几张图图再来统计吧!")
     else:
         word_list = await asyncio.get_event_loop().run_in_executor(None, get_tags_list, False)
         
     def count_word_frequency(word_list):
@@ -852,17 +862,18 @@
         await genera_aging.finish("未连接redis, 此功能不可用")
 
 
 @reload_.handle()
 async def _(msg: Message = CommandArg()):
     if not msg:
         await reload_.finish("你要释放哪个后端的显存捏?")
-    text_msg = int(msg.extract_plain_text())
+    text_msg = msg.extract_plain_text()
     if not text_msg.isdigit():
         await reload_.finish("笨蛋!后端编号是数字啦!!")
+    text_msg = int(text_msg)
     try:
         await unload_and_reload(text_msg)
     except Exception:
         logger.error(traceback.print_exc())
     else:
         await reload_.finish(f"为后端{config.backend_name_list[text_msg]}重载成功啦!")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files 12% similar despite different names*

```diff
@@ -142,43 +142,11 @@
                         list_tuple.append((backend_site, weight*multi))
             else:
                 for backend, weight in zip(normal_backend, weight_list):
                     list_tuple.append((backend, weight))
             print(list_tuple)
             fifo = AIDRAW()
             ava_url = fifo.weighted_choice(list_tuple)
-    if redis_client:
-        try:
-            r = redis_client[2]
-            if r.exists(day):
-                backend_info = r.get(day)
-                backend_info = backend_info.decode("utf-8")
-                backend_info = ast.literal_eval(backend_info)
-                if backend_info.get("gpu"):
-                    backend_dict = backend_info.get("gpu")
-                    backend_dict[reverse_dict[ava_url]] = backend_dict[reverse_dict[ava_url]] + 1
-                    backend_info["gpu"] = backend_dict
-                else:
-                    backend_dict = {}
-                    backend_info["gpu"] = {}
-                    for i in list(config.novelai_backend_url_dict.keys()):
-                        backend_dict[i] = 1
-                        backend_info["gpu"] = backend_dict
-                r.set(day, str(backend_info))
-        except Exception:
-            logger.warning("redis出错惹!不过问题不大")
-            logger.info(traceback.print_exc())
-    else:
-        filename = "data/novelai/day_limit_data.json"
-        if os.path.exists(filename):
-            async with aiofiles.open(filename, "r") as f:
-                json_ = await f.read()
-                json_ = json.loads(json_)
-            json_[day]["gpu"][reverse_dict[ava_url]] = json_[day]["gpu"][reverse_dict[ava_url]] + 1
-            async with aiofiles.open(filename, "w") as f:
-                await f.write(json.dumps(json_))
-        else:
-            pass
     logger.info(f"已选择后端{reverse_dict[ava_url]}")
     ava_url_index = list(backend_url_dict.values()).index(ava_url)
     ava_url_tuple = (ava_url, reverse_dict[ava_url], all_resp, len(normal_backend))
     return ava_url_index, ava_url_tuple, normal_backend
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9"
+version = "0.3.9.1"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

