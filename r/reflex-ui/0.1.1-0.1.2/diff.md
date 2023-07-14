# Comparing `tmp/reflex_ui-0.1.1.tar.gz` & `tmp/reflex_ui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_ui-0.1.1.tar", max compression
+gzip compressed data, was "reflex_ui-0.1.2.tar", max compression
```

## Comparing `reflex_ui-0.1.1.tar` & `reflex_ui-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1075 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/README.md
--rw-r--r--   0        0        0      944 2023-07-02 17:23:41.010505 reflex_ui-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      110 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/__init__.py
--rw-r--r--   0        0        0     4932 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/app.py
--rw-r--r--   0        0        0    15243 2023-07-02 17:23:24.247163 reflex_ui-0.1.1/reflex/app_server.py
--rw-r--r--   0        0        0     1530 2023-06-01 16:08:46.937561 reflex_ui-0.1.1/reflex/assets.py
--rw-r--r--   0        0        0     2480 2023-07-02 17:23:24.247163 reflex_ui-0.1.1/reflex/common.py
--rw-r--r--   0        0        0       47 2023-06-02 09:45:54.484185 reflex_ui-0.1.1/reflex/errors.py
--rw-r--r--   0        0        0    36522 2023-07-02 17:49:31.901177 reflex_ui-0.1.1/reflex/generated/app.js
--rw-r--r--   0        0        0    80229 2023-07-02 17:49:31.924510 reflex_ui-0.1.1/reflex/generated/app.js.map
--rw-r--r--   0        0        0      287 2023-07-02 17:49:30.104509 reflex_ui-0.1.1/reflex/generated/index.html
--rw-r--r--   0        0        0     4350 2023-07-02 17:49:30.834510 reflex_ui-0.1.1/reflex/generated/style.css
--rw-r--r--   0        0        0     7562 2023-07-02 17:49:30.837843 reflex_ui-0.1.1/reflex/generated/style.css.map
--rw-r--r--   0        0        0    75209 2022-04-21 09:32:25.000000 reflex_ui-0.1.1/reflex/hosted-assets/showdown.min.js
--rw-r--r--   0        0        0     2521 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/image_source.py
--rw-r--r--   0        0        0     1229 2023-06-02 09:31:52.003332 reflex_ui-0.1.1/reflex/messages.py
--rw-r--r--   0        0        0    39029 2023-07-02 17:50:56.407878 reflex_ui-0.1.1/reflex/session.py
--rw-r--r--   0        0        0      121 2023-05-28 09:40:21.000000 reflex_ui-0.1.1/reflex/styling/__init__.py
--rw-r--r--   0        0        0     3648 2023-06-01 11:11:54.202507 reflex_ui-0.1.1/reflex/styling/box_style.py
--rw-r--r--   0        0        0     9391 2023-06-16 18:28:59.043338 reflex_ui-0.1.1/reflex/styling/color.py
--rw-r--r--   0        0        0     2874 2023-05-28 09:43:35.000000 reflex_ui-0.1.1/reflex/styling/fills.py
--rw-r--r--   0        0        0     2671 2023-05-28 16:11:56.000000 reflex_ui-0.1.1/reflex/styling/markdown_style.py
--rw-r--r--   0        0        0     1760 2023-05-28 16:11:33.000000 reflex_ui-0.1.1/reflex/styling/text_style.py
--rw-r--r--   0        0        0      274 2023-05-30 05:41:43.000000 reflex_ui-0.1.1/reflex/theme.py
--rw-r--r--   0        0        0    12670 2023-06-18 14:30:30.191229 reflex_ui-0.1.1/reflex/validator.py
--rw-r--r--   0        0        0      467 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/widgets/__init__.py
--rw-r--r--   0        0        0     2424 2023-07-01 11:10:37.780000 reflex_ui-0.1.1/reflex/widgets/auto_form.py
--rw-r--r--   0        0        0     8439 2023-07-02 17:50:56.411212 reflex_ui-0.1.1/reflex/widgets/button.py
--rw-r--r--   0        0        0     1577 2023-07-02 17:50:56.411212 reflex_ui-0.1.1/reflex/widgets/column.py
--rw-r--r--   0        0        0      226 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/reflex/widgets/container.py
--rw-r--r--   0        0        0     1828 2023-06-10 18:22:34.826680 reflex_ui-0.1.1/reflex/widgets/dropdown.py
--rw-r--r--   0        0        0      507 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/widgets/image.py
--rw-r--r--   0        0        0     1175 2023-06-09 18:12:36.907709 reflex_ui-0.1.1/reflex/widgets/markdown_view.py
--rw-r--r--   0        0        0      552 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/widgets/media_player.py
--rw-r--r--   0        0        0      724 2023-06-18 14:35:53.924200 reflex_ui-0.1.1/reflex/widgets/metadata.py
--rw-r--r--   0        0        0     3524 2023-06-10 18:04:23.870009 reflex_ui-0.1.1/reflex/widgets/mouse_event_listener.py
--rw-r--r--   0        0        0      484 2023-06-14 20:50:37.701043 reflex_ui-0.1.1/reflex/widgets/plot.py
--rw-r--r--   0        0        0     1665 2023-07-02 17:50:56.411212 reflex_ui-0.1.1/reflex/widgets/progress_circle.py
--rw-r--r--   0        0        0      533 2023-06-09 18:05:31.920936 reflex_ui-0.1.1/reflex/widgets/rectangle.py
--rw-r--r--   0        0        0     1594 2023-07-02 17:44:56.264397 reflex_ui-0.1.1/reflex/widgets/row.py
--rw-r--r--   0        0        0      242 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/reflex/widgets/stack.py
--rw-r--r--   0        0        0     1567 2023-06-11 11:50:08.153416 reflex_ui-0.1.1/reflex/widgets/switch.py
--rw-r--r--   0        0        0      363 2023-05-28 16:37:28.000000 reflex_ui-0.1.1/reflex/widgets/text.py
--rw-r--r--   0        0        0     1895 2023-06-21 05:55:32.753397 reflex_ui-0.1.1/reflex/widgets/text_input.py
--rw-r--r--   0        0        0    20757 2023-07-02 17:50:56.414545 reflex_ui-0.1.1/reflex/widgets/widget_base.py
--rw-r--r--   0        0        0     3891 2023-06-11 10:23:10.760064 reflex_ui-0.1.1/reflex/world_units.py
--rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 reflex_ui-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/README.md
+-rw-r--r--   0        0        0     1041 2023-07-14 08:40:45.243231 reflex_ui-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-14 08:24:26.573241 reflex_ui-0.1.2/reflex/__init__.py
+-rw-r--r--   0        0        0     5242 2023-07-14 08:24:26.583241 reflex_ui-0.1.2/reflex/app.py
+-rw-r--r--   0        0        0    15243 2023-07-02 17:23:24.247163 reflex_ui-0.1.2/reflex/app_server.py
+-rw-r--r--   0        0        0     1918 2023-07-14 07:50:58.893264 reflex_ui-0.1.2/reflex/assets.py
+-rw-r--r--   0        0        0     2480 2023-07-02 17:23:24.247163 reflex_ui-0.1.2/reflex/common.py
+-rw-r--r--   0        0        0       47 2023-06-02 09:45:54.484185 reflex_ui-0.1.2/reflex/errors.py
+-rw-r--r--   0        0        0    36522 2023-07-02 17:49:31.901177 reflex_ui-0.1.2/reflex/generated/app.js
+-rw-r--r--   0        0        0    80229 2023-07-02 17:49:31.924510 reflex_ui-0.1.2/reflex/generated/app.js.map
+-rw-r--r--   0        0        0      287 2023-07-02 17:49:30.104509 reflex_ui-0.1.2/reflex/generated/index.html
+-rw-r--r--   0        0        0     4350 2023-07-02 17:49:30.834510 reflex_ui-0.1.2/reflex/generated/style.css
+-rw-r--r--   0        0        0     7562 2023-07-02 17:49:30.837843 reflex_ui-0.1.2/reflex/generated/style.css.map
+-rw-r--r--   0        0        0    75209 2022-04-21 09:32:25.000000 reflex_ui-0.1.2/reflex/hosted-assets/showdown.min.js
+-rw-r--r--   0        0        0     2521 2023-07-14 08:25:05.986574 reflex_ui-0.1.2/reflex/image_source.py
+-rw-r--r--   0        0        0     1229 2023-06-02 09:31:52.003332 reflex_ui-0.1.2/reflex/messages.py
+-rw-r--r--   0        0        0    38949 2023-07-14 07:51:46.796596 reflex_ui-0.1.2/reflex/session.py
+-rw-r--r--   0        0        0      123 2023-07-14 08:25:08.029908 reflex_ui-0.1.2/reflex/styling/__init__.py
+-rw-r--r--   0        0        0     3605 2023-07-14 07:53:45.156595 reflex_ui-0.1.2/reflex/styling/box_style.py
+-rw-r--r--   0        0        0     9391 2023-06-16 18:28:59.043338 reflex_ui-0.1.2/reflex/styling/color.py
+-rw-r--r--   0        0        0     2751 2023-07-14 07:53:45.159928 reflex_ui-0.1.2/reflex/styling/fills.py
+-rw-r--r--   0        0        0     2673 2023-07-14 08:24:26.589908 reflex_ui-0.1.2/reflex/styling/markdown_style.py
+-rw-r--r--   0        0        0     1762 2023-07-14 08:24:26.586575 reflex_ui-0.1.2/reflex/styling/text_style.py
+-rw-r--r--   0        0        0      274 2023-05-30 05:41:43.000000 reflex_ui-0.1.2/reflex/theme.py
+-rw-r--r--   0        0        0    12658 2023-07-14 08:24:26.576575 reflex_ui-0.1.2/reflex/validator.py
+-rw-r--r--   0        0        0      466 2023-07-14 08:40:58.956564 reflex_ui-0.1.2/reflex/widgets/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-14 08:25:06.019908 reflex_ui-0.1.2/reflex/widgets/auto_form.py
+-rw-r--r--   0        0        0     8439 2023-07-02 17:50:56.411212 reflex_ui-0.1.2/reflex/widgets/button.py
+-rw-r--r--   0        0        0     1577 2023-07-02 17:50:56.411212 reflex_ui-0.1.2/reflex/widgets/column.py
+-rw-r--r--   0        0        0      226 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/reflex/widgets/container.py
+-rw-r--r--   0        0        0     1827 2023-07-14 08:24:26.603242 reflex_ui-0.1.2/reflex/widgets/dropdown.py
+-rw-r--r--   0        0        0      506 2023-07-14 08:25:06.009908 reflex_ui-0.1.2/reflex/widgets/image.py
+-rw-r--r--   0        0        0     1175 2023-07-14 08:24:26.609908 reflex_ui-0.1.2/reflex/widgets/markdown_view.py
+-rw-r--r--   0        0        0      575 2023-07-14 08:25:06.013241 reflex_ui-0.1.2/reflex/widgets/media_player.py
+-rw-r--r--   0        0        0      939 2023-07-14 08:40:58.959897 reflex_ui-0.1.2/reflex/widgets/metadata.py
+-rw-r--r--   0        0        0     3524 2023-06-10 18:04:23.870009 reflex_ui-0.1.2/reflex/widgets/mouse_event_listener.py
+-rw-r--r--   0        0        0      498 2023-07-14 08:36:51.036567 reflex_ui-0.1.2/reflex/widgets/plot.py
+-rw-r--r--   0        0        0     1665 2023-07-02 17:50:56.411212 reflex_ui-0.1.2/reflex/widgets/progress_circle.py
+-rw-r--r--   0        0        0      506 2023-07-14 08:24:26.603242 reflex_ui-0.1.2/reflex/widgets/rectangle.py
+-rw-r--r--   0        0        0     1594 2023-07-02 17:44:56.264397 reflex_ui-0.1.2/reflex/widgets/row.py
+-rw-r--r--   0        0        0      242 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/reflex/widgets/stack.py
+-rw-r--r--   0        0        0     1566 2023-07-14 08:24:26.606575 reflex_ui-0.1.2/reflex/widgets/switch.py
+-rw-r--r--   0        0        0      363 2023-05-28 16:37:28.000000 reflex_ui-0.1.2/reflex/widgets/text.py
+-rw-r--r--   0        0        0     1894 2023-07-14 08:24:26.606575 reflex_ui-0.1.2/reflex/widgets/text_input.py
+-rw-r--r--   0        0        0    20757 2023-07-02 17:50:56.414545 reflex_ui-0.1.2/reflex/widgets/widget_base.py
+-rw-r--r--   0        0        0     3890 2023-07-14 08:24:26.583241 reflex_ui-0.1.2/reflex/world_units.py
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 reflex_ui-0.1.2/PKG-INFO
```

### Comparing `reflex_ui-0.1.1/LICENSE.txt` & `reflex_ui-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/pyproject.toml` & `reflex_ui-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "reflex-ui"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>", "Paul Pinterits"]
 readme = "README.md"
 packages = [{ include = "reflex" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typing-extensions = "^4.5.0"
+aiohttp = "^3.8.4"
+cefpython3 = { version = "^66.1", platform = "windows", optional = true }
 fastapi = "^0.95.1"
-uvicorn = "^0.22.0"
-uniserde = "^0.2.5"
-pillow = "^9.5.0"
-websocket = "^0.2.1"
-websockets = "^11.0.3"
-timer-dict = "^1.0.0"
 introspection = "^1.5.2"
-aiohttp = "^3.8.4"
-python-multipart = "^0.0.6"
-plotly = "^5.15.0"
+pillow = "^9.5.0"
+pygobject = { version = "^3.44.1", platform = "linux", optional = true }
 pytest = "^7.3.1"
-cefpython3 = { version = "^66.1", platform = "windows" }
-pygobject = { version = "^3.44.1", platform = "linux" }
-pywebview = "^4.2.2"
+python-multipart = "^0.0.6"
+pywebview = { version = "^4.2.2", optional = true }
+timer-dict = "^1.0.0"
+typing-extensions = "^4.5.0"
+uniserde = "^0.2.5"
+uvicorn = "^0.22.0"
+websockets = "^11.0.3"
+
+[tool.poetry.extras]
+window = ["cefpython3", "pygobject", "pywebview"]
 
 
 [tool.poetry.group.dev.dependencies]
 alt-pytest-asyncio = "^0.7.0"
 black = "^23.1.0"
 coverage = "^7.2.2"
 isort = "^5.12.0"
```

### Comparing `reflex_ui-0.1.1/reflex/app.py` & `reflex_ui-0.1.2/reflex/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 import asyncio
 import threading
 import webbrowser
 from typing import Awaitable, Callable, Optional
 
 import fastapi
 import uvicorn
-import webview
+
+import reflex as rx
 
 from . import app_server, validator
 from .image_source import ImageLike, ImageSource
 from .widgets import widget_base
-import reflex as rx
+
+# Only available with the `window` extra
+try:
+    import webview
+except ImportError:
+    webview = None
 
 
 __all__ = [
     "App",
 ]
 
 
@@ -116,22 +122,29 @@
             _validator_factory=_validator_factory,
             _on_startup=on_startup,
         )
 
     def run_in_window(
         self,
         quiet: bool = True,
-        _validator_factory: Optional[Callable[[rx.Session], validator.Validator]] = None,
+        _validator_factory: Optional[
+            Callable[[rx.Session], validator.Validator]
+        ] = None,
     ):
+        if webview is None:
+            raise Exception(
+                "The `window` extra is required to use `App.run_in_window`. Use `pip install reflex[window]` to install it."
+            )
+
         # Unfortunately, WebView must run in the main thread, which makes this
         # tricky. We'll have to banish uvicorn to a background thread, and shut
         # it down when the window is closed.
 
         # TODO: How to choose a free port?
-        host = 'localhost'
+        host = "localhost"
         port = 8000
         url = f"http://{host}:{port}"
 
         # This lock is released once the server is running
         lock = threading.Lock()
         lock.acquire()
```

### Comparing `reflex_ui-0.1.1/reflex/app_server.py` & `reflex_ui-0.1.2/reflex/app_server.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/assets.py` & `reflex_ui-0.1.2/reflex/assets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import secrets
 from pathlib import Path
-from typing import Union
+from typing import *  # type: ignore
 
 
 class HostedAsset:
     def __init__(
         self,
         media_type: str,
         data: Union[bytes, Path],
@@ -21,21 +21,31 @@
         # file containing the asset's data. The file must exist for the duration
         # of the asset's lifetime.
         self.data = data
 
         if isinstance(data, Path):
             assert data.exists(), f"Asset file {data} does not exist"
 
-    def url(self, server_external_url: str) -> str:
-        # TODO document this and/or enfoce it in the `AppServer` class already
-        assert not server_external_url.endswith(
-            "/"
-        ), "server_external_url must not end with a slash"
-
-        return f"{server_external_url}/reflex/asset/temp-{self.secret_id}"
+    def url(self, server_external_url: Optional[str] = None) -> str:
+        """
+        Returns the URL at which the asset can be accessed. If
+        `server_external_url` is passed the result will be an absolute URL. If
+        not, a relative URL is returned instead.
+        """
+
+        relative_url = f"/reflex/asset/temp-{self.secret_id}"
+
+        if server_external_url is None:
+            return relative_url
+        else:
+            # TODO document this and/or enfoce it in the `AppServer` class already
+            assert not server_external_url.endswith(
+                "/"
+            ), "server_external_url must not end with a slash"
+            return server_external_url + relative_url
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, HostedAsset):
             return NotImplemented
 
         if self.media_type != other.media_type:
             return False
```

### Comparing `reflex_ui-0.1.1/reflex/common.py` & `reflex_ui-0.1.2/reflex/common.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/generated/app.js` & `reflex_ui-0.1.2/reflex/generated/app.js`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/generated/app.js.map` & `reflex_ui-0.1.2/reflex/generated/app.js.map`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/generated/style.css` & `reflex_ui-0.1.2/reflex/generated/style.css`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/generated/style.css.map` & `reflex_ui-0.1.2/reflex/generated/style.css.map`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/hosted-assets/showdown.min.js` & `reflex_ui-0.1.2/reflex/hosted-assets/showdown.min.js`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/image_source.py` & `reflex_ui-0.1.2/reflex/image_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from . import assets
 
 
 class ImageSource:
     def __init__(
         self,
-        image: 'ImageLike',
+        image: "ImageLike",
         *,
         media_type: Optional[str] = None,
     ):
         if isinstance(image, ImageSource):
             self._url = image._url
             self._asset = image._asset
```

### Comparing `reflex_ui-0.1.1/reflex/messages.py` & `reflex_ui-0.1.2/reflex/messages.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/session.py` & `reflex_ui-0.1.2/reflex/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,15 +439,15 @@
             # by the server so the client can access it
             if (
                 isinstance(as_fill, styling.ImageFill)
                 and as_fill._image._asset is not None
             ):
                 self.app_server.weakly_host_asset(as_fill._image._asset)
 
-            return as_fill._serialize(self.app_server.external_url)
+            return as_fill._serialize()
 
         # Colors
         if type_ is styling.Color:
             return value.rgba
 
         # TextStyle
         if type_ is styling.TextStyle:
@@ -461,15 +461,15 @@
             # by the server so the client can access it
             if (
                 isinstance(value.fill, styling.ImageFill)
                 and value.fill._image._asset is not None
             ):
                 self.app_server.weakly_host_asset(value.fill._image._asset)
 
-            return value._serialize(self.app_server.external_url)
+            return value._serialize()
 
         # MarkdownStyle
         if type_ is styling.MarkdownStyle:
             return value._serialize()
 
         # Optional
         if origin is Union and len(args) == 2 and type(None) in args:
@@ -1033,15 +1033,15 @@
         self.app_server.weakly_host_asset(as_asset)
 
         # Tell the frontend to download the file
         await self.send_message(
             messages.EvaluateJavascript(
                 f"""
 const a = document.createElement('a')
-a.href = {json.dumps(as_asset.url(self.app_server.external_url))}
+a.href = {json.dumps(as_asset.url(None))}
 a.download = {json.dumps(file_name)}
 a.target = "_blank"
 document.body.appendChild(a)
 a.click()
 document.body.removeChild(a)
 """
             )
```

### Comparing `reflex_ui-0.1.1/reflex/styling/box_style.py` & `reflex_ui-0.1.2/reflex/styling/box_style.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing_extensions import Self
-from typing import Optional, Dict, Union, Tuple
-from .color import Color
 from dataclasses import dataclass
+from typing import Dict, Optional, Tuple, Union
+
+from typing_extensions import Self
+
 from ..common import Jsonable
 from . import fills
+from .color import Color
 
 
 @dataclass(frozen=True)
 class BoxStyle:
     fill: fills.Fill
     stroke_color: Color
     stroke_width: float
@@ -92,17 +94,17 @@
             if shadow_offset_x is None
             else shadow_offset_x,
             shadow_offset_y=self.shadow_offset_y
             if shadow_offset_y is None
             else shadow_offset_y,
         )
 
-    def _serialize(self, external_server_url: str) -> Dict[str, Jsonable]:
+    def _serialize(self) -> Dict[str, Jsonable]:
         return {
-            "fill": self.fill._serialize(external_server_url),
+            "fill": self.fill._serialize(),
             "strokeColor": self.stroke_color.rgba,
             "strokeWidth": self.stroke_width,
             "cornerRadius": self.corner_radius,
             "shadowColor": self.shadow_color.rgba,
             "shadowRadius": self.shadow_radius,
             "shadowOffset": (self.shadow_offset_x, self.shadow_offset_y),
         }
```

### Comparing `reflex_ui-0.1.1/reflex/styling/color.py` & `reflex_ui-0.1.2/reflex/styling/color.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/styling/fills.py` & `reflex_ui-0.1.2/reflex/styling/fills.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Iterable, Literal, Tuple, Union
-from ..image_source import ImageLike, ImageSource
 
 from ..common import Jsonable
+from ..image_source import ImageLike, ImageSource
 from .color import Color
 
 __all__ = [
     "Fill",
     "FillLike",
     "ImageFill",
     "LinearGradientFill",
@@ -26,23 +26,23 @@
 
         if isinstance(value, Color):
             return SolidFill(value)
 
         raise TypeError(f"Expected Fill or Color, got {type(value)}")
 
     @abstractmethod
-    def _serialize(self, server_external_url: str) -> Dict[str, Jsonable]:
+    def _serialize(self) -> Dict[str, Jsonable]:
         raise NotImplementedError()
 
 
 @dataclass(frozen=True, eq=True)
 class SolidFill(Fill):
     color: Color
 
-    def _serialize(self, server_external_url: str) -> Dict[str, Jsonable]:
+    def _serialize(self) -> Dict[str, Jsonable]:
         return {
             "type": "solid",
             "color": self.color.rgba,
         }
 
 
 @dataclass(frozen=True, eq=True)
@@ -61,15 +61,15 @@
 
         # Sort and store the stops
         vars(self).update(
             stops=tuple(sorted(stops, key=lambda x: x[1])),
             angle_degrees=angle_degrees,
         )
 
-    def _serialize(self, server_external_url: str) -> Dict[str, Jsonable]:
+    def _serialize(self) -> Dict[str, Jsonable]:
         return {
             "type": "linearGradient",
             "stops": [(color.rgba, position) for color, position in self.stops],
             "angleDegrees": self.angle_degrees,
         }
 
 
@@ -81,17 +81,17 @@
         fill_mode: Literal["fit", "stretch", "tile", "zoom"] = "fit",
         keep_aspect_ratio: bool = True,
         fill_entire_shape: bool = False,
     ):
         self._image = ImageSource(image)
         self._fill_mode = fill_mode
 
-    def _serialize(self, server_external_url: str) -> Dict[str, Jsonable]:
+    def _serialize(self) -> Dict[str, Jsonable]:
         image_url = (
-            self._image._asset.url(server_external_url)
+            self._image._asset.url()
             if self._image._asset is not None
             else self._image._url
         )
 
         return {
             "type": "image",
             "imageUrl": image_url,
```

### Comparing `reflex_ui-0.1.1/reflex/styling/markdown_style.py` & `reflex_ui-0.1.2/reflex/styling/markdown_style.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from dataclasses import dataclass, KW_ONLY
+from dataclasses import KW_ONLY, dataclass
+from typing import Literal, Optional, Tuple, Union
+
 from typing_extensions import Self
-from typing import Optional, Literal, Union, Tuple
+
 from .. import theme
 from . import text_style
 
 
 @dataclass(frozen=True)
 class MarkdownStyle:
     # Headers
```

### Comparing `reflex_ui-0.1.1/reflex/styling/text_style.py` & `reflex_ui-0.1.2/reflex/styling/text_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from dataclasses import dataclass, KW_ONLY
+from dataclasses import KW_ONLY, dataclass
+from typing import Dict, Literal, Optional
+
 from typing_extensions import Self
-from typing import Optional, Literal, Dict
-from .color import Color
+
 from ..common import Jsonable
+from .color import Color
 
 
 @dataclass(frozen=True)
 class TextStyle:
     _: KW_ONLY
     font_name: Optional[str] = None
     font_color: Color = Color.BLACK
```

### Comparing `reflex_ui-0.1.1/reflex/validator.py` & `reflex_ui-0.1.2/reflex/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import copy
 import json
 import re
 from dataclasses import dataclass
-import reflex.widgets.metadata
-from . import session
 from pathlib import Path
 from typing import Dict, Iterable, List, Optional, Set, Union
 
-from . import messages
+import reflex.widgets.metadata
+
+from . import messages, session
 from .common import Jsonable
 
 __all__ = [
     "ClientWidget",
     "ValidationError",
     "Validator",
 ]
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/auto_form.py` & `reflex_ui-0.1.2/reflex/widgets/auto_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-import reflex as rx
+import enum
 from dataclasses import dataclass
 from typing import *  # type: ignore
-import enum
 
+import reflex as rx
 
 __all__ = [
     "AutoFormBuilder",
 ]
 
 
 T = TypeVar("T")
@@ -73,16 +73,16 @@
     def build(self) -> rx.Widget:
         rows: List[rx.Widget] = []
 
         # One row per field
         for field in self.fields:
             rows.append(
                 rx.Row(
-                        rx.Text(field.name),
-                        self._build_input_field(field),
+                    rx.Text(field.name),
+                    self._build_input_field(field),
                     spacing=self.spacing,
                 )
             )
 
         # Add a submit button
         rows.append(
             rx.Button.major(
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/button.py` & `reflex_ui-0.1.2/reflex/widgets/button.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/widgets/column.py` & `reflex_ui-0.1.2/reflex/widgets/column.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/widgets/dropdown.py` & `reflex_ui-0.1.2/reflex/widgets/dropdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 from dataclasses import KW_ONLY, dataclass
 from typing import *  # type: ignore
 
-
 import reflex as rx
 
 from ..styling import *
 from . import widget_base
 
 __all__ = [
     "Dropdown",
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/markdown_view.py` & `reflex_ui-0.1.2/reflex/widgets/markdown_view.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-from .. import session
 
+from .. import session
 from . import widget_base
 
 __all__ = [
     "MarkdownView",
 ]
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/media_player.py` & `reflex_ui-0.1.2/reflex/widgets/media_player.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
 from pathlib import Path
 from typing import Union
 
 from . import widget_base
@@ -16,11 +15,13 @@
     loop: bool = True
     autoplay: bool = True
     controls: bool = True
     muted: bool = False
     volume: float = 1.0
 
     def __post_init__(self):
-        self._media_url = self.media if isinstance(self.media, str) else self.media.FIXME
+        self._media_url = (
+            self.media if isinstance(self.media, str) else self.media.FIXME
+        )
 
 
 MediaPlayer._unique_id = "MediaPlayer-builtin"
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/mouse_event_listener.py` & `reflex_ui-0.1.2/reflex/widgets/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/widgets/progress_circle.py` & `reflex_ui-0.1.2/reflex/widgets/progress_circle.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/widgets/row.py` & `reflex_ui-0.1.2/reflex/widgets/row.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/widgets/switch.py` & `reflex_ui-0.1.2/reflex/widgets/switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
 from typing import Dict
 
-from reflex.common import Jsonable
-from .. import theme
-
 from typing_extensions import Self
 
 import reflex as rx
+from reflex.common import Jsonable
 
+from .. import theme
 from ..common import Jsonable
 from . import widget_base
 
 __all__ = ["Switch", "SwitchChangeEvent"]
 
 
 @dataclass
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/text_input.py` & `reflex_ui-0.1.2/reflex/widgets/text_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY, dataclass
 from typing import *  # type: ignore
 
-
 from ..common import Jsonable
 from . import widget_base
 
 __all__ = [
     "TextInput",
     "TextInputChangeEvent",
     "TextInputConfirmEvent",
```

### Comparing `reflex_ui-0.1.1/reflex/widgets/widget_base.py` & `reflex_ui-0.1.2/reflex/widgets/widget_base.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.1/reflex/world_units.py` & `reflex_ui-0.1.2/reflex/world_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from dataclasses import dataclass, KW_ONLY
+from dataclasses import KW_ONLY, dataclass
 from typing import *  # type: ignore
 
-
 # https://github.com/forgedsoftware/measurementcommon/blob/master/systems.json
 
 
 SI_PREFIXES = (
     (24, "yotta", "Y"),
     (21, "zetta", "Z"),
     (18, "exa", "E"),
```

### Comparing `reflex_ui-0.1.1/PKG-INFO` & `reflex_ui-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: reflex-ui
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: window
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: cefpython3 (>=66.1,<67.0) ; sys_platform == "windows"
+Requires-Dist: cefpython3 (>=66.1,<67.0) ; (sys_platform == "windows") and (extra == "window")
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: introspection (>=1.5.2,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: plotly (>=5.15.0,<6.0.0)
-Requires-Dist: pygobject (>=3.44.1,<4.0.0) ; sys_platform == "linux"
+Requires-Dist: pygobject (>=3.44.1,<4.0.0) ; (sys_platform == "linux") and (extra == "window")
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
-Requires-Dist: pywebview (>=4.2.2,<5.0.0)
+Requires-Dist: pywebview (>=4.2.2,<5.0.0) ; extra == "window"
 Requires-Dist: timer-dict (>=1.0.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: uniserde (>=0.2.5,<0.3.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
-Requires-Dist: websocket (>=0.2.1,<0.3.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
```

