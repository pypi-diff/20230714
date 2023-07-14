# Comparing `tmp/RelayMe-0.0.2.tar.gz` & `tmp/RelayMe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RelayMe-0.0.2.tar", last modified: Fri Jul 14 16:18:58 2023, max compression
+gzip compressed data, was "RelayMe-0.0.4.tar", last modified: Fri Jul 14 16:46:56 2023, max compression
```

## Comparing `RelayMe-0.0.2.tar` & `RelayMe-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:18:58.817290 RelayMe-0.0.2/
--rw-rw-rw-   0        0        0      250 2023-07-14 16:12:25.000000 RelayMe-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-07-13 14:27:01.000000 RelayMe-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-13 14:09:08.000000 RelayMe-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2193 2023-07-14 16:18:58.816293 RelayMe-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-07-14 16:08:09.000000 RelayMe-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 16:18:58.786373 RelayMe-0.0.2/RelayMe/
--rw-rw-rw-   0        0        0     1380 2023-07-14 16:17:24.000000 RelayMe-0.0.2/RelayMe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:18:58.814297 RelayMe-0.0.2/RelayMe.egg-info/
--rw-rw-rw-   0        0        0     2193 2023-07-14 16:18:58.000000 RelayMe-0.0.2/RelayMe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-07-14 16:18:58.000000 RelayMe-0.0.2/RelayMe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:18:58.000000 RelayMe-0.0.2/RelayMe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 16:18:58.000000 RelayMe-0.0.2/RelayMe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 16:18:58.817290 RelayMe-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-07-14 16:08:58.000000 RelayMe-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:46:56.553651 RelayMe-0.0.4/
+-rw-rw-rw-   0        0        0      345 2023-07-14 16:45:21.000000 RelayMe-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-07-13 14:27:01.000000 RelayMe-0.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-13 14:09:08.000000 RelayMe-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2439 2023-07-14 16:46:56.552647 RelayMe-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1550 2023-07-14 16:45:26.000000 RelayMe-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 16:46:56.530704 RelayMe-0.0.4/RelayMe/
+-rw-rw-rw-   0        0        0     1416 2023-07-14 16:38:34.000000 RelayMe-0.0.4/RelayMe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:46:56.550652 RelayMe-0.0.4/RelayMe.egg-info/
+-rw-rw-rw-   0        0        0     2439 2023-07-14 16:46:56.000000 RelayMe-0.0.4/RelayMe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-14 16:46:56.000000 RelayMe-0.0.4/RelayMe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:46:56.000000 RelayMe-0.0.4/RelayMe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 16:46:56.000000 RelayMe-0.0.4/RelayMe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:46:56.553651 RelayMe-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-07-14 16:45:54.000000 RelayMe-0.0.4/setup.py
```

### Comparing `RelayMe-0.0.2/LICENCE.txt` & `RelayMe-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `RelayMe-0.0.2/PKG-INFO` & `RelayMe-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: RelayMe
-Version: 0.0.2
+Version: 0.0.4
 Summary: Sends emails with chosen email relay service
 Home-page: 
 Author: Elijah Phifer
 Author-email: elijahphifer9@gmail.com
 License: MIT
-Keywords: mail,email,relay
+Keywords: mail,email,relay,relayservice
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
 RelayMe
 =======
 
-0.0.2
+0.0.4
 -----
 
 This module is geared towards emailing using email relay services.
 
 Prerequisites
 -------------
 
@@ -38,14 +38,15 @@
 - `server`
 - `port`
 - `sender`
 - `username`
 - `password`
 
 (Case doesn't matter, but spelling is important. The keys could also be named 'Server', 'PORT', 'UserName', etc.)
+(Asleo the 'username' and 'password' keys are optional if your relay service doesn't require a user name and pass word to authenticate.)
 
 Here is an example config key:
 
 .. code-block:: python
 
    'EmailSender': {
        'server': 'smtp.example.com',
@@ -71,14 +72,18 @@
 
    sender.send_email(subject, body, recipient)
 
 
 Change Log
 =============
 
+0.0.4 (07/14/2023)
+-------------------
+-Added more details about usage to the README file
+
 0.0.2 (07/14/2023)
 -------------------
 -Improved code to read config keys regardless of capitalization
 -Changed module name from 'EmailSender' to 'SenderConfig'
 
 0.0.1 (07/13/2023)
 ------------------
```

