# Comparing `tmp/nonebot_plugin_game_collection-2.3.4.tar.gz` & `tmp/nonebot_plugin_game_collection-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.3.4.tar", last modified: Fri Jul 14 11:47:25 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.3.6.tar", last modified: Fri Jul 14 15:20:34 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.3.4.tar` & `nonebot_plugin_game_collection-2.3.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.518237 nonebot_plugin_game_collection-2.3.4/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.4/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-07-14 11:47:25.517737 nonebot_plugin_game_collection-2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.451489 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21635 2023-07-13 18:22:12.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Alchemy.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.463500 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Fortress/
--rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Fortress/core.py
--rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.472507 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10598 2023-07-13 18:15:22.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    23104 2023-07-13 19:13:31.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    32544 2023-07-14 10:55:41.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0    11300 2023-07-13 19:07:21.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.476010 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.499773 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.501774 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.515735 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    21412 2023-06-29 17:01:38.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:47:25.461498 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-14 11:47:25.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-14 11:47:25.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:47:25.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-14 11:47:25.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-14 11:47:25.000000 nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 11:47:25.518237 nonebot_plugin_game_collection-2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-07-14 11:47:20.000000 nonebot_plugin_game_collection-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.519461 nonebot_plugin_game_collection-2.3.6/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.6/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-07-14 15:20:34.518961 nonebot_plugin_game_collection-2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.467916 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21648 2023-07-14 14:56:24.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.478926 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Fortress/
+-rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Fortress/core.py
+-rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.486433 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10598 2023-07-13 18:15:22.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    23104 2023-07-13 19:13:31.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    32678 2023-07-14 14:30:15.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0    11300 2023-07-13 19:07:21.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.489935 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.509452 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.511454 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.517459 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    22338 2023-07-14 15:16:16.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.477425 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:20:34.519961 nonebot_plugin_game_collection-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-07-14 15:20:30.000000 nonebot_plugin_game_collection-2.3.6/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.3.4/LICENSE` & `nonebot_plugin_game_collection-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/README.md` & `nonebot_plugin_game_collection-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Account.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import time
 import datetime
 
 from .utils.chart import (
     bar_chart,
     my_info_head,
     my_info_account,
+    my_exchange_head,
     linecard,
     info_splicing
     )
 from .data import Company, UserDict, GroupAccount
 from .data import props_library, props_index
 from .config import bot_name,sign_gold, revolt_gold, revolt_cd, revolt_gini, max_bet_gold
 
@@ -337,15 +338,15 @@
                     account_name = "本群"
                 else:
                     account_name = group_data[exchange.group_id].company.company_name
                     account_name = account_name if account_name else f"({str(exchange.group_id)[4]}...)"
                 msg += f"[pixel][20]报价 [nowrap]\n[color][green]{exchange.quote}[nowrap]\n[pixel][400]发布 [nowrap]\n[color][green]{exchange.n}\n"
             info.append(linecard(msg, width = 880,endline = f"报价账户：{account_name}" if account_name else "无报价"))
     if info:
