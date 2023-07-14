# Comparing `tmp/herta_villa_sdk-0.5.0.tar.gz` & `tmp/herta_villa_sdk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.5.0.tar", last modified: Thu Jul 13 05:07:03 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.5.1.tar", last modified: Fri Jul 14 10:04:15 2023, max compression
```

## Comparing `herta_villa_sdk-0.5.0.tar` & `herta_villa_sdk-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1068 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0     4060 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/README.md
--rw-r--r--   0        0        0      668 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/__init__.py
--rw-r--r--   0        0        0      782 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/auth.py
--rw-r--r--   0        0        0     1387 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/base.py
--rw-r--r--   0        0        0      520 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/emoticon.py
--rw-r--r--   0        0        0     2174 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/member.py
--rw-r--r--   0        0        0     2710 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/message.py
--rw-r--r--   0        0        0     4422 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/role.py
--rw-r--r--   0        0        0     4190 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/room.py
--rw-r--r--   0        0        0      645 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/apis/villa.py
--rw-r--r--   0        0        0     7235 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/bot.py
--rw-r--r--   0        0        0     5398 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/event.py
--rw-r--r--   0        0        0      738 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     3799 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1414 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/message/types.py
--rw-r--r--   0        0        0     6280 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/model.py
--rw-r--r--   0        0        0      970 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/__init__.py
--rw-r--r--   0        0        0     1287 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/aiohttp.py
--rw-r--r--   0        0        0     1548 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/fastapi.py
--rw-r--r--   0        0        0     2888 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/server/internal.py
--rw-r--r--   0        0        0      564 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-07-13 05:06:36.222119 herta_villa_sdk-0.5.0/hertavilla/version.py
--rw-r--r--   0        0        0     2234 2023-07-13 05:07:03.270099 herta_villa_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      528 2023-07-13 05:06:36.226119 herta_villa_sdk-0.5.0/tests/test_utils.py
--rw-r--r--   0        0        0     4818 1970-01-01 00:00:00.000000 herta_villa_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4060 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/README.md
+-rw-r--r--   0        0        0      668 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0      782 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1491 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      520 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0      611 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/img.py
+-rw-r--r--   0        0        0     2174 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2710 2023-07-14 10:03:48.579653 herta_villa_sdk-0.5.1/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4422 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4190 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      645 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     7296 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/bot.py
+-rw-r--r--   0        0        0     5398 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/event.py
+-rw-r--r--   0        0        0     1016 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     3799 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1414 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6280 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/model.py
+-rw-r--r--   0        0        0      970 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/aiohttp.py
+-rw-r--r--   0        0        0     1548 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/fastapi.py
+-rw-r--r--   0        0        0     2888 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/server/internal.py
+-rw-r--r--   0        0        0      564 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/hertavilla/version.py
+-rw-r--r--   0        0        0     2234 2023-07-14 10:04:15.456239 herta_villa_sdk-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-07-14 10:03:48.583653 herta_villa_sdk-0.5.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4818 1970-01-01 00:00:00.000000 herta_villa_sdk-0.5.1/PKG-INFO
```

### Comparing `herta_villa_sdk-0.5.0/LICENSE` & `herta_villa_sdk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/README.md` & `herta_villa_sdk-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/__init__.py` & `herta_villa_sdk-0.5.1/hertavilla/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/auth.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/auth.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/base.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, Literal
 
-from hertavilla.exception import raise_exception
+from hertavilla.exception import HTTPStatusError, raise_exception
 
 from aiohttp import ClientSession
 
 logger = logging.getLogger("hertavilla.api")
 BASE_API = "https://bbs-api.miyoushe.com/vila/api/bot/platform"
 
 
@@ -38,10 +38,12 @@
             async with session.request(
                 method,
                 f"{BASE_API}{api}",
                 json=data,
                 params=params,
                 headers=self._make_header(villa_id) if villa_id else None,
             ) as resp:
