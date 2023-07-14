# Comparing `tmp/1secMail-0.5.0.tar.gz` & `tmp/1secMail-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1secMail-0.5.0.tar", last modified: Thu Jul 13 15:44:44 2023, max compression
+gzip compressed data, was "1secMail-1.0.0.tar", last modified: Fri Jul 14 15:17:55 2023, max compression
```

## Comparing `1secMail-0.5.0.tar` & `1secMail-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:44:44.739541 1secMail-0.5.0/
-drwxrwxrwx   0        0        0        0 2023-07-13 15:44:44.732876 1secMail-0.5.0/1secMail.egg-info/
--rw-rw-rw-   0        0        0     3151 2023-07-13 15:44:44.000000 1secMail-0.5.0/1secMail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-13 15:44:44.000000 1secMail-0.5.0/1secMail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:44:44.000000 1secMail-0.5.0/1secMail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-13 15:44:44.000000 1secMail-0.5.0/1secMail.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 15:44:44.000000 1secMail-0.5.0/1secMail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2023-07-13 09:01:53.000000 1secMail-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     3151 2023-07-13 15:44:44.738473 1secMail-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2309 2023-07-13 15:33:38.000000 1secMail-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 15:44:44.737453 1secMail-0.5.0/secmail/
--rw-rw-rw-   0        0        0      123 2023-07-13 15:44:12.000000 1secMail-0.5.0/secmail/__init__.py
--rw-rw-rw-   0        0        0     6702 2023-07-13 15:33:10.000000 1secMail-0.5.0/secmail/client.py
--rw-rw-rw-   0        0        0      443 2023-07-13 15:33:44.000000 1secMail-0.5.0/secmail/config.py
--rw-rw-rw-   0        0        0     3388 2023-07-13 14:14:41.000000 1secMail-0.5.0/secmail/models.py
--rw-rw-rw-   0        0        0       42 2023-07-13 15:44:44.739541 1secMail-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1397 2023-07-13 15:42:15.000000 1secMail-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:17:55.564603 1secMail-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:17:55.558721 1secMail-1.0.0/1secMail.egg-info/
+-rw-rw-rw-   0        0        0     4060 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 15:17:55.000000 1secMail-1.0.0/1secMail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2023-07-13 09:01:53.000000 1secMail-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4060 2023-07-14 15:17:55.563241 1secMail-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3197 2023-07-14 03:57:35.000000 1secMail-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:17:55.563241 1secMail-1.0.0/secmail/
+-rw-rw-rw-   0        0        0      123 2023-07-13 15:44:12.000000 1secMail-1.0.0/secmail/__init__.py
+-rw-rw-rw-   0        0        0    12071 2023-07-14 15:17:50.000000 1secMail-1.0.0/secmail/client.py
+-rw-rw-rw-   0        0        0      443 2023-07-14 15:09:27.000000 1secMail-1.0.0/secmail/config.py
+-rw-rw-rw-   0        0        0     3384 2023-07-14 03:38:35.000000 1secMail-1.0.0/secmail/models.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:17:55.564603 1secMail-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1473 2023-07-14 15:17:52.000000 1secMail-1.0.0/setup.py
```

### Comparing `1secMail-0.5.0/1secMail.egg-info/PKG-INFO` & `1secMail-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: 1secMail
-Version: 0.5.0
-Summary: Create and receive email in only 1 second! 📧 An API wrapper for www.1secmail.com written in Python.
-Home-page: https://github.com/qvco/1secMail-Python
-Download-URL: https://github.com/qvco/1secMail-Python
-Author: qvco
-Author-email: nikola.desuga@gmail.com
-Maintainer: qvco
-Maintainer-email: nikola.desuga@gmail.com
-License: MIT
-Keywords: 1secmail,onesecmail,tempmail,email,api,wrapper,library
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <br>
   <img src="https://github.com/qvco/1secMail-Python/assets/77382767/fde69c1a-b95f-4d78-af1a-2dca315204bc" alt="1secMail" width="700">
 <!--   <br>
   1secMail for Python
   <br> -->
 </p>
@@ -33,76 +12,103 @@
     <img src="https://img.shields.io/github/release/qvco/1secMail-Python">
     <img src="https://img.shields.io/badge/python-3.8-blue.svg">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg">
   </p>
 
 ### About
 
