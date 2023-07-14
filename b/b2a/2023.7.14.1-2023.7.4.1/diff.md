# Comparing `tmp/b2a-2023.7.14.1.tar.gz` & `tmp/b2a-2023.7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2a-2023.7.14.1.tar", last modified: Fri Jul 14 06:12:56 2023, max compression
+gzip compressed data, was "b2a-2023.7.4.1.tar", last modified: Fri Jul 14 03:18:41 2023, max compression
```

## Comparing `b2a-2023.7.14.1.tar` & `b2a-2023.7.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:12:56.613423 b2a-2023.7.14.1/
--rw-rw-rw-   0        0        0      220 2023-07-14 06:12:56.612423 b2a-2023.7.14.1/PKG-INFO
--rw-rw-rw-   0        0        0     2026 2023-07-14 02:17:07.000000 b2a-2023.7.14.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 06:12:56.577427 b2a-2023.7.14.1/b2a/
--rw-rw-rw-   0        0        0     8301 2023-07-14 06:12:34.000000 b2a-2023.7.14.1/b2a/__init__.py
--rw-rw-rw-   0        0        0    14512 2023-07-14 06:10:44.000000 b2a-2023.7.14.1/b2a/aliplat.py
--rw-rw-rw-   0        0        0     5160 2023-07-14 03:12:52.000000 b2a-2023.7.14.1/b2a/bdyplat.py
--rw-rw-rw-   0        0        0      740 2021-08-04 01:00:20.000000 b2a-2023.7.14.1/b2a/common.py
--rw-rw-rw-   0        0        0     1126 2023-07-14 03:14:28.000000 b2a-2023.7.14.1/b2a/config.py
--rw-rw-rw-   0        0        0     4089 2023-07-14 02:55:04.000000 b2a-2023.7.14.1/b2a/downloader.py
--rw-rw-rw-   0        0        0     1329 2021-07-30 06:38:18.000000 b2a-2023.7.14.1/b2a/platformImp.py
--rw-rw-rw-   0        0        0     3204 2023-07-14 03:04:24.000000 b2a-2023.7.14.1/b2a/trans.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:12:56.604424 b2a-2023.7.14.1/b2a.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-14 06:12:56.000000 b2a-2023.7.14.1/b2a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-07-14 06:12:56.000000 b2a-2023.7.14.1/b2a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:12:56.000000 b2a-2023.7.14.1/b2a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-14 06:12:56.000000 b2a-2023.7.14.1/b2a.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-14 06:12:56.000000 b2a-2023.7.14.1/b2a.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 06:12:56.000000 b2a-2023.7.14.1/b2a.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 06:12:56.610424 b2a-2023.7.14.1/b2a_gui/
--rw-rw-rw-   0        0        0     1036 2022-06-07 03:58:14.000000 b2a-2023.7.14.1/b2a_gui/__init__.py
--rw-rw-rw-   0        0        0     3959 2021-07-27 06:28:28.000000 b2a-2023.7.14.1/b2a_gui/download.py
--rw-rw-rw-   0        0        0     2712 2021-07-27 03:01:49.000000 b2a-2023.7.14.1/b2a_gui/main.py
--rw-rw-rw-   0        0        0       42 2023-07-14 06:12:56.614425 b2a-2023.7.14.1/setup.cfg
--rw-rw-rw-   0        0        0      508 2021-09-23 08:50:57.000000 b2a-2023.7.14.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:18:41.154370 b2a-2023.7.4.1/
+-rw-rw-rw-   0        0        0      219 2023-07-14 03:18:41.153370 b2a-2023.7.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2026 2023-07-14 02:17:07.000000 b2a-2023.7.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 03:18:41.110370 b2a-2023.7.4.1/b2a/
+-rw-rw-rw-   0        0        0     8301 2023-07-14 03:16:24.000000 b2a-2023.7.4.1/b2a/__init__.py
+-rw-rw-rw-   0        0        0    14056 2023-07-14 02:17:07.000000 b2a-2023.7.4.1/b2a/aliplat.py
+-rw-rw-rw-   0        0        0     5160 2023-07-14 03:12:52.000000 b2a-2023.7.4.1/b2a/bdyplat.py
+-rw-rw-rw-   0        0        0      740 2021-08-04 01:00:20.000000 b2a-2023.7.4.1/b2a/common.py
+-rw-rw-rw-   0        0        0     1126 2023-07-14 03:14:28.000000 b2a-2023.7.4.1/b2a/config.py
+-rw-rw-rw-   0        0        0     4089 2023-07-14 02:55:04.000000 b2a-2023.7.4.1/b2a/downloader.py
+-rw-rw-rw-   0        0        0     1329 2021-07-30 06:38:18.000000 b2a-2023.7.4.1/b2a/platformImp.py
+-rw-rw-rw-   0        0        0     3204 2023-07-14 03:04:24.000000 b2a-2023.7.4.1/b2a/trans.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:18:41.126371 b2a-2023.7.4.1/b2a.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-07-14 03:18:40.000000 b2a-2023.7.4.1/b2a.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-07-14 03:18:40.000000 b2a-2023.7.4.1/b2a.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 03:18:40.000000 b2a-2023.7.4.1/b2a.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-14 03:18:40.000000 b2a-2023.7.4.1/b2a.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-07-14 03:18:40.000000 b2a-2023.7.4.1/b2a.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 03:18:40.000000 b2a-2023.7.4.1/b2a.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 03:18:41.151380 b2a-2023.7.4.1/b2a_gui/
+-rw-rw-rw-   0        0        0     1036 2022-06-07 03:58:14.000000 b2a-2023.7.4.1/b2a_gui/__init__.py
+-rw-rw-rw-   0        0        0     3959 2021-07-27 06:28:28.000000 b2a-2023.7.4.1/b2a_gui/download.py
+-rw-rw-rw-   0        0        0     2712 2021-07-27 03:01:49.000000 b2a-2023.7.4.1/b2a_gui/main.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 03:18:41.154370 b2a-2023.7.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      508 2021-09-23 08:50:57.000000 b2a-2023.7.4.1/setup.py
```

### Comparing `b2a-2023.7.14.1/README.md` & `b2a-2023.7.4.1/README.md`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a/__init__.py` & `b2a-2023.7.4.1/b2a/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 |______/| $$__  $$ /$$____/ | $$__  $$|______/
         | $$  \ $$| $$      | $$  | $$        
         | $$$$$$$/| $$$$$$$$| $$  | $$        
         |_______/ |________/|__/  |__/        
 
   https://github.com/yaronzz/BaiduYunToAliYun 
 '''
-VERSION = '2023.07.14.1'
+VERSION = '2023.07.04.1'
 
 aliplat = AliPlat()
 bdyplat = BdyPlat()
 config = B2aConfig()
 trans = Trans(aliplat, bdyplat, config.path)
```

