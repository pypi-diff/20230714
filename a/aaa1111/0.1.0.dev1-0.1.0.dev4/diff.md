# Comparing `tmp/aaa1111-0.1.0.dev1.tar.gz` & `tmp/aaa1111-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaa1111-0.1.0.dev1.tar", last modified: Thu Jul 13 16:02:33 2023, max compression
+gzip compressed data, was "aaa1111-0.1.0.dev4.tar", last modified: Fri Jul 14 13:10:42 2023, max compression
```

## Comparing `aaa1111-0.1.0.dev1.tar` & `aaa1111-0.1.0.dev4.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     1083 2023-07-13 05:37:34.132225 aaa1111-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0       88 2023-07-13 15:33:45.322313 aaa1111-0.1.0.dev1/README.md
--rw-r--r--   0        0        0        0 2023-07-13 05:44:31.695257 aaa1111-0.1.0.dev1/aaa1111/__init__.py
--rw-r--r--   0        0        0     3721 2023-07-13 15:50:27.328303 aaa1111-0.1.0.dev1/aaa1111/__main__.py
--rw-r--r--   0        0        0       28 2023-07-13 15:34:46.644465 aaa1111-0.1.0.dev1/aaa1111/__version__.py
--rw-r--r--   0        0        0     5706 2023-07-13 15:47:51.176447 aaa1111-0.1.0.dev1/aaa1111/client.py
--rw-r--r--   0        0        0     3529 2023-07-13 12:43:21.501472 aaa1111-0.1.0.dev1/aaa1111/types.py
--rw-r--r--   0        0        0     3855 2023-07-13 15:51:29.446528 aaa1111-0.1.0.dev1/aaa1111/utils.py
--rw-r--r--   0        0        0     1186 2023-07-13 16:02:33.009190 aaa1111-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 aaa1111-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-13 05:37:34.132225 aaa1111-0.1.0.dev4/LICENSE
+-rw-r--r--   0        0        0       88 2023-07-13 15:33:45.322313 aaa1111-0.1.0.dev4/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 05:44:31.695257 aaa1111-0.1.0.dev4/aaa1111/__init__.py
+-rw-r--r--   0        0        0     6235 2023-07-14 12:34:58.164236 aaa1111-0.1.0.dev4/aaa1111/__main__.py
+-rw-r--r--   0        0        0       28 2023-07-14 07:05:38.542707 aaa1111-0.1.0.dev4/aaa1111/__version__.py
+-rw-r--r--   0        0        0       52 2023-07-14 05:41:34.045117 aaa1111-0.1.0.dev4/aaa1111/client/__init__.py
+-rw-r--r--   0        0        0     3435 2023-07-14 07:07:50.741981 aaa1111-0.1.0.dev4/aaa1111/client/extras.py
+-rw-r--r--   0        0        0     3461 2023-07-14 07:08:57.775642 aaa1111-0.1.0.dev4/aaa1111/client/main.py
+-rw-r--r--   0        0        0     3387 2023-07-14 06:19:38.538109 aaa1111-0.1.0.dev4/aaa1111/client/toimg.py
+-rw-r--r--   0        0        0      386 2023-07-14 06:13:53.739597 aaa1111-0.1.0.dev4/aaa1111/types/__init__.py
+-rw-r--r--   0        0        0      427 2023-07-14 12:29:28.450074 aaa1111-0.1.0.dev4/aaa1111/types/base.py
+-rw-r--r--   0        0        0     1980 2023-07-14 07:08:09.213639 aaa1111-0.1.0.dev4/aaa1111/types/extras.py
+-rw-r--r--   0        0        0     3547 2023-07-14 06:13:46.741195 aaa1111-0.1.0.dev4/aaa1111/types/toimg.py
+-rw-r--r--   0        0        0     4724 2023-07-14 12:31:45.041606 aaa1111-0.1.0.dev4/aaa1111/utils.py
+-rw-r--r--   0        0        0     1186 2023-07-14 13:10:42.713395 aaa1111-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 aaa1111-0.1.0.dev4/PKG-INFO
```

### Comparing `aaa1111-0.1.0.dev1/LICENSE` & `aaa1111-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev1/aaa1111/types.py` & `aaa1111-0.1.0.dev4/aaa1111/types/toimg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from enum import IntEnum
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Mapping, Optional, Sized, Union
+from typing import Any, Dict, List, Literal, Mapping, Optional, Union
 
 from beartype import beartype
 from PIL import Image
 
+from aaa1111.utils import base64_to_image
+
+from .base import AsdictMixin
+
 Number = Union[int, float]
 
 
 @beartype
 @dataclass
