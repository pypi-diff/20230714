# Comparing `tmp/dingtalk-stream-0.7.0.tar.gz` & `tmp/dingtalk-stream-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.7.0.tar", last modified: Wed Jul 12 01:21:54 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.7.1.tar", last modified: Fri Jul 14 03:09:07 2023, max compression
```

## Comparing `dingtalk-stream-0.7.0.tar` & `dingtalk-stream-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23572 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:09:07.319051 dingtalk-stream-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-14 03:09:07.319051 dingtalk-stream-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:09:07.319051 dingtalk-stream-0.7.1/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:09:07.319051 dingtalk-stream-0.7.1/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-14 03:09:07.000000 dingtalk-stream-0.7.1/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-14 03:09:07.000000 dingtalk-stream-0.7.1/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:09:07.000000 dingtalk-stream-0.7.1/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 03:09:07.000000 dingtalk-stream-0.7.1/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 03:09:07.000000 dingtalk-stream-0.7.1/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:09:07.319051 dingtalk-stream-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-14 03:09:06.000000 dingtalk-stream-0.7.1/setup.py
```

### Comparing `dingtalk-stream-0.7.0/LICENSE` & `dingtalk-stream-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.0/PKG-INFO` & `dingtalk-stream-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.0/README.md` & `dingtalk-stream-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.7.1/dingtalk_stream/card_instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         :param title:
         :param logo:
         :param at_sender:
         :param at_all:
         :return:
         """
         self.card_instance_id = self.create_and_send_card(self.card_template_id, self._get_card_data(markdown),
-                                                          at_sender, at_all)
+                                                          at_sender=at_sender, at_all=at_all)
 
     def update(self, markdown: str):
         """
         更新markdown内容，如果你reply了多次，这里只会更新最后一张卡片
         :param markdown:
         :return:
         """
@@ -186,7 +186,86 @@
         if self.title is not None and self.title != "":
             card_data["msgTitle"] = self.title
 
         if self.logo is not None and self.logo != "":
             card_data["logo"] = self.logo
 
         self.fail(self.card_instance_id, card_data)
+
+
+class CarouselCardInstance(AICardReplier):
+    """
+    轮播图卡片
+    """
+
+    def __init__(self, dingtalk_client, incoming_message):
+        super(CarouselCardInstance, self).__init__(dingtalk_client, incoming_message)
+        self.card_template_id = "382e4302-551d-4880-bf29-a30acfab2e71.schema"
+        self.card_instance_id = None
+        self.title = None
+        self.logo = None
+
+    def set_title_and_logo(self, title: str, logo: str):
+        self.title = title
+        self.logo = logo
+
+    def ai_start(self):
+        """
+        开始执行中
+        :return:
+        """
+        self.card_instance_id = self.start(self.card_template_id, {})
+
+    def reply(self, markdown: str, image_slider_list: list, button_text: str = "submit"):
+        """
+        回复卡片
+        :param button_text:
+        :param image_slider_list:
+        :param markdown:
+        :return:
+        """
+
+        sys_full_json_obj = {
+            "order": [
+                "msgTitle",
+                "msgMarkdown",
+                "msgSlider",
+                "msgImages",
+                "msgTextList",
+                "msgButtons",
+            ],
+            "msgSlider": [],
+            "msgButtons": [
+                {
+                    "text": button_text,
+                    "color": "blue",
+                    "id": "image_slider_select_button",
+                    "request": True
+                }
+            ]
+        }
+
+        if button_text is not None and button_text!="":
+            sys_full_json_obj["msgButtons"][0]["text"] = button_text
+
+        for image_slider in image_slider_list:
+            sys_full_json_obj["msgSlider"].append({
+                "title": image_slider[0],
+                "image": image_slider[1]
+            })
+
+        card_data = {
+            "msgMarkdown": markdown,
+            "sys_full_json_obj": json.dumps(sys_full_json_obj)
+        }
+
+        if self.title is not None and self.title != "":
+            card_data["msgTitle"] = self.title
+
+        if self.logo is not None and self.logo != "":
+            card_data["logo"] = self.logo
+
+        self.card_instance_id = self.create_and_send_card(self.card_template_id,
+                                                          {"flowStatus": AICardStatus.PROCESSING},
+                                                          callback_type="STREAM")
+
+        self.finish(self.card_instance_id, card_data)
```

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.7.1/dingtalk_stream/card_replier.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
             'Accept': '*/*',
             'x-acs-dingtalk-access-token': access_token,
             'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
                            '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
                            ) % platform.python_version(),
         }
 
-    def create_and_send_card(self, card_template_id: str, card_data: dict, at_sender: bool = False,
+    def create_and_send_card(self, card_template_id: str, card_data: dict, callback_type: str = "",
+                             callback_route_key: str = "", at_sender: bool = False,
                              at_all: bool = False) -> str:
         """
         发送卡片，两步骤：创建+投放。
         https://open.dingtalk.com/document/orgapp/interface-for-creating-a-card-instance
         :param card_template_id: 卡片模板ID
         :param card_data: 卡片数据
         :param at_sender:
