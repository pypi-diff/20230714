# Comparing `tmp/aikopanel-bot-1.1.tar.gz` & `tmp/aikopanel-bot-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikopanel-bot-1.1.tar", last modified: Fri Jul 14 14:35:26 2023, max compression
+gzip compressed data, was "aikopanel-bot-1.2.tar", last modified: Fri Jul 14 16:16:35 2023, max compression
```

## Comparing `aikopanel-bot-1.1.tar` & `aikopanel-bot-1.2.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/Commands/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/bind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/buyplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/checkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/getapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/idapple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/myinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/myinvite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/mysub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/myusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/sni.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/topserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/topused.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/unbind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/website.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Commands/yesterdayorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/Modules/ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/aikopanel_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 14:35:26.000000 aikopanel-bot-1.1/aikopanel_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:35:26.544413 aikopanel-bot-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 14:35:12.000000 aikopanel-bot-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/Commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/buyplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/checkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/getapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/idapple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/myinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/myinvite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/mysub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/myusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/sni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/topserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/topused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Commands/website.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/Modules/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/aikopanel_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 16:16:35.000000 aikopanel-bot-1.2/aikopanel_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:16:35.842570 aikopanel-bot-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 16:16:21.000000 aikopanel-bot-1.2/setup.py
```

### Comparing `aikopanel-bot-1.1/Commands/bind.py` & `aikopanel-bot-1.2/Commands/bind.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/buyplan.py` & `aikopanel-bot-1.2/Commands/buyplan.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/check.py` & `aikopanel-bot-1.2/Commands/check.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/checkinfo.py` & `aikopanel-bot-1.2/Commands/checkinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/getapp.py` & `aikopanel-bot-1.2/Commands/getapp.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/idapple.py` & `aikopanel-bot-1.2/Commands/idapple.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/myinfo.py` & `aikopanel-bot-1.2/Commands/myinfo.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/myinvite.py` & `aikopanel-bot-1.2/Commands/myinvite.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/mysub.py` & `aikopanel-bot-1.2/Commands/mysub.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/myusage.py` & `aikopanel-bot-1.2/Commands/myusage.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/ping.py` & `aikopanel-bot-1.2/Commands/ping.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/sni.py` & `aikopanel-bot-1.2/Commands/sni.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/start.py` & `aikopanel-bot-1.2/Commands/start.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from telegram.ext import ContextTypes
 
 desc = 'Bắt dầu với bot'
 config = aikopanel_bot.config['bot']
 
 
 def getContent():
-    text = '🗺*Chào mừng bạn đến với Bot quản lý của Aiko*\n\n🏁Cách sử dụng bot : `/bind User Pass`\n📮user: là tài khoản DK trên web (mail)\n🔑Pass: mật khẩu login trên web Aiko\n\n!!! Lưu ý: Hãy IBox riêng với bot để bảo mật thông tin\n\n🌐Nhấp vào nút bên dưới để nhắn tin riêng với bot'
+    text = f'🗺*Chào mừng bạn đến với Bot quản lý của {config["website"]}*\n\n🏁Cách sử dụng bot : `/bind User Pass`\n📮user: là tài khoản DK trên web (mail)\n🔑Pass: mật khẩu login trên web Aiko\n\n!!! Lưu ý: Hãy IBox riêng với bot để bảo mật thông tin\n\n🌐Nhấp vào nút bên dưới để nhắn tin riêng với bot'
     keyboard = [[InlineKeyboardButton(
         text='AikoPanel Bot', url=f'https://t.me/{config["username_bot"]}')]]
     reply_markup = InlineKeyboardMarkup(keyboard)
     return text, reply_markup
 
 
 async def autoDelete(context: ContextTypes.DEFAULT_TYPE) -> None:
```

### Comparing `aikopanel-bot-1.1/Commands/topserver.py` & `aikopanel-bot-1.2/Commands/topserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     send_user = True
     index = 10
     send_order = True
 
 def getTimestemp():
     yesterday = (datetime.datetime.now(timezone) - datetime.timedelta(days=1)).strftime("%d-%m-%Y")
     inconvert = datetime.datetime.strptime(yesterday, "%d-%m-%Y")
-    timestemp = int(calendar.timegm(inconvert.timetuple()) + 25200)  # Add 7 hours in seconds
+    timestemp = int(calendar.timegm(inconvert.timetuple()) - 25200)  # Add 7 hours in seconds
     return timestemp
 
 
 def onSendServer():
     result = onQuery(
         "SELECT server_id, server_type, u, d FROM v2_stat_server WHERE record_at = %s" % getTimestemp())
     if result is None or len(result) == 0:
```

### Comparing `aikopanel-bot-1.1/Commands/topused.py` & `aikopanel-bot-1.2/Commands/topused.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     send_user = True
     index = 10
     send_order = True
 
 def getTimestemp():
     yesterday = (datetime.datetime.now(timezone) - datetime.timedelta(days=1)).strftime("%d-%m-%Y")
     inconvert = datetime.datetime.strptime(yesterday, "%d-%m-%Y")