-class _2IMG:  # noqa: N801
+class _2IMG(AsdictMixin):  # noqa: N801
     prompt: str = ""
     styles: List[str] = field(default_factory=list)
     seed: int = -1
     subseed: int = -1
     subseed_strength: Number = 0.0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
@@ -41,24 +45,14 @@
     override_settings_restore_afterwards: bool = True
     script_args: List[Any] = field(default_factory=list)
     script_name: Optional[str] = None
     send_images: bool = True
     save_images: bool = False
     alwayson_scripts: Mapping[str, Any] = field(default_factory=dict)
 
-    def asdict(self) -> Dict[str, Any]:
-        d = asdict(self)
-        for attr in self.__dataclass_fields__:
-            value = getattr(self, attr)
-            default = self.__dataclass_fields__[attr].default
-
-            if value == default or (isinstance(value, Sized) and not value):
-                del d[attr]
-        return d
-
 
 @beartype
 @dataclass
 class TXT2IMG(_2IMG):
     enable_hr: bool = False
     denoising_strength: Number = 0.0
     firstphase_width: int = 0
@@ -107,13 +101,21 @@
     inpaint_full_res: bool = True
     inpaint_full_res_padding: int = 0
     inpainting_mask_invert: Union[
         InpaintingMaskInvert, Literal[0, 1]
     ] = InpaintingMaskInvert.Inpaint_masked
     initial_noise_multiplier: Optional[Number] = None
 
+    ResizeMode = ResizeMode
+    InpaintingFill = InpaintingFill
+    InpaintingMaskInvert = InpaintingMaskInvert
+
 
 @dataclass
-class Response:
+class ToImageResponse:
     images: List[Image.Image]
     parameters: Dict[str, Any]
     info: Dict[str, Any]
+
+    def __post_init__(self):
+        if self.images and isinstance(self.images[0], str):
+            self.images = [base64_to_image(img) for img in self.images]
```

### Comparing `aaa1111-0.1.0.dev1/aaa1111/utils.py` & `aaa1111-0.1.0.dev4/aaa1111/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import base64
 import io
 from pathlib import Path
-from typing import Any, Dict, Mapping, Sequence, Union
+from typing import Any, Dict, Mapping, Optional, Sequence, Union
 
 import filetype
 import orjson
 import rtoml
 from aiofile import async_open
-from PIL import Image
+from PIL import Image, PngImagePlugin
 from ruamel.yaml import YAML
+from ulid import ULID
 
 Image_Type = Union[str, Path, Image.Image]
 DICT_EXT = (".toml", ".yaml", ".yml", ".json")
 
 
 def image_to_base64(img: Image_Type) -> str:
     if isinstance(img, Image.Image):
@@ -122,7 +123,34 @@
         data = await raw.read()
         if ext == ".toml":
             return rtoml.loads(data)
         if ext == ".json":
             return orjson.loads(data)
         yaml = YAML()
         return dict(yaml.load(data))
+
+
+def save_image(
+    image: Image.Image,
+    save_dir: Path,
+    infotext: Optional[str] = None,
+    ext: str = "png",
+    quality: int = 95,
+    lossless: bool = True,
+):
+    if not ext.startswith("."):
+        ext = "." + ext
+    path = save_dir.joinpath(str(ULID())).with_suffix(ext)
+    if not infotext:
+        image.save(path, quality=quality, lossless=lossless)
+        return
+
+    if ext.lower().endswith("png"):
+        pnginfo = PngImagePlugin.PngInfo()
+        pnginfo.add_text("parameters", infotext)
+        image.save(path, pnginfo=pnginfo, quality=quality)
+        return
+
+    exif = image.getexif()
+    # https://github.com/python-pillow/Pillow/issues/4935#issuecomment-698027721
+    exif[0x9286] = infotext
+    image.save(path, quality=quality, lossless=lossless, exif=exif)
```

### Comparing `aaa1111-0.1.0.dev1/pyproject.toml` & `aaa1111-0.1.0.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "python-ulid",
     "rich",
     "typer",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.0.dev1"
+version = "0.1.0.dev4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/Bing-su/AAA1111"
```

### Comparing `aaa1111-0.1.0.dev1/PKG-INFO` & `aaa1111-0.1.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaa1111
-Version: 0.1.0.dev1
+Version: 0.1.0.dev4
 Summary: An Api for Automatic1111
 Author-Email: Bingsu <ks2515@naver.com>
 License: MIT
 Project-URL: Repository, https://github.com/Bing-su/AAA1111
 Requires-Python: >=3.8
 Requires-Dist: httpx
 Requires-Dist: aiofile
```

