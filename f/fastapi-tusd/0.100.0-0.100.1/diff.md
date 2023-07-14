# Comparing `tmp/fastapi-tusd-0.100.0.tar.gz` & `tmp/fastapi-tusd-0.100.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/fastapi-tusd/fastapi-tusd/dist/.tmp-ii5lsn6e/fastapi-tusd-0.100.0.tar", last modified: Thu Jul 13 03:51:04 2023, max compression
+gzip compressed data, was "/home/runner/work/fastapi-tusd/fastapi-tusd/dist/.tmp-xh6n_k3e/fastapi-tusd-0.100.1.tar", last modified: Fri Jul 14 07:35:45 2023, max compression
```

## Comparing `fastapi-tusd-0.100.0.tar` & `fastapi-tusd-0.100.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/examples/app_tusd.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-13 03:50:53.000000 fastapi-tusd-0.100.0/src/fastapi_tusd/tusd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 03:51:04.000000 fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/examples/app_tusd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-14 07:35:32.000000 fastapi-tusd-0.100.1/src/fastapi_tusd/tusd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:35:44.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 07:35:45.000000 fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/top_level.txt
```

### Comparing `fastapi-tusd-0.100.0/.github/workflows/publish.yml` & `fastapi-tusd-0.100.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.0/.gitignore` & `fastapi-tusd-0.100.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.0/LICENSE` & `fastapi-tusd-0.100.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.0/PKG-INFO` & `fastapi-tusd-0.100.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tusd
-Version: 0.100.0
+Version: 0.100.1
 Summary: FastAPI extention implementing the tus server
 Home-page: https://github.com/liviaerxin/fastapi_tusd
 Author: Frank
 Author-email: 1yue8haogaoqi@gmail.com
 License: MIT license
 Keywords: fastapi_tusd
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -38,15 +38,15 @@
 
 ```py title=main.py
 from fastapi import FastAPI
 from fastapi_tusd import TusRouter
 
 app = FastAPI()
 
-app.include_router(TusRouter(store_dir="./files", prefix="/files"))
+app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/files")
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
 ### Examples
 
 There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
```

### Comparing `fastapi-tusd-0.100.0/README.md` & `fastapi-tusd-0.100.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```py title=main.py
 from fastapi import FastAPI
 from fastapi_tusd import TusRouter
 
 app = FastAPI()
 
-app.include_router(TusRouter(store_dir="./files", prefix="/files"))
+app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/files")
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
 ### Examples
 
 There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
```

### Comparing `fastapi-tusd-0.100.0/examples/app_tusd.py` & `fastapi-tusd-0.100.1/examples/app_tusd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi import FastAPI
 from fastapi.responses import HTMLResponse, JSONResponse, Response
 from fastapi_tusd import TusRouter
 
 app = FastAPI()
 
-app.include_router(TusRouter(store_dir="./files"))
+app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/files")
 
 # fmt: off
 html_content = """
 <!doctype html>
 <html>
 <head>
     <meta charset="utf-8">
@@ -32,14 +32,16 @@
     })
 </script>
 </body>
 </html>
 """
 # fmt: on
 
+
 @app.get("/")
 async def home():
     return {"message": "Hello World"}
 
+
 @app.get("/upload.html")
 async def read_uppy():
-    return HTMLResponse(html_content)
+    return HTMLResponse(html_content)
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 from fastapi import FastAPI from fastapi.responses import HTMLResponse,
 JSONResponse, Response from fastapi_tusd import TusRouter app = FastAPI()
-app.include_router(TusRouter(store_dir="./files")) # fmt: off html_content =
-"""
+app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/
+files") # fmt: off html_content = """
 """ # fmt: on @app.get("/") async def home(): return {"message": "Hello World"}
 @app.get("/upload.html") async def read_uppy(): return HTMLResponse
 (html_content)
```

### Comparing `fastapi-tusd-0.100.0/setup.cfg` & `fastapi-tusd-0.100.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.0/src/fastapi_tusd/filestore.py` & `fastapi-tusd-0.100.1/src/fastapi_tusd/filestore.py`

 * *Files identical despite different names*

### Comparing `fastapi-tusd-0.100.0/src/fastapi_tusd/tusd.py` & `fastapi-tusd-0.100.1/src/fastapi_tusd/tusd.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     )
     tus_checksum_algorithm = "md5,sha1,crc32"
 
     def __init__(
         self,
         store_dir: str,
         max_size: int = 128849018880,
-        prefix: str = "/files",
+        location: str = "http://127.0.0.1:8000/files",
         *args,
         **kwargs,
     ):
-        super().__init__(prefix=prefix, *args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         self.store_dir = store_dir
         self.max_size = max_size
         # TODO: support s3
         self.datastore = FileStore(path=store_dir)
 
-        self.location = self.prefix
+        self.location = location
 
         self.add_core_routes()
 
     def add_core_routes(self):
         @self.options("")
         # read information about server configuration
         async def read_server_config(request: Request, response: Response) -> Response:
```

### Comparing `fastapi-tusd-0.100.0/src/fastapi_tusd.egg-info/PKG-INFO` & `fastapi-tusd-0.100.1/src/fastapi_tusd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-tusd
-Version: 0.100.0
+Version: 0.100.1
 Summary: FastAPI extention implementing the tus server
 Home-page: https://github.com/liviaerxin/fastapi_tusd
 Author: Frank
 Author-email: 1yue8haogaoqi@gmail.com
 License: MIT license
 Keywords: fastapi_tusd
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -38,15 +38,15 @@
 
 ```py title=main.py
 from fastapi import FastAPI
 from fastapi_tusd import TusRouter
 
 app = FastAPI()
 
-app.include_router(TusRouter(store_dir="./files", prefix="/files"))
+app.include_router(TusRouter(store_dir="./files", location="/files"), prefix="/files")
 ```
 
 Then the tus upload endpoints will be served at `http://127.0.0.1:8000/files`, more information is available at `http://127.0.0.1:8000/docs`
 
 ### Examples
 
 There a simple example with web file upload client supporting for `Tus` protocol, thanks to `Uppy`!
```

