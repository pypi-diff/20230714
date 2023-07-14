# Comparing `tmp/filedata-ext-0.2.1.tar.gz` & `tmp/filedata-ext-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedata-ext-0.2.1.tar", last modified: Thu Jun 15 10:27:58 2023, max compression
+gzip compressed data, was "filedata-ext-0.2.2.tar", last modified: Fri Jul 14 10:49:59 2023, max compression
```

## Comparing `filedata-ext-0.2.1.tar` & `filedata-ext-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.450572 filedata-ext-0.2.1/
--rwxrwxrwx   0 root         (0) root         (0)      111 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-06-15 10:27:58.450572 filedata-ext-0.2.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:57.807084 filedata-ext-0.2.1/filedata_ext/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-15 10:27:12.000000 filedata-ext-0.2.1/filedata_ext/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       83 2023-06-14 00:46:36.000000 filedata-ext-0.2.1/filedata_ext/constants.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.090324 filedata-ext-0.2.1/filedata_ext/data_models/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/data_models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      378 2023-06-14 05:25:29.000000 filedata-ext-0.2.1/filedata_ext/data_models/file_info.py
--rwxrwxrwx   0 root         (0) root         (0)      368 2023-06-13 09:47:04.000000 filedata-ext-0.2.1/filedata_ext/data_models/ocr.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.200069 filedata-ext-0.2.1/filedata_ext/services/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/services/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8500 2023-06-14 05:26:37.000000 filedata-ext-0.2.1/filedata_ext/services/file_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     5911 2023-06-15 10:26:31.000000 filedata-ext-0.2.1/filedata_ext/services/filedata_cache.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.246944 filedata-ext-0.2.1/filedata_ext/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      450 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/filedata_ext/utils/video.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:57.933092 filedata-ext-0.2.1/filedata_ext.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      726 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.2.1/filedata_ext.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-06-15 10:27:57.000000 filedata-ext-0.2.1/filedata_ext.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.278202 filedata-ext-0.2.1/requirements/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/requirements/test.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-15 10:27:58.450572 filedata-ext-0.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1453 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.325562 filedata-ext-0.2.1/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.1/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1748 2023-06-14 05:29:55.000000 filedata-ext-0.2.1/tests/file_handler_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 10:27:58.419324 filedata-ext-0.2.1/tests/resources/
--rwxrwxrwx   0 root         (0) root         (0)    18180 2023-06-14 00:39:13.000000 filedata-ext-0.2.1/tests/resources/example.docx
--rwxrwxrwx   0 root         (0) root         (0)   130941 2023-06-14 00:42:50.000000 filedata-ext-0.2.1/tests/resources/example.pdf
--rwxrwxrwx   0 root         (0) root         (0)   231039 2023-06-14 00:27:17.000000 filedata-ext-0.2.1/tests/resources/example.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.627769 filedata-ext-0.2.2/
+-rwxrwxrwx   0 root         (0) root         (0)      111 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-07-14 10:49:59.622734 filedata-ext-0.2.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:58.945634 filedata-ext-0.2.2/filedata_ext/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-07-14 10:06:55.000000 filedata-ext-0.2.2/filedata_ext/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       83 2023-06-14 00:46:36.000000 filedata-ext-0.2.2/filedata_ext/constants.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.220038 filedata-ext-0.2.2/filedata_ext/data_models/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/filedata_ext/data_models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      378 2023-06-14 05:25:29.000000 filedata-ext-0.2.2/filedata_ext/data_models/file_info.py
+-rwxrwxrwx   0 root         (0) root         (0)      368 2023-06-13 09:47:04.000000 filedata-ext-0.2.2/filedata_ext/data_models/ocr.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.323269 filedata-ext-0.2.2/filedata_ext/services/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/filedata_ext/services/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8500 2023-06-14 05:26:37.000000 filedata-ext-0.2.2/filedata_ext/services/file_handler.py
+-rwxrwxrwx   0 root         (0) root         (0)     6288 2023-07-14 10:48:36.000000 filedata-ext-0.2.2/filedata_ext/services/filedata_cache.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.385884 filedata-ext-0.2.2/filedata_ext/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/filedata_ext/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      450 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/filedata_ext/utils/video.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.143800 filedata-ext-0.2.2/filedata_ext.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-07-14 10:49:58.000000 filedata-ext-0.2.2/filedata_ext.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      726 2023-07-14 10:49:58.000000 filedata-ext-0.2.2/filedata_ext.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-14 10:49:58.000000 filedata-ext-0.2.2/filedata_ext.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-14 08:37:07.000000 filedata-ext-0.2.2/filedata_ext.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-07-14 10:49:58.000000 filedata-ext-0.2.2/filedata_ext.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-14 10:49:58.000000 filedata-ext-0.2.2/filedata_ext.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.401514 filedata-ext-0.2.2/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/requirements/test.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-14 10:49:59.627769 filedata-ext-0.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1453 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.463773 filedata-ext-0.2.2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 00:03:29.000000 filedata-ext-0.2.2/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1748 2023-07-01 00:54:32.000000 filedata-ext-0.2.2/tests/file_handler_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 10:49:59.590840 filedata-ext-0.2.2/tests/resources/
+-rwxrwxrwx   0 root         (0) root         (0)    18180 2023-06-14 00:39:13.000000 filedata-ext-0.2.2/tests/resources/example.docx
+-rwxrwxrwx   0 root         (0) root         (0)   130941 2023-06-14 00:42:50.000000 filedata-ext-0.2.2/tests/resources/example.pdf
+-rwxrwxrwx   0 root         (0) root         (0)   231039 2023-06-14 00:27:17.000000 filedata-ext-0.2.2/tests/resources/example.png
```

### Comparing `filedata-ext-0.2.1/PKG-INFO` & `filedata-ext-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedata-ext
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extensions of filedata for guniflask
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filedata-ext-0.2.1/filedata_ext/services/file_handler.py` & `filedata-ext-0.2.2/filedata_ext/services/file_handler.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2.1/filedata_ext/services/filedata_cache.py` & `filedata-ext-0.2.2/filedata_ext/services/filedata_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import datetime as dt
 import io
 from typing import List, Optional, Any, Type, TypeVar
 
 import gevent
 import requests
 from PIL import Image
 from filedata.image import ocr_with_angle_correction, OCRResult
 from filedata.pdf import pdf_to_image
 from filedata.retry import retry_api
