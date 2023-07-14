# Comparing `tmp/anicli_api-0.4.1.tar.gz` & `tmp/anicli_api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.4.1.tar", max compression
+gzip compressed data, was "anicli_api-0.4.2.tar", max compression
```

## Comparing `anicli_api-0.4.1.tar` & `anicli_api-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.1/README.MD
--rw-r--r--   0        0        0     2987 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/_http.py
--rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/_logger.py
--rw-r--r--   0        0        0     2474 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/base.py
--rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/player/__init__.py
--rw-r--r--   0        0        0      918 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/__template__.py
--rw-r--r--   0        0        0     2280 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/aniboom.py
--rw-r--r--   0        0        0     1179 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/animejoy.py
--rw-r--r--   0        0        0     3430 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/base.py
--rw-r--r--   0        0        0     1282 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/csst.py
--rw-r--r--   0        0        0     1394 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/dzen.py
--rw-r--r--   0        0        0     3930 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/kodik.py
--rw-r--r--   0        0        0     1875 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/mailru.py
--rw-r--r--   0        0        0     1290 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/okru.py
--rw-r--r--   0        0        0     1089 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/sibnet.py
--rw-r--r--   0        0        0     1145 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/player/sovetromantica.py
--rw-r--r--   0        0        0     1256 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/player/vkcom.py
--rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/source/__init__.py
--rw-r--r--   0        0        0     1254 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/source/__template__.py
--rw-r--r--   0        0        0     6196 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/source/anilibria.py
--rw-r--r--   0        0        0     9524 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/source/animego.py
--rw-r--r--   0        0        0     8455 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/source/animejoy.py
--rw-r--r--   0        0        0     5590 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/source/animevost.py
--rw-r--r--   0        0        0     6294 2023-05-15 08:38:52.517152 anicli_api-0.4.1/anicli_api/source/sovetromantica.py
--rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.1/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.1/anicli_api/tools/random_useragent.py
--rw-r--r--   0        0        0     2050 2023-05-15 08:39:54.655981 anicli_api-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 anicli_api-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4216 2023-05-15 08:36:21.974286 anicli_api-0.4.2/README.MD
+-rw-r--r--   0        0        0     2940 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/_http.py
+-rw-r--r--   0        0        0     1511 2023-05-15 08:36:21.974286 anicli_api-0.4.2/anicli_api/_logger.py
+-rw-r--r--   0        0        0     3242 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/base.py
+-rw-r--r--   0        0        0      615 2023-05-15 08:38:52.517152 anicli_api-0.4.2/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      921 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     2147 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0     1055 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3434 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1198 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1456 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     3894 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1837 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1697 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1106 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0     1139 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/sovetromantica.py
+-rw-r--r--   0        0        0     1527 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.4.2/anicli_api/source/__init__.py
+-rw-r--r--   0        0        0     2516 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     6163 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0    10586 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     8722 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     5543 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0     6462 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/source/sovetromantica.py
+-rw-r--r--   0        0        0       58 2023-05-15 08:36:21.974286 anicli_api-0.4.2/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     2704 2022-12-17 13:02:20.525429 anicli_api-0.4.2/anicli_api/tools/random_useragent.py
+-rw-r--r--   0        0        0      198 2023-07-14 17:47:29.562755 anicli_api-0.4.2/anicli_api/tools/utils.py
+-rw-r--r--   0        0        0     2342 2023-07-14 17:48:12.823988 anicli_api-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5483 1970-01-01 00:00:00.000000 anicli_api-0.4.2/PKG-INFO
```

### Comparing `anicli_api-0.4.1/README.MD` & `anicli_api-0.4.2/README.MD`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.1/anicli_api/_http.py` & `anicli_api-0.4.2/anicli_api/_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 This module contains httpx.Client and httpx.AsyncClient classes with the following settings:
 
-1. User-agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.114
+1. User-agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N)
+AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.114
 
 2. x-requested-with: XMLHttpRequest
 
 """
-import ssl
 from typing import Dict
 
 from httpx import AsyncClient, Client, Response
 
 from anicli_api._logger import logger
 
 HEADERS: Dict[str, str] = {
@@ -55,26 +55,22 @@
 def check_ddos_protect_hook(resp: Response):
     """
     Simple ddos protect check hook.
 
     If response return 403 code or server headers contains *cloudflare* or *ddos-guard* strings and
     **Connection = close,** throw ConnectionError traceback
     """
-    logger.debug(
-        "{} check DDOS protect :\nstatus [{}] {}", resp.url, resp.status_code, resp.headers
-    )
+    logger.debug("{} check DDOS protect :\nstatus [{}] {}", resp.url, resp.status_code, resp.headers)
     if (
         resp.headers.get("Server") in DDOS_SERVICES
         and resp.headers.get("Connection", None) == "close"
         or resp.status_code == 403
     ):
         logger.error("Ooops, {} have ddos protect :(", resp.url)
-        raise ConnectionError(
-            f"{resp.url} have '{resp.headers.get('Server', 'unknown')}' and return 403 code."
-        )
+        raise ConnectionError(f"{resp.url} have '{resp.headers.get('Server', 'unknown')}' and return 403 code.")
 
 
 class HTTPSync(Singleton, BaseHTTPSync):
     """
     Base singleton **sync** HTTP class with recommended config.
 
     Used in extractors and can configure at any point in the program"""
```

### Comparing `anicli_api-0.4.1/anicli_api/_logger.py` & `anicli_api-0.4.2/anicli_api/_logger.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.1/anicli_api/player/__init__.py` & `anicli_api-0.4.2/anicli_api/player/__init__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.1/anicli_api/player/__template__.py` & `anicli_api-0.4.2/anicli_api/player/__template__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from typing import List
 
-from scrape_schema.fields.regex import ReMatch
-
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
+# from scrape_schema import Parsel, Sc, sc_param
+
+
 __all__ = ["PlayerExtractor"]
 # url validator pattern
 _URL_EQ = re.compile(r"https?://(www\.)?.")
 # url validate decorator
 player_validator = url_validator(_URL_EQ)
```

### Comparing `anicli_api-0.4.1/anicli_api/player/aniboom.py` & `anicli_api-0.4.2/anicli_api/player/aniboom.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import json
 import re
-from html import unescape
 from typing import List
 
 from parsel import Selector
 
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 __all__ = ["Aniboom"]
@@ -16,15 +14,16 @@
 class Aniboom(BaseVideoExtractor):
     URL_RULE = _URL_EQ
     DEFAULT_HTTP_CONFIG = {"headers": {"referer": "https://animego.org/"}}
     VIDEO_HEADERS = {
         "Referer": "https://aniboom.one/",
         "Accept-Language": "ru-RU",
         "Origin": "https://aniboom.one",
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 "
+        "(KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
     }
 
     @player_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
         response = self.http.get(url).text
         return self._extract(response)
 
@@ -33,37 +32,33 @@
         async with self.a_http as client:
             response = (await client.get(url)).text
             return self._extract(response)
 
     def _extract(self, response: str) -> List[Video]:
         # if pre unescape response - parsel selector uncorrect get data-parameters attr
         sel = Selector(response)
-        jsn_string = sel.xpath('//*[@id="video"]/@data-parameters').get()
-        jsn = json.loads(unescape(jsn_string))  # type: ignore
+        jsn = sel.xpath('//*[@id="video"]/@data-parameters')
         # TODO create m3u8, dash URL parsers
-        if jsn.get("dash"):
-            return [
+        videos: List[Video] = []
+        if dash := jsn.jmespath("dash"):
+            videos.append(
                 Video(
                     type="mpd",
                     quality=1080,
-                    url=json.loads(jsn["dash"])["src"],
+                    url=dash.re(r"https:.*\.mpd")[0].replace("\\", ""),
                     headers=self.VIDEO_HEADERS,
-                ),
+                )
+            )
+        if hls := jsn.jmespath("hls"):
+            videos.append(
                 Video(
                     type="m3u8",
                     quality=1080,
-                    url=json.loads(jsn["hls"])["src"],
+                    url=hls.re(r"https:.*\.m3u8")[0].replace("\\", ""),
                     headers=self.VIDEO_HEADERS,
-                ),
-            ]
-        return [
-            Video(
-                type="m3u8",
-                quality=1080,
-                url=json.loads(jsn["hls"])["src"],
-                headers=self.VIDEO_HEADERS,
-            ),
-        ]
+                )
+            )
+        return videos
 
 
 if __name__ == "__main__":
     print(Aniboom().parse("https://aniboom.one/embed/6BmMbB7MxWO?episode=1&translation=30"))
```

### Comparing `anicli_api-0.4.1/anicli_api/player/animejoy.py` & `anicli_api-0.4.2/anicli_api/player/sibnet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import re
 from typing import List
 
-from scrape_schema.fields.regex import ReMatchList
-
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
-__all__ = ["AnimeJoy"]
-_URL_EQ = re.compile(r"https://(www\.)?animejoy\.ru/player")
+__all__ = ["SibNet"]
+_URL_EQ = re.compile(r"https?://(www\.)?video\.sibnet")
 player_validator = url_validator(_URL_EQ)
 
 
