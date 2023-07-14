# Comparing `tmp/jmcomic-2.1.1.tar.gz` & `tmp/jmcomic-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.1.tar", last modified: Thu Jul 13 14:04:49 2023, max compression
+gzip compressed data, was "jmcomic-2.1.2.tar", last modified: Fri Jul 14 11:53:26 2023, max compression
```

## Comparing `jmcomic-2.1.1.tar` & `jmcomic-2.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.065920 jmcomic-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-13 14:04:34.000000 jmcomic-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 14:04:49.065920 jmcomic-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-13 14:04:34.000000 jmcomic-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:04:49.065920 jmcomic-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-13 14:04:34.000000 jmcomic-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.061920 jmcomic-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.065920 jmcomic-2.1.1/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-13 14:04:34.000000 jmcomic-2.1.1/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:04:49.065920 jmcomic-2.1.1/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 14:04:49.000000 jmcomic-2.1.1/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:53:26.479011 jmcomic-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-14 11:53:17.000000 jmcomic-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-14 11:53:26.479011 jmcomic-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-14 11:53:17.000000 jmcomic-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:53:26.479011 jmcomic-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 11:53:17.000000 jmcomic-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:53:26.479011 jmcomic-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:53:26.479011 jmcomic-2.1.2/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-14 11:53:17.000000 jmcomic-2.1.2/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:53:26.479011 jmcomic-2.1.2/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-14 11:53:26.000000 jmcomic-2.1.2/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-14 11:53:26.000000 jmcomic-2.1.2/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:53:26.000000 jmcomic-2.1.2/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 11:53:26.000000 jmcomic-2.1.2/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 11:53:26.000000 jmcomic-2.1.2/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.1/LICENSE` & `jmcomic-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/PKG-INFO` & `jmcomic-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.1.1/README.md` & `jmcomic-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/setup.py` & `jmcomic-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/src/jmcomic/api.py` & `jmcomic-2.1.2/src/jmcomic/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 
     option, jm_client = build_client(option)
     album: JmAlbumDetail = jm_client.get_album_detail(jm_album_id)
 
     jm_debug('album',
              f'本子获取成功: [{album.id}], '
              f'作者: [{album.author}], '
-             f'章节数: [{len(album)}]'
+             f'章节数: [{len(album)}], '
              f'标题: [{album.title}], '
              )
 
     def download_photo(photo: JmPhotoDetail,
                        debug_topic='photo',
                        ):
         jm_client.check_photo(photo)
 
         jm_debug(debug_topic,
                  f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}]), '
                  f'标题: [{photo.title}], '
-                 f'图片数为[{len(photo)}]')
+                 f'图片数为[{len(photo)}]'
+                 )
 
         download_by_photo_detail(photo, option)
 
-        jm_debug(debug_topic, f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}])')
+        jm_debug(debug_topic,
+                 f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(album)}])'
+                 )
 
     thread_pool_executor(
         iter_objs=album,
         apply_each_obj_func=download_photo,
     )
 
     jm_debug('album', f'本子下载完成: [{album.id}]')
@@ -94,26 +97,28 @@
     def download_image(index, image: JmImageDetail, debug_topic='image'):
         img_save_path = option.decide_image_filepath(photo_detail, index)
         debug_tag = f'{image.aid}/{image.filename} [{index + 1}/{len(photo_detail)}]'
 
         # 已下载过，缓存命中
         if use_cache is True and file_exists(img_save_path):
             jm_debug(debug_topic,
-                     f'图片已存在: {debug_tag} ← [{img_save_path}]')
+                     f'图片已存在: {debug_tag} ← [{img_save_path}]'
+                     )
             return
 
         # 开始下载
         jm_client.download_by_image_detail(
             image,
             img_save_path,
             decode_image=decode_image,
         )
 
         jm_debug(debug_topic,
-                 f'图片下载完成: {debug_tag}, [{image.img_url}] → [{img_save_path}]')
+                 f'图片下载完成: {debug_tag}, [{image.img_url}] → [{img_save_path}]'
+                 )
 
     length = len(photo_detail)
     # 根据图片数，决定下载策略
     if length <= option.download_threading_batch_count:
         # 如果图片数小的话，直接使用多线程下载，一张图一个线程。
         multi_thread_launcher(
             iter_objs=enumerate(photo_detail),
```

### Comparing `jmcomic-2.1.1/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.2/src/jmcomic/jm_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
     def get_jm_image(self, img_url) -> JmImageResp:
 
         def get_if_fail_raise(url):
             """
             使用此方法包装 self.get
             """
-            resp = JmImageResp(self.get(url))
+            resp = JmImageResp(self.get(url, params={'v': format_ts()}))
 
             if resp.is_success:
                 return resp
 
             self.raise_request_error(
                 resp.resp, resp.get_error_msg()
             )
```

### Comparing `jmcomic-2.1.1/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.2/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/src/jmcomic/jm_config.py` & `jmcomic-2.1.2/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/src/jmcomic/jm_entity.py` & `jmcomic-2.1.2/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/src/jmcomic/jm_option.py` & `jmcomic-2.1.2/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.2/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.1/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.2/src/jmcomic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

