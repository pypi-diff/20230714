# Comparing `tmp/botoy-9.1.tar.gz` & `tmp/botoy-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/botoy-9.1.tar", last modified: Fri Jun  2 01:05:39 2023, max compression
+gzip compressed data, was "dist/botoy-9.2.tar", last modified: Fri Jul 14 14:17:21 2023, max compression
```

## Comparing `botoy-9.1.tar` & `botoy-9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 01:05:28.000000 botoy-9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-02 01:05:39.000000 botoy-9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-02 01:05:28.000000 botoy-9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 01:05:28.000000 botoy-9.1/botoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 01:05:28.000000 botoy-9.1/botoy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-02 01:05:28.000000 botoy-9.1/botoy/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44649 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/_internal/config/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/config/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/contrib.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/mahiro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy/_internal/models/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/models/friend_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/models/group_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-02 01:05:28.000000 botoy-9.1/botoy/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 01:05:39.000000 botoy-9.1/botoy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 01:05:28.000000 botoy-9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:05:39.000000 botoy-9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-02 01:05:28.000000 botoy-9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:21.000000 botoy-9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 14:17:10.000000 botoy-9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-14 14:17:21.000000 botoy-9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-14 14:17:10.000000 botoy-9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:21.000000 botoy-9.2/botoy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-14 14:17:10.000000 botoy-9.2/botoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 14:17:10.000000 botoy-9.2/botoy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-14 14:17:10.000000 botoy-9.2/botoy/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:21.000000 botoy-9.2/botoy/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44379 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:21.000000 botoy-9.2/botoy/_internal/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/mahiro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:21.000000 botoy-9.2/botoy/_internal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/models/friend_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/models/group_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-14 14:17:10.000000 botoy-9.2/botoy/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 14:17:21.000000 botoy-9.2/botoy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 14:17:10.000000 botoy-9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:17:21.000000 botoy-9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-14 14:17:10.000000 botoy-9.2/setup.py
```

### Comparing `botoy-9.1/PKG-INFO` & `botoy-9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botoy
-Version: 9.1
+Version: 9.2
 Summary: OPQBot/IOTQQ/IOTBot的Python开发助手
 Home-page: https://github.com/xiyaowong/botoy
 Author: wongxy
 Author-email: xiyao.wong@foxmail.com
 License: MIT
 Description: # botoy
```

### Comparing `botoy-9.1/README.md` & `botoy-9.2/README.md`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/__init__.py` & `botoy-9.2/botoy/__init__.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/__version__.py` & `botoy-9.2/botoy/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=C0415,C0413
 # type: ignore
-__version__ = "9.1"
+__version__ = "9.2"
 
 
 def check_version(daemon=True):
     def _check_version():
         from distutils.version import LooseVersion as V
         from xml.etree import ElementTree
```

### Comparing `botoy-9.1/botoy/_internal/action.py` & `botoy-9.2/botoy/_internal/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             # TODO: 自动获取qq号
             raise ValueError("bot qq不能为0，请通过参数指定或配置文件中指定")
             # self._qq = (await self.getAllBots())[0]
         return int(self._qq)
 
     def set_url(self, url):
         self.base_url = get_base_url(url)
+        self.c.base_url = self.base_url
 
     def set_qq(self, qq: int):
         self._qq = qq
 
     async def close(self):
         return await self.c.aclose()
 
@@ -292,15 +293,18 @@
         elif base64:
             req["Base64Buf"] = base64  # type: ignore
         elif path:
             req["FilePath"] = path  # type: ignore
         else:
             raise ValueError("缺少参数")
         data = await self.post(
-            self.build_request(req, "PicUp.DataUp"), timeout=60  # 这个timeout可能不能写死
+            self.build_request(req, "PicUp.DataUp"),
+            path="/v1/upload",
+            funcname="",
+            timeout=60,  # 这个timeout可能不能写死
         )
         return self.UploadResponse.parse_obj(data)
 
     class SendGroupPicResponse(BaseModel):
         MsgTime: int
         MsgSeq: int
 
@@ -1154,42 +1158,29 @@
         funcname: str,
         path: str,
         payload: Optional[dict] = None,
         params: Optional[dict] = None,
         timeout: Optional[int] = None,
     ):
         """基础请求方法, 提供部分提示信息，出错返回空字典，其他返回服务端响应结果"""
-
         async with lock:
             await asyncio.sleep(0.5)
 
         params = params or {}
         params["funcname"] = funcname
         if "qq" not in params:
             params["qq"] = await self.qq
 
         try:
-            request_task = asyncio.ensure_future(
-                self.c.request(
-                    method,
-                    httpx.URL(url=path, params=params),
-                    json=payload,
-                    timeout=timeout,
-                )
+            resp = await self.c.request(
+                method,
+                httpx.URL(url=path, params=params),
+                json=payload,
+                timeout=timeout,
             )
-
-            resp = None
-            async with lock:
-                try:
-                    resp = await asyncio.wait_for(request_task, 2)
-                except TimeoutError:
-                    pass
-            if resp is None or not request_task.done():
-                resp = await request_task
-
             # TODO: 处理更多细节
             resp_model = Response.parse_obj(resp.json())
             if resp_model.CgiBaseResponse.ErrMsg:
                 if resp_model.CgiBaseResponse.Ret == 0:
                     logger.success(resp_model.CgiBaseResponse.ErrMsg)
                 else:
                     logger.error(resp_model.CgiBaseResponse.ErrMsg)
```

### Comparing `botoy-9.1/botoy/_internal/cli.py` & `botoy-9.2/botoy/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/client.py` & `botoy-9.2/botoy/_internal/client.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/config/config.py` & `botoy-9.2/botoy/_internal/config/config.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/config/util.py` & `botoy-9.2/botoy/_internal/config/util.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/context.py` & `botoy-9.2/botoy/_internal/context.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/contrib.py` & `botoy-9.2/botoy/_internal/contrib.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/log.py` & `botoy-9.2/botoy/_internal/log.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/mahiro.py` & `botoy-9.2/botoy/_internal/mahiro.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/models/friend_msg.py` & `botoy-9.2/botoy/_internal/models/friend_msg.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/models/group_msg.py` & `botoy-9.2/botoy/_internal/models/group_msg.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/pool.py` & `botoy-9.2/botoy/_internal/pool.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/receiver.py` & `botoy-9.2/botoy/_internal/receiver.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/runner.py` & `botoy-9.2/botoy/_internal/runner.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/schedule.py` & `botoy-9.2/botoy/_internal/schedule.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/sugar.py` & `botoy-9.2/botoy/_internal/sugar.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy/_internal/utils.py` & `botoy-9.2/botoy/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `botoy-9.1/botoy.egg-info/PKG-INFO` & `botoy-9.2/botoy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botoy
-Version: 9.1
+Version: 9.2
 Summary: OPQBot/IOTQQ/IOTBot的Python开发助手
 Home-page: https://github.com/xiyaowong/botoy
 Author: wongxy
 Author-email: xiyao.wong@foxmail.com
 License: MIT
 Description: # botoy
```

### Comparing `botoy-9.1/botoy.egg-info/SOURCES.txt` & `botoy-9.2/botoy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botoy-9.1/setup.py` & `botoy-9.2/setup.py`

 * *Files identical despite different names*

