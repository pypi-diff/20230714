# Comparing `tmp/scrapetube-2.4.0-py3-none-any.whl.zip` & `tmp/scrapetube-2.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5328 bytes, number of entries: 7
--rw-r--r--  2.0 unx       85 b- defN 23-Jun-12 20:17 scrapetube/__init__.py
--rw-r--r--  2.0 unx     8970 b- defN 23-Jun-12 20:15 scrapetube/scrapetube.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1656 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      559 b- defN 23-Jun-12 20:17 scrapetube-2.4.0.dist-info/RECORD
-7 files, 12445 bytes uncompressed, 4334 bytes compressed:  65.2%
+Zip file size: 5595 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       85 b- defN 23-Jul-14 00:13 scrapetube/__init__.py
+-rw-r--r--  2.0 unx    10181 b- defN 23-Jul-14 00:10 scrapetube/scrapetube.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jul-14 00:14 scrapetube-2.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1656 b- defN 23-Jul-14 00:14 scrapetube-2.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 00:14 scrapetube-2.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-14 00:14 scrapetube-2.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      560 b- defN 23-Jul-14 00:14 scrapetube-2.5.0.dist-info/RECORD
+7 files, 13657 bytes uncompressed, 4601 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: scrapetube/__init__.py
 Comment: 
 
 Filename: scrapetube/scrapetube.py
 Comment: 
 
-Filename: scrapetube-2.4.0.dist-info/LICENSE
+Filename: scrapetube-2.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: scrapetube-2.4.0.dist-info/METADATA
+Filename: scrapetube-2.5.0.dist-info/METADATA
 Comment: 
 
-Filename: scrapetube-2.4.0.dist-info/WHEEL
+Filename: scrapetube-2.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: scrapetube-2.4.0.dist-info/top_level.txt
+Filename: scrapetube-2.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: scrapetube-2.4.0.dist-info/RECORD
+Filename: scrapetube-2.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scrapetube/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .scrapetube import get_channel, get_search, get_playlist
 
