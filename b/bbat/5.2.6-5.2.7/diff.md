# Comparing `tmp/bbat-5.2.6.tar.gz` & `tmp/bbat-5.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-5.2.6.tar", last modified: Wed Jul 12 02:28:31 2023, max compression
+gzip compressed data, was "bbat-5.2.7.tar", last modified: Fri Jul 14 08:32:41 2023, max compression
```

## Comparing `bbat-5.2.6.tar` & `bbat-5.2.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.430219 bbat-5.2.6/
--rw-rw-rw-   0        0        0      289 2023-07-12 02:28:31.428220 bbat-5.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.382219 bbat-5.2.6/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.6/bbat/__init__.py
--rw-rw-rw-   0        0        0     1720 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/config.py
--rw-rw-rw-   0        0        0     3085 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/crypto.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 01:11:37.000000 bbat-5.2.6/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.402223 bbat-5.2.6/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.6/bbat/db/aio_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/db/aio_sqlite.py
--rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.6/bbat/db/mysql.py
--rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-11 01:47:46.000000 bbat-5.2.6/bbat/image.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.405219 bbat-5.2.6/bbat/llm/
--rw-rw-rw-   0        0        0        0 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/llm/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/llm/chatgpt.py
--rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.6/bbat/log.py
--rw-rw-rw-   0        0        0      822 2023-07-11 01:47:51.000000 bbat-5.2.6/bbat/machine.py
--rw-rw-rw-   0        0        0     1868 2023-07-11 02:21:26.000000 bbat-5.2.6/bbat/notice.py
--rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.6/bbat/np.py
--rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.6/bbat/path.py
--rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.6/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.414222 bbat-5.2.6/bbat/web/
--rw-rw-rw-   0        0        0        0 2023-07-11 01:54:28.000000 bbat-5.2.6/bbat/web/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-07-11 01:55:27.000000 bbat-5.2.6/bbat/web/client.py
--rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/cors.py
--rw-rw-rw-   0        0        0     3929 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/flask_app.py
--rw-rw-rw-   0        0        0     1566 2023-07-11 01:11:37.000000 bbat-5.2.6/bbat/web/sanic_app.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.424222 bbat-5.2.6/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.6/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7552 2023-07-10 07:04:45.000000 bbat-5.2.6/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.6/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.6/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.6/bbat/web/url_to_sql/where.py
--rw-rw-rw-   0        0        0     2156 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/zcli.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.395221 bbat-5.2.6/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 02:28:31.430219 bbat-5.2.6/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-07-12 02:28:27.000000 bbat-5.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.427221 bbat-5.2.6/test/
--rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.6/test/test_config.py
--rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.6/test/test_db_mysql.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.891872 bbat-5.2.7/
+-rw-rw-rw-   0        0        0      289 2023-07-14 08:32:41.891872 bbat-5.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.837277 bbat-5.2.7/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.7/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1720 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/config.py
+-rw-rw-rw-   0        0        0     3085 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/crypto.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 01:11:37.000000 bbat-5.2.7/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.860872 bbat-5.2.7/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.7/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.7/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-11 01:47:46.000000 bbat-5.2.7/bbat/image.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.863875 bbat-5.2.7/bbat/llm/
+-rw-rw-rw-   0        0        0        0 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/llm/__init__.py
+-rw-rw-rw-   0        0        0     2387 2023-07-13 04:46:10.000000 bbat-5.2.7/bbat/llm/chatgpt.py
+-rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.7/bbat/log.py
+-rw-rw-rw-   0        0        0      828 2023-07-12 02:35:59.000000 bbat-5.2.7/bbat/machine.py
+-rw-rw-rw-   0        0        0     1868 2023-07-11 02:21:26.000000 bbat-5.2.7/bbat/notice.py
+-rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.7/bbat/np.py
+-rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.7/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.7/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.874874 bbat-5.2.7/bbat/web/
+-rw-rw-rw-   0        0        0        0 2023-07-11 01:54:28.000000 bbat-5.2.7/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-07-11 01:55:27.000000 bbat-5.2.7/bbat/web/client.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     3929 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      178 2023-07-13 05:18:31.000000 bbat-5.2.7/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1566 2023-07-11 01:11:37.000000 bbat-5.2.7/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.885874 bbat-5.2.7/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.7/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7552 2023-07-10 07:04:45.000000 bbat-5.2.7/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.7/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.7/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.7/bbat/web/url_to_sql/where.py
+-rw-rw-rw-   0        0        0     1614 2023-07-12 09:36:02.000000 bbat-5.2.7/bbat/zcli.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.855872 bbat-5.2.7/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 08:32:41.892874 bbat-5.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-07-14 08:32:38.000000 bbat-5.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.889874 bbat-5.2.7/test/
+-rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.7/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.7/test/test_db_mysql.py
```

### Comparing `bbat-5.2.6/bbat/config.py` & `bbat-5.2.7/bbat/config.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/crypto.py` & `bbat-5.2.7/bbat/crypto.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/date.py` & `bbat-5.2.7/bbat/date.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/db/aio_mysql.py` & `bbat-5.2.7/bbat/db/aio_mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/db/aio_sqlite.py` & `bbat-5.2.7/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/db/mysql.py` & `bbat-5.2.7/bbat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/image.py` & `bbat-5.2.7/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/llm/chatgpt.py` & `bbat-5.2.7/bbat/llm/chatgpt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 import openai
 
 openai.api_key = ''
 openai.proxy = {
     'http': '127.0.0.1:10809',
     'https': '127.0.0.1:10809',
 }