-This is a simple Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily generate temporary email addresses as much as you want and retrieve emails sent to those addresses.
+This is an easy to use yet full-featured Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily create temporary email addresses for testing, verification, or other purposes where you need a disposable email address.
 
 ### Install
 
-To install this package, you'll need Python 3.8 or above installed on your computer. From your command line:
+To install the package, you'll need Python 3.8 or above installed on your computer. From your command line:
 
 ```bash
 pip install 1secMail
 ```
 
 <br>
 
 > **Note**
 > If you're willing to install the development version, do the following:
 
 ```bash
-git clone https://github.com/qvco/1secMail-Python
+git clone https://github.com/qvco/1secMail-Python.git
 
 cd 1secMail-Python
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
-### How To Use
+## Usage
+
+### Generating Email Addresses
+
+To generate a list of random email addresses, use the `random_email()` method:
 
 ```python
 import secmail
 
 client = secmail.Client()
 
-client.random_email(amount=1)[0]
->>> 'vsd2bq6zo3@1secmail.net'
+client.random_email(amount=3)
+>>> ['c3fho3cry1@1secmail.net', '5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net']
+```
+
+You can also generate a custom email address by specifying the username and domain:
 
+> **Note**
+> Specifying a domain is optional!
+
+```python
 client.custom_email(username="bobby-bob", domain="kzccv.com")
 >>> 'bobby-bob@kzccv.com'
+```
+
+### Receiving Messages
 
+To wait until a new message is received, use the `await_new_message()` method:
 
-# Checking your mailbox:
-messages = client.get_messages("bobby-bob@kzccv.com")
+```python
+message = client.await_new_message(address)
+```
+
+To check all messages received on a particular email address, use the `get_inbox()` method and pass the email address:
+
+```python
+messages = client.get_inbox("bobby-bob@kzccv.com")
 for message in messages:
     print(message.id)
     print(message.from_address)
     print(message.subject)
     print(message.date)
+```
 
+You can also fetch a single message using the `get_message()` method and passing the email address and message ID:
 
-# Fetching single message:
+```python
 message = client.get_message(address="bobby-bob@kzccv.com", message_id=235200687)
 print(message.id)
 print(message.subject)
 print(message.body)
 print(message.text_body)
 print(message.html_body)
 print(message.attachments)
 print(message.date)
+```
 
+### Attachment Information
 
-# Checking attachment informations
+To check attachment information, loop through the attachments in the message object and print the filename, content type, and size:
+
+```python
 for attachment in message.attachments:
     print(attachment.filename)
     print(attachment.content_type)
     print(attachment.size)
 ```
 
-### Licnese
+## Licnese
 
 This software is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) © [Qvco](https://github.com/qvco).
```

#### html2text {}

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 2.1 Name: 1secMail Version: 0.5.0 Summary: Create and receive
-email in only 1 second! ð§ An API wrapper for www.1secmail.com written in
-Python. Home-page: https://github.com/qvco/1secMail-Python Download-URL: https:
-//github.com/qvco/1secMail-Python Author: qvco Author-email:
-nikola.desuga@gmail.com Maintainer: qvco Maintainer-email:
-nikola.desuga@gmail.com License: MIT Keywords:
-1secmail,onesecmail,tempmail,email,api,wrapper,library Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown License-File: LICENSE
 
                                   [1secMail]
         *** An API wrapper for www.1secmail.com written in Python. ***
     [https://img.shields.io/github/release/qvco/1secMail-Python] [https://
    img.shields.io/badge/python-3.8-blue.svg] [https://img.shields.io/badge/
                              License-MIT-blue.svg]
-### About This is a simple Python API wrapper for www.1secmail.com â using
-the official 1secMail API. It allows you to easily generate temporary email
-addresses as much as you want and retrieve emails sent to those addresses. ###
-Install To install this package, you'll need Python 3.8 or above installed on
-your computer. From your command line: ```bash pip install 1secMail ```
+### About This is an easy to use yet full-featured Python API wrapper for
+www.1secmail.com â using the official 1secMail API. It allows you to easily
+create temporary email addresses for testing, verification, or other purposes
+where you need a disposable email address. ### Install To install the package,
+you'll need Python 3.8 or above installed on your computer. From your command
+line: ```bash pip install 1secMail ```
 > **Note** > If you're willing to install the development version, do the