+from filedata.time import get_current_datetime
 from guniflask.config import settings
 from kikyo import Kikyo, OSS
 from kikyo.bundle.search import EsBasedSearch
 from pydantic import BaseModel
 
 from filedata_ext.constants import FILEDATA_CACHE_ENDPOINT, THUMBNAIL_NUM
 from filedata_ext.data_models.file_info import FileInfo
@@ -18,14 +20,15 @@
 
 
 class Cache(BaseModel):
     filename: str = None
     md5: str
     file_link: str = None
     data: Any
+    create_time: dt.datetime = None
 
 
 class CacheKey:
     OCR = 'ocr'
     FILE_INFO = 'file_info'
 
 
@@ -163,14 +166,15 @@
         )
         if resp.status_code == 404:
             return
         resp.raise_for_status()
         return Cache(**resp.json()['data'])
 
     def save_cache(self, key: str, cache: Cache):
+        cache.create_time = None
         self.session.post(
             f'{self.endpoint}api/cache',
             json=cache.dict(),
             params={
                 'key': key,
             },
             timeout=20,
@@ -182,15 +186,22 @@
             params={
                 'md5': md5,
                 'key': key,
             },
             timeout=20,
         )
 
-    def get_typed_cache(self, key: str, md5: str, cls: Type[T]) -> Optional[T]:
+    def get_typed_cache(self, key: str, md5: str, cls: Type[T], shelf_life: int = None) -> Optional[T]:
         cache = self.get_cache(key=key, md5=md5)
         if cache is None:
             return
+
+        if shelf_life is not None:
+            if cache.create_time is None:
+                return
+            if (get_current_datetime() - cache.create_time).total_seconds() > shelf_life:
+                return
+
         return cls(**cache.data)
 
     def save_typed_cache(self, key: str, md5: str, data: Any):
         self.save_cache(key=key, cache=Cache(md5=md5, data=data))
```

### Comparing `filedata-ext-0.2.1/filedata_ext.egg-info/PKG-INFO` & `filedata-ext-0.2.2/filedata_ext.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedata-ext
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extensions of filedata for guniflask
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `filedata-ext-0.2.1/filedata_ext.egg-info/SOURCES.txt` & `filedata-ext-0.2.2/filedata_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2.1/setup.py` & `filedata-ext-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2.1/tests/file_handler_test.py` & `filedata-ext-0.2.2/tests/file_handler_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 @pytest.fixture(scope='module')
 def file_handler(kikyo_client, filedata_cache):
     return FileHandlerService(kikyo_client=kikyo_client, filedata_cache=filedata_cache)
 
 
-resource_dir = join(dirname(__name__), 'resources')
+resource_dir = join(dirname(__file__), 'resources')
 
 
 def test_image(file_handler: FileHandlerService):
     with open(join(resource_dir, 'example.png'), 'rb') as f:
         img_bytes = f.read()
     result = file_handler.extract_file_content(file_bytes=img_bytes)
     assert isinstance(result, FileContentResult)
```

### Comparing `filedata-ext-0.2.1/tests/resources/example.docx` & `filedata-ext-0.2.2/tests/resources/example.docx`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2.1/tests/resources/example.pdf` & `filedata-ext-0.2.2/tests/resources/example.pdf`

 * *Files identical despite different names*

### Comparing `filedata-ext-0.2.1/tests/resources/example.png` & `filedata-ext-0.2.2/tests/resources/example.png`

 * *Files identical despite different names*