-class AnimeJoy(BaseVideoExtractor):
+class SibNet(BaseVideoExtractor):
     URL_RULE = _URL_EQ
 
     @player_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
-        return self._extract(url)
+        response = self.http.get(url).text
+        return self._extract(response)
 
     @player_validator
     async def a_parse(self, url: str, **kwargs) -> List[Video]:
-        return self._extract(url)
+        async with self.a_http as client:
+            response = (await client.get(url)).text
+            return self._extract(response)
 
     def _extract(self, response: str) -> List[Video]:
-        # some extract logic
-        url_1080, url_360 = ReMatchList(re.compile(r"](https?://(?:www\.)?.*?\.mp4)")).extract(
-            response
-        )
-        return [
-            Video(type="mp4", quality=1080, url=url_1080),
-            Video(type="mp4", quality=360, url=url_360),
-        ]
+
+        if path := re.search(r'"(?P<url>/v/.*?\.mp4)"', response):
+            url = f"https://video.sibnet.ru{path[1]}"
+            return [Video(type="mp4", quality=480, url=url, headers={"Referer": url})]
+        else:
+            raise IndexError("Failed parse sibnet")
 
 
 if __name__ == "__main__":
-    U = """https://animejoy.ru/player/playerjs.html?file=[1080p]https://noda3.cdnjoy.site/Tsunlise/KAZOKU/01-1080.mp4,[360p]https://noda3.cdnjoy.site/Tsunlise/KAZOKU/01-360.mp4"""
-    print(AnimeJoy().parse(U))
+    SibNet().parse("https://video.sibnet.ru/shell.php?videoid=4779967")
```

### Comparing `anicli_api-0.4.1/anicli_api/player/base.py` & `anicli_api-0.4.2/anicli_api/player/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             "type": self.type,
             "quality": self.quality,
             "url": self.url,
             "headers": self.headers,
         }
 
     def __str__(self):
-        return f"{self.type} {self.quality} {urlparse(self.url).netloc}"
+        return f"[{self.quality}] {urlparse(self.url).netloc}...{self.type}"
 
     def __hash__(self):
         return hash((self.type, self.quality, urlparse(self.url).netloc))
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `anicli_api-0.4.1/anicli_api/player/csst.py` & `anicli_api-0.4.2/anicli_api/player/csst.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """NOTE: THIS Extractor not work in RU"""
 import re
 from typing import List
 
-from scrape_schema.fields.regex import ReMatchListDict
-
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 __all__ = ["CsstOnline"]
 # url validator pattern
 _URL_EQ = re.compile(r"https?://(www\.)?csst\.online/embed/\d+")
 # url validate decorator
 player_validator = url_validator(_URL_EQ)
@@ -25,15 +23,13 @@
     @player_validator
     async def a_parse(self, url: str, **kwargs) -> List[Video]:
         async with self.a_http as client:
             response = (await client.get(url)).text
             return self._extract(response)
 
     def _extract(self, response: str) -> List[Video]:
-        url_data = ReMatchListDict(self.RE_URLS).extract(response)
-        return [
-            Video(type="mp4", quality=data["quality"], url=data["url"]) for data in url_data[:4]
-        ]
+        url_data = list(re.finditer(self.RE_URLS, response))
+        return [Video(type="mp4", quality=data["quality"], url=data["url"]) for data in url_data[:4]]
 
 
 if __name__ == "__main__":
     print(*CsstOnline().parse("https://csst.online/embed/487794"), sep="\n")
```

### Comparing `anicli_api-0.4.1/anicli_api/player/dzen.py` & `anicli_api-0.4.2/anicli_api/player/dzen.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import json
 import re
 from typing import List
 
+import chompjs
 from parsel import Selector
 
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 __all__ = ["Dzen"]
 _URL_EQ = re.compile(r"https://(www.)?dzen\.ru/embed/\w+\?")
 player_validator = url_validator(_URL_EQ)
@@ -24,18 +24,21 @@
         async with self.a_http as client:
             response = (await client.get(url)).text
             return self._extract(response)
 
     def _extract(self, response) -> List[Video]:
         sel = Selector(response)
         js_script = sel.xpath("//body/script/text()").get()  # type: ignore
-        jsn = js_script.strip().replace(");", "").replace("Sandbox.init(", "")  # type: ignore
-        jsn = json.loads(jsn)
+        jsn = chompjs.parse_js_object(js_script)
         url_audio = jsn["data"]["content"]["audio_source_url"]
         url_mpd = jsn["data"]["content"]["streams"][0]["url"]
         url_m3u8 = jsn["data"]["content"]["streams"][1]["url"]
 
         return [
             Video(type="audio", quality=0, url=url_audio),
             Video(type="mpd", quality=1080, url=url_mpd),
             Video(type="m3u8", quality=1080, url=url_m3u8),
         ]
+
+
+if __name__ == "__main__":
+    Dzen().parse("https://dzen.ru/embed/vh1fMeui3d3Y?from_block=partner&from=zen&mute=1&autoplay=0&tv=0")
```

### Comparing `anicli_api-0.4.1/anicli_api/player/kodik.py` & `anicli_api-0.4.2/anicli_api/player/kodik.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import re
 from base64 import b64decode
 from typing import Dict, List
 from urllib.parse import urlsplit
 
-from scrape_schema import BaseSchema, ScField
-from scrape_schema.fields.regex import ReMatch
+from scrape_schema import BaseSchema, Parsel, Sc, sc_param
 
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 __all__ = ["Kodik"]
 _URL_EQ = re.compile(r"https://(www\.)?\w{5,32}\.\w{2,6}/(?:seria|video|film)/\d+/\w+/\d{3,4}p")
 kodik_validator = url_validator(_URL_EQ)
 
 
 class _KodikPayload(BaseSchema):
     # first parse params for JSON request to .../gvi entrypoint
-    domain: ScField[str, ReMatch(r'var domain = "(.*?)";')]
-    d_sign: ScField[str, ReMatch(r'var d_sign = "(.*?)";')]
-    pd: ScField[str, ReMatch(r'var pd = "(.*?)";')]
-    ref: ScField[str, ReMatch(r'var ref = "(.*?)";')]
-    type: ScField[str, ReMatch(r"videoInfo.type = '(.*?)';")]
-    hash: ScField[str, ReMatch(r"videoInfo.hash = '(.*?)';")]
-    id: ScField[str, ReMatch(r"videoInfo.id = '(.*?)';")]
-    bad_user = property(lambda self: True)
-    info = property(lambda self: {})
+    domain: Sc[str, Parsel().re(r'var domain = "(.*?)";')[0]]
+    d_sign: Sc[str, Parsel().re(r'var d_sign = "(.*?)";')[0]]
+    pd: Sc[str, Parsel().re(r'var pd = "(.*?)";')[0]]
+    ref: Sc[str, Parsel().re(r'var ref = "(.*?)";')[0]]
+    type: Sc[str, Parsel().re(r"videoInfo.type = '(.*?)';")[0]]
+    hash: Sc[str, Parsel().re(r"videoInfo.hash = '(.*?)';")[0]]
+    id: Sc[str, Parsel().re(r"videoInfo.id = '(.*?)';")[0]]
+    bad_user = sc_param(lambda self: True)
+    info = sc_param(lambda self: {})
 
 
 class Kodik(BaseVideoExtractor):
     URL_RULE = _URL_EQ
 
     @staticmethod
     def _decode(url_encoded: str) -> str:
@@ -36,16 +35,15 @@
         # with characters that are shifted 13 places in the alphabetical order,
         # wrapping around to the beginning or end of the alphabet as necessary.
         # This is a basic form of a Caesar cipher, a type of substitution cipher.
 
         # Note: this solution writen by chatgpt
         def char_wrapper(e):
             return chr(
-                (ord(e.group(0)) + 13 - (65 if e.group(0) <= "Z" else 97)) % 26
-                + (65 if e.group(0) <= "Z" else 97)
+                (ord(e.group(0)) + 13 - (65 if e.group(0) <= "Z" else 97)) % 26 + (65 if e.group(0) <= "Z" else 97)
             )
 
         base64_url = re.sub(r"[a-zA-Z]", char_wrapper, url_encoded)
         if not base64_url.endswith("=="):
             base64_url += "=="
         return f"https:{b64decode(base64_url).decode()}"
```

### Comparing `anicli_api-0.4.1/anicli_api/player/mailru.py` & `anicli_api-0.4.2/anicli_api/player/mailru.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
-from typing import Dict, List
+from typing import List
 
 from httpx import Response
-from scrape_schema.fields.regex import ReMatch
 
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 __all__ = ["MailRu"]
 # url validator pattern
 _URL_EQ = re.compile(r"https?://(www\.)?my\.mail\.ru/video/embed")
 # url validate decorator
