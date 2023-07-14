# Comparing `tmp/b2a-2022.7.7.1.tar.gz` & `tmp/b2a-2023.7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2a-2022.7.7.1.tar", last modified: Thu Jul  7 05:43:24 2022, max compression
+gzip compressed data, was "b2a-2023.7.4.1.tar", last modified: Fri Jul 14 03:18:41 2023, max compression
```

## Comparing `b2a-2022.7.7.1.tar` & `b2a-2023.7.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-07-07 05:43:24.757359 b2a-2022.7.7.1/
--rw-rw-rw-   0        0        0      219 2022-07-07 05:43:24.755357 b2a-2022.7.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1912 2022-06-07 03:28:24.000000 b2a-2022.7.7.1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-07 05:43:24.665358 b2a-2022.7.7.1/b2a/
--rw-rw-rw-   0        0        0     8301 2022-07-07 05:41:15.000000 b2a-2022.7.7.1/b2a/__init__.py
--rw-rw-rw-   0        0        0    14049 2022-07-07 05:37:49.000000 b2a-2022.7.7.1/b2a/aliplat.py
--rw-rw-rw-   0        0        0     4938 2022-07-07 05:37:37.000000 b2a-2022.7.7.1/b2a/bdyplat.py
--rw-rw-rw-   0        0        0      740 2021-08-04 01:00:20.000000 b2a-2022.7.7.1/b2a/common.py
--rw-rw-rw-   0        0        0     1126 2021-12-31 03:16:34.000000 b2a-2022.7.7.1/b2a/config.py
--rw-rw-rw-   0        0        0     4089 2022-06-07 05:37:13.000000 b2a-2022.7.7.1/b2a/downloader.py
--rw-rw-rw-   0        0        0     1329 2021-07-30 06:38:18.000000 b2a-2022.7.7.1/b2a/platformImp.py
--rw-rw-rw-   0        0        0     3201 2021-12-31 03:23:01.000000 b2a-2022.7.7.1/b2a/trans.py
-drwxrwxrwx   0        0        0        0 2022-07-07 05:43:24.745362 b2a-2022.7.7.1/b2a.egg-info/
--rw-rw-rw-   0        0        0      219 2022-07-07 05:43:24.000000 b2a-2022.7.7.1/b2a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2022-07-07 05:43:24.000000 b2a-2022.7.7.1/b2a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-07 05:43:24.000000 b2a-2022.7.7.1/b2a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2022-07-07 05:43:24.000000 b2a-2022.7.7.1/b2a.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2022-07-07 05:43:24.000000 b2a-2022.7.7.1/b2a.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-07-07 05:43:24.000000 b2a-2022.7.7.1/b2a.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-07 05:43:24.753355 b2a-2022.7.7.1/b2a_gui/
--rw-rw-rw-   0        0        0     1036 2022-06-07 03:58:14.000000 b2a-2022.7.7.1/b2a_gui/__init__.py
--rw-rw-rw-   0        0        0     3959 2021-07-27 06:28:28.000000 b2a-2022.7.7.1/b2a_gui/download.py
--rw-rw-rw-   0        0        0     2712 2021-07-27 03:01:49.000000 b2a-2022.7.7.1/b2a_gui/main.py
--rw-rw-rw-   0        0        0       42 2022-07-07 05:43:24.757359 b2a-2022.7.7.1/setup.cfg
--rw-rw-rw-   0        0        0      508 2021-09-23 08:50:57.000000 b2a-2022.7.7.1/setup.py
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

### Comparing `b2a-2022.7.7.1/README.md` & `b2a-2023.7.4.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # B2A
 同步百度云网盘到阿里云
 
 ## 📺 安装 
+- pip 安装
 需要 Python 版本大于或等于 3.7
 ```shell
 pip3 install b2a --upgrade
 ```
+- docker 安装
+```
+docker run -itd --name b2a --restart always calmyin/b2a:v2021.12.31.1
+```
 
 ## 🤖 功能
 
 - 登录百度云盘
 - 登录阿里云盘
 - 迁移文件
 - 显示目录