@@ -10,52 +11,47 @@
 def generate(messages, stream=True, **kwargs):
     # 避免传入的messages内容过大，保持最新的5条数据
     params = dict(
         model = 'gpt-3.5-turbo',
         # 控制输出的多样性，0-1，其中0表示最保守的输出，1表示最多样化的输出。
         temperature=0.5,
         # 输出的最大长度（输入+输出的token不能大于模型的最大token）,可以动态调整
-        max_tokens=1500,
+        max_tokens=512,
         # [控制字符的重复度] -2.0 ~ 2.0 之间的数字，正值会根据新 tokens 在文本中的现有频率对其进行惩罚，从而降低模型逐字重复同一行的可能性
         frequency_penalty=0.2,
         # [控制主题的重复度] -2.0 ~ 2.0 之间的数字，正值会根据到目前为止是否出现在文本中来惩罚新 tokens，从而增加模型谈论新主题的可能性
         presence_penalty=0.15,
     )
     params.update(kwargs)
-
     try:
         if stream == True:
             response = openai.ChatCompletion.create(
                 messages=messages,
                 stream=True,
                 **params
             )
-            content = {'role': '', 'content': ''}
+            # content = {'role': '', 'content': ''}
             for event in response:
                 if event['choices'][0]['finish_reason'] == 'stop':
-                    # print(f'收到的完成数据: {content}')
-                    # break
-                    return  content
-                for delta_k, delta_v in event['choices'][0]['delta'].items():
-                    yield delta_k, delta_v
-                    # print(f'流响应数据: {delta_k} = {delta_v}')
-                    content[delta_k] += delta_v
+                    return None
+                for delta_v in event['choices'][0]['delta'].get('content', ''):
+                    yield delta_v
         else:
             response = openai.ChatCompletion.create(
                 messages=messages,
                 **params
             )
             messages.append({
                 "role": response['choices'][0]['message']['role'],
                 "content": response['choices'][0]['message']['content']
             })
             msg = response['choices'][0]['message']
-            print(f'{msg}')
             return msg
     except Exception as err:
+        traceback.print_exc()
         print(f'OpenAI API 异常: {err}')
         return None
 
 
 if __name__ == '__main__':
     messages = [{'role': 'user', 'content': 'Hello!'}]
     for role, content in generate(messages):
```

### Comparing `bbat-5.2.6/bbat/log.py` & `bbat-5.2.7/bbat/log.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/machine.py` & `bbat-5.2.7/bbat/machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 import numpy as np
 import psutil
 
 def info():
     cpu_per = psutil.cpu_percent(True, True)