### Comparing `b2a-2023.7.14.1/b2a/aliplat.py` & `b2a-2023.7.4.1/b2a/aliplat.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,51 +106,41 @@
 
     def list(self, remotePath: str, nextMarker: str = None) -> List[FileAttr]:
         remotePath = remotePath.rstrip('/')
         sid = self.__getPathId__(remotePath)
         if not sid:
             return []
 
-        retry = 3
-        while True:
-            try:
-                retry -= 1
-                requests_data = {"drive_id": self.driveId, "parent_file_id": sid, 'marker': nextMarker, 'limit': 100}
-                requests_post = requests.post('https://api.aliyundrive.com/adrive/v3/file/list',
-                                            data=json.dumps(requests_data),
-                                            headers=self.headers,
-                                            verify=False).json()
-                if 'items' not in requests_post:
-                    if retry > 0:
-                        time.sleep(1)
-                        continue
-                    printErr("获取目录文件列表失败：" + requests_post['code'])
-                    return []
-                
-                ret = []
-                for item in requests_post['items']:
-                    obj = FileAttr()
-                    obj.isfile = item['type'] != 'folder'
-                    obj.name = item['name']
-                    obj.path = remotePath + '/' + item['name']
-                    obj.uid = item['file_id']
-                    obj.size = item['size'] if 'size' in item else 0
-                    if not obj.isfile:
-                        self.__updatePathId__(obj.path, obj.uid)
-
-                    ret.append(obj)
-
-                next_marker = requests_post.get('next_marker')
-                if next_marker and nextMarker != requests_post['next_marker']:
-                    ret.extend(self.list(remotePath, next_marker))
-
-                return ret
-            except Exception as e:
-                printErr("获取目录文件列表失败：" + str(e))
-                return []
+        try:
+            requests_data = {"drive_id": self.driveId, "parent_file_id": sid, 'marker': nextMarker, 'limit': 100}
+            requests_post = requests.post('https://api.aliyundrive.com/adrive/v3/file/list',
+                                          data=json.dumps(requests_data),
+                                          headers=self.headers,
+                                          verify=False).json()
+            ret = []
+            for item in requests_post['items']:
+                obj = FileAttr()
+                obj.isfile = item['type'] != 'folder'
+                obj.name = item['name']
+                obj.path = remotePath + '/' + item['name']
+                obj.uid = item['file_id']
+                obj.size = item['size'] if 'size' in item else 0
+                if not obj.isfile:
+                    self.__updatePathId__(obj.path, obj.uid)
+
+                ret.append(obj)
+
+            next_marker = requests_post.get('next_marker')
+            if next_marker and nextMarker != requests_post['next_marker']:
+                ret.extend(self.list(remotePath, next_marker))
+
+            return ret
+        except Exception as e:
+            printErr("获取目录文件列表失败：" + str(e))
+            return []
 
     def __mkdir__(self, folderName, parentFolderId='root') -> (bool, str):
         folderName = folderName.strip('/')
         try:
             requests_data = {
                 "drive_id": self.driveId,
                 "parent_file_id": parentFolderId,
```

### Comparing `b2a-2023.7.14.1/b2a/bdyplat.py` & `b2a-2023.7.4.1/b2a/bdyplat.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a/common.py` & `b2a-2023.7.4.1/b2a/common.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a/config.py` & `b2a-2023.7.4.1/b2a/config.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a/downloader.py` & `b2a-2023.7.4.1/b2a/downloader.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a/platformImp.py` & `b2a-2023.7.4.1/b2a/platformImp.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a/trans.py` & `b2a-2023.7.4.1/b2a/trans.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a_gui/__init__.py` & `b2a-2023.7.4.1/b2a_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a_gui/download.py` & `b2a-2023.7.4.1/b2a_gui/download.py`

 * *Files identical despite different names*

### Comparing `b2a-2023.7.14.1/b2a_gui/main.py` & `b2a-2023.7.4.1/b2a_gui/main.py`

 * *Files identical despite different names*