-following: ```bash git clone https://github.com/qvco/1secMail-Python cd
-1secMail-Python pip install -r requirements.txt pip install -e . ``` ### How To
-Use ```python import secmail client = secmail.Client() client.random_email
-(amount=1)[0] >>> 'vsd2bq6zo3@1secmail.net' client.custom_email
-(username="bobby-bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' # Checking
-your mailbox: messages = client.get_messages("bobby-bob@kzccv.com") for message
-in messages: print(message.id) print(message.from_address) print
-(message.subject) print(message.date) # Fetching single message: message =
-client.get_message(address="bobby-bob@kzccv.com", message_id=235200687) print
-(message.id) print(message.subject) print(message.body) print
-(message.text_body) print(message.html_body) print(message.attachments) print
-(message.date) # Checking attachment informations for attachment in
-message.attachments: print(attachment.filename) print(attachment.content_type)
-print(attachment.size) ``` ### Licnese This software is licensed under the
-[MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) Â© [Qvco]
-(https://github.com/qvco).
+following: ```bash git clone https://github.com/qvco/1secMail-Python.git cd
+1secMail-Python pip install -r requirements.txt pip install -e . ``` ## Usage
+### Generating Email Addresses To generate a list of random email addresses,
+use the `random_email()` method: ```python import secmail client =
+secmail.Client() client.random_email(amount=3) >>> ['c3fho3cry1@1secmail.net',
+'5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net'] ``` You can also generate
+a custom email address by specifying the username and domain: > **Note** >
+Specifying a domain is optional! ```python client.custom_email(username="bobby-
+bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' ``` ### Receiving Messages
+To wait until a new message is received, use the `await_new_message()` method:
+```python message = client.await_new_message(address) ``` To check all messages
+received on a particular email address, use the `get_inbox()` method and pass
+the email address: ```python messages = client.get_inbox("bobby-bob@kzccv.com")
+for message in messages: print(message.id) print(message.from_address) print
+(message.subject) print(message.date) ``` You can also fetch a single message
+using the `get_message()` method and passing the email address and message ID:
+```python message = client.get_message(address="bobby-bob@kzccv.com",
+message_id=235200687) print(message.id) print(message.subject) print
+(message.body) print(message.text_body) print(message.html_body) print
+(message.attachments) print(message.date) ``` ### Attachment Information To
+check attachment information, loop through the attachments in the message
+object and print the filename, content type, and size: ```python for attachment
+in message.attachments: print(attachment.filename) print
+(attachment.content_type) print(attachment.size) ``` ## Licnese This software
+is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/
+master/LICENSE) Â© [Qvco](https://github.com/qvco).
```

### Comparing `1secMail-0.5.0/LICENSE` & `1secMail-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `1secMail-0.5.0/PKG-INFO` & `1secMail-1.0.0/1secMail.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: 1secMail
-Version: 0.5.0
+Version: 1.0.0
 Summary: Create and receive email in only 1 second! 📧 An API wrapper for www.1secmail.com written in Python.
 Home-page: https://github.com/qvco/1secMail-Python
 Download-URL: https://github.com/qvco/1secMail-Python
 Author: qvco
 Author-email: nikola.desuga@gmail.com
 Maintainer: qvco
 Maintainer-email: nikola.desuga@gmail.com
 License: MIT
-Keywords: 1secmail,onesecmail,tempmail,email,api,wrapper,library
+Keywords: 1secmail,onesecmail,tempmail,disposable,temporary,email,api,wrapper,library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -33,76 +33,103 @@
     <img src="https://img.shields.io/github/release/qvco/1secMail-Python">
     <img src="https://img.shields.io/badge/python-3.8-blue.svg">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg">
   </p>
 
 ### About
 
-This is a simple Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily generate temporary email addresses as much as you want and retrieve emails sent to those addresses.
+This is an easy to use yet full-featured Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily create temporary email addresses for testing, verification, or other purposes where you need a disposable email address.
 
 ### Install
 
-To install this package, you'll need Python 3.8 or above installed on your computer. From your command line:
+To install the package, you'll need Python 3.8 or above installed on your computer. From your command line:
 
 ```bash
 pip install 1secMail
 ```
 
 <br>
 
 > **Note**
 > If you're willing to install the development version, do the following:
 
 ```bash
-git clone https://github.com/qvco/1secMail-Python
+git clone https://github.com/qvco/1secMail-Python.git
 
 cd 1secMail-Python
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
-### How To Use
+## Usage
+
+### Generating Email Addresses
+
+To generate a list of random email addresses, use the `random_email()` method:
 
 ```python
 import secmail
 
 client = secmail.Client()
 
-client.random_email(amount=1)[0]
->>> 'vsd2bq6zo3@1secmail.net'
+client.random_email(amount=3)
+>>> ['c3fho3cry1@1secmail.net', '5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net']
+```
+
+You can also generate a custom email address by specifying the username and domain:
+
+> **Note**
+> Specifying a domain is optional!
 
+```python
 client.custom_email(username="bobby-bob", domain="kzccv.com")
 >>> 'bobby-bob@kzccv.com'
+```
 
+### Receiving Messages
 
-# Checking your mailbox:
-messages = client.get_messages("bobby-bob@kzccv.com")
+To wait until a new message is received, use the `await_new_message()` method:
+
+```python
+message = client.await_new_message(address)
+```
+
+To check all messages received on a particular email address, use the `get_inbox()` method and pass the email address:
+
+```python
+messages = client.get_inbox("bobby-bob@kzccv.com")
 for message in messages:
     print(message.id)
     print(message.from_address)
     print(message.subject)
     print(message.date)
+```
 
+You can also fetch a single message using the `get_message()` method and passing the email address and message ID:
 
-# Fetching single message:
+```python
 message = client.get_message(address="bobby-bob@kzccv.com", message_id=235200687)
 print(message.id)
 print(message.subject)
 print(message.body)
 print(message.text_body)
 print(message.html_body)
 print(message.attachments)
 print(message.date)
+```
 
+### Attachment Information
 
-# Checking attachment informations
+To check attachment information, loop through the attachments in the message object and print the filename, content type, and size:
+
+```python
 for attachment in message.attachments:
     print(attachment.filename)
     print(attachment.content_type)
     print(attachment.size)
 ```
 
-### Licnese
+## Licnese
 
 This software is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) © [Qvco](https://github.com/qvco).
```

#### html2text {}

```diff
@@ -1,40 +1,51 @@
-Metadata-Version: 2.1 Name: 1secMail Version: 0.5.0 Summary: Create and receive
+Metadata-Version: 2.1 Name: 1secMail Version: 1.0.0 Summary: Create and receive
 email in only 1 second! ð§ An API wrapper for www.1secmail.com written in
 Python. Home-page: https://github.com/qvco/1secMail-Python Download-URL: https:
 //github.com/qvco/1secMail-Python Author: qvco Author-email:
 nikola.desuga@gmail.com Maintainer: qvco Maintainer-email:
 nikola.desuga@gmail.com License: MIT Keywords:
-1secmail,onesecmail,tempmail,email,api,wrapper,library Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown License-File: LICENSE
+1secmail,onesecmail,tempmail,disposable,temporary,email,api,wrapper,library
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
 
                                   [1secMail]
         *** An API wrapper for www.1secmail.com written in Python. ***
     [https://img.shields.io/github/release/qvco/1secMail-Python] [https://
    img.shields.io/badge/python-3.8-blue.svg] [https://img.shields.io/badge/
                              License-MIT-blue.svg]
-### About This is a simple Python API wrapper for www.1secmail.com â using
-the official 1secMail API. It allows you to easily generate temporary email
-addresses as much as you want and retrieve emails sent to those addresses. ###
-Install To install this package, you'll need Python 3.8 or above installed on
-your computer. From your command line: ```bash pip install 1secMail ```
+### About This is an easy to use yet full-featured Python API wrapper for
+www.1secmail.com â using the official 1secMail API. It allows you to easily
+create temporary email addresses for testing, verification, or other purposes
+where you need a disposable email address. ### Install To install the package,
+you'll need Python 3.8 or above installed on your computer. From your command
+line: ```bash pip install 1secMail ```
 > **Note** > If you're willing to install the development version, do the
-following: ```bash git clone https://github.com/qvco/1secMail-Python cd
-1secMail-Python pip install -r requirements.txt pip install -e . ``` ### How To
-Use ```python import secmail client = secmail.Client() client.random_email
-(amount=1)[0] >>> 'vsd2bq6zo3@1secmail.net' client.custom_email
-(username="bobby-bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' # Checking
-your mailbox: messages = client.get_messages("bobby-bob@kzccv.com") for message
-in messages: print(message.id) print(message.from_address) print
-(message.subject) print(message.date) # Fetching single message: message =
-client.get_message(address="bobby-bob@kzccv.com", message_id=235200687) print
-(message.id) print(message.subject) print(message.body) print
-(message.text_body) print(message.html_body) print(message.attachments) print
-(message.date) # Checking attachment informations for attachment in
-message.attachments: print(attachment.filename) print(attachment.content_type)
-print(attachment.size) ``` ### Licnese This software is licensed under the
-[MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) Â© [Qvco]
-(https://github.com/qvco).
+following: ```bash git clone https://github.com/qvco/1secMail-Python.git cd
+1secMail-Python pip install -r requirements.txt pip install -e . ``` ## Usage
+### Generating Email Addresses To generate a list of random email addresses,
+use the `random_email()` method: ```python import secmail client =
+secmail.Client() client.random_email(amount=3) >>> ['c3fho3cry1@1secmail.net',
+'5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net'] ``` You can also generate
+a custom email address by specifying the username and domain: > **Note** >
+Specifying a domain is optional! ```python client.custom_email(username="bobby-
+bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' ``` ### Receiving Messages
+To wait until a new message is received, use the `await_new_message()` method:
+```python message = client.await_new_message(address) ``` To check all messages
+received on a particular email address, use the `get_inbox()` method and pass
+the email address: ```python messages = client.get_inbox("bobby-bob@kzccv.com")
+for message in messages: print(message.id) print(message.from_address) print
+(message.subject) print(message.date) ``` You can also fetch a single message
+using the `get_message()` method and passing the email address and message ID:
+```python message = client.get_message(address="bobby-bob@kzccv.com",
+message_id=235200687) print(message.id) print(message.subject) print
+(message.body) print(message.text_body) print(message.html_body) print
+(message.attachments) print(message.date) ``` ### Attachment Information To
+check attachment information, loop through the attachments in the message
+object and print the filename, content type, and size: ```python for attachment
+in message.attachments: print(attachment.filename) print
+(attachment.content_type) print(attachment.size) ``` ## Licnese This software
+is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/
+master/LICENSE) Â© [Qvco](https://github.com/qvco).
```

### Comparing `1secMail-0.5.0/README.md` & `1secMail-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: 1secMail
+Version: 1.0.0
+Summary: Create and receive email in only 1 second! 📧 An API wrapper for www.1secmail.com written in Python.
+Home-page: https://github.com/qvco/1secMail-Python
+Download-URL: https://github.com/qvco/1secMail-Python
+Author: qvco
+Author-email: nikola.desuga@gmail.com
+Maintainer: qvco
+Maintainer-email: nikola.desuga@gmail.com
+License: MIT
+Keywords: 1secmail,onesecmail,tempmail,disposable,temporary,email,api,wrapper,library
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <br>
   <img src="https://github.com/qvco/1secMail-Python/assets/77382767/fde69c1a-b95f-4d78-af1a-2dca315204bc" alt="1secMail" width="700">
 <!--   <br>
   1secMail for Python
   <br> -->
 </p>
@@ -12,76 +33,103 @@
     <img src="https://img.shields.io/github/release/qvco/1secMail-Python">
     <img src="https://img.shields.io/badge/python-3.8-blue.svg">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg">
   </p>
 
 ### About
 
-This is a simple Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily generate temporary email addresses as much as you want and retrieve emails sent to those addresses.
+This is an easy to use yet full-featured Python API wrapper for www.1secmail.com ↗ using the official 1secMail API. It allows you to easily create temporary email addresses for testing, verification, or other purposes where you need a disposable email address.
 
 ### Install
 
-To install this package, you'll need Python 3.8 or above installed on your computer. From your command line:
+To install the package, you'll need Python 3.8 or above installed on your computer. From your command line:
 
 ```bash
 pip install 1secMail
 ```
 
 <br>
 
 > **Note**
 > If you're willing to install the development version, do the following:
 
 ```bash
-git clone https://github.com/qvco/1secMail-Python
+git clone https://github.com/qvco/1secMail-Python.git
 
 cd 1secMail-Python
 
 pip install -r requirements.txt
 
 pip install -e .
 ```
 
-### How To Use
+## Usage
+
+### Generating Email Addresses
+
+To generate a list of random email addresses, use the `random_email()` method:
 
 ```python
 import secmail
 
 client = secmail.Client()
 
-client.random_email(amount=1)[0]
->>> 'vsd2bq6zo3@1secmail.net'
+client.random_email(amount=3)
+>>> ['c3fho3cry1@1secmail.net', '5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net']
+```
+
+You can also generate a custom email address by specifying the username and domain:
 
+> **Note**
+> Specifying a domain is optional!
+
+```python
 client.custom_email(username="bobby-bob", domain="kzccv.com")
 >>> 'bobby-bob@kzccv.com'
+```
+
+### Receiving Messages
 
+To wait until a new message is received, use the `await_new_message()` method:
 
-# Checking your mailbox:
-messages = client.get_messages("bobby-bob@kzccv.com")
+```python
+message = client.await_new_message(address)
+```
+
+To check all messages received on a particular email address, use the `get_inbox()` method and pass the email address:
+
+```python
+messages = client.get_inbox("bobby-bob@kzccv.com")
 for message in messages:
     print(message.id)
     print(message.from_address)
     print(message.subject)
     print(message.date)
+```
 
+You can also fetch a single message using the `get_message()` method and passing the email address and message ID:
 
-# Fetching single message:
+```python
 message = client.get_message(address="bobby-bob@kzccv.com", message_id=235200687)
 print(message.id)
 print(message.subject)
 print(message.body)
 print(message.text_body)
 print(message.html_body)
 print(message.attachments)
 print(message.date)
+```
 
+### Attachment Information
 
-# Checking attachment informations
+To check attachment information, loop through the attachments in the message object and print the filename, content type, and size:
+
+```python
 for attachment in message.attachments:
     print(attachment.filename)
     print(attachment.content_type)
     print(attachment.size)
 ```
 
-### Licnese
+## Licnese
 
 This software is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) © [Qvco](https://github.com/qvco).
```

#### html2text {}

```diff
@@ -1,28 +1,51 @@
+Metadata-Version: 2.1 Name: 1secMail Version: 1.0.0 Summary: Create and receive
+email in only 1 second! ð§ An API wrapper for www.1secmail.com written in
+Python. Home-page: https://github.com/qvco/1secMail-Python Download-URL: https:
+//github.com/qvco/1secMail-Python Author: qvco Author-email:
+nikola.desuga@gmail.com Maintainer: qvco Maintainer-email:
+nikola.desuga@gmail.com License: MIT Keywords:
+1secmail,onesecmail,tempmail,disposable,temporary,email,api,wrapper,library
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE
 
                                   [1secMail]
         *** An API wrapper for www.1secmail.com written in Python. ***
     [https://img.shields.io/github/release/qvco/1secMail-Python] [https://
    img.shields.io/badge/python-3.8-blue.svg] [https://img.shields.io/badge/
                              License-MIT-blue.svg]
-### About This is a simple Python API wrapper for www.1secmail.com â using
-the official 1secMail API. It allows you to easily generate temporary email
-addresses as much as you want and retrieve emails sent to those addresses. ###
-Install To install this package, you'll need Python 3.8 or above installed on
-your computer. From your command line: ```bash pip install 1secMail ```
+### About This is an easy to use yet full-featured Python API wrapper for
+www.1secmail.com â using the official 1secMail API. It allows you to easily
+create temporary email addresses for testing, verification, or other purposes
+where you need a disposable email address. ### Install To install the package,
+you'll need Python 3.8 or above installed on your computer. From your command
+line: ```bash pip install 1secMail ```
 > **Note** > If you're willing to install the development version, do the
-following: ```bash git clone https://github.com/qvco/1secMail-Python cd
-1secMail-Python pip install -r requirements.txt pip install -e . ``` ### How To
-Use ```python import secmail client = secmail.Client() client.random_email
-(amount=1)[0] >>> 'vsd2bq6zo3@1secmail.net' client.custom_email
-(username="bobby-bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' # Checking
-your mailbox: messages = client.get_messages("bobby-bob@kzccv.com") for message
-in messages: print(message.id) print(message.from_address) print
-(message.subject) print(message.date) # Fetching single message: message =
-client.get_message(address="bobby-bob@kzccv.com", message_id=235200687) print
-(message.id) print(message.subject) print(message.body) print
-(message.text_body) print(message.html_body) print(message.attachments) print
-(message.date) # Checking attachment informations for attachment in
-message.attachments: print(attachment.filename) print(attachment.content_type)
-print(attachment.size) ``` ### Licnese This software is licensed under the
-[MIT](https://github.com/qvco/1secMail-Python/blob/master/LICENSE) Â© [Qvco]
-(https://github.com/qvco).
+following: ```bash git clone https://github.com/qvco/1secMail-Python.git cd
+1secMail-Python pip install -r requirements.txt pip install -e . ``` ## Usage
+### Generating Email Addresses To generate a list of random email addresses,
+use the `random_email()` method: ```python import secmail client =
+secmail.Client() client.random_email(amount=3) >>> ['c3fho3cry1@1secmail.net',
+'5qcd3d36zr@1secmail.org', 'b6fgeothtg@1secmail.net'] ``` You can also generate
+a custom email address by specifying the username and domain: > **Note** >
+Specifying a domain is optional! ```python client.custom_email(username="bobby-
+bob", domain="kzccv.com") >>> 'bobby-bob@kzccv.com' ``` ### Receiving Messages
+To wait until a new message is received, use the `await_new_message()` method:
+```python message = client.await_new_message(address) ``` To check all messages
+received on a particular email address, use the `get_inbox()` method and pass
+the email address: ```python messages = client.get_inbox("bobby-bob@kzccv.com")
+for message in messages: print(message.id) print(message.from_address) print
+(message.subject) print(message.date) ``` You can also fetch a single message
+using the `get_message()` method and passing the email address and message ID:
+```python message = client.get_message(address="bobby-bob@kzccv.com",
+message_id=235200687) print(message.id) print(message.subject) print
+(message.body) print(message.text_body) print(message.html_body) print
+(message.attachments) print(message.date) ``` ### Attachment Information To
+check attachment information, loop through the attachments in the message
+object and print the filename, content type, and size: ```python for attachment
+in message.attachments: print(attachment.filename) print
+(attachment.content_type) print(attachment.size) ``` ## Licnese This software
+is licensed under the [MIT](https://github.com/qvco/1secMail-Python/blob/
+master/LICENSE) Â© [Qvco](https://github.com/qvco).
```

### Comparing `1secMail-0.5.0/secmail/models.py` & `1secMail-1.0.0/secmail/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-class MailBox:
-    """The mailbox object contains an array of email objects, each with an unique ID,\n
+class Inbox:
+    """The inbox object contains an array of email objects, each with an unique ID,\n
     sender's email address, subject line, and date and time the email was sent.
 
     ---
 
     Attributes:
     ----------
```

### Comparing `1secMail-0.5.0/setup.py` & `1secMail-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 author = "qvco"
 author_email = "nikola.desuga@gmail.com"
 description = "Create and receive email in only 1 second! 📧 An API wrapper for www.1secmail.com written in Python."
 long_description_content_type = "text/markdown"
 license = "MIT"
 url = "https://github.com/qvco/1secMail-Python"
 
-keywords = ["1secmail", "onesecmail", "tempmail", "email", "api", "wrapper", "library"]
+keywords = [
+    "1secmail",
+    "onesecmail",
+    "tempmail",
+    "disposable",
+    "temporary",
+    "email",
+    "api",
+    "wrapper",
+    "library",
+]
 
 install_requires = ["httpx>=0.17.1"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