+                if not resp.ok:
+                    raise HTTPStatusError(resp.status)
                 payload = await resp.json()
                 raise_exception(payload)
                 return payload["data"]
```

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/emoticon.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/emoticon.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/member.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/member.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/message.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/message.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/role.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/role.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/room.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/room.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/apis/villa.py` & `herta_villa_sdk-0.5.1/hertavilla/apis/villa.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/bot.py` & `herta_villa_sdk-0.5.1/hertavilla/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Coroutine,
     Generic,
     NamedTuple,
     TypeVar,
 )
 
 from hertavilla.apis.auth import AuthAPIMixin
+from hertavilla.apis.img import ImgAPIMixin
 from hertavilla.apis.member import MemberAPIMixin
 from hertavilla.apis.message import MessageAPIMixin
 from hertavilla.apis.role import RoleAPIMixin
 from hertavilla.apis.room import RoomAPIMixin
 from hertavilla.apis.villa import VillaAPIMixin
 from hertavilla.match import Endswith, Keywords, Match, Regex, Startswith
 
@@ -63,14 +64,15 @@
 class VillaBot(
     AuthAPIMixin,
     MemberAPIMixin,
     MessageAPIMixin,
     RoomAPIMixin,
     VillaAPIMixin,
     RoleAPIMixin,
+    ImgAPIMixin,
 ):
     def __init__(
         self,
         bot_id: str,
         secret: str,
         callback_endpoint: str,
         bot_info: "Template" | None = None,
```

### Comparing `herta_villa_sdk-0.5.0/hertavilla/event.py` & `herta_villa_sdk-0.5.1/hertavilla/event.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/exception.py` & `herta_villa_sdk-0.5.1/hertavilla/exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 from __future__ import annotations
 
 from typing import Any
 
 
-class _ExceptionWithRetcode(Exception):
+class SDKException(Exception):
+    ...
+
+
+class HTTPStatusError(SDKException):
+    def __init__(
+        self,
+        /,
+        status: int,
+    ) -> None:
+        self.status = status
+
+    def __repr__(self) -> str:
+        return "<HTTPStatusError status={self.status}"
+
+
+class _ExceptionWithRetcode(SDKException):
     def __init__(self, /, retcode: int, message: str) -> None:
         self.retcode = retcode
         self.message = message
 
     def to_dict(self):
         return {"retcode": self.retcode, "message": self.message}
```

### Comparing `herta_villa_sdk-0.5.0/hertavilla/match.py` & `herta_villa_sdk-0.5.1/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/message/chain.py` & `herta_villa_sdk-0.5.1/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/message/image.py` & `herta_villa_sdk-0.5.1/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/message/post.py` & `herta_villa_sdk-0.5.1/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/message/text.py` & `herta_villa_sdk-0.5.1/hertavilla/message/text.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/model.py` & `herta_villa_sdk-0.5.1/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/server/__init__.py` & `herta_villa_sdk-0.5.1/hertavilla/server/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/server/aiohttp.py` & `herta_villa_sdk-0.5.1/hertavilla/server/aiohttp.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/server/fastapi.py` & `herta_villa_sdk-0.5.1/hertavilla/server/fastapi.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/server/internal.py` & `herta_villa_sdk-0.5.1/hertavilla/server/internal.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/typing.py` & `herta_villa_sdk-0.5.1/hertavilla/typing.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/hertavilla/utils.py` & `herta_villa_sdk-0.5.1/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/pyproject.toml` & `herta_villa_sdk-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
 dynamic = []
-version = "0.5.0"
+version = "0.5.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Herta-villa/Herta-villa-SDK"
 Documentation = "https://github.com/Herta-villa/Herta-villa-SDK"
```

### Comparing `herta_villa_sdk-0.5.0/tests/test_utils.py` & `herta_villa_sdk-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.5.0/PKG-INFO` & `herta_villa_sdk-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.5.0
+Version: 0.5.1
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Repository, https://github.com/Herta-villa/Herta-villa-SDK
```

