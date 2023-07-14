# Comparing `tmp/instagram_archiver-0.2.0.tar.gz` & `tmp/instagram_archiver-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_archiver-0.2.0.tar", max compression
+gzip compressed data, was "instagram_archiver-0.2.1.tar", max compression
```

## Comparing `instagram_archiver-0.2.0.tar` & `instagram_archiver-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1080 2023-04-09 18:35:32.311409 instagram_archiver-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      310 2023-04-02 01:53:21.596308 instagram_archiver-0.2.0/README.md
--rw-r--r--   0        0        0       44 2023-04-02 01:54:39.428228 instagram_archiver-0.2.0/instagram_archiver/__init__.py
--rw-r--r--   0        0        0    14066 2023-06-24 03:51:06.849364 instagram_archiver-0.2.0/instagram_archiver/client.py
--rw-r--r--   0        0        0     3490 2023-04-13 17:30:33.623333 instagram_archiver-0.2.0/instagram_archiver/constants.py
--rw-r--r--   0        0        0     2361 2023-04-13 21:34:35.792248 instagram_archiver-0.2.0/instagram_archiver/ig_typing.py
--rw-r--r--   0        0        0     2463 2023-04-13 21:41:21.669932 instagram_archiver-0.2.0/instagram_archiver/main.py
--rw-r--r--   0        0        0     3169 2023-04-13 21:41:38.791929 instagram_archiver-0.2.0/instagram_archiver/utils.py
--rw-r--r--   0        0        0      978 2023-06-24 03:51:06.849364 instagram_archiver-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 instagram_archiver-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-09 18:35:32.311409 instagram_archiver-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      469 2023-07-14 11:55:09.492445 instagram_archiver-0.2.1/README.md
+-rw-r--r--   0        0        0       80 2023-07-14 11:57:26.846146 instagram_archiver-0.2.1/instagram_archiver/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-14 11:57:18.932162 instagram_archiver-0.2.1/instagram_archiver/__main__.py
+-rw-r--r--   0        0        0    13948 2023-07-14 20:56:07.333613 instagram_archiver-0.2.1/instagram_archiver/client.py
+-rw-r--r--   0        0        0     3691 2023-07-14 21:10:36.340535 instagram_archiver-0.2.1/instagram_archiver/constants.py
+-rw-r--r--   0        0        0     1186 2023-07-14 20:56:40.236579 instagram_archiver-0.2.1/instagram_archiver/find_query_hashes.py
+-rw-r--r--   0        0        0     4265 2023-07-14 20:57:06.075552 instagram_archiver-0.2.1/instagram_archiver/ig_typing.py
+-rw-r--r--   0        0        0     3067 2023-07-14 21:15:39.922449 instagram_archiver-0.2.1/instagram_archiver/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 12:03:28.860478 instagram_archiver-0.2.1/instagram_archiver/py.typed
+-rw-r--r--   0        0        0     3646 2023-07-14 19:09:41.265536 instagram_archiver-0.2.1/instagram_archiver/utils.py
+-rw-r--r--   0        0        0     5405 2023-07-14 21:03:53.453483 instagram_archiver-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 instagram_archiver-0.2.1/PKG-INFO
```

### Comparing `instagram_archiver-0.2.0/LICENSE.txt` & `instagram_archiver-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `instagram_archiver-0.2.0/instagram_archiver/client.py` & `instagram_archiver-0.2.1/instagram_archiver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from inspect import Traceback
 from os import makedirs, utime
 from pathlib import Path
 from pprint import pprint as pp
 from typing import Collection, Literal, Mapping, Type, TypeVar, overload
 from urllib.parse import urlparse
 import json
@@ -13,41 +14,41 @@
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 from yt_dlp.cookies import extract_cookies_from_browser
 import requests
 import yt_dlp
 
 from .constants import LOG_SCHEMA, RETRY_ABORT_NUM, SHARED_HEADERS, SHARED_YT_DLP_OPTIONS
-from .ig_typing import (CarouselMedia, Comments, Edge, HighlightsTray, MediaInfo, MediaInfoItem,
-                        MediaInfoItemImageVersions2Candidate, WebProfileInfo)
+from .ig_typing import (BrowserName, CarouselMedia, Comments, Edge, HighlightsTray, MediaInfo,
+                        MediaInfoItem, MediaInfoItemImageVersions2Candidate, WebProfileInfo)
 from .utils import chdir, get_extension, json_dumps_formatted, write_if_new
 
 __all__ = ('InstagramClient',)
 
-Browser = Literal['brave', 'chrome', 'chromium', 'edge', 'opera', 'vivaldi', 'firefox', 'safari']
 T = TypeVar('T')
 
 
 def _clean_url(url: str) -> str:
     parsed = urlparse(url)
     return f'https://{parsed.netloc}{parsed.path}'
 
 
 class AuthenticationError(Exception):
     pass
 
 
 class InstagramClient:
+    """The client."""
     def __init__(self,
                  *,
                  username: str,
                  log_file: str | Path | None = None,
-                 output_dir: str | None = None,
+                 output_dir: str | Path | None = None,
                  disable_log: bool = False,
-                 browser: Browser = 'chrome',
+                 browser: BrowserName = 'chrome',
                  browser_profile: str = 'Default',
                  debug: bool = False,
                  comments: bool = False) -> None:
         self._no_log = disable_log
         self._session = requests.Session()
         self._browser = browser
         self._browser_profile = browser_profile
@@ -70,16 +71,15 @@
     def _setup_db(self) -> None:
         existed = self._log_db.exists()
         if not existed or (existed and self._log_db.stat().st_size == 0):
             logger.debug('Creating schema')
             self._cursor.execute(LOG_SCHEMA)
 
     def _setup_session(self,
-                       browser: Literal['brave', 'chrome', 'chromium', 'edge', 'opera', 'vivaldi',
-                                        'firefox', 'safari'] = 'chrome',
+                       browser: BrowserName = 'chrome',
                        browser_profile: str = 'Default') -> None:
         self._session.mount(
             'https://',
             HTTPAdapter(max_retries=Retry(
                 backoff_factor=1.5,  # wait times are normally 1 and 3 seconds
                 redirect=0,
                 status=0,
@@ -239,21 +239,24 @@
     def _highlights_tray(self, user_id: int | str) -> HighlightsTray:
         return self._get_rate_limited(
             f'https://i.instagram.com/api/v1/highlights/{user_id}/'
             'highlights_tray/',
             cast_to=HighlightsTray)
 
     def __enter__(self) -> 'InstagramClient':
+        """Recommended way to initialise the client."""
         return self
 
     def __exit__(self, _: Type[BaseException], __: BaseException, ___: Traceback) -> None:
+        """Clean up."""
         self._cursor.close()
         self._connection.close()
 
     def process(self) -> None:
+        """Process posts."""
         with chdir(self._output_dir):
             self._get_rate_limited(f'https://www.instagram.com/{self._username}/',
                                    return_json=False)
             r = self._get_rate_limited('https://i.instagram.com/api/v1/users/web_profile_info/',
                                        params={'username': self._username},
                                        cast_to=WebProfileInfo)
             with open('web_profile_info.json', 'w') as f:
@@ -278,24 +281,22 @@
                 media = self._get_rate_limited(
                     'https://www.instagram.com/graphql/query/',
                     params=params,
                     cast_to=WebProfileInfo)['data']['user']['edge_owner_to_timeline_media']
                 page_info = media['page_info']
                 self._save_stuff(media['edges'])
             if len(self._video_urls) > 0:
-                with yt_dlp.YoutubeDL({
-                        **SHARED_YT_DLP_OPTIONS,  # type: ignore[misc]
-                        **{
-                            'cookiesfrombrowser': [
-                                self._browser, self._browser_profile, None, None
-                            ],
-                            'getcomments': self._get_comments,
-                            'verbose': self._debug
-                        }
-                }) as ydl:
+                options = deepcopy(SHARED_YT_DLP_OPTIONS)
+                options.update({
+                    'cookiefile': None,
+                    'cookiesfrombrowser': (self._browser, self._browser_profile),
+                    'getcomments': self._get_comments,
+                    'verbose': self._debug
+                })
+                with yt_dlp.YoutubeDL(options) as ydl:
                     failed_urls: list[str] = []
                     while (self._video_urls and (url := self._video_urls.pop())):
                         if self._is_saved(url):
                             logger.debug(f'{url} is already saved')
                             continue
                         if ydl.extract_info(url):
                             logger.debug(f'Extracting {url}')
```