-__version__ = "2.4.0"
+__version__ = "2.5.0"
```

## scrapetube/scrapetube.py

```diff
@@ -54,31 +54,28 @@
         content_type (``str``, *optional*):
             In order to get content type. Pass one of the following values.
             ``"videos"``: Videos
             ``"shorts"``: Shorts
             ``"streams"``: Streams
     """
 
-    sort_by_map = {"newest": "dd", "oldest": "da", "popular": "p"}
-
     base_url = ""
     if channel_url:
         base_url = channel_url
     elif channel_id:
         base_url = f"https://www.youtube.com/channel/{channel_id}"
     elif channel_username:
         base_url = f"https://www.youtube.com/@{channel_username}"
 
-    url = "{base_url}/{content_type}?view=0&sort={sort_by}&flow=grid".format(
+    url = "{base_url}/{content_type}?view=0&flow=grid".format(
         base_url=base_url,
         content_type=content_type,
-        sort_by=sort_by_map[sort_by],
     )
     api_endpoint = "https://www.youtube.com/youtubei/v1/browse"
-    videos = get_videos(url, api_endpoint, type_property_map[content_type], limit, sleep)
+    videos = get_videos(url, api_endpoint, type_property_map[content_type], limit, sleep, sort_by)
     for video in videos:
         yield video
 
 
 def get_playlist(
     playlist_id: str, limit: int = None, sleep: int = 1
 ) -> Generator[dict, None, None]:
@@ -158,60 +155,94 @@
     videos = get_videos(
         url, api_endpoint, results_type_map[results_type][1], limit, sleep
     )
     for video in videos:
         yield video
 
 
+
+def get_video(
+    id: str,
+) -> dict:
+
+    """Get a single video.
+
+    Parameters:
+        id (``str``):
+            The video id from the video you want to get.
+    """
+
+    session = get_session()
+    url = f"https://www.youtube.com/watch?v={id}"
+    html = get_initial_data(session, url)
+    client = json.loads(
+        get_json_from_html(html, "INNERTUBE_CONTEXT", 2, '"}},') + '"}}'
+    )["client"]
+    session.headers["X-YouTube-Client-Name"] = "1"
+    session.headers["X-YouTube-Client-Version"] = client["clientVersion"]
+    data = json.loads(
+        get_json_from_html(html, "var ytInitialData = ", 0, "};") + "}"
+    )
+    return next(search_dict(data, "videoPrimaryInfoRenderer"))
+
+
+
 def get_videos(
-    url: str, api_endpoint: str, selector: str, limit: int, sleep: int
+    url: str, api_endpoint: str, selector: str, limit: int, sleep: int, sort_by: str = None
 ) -> Generator[dict, None, None]:
-    session = requests.Session()
-    session.headers[
-        "User-Agent"
-    ] = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.101 Safari/537.36"
+    session = get_session()
     is_first = True
-    quit = False
+    quit_it = False
     count = 0
     while True:
         if is_first:
             html = get_initial_data(session, url)
             client = json.loads(
                 get_json_from_html(html, "INNERTUBE_CONTEXT", 2, '"}},') + '"}}'
             )["client"]
             api_key = get_json_from_html(html, "innertubeApiKey", 3)
             session.headers["X-YouTube-Client-Name"] = "1"
             session.headers["X-YouTube-Client-Version"] = client["clientVersion"]
             data = json.loads(
                 get_json_from_html(html, "var ytInitialData = ", 0, "};") + "}"
             )
-            next_data = get_next_data(data)
+            next_data = get_next_data(data, sort_by)
             is_first = False
+            if sort_by and sort_by != "newest": 
+                continue
         else:
             data = get_ajax_data(session, api_endpoint, api_key, next_data, client)
             next_data = get_next_data(data)
         for result in get_videos_items(data, selector):
             try:
                 count += 1
                 yield result
                 if count == limit:
-                    quit = True
+                    quit_it = True
                     break
             except GeneratorExit:
-                quit = True
+                quit_it = True
                 break
 
-        if not next_data or quit:
+        if not next_data or quit_it:
             break
 
         time.sleep(sleep)
 
     session.close()
 
 
+def get_session() -> requests.Session:
+    session = requests.Session()
+    session.headers[
+        "User-Agent"
+    ] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36"
+    session.headers["Accept-Language"] = "en"
+    return session
+
 def get_initial_data(session: requests.Session, url: str) -> str:
     session.cookies.set("CONSENT", "YES+cb", domain=".youtube.com")
     response = session.get(url)
 
     html = response.text
     return html
 
@@ -233,21 +264,31 @@
 
 def get_json_from_html(html: str, key: str, num_chars: int = 2, stop: str = '"') -> str:
     pos_begin = html.find(key) + len(key) + num_chars
     pos_end = html.find(stop, pos_begin)
     return html[pos_begin:pos_end]
 
 
-def get_next_data(data: dict) -> dict:
-    raw_next_data = next(search_dict(data, "continuationEndpoint"), None)
-    if not raw_next_data:
+def get_next_data(data: dict, sort_by: str = None) -> dict:
+    # Youtube, please don't change the order of these
+    sort_by_map = {
+        "newest": 0, 
+        "popular": 1,
+        "oldest": 2, 
+    }
+    if sort_by and sort_by != "newest":
+        endpoint = next(
+            search_dict(data, "feedFilterChipBarRenderer"), None)["contents"][sort_by_map[sort_by]]["chipCloudChipRenderer"]["navigationEndpoint"]
+    else:
+        endpoint = next(search_dict(data, "continuationEndpoint"), None)
+    if not endpoint:
         return None
     next_data = {
-        "token": raw_next_data["continuationCommand"]["token"],
-        "click_params": {"clickTrackingParams": raw_next_data["clickTrackingParams"]},
+        "token": endpoint["continuationCommand"]["token"],
+        "click_params": {"clickTrackingParams": endpoint["clickTrackingParams"]},
     }
 
     return next_data
 
 
 def search_dict(partial: dict, search_key: str) -> Generator[dict, None, None]:
     stack = [partial]
```

## Comparing `scrapetube-2.4.0.dist-info/LICENSE` & `scrapetube-2.5.0.dist-info/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Cheskel Twersky
+Copyright (c) 2023 Cheskel Twersky
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `scrapetube-2.4.0.dist-info/METADATA` & `scrapetube-2.5.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapetube
-Version: 2.4.0
+Version: 2.5.0
 Summary: Scrape youtube without the official youtube api and without selenium.
 Home-page: https://github.com/dermasmid/scrapetube
 Author: Cheskel Twersky
 Author-email: twerskycheskel@gmail.com
 License: MIT
 Project-URL: Documentation, https://scrapetube.readthedocs.io/en/latest/
 Keywords: youtube python channel videos search playlist list get
```