@@ -64,14 +65,20 @@
                 "supportForward": False
             },
             "imRobotOpenSpaceModel": {
                 "supportForward": False
             }
         }
 
+        if callback_type == "STREAM":
+            body["callbackType"] = "STREAM"
+        elif callback_type == "HTTP":
+            body["callbackType"] = "HTTP"
+            body["callbackRouteKey"] = callback_route_key
+
         # 创建卡片实例。https://open.dingtalk.com/document/orgapp/interface-for-creating-a-card-instance
         url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/card/instances'
         try:
             response = requests.post(url,
                                      headers=self.get_request_header(access_token),
                                      json=body)
 
@@ -175,15 +182,15 @@
         AI卡片的创建接口
         :param card_template_id:
         :param card_data:
         :return:
         """
         card_data_with_status = copy.deepcopy(card_data)
         card_data_with_status["flowStatus"] = AICardStatus.PROCESSING
-        return self.create_and_send_card(card_template_id, card_data_with_status, False, False)
+        return self.create_and_send_card(card_template_id, card_data_with_status, at_sender=False, at_all=False)
 
     def finish(self, card_instance_id: str, card_data: dict):
         """
         AI卡片执行完成的接口，整体更新
         :param card_instance_id:
         :param card_data:
         :return:
```

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.7.1/dingtalk_stream/chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import hashlib
 from .stream import CallbackHandler, CallbackMessage
 from .frames import AckMessage, Headers
 from .interactive_card import generate_multi_text_line_card_data
 from .utils import DINGTALK_OPENAPI_ENDPOINT
 from concurrent.futures import ThreadPoolExecutor
 import uuid
-from .card_instance import MarkdownCardInstance, AIMarkdownCardInstance
+from .card_instance import MarkdownCardInstance, AIMarkdownCardInstance, CarouselCardInstance
 import traceback
 
 
 class AtUser(object):
     def __init__(self):
         self.dingtalk_id = None
         self.staff_id = None
@@ -288,14 +288,34 @@
         markdown_card_instance = MarkdownCardInstance(self.dingtalk_client, incoming_message)
         markdown_card_instance.set_title_and_logo(title, logo)
 
         markdown_card_instance.reply(markdown, at_sender, at_all)
 
         return markdown_card_instance
 
+    def reply_carousel_card(self, incoming_message: ChatbotMessage, markdown: str, image_slider, button_text,
+                            title: str = "",
+                            logo: str = "") -> CarouselCardInstance:
+        """
+        回复一个轮播图卡片
+        :param markdown:
+        :param incoming_message:
+        :param title:
+        :param logo:
+        :param image_slider:
+        :param button_text:
+        :return:
+        """
+        carousel_card_instance = CarouselCardInstance(self.dingtalk_client, incoming_message)
+        carousel_card_instance.set_title_and_logo(title, logo)
+
+        carousel_card_instance.reply(markdown, image_slider, button_text)
+
+        return carousel_card_instance
+
     def ai_markdown_card_start(self, incoming_message: ChatbotMessage, title: str = "",
                                logo: str = "") -> AIMarkdownCardInstance:
         """
         发起一个AI卡片
         :param incoming_message:
         :param title:
         :param logo:
```

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/frames.py` & `dingtalk-stream-0.7.1/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/handlers.py` & `dingtalk-stream-0.7.1/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.7.1/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream/stream.py` & `dingtalk-stream-0.7.1/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.7.1/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.0/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.7.1/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 dingtalk_stream/__init__.py
+dingtalk_stream/card_callback.py
 dingtalk_stream/card_instance.py
 dingtalk_stream/card_replier.py
 dingtalk_stream/chatbot.py
 dingtalk_stream/credential.py
 dingtalk_stream/frames.py
 dingtalk_stream/handlers.py
 dingtalk_stream/interactive_card.py
```

### Comparing `dingtalk-stream-0.7.0/setup.py` & `dingtalk-stream-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.7.0',
+    version='0.7.1',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