### Comparing `instagram_archiver-0.2.0/instagram_archiver/constants.py` & `instagram_archiver-0.2.1/instagram_archiver/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TYPE_CHECKING, Final, Mapping
 
 from .utils import YoutubeDLLogger
 
-__all__ = ('LOG_SCHEMA', 'RETRY_ABORT_NUM', 'SHARED_HEADERS', 'SHARED_YT_DLP_OPTIONS',
-           'YT_DLP_SLEEP_INTERVAL', 'USER_AGENT')
+__all__ = ('BROWSER_CHOICES', 'LOG_SCHEMA', 'RETRY_ABORT_NUM', 'SHARED_HEADERS',
+           'SHARED_YT_DLP_OPTIONS', 'YT_DLP_SLEEP_INTERVAL', 'USER_AGENT')
 
 if TYPE_CHECKING:
-    from yt_dlp import YoutubeDLOptions
+    from yt_dlp import YDLOpts
 
 USER_AGENT: Final[str] = ('Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) '
                           'Chrome/112.0.0.0 Safari/537.36')
 # Do not set the x-ig-d header as this will cause API calls to return 404
 SHARED_HEADERS: Final[Mapping[str, str]] = {
     'accept': ('text/html,application/xhtml+xml,application/xml;q=0.9,image/jxl,'
                'image/avif,image/webp,image/apng,*/*;q=0.8,'
@@ -28,19 +28,21 @@
 }
 LOG_SCHEMA: Final[str] = '''
 CREATE TABLE log (
     url TEXT PRIMARY KEY NOT NULL,
     date TEXT DEFAULT CURRENT_TIMESTAMP NOT NULL
 );
 '''
+#: Calls per minute allowed.
 CALLS_PER_MINUTE: Final[int] = 10
-YT_DLP_SLEEP_INTERVAL: Final[float] = 60 / CALLS_PER_MINUTE
+#: yt-dlp sleep interval.
+YT_DLP_SLEEP_INTERVAL: Final[int] = 60 // CALLS_PER_MINUTE
 #: Value taken from Instagram's JS under BootloaderConfig
 RETRY_ABORT_NUM: Final[int] = 2
-SHARED_YT_DLP_OPTIONS: 'YoutubeDLOptions' = {
+SHARED_YT_DLP_OPTIONS: 'YDLOpts' = {
     'allowed_extractors': ['Instagram.*'],
     'allsubtitles': True,
     'cookiesfrombrowser': None,
     'geo_bypass': True,
     'getcomments': False,
     'hls_use_mpegts': True,
     'http_headers': SHARED_HEADERS,
@@ -48,15 +50,15 @@
     'ignoreerrors': True,
     'logger': YoutubeDLLogger(),
     'outtmpl': {
         'default': '%(title).128s___src=%(extractor)s___id=%(id)s.%(ext)s',
         'pl_thumbnail': ''
     },
     'overwrites': False,
-    'max_sleep_interval': 6.0,
+    'max_sleep_interval': 6,
     'merge_output_format': 'mkv',
     'postprocessors': [{
         'api': 'https://sponsor.ajay.app',
         'categories': [
             'preview', 'selfpromo', 'interaction', 'music_offtopic', 'sponsor', 'poi_highlight',
             'intro', 'outro', 'filler', 'chapter'
         ],
@@ -97,7 +99,9 @@
     'subtitleslangs': ['all'],
     'verbose': False,
     'writeautomaticsub': True,
     'writesubtitles': True,
     'writeinfojson': True,
     'writethumbnail': True,
 }
+#: Possible browser choices to get cookies from.
+BROWSER_CHOICES = ('brave', 'chrome', 'chromium', 'edge', 'opera', 'vivaldi', 'firefox', 'safari')
```

### Comparing `instagram_archiver-0.2.0/instagram_archiver/utils.py` & `instagram_archiver-0.2.1/instagram_archiver/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,53 +7,58 @@
 import json
 import logging
 import sys
 
 from loguru import logger
 import click
 
-__all__ = ('UnknownMimetypeError', 'chdir', 'get_extension', 'json_dumps_formatted', 'write_if_new')
+__all__ = ('UnknownMimetypeError', 'YoutubeDLLogger', 'chdir', 'get_extension',
+           'json_dumps_formatted', 'setup_logging', 'write_if_new')
 
 T = TypeVar('T')
 
 
 class JSONFormattedString(Generic[T]):  # pylint: disable=too-few-public-methods
     def __init__(self, formatted: str, original: T) -> None:
         self.formatted = formatted
         self.original_value = original
 
     def __str__(self) -> str:
         return self.formatted
 
 
 def json_dumps_formatted(obj: T) -> JSONFormattedString[T]:
+    """Returns a special object with the formatted version of the JSON str and the original."""
     return JSONFormattedString(json.dumps(obj, sort_keys=True, indent=2), obj)
 
 
 @contextmanager
 def chdir(path: str | Path) -> Iterator[None]:
+    """Context-managing ``chdir``. Changes to old path on exit."""
     old_path = getcwd()
     os_chdir(path)
     try:
         yield
     finally:
         chdir(old_path)
 
 
 def write_if_new(target: Path | str, content: str | bytes, mode: str = 'w') -> None:
+    """Write a file only if it will be a new file."""
     if not isfile(target):
         with click.open_file(str(target), mode) as f:
             f.write(content)
 
 
 class UnknownMimetypeError(Exception):
-    pass
+    """Raised when an unknown mimetype is encountered in ``get_extension()``."""
 
 
 def get_extension(mimetype: str) -> Literal['png', 'jpg']:
+    """Gets the appropriate three-letter extension for a mimetype."""
     if mimetype == 'image/jpeg':
         return 'jpg'
     if mimetype == 'image/png':
         return 'png'
     raise UnknownMimetypeError(mimetype)
 
 
@@ -90,14 +95,15 @@
             format='<level>{message}</level>',
             level='INFO',
             sink=sys.stderr,
         ),))
 
 
 class YoutubeDLLogger:
+    """Basic logger front-end to loguru for use with ``YoutubeDL``."""
     def debug(self, message: str) -> None:
         if message.startswith('[debug] '):
             logger.debug(message)
         else:
             logger.info(message)
 
     def info(self, message: str) -> None:
```

### Comparing `instagram_archiver-0.2.0/PKG-INFO` & `instagram_archiver-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: instagram-archiver
-Version: 0.2.0
+Version: 0.2.1
 Summary: Archive Instagram content.
 License: MIT
 Author: Andrew Udvare
 Author-email: audvare@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: click (>=8.0,<8.1.4)
+Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: mutagen (>=1.46.0,<2.0.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: yt-dlp (>=2023.6.22,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # Instagram Archiver
 
-Tool to download data from an Instagram profile you have access to. It downloads the images, videos, and related metadata (stored as JSON files).
+[![QA](https://github.com/Tatsh/instagram-archiver/actions/workflows/qa.yml/badge.svg)](https://github.com/Tatsh/instagram-archiver/actions/workflows/qa.yml)
+
+Tool to download data from an Instagram profile you have access to. It downloads the images, videos,
+and related metadata (stored as JSON files).
 
 ## Installation
 
 ```shell
 pip install instagram-archiver
 ```
```

