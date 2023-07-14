# Comparing `tmp/nonebot_plugin_cp_broadcast-0.3.0.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-1.0.0.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-0.3.0.tar` & `nonebot_plugin_cp_broadcast-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/LICENSE
--rw-r--r--   0        0        0     4488 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/README.md
--rw-r--r--   0        0        0     7505 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2699 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     1946 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      438 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0      732 2023-07-13 07:11:12.927023 nonebot_plugin_cp_broadcast-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 13:38:10.859183 nonebot_plugin_cp_broadcast-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5298 2023-07-14 13:38:10.859183 nonebot_plugin_cp_broadcast-1.0.0/README.md
+-rw-r--r--   0        0        0     8429 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2699 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     3257 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      589 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0     6778 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/sqlite3.py
+-rw-r--r--   0        0        0      732 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6255 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/LICENSE` & `nonebot_plugin_cp_broadcast-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/README.md` & `nonebot_plugin_cp_broadcast-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 除了简单的指令外，它支持每天定时发送三种比赛的信息。
 
 查询的结果会存到列表里，以减少网站爬取的次数。
 
 由于 AtCoder 网站没提供比赛信息的 API，因此是直接对网页进行爬取的，代码中是爬取两个比赛，你可以自己修改得更多。
 
+除了爬取比赛这一基本功能外，它还支持 Codeforces 平台一些信息的查询，具体指令将在下文介绍。
+
 为什么取 cp-broadcast 这个英文名呢？因为竞赛性编程的英文是：Competitive Programming，直接拿来做名字感觉太长了，因此我把它写成了缩写，broadcast 是播报的意思，因此就用 cp-broadcast 来当名字了。
 
 这是本蒟蒻的第一个上传至 pypi 的 nonebot2 项目，可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
 
 有任何问题可联系QQ：3411907440。
 
 ## 💿 安装
@@ -98,10 +100,32 @@
 | `cf` | 群员 | 否 | 群聊 | 发送最近三场 Codeforces 比赛的信息 |
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
 | `atc` | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
 | `today` | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
 | `next` | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
 | `help` | 群员 | 是 | 群聊 | 发送帮助信息 |
 | `update` | 群员 | 否 | 群聊 | 手动更新比赛信息 |
+| `cf监视` | 群员 | 是 | 群聊 | 监视某人的 rating 变化 |
+| `cf监视列表` | 群员 | 是 | 群聊 | 展示已经监视了哪些人 |
+| `cf查询` | 群员 | 是 | 群聊 | 查询对应 id 的相关信息 |
+
+
 ### 效果图
-<img src="./docs/preview.webp" style="zoom:30%;" />
+<img src="./docs/cf.JPG" style="zoom:30%;" />
+
+<img src="./docs/nc.JPG" style="zoom:30%;" />
+
+<img src="./docs/atc.JPG" style="zoom:30%;" />
+
+<img src="./docs/today.JPG" style="zoom:30%;" />
+
+<img src="./docs/next.JPG" style="zoom:30%;" />
+
+<img src="./docs/help.JPG" style="zoom:30%;" />
+
+<img src="./docs/update.JPG" style="zoom:30%;" />
+
+<img src="./docs/cfjianshi.JPG" style="zoom:30%;" />
+
+<img src="./docs/cfjianshiliebiao.JPG" style="zoom:30%;" />
 
+<img src="./docs/cfchaxun.JPG" style="zoom:30%;" />
```

#### html2text {}

```diff
@@ -6,15 +6,17 @@
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
 è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã
 é¤äºç®åçæä»¤å¤ï¼å®æ¯ææ¯å¤©å®æ¶åéä¸ç§æ¯èµçä¿¡æ¯ã
 æ¥è¯¢çç»æä¼å­å°åè¡¨éï¼ä»¥åå°ç½ç«ç¬åçæ¬¡æ°ã ç±äº
 AtCoder ç½ç«æ²¡æä¾æ¯èµä¿¡æ¯ç
 APIï¼å æ­¤æ¯ç´æ¥å¯¹ç½é¡µè¿è¡ç¬åçï¼ä»£ç ä¸­æ¯ç¬åä¸¤ä¸ªæ¯èµï¼ä½ å¯ä»¥èªå·±ä¿®æ¹å¾æ´å¤ã
