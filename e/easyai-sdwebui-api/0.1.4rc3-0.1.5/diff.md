# Comparing `tmp/easyai-sdwebui-api-0.1.4rc3.tar.gz` & `tmp/easyai_sdwebui_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyai-sdwebui-api-0.1.4rc3.tar", last modified: Tue Jun  6 15:55:30 2023, max compression
+gzip compressed data, was "easyai_sdwebui_api-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easyai-sdwebui-api-0.1.4rc3.tar` & `easyai_sdwebui_api-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai-sdwebui-api-0.1.4rc3/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai-sdwebui-api-0.1.4rc3/.coveragerc
--rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai-sdwebui-api-0.1.4rc3/.editorconfig
--rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai-sdwebui-api-0.1.4rc3/.gitignore
--rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai-sdwebui-api-0.1.4rc3/.isort.cfg
--rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai-sdwebui-api-0.1.4rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai-sdwebui-api-0.1.4rc3/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai-sdwebui-api-0.1.4rc3/LICENSE
--rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai-sdwebui-api-0.1.4rc3/Makefile
--rw-r--r--   0        0        0    11590 2023-06-06 15:54:26.166287 easyai-sdwebui-api-0.1.4rc3/README.md
--rw-r--r--   0        0        0      546 2023-06-06 15:55:06.324823 easyai-sdwebui-api-0.1.4rc3/easyai/__init__.py
--rw-r--r--   0        0        0     9915 2023-06-06 15:54:26.178327 easyai-sdwebui-api-0.1.4rc3/easyai/base.py
--rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai-sdwebui-api-0.1.4rc3/easyai/controlnet.py
--rw-r--r--   0        0        0      735 2023-06-06 02:58:53.947830 easyai-sdwebui-api-0.1.4rc3/easyai/image.py
--rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai-sdwebui-api-0.1.4rc3/easyai/interfaces.py
--rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai-sdwebui-api-0.1.4rc3/easyai/main.py
--rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai-sdwebui-api-0.1.4rc3/easyai/result.py
--rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai-sdwebui-api-0.1.4rc3/easyai/upscaler.py
--rw-r--r--   0        0        0     3706 2023-06-05 09:52:38.517957 easyai-sdwebui-api-0.1.4rc3/easyai_demo.ipynb
--rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai-sdwebui-api-0.1.4rc3/pyproject.toml
--rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai-sdwebui-api-0.1.4rc3/setup.cfg
--rw-r--r--   0        0        0    13540 1970-01-01 00:00:00.000000 easyai-sdwebui-api-0.1.4rc3/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-06-05 08:39:39.849380 easyai_sdwebui_api-0.1.5/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2023-06-05 08:39:39.850791 easyai_sdwebui_api-0.1.5/.coveragerc
+-rw-r--r--   0        0        0      386 2023-06-05 08:39:39.852457 easyai_sdwebui_api-0.1.5/.editorconfig
+-rw-r--r--   0        0        0     6362 2023-06-05 08:39:39.855218 easyai_sdwebui_api-0.1.5/.gitignore
+-rw-r--r--   0        0        0       53 2023-06-05 08:39:39.856225 easyai_sdwebui_api-0.1.5/.isort.cfg
+-rw-r--r--   0        0        0      907 2023-06-05 08:39:39.857342 easyai_sdwebui_api-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-06-05 08:39:39.858679 easyai_sdwebui_api-0.1.5/.pylintrc
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easyai_sdwebui_api-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1285 2023-06-05 08:39:39.860297 easyai_sdwebui_api-0.1.5/Makefile
+-rw-r--r--   0        0        0    11601 2023-07-14 06:27:18.520911 easyai_sdwebui_api-0.1.5/README.md
+-rw-r--r--   0        0        0      543 2023-07-14 07:20:50.975129 easyai_sdwebui_api-0.1.5/easyai/__init__.py
+-rw-r--r--   0        0        0     9909 2023-07-14 07:18:43.740673 easyai_sdwebui_api-0.1.5/easyai/base.py
+-rw-r--r--   0        0        0     2230 2023-06-05 08:39:39.867964 easyai_sdwebui_api-0.1.5/easyai/controlnet.py
+-rw-r--r--   0        0        0      735 2023-06-29 07:59:21.580853 easyai_sdwebui_api-0.1.5/easyai/image.py
+-rw-r--r--   0        0        0     8999 2023-06-05 08:39:39.871238 easyai_sdwebui_api-0.1.5/easyai/interfaces.py
+-rw-r--r--   0        0        0    11987 2023-06-06 02:53:32.725162 easyai_sdwebui_api-0.1.5/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-06-05 08:39:39.875095 easyai_sdwebui_api-0.1.5/easyai/result.py
+-rw-r--r--   0        0        0      822 2023-06-05 08:39:39.876281 easyai_sdwebui_api-0.1.5/easyai/upscaler.py
+-rw-r--r--   0        0        0     3710 2023-06-06 16:10:46.710175 easyai_sdwebui_api-0.1.5/easyai_demo.ipynb
+-rw-r--r--   0        0        0     1671 2023-06-06 02:53:31.609585 easyai_sdwebui_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2288 2023-06-05 08:39:39.880238 easyai_sdwebui_api-0.1.5/setup.cfg
+-rw-r--r--   0        0        0    13548 1970-01-01 00:00:00.000000 easyai_sdwebui_api-0.1.5/PKG-INFO
```

### Comparing `easyai-sdwebui-api-0.1.4rc3/.gitignore` & `easyai_sdwebui_api-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/.pre-commit-config.yaml` & `easyai_sdwebui_api-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/LICENSE` & `easyai_sdwebui_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/Makefile` & `easyai_sdwebui_api-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/README.md` & `easyai_sdwebui_api-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # easyai-sdwebui-api
 API client for AUTOMATIC1111/stable-diffusion-webui
 
-Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.1 and Mikubill/sd-webui-controlnet v1.1.189
+Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.x/v1.4.x and Mikubill/sd-webui-controlnet v1.1.232
 
 * Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
 
 * API support have to be enabled from webui. Add --api when running webui.
 It's explained [here](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/API).
 
 * You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 * API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easy-webui-api
+pip install easyai-sdwebui-api
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
```

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/__init__.py` & `easyai_sdwebui_api-0.1.5/easyai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     ControlNetInterface,
     InstructPix2PixInterface,
     ModelKeywordInterface,
 )
 from .main import EasyAI, EasyAPI, easyai
 from .upscaler import HiResUpscaler, Upscaler
 
-__version__ = "0.1.4rc3"
+__version__ = "0.1.5"
 
 __all__ = [
     "easyai",
     "EasyAI",
     "EasyAPI",
     "ModelKeywordInterface",
     "InstructPix2PixInterface",
```

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/base.py` & `easyai_sdwebui_api-0.1.5/easyai/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,23 +95,23 @@
         parameters = ""
         if "parameters" in json_result.keys():
             parameters = json_result["parameters"]
 
         return APIResult(images, parameters, info)
 
     def _to_api_result(self, response):
-        if response.status_code != 200:
-            raise RuntimeError(response.status_code, response.text)
+        if response.status != 200:
+            raise RuntimeError(response.status, response.text())
 
         r = response.json()
         return self._extract_result(r)
 
     async def _to_api_result_async(self, response):
         if response.status != 200:
-            raise RuntimeError(response.status, await response.text)
+            raise RuntimeError(response.status, await response.text())
 
         r = await response.json()
         return self._extract_result(r)
 
     # XXX 500 error (2022/12/26)
     def png_info(self, image):
         payload = {
```

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/controlnet.py` & `easyai_sdwebui_api-0.1.5/easyai/controlnet.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/image.py` & `easyai_sdwebui_api-0.1.5/easyai/image.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/interfaces.py` & `easyai_sdwebui_api-0.1.5/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/main.py` & `easyai_sdwebui_api-0.1.5/easyai/main.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai/upscaler.py` & `easyai_sdwebui_api-0.1.5/easyai/upscaler.py`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/easyai_demo.ipynb` & `easyai_sdwebui_api-0.1.5/easyai_demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999834656084656%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '!pip install easyai-sdwebui-api\\n')], delete: [0]}}}"}*

```diff
@@ -18,15 +18,15 @@
                 "pycharm": {
                     "is_executing": true
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "!pip install easy-webui-api\n",
+                "!pip install easyai-sdwebui-api\n",
                 "import easyai\n",
                 "\n",
                 "# create API client\n",
                 "\n",
                 "# create API client with custom host, port and https, default sampler, steps.\n",
                 "api = easyai.EasyAPI(host='127.0.0.1', port=443, use_https=False, sampler='Euler a', steps=20)\n",
                 "\n",
```

### Comparing `easyai-sdwebui-api-0.1.4rc3/pyproject.toml` & `easyai_sdwebui_api-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/setup.cfg` & `easyai_sdwebui_api-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyai-sdwebui-api-0.1.4rc3/PKG-INFO` & `easyai_sdwebui_api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyai-sdwebui-api
-Version: 0.1.4rc3
+Version: 0.1.5
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -43,30 +43,30 @@
 Project-URL: Documentation, https://github.com/freemindcore/sdwebuiapi
 Provides-Extra: dev
 Provides-Extra: test
 
 # easyai-sdwebui-api
 API client for AUTOMATIC1111/stable-diffusion-webui
 
-Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.1 and Mikubill/sd-webui-controlnet v1.1.189
+Tested on AUTOMATIC1111/stable-diffusion-webui v1.2.x/v1.4.x and Mikubill/sd-webui-controlnet v1.1.232
 
 * Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
 
 * API support have to be enabled from webui. Add --api when running webui.
 It's explained [here](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/API).
 
 * You can use --api-auth user1:pass1,user2:pass2 option to enable authentication for api access.
 (Since it's basic http authentication the password is transmitted in cleartext)
 
 * API calls are (almost) direct translation from http://127.0.0.1:7860/docs as of 2022/11/21.
 
 # Install
 
 ```
-pip install easy-webui-api
+pip install easyai-sdwebui-api
 ```
 
 # Usage
 
 easyai_demo.ipynb contains example code with original images. Images are compressed as jpeg in this document.
 
 ## create API client
```

