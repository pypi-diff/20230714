# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.7.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.7.tar", last modified: Thu Jul 13 15:23:17 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.8.tar", last modified: Fri Jul 14 01:49:19 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.7/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    25240 2023-07-13 15:22:45.034582 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    14048 2023-07-10 03:47:58.215732 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    17924 2023-07-10 13:46:44.820439 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    37732 2023-07-11 04:51:28.097135 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4417 2023-07-10 13:38:19.527767 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7818 2023-07-10 12:44:00.159159 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      726 2023-07-13 15:23:17.402105 nonebot_plugin_stable_diffusion_diao-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.8/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    25578 2023-07-14 01:47:47.881837 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     3894 2023-06-12 05:12:59.000048 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    14048 2023-07-10 03:47:58.215732 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     5834 2023-07-12 05:55:25.827666 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    17924 2023-07-10 13:46:44.820439 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9229 2023-06-14 05:11:03.238536 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2754 2023-07-09 06:10:57.298081 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11373 2023-07-10 03:48:14.234739 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-03 04:27:28.351334 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    37733 2023-07-13 16:22:00.918325 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4417 2023-07-10 13:38:19.527767 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7818 2023-07-10 12:44:00.159159 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      648 2023-07-09 16:19:12.987305 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      726 2023-07-14 01:49:19.208000 nonebot_plugin_stable_diffusion_diao-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.8/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     parser=aidraw_parser,
     priority=5
 )
 
 
 @aidraw.handle()
 async def aidraw_get(bot: Bot, event: MessageEvent, args: Namespace = ShellCommandArgs()):
+    info_style = None
     style_tag, style_ntag = "", ""
     user_id = str(event.user_id)
     if isinstance(event, PrivateMessageEvent):
         group_id = str(event.user_id)+"_private"
     else:
         group_id = str(event.group_id)
     global bot_id
@@ -183,58 +184,61 @@
             tags_list = tags
         org_tag_list = tags_list
         new_tags_list = []
         if args.match or not config.auto_match:
             pass
         elif redis_client:
             r2 = redis_client[1]