-ä¸ºä»ä¹å cp-broadcast
+é¤äºç¬åæ¯èµè¿ä¸åºæ¬åè½å¤ï¼å®è¿æ¯æ Codeforces
+å¹³å°ä¸äºä¿¡æ¯çæ¥è¯¢ï¼å·ä½æä»¤å°å¨ä¸æä»ç»ã ä¸ºä»ä¹å
+cp-broadcast
 è¿ä¸ªè±æåå¢ï¼å ä¸ºç«èµæ§ç¼ç¨çè±ææ¯ï¼Competitive
 Programmingï¼ç´æ¥æ¿æ¥ååå­æè§å¤ªé¿äºï¼å æ­¤ææå®åæäºç¼©åï¼broadcast
 æ¯æ­æ¥çææï¼å æ­¤å°±ç¨ cp-broadcast æ¥å½åå­äºã
 è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot2
 é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
 requestsã æä»»ä½é®é¢å¯èç³»QQï¼3411907440ã ## ð¿ å®è£  ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
@@ -44,8 +46,14 @@
 -----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
 åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
-æå¨æ´æ°æ¯èµä¿¡æ¯ | ### ææå¾ [./docs/preview.webp]
+æå¨æ´æ°æ¯èµä¿¡æ¯ | | `cfçè§` | ç¾¤å | æ¯ | ç¾¤è |
+çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ | ç¾¤è |
+å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è |
+æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/nc.JPG]
+[./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG] [./
+docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/cfjianshiliebiao.JPG] [./docs/
+cfchaxun.JPG]
```

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .config import Config, cp_broadcast_config
 from .codeforces import *
 from .nowcoder import *
 from .atcoder import *
+from .sqlite3 import *
 import datetime
 from datetime import timedelta
 from nonebot.plugin import on_fullmatch
 from nonebot import require, get_bot
 from nonebot.rule import to_me
 from nonebot.log import logger
 import asyncio
@@ -17,14 +18,17 @@
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="算法竞赛比赛查询",
     description="可以查询牛客、atcoder、codeforces平台的今天和近几天的比赛信息",
     usage="cf->查询cf比赛\n"\
+        "@{botname} cf查询+id->查询某人信息\n"\
+        "@{botname} cf监视+id->监视某人rating变化\n"\
+        "@{botname} cf监视列表->展示已监视的选手id\n"\
         "nc/牛客->查询牛客比赛\n"\
         "atc->查询atcoder比赛\n"\
         "today->查询今天的比赛\n"\
         "next->查询明天之后的部分比赛\n"
         "update->更新比赛数据\n"\
         "about->{botname}的一些信息\n",
     type="application",
@@ -33,16 +37,22 @@
     supported_adapters = {"nonebot.adapters.onebot.v11"},
 )
 
 
 try:
     scheduler = require("nonebot_plugin_apscheduler").scheduler
 except BaseException:
-    logger.warning('未检测到定时插件，定时功能将不启用')
     scheduler = None
+
+logger.opt(colors=True).info(
+    "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
+    if scheduler
+    else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>, <r>禁用定时任务功能</r>"
+)
+
 ###列表下标0为比赛名称、下标1为比赛时间、下标2为比赛链接
 
 async def ans_today():  #today
     global cf
     global atc
     global nc
     msg = ''
@@ -190,15 +200,15 @@
     await asyncio.sleep(1)
     for id in cp_broadcast_list:
         await asyncio.sleep(2)
         await get_bot().send_group_msg(group_id=id, message='早上好呀！'+ await ans_today())
 
 if scheduler:
     scheduler.add_job(auto_broadcast, 
-                      "cron", hour=cp_broadcast_time['hour'],minute=cp_broadcast_time['minute'],id="_-"
+                      "cron", hour=cp_broadcast_time['hour'],minute=cp_broadcast_time['minute'],id="auto_broadcast"
                       )
 
 #凌晨12点自动更新比赛信息
 async def update():
     global cf
     global atc
     global nc
@@ -219,8 +229,28 @@
         )
 
 #更新数据
 update_matcher = on_fullmatch('update', priority=70, block=True)
 @update_matcher.handle()
 async def reply():
     await update()
-    await update_matcher.finish('数据已更新完成')
+    await update_matcher.finish('数据已更新完成')
+
+
+#cf分数变化提醒
+async def ratingReminder():
+    await asyncio.sleep(1)
+    logger.info('cf分数变化检测开始')
+    messList = await returRatingChangeInfo()
+    if len(messList) == 0:
+        return
+    for id in cp_broadcast_list:
+        await asyncio.sleep(2)
+        for mess in messList:
+            await get_bot().send_group_msg(group_id=id, message=mess['output'])
+            await asyncio.sleep(2)
+
+
+if scheduler:
+    scheduler.add_job(
+        ratingReminder, "interval", minutes=20, id="ratingReminder"
+    )
```

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,76 @@
+import datetime
 import time
 from httpx import AsyncClient
 from nonebot.plugin import on_fullmatch