-        info.insert(0,await my_info_head(user,group_account.nickname))
+        info.insert(0,await my_exchange_head(group_account))
         return MessageSegment.image(info_splicing(info,Manager.BG_path(event.user_id)))
     else:
         return "你的股票信息为空。"
 
 def my_props(event:MessageEvent) -> Message:
     """
     我的道具
```

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Alchemy.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Alchemy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Fortress/core.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Fortress/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,14 @@
     config = Config,
     extra = {'menu_data':menu_data,'menu_template':'default'})
 
 data = Manager.data
 company_index = Manager.company_index
 current_games = Game.current_games
 
-scheduler = require("nonebot_plugin_apscheduler").scheduler
-
 def to_int(arg:Message, default:int = bet_gold):
     num = arg.extract_plain_text().strip()
     if num.isdigit():
         return int(num)
     else:
         return default
 
@@ -906,41 +904,45 @@
 Market_reset = on_fullmatch("市场重置", permission = SUPERUSER, priority = 20, block = True)
 
 @Market_reset.handle()
 async def _():
     Market.reset()
     await Market_reset.finish("市场已重置。")
 
+require("nonebot_plugin_apscheduler")
+
+from nonebot_plugin_apscheduler import scheduler
+
 # 市场更新
-@scheduler.scheduled_job("cron", minute = "*/5")
+@scheduler.scheduled_job("cron", minute = "*/5", misfire_grace_time = 120)
 async def _():
     log = Market.update()
     if log:
         logger.info("\n" + log)
 
 # 数据备份
 Backup = on_command("Backup", aliases = {"数据备份", "游戏备份"}, permission = SUPERUSER, priority = 20, block = True)
 
 @Backup.handle()
-@scheduler.scheduled_job("cron", hour = "*/4")
+@scheduler.scheduled_job("cron", hour = "*/4", misfire_grace_time = 120)
 async def _():
     now = time.strftime('%Y-%m-%d %H-%M-%S', time.localtime(time.time()))
     now = now.split()
     backup_today = backup / now[0]
     if not backup_today.exists():
         backup_today.mkdir()
     data.save()
     shutil.copy(f"{path}/russian_data.json",f"{backup_today}/russian_data {now[1]}.json")
     logger.info(f'russian_data.json 备份成功！')
 
 # 刷新每日
 Newday = on_command("Newday", aliases = {"刷新每日", "刷新签到"}, permission = SUPERUSER, priority = 20, block = True)
 
 @Newday.handle()
-@scheduler.scheduled_job("cron", hour = 0)
+@scheduler.scheduled_job("cron", hour = 0, misfire_grace_time = 120)
 async def _():
     Manager.update_company_index()
     log = data.verification()
     logger.info(f"\n{log}")
     data.Newday()
     with open(path / "Newday.log","a",encoding = "utf8") as f:
         f.write(f"\n{datetime.datetime.fromtimestamp(time.time()).strftime('%Y 年 %m 月 %d 日 %H:%M:%S')}\n"
@@ -953,13 +955,13 @@
             shutil.rmtree(folder)
             logger.info(f'备份 {folder} 已删除！')
 
 # 保存数据
 DataSave = on_command("DataSave", aliases = {"保存数据", "保存游戏"},permission = SUPERUSER, priority = 20, block = True)
 
 @DataSave.handle()
-@scheduler.scheduled_job("cron", minute = "*/10")
+@scheduler.scheduled_job("cron", minute = "*/10", misfire_grace_time = 120)
 async def _():
     data.save()
     with open(Market.market_history_file, "w", encoding = "utf8") as f:
         json.dump(Market.market_history, f, ensure_ascii = False, indent = 4)
     logger.info(f'游戏数据已保存！！')
```

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,14 +523,32 @@
     draw.text((300,190),f"单位：{str(group_id)[:4]}...", fill = (0,0,0),font = font_normal)
     draw.rectangle(((300,240), (740,280)), fill = "#00000033")
     draw.rectangle(((300,240), (300 + int(440 * member_count[0]/(member_count[1])),280)), fill = "#99CCFF")
     draw.text((310,240),f"{member_count[0]}/{member_count[1]}", fill = (0,0,0),font = font_normal )
     draw.text((750,240),f"{round(100 * member_count[0]/member_count[1],1)}%", fill = (0,0,0),font = font_normal)
     return canvas
 
+async def my_exchange_head(group_account:GroupAccount):
+    """
+    我的交易信息第一个信息
+    """
+    gold = group_account.gold
+    canvas = Image.new("RGBA", (880, 250))
+    avatar = Image.open(await download_avatar(group_account.user_id))
+    avatar = avatar.resize((210,210))
+    circle_mask = Image.new("RGBA", avatar.size, (255, 255, 255, 0))
+    ImageDraw.Draw(circle_mask).ellipse(((0,0),avatar.size), fill="black")
+    canvas.paste(avatar, (20, 20), circle_mask)
+    draw = ImageDraw.Draw(canvas)
+    draw.text((250,40),f"{group_account.nickname}", fill = (0,0,0),font = font_big)
+    draw.line(((250, 120), (860, 120)), fill = "gray", width = 4)
+    draw.text((250,140),f"金币 {'{:,}'.format(group_account.gold)}", fill = (0,0,0),font = font_normal)
+    draw.text((250,190),f"股票 {'{:,}'.format(round(group_account.value,2))}", fill = (0,0,0),font = font_normal)
+    return canvas
+
 def info_splicing(info:List[IMG],BG_path, spacing:int = 20):
     """
     信息拼接
         info:信息图片列表
         bg_path:背景地址
     """
     bg = Image.open(BG_path).convert("RGBA")
```

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.4/setup.py` & `nonebot_plugin_game_collection-2.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.3.4',
+version='2.3.6',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