@@ -14,15 +13,16 @@
 
 
 class MailRu(BaseVideoExtractor):
     URL_RULE = _URL_EQ
     DEFAULT_HTTP_CONFIG = {
         "headers": {
             "Upgrade-Insecure-Requests": "1",
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,"
+            "Accept": "text/html,application/xhtml+xml,application/"
+            "xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,"
             "application/signed-exchange;v=b3;q=0.7",
         }
     }
 
     @player_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
         video_id = url.split("/")[-1]
```

### Comparing `anicli_api-0.4.1/anicli_api/player/okru.py` & `anicli_api-0.4.2/anicli_api/player/okru.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,55 @@
-#
-import json
 import re
-from html import unescape
-from typing import List
+from typing import Dict, List
 
+import chompjs
+import jmespath
 from parsel import Selector
 
-from anicli_api.player.base import ALL_QUALITIES, BaseVideoExtractor, Video, url_validator
+from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 _URL_EQ = re.compile(r"https://(www.)?ok\.ru/videoembed/\d+")
 player_validator = url_validator(_URL_EQ)
 
 
 class OkRu(BaseVideoExtractor):
     URL_RULE = _URL_EQ
+    _QUALITIES_TABLE: Dict[str, int] = {
+        "mobile": 144,
+        "lowest": 240,
+        "low": 360,
+        "sd": 480,
+        "hd": 720,
+        "full": 1080,
+    }
 
     @player_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
         response = self.http.get(url).text
         return self._extract(response)
 
     @player_validator
     async def a_parse(self, url: str, **kwargs) -> List[Video]:
         async with self.a_http as client:
             response = (await client.get(url)).text
             return self._extract(response)
 
     def _extract(self, response: str) -> List[Video]:
         sel = Selector(response)
-        raw_jsn = sel.xpath('//div[@class="vid-card_cnt h-mod"]/@data-options').get()
-        jsn_1 = json.loads(unescape(raw_jsn))  # type: ignore
-        json_metadata = json.loads(jsn_1["flashvars"]["metadata"])
-        return [
-            Video(type="m3u8", quality=q, url=data["url"])
-            for q, data in zip(ALL_QUALITIES, json_metadata["videos"])
-        ]
+        raw_jsn = sel.xpath('//div[@class="vid-card_cnt h-mod"]/@data-options').jmespath("flashvars.metadata").get()
+
+        if jsn := chompjs.parse_js_object(raw_jsn):
+            results: List[Dict[str, str]] = jmespath.search("videos[*].{name:name, url:url}", jsn)
+            videos: List[Video] = [
+                Video(
+                    type="mp4",
+                    quality=self._QUALITIES_TABLE.get(result["name"], 0),
+                    url=result["url"],
+                )
+                for result in results
+            ]
+            return videos
+        raise Exception("Failed extract video")
 
 
 if __name__ == "__main__":
-    OkRu().parse("https://ok.ru/videoembed/4998442453635")
+    print(OkRu().parse("https://ok.ru/videoembed/4998442453635"))
```

### Comparing `anicli_api-0.4.1/anicli_api/player/sibnet.py` & `anicli_api-0.4.2/anicli_api/player/sovetromantica.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import re
 from typing import List
 
-from scrape_schema.fields.regex import ReMatch
-
 from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
-__all__ = ["SibNet"]
-_URL_EQ = re.compile(r"https?://(www\.)?video\.sibnet")
+__all__ = ["SovietRomanticaPlayer"]
+# url validator pattern
+_URL_EQ = re.compile(r"https?://(www\.)?[a-z1-9]{1,6}\.sovetromantica\.com/(?:anime|dorama)/.*\.m3u8")
+# url validate decorator
 player_validator = url_validator(_URL_EQ)
 
 
-class SibNet(BaseVideoExtractor):
+class SovietRomanticaPlayer(BaseVideoExtractor):
     URL_RULE = _URL_EQ
 
     @player_validator
     def parse(self, url: str, **kwargs) -> List[Video]:
-        response = self.http.get(url).text
-        return self._extract(response)
+        # response = self.http.get(url)
+        return self._extract(url)
 
     @player_validator
     async def a_parse(self, url: str, **kwargs) -> List[Video]:
-        async with self.a_http as client:
-            response = (await client.get(url)).text
-            return self._extract(response)
-
-    def _extract(self, response: str) -> List[Video]:
-        path = ReMatch(re.compile(r'"(?P<url>/v/.*?\.mp4)"')).extract(response)
-        url = f"https://video.sibnet.ru{path}"
-        return [Video(type="mp4", quality=480, url=url, headers={"Referer": url})]
+        # async with self.a_http as client:
+        #    response = await client.get(url)
+        return self._extract(url)
+
+    def _extract(self, response) -> List[Video]:
+        # any extract logic
+        return [Video(type="m3u8", quality=1080, url=response)]
 
 
 if __name__ == "__main__":
-    SibNet().parse("https://video.sibnet.ru/shell.php?videoid=4779967")
+    SovietRomanticaPlayer().parse(
+        "https://scp1.sovetromantica.com/anime/1368_akuyaku-reijou-nanode-last-boss-wo-kattemimashita/episodes/subtitles/episode_1/episode_1.m3u8"
+    )
```

### Comparing `anicli_api-0.4.1/anicli_api/player/vkcom.py` & `anicli_api-0.4.2/anicli_api/player/vkcom.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import re
-from base64 import b64decode
-from typing import Dict, List
-from urllib.parse import urlsplit
+from typing import List
 
+import chompjs
+import jmespath
 from parsel import Selector
-from scrape_schema import BaseSchema, ScField
-from scrape_schema.fields.regex import ReMatch
 
-from anicli_api.player.base import ALL_QUALITIES, BaseVideoExtractor, Video, url_validator
+from anicli_api.player.base import BaseVideoExtractor, Video, url_validator
 
 _URL_EQ = re.compile(r"https://(www\.)?vk\.com/video_ext\.php\?")
 player_validator = url_validator(_URL_EQ)
 
 
 class VkCom(BaseVideoExtractor):
     URL_RULE = _URL_EQ
@@ -25,13 +23,20 @@
     async def a_parse(self, url: str, **kwargs) -> List[Video]:
         async with self.a_http as client:
             response = (await client.get(url)).text
             return self._extract(response)
 
     def _extract(self, response: str) -> List[Video]:
         sel = Selector(response)
-        videos = sel.xpath('//video[@id="video_player"]/source/@src').getall()
-        return [Video(type="mp4", quality=q, url=u) for q, u in zip(ALL_QUALITIES, videos)]
+        player_params = sel.xpath("//script/text()").re(r"var playerParams = (\{.*\})")[0]
+        jsn = chompjs.parse_js_object(player_params)["params"][0]
+        urls_keys = jmespath.search("keys(@)[?starts_with(@, 'url')]", jsn)
+        videos: List[Video] = [
+            Video(type="mp4", url=jsn[url_key], quality=int(url_key.lstrip("url"))) for url_key in urls_keys
+        ]
+        return videos
+        # videos = sel.xpath('//video[@id="video_player"]/source/@src').getall()
+        # return [Video(type="mp4", quality=q, url=u) for q, u in zip(ALL_QUALITIES, videos)]
 
 
 if __name__ == "__main__":
-    VkCom().parse("https://vk.com/video_ext.php?oid=793268683&id=456239019&hash=0f28589bfca114f7")
+    print(VkCom().parse("https://vk.com/video_ext.php?oid=793268683&id=456239019&hash=0f28589bfca114f7"))
```

### Comparing `anicli_api-0.4.1/anicli_api/source/anilibria.py` & `anicli_api-0.4.2/anicli_api/source/anilibria.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 from typing import Any, List, Optional
 from urllib.parse import urlsplit
 
-from anicli_api.base import (
-    BaseAnime,
-    BaseEpisode,
-    BaseExtractor,
-    BaseOngoing,
-    BaseSearch,
-    BaseSource,
-    MainSchema,
-)
+from anicli_api.base import BaseAnime, BaseEpisode, BaseExtractor, BaseOngoing, BaseSearch, BaseSource, MainSchema
 from anicli_api.player.base import Video
 
 
 class Anilibria:
     """Dummmy API interface
     https://github.com/anilibria/docs/blob/master/api_v2.md
     """
```

### Comparing `anicli_api-0.4.1/anicli_api/source/animego.py` & `anicli_api-0.4.2/anicli_api/source/animego.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,265 +1,272 @@
-from typing import Dict, List
+from typing import Dict, List, Tuple
 from urllib.parse import urlsplit
 
 from parsel import Selector
-from scrape_schema import ScField
-from scrape_schema.callbacks.parsel import crop_by_xpath_all as cbxa
-from scrape_schema.callbacks.parsel import get_attr, get_text, replace_text
-from scrape_schema.fields.parsel import ParselXPath, ParselXPathList
-
-from anicli_api.base import (
-    BaseAnime,
-    BaseEpisode,
-    BaseExtractor,
-    BaseOngoing,
-    BaseSearch,
-    BaseSource,
-)
+from scrape_schema import Parsel, Sc, sc_param
+
+from anicli_api.base import BaseAnime, BaseEpisode, BaseExtractor, BaseOngoing, BaseSearch, BaseSource
 
 
 class Extractor(BaseExtractor):
     BASE_URL = "https://animego.org"
 
     def search(self, query: str) -> List["Search"]:
         response = self.HTTP().get(f"{self.BASE_URL}/search/anime", params={"q": query})