+from fake_useragent import FakeUserAgent
 from nonebot.adapters.onebot.v11.message import Message
 import asyncio
 
+headers = {
+    'user-agent': FakeUserAgent().random
+}
+
 ###列表下标0为比赛名称、下标1为比赛时间、下标2为比赛链接
-cf = [] 
+nc = []
 
-async def get_data_cf() -> bool:
-    global cf
-    url = 'https://codeforces.com/api/contest.list?gym=false'
-    num = 0 #尝试获取的次数，最多尝试三次
-    while num < 3 :
+async def get_data_nc() -> bool:
+    global nc
+    url = 'https://ac.nowcoder.com/acm/calendar/contest'
+    num = 0 #爬取次数,最大为3
+    while num < 3:
         try:
-            if(len(cf) > 0):
-                cf.clear()
+            date = str(datetime.datetime.now().year) + ' - ' + str(datetime.datetime.now().month)
+            second = '{:.3f}'.format(time.time())
+            params = {
+                'token': '',
+                'month': date,
+                '_': second
+            }
+            if(len(nc) > 0):
+                nc.clear()
+            
             async with AsyncClient() as client:
-                r = await client.get(url, timeout=10)
-            for each in r.json()['result'][0::]:
-                if each['phase'] != "BEFORE":
-                    break
-                contest_name = each['name']
-                contest_time = time.strftime("%Y-%m-%d %H:%M", time.localtime(each['startTimeSeconds']))
-                id = each['id']
-                contest_url = f'https://codeforces.com/contest/{id}'
-                cf.append([contest_name, contest_time, contest_url])  #从左到右分别为比赛名称、比赛时间、比赛链接
-            cf.reverse()
-            return True
+                r = await client.get(url, headers=headers, params=params, timeout=20)
+            
+            r = r.json()
+            second2 = int(float(second)*1000)
+            if r['msg'] == "OK" and r['code'] == 0 :
+                for data in r["data"]:
+                    if data["startTime"] >= second2:
+                        contest_name = data["contestName"]
+                        contest_time = time.strftime("%Y-%m-%d %H:%M", time.localtime(data['startTime']/1000))
+                        contest_url = data["link"]
+                        nc.append([contest_name, contest_time, contest_url])
+                return True
+            else:
+                return False
         except:
             num += 1
-            await asyncio.sleep(2)  #两秒后再次获取信息
+            await asyncio.sleep(2)
     return False
 
