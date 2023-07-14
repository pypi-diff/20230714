# Comparing `tmp/whatsapp-api-client-python-0.0.39.tar.gz` & `tmp/whatsapp-api-client-python-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-client-python-0.0.39.tar", last modified: Wed Jul  5 15:42:59 2023, max compression
+gzip compressed data, was "whatsapp-api-client-python-0.0.40.tar", last modified: Fri Jul 14 05:06:05 2023, max compression
```

## Comparing `whatsapp-api-client-python-0.0.39.tar` & `whatsapp-api-client-python-0.0.40.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.751853 whatsapp-api-client-python-0.0.39/
--rw-rw-rw-   0        0        0    18132 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/LICENSE
--rw-rw-rw-   0        0        0    21777 2023-07-05 15:42:59.750849 whatsapp-api-client-python-0.0.39/PKG-INFO
--rw-rw-rw-   0        0        0    20328 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 15:42:59.751853 whatsapp-api-client-python-0.0.39/setup.cfg
--rw-rw-rw-   0        0        0     1802 2023-07-05 15:41:59.000000 whatsapp-api-client-python-0.0.39/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.735968 whatsapp-api-client-python-0.0.39/tests/
--rw-rw-rw-   0        0        0     4261 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/tests/test_methods.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.737973 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/
--rw-rw-rw-   0        0        0     2211 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/API.py
--rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/__init__.py
--rw-rw-rw-   0        0        0      363 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/response.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.749847 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/
--rw-rw-rw-   0        0        0        0 2023-07-01 06:40:11.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-07-01 10:03:15.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/account.py
--rw-rw-rw-   0        0        0      595 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/device.py
--rw-rw-rw-   0        0        0     4518 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/groups.py
--rw-rw-rw-   0        0        0     2134 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/journals.py
--rw-rw-rw-   0        0        0      763 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/marking.py
--rw-rw-rw-   0        0        0      928 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/queues.py
--rw-rw-rw-   0        0        0     1437 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/receiving.py
--rw-rw-rw-   0        0        0     8004 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/sending.py
--rw-rw-rw-   0        0        0     3599 2023-07-03 08:40:42.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/serviceMethods.py
--rw-rw-rw-   0        0        0     2676 2023-07-05 15:29:45.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/webhooks.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:42:59.741829 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/
--rw-rw-rw-   0        0        0    21777 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      902 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-05 15:42:59.000000 whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 05:06:05.959317 whatsapp-api-client-python-0.0.40/
+-rw-rw-rw-   0        0        0    18132 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/LICENSE
+-rw-rw-rw-   0        0        0    22054 2023-07-14 05:06:05.959317 whatsapp-api-client-python-0.0.40/PKG-INFO
+-rw-rw-rw-   0        0        0    20605 2023-07-13 12:59:59.000000 whatsapp-api-client-python-0.0.40/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:06:05.959317 whatsapp-api-client-python-0.0.40/setup.cfg
+-rw-rw-rw-   0        0        0     1802 2023-07-14 04:54:15.000000 whatsapp-api-client-python-0.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:06:05.937337 whatsapp-api-client-python-0.0.40/tests/
+-rw-rw-rw-   0        0        0     4261 2023-07-13 12:45:57.000000 whatsapp-api-client-python-0.0.40/tests/test_methods.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:06:05.940266 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/
+-rw-rw-rw-   0        0        0     2211 2023-07-13 12:13:31.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/API.py
+-rw-rw-rw-   0        0        0        0 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/__init__.py
+-rw-rw-rw-   0        0        0      363 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/response.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:06:05.958314 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/account.py
+-rw-rw-rw-   0        0        0      595 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/device.py
+-rw-rw-rw-   0        0        0     4518 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/groups.py
+-rw-rw-rw-   0        0        0     2134 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/journals.py
+-rw-rw-rw-   0        0        0      763 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/marking.py
+-rw-rw-rw-   0        0        0      928 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/queues.py
+-rw-rw-rw-   0        0        0     1437 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/receiving.py
+-rw-rw-rw-   0        0        0     8462 2023-07-13 12:59:59.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/sending.py
+-rw-rw-rw-   0        0        0     3599 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/serviceMethods.py
+-rw-rw-rw-   0        0        0     2676 2023-07-09 08:30:04.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/webhooks.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:06:05.946282 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/
+-rw-rw-rw-   0        0        0    22054 2023-07-14 05:06:05.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      902 2023-07-14 05:06:05.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:06:05.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 05:06:05.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-14 05:06:05.000000 whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-client-python-0.0.39/LICENSE` & `whatsapp-api-client-python-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/PKG-INFO` & `whatsapp-api-client-python-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.39
+Version: 0.0.40
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -213,14 +213,15 @@
 | `receiving.downloadFile`               | The method is for downloading received and sent files                                                                    | [DownloadFile](https://green-api.com/en/docs/api/receiving/files/DownloadFile/)                             |
 | `sending.sendMessage`                  | The method is designed to send a text message to a personal or group chat                                                | [SendMessage](https://green-api.com/en/docs/api/sending/SendMessage/)                                       |
 | `sending.sendButtons`                  | The method is designed to send a message with buttons to a personal or group chat                                        | [SendButtons](https://green-api.com/en/docs/api/sending/SendButtons/)                                       |
 | `sending.sendTemplateButtons`          | The method is designed to send a message with interactive buttons from the list of templates in a personal or group chat | [SendTemplateButtons](https://green-api.com/en/docs/api/sending/SendTemplateButtons/)                       |
 | `sending.sendListMessage`              | The method is designed to send a message with a selection button from a list of values to a personal or group chat       | [SendListMessage](https://green-api.com/en/docs/api/sending/SendListMessage/)                               |
 | `sending.sendFileByUpload`             | The method is designed to send a file loaded through a form (form-data)                                                  | [SendFileByUpload](https://green-api.com/en/docs/api/sending/SendFileByUpload/)                             |
 | `sending.sendFileByUrl`                | The method is designed to send a file downloaded via a link                                                              | [SendFileByUrl](https://green-api.com/en/docs/api/sending/SendFileByUrl/)                                   |
+| `sending.uploadFile`                   | The method is designed to upload a file to the cloud storage, which can be sent using the sendFileByUrl method           | [UploadFile](https://green-api.com/en/docs/api/sending/UploadFile/)                                         |
 | `sending.sendLocation`                 | The method is designed to send a geolocation message                                                                     | [SendLocation](https://green-api.com/en/docs/api/sending/SendLocation/)                                     |
 | `sending.sendContact`                  | The method is for sending a message with a contact                                                                       | [SendContact](https://green-api.com/en/docs/api/sending/SendContact/)                                       |
 | `sending.sendLink`                     | The method is designed to send a message with a link that will add an image preview, title and description               | [SendLink](https://green-api.com/en/docs/api/sending/SendLink/)                                             |
 | `sending.forwardMessages`              | The method is designed for forwarding messages to a personal or group chat                                               | [ForwardMessages](https://green-api.com/en/docs/api/sending/ForwardMessages/)                               |
 | `serviceMethods.checkWhatsapp`         | The method checks if there is a WhatsApp account on the phone number                                                     | [CheckWhatsapp](https://green-api.com/en/docs/api/service/CheckWhatsapp/)                                   |
 | `serviceMethods.getAvatar`             | The method returns the avatar of the correspondent or group chat                                                         | [GetAvatar](https://green-api.com/en/docs/api/service/GetAvatar/)                                           |
 | `serviceMethods.getContacts`           | The method is designed to get a list of contacts of the current account                                                  | [GetContacts](https://green-api.com/en/docs/api/service/GetContacts/)                                       |
```

### Comparing `whatsapp-api-client-python-0.0.39/README.md` & `whatsapp-api-client-python-0.0.40/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 | `receiving.downloadFile`               | The method is for downloading received and sent files                                                                    | [DownloadFile](https://green-api.com/en/docs/api/receiving/files/DownloadFile/)                             |
 | `sending.sendMessage`                  | The method is designed to send a text message to a personal or group chat                                                | [SendMessage](https://green-api.com/en/docs/api/sending/SendMessage/)                                       |
 | `sending.sendButtons`                  | The method is designed to send a message with buttons to a personal or group chat                                        | [SendButtons](https://green-api.com/en/docs/api/sending/SendButtons/)                                       |
 | `sending.sendTemplateButtons`          | The method is designed to send a message with interactive buttons from the list of templates in a personal or group chat | [SendTemplateButtons](https://green-api.com/en/docs/api/sending/SendTemplateButtons/)                       |
 | `sending.sendListMessage`              | The method is designed to send a message with a selection button from a list of values to a personal or group chat       | [SendListMessage](https://green-api.com/en/docs/api/sending/SendListMessage/)                               |
 | `sending.sendFileByUpload`             | The method is designed to send a file loaded through a form (form-data)                                                  | [SendFileByUpload](https://green-api.com/en/docs/api/sending/SendFileByUpload/)                             |
 | `sending.sendFileByUrl`                | The method is designed to send a file downloaded via a link                                                              | [SendFileByUrl](https://green-api.com/en/docs/api/sending/SendFileByUrl/)                                   |
+| `sending.uploadFile`                   | The method is designed to upload a file to the cloud storage, which can be sent using the sendFileByUrl method           | [UploadFile](https://green-api.com/en/docs/api/sending/UploadFile/)                                         |
 | `sending.sendLocation`                 | The method is designed to send a geolocation message                                                                     | [SendLocation](https://green-api.com/en/docs/api/sending/SendLocation/)                                     |
 | `sending.sendContact`                  | The method is for sending a message with a contact                                                                       | [SendContact](https://green-api.com/en/docs/api/sending/SendContact/)                                       |
 | `sending.sendLink`                     | The method is designed to send a message with a link that will add an image preview, title and description               | [SendLink](https://green-api.com/en/docs/api/sending/SendLink/)                                             |
 | `sending.forwardMessages`              | The method is designed for forwarding messages to a personal or group chat                                               | [ForwardMessages](https://green-api.com/en/docs/api/sending/ForwardMessages/)                               |
 | `serviceMethods.checkWhatsapp`         | The method checks if there is a WhatsApp account on the phone number                                                     | [CheckWhatsapp](https://green-api.com/en/docs/api/service/CheckWhatsapp/)                                   |
 | `serviceMethods.getAvatar`             | The method returns the avatar of the correspondent or group chat                                                         | [GetAvatar](https://green-api.com/en/docs/api/service/GetAvatar/)                                           |
 | `serviceMethods.getContacts`           | The method is designed to get a list of contacts of the current account                                                  | [GetContacts](https://green-api.com/en/docs/api/service/GetContacts/)                                       |
```

### Comparing `whatsapp-api-client-python-0.0.39/setup.py` & `whatsapp-api-client-python-0.0.40/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-api-client-python",
-    version="0.0.39",
+    version="0.0.40",
     description=(
         "This library helps you easily create"
         " a Python application with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-api-client-python-0.0.39/tests/test_methods.py` & `whatsapp-api-client-python-0.0.40/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/API.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/API.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/account.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/account.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/device.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/device.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/groups.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/groups.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/journals.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/journals.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/marking.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/marking.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/queues.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/queues.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/receiving.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/receiving.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/sending.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/sending.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import mimetypes
 import pathlib
 from typing import Dict, List, Optional, TYPE_CHECKING, Union
 
+from requests import Session
+
 from ..response import Response
 
 if TYPE_CHECKING:
     from ..API import GreenApi
 
 
 class Sending:
@@ -159,22 +161,29 @@
         The method is designed to upload a file to the cloud storage,
         which can be sent using the sendFileByUrl method.
         """
 
         file_name = pathlib.Path(path).name
         content_type = mimetypes.guess_type(file_name)[0]
 
-        files = {"file": (file_name, open(path, "rb"), content_type)}
-
-        return self.api.request(
-            "POST", (
-                "{{media}}/waInstance{{idInstance}}/"
-                "uploadFile/{{apiTokenInstance}}"
-            ), files=files
-        )
+        try:
+            with open(path, "rb") as file:
+                with Session() as session:
+                    response = session.request(
+                        method="POST",
+                        url=(
+                            f"{self.api.media}/waInstance{self.api.idInstance}/"
+                            f"uploadFile/{self.api.apiTokenInstance}"
+                        ),
+                        data=file.read(),
+                        headers={"Content-Type": content_type}
+                    )
+        except Exception as error:
+            return Response(None, f"Other error occurred: {error}.")
+        return Response(response.status_code, response.text)
 
     def sendLocation(
             self,
             chatId: str,
             latitude: float,
             longitude: float,
             nameLocation: Optional[str] = None,
```

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/serviceMethods.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/serviceMethods.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python/tools/webhooks.py` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python/tools/webhooks.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/PKG-INFO` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-client-python
-Version: 0.0.39
+Version: 0.0.40
 Summary: This library helps you easily create a Python application with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-api-client-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -213,14 +213,15 @@
 | `receiving.downloadFile`               | The method is for downloading received and sent files                                                                    | [DownloadFile](https://green-api.com/en/docs/api/receiving/files/DownloadFile/)                             |
 | `sending.sendMessage`                  | The method is designed to send a text message to a personal or group chat                                                | [SendMessage](https://green-api.com/en/docs/api/sending/SendMessage/)                                       |
 | `sending.sendButtons`                  | The method is designed to send a message with buttons to a personal or group chat                                        | [SendButtons](https://green-api.com/en/docs/api/sending/SendButtons/)                                       |
 | `sending.sendTemplateButtons`          | The method is designed to send a message with interactive buttons from the list of templates in a personal or group chat | [SendTemplateButtons](https://green-api.com/en/docs/api/sending/SendTemplateButtons/)                       |
 | `sending.sendListMessage`              | The method is designed to send a message with a selection button from a list of values to a personal or group chat       | [SendListMessage](https://green-api.com/en/docs/api/sending/SendListMessage/)                               |
 | `sending.sendFileByUpload`             | The method is designed to send a file loaded through a form (form-data)                                                  | [SendFileByUpload](https://green-api.com/en/docs/api/sending/SendFileByUpload/)                             |
 | `sending.sendFileByUrl`                | The method is designed to send a file downloaded via a link                                                              | [SendFileByUrl](https://green-api.com/en/docs/api/sending/SendFileByUrl/)                                   |
+| `sending.uploadFile`                   | The method is designed to upload a file to the cloud storage, which can be sent using the sendFileByUrl method           | [UploadFile](https://green-api.com/en/docs/api/sending/UploadFile/)                                         |
 | `sending.sendLocation`                 | The method is designed to send a geolocation message                                                                     | [SendLocation](https://green-api.com/en/docs/api/sending/SendLocation/)                                     |
 | `sending.sendContact`                  | The method is for sending a message with a contact                                                                       | [SendContact](https://green-api.com/en/docs/api/sending/SendContact/)                                       |
 | `sending.sendLink`                     | The method is designed to send a message with a link that will add an image preview, title and description               | [SendLink](https://green-api.com/en/docs/api/sending/SendLink/)                                             |
 | `sending.forwardMessages`              | The method is designed for forwarding messages to a personal or group chat                                               | [ForwardMessages](https://green-api.com/en/docs/api/sending/ForwardMessages/)                               |
 | `serviceMethods.checkWhatsapp`         | The method checks if there is a WhatsApp account on the phone number                                                     | [CheckWhatsapp](https://green-api.com/en/docs/api/service/CheckWhatsapp/)                                   |
 | `serviceMethods.getAvatar`             | The method returns the avatar of the correspondent or group chat                                                         | [GetAvatar](https://green-api.com/en/docs/api/service/GetAvatar/)                                           |
 | `serviceMethods.getContacts`           | The method is designed to get a list of contacts of the current account                                                  | [GetContacts](https://green-api.com/en/docs/api/service/GetContacts/)                                       |
```

### Comparing `whatsapp-api-client-python-0.0.39/whatsapp_api_client_python.egg-info/SOURCES.txt` & `whatsapp-api-client-python-0.0.40/whatsapp_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