-    timestemp = int(calendar.timegm(inconvert.timetuple()) + 25200)  # Add 7 hours in seconds
+    timestemp = int(calendar.timegm(inconvert.timetuple()) - 25200)
     return timestemp
 
 def onSendUser():
     # Get the data from the database
     result = onQuery(
         "SELECT user_id, u, d FROM v2_stat_user WHERE record_at = %s" % getTimestemp())
     if result is None or len(result) == 0:
@@ -51,15 +51,15 @@
     index = min(Settings.index, len(result_list))
     text = f'Trước khi sử dụng {index} Tên người dùng:\n\n'
     for i in range(index):
         user = onQuery("SELECT * FROM v2_user WHERE id = %s" % result_list[i][0])
         total = round(result_list[i][1] / 1024 / 1024 / 1024, 2)
         # Display the first 5 characters of the user's email
         email_start = user[0][3][:5]
-        text += f'{email_start}...@aikocute.tech - {total} GB\n'
+        text += f'{email_start}...@{config["website"]} - {total} GB\n'
     return text
 
 
 async def exec(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     msg = update.effective_message
     user_id = msg.from_user.id
     chat_id = msg.chat_id
```

### Comparing `aikopanel-bot-1.1/Commands/unbind.py` & `aikopanel-bot-1.2/Commands/unbind.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Commands/website.py` & `aikopanel-bot-1.2/Commands/website.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,12 +25,16 @@
 async def exec(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     msg = update.effective_message
     chat_id = msg.chat_id
     chat_type = update.effective_chat.type
     if chat_type == 'private' or chat_id == config['group_id']:
         text, reply_markup = getContent()
         # Send the QR code image with caption
-        with open(os.path.join(".", "image", "qrweb.jpg"), 'rb') as photo:
-            await context.bot.send_photo(chat_id, photo, caption=text, reply_markup=reply_markup)
+        # with open(os.path.join(".", "image", "qrweb.jpg"), 'rb') as photo:
+        #     await context.bot.send_photo(chat_id, photo, caption=text, reply_markup=reply_markup)
+        if config['qr_website'] is None:
+            await msg.reply_markdown(text, reply_markup=reply_markup)
+        else:
+            await context.bot.send_photo(chat_id, photo="%s" % config['qr_website'], caption=text, reply_markup=reply_markup)
         if chat_type != 'private':
             context.job_queue.run_once(
                 autoDelete, 300, data=msg.id, chat_id=chat_id, name=str(msg.id))
```

### Comparing `aikopanel-bot-1.1/LICENSE` & `aikopanel-bot-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Modules/daily.py` & `aikopanel-bot-1.2/Modules/daily.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         db.close()
         return result
 
 
 def getTimestemp():
     yesterday = (datetime.datetime.now(timezone) - datetime.timedelta(days=1)).strftime("%d-%m-%Y")
     inconvert = datetime.datetime.strptime(yesterday, "%d-%m-%Y")
-    timestemp = int(calendar.timegm(inconvert.timetuple()) + 25200)  # Add 7 hours in seconds
+    timestemp = int(calendar.timegm(inconvert.timetuple()) - 25200)  # Add 7 hours in seconds
     return timestemp
 
 
 def onSendServer():
     result = onQuery(
         "SELECT server_id, server_type, u, d FROM v2_stat_server WHERE record_at = %s" % getTimestemp())
     if result is None or len(result) == 0:
```

### Comparing `aikopanel-bot-1.1/Modules/order.py` & `aikopanel-bot-1.2/Modules/order.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/Modules/ticket.py` & `aikopanel-bot-1.2/Modules/ticket.py`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/PKG-INFO` & `aikopanel-bot-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanel-bot
-Version: 1.1
+Version: 1.2
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanel-bot-1.1/README.md` & `aikopanel-bot-1.2/README.md`

 * *Files identical despite different names*

### Comparing `aikopanel-bot-1.1/aikopanel_bot.egg-info/PKG-INFO` & `aikopanel-bot-1.2/aikopanel_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aikopanel-bot
-Version: 1.1
+Version: 1.2
 Summary: Description of the aikopanel-bot project
 Home-page: https://github.com/Github-Aiko/AikoPanel-bot
 Author: AikoCute
 Author-email: aiko@aikocute.tech
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aikopanel-bot-1.1/aikopanel_bot.egg-info/SOURCES.txt` & `aikopanel-bot-1.2/aikopanel_bot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 Commands/ping.py
 Commands/sni.py
 Commands/start.py
 Commands/topserver.py
 Commands/topused.py
 Commands/unbind.py
 Commands/website.py
-Commands/yesterdayorder.py
 Modules/__init__.py
 Modules/daily.py
 Modules/order.py
 Modules/ticket.py
 aikopanel_bot.egg-info/PKG-INFO
 aikopanel_bot.egg-info/SOURCES.txt
 aikopanel_bot.egg-info/dependency_links.txt
```

### Comparing `aikopanel-bot-1.1/setup.py` & `aikopanel-bot-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='aikopanel-bot',
-    version='1.1',
+    version='1.2',
     author='AikoCute',
     author_email='aiko@aikocute.tech',
     description='Description of the aikopanel-bot project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Github-Aiko/AikoPanel-bot',
     packages=find_packages(),
```