### Comparing `RelayMe-0.0.2/README.txt` & `RelayMe-0.0.4/README.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 RelayMe
 =======
 
-0.0.2
+0.0.4
 -----
 
 This module is geared towards emailing using email relay services.
 
 Prerequisites
 -------------
 
@@ -22,14 +22,15 @@
 - `server`
 - `port`
 - `sender`
 - `username`
 - `password`
 
 (Case doesn't matter, but spelling is important. The keys could also be named 'Server', 'PORT', 'UserName', etc.)
+(Asleo the 'username' and 'password' keys are optional if your relay service doesn't require a user name and pass word to authenticate.)
 
 Here is an example config key:
 
 .. code-block:: python
 
    'EmailSender': {
        'server': 'smtp.example.com',
```

### Comparing `RelayMe-0.0.2/RelayMe/__init__.py` & `RelayMe-0.0.4/RelayMe/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import smtplib
 from email.message import EmailMessage
 
+# This is code for RelayMe-0.0.3
+
 
 class SenderConfig:
     def __init__(self, config):
         self.config = {key.lower(): value for key, value in config.items()}
         self.logger = logging.getLogger('Sending Email')
         self.logger.setLevel(logging.INFO)
         formatter = logging.Formatter(
```

### Comparing `RelayMe-0.0.2/RelayMe.egg-info/PKG-INFO` & `RelayMe-0.0.4/RelayMe.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: RelayMe
-Version: 0.0.2
+Version: 0.0.4
 Summary: Sends emails with chosen email relay service
 Home-page: 
 Author: Elijah Phifer
 Author-email: elijahphifer9@gmail.com
 License: MIT
-Keywords: mail,email,relay
+Keywords: mail,email,relay,relayservice
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
 RelayMe
 =======
 
-0.0.2
+0.0.4
 -----
 
 This module is geared towards emailing using email relay services.
 
 Prerequisites
 -------------
 
@@ -38,14 +38,15 @@
 - `server`
 - `port`
 - `sender`
 - `username`
 - `password`
 
 (Case doesn't matter, but spelling is important. The keys could also be named 'Server', 'PORT', 'UserName', etc.)
+(Asleo the 'username' and 'password' keys are optional if your relay service doesn't require a user name and pass word to authenticate.)
 
 Here is an example config key:
 
 .. code-block:: python
 
    'EmailSender': {
        'server': 'smtp.example.com',
@@ -71,14 +72,18 @@
 
    sender.send_email(subject, body, recipient)
 
 
 Change Log
 =============
 
+0.0.4 (07/14/2023)
+-------------------
+-Added more details about usage to the README file
+
 0.0.2 (07/14/2023)
 -------------------
 -Improved code to read config keys regardless of capitalization
 -Changed module name from 'EmailSender' to 'SenderConfig'
 
 0.0.1 (07/13/2023)
 ------------------
```

### Comparing `RelayMe-0.0.2/setup.py` & `RelayMe-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='RelayMe',
-    version='0.0.2',
+    version='0.0.4',
     description='Sends emails with chosen email relay service',
     long_description=open('README.txt').read() + '\n\n' +
     open('CHANGELOG.txt').read(),
     url='',
     author='Elijah Phifer',
     author_email='elijahphifer9@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords=['mail', 'email', 'relay'],
+    keywords=['mail', 'email', 'relay', 'relayservice'],
     packages=find_packages(),
     install_requires=['']
 )
```