+    
     cpu_per = round(np.array(cpu_per).mean(), 2)
     mem = psutil.virtual_memory()
     cpu_num = psutil.cpu_count(logical=True)
     mem_total = round(mem.total / 2 ** 32, 2)
     mem_per = round(mem.percent, 2)
     disk = []
     partitions = psutil.disk_partitions()
```

### Comparing `bbat-5.2.6/bbat/notice.py` & `bbat-5.2.7/bbat/notice.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/np.py` & `bbat-5.2.7/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/path.py` & `bbat-5.2.7/bbat/path.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/text.py` & `bbat-5.2.7/bbat/text.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/client.py` & `bbat-5.2.7/bbat/web/client.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/db_server.py` & `bbat-5.2.7/bbat/web/db_server.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/sanic_app.py` & `bbat-5.2.7/bbat/web/sanic_app.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/url_to_sql/field.py` & `bbat-5.2.7/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/url_to_sql/query.py` & `bbat-5.2.7/bbat/web/url_to_sql/query.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/url_to_sql/relation.py` & `bbat-5.2.7/bbat/web/url_to_sql/relation.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/url_to_sql/test.py` & `bbat-5.2.7/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/url_to_sql/util.py` & `bbat-5.2.7/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/web/url_to_sql/where.py` & `bbat-5.2.7/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/bbat/zcli.py` & `bbat-5.2.7/bbat/zcli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-import click
+import typer
 
-@click.group()
-def main():
-    pass
+main = typer.Typer()
 
 @main.command(help='hi')
 def hi():
     from bbat import hi
 
-@main.command(help='启动 db http server')
-@click.option('--host', default='localhost', help="Database params")
-@click.option('--port', default=3306, type=int, help="Database params")
-@click.option('--user', default='root', help="Database params")
-@click.option('--password', default='123456', help="Database params")
-@click.option('--database', default='project', help="Database params")
-def server(host, port, user, password, database):
+@main.command()
+def server(host='localhost', port:int=3306, user='root', password='123456', database='project'):
     from bbat.web.db_server import app
     from bbat.db.aio_mysql import Mysql
     
     print('>>>', f"mysql://{user}:{password}@{host}:{port}/{database}")
     db = Mysql(host, port, database, user, password)
     app.ctx.db = db
     app.run()
 
 
 
 @main.command(help='md5加密')
-@click.argument('val')
 def md5(val):
     from bbat.crypto import md5
     print(md5(val))
 
 
-@main.command(help='md5加密')
-@click.argument('val')
-@click.option('-d', '--decode', is_flag=True, help="base64解密")
-def base64(val, decode):
+@main.command(help='base64加密，解密--decode')
+def base64(val, decode:bool=False):
     from bbat.crypto import base64_encode, base64_decode
     if decode:
         print(base64_decode(val))
         return 
     print(base64_encode(val))
 
 
@@ -47,30 +37,27 @@
 @main.command(help='机器--配置/使用量')
 def machine():
     from bbat.machine import info
     [print(name, value) for name, value in info().items()]
 
 
 @main.command(help='命令行chatGPT聊天')
-@click.option('-k', '--key', default="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", help="base64解密")
-@click.argument('val')
-def chatgpt(val, key):
+def chatgpt(val, key="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"):
     from bbat.llm.chatgpt import generate
     import openai
     
     openai.api_key = key
     messages = [{'role': 'user', 'content': val}]
     for role, content in generate(messages):
         if role == 'role':
             continue
         print(content, flush=True, end="")
 
 
 @main.command(help='有道翻译')
-@click.argument('val')
 def translate(val):
     from bbat.text import Translator
     translator = Translator()
     print(translator(val), '\n')
 
 
 if __name__ == "__main__":
```

### Comparing `bbat-5.2.6/bbat.egg-info/SOURCES.txt` & `bbat-5.2.7/bbat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbat-5.2.6/setup.py` & `bbat-5.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 name = "bbat"
-version = "5.2.6"
+version = "5.2.7"
 
 setuptools.setup(
     name=name,
     version=version,
     author="zlge",
     author_email="test@test.com",
     description="",
```