-async def ans_cf() -> str:
-    global cf
-    if len(cf) == 0:
-        await get_data_cf()
-    if len(cf) == 0:
+
+async def ans_nc() -> str:
+    global nc
+    if len(nc) == 0:
+        await get_data_nc()
+    if len(nc) == 0:
         return f'突然出错了，稍后再试哦~'
+    #second = '{:.3f}'.format(time.time())
+    #second2 = int(float(second)*1000)
     msg = ''
-    tot = 0
-    for each in cf:
-        msg += '比赛名称：' + each[0] + '\n'\
-            + '比赛时间：' + each[1] + '\n'\
-            + '比赛链接' + each[2]
-        tot += 1
-        if (tot != 3):
-            msg += '\n'
-        else:
+    n = 0
+    for data in nc:
+        n += 1
+        msg += "比赛名称：" + data[0] + '\n'
+        msg += "比赛时间：" + data[1] + '\n'
+        msg += "比赛链接：" + data[2] + '\n'
+        if n == 3:
             break
-    return f"找到最近的 {tot} 场cf比赛为：\n" + msg
+    return f"找到最近的 {n} 场牛客比赛为：\n" + msg
 
-cf_matcher = on_fullmatch('cf',priority = 80,block=True)
-@cf_matcher.handle()
-async def reply_handle():
-    msg = await ans_cf()
-    await cf_matcher.finish(msg)
+nc_matcher = on_fullmatch(('牛客', 'nc'),priority=70,block=True)
+@nc_matcher.handle()
+async def _():
+    msg = await ans_nc()
+    await nc_matcher.finish(msg)
```

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/pyproject.toml` & `nonebot_plugin_cp_broadcast-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "0.3.0"
+version = "1.0.0"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
```

### Comparing `nonebot_plugin_cp_broadcast-0.3.0/PKG-INFO` & `nonebot_plugin_cp_broadcast-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 0.3.0
+Version: 1.0.0
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -51,14 +51,16 @@
 
 除了简单的指令外，它支持每天定时发送三种比赛的信息。
 
 查询的结果会存到列表里，以减少网站爬取的次数。
 
 由于 AtCoder 网站没提供比赛信息的 API，因此是直接对网页进行爬取的，代码中是爬取两个比赛，你可以自己修改得更多。
 
+除了爬取比赛这一基本功能外，它还支持 Codeforces 平台一些信息的查询，具体指令将在下文介绍。
+
 为什么取 cp-broadcast 这个英文名呢？因为竞赛性编程的英文是：Competitive Programming，直接拿来做名字感觉太长了，因此我把它写成了缩写，broadcast 是播报的意思，因此就用 cp-broadcast 来当名字了。
 
 这是本蒟蒻的第一个上传至 pypi 的 nonebot2 项目，可能有很多不完善的地方，欢迎大家来提 issue 和 pull requests。 
 
 有任何问题可联系QQ：3411907440。
 
 ## 💿 安装
@@ -122,11 +124,33 @@
 | `cf` | 群员 | 否 | 群聊 | 发送最近三场 Codeforces 比赛的信息 |
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
 | `atc` | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
 | `today` | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
 | `next` | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
 | `help` | 群员 | 是 | 群聊 | 发送帮助信息 |
 | `update` | 群员 | 否 | 群聊 | 手动更新比赛信息 |
+| `cf监视` | 群员 | 是 | 群聊 | 监视某人的 rating 变化 |
+| `cf监视列表` | 群员 | 是 | 群聊 | 展示已经监视了哪些人 |
+| `cf查询` | 群员 | 是 | 群聊 | 查询对应 id 的相关信息 |
+
+
 ### 效果图