-        return Search.from_crop_rule_list(
-            response.text,
-            crop_rule=cbxa(
+        chunks = (
+            Parsel()
+            .xpath(
                 "//div[@class='row']/div[@class='animes-grid-item col-6 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-ul-2']"
-            ),
+            )
+            .sc_parse(response.text)
         )
+        return [Search(chunk) for chunk in chunks.getall()]
 
     async def a_search(self, query: str) -> List["Search"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(f"{self.BASE_URL}search/anime", params={"q": query})
-            return Search.from_crop_rule_list(
-                response.text,
-                crop_rule=cbxa(
-                    "//div[@class='row']/div[@class='animes-grid-item col-6 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-ul-2']"
-                ),
+            chunks = (
+                Parsel()
+                .xpath(
+                    "//div[@class='row']/div[@class='animes-grid-item col-6 col-sm-6 col-md-4 col-lg-3 col-xl-2 "
+                    "col-ul-2']"
+                )
+                .getall()
+                .sc_parse(response.text)
             )
+            return [Search(chunk) for chunk in chunks]
+
+    @staticmethod
+    def _ongoing_clear_dupes(ongoings: List["Ongoing"]) -> List["Ongoing"]:
+        """remove url duplicates for decrease output result"""
+        result: Dict[Tuple[int, str], Ongoing] = {}
+        for ongoing in ongoings:
+            tuple_key = (ongoing.num, ongoing.url)
+            if not result.get(tuple_key, None):
+                result[tuple_key] = ongoing
+            else:
+                result[tuple_key].dub += f", {ongoing.dub}"
+        return list(result.values())
 
     def ongoing(self) -> List["Ongoing"]:
         response = self.HTTP().get(self.BASE_URL)
-        return Ongoing.from_crop_rule_list(
-            response.text, crop_rule=cbxa('//*[starts-with(@class, "last-update-item")]')
-        )
+        chunks = Parsel().xpath('//*[starts-with(@class, "last-update-item")]').getall().sc_parse(response.text)
+        return self._ongoing_clear_dupes([Ongoing(chunk) for chunk in chunks])
 
     async def a_ongoing(self) -> List["Ongoing"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.BASE_URL)
-            return Ongoing.from_crop_rule_list(
-                response.text, crop_rule=cbxa('//*[starts-with(@class, "last-update-item")]')
-            )
+            chunks = Parsel().xpath('//*[starts-with(@class, "last-update-item")]').getall().sc_parse(response.text)
+            return self._ongoing_clear_dupes([Ongoing(chunk) for chunk in chunks])
 
 
 class Search(BaseSearch):
-    thumbnail: ScField[str, ParselXPath("//a/div", callback=get_attr("data-original"))]
-    rating: ScField[
-        float,
-        ParselXPath(
-            "//div[@class='p-rate-flag__text']", default="0", callback=replace_text(",", ".")
-        ),
-    ]
-    name: ScField[
-        str, ParselXPath("//div[@class='text-gray-dark-6 small mb-1 d-none d-sm-block']/div")
+    title: Sc[
+        str,
+        Parsel().xpath("//div[@class='h5 font-weight-normal mb-2 card-title text-truncate']/a/@title").get(),
     ]
-    title: ScField[
+    url: Sc[
         str,
-        ParselXPath(
-            "//div[@class='h5 font-weight-normal mb-2 card-title text-truncate']/a",
-            callback=get_attr("title"),
-        ),
+        Parsel().xpath("//div[@class='h5 font-weight-normal mb-2 card-title text-truncate']/a/@href").get(),
+    ]
+    thumbnail: Sc[str, Parsel().xpath("//a/div/@data-original").get()]
+
+    rating: Sc[
+        float,
+        Parsel(default=0.0).xpath("//div[@class='p-rate-flag__text']/text()").get().sc_replace(",", "."),
     ]
-    url: ScField[
+    name: Sc[
         str,
-        ParselXPath(
-            "//div[@class='h5 font-weight-normal mb-2 card-title text-truncate']/a",
-            callback=get_attr("href"),
-        ),
+        Parsel().xpath("//div[@class='text-gray-dark-6 small mb-1 d-none d-sm-block']/div/text()").get(),
     ]
 
     def __str__(self):
-        return f"{self.title} {self.name} ({self.rating})"
+        return f"{self.title} [{self.name}] ({self.rating}/10)"
 
     def get_anime(self) -> "Anime":
         response = self.HTTP().get(self.url)
         return Anime(response.text)
 
     async def a_get_anime(self) -> "Anime":
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.url)
             return Anime(response.text)
 
 
 class Ongoing(BaseOngoing):
-    _thumb_style: ScField[
-        str, ParselXPath("//div[@class='img-square lazy br-50']", callback=get_attr("style"))
-    ]
-    title: ScField[str, ParselXPath("//span[@class='last-update-title font-weight-600']")]
-    episode: ScField[str, ParselXPath("//div[@class='font-weight-600 text-truncate']")]
-    dub: ScField[
-        str, ParselXPath("//div[@class='ml-3 text-right']/div[@class='text-gray-dark-6']")
-    ]
-    _onclick: ScField[str, ParselXPath("//div", callback=get_attr("onclick"))]
-
-    def __str__(self):
-        return f"{self.title} {self.episode} ({self.dub})"
+    _onclick: Sc[str, Parsel().xpath("//div/@onclick").get()]
+    _thumb_style: Sc[str, Parsel().xpath("//div[@class='img-square lazy br-50']/@style").get()]
 
-    @property
-    def thumbnail(self):
-        return self._thumb_style.replace("background-image: url(", "").replace(");", "")
+    title: Sc[str, Parsel().xpath("//span[@class='last-update-title font-weight-600']/text()").get()]
+    thumbnail: str = sc_param(lambda self: self._thumb_style.replace("background-image: url(", "").replace(");", ""))
 
-    @property
-    def url(self):
+    @sc_param
+    def url(self) -> str:
         path = self._onclick.replace("location.href='", "").replace("'", "")
         return f"https://animego.org{path}"
 
-    @property
-    def num(self):
-        return int(self.episode.replace(" серия", "").replace(" Серия", ""))
+    name: Sc[str, Parsel().xpath("//div[@class='font-weight-600 text-truncate']/text()").get()]
+    dub: Sc[
+        str,
+        Parsel().xpath("//div[@class='ml-3 text-right']/div[@class='text-gray-dark-6']/text()").get(),
+    ]
+
+    def __str__(self):
+        return f"{self.title} {self.name} ({self.dub})"
+
+    @sc_param
+    def num(self) -> int:
+        return int(self.name.replace(" серия", "").replace(" Серия", ""))
 
     def get_anime(self) -> "Anime":
         response = self.HTTP().get(self.url)
         return Anime(response.text)
 
     async def a_get_anime(self) -> "Anime":
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.url)
             return Anime(response.text)
 
 
 class Anime(BaseAnime):
-    rating: ScField[
-        float,
-        ParselXPath(
-            '//*[@id="itemRatingBlock"]/div[1]/div[2]/div[1]/span[1]',
-            default="0",
-            callback=replace_text(",", "."),
-        ),
-    ]
-    title: ScField[str, ParselXPath("//div[@class='anime-title']/div/h1")]
-    alt_titles: ScField[List[str], ParselXPathList('//ul[@class="list-unstyled small mb-0"]/li')]
-    # todo create normal structure
-    _raw_metadata: ScField[
-        str,
-        ParselXPath(
-            '//div[@class="anime-info"]/dl[@class="row"]',
-            callback=get_text(strip=True, deep=True, sep=" "),
-        ),
-    ]
-    url: ScField[str, ParselXPath("//html/head/link[@rel='canonical']", callback=get_attr("href"))]
-    description: ScField[
-        str,
-        ParselXPath(
-            "//div[@class='description pb-3']", callback=get_text(strip=True, sep=" ")
-        ),  # mobile agent
-        ParselXPath("//div[@data-readmore='content']", callback=get_text(strip=True, sep=" ")),
-    ]  # desktop agent
-    anime_id = property(lambda self: self.url.split("-")[-1])
+    _script_jmespath: Sc[Selector, Parsel(auto_type=False).xpath("//script[@type='application/ld+json']/text()")]
 
-    def __str__(self):
-        return f"{self.title} {self.alt_titles} ({self.rating})"
+    @sc_param
+    def title(self) -> str:
+        return self._script_jmespath.jmespath("name").get()
+
+    @sc_param
+    def alt_titles(self) -> List[str]:
+        return self._script_jmespath.jmespath("alternativeHeadline").getall()
+
+    episodes_available: Sc[int, Parsel(default=0).xpath("//dl/dd[2]").re(r"\d+")[0]]
+    thumbnail: Sc[str, Parsel().css("#content img").xpath("@src").get()]
+    _description: Sc[List[str], Parsel().xpath("//div[@data-readmore='content']/text()").getall()]  # mobile agent
+
+    @sc_param
+    def description(self) -> str:
+        return " ".join(s.strip() for s in self._description)
+
+    @sc_param
+    def genres(self) -> List[str]:
+        return self._script_jmespath.jmespath("genre").getall()
+
+    @sc_param
+    def episodes_total(self) -> int:
+        return int(self._script_jmespath.jmespath("numberOfEpisodes").get())
+
+    @sc_param
+    def aired(self) -> str:
+        if end_date := self._script_jmespath.jmespath("endDate").get():
+            return self._script_jmespath.jmespath("startDate").get() + " " + end_date
+        return self._script_jmespath.jmespath("startDate").get() + " " + " ?"
+
+    url: Sc[str, Parsel().xpath("//html/head/link[@rel='canonical']/@href").get()]
+    anime_id = sc_param(lambda self: self.url.split("-")[-1])
+
+    @sc_param
+    def rating(self) -> float:
+        return float(self._script_jmespath.jmespath("aggregateRating.ratingValue").get())
 
     @staticmethod
     def _get_dubbers(response: str) -> Dict[str, str]:
-        sel = Selector(response)
-        dubbers_id: List[str] = ParselXPathList(
-            '//*[@id="video-dubbing"]/span', callback=get_attr("data-dubbing")
-        ).extract(sel, type_=List[str])
-        dubbers_name: List[str] = ParselXPathList(
-            '//*[@id="video-dubbing"]/span', callback=get_text(deep=True, strip=True)
-        ).extract(sel)
+        # sel = Selector(response)
+        dubbers_id: List[str] = (
+            Parsel().xpath('//*[@id="video-dubbing"]/span/@data-dubbing').getall().sc_parse(response)
+        )
+        dubbers_name: List[str] = Parsel().xpath('//*[@id="video-dubbing"]/span/text()').getall().sc_parse(response)
         return dict(zip(dubbers_id, dubbers_name))
 
     def get_episodes(self) -> List["Episode"]:
-        response = (
-            self.HTTP()
-            .get(f"https://animego.org/anime/{self.anime_id}/player?_allow=true")
-            .json()["content"]
-        )
+        response = self.HTTP().get(f"https://animego.org/anime/{self.anime_id}/player?_allow=true").json()["content"]
 
         _dubbers_table = self._get_dubbers(response)
-        return Episode.from_crop_rule_list(
-            response,
-            crop_rule=cbxa('//*[@id="video-carousel"]/div/div'),
-            _dubbers_table=_dubbers_table,
-        )
+        chunks = Parsel().xpath('//*[@id="video-carousel"]/div/div').getall().sc_parse(response)
+        episodes = [Episode(chunk) for chunk in chunks]
+        for ep in episodes:
+            setattr(ep, "_dubbers_table", _dubbers_table)
+        return episodes
 
     async def a_get_episodes(self) -> List["Episode"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.url)
             _dubbers_table = self._get_dubbers(response)
-            return Episode.from_crop_rule_list(
-                response,
-                crop_rule=cbxa('//*[@id="video-carousel"]/div/div'),
-                _dubbers_table=_dubbers_table,
-            )
+            chunks = Parsel().xpath('//*[@id="video-carousel"]/div/div').getall().sc_parse(response)
+            episodes = [Episode(chunk) for chunk in chunks]
+            for ep in episodes:
+                setattr(ep, "_dubbers_table", _dubbers_table)
+            return episodes
 
 
 class Episode(BaseEpisode):
-    num: ScField[int, ParselXPath("//div", callback=get_attr("data-episode"))]
-    _episode_type: ScField[int, ParselXPath("//div", callback=get_attr("data-episode-type"))]
-    data_id: ScField[int, ParselXPath("//div", callback=get_attr("data-id"))]
-    title: ScField[str, ParselXPath("//div", callback=get_attr("data-episode-title"))]
-    released: ScField[str, ParselXPath("//div", callback=get_attr("data-episode-released"))]
+    num: Sc[int, Parsel().xpath("//div/@data-episode").get()]
+    title: Sc[str, Parsel().xpath("//div/@data-episode-title").get()]
+
+    _episode_type: Sc[int, Parsel().xpath("//div/@data-episode-type").get()]
     _dubbers_table: Dict[str, str]
+    data_id: Sc[int, Parsel().xpath("//div/@data-id").get()]
+    released: Sc[str, Parsel().xpath("//div/@data-episode-released").get()]
 
     def __str__(self):
         return f"{self.title} {self.num} {self.released}"
 
     def get_sources(self) -> List["Source"]:
         response = (
             self.HTTP()
             .get(
                 "https://animego.org/anime/series",
                 params={"dubbing": 2, "provider": 24, "episode": self.num, "id": self.data_id},
             )
             .json()["content"]
         )
-        return Source.from_crop_rule_list(
-            response,
-            crop_rule=cbxa(
-                '//*[@id="video-players"]/span',
-            ),
-            _dubbers_table=self._dubbers_table,
-        )
+
+        chunks = Parsel().xpath('//*[@id="video-players"]/span').getall().sc_parse(response)
+        sources = [Source(chunk) for chunk in chunks]
+        for source in sources:
+            setattr(source, "_dubbers_table", self._dubbers_table)
+        return sources
 
     async def a_get_sources(self) -> List["Source"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(
                 "https://animego.org/anime/series",
                 params={"dubbing": 2, "provider": 24, "episode": self.num, "id": self.data_id},
             ).json()["content"]
-            return Source.from_crop_rule_list(
-                response,
-                crop_rule=cbxa(
-                    '//*[@id="video-players"]/span',
-                ),
-                _dubbers_table=self._dubbers_table,
-            )
+            chunks = Parsel().xpath('//*[@id="video-players"]/span').getall().sc_parse(response)
+            sources = [Source(chunk) for chunk in chunks]
+            for source in sources:
+                setattr(source, "_dubbers_table", self._dubbers_table)
+            return sources
 
 
 class Source(BaseSource):
     _dubbers_table: Dict[str, str]
-    _url: ScField[str, ParselXPath("//span", callback=get_attr("data-player"))]
-    _data_provider: ScField[str, ParselXPath("//span", callback=get_attr("data-provider"))]
-    _data_provide_dubbing: ScField[
-        str, ParselXPath("//span", callback=get_attr("data-provide-dubbing"))
-    ]
-    name: ScField[str, ParselXPath("//span/span")]
-    url = property(lambda self: f"https:{self._url}")
-    dub = property(lambda self: self._dubbers_table.get(self._data_provide_dubbing))
+    _url: Sc[str, Parsel().xpath("//span/@data-player").get()]
+    _data_provider: Sc[str, Parsel().xpath("//span/@data-provider").get()]
+    _data_provide_dubbing: Sc[str, Parsel().xpath("//span/@data-provide-dubbing").get()]
+    name: Sc[str, Parsel().xpath("//span/span/@text").get()]
+    url = sc_param(lambda self: f"https:{self._url}")
+    dub = sc_param(lambda self: self._dubbers_table.get(self._data_provide_dubbing))
 
     def __str__(self):
         return f"{urlsplit(self.url).netloc} {self.name} ({self.dub})"
 
 
 if __name__ == "__main__":
+    import logging
+
+    logger = logging.getLogger("scrape_schema")
+    logger.setLevel(logging.DEBUG)
     ex = Extractor()
+    # res = ex.ongoing()
     res = ex.search("lain")
     an = res[0].get_anime()
-    episodes = an.get_episodes()
-    sss = episodes[0].get_sources()
-    vids = sss[0].get_videos()
-    print(*vids)
+    eps = an.get_episodes()
+    sources = eps[0].get_sources()
+    print()
+    # ongs = ex.ongoing()
+    # an2 = ongs[0].get_anime()
+    # print()
+    # episodes = an.get_episodes()
+    # sss = episodes[0].get_sources()
+    # vids = sss[0].get_videos()
+    # print(*vids)
```

### Comparing `anicli_api-0.4.1/anicli_api/source/animejoy.py` & `anicli_api-0.4.2/anicli_api/source/animejoy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 from typing import Dict, List, TypedDict
 from urllib.parse import urlsplit
 
-from parsel import Selector
-from scrape_schema import ScField
-from scrape_schema.callbacks.parsel import crop_by_xpath_all as cbxa
-from scrape_schema.callbacks.parsel import get_attr, get_text
-from scrape_schema.fields.parsel import ParselXPath, ParselXPathList
-
-from anicli_api.base import (
-    BaseAnime,
-    BaseEpisode,
-    BaseExtractor,
-    BaseOngoing,
-    BaseSearch,
-    BaseSource,
-)
+from scrape_schema import Parsel, Sc, sc_param
+
+from anicli_api.base import BaseAnime, BaseEpisode, BaseExtractor, BaseOngoing, BaseSearch, BaseSource
 
 _SourceDict = TypedDict("_SourceDict", {"player_id": str, "url": str, "name": str})
 
 
 class Extractor(BaseExtractor):
     BASE_URL = "https://animejoy.ru"
 
@@ -28,58 +17,56 @@
             self.HTTP()
             .post(
                 self.BASE_URL,
                 data={"story": query, "do": "search", "subaction": "search"},
             )
             .text
         )
-        return Search.from_crop_rule_list(
-            response,
-            crop_rule=cbxa('//*[@id="dle-content"]/article[@class="block story shortstory"]'),
+        chunks = (
+            Parsel()
+            .xpath('//*[@id="dle-content"]/article[@class="block story shortstory"]')
+            .getall()
+            .sc_parse(response)
         )
+        return [Search(ch) for ch in chunks]
 
     async def a_search(self, query: str) -> List["Search"]:
         async with self.HTTP_ASYNC() as client:
-            response = await client.post(
-                self.BASE_URL, data={"story": query, "do": "search", "subaction": "search"}
-            )
-            return Search.from_crop_rule_list(
-                response,
-                crop_rule=cbxa('//*[@id="dle-content"]/article[@class="block story shortstory"]'),
+            response = await client.post(self.BASE_URL, data={"story": query, "do": "search", "subaction": "search"})
+            chunks = (
+                Parsel()
+                .xpath('//*[@id="dle-content"]/article[@class="block story shortstory"]')
+                .getall()
+                .sc_parse(response)
             )
+            return [Search(ch) for ch in chunks]
 
     def ongoing(self) -> List["Ongoing"]:
         # ongoing entrypoint
         response = self.HTTP().get(self.BASE_URL).text
-        return Ongoing.from_crop_rule_list(
-            response, crop_rule=cbxa('//div[@id="dle-content"]/article')
-        )
+        chunks = Parsel().xpath('//div[@id="dle-content"]/article').getall().sc_parse(response)
+        return [Ongoing(ch) for ch in chunks]
 
     async def a_ongoing(self) -> List["Ongoing"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.BASE_URL)
-            return Ongoing.from_crop_rule_list(
-                response.text, crop_rule=cbxa('//div[@id="dle-content"]/article')
-            )
+            chunks = Parsel().xpath('//div[@id="dle-content"]/article').getall().sc_parse(response)
+            return [Ongoing(ch) for ch in chunks]
 
 
 class Search(BaseSearch):
-    url: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a', callback=get_attr("href"))]
-    title: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a')]
-    alt_name: ScField[
-        str, ParselXPath('//div[@class="blkdesc"]/p/span[@itemprop="alternativeHeadline"]')
-    ]
-    _thumbnail_path: ScField[str, ParselXPath('//div[@class="text"]/picture/img')]
-    _metadata: ScField[
-        List[str],
-        ParselXPathList(
-            '//div[@class="blkdesc"]/p[@class="zerop"]', callback=get_text(strip=True, deep=True)
-        ),
-    ]
-    thumbnail = property(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
+    url: Sc[str, Parsel().xpath('//div[@class="titleup"]/h2/a/@href').get()]
+    title: Sc[str, Parsel().xpath('//div[@class="titleup"]/h2/a/text()').get()]
+    alt_name: Sc[
+        str,
+        Parsel().xpath('//div[@class="blkdesc"]/p/span[@itemprop="alternativeHeadline"]/text()').get(),
+    ]
+    _thumbnail_path: Sc[str, Parsel().xpath('//div[@class="text"]/picture/img').get()]
+    _metadata: Sc[List[str], Parsel().xpath('//div[@class="blkdesc"]/p[@class="zerop"]/text()').getall()]
+    thumbnail = sc_param(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
 
     def get_anime(self) -> "Anime":
         response = self.HTTP().get(self.url).text
         return Anime(response)
 
     async def a_get_anime(self) -> "Anime":
         async with self.HTTP_ASYNC() as client:
@@ -87,29 +74,23 @@
             return Anime(response.text)
 
     def __str__(self):
         return f"{self.title} ({self.alt_name})"
 
 
 class Ongoing(BaseOngoing):
-    url: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a', callback=get_attr("href"))]
-    title: ScField[str, ParselXPath('//div[@class="titleup"]/h2/a')]
-    alt_name: ScField[
-        str, ParselXPath('//div[@class="blkdesc"]/p/span[@itemprop="alternativeHeadline"]')
-    ]
-    _thumbnail_path: ScField[
-        str, ParselXPath('//div[@class="text"]/picture/img', callback=get_attr("src"))
-    ]
-    _metadata: ScField[
-        List[str],
-        ParselXPathList(
-            '//div[@class="blkdesc"]/p[@class="zerop"]', callback=get_text(strip=True, deep=True)
-        ),
-    ]
-    thumbnail = property(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
+    url: Sc[str, Parsel().xpath('//div[@class="titleup"]/h2/a/@href').get()]
+    title: Sc[str, Parsel().xpath('//div[@class="titleup"]/h2/a/text()').get()]
+    alt_name: Sc[
+        str,
+        Parsel().xpath('//div[@class="blkdesc"]/p/span[@itemprop="alternativeHeadline"]/text()').get(),
+    ]
+    _thumbnail_path: Sc[str, Parsel().xpath('//div[@class="text"]/picture/img/@src').get()]
+    _metadata: Sc[List[str], Parsel().xpath('//div[@class="blkdesc"]/p[@class="zerop"]/text()').getall()]
+    thumbnail = sc_param(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
 
     def get_anime(self) -> "Anime":
         response = self.HTTP().get(self.url)
         return Anime(response)
 
     async def a_get_anime(self) -> "Anime":
         async with self.HTTP_ASYNC() as client:
@@ -117,73 +98,79 @@
             return Anime(response)
 
     def __str__(self):
         return f"{self.title} ({self.alt_name})"
 
 
 class Anime(BaseAnime):
-    title: ScField[str, ParselXPath('//h1[@class="h2 ntitle"]')]
-    alt_name: ScField[str, ParselXPath('//h2[@class="romanji"]')]
-    _thumbnail_path: ScField[
-        str, ParselXPath('//div[@class="text"]/picture/img', callback=get_attr("src"))
-    ]
-    thumbnail = property(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
-    _metadata: ScField[List[str], ParselXPathList('//div[@class="blkdesc"]/p[@class="zerop"]')]
-    description: ScField[
-        str, ParselXPath('//div[@class="pcdescrf"]', callback=get_text(deep=True))
-    ]
-    screenshots: ScField[
-        List[str],
-        ParselXPathList('//div[@class="photo-row clearfix"]/a', callback=get_attr("href")),
+    _thumbnail_path: Sc[str, Parsel().css(".fr-fil").xpath("@src").get()]
+    _released_episodes: Sc[List[int], Parsel().css("li > span::text")[-1].re(r"(\d+)")]
+    _alt_titles: Sc[str, Parsel().xpath('//h2[@class="romanji"]/text()').get()]
+
+    title: Sc[str, Parsel().xpath('//h1[@class="h2 ntitle"]/text()').get()]
+
+    @sc_param
+    def alt_titles(self):
+        return [self._alt_titles]
+
+    thumbnail = sc_param(lambda self: f"https://animejoy.ru{self._thumbnail_path}")
+    description: Sc[str, Parsel().xpath('//div[@class="pcdescrf"]/p/text()').get()]
+    genres: Sc[List[str], Parsel().css(".zerop:nth-child(2) > span > a::text").getall()]
+
+    @sc_param
+    def episodes_total(self) -> int:
+        return self._released_episodes[-1]
+
+    @sc_param
+    def episodes_available(self) -> int:
+        return self._released_episodes[0]
+
+    aired: Sc[
+        str,
+        Parsel().xpath('//*[@id="dle-content"]/article/div[1]/div[2]/div[2]/p[5]/text()').get(),
     ]
-    url: ScField[str, ParselXPath('//meta[@property="og:url"]', callback=get_attr("content"))]
-    news_id = property(lambda self: self.url.split("/")[-1].split("-")[0])
+
+    url: Sc[str, Parsel().xpath('//meta[@property="og:url"]/@content').get()]
+    news_id = sc_param(lambda self: self.url.split("/")[-1].split("-")[0])
 
     def __str__(self):
-        return f"{self.title} ({self.alt_name})"
+        return f"{self.title} {self.alt_titles}"
 
     def _extract_episode_meta(self, response: str) -> List["Episode"]:
-        sel = Selector(response)
         # get player ids and names for better output
-        players_ids = sel.xpath(
-            '//div[@class="playlists-lists"]/div[@class="playlists-items"]/ul/li/@data-id'
-        ).getall()
-        players_names = sel.xpath(
-            '//div[@class="playlists-lists"]/div[@class="playlists-items"]/ul/li/text()'
-        ).getall()
+        sel = self.__selector__.__class__(response)
+        players_ids = sel.xpath('//div[@class="playlists-lists"]/div[@class="playlists-items"]/ul/li/@data-id').getall()
+
+        players_names = sel.xpath('//div[@class="playlists-lists"]/div[@class="playlists-items"]/ul/li/text()').getall()
         players_table = dict(zip(players_ids, players_names))
 
         # extract episodes names, video urls, and player ids
-        series_names = sel.xpath(
-            '//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/text()'
-        ).getall()
+        series_names = sel.xpath('//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/text()').getall()
         series_urls = sel.xpath(
             '//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/@data-file'
         ).getall()
         series_player_id = sel.xpath(
             '//div[@class="playlists-videos"]/div[@class="playlists-items"]/ul/li/@data-id'
         ).getall()
+
         episodes_dict: Dict[str, List[Dict[str, str]]] = {}
         for name, url, player_id in zip(series_names, series_urls, series_player_id):
             if not episodes_dict.get(name):
                 episodes_dict[name] = []
             if url.startswith("//"):
                 url = f"https:{url}"
 
             episodes_dict[name].append(
                 {
                     "url": url,
                     "name": players_table.get(player_id, "unknown"),
                     "player_id": player_id,
                 }
             )
-        return [
-            Episode.from_kwargs(name=name, _video_meta=video_meta)
-            for name, video_meta in episodes_dict.items()
-        ]
+        return [Episode.from_kwargs(name=name, _video_meta=video_meta) for name, video_meta in episodes_dict.items()]
 
     def get_episodes(self) -> List["Episode"]:
         response = (
             self.HTTP()
             .get(
                 "https://animejoy.ru/engine/ajax/playlists.php",
                 params={"news_id": self.news_id, "xfield": "playlist"},
@@ -196,24 +183,32 @@
         async with self.HTTP_ASYNC() as client:
             response = (
                 await client.get(
                     "https://animejoy.ru/engine/ajax/playlists.php",
                     params={"news_id": self.news_id, "xfield": "playlist"},
                 )
             ).json()["response"]
+            # crop to parts html players, series tags for better view outup
             return self._extract_episode_meta(response)
 
 
 class Episode(BaseEpisode):
     _video_meta: List[_SourceDict]
     name: str
 
     def __str__(self):
         return self.name
 
+    @sc_param
+    def num(self) -> int:
+        return int(self.name.split(" ")[0])
+
+    def dict(self):
+        return {"name": self.name, "meta": self._video_meta}
+
     def get_sources(self) -> List["Source"]:
         return [
             Source.from_kwargs(url=meta["url"], name=meta["name"], player_id=meta["player_id"])
             for meta in self._video_meta
         ]
 
     async def a_get_sources(self) -> List["Source"]:
@@ -221,19 +216,22 @@
 
 
 class Source(BaseSource):
     url: str
     name: str
     player_id: str
 
+    def dict(self):
+        return {"url": self.url, "name": self.name, "player_id": self.player_id}
+
     def __str__(self):
         return f"{urlsplit(self.url).netloc} ({self.name})"
 
 
 if __name__ == "__main__":
     ex = Extractor()
     res = ex.search("lai")
     an = res[0].get_anime()
     eps = an.get_episodes()
     vids = eps[0].get_sources()
-    print(*[v.raw_dict() for v in vids], sep="\n")
+    print(*[v.dict() for v in vids], sep="\n")
     print(vids[1].get_videos())
```

### Comparing `anicli_api-0.4.1/anicli_api/source/animevost.py` & `anicli_api-0.4.2/anicli_api/source/animevost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 from typing import Dict, List, Union
 
-from anicli_api.base import (
-    BaseAnime,
-    BaseEpisode,
-    BaseExtractor,
-    BaseOngoing,
-    BaseSearch,
-    BaseSource,
-    MainSchema,
-)
+from anicli_api.base import BaseAnime, BaseEpisode, BaseExtractor, BaseOngoing, BaseSearch, BaseSource, MainSchema
 from anicli_api.player.base import Video
 
 
 class VostAPI:
     """dummy animevost API implementation"""
 
     HTTP = BaseExtractor.HTTP
     HTTP_ASYNC = BaseExtractor.HTTP_ASYNC
     BASE_URL = "https://api.animevost.org/v1/"
 
     def api_request(self, method: str, *, api_method: str, **kwargs) -> Union[Dict, List[Dict]]:
         response = self.HTTP().request(method, self.BASE_URL + api_method, **kwargs)
         return response.json()
 
-    async def a_api_request(
-        self, method: str, *, api_method: str, **kwargs
-    ) -> Union[Dict, List[Dict]]:
+    async def a_api_request(self, method: str, *, api_method: str, **kwargs) -> Union[Dict, List[Dict]]:
         async with self.HTTP_ASYNC() as session:
             response = await session.request(method, self.BASE_URL + api_method, **kwargs)
             return response.json()
 
     @staticmethod
     def _kwargs_pop_params(kwargs, **params) -> dict:
         data = kwargs.pop("params") if kwargs.get("params") else {}
```

### Comparing `anicli_api-0.4.1/anicli_api/source/sovetromantica.py` & `anicli_api-0.4.2/anicli_api/source/sovetromantica.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,48 @@
 import warnings
 from typing import List
 
-from parsel import Selector
-from scrape_schema import ScField
-from scrape_schema.callbacks.parsel import crop_by_xpath_all as cbxa
-from scrape_schema.callbacks.parsel import get_attr, get_text, replace_text
-from scrape_schema.fields.parsel import NestedParselList, ParselXPath
-
-from anicli_api.base import (
-    BaseAnime,
-    BaseEpisode,
-    BaseExtractor,
-    BaseOngoing,
-    BaseSearch,
-    BaseSource,
-    MainSchema,
-)
+from scrape_schema import Nested, Parsel, Sc, sc_param
+
+from anicli_api.base import BaseAnime, BaseEpisode, BaseExtractor, BaseOngoing, BaseSearch, BaseSource, MainSchema
 
 
 class Extractor(BaseExtractor):
     BASE_URL = "https://sovetromantica.com"  # BASEURL
 
     def search(self, query: str) -> List["Search"]:
         response = self.HTTP().get(f"{self.BASE_URL}/anime", params={"query": query})
-        return Search.from_crop_rule_list(
-            response.text, crop_rule=cbxa('//div[@class="anime--block__desu"]')
-        )
+        chunks = Parsel().xpath('//div[@class="anime--block__desu"]').getall().sc_parse(response.text)
+        return [Search(ch) for ch in chunks]
 
     async def a_search(self, query: str) -> List["Search"]:
         # async search entrypoint
         async with self.HTTP_ASYNC() as client:
             response = await client.get(f"{self.BASE_URL}/anime", params={"query": query})
-            return Search.from_crop_rule_list(response.text,
-                                              crop_rule=cbxa('//div[@class="anime--block__desu"]'))
+            chunks = Parsel().xpath('//div[@class="anime--block__desu"]').getall().sc_parse(response.text)
+            return [Search(ch) for ch in chunks]
 
     def ongoing(self) -> List["Ongoing"]:
         # ongoing entrypoint
-        response = self.HTTP().get(self.BASE_URL)
-        return Ongoing.from_crop_rule_list(
-            response.text, crop_rule=cbxa('//div[@class="anime--block__desu"]')
-        )
+        response = self.HTTP().get(f"{self.BASE_URL}/anime")
+        chunks = Parsel().xpath('//div[@class="anime--block__desu"]').getall().sc_parse(response.text)
+        return [Ongoing(ch) for ch in chunks]
 
     async def a_ongoing(self) -> List["Ongoing"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.BASE_URL)
-            return Ongoing.from_crop_rule_list(
-                response.text, crop_rule=cbxa('//div[@class="anime--block__desu"]')
-            )
+            chunks = Parsel().xpath('//div[@class="anime--block__desu"]').getall().sc_parse(response.text)
+            return [Ongoing(ch) for ch in chunks]
 
 
 class Search(BaseSearch):
     # past xpath to main anime page
-    url: ScField[str, ParselXPath("//a", callback=get_attr("href"))]
-    name: ScField[
-        str,
-        ParselXPath(
-            '//div[@class="anime--block__name"]', callback=get_text(deep=True, strip=True, sep=" ")
-        ),
-    ]
+    url: Sc[str, Parsel().xpath("//a/@href").get()]
+    title: Sc[str, Parsel().xpath('//div[@class="anime--block__name"]/text()').get()]
+    thumbnail: Sc[str, Parsel().xpath('//*[@class="anime--poster lazy loaded"]/@src').get()]
     # url = property(lambda self: f"https://sovetromantica.com{self._path}")
 
     def get_anime(self) -> "Anime":
         response = self.HTTP().get(self.url)
         return Anime(response.text)
 
     async def a_get_anime(self) -> "Anime":
@@ -71,19 +52,17 @@
 
     def __str__(self):
         return self.name
 
 
 class Ongoing(BaseOngoing):
     # past xpath to main anime page
-    _path: ScField[
-        str, ParselXPath('//div[@class="block--full block--shadow"]/a', callback=get_attr("href"))
-    ]
-    name: ScField[str, ParselXPath('//meta[@itemprop="name"]', callback=get_attr("content"))]
-    url = property(lambda self: f"https://sovetromantica.com{self._path}")
+    url: Sc[str, Parsel().xpath("//a/@href").get()]
+    title: Sc[str, Parsel().xpath('//div[@class="anime--block__name"]/text()').get()]
+    thumbnail: Sc[str, Parsel().xpath('//*[@class="anime--poster lazy loaded"]/@src').get()]
 
     def get_anime(self) -> "Anime":
         response = self.HTTP().get(self.url)
         return Anime(response.text)
 
     async def a_get_anime(self) -> "Anime":
         async with self.HTTP_ASYNC() as client:
@@ -92,95 +71,111 @@
 
     def __str__(self):
         return self.name
 
 
 class Anime(BaseAnime):
     class _Episode(MainSchema):
-        name: ScField[str, ParselXPath("//a/div/span")]
-        _url_path: ScField[str, ParselXPath("//a", callback=get_attr("href"))]
-        image: ScField[str, ParselXPath("//a/img", callback=get_attr("src"))]
-        ep_id: ScField[str, ParselXPath("//div", callback=get_attr("id"))]
+        title: Sc[str, Parsel().xpath("//a/div/span/text()").get()]
+        _url_path: Sc[str, Parsel().xpath("//a/@href").get()]
+        image: Sc[str, Parsel().xpath("//a/img/@src").get()]
+        ep_id: Sc[str, Parsel().xpath("//div/@id").get()]
+
+        @sc_param
+        def num(self) -> int:
+            return int(self.title.split("#")[-1])
 
-        @property
+        @sc_param
         def url(self):
             return f"https://sovetromantica.com{self._url_path}"
 
-    name: ScField[
-        str, ParselXPath('//div[@class="block--full anime-name"]/div[@class="block--container"]')
+    _titles: Sc[
+        str,
+        Parsel().xpath('//div[@class="block--full anime-name"]/div[@class="block--container"]/text()').get(),
     ]
-    _episodes: ScField[
+
+    _episodes: Sc[
         List[_Episode],
-        NestedParselList(
-            _Episode, crop_rule=cbxa("//div[contains(@class, 'episodes-slick_item')]")
-        ),
+        Nested(Parsel().xpath("//div[contains(@class, 'episodes-slick_item')]").getall()),
     ]
 
+    @sc_param
+    def title(self):
+        return self._titles.split(" / ")[0]
+
+    @sc_param
+    def alt_titles(self):
+        return [self._titles.split(" / ")[-1]]
+
+    thumbnail: Sc[str, Parsel().xpath('//*[@id="poster"]/@src').get()]
+    description = None
+    genres: Sc[List[str], Parsel().xpath('//div[@class="animeTagInfo"]/a/text()').getall()]
+    episodes_available = None
+    episodes_total = None
+    aired = None
+
     def get_episodes(self) -> List["Episode"]:
         if not self._episodes:
             # episodes may not be uploaded. e.g:
             # https://sovetromantica.com/anime/1398-tsundere-akuyaku-reijou-liselotte-to-jikkyou-no-endou-kun-to-kaisetsu-no-kobayashi-san
-            warnings.warn(
-                "Episodes not available, return empty list", category=RuntimeWarning, stacklevel=3
-            )
+            warnings.warn("Episodes not available, return empty list", category=RuntimeWarning, stacklevel=3)
             return []
         return [Episode.from_kwargs(**ep.dict()) for ep in self._episodes]
 
     async def a_get_episodes(self) -> List["Episode"]:
         if not self._episodes:
             # episodes may not be uploaded. e.g:
             # https://sovetromantica.com/anime/1398-tsundere-akuyaku-reijou-liselotte-to-jikkyou-no-endou-kun-to-kaisetsu-no-kobayashi-san
-            warnings.warn(
-                "Episodes not available, return empty list", category=RuntimeWarning, stacklevel=3
-            )
+            warnings.warn("Episodes not available, return empty list", category=RuntimeWarning, stacklevel=3)
             return []
         return [Episode.from_kwargs(**ep.dict()) for ep in self._episodes]
 
     def __str__(self):
-        return self.name
+        return self.title
 
 
 class Episode(BaseEpisode):
-    name: str
+    title: str
+    num: int
     image: str
     ep_id: str
     url: str
 
+    def dict(self):
+        return {"title": self.title, "num": self.num}
+
     def get_sources(self) -> List["Source"]:
         response = self.HTTP().get(self.url)
-        sel = Selector(response.text)
-        video = ParselXPath(
-            '//meta[@property="ya:ovs:content_url"]', callback=get_attr("content")
-        ).extract(sel)
+        video = Parsel().xpath('//meta[@property="ya:ovs:content_url"]/@content').get().sc_parse(response.text)
         return [Source.from_kwargs(url=video)]
 
     async def a_get_sources(self) -> List["Source"]:
         async with self.HTTP_ASYNC() as client:
             response = await client.get(self.url)
-            sel = Selector(response.text)
-            video = ParselXPath(
-                '//meta[@property="ya:ovs:content_url"]', callback=get_attr("content")
-            ).extract(sel)
+            video = Parsel().xpath('//meta[@property="ya:ovs:content_url"]/@content').get().sc_parse(response.text)
             return [Source.from_kwargs(url=video)]
 
     def __str__(self):
-        return self.name
+        return self.title
 
 
 class Source(BaseSource):
     url: str
     name: str = "SovietRomantica (Subtitles)"
 
+    def dict(self):
+        return {"url": self.url, "name": self.name}
+
     def __str__(self):
         return self.name
 
 
 if __name__ == "__main__":
     ex = Extractor()
     s = ex.search("lai")
     ong = ex.ongoing()
     an = s[1].get_anime()
     s[0].get_anime().get_episodes()  # not founded eps
     eps = an.get_episodes()
     sou = eps[0].get_sources()
     vid = sou[0].get_videos()
-    print()
+    print(vid)
```

### Comparing `anicli_api-0.4.1/anicli_api/tools/random_useragent.py` & `anicli_api-0.4.2/anicli_api/tools/random_useragent.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.4.1/pyproject.toml` & `anicli_api-0.4.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.4.1"
+version = "0.4.2"
 description = "Anime extractor api implementation"
 authors = ["Georgiy aka Vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/"]
 keywords = [
@@ -32,21 +32,22 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/vypivshiy/anicli-api/issues"
 "Cli app" = "https://github.com/vypivshiy/ani-cli-ru"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = {extras = ["http2"], version = "^0.24.0"}
-scrape-schema = {extras = ["parsel"], version = "^0.2.3"}
+scrape-schema = {version = "^0.3.0"}
+chompjs = "^1.2.2"
+ruff = "^0.0.278"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = {extras = ["coverage"], version = "^7.2.0"}
 pytest-cov = "^4.0.0"
-flake8 = "^5.0.0"
 pyproject-flake8 = "5.0.4"
 mypy = "^0.982"
 pytest-asyncio = "^0.20.2"
 twine = "^4.0.1"
 isort = "^5.10.1"
 black = "^22.10.0"
 urllib3 = "1.26.15"
@@ -59,35 +60,47 @@
 [tool.poetry.group.codegen.dependencies]
 jinja2 = "^3.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-
-[tool.flake8]
-exclude = [
-'.git',
-'__pycache__',
-'dist',
-'env',
-'venv',
-'.venv',
-'__template__.py']
-max-line-length = 120
-max-complexity = 8
-ignore = ['F405', 'F403', 'W503', 'E501', 'F401', 'E203', 'F722', 'F821']
-
 [tool.mypy]
 python_version = 3.8
 pretty = true
 ignore_missing_imports = true
 exclude = ["env", ".env", "venv", "__pycache__", "examples", "__template__.py"]
 files=["anicli_api/*"]
 
+
+[tool.ruff]
+target-version = "py38"
+line-length = 120
+select = ["E", "F"]
+ignore = [
+  # Allow non-abstract empty methods in abstract base classes
+  "B027",
+  # Allow boolean positional values in function calls, like `dict.get(... True)`
+  "FBT003",
+  # Ignore checks for possible passwords
+  "S105", "S106", "S107",
+  # Ignore complexity
+  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+]
+unfixable = [
+  # Don't touch unused imports
+  "F401",
+]
+
+exclude = [
+  "examples",
+  "venv",
+  "__init__.py"
+]
+
 [tool.black]
-line-length = 99
+line-length = 120
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
-line_length = 99
+line_length = 120
```

### Comparing `anicli_api-0.4.1/PKG-INFO` & `anicli_api-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: Anime extractor api implementation
 License: MIT
 Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
 Author: Georgiy aka Vypivshiy
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
+Requires-Dist: chompjs (>=1.2.2,<2.0.0)
 Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
-Requires-Dist: scrape-schema[parsel] (>=0.2.3,<0.3.0)
+Requires-Dist: ruff (>=0.0.278,<0.0.279)
+Requires-Dist: scrape-schema (>=0.3.0,<0.4.0)
 Project-URL: Bug Tracker, https://github.com/vypivshiy/anicli-api/issues
 Project-URL: Cli app, https://github.com/vypivshiy/ani-cli-ru
 Description-Content-Type: text/plain
 
 # anicli-api
 
 Программный интерфейс набора парсеров аниме с различных источников.
```