-            if r2.exists("lora"):
-                all_lora_dict = r2.get("lora")
-                all_emb_dict = r2.get("emb")
-                all_backend_lora_list = ast.literal_eval(all_lora_dict.decode("utf-8"))
-                all_backend_emb_list = ast.literal_eval(all_emb_dict.decode("utf-8"))
-                cur_backend_lora_list = all_backend_lora_list[fifo.backend_name]
-                cur_backend_emb_list = all_backend_emb_list[fifo.backend_name]
-                if fifo.backend_name in all_backend_lora_list and all_backend_lora_list[fifo.backend_name] is None:
-                    logger.info("此后端没有lora数据,尝试重新载入")
-                    cur_backend_lora_list, _ = await get_and_process_lora(fifo.backend_site, fifo.backend_name)
-                    cur_backend_emb_list, _ = await get_and_process_emb(fifo.backend_site, fifo.backend_name)
-                    pipe_ = r2.pipeline()
-                    all_backend_lora_list[fifo.backend_name] = cur_backend_lora_list
-                    all_backend_emb_list[fifo.backend_name] = cur_backend_emb_list
-                    pipe_.set("lora", str(all_backend_lora_list))
-                    pipe_.set("emb", str(all_backend_emb_list))
-                    pipe_.execute()
-                
-                tag_index = -1
-                for tag in org_tag_list:
-                    tag_index += 1
-                    index = -1
-                    for lora in list(cur_backend_lora_list.values()):
-                        index += 1
-                        if re.search(tag, lora, re.IGNORECASE):
-                            info_ = f"自动找到的lora模型: {lora}"
-                            fifo.extra_info += f"{info_}\n"
-                            logger.info(info_)
-                            new_tags_list.append(f"<lora:{lora}:0.9>, ")
-                            tags_list.pop(org_tag_list.index(tag))
-                            break
-                tag_index = -1
-                for tag in org_tag_list:
-                    tag_index += 1
-                    index = -1
-                    for emb in list(cur_backend_emb_list.values()):
-                        index += 1
-                        if re.search(tag, emb, re.IGNORECASE):
-                            new_tags_list.append(emb)
-                            info_ = f"自动找到的嵌入式模型: {emb}, "
-                            fifo.extra_info += f"{info_}\n"
-                            logger.info(info_)
-                            tags_list.pop(org_tag_list.index(tag))
-                            break
+            try:
+                tag = ""
+                if r2.exists("lora"):
+                    all_lora_dict = r2.get("lora")
+                    all_emb_dict = r2.get("emb")
+                    all_backend_lora_list = ast.literal_eval(all_lora_dict.decode("utf-8"))
+                    all_backend_emb_list = ast.literal_eval(all_emb_dict.decode("utf-8"))
+                    cur_backend_lora_list = all_backend_lora_list[fifo.backend_name]
+                    cur_backend_emb_list = all_backend_emb_list[fifo.backend_name]
+                    if fifo.backend_name in all_backend_lora_list and all_backend_lora_list[fifo.backend_name] is None:
+                        logger.info("此后端没有lora数据,尝试重新载入")
+                        cur_backend_lora_list, _ = await get_and_process_lora(fifo.backend_site, fifo.backend_name)
+                        cur_backend_emb_list, _ = await get_and_process_emb(fifo.backend_site, fifo.backend_name)
+                        pipe_ = r2.pipeline()
+                        all_backend_lora_list[fifo.backend_name] = cur_backend_lora_list
+                        all_backend_emb_list[fifo.backend_name] = cur_backend_emb_list
+                        pipe_.set("lora", str(all_backend_lora_list))
+                        pipe_.set("emb", str(all_backend_emb_list))
+                        pipe_.execute()
+                    tag_index = -1
+                    for tag in org_tag_list:
+                        tag_index += 1
+                        index = -1
+                        for lora in list(cur_backend_lora_list.values()):
+                            index += 1
+                            if re.search(tag, lora, re.IGNORECASE):
+                                info_ = f"自动找到的lora模型: {lora}"
+                                fifo.extra_info += f"{info_}\n"
+                                logger.info(info_)
+                                new_tags_list.append(f"<lora:{lora}:0.9>, ")
+                                tags_list.pop(org_tag_list.index(tag))
+                                break
+                    tag_index = -1
+                    for tag in org_tag_list:
+                        tag_index += 1
+                        index = -1
+                        for emb in list(cur_backend_emb_list.values()):
+                            index += 1
+                            if re.search(tag, emb, re.IGNORECASE):
+                                new_tags_list.append(emb)
+                                info_ = f"自动找到的嵌入式模型: {emb}, "
+                                fifo.extra_info += f"{info_}\n"
+                                logger.info(info_)
+                                tags_list.pop(org_tag_list.index(tag))
+                                break
+            except Exception as e:
+                logger.warning(f"tag自动匹配失效,出现问题的: {tag}")
         # 检测是否有18+词条
         try:  # 检查翻译API是否失效
             tags_list: str = await prepocess_tags(tags_list)
         except Exception as e:
             logger.debug(str(e))
             await aidraw.finish("tag处理失败!可能是翻译API错误, 请稍后重试, 或者使用英文重试")
         fifo.ntags = await prepocess_tags(fifo.ntags)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -877,15 +877,15 @@
             style_list = r.lrange("style", 0, -1)
             style_list = [ast.literal_eval(style.decode("utf-8")) for style in style_list]
             if r.exists("user_style"):
                 user_style_list = r.lrange("user_style", 0, -1)
                 user_style_list = [ast.literal_eval(style.decode("utf-8")) for style in user_style_list]
                 style_list += user_style_list
     else:
-        await style.finish("需要redis以使用此功能")
+        await style_.finish("需要redis以使用此功能")
     if args.delete:
         delete_name = args.delete[0] if isinstance(args.delete, list) else args.delete
         find_style = False
         style_index = -1
         for style in user_style_list:
             style_index += 1
             if style["name"] == delete_name:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.8/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.7/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.7"
+version = "0.3.8"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