@@ -50,8 +55,8 @@
 - [aliyundrive-uploader](https://github.com/Hidove/aliyundrive-uploader)
 - [aliyunpan](https://github.com/wxy1343/aliyunpan)
 
 ## 📜 免责声明 
 1. 本软件为免费开源项目，无任何形式的盈利行为
 2. 本软件不提供各种破解与加速等功能实现
 3. 本软件仅供个人数据的多端备份使用
-4. 严禁使用本软件进行盈利、损坏官方、散落任何违法信息等行为
+4. 严禁使用本软件进行盈利、损坏官方、散落任何违法信息等行为
```

### Comparing `b2a-2022.7.7.1/b2a/__init__.py` & `b2a-2023.7.4.1/b2a/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 |______/| $$__  $$ /$$____/ | $$__  $$|______/
         | $$  \ $$| $$      | $$  | $$        
         | $$$$$$$/| $$$$$$$$| $$  | $$        
         |_______/ |________/|__/  |__/        
 
   https://github.com/yaronzz/BaiduYunToAliYun 
 '''
-VERSION = '2022.07.07.1'
+VERSION = '2023.07.04.1'
 
 aliplat = AliPlat()
 bdyplat = BdyPlat()
 config = B2aConfig()
 trans = Trans(aliplat, bdyplat, config.path)
```

### Comparing `b2a-2022.7.7.1/b2a/aliplat.py` & `b2a-2023.7.4.1/b2a/aliplat.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         remotePath = remotePath.rstrip('/')
         sid = self.__getPathId__(remotePath)
         if not sid:
             return []
 
         try:
             requests_data = {"drive_id": self.driveId, "parent_file_id": sid, 'marker': nextMarker, 'limit': 100}
-            requests_post = requests.post('https://api.aliyundrive.com/v2/file/list',
+            requests_post = requests.post('https://api.aliyundrive.com/adrive/v3/file/list',
                                           data=json.dumps(requests_data),
                                           headers=self.headers,
                                           verify=False).json()
             ret = []
             for item in requests_post['items']:
                 obj = FileAttr()
                 obj.isfile = item['type'] != 'folder'
```

### Comparing `b2a-2022.7.7.1/b2a/bdyplat.py` & `b2a-2023.7.4.1/b2a/bdyplat.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 @File    :  bdyplat.py
 @Date    :  2021/06/17
 @Author  :  Yaronzz
 @Version :  1.0
 @Contact :  yaronhuang@foxmail.com
 @Desc    :
 """
+import os
+import subprocess
 import aigpy
 from baidupcs_py.baidupcs import BaiduPCSApi
 # from common.io import RangeRequestIO
 from baidupcs_py.common.io import RangeRequestIO
 
 from b2a.common import printErr
 from b2a.downloader import Downloader
@@ -116,29 +118,33 @@
         #             curSize += len(data)
         #             if curSize >= totalSize:
         #                 break
         #
         # stream.close()
         # return True
 
-        headers = {
-            "Cookie ": "; ".join(
-                [f"{k}={v if v is not None else ''}" for k, v in self.key.api.cookies.items()]
-            ),
-            "User-Agent": "netdisk;2.2.51.6;netdisk;10.0.63;PC;android-android",
-            "Connection": "Keep-Alive",
-        }
-
-        link = self.__safeAPI__('download_link', fileAttr.path)
-        if not link or len(link) <= 0:
-            return False
+        # headers = {
+        #     "Cookie ": "; ".join(
+        #         [f"{k}={v if v is not None else ''}" for k, v in self.key.api.cookies.items()]
+        #     ),
+        #     "User-Agent": "netdisk;2.2.51.6;netdisk;10.0.63;PC;android-android",
+        #     "Connection": "Keep-Alive",
+        # }
 
-        dl = Downloader(link, headers, localFilePath, fileAttr.size, 6)
-        check = dl.run()
-        return check
+        # link = self.__safeAPI__('download_link', fileAttr.path)
+        # if not link or len(link) <= 0:
+        #     return False
+        
+        # dl = Downloader(link, headers, localFilePath, fileAttr.size, 1)
+        # check = dl.run()
+        # return check
+        
+        cmd = f'BaiduPCS-Py download -o \"{path}\" \"{fileAttr.path}\"'
+        child = subprocess.run(cmd)
+        return child.returncode == 0
 
     def uploadFile(self, localFilePath: str, remoteFilePath: str) -> bool:
         return False
 
     def downloadLink(self, remoteFilePath: str):
         link = self.__safeAPI__('download_link', remoteFilePath)
         return link
```

### Comparing `b2a-2022.7.7.1/b2a/common.py` & `b2a-2023.7.4.1/b2a/common.py`

 * *Files identical despite different names*

### Comparing `b2a-2022.7.7.1/b2a/config.py` & `b2a-2023.7.4.1/b2a/config.py`

 * *Files identical despite different names*

### Comparing `b2a-2022.7.7.1/b2a/downloader.py` & `b2a-2023.7.4.1/b2a/downloader.py`

 * *Files identical despite different names*

### Comparing `b2a-2022.7.7.1/b2a/platformImp.py` & `b2a-2023.7.4.1/b2a/platformImp.py`

 * *Files identical despite different names*

### Comparing `b2a-2022.7.7.1/b2a/trans.py` & `b2a-2023.7.4.1/b2a/trans.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,24 +52,24 @@
             printInfo(f"[{self.index}] 跳过文件: {item.path}")
             return True
 
         printInfo(f"[{self.index}] 迁移文件: {item.path}")
         localFilePath = self.downloadPath + item.path
         localSize = aigpy.file.getSize(localFilePath)
         if localSize <= 0:
-            tmpFile = localFilePath + ".tmp"
+            tmpFile = localFilePath# + ".tmp"
             check = self._bdyplat.downloadFile(item, tmpFile)
             if not check:
                 aigpy.path.remove(tmpFile)
                 printErr("[错误] 下载失败!")
                 self.errCnt += 1
                 return False
             else:
                 printInfo("下载成功！")
-                os.rename(tmpFile, localFilePath)
+                # os.rename(tmpFile, localFilePath)
 
         check = self._aliplat.uploadFile(localFilePath, uploadFilePath)
         if not check:
             printErr("[错误] 上传失败!")
             self.errCnt += 1
         else:
             self.successCnt += 1
```

### Comparing `b2a-2022.7.7.1/b2a_gui/__init__.py` & `b2a-2023.7.4.1/b2a_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `b2a-2022.7.7.1/b2a_gui/download.py` & `b2a-2023.7.4.1/b2a_gui/download.py`

 * *Files identical despite different names*

### Comparing `b2a-2022.7.7.1/b2a_gui/main.py` & `b2a-2023.7.4.1/b2a_gui/main.py`

 * *Files identical despite different names*