-<img src="./docs/preview.webp" style="zoom:30%;" />
+<img src="./docs/cf.JPG" style="zoom:30%;" />
+
+<img src="./docs/nc.JPG" style="zoom:30%;" />
+
+<img src="./docs/atc.JPG" style="zoom:30%;" />
+
+<img src="./docs/today.JPG" style="zoom:30%;" />
+
+<img src="./docs/next.JPG" style="zoom:30%;" />
+
+<img src="./docs/help.JPG" style="zoom:30%;" />
+
+<img src="./docs/update.JPG" style="zoom:30%;" />
+
+<img src="./docs/cfjianshi.JPG" style="zoom:30%;" />
+
+<img src="./docs/cfjianshiliebiao.JPG" style="zoom:30%;" />
 
+<img src="./docs/cfchaxun.JPG" style="zoom:30%;" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.0.0 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
 HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
@@ -19,15 +19,17 @@
 æ¥è¯´ï¼åå ç¼ç¨ç«èµæ¯å¿ä¸å¯å°çï¼è¿ä¸ªæä»¶å®ç°äº
 Codeforcesãçå®¢ç«èµãAtCoder
 è¿ä¸ä¸ªä¸»æµçç¼ç¨ç«èµå¹³å°çæ¯èµæ¥è¯¢åæ­æ¥ã
 é¤äºç®åçæä»¤å¤ï¼å®æ¯ææ¯å¤©å®æ¶åéä¸ç§æ¯èµçä¿¡æ¯ã
 æ¥è¯¢çç»æä¼å­å°åè¡¨éï¼ä»¥åå°ç½ç«ç¬åçæ¬¡æ°ã ç±äº
 AtCoder ç½ç«æ²¡æä¾æ¯èµä¿¡æ¯ç
 APIï¼å æ­¤æ¯ç´æ¥å¯¹ç½é¡µè¿è¡ç¬åçï¼ä»£ç ä¸­æ¯ç¬åä¸¤ä¸ªæ¯èµï¼ä½ å¯ä»¥èªå·±ä¿®æ¹å¾æ´å¤ã
-ä¸ºä»ä¹å cp-broadcast
+é¤äºç¬åæ¯èµè¿ä¸åºæ¬åè½å¤ï¼å®è¿æ¯æ Codeforces
+å¹³å°ä¸äºä¿¡æ¯çæ¥è¯¢ï¼å·ä½æä»¤å°å¨ä¸æä»ç»ã ä¸ºä»ä¹å
+cp-broadcast
 è¿ä¸ªè±æåå¢ï¼å ä¸ºç«èµæ§ç¼ç¨çè±ææ¯ï¼Competitive
 Programmingï¼ç´æ¥æ¿æ¥ååå­æè§å¤ªé¿äºï¼å æ­¤ææå®åæäºç¼©åï¼broadcast
 æ¯æ­æ¥çææï¼å æ­¤å°±ç¨ cp-broadcast æ¥å½åå­äºã
 è¿æ¯æ¬èè»çç¬¬ä¸ä¸ªä¸ä¼ è³ pypi ç nonebot2
 é¡¹ç®ï¼å¯è½æå¾å¤ä¸å®åçå°æ¹ï¼æ¬¢è¿å¤§å®¶æ¥æ issue å pull
 requestsã æä»»ä½é®é¢å¯èç³»QQï¼3411907440ã ## ð¿ å®è£  ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
@@ -57,8 +59,14 @@
 -----:|:----:|:----:|:----:|:----:| | `cf` | ç¾¤å | å¦ | ç¾¤è |
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
 åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
-æå¨æ´æ°æ¯èµä¿¡æ¯ | ### ææå¾ [./docs/preview.webp]
+æå¨æ´æ°æ¯èµä¿¡æ¯ | | `cfçè§` | ç¾¤å | æ¯ | ç¾¤è |
+çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ | ç¾¤è |
+å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è |
+æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/nc.JPG]
+[./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG] [./
+docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/cfjianshiliebiao.JPG] [./docs/
+cfchaxun.JPG]
```

