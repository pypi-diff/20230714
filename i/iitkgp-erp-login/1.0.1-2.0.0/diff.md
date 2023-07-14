# Comparing `tmp/iitkgp_erp_login-1.0.1.tar.gz` & `tmp/iitkgp_erp_login-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-1.0.1.tar", last modified: Mon Jul 10 21:19:19 2023, max compression
+gzip compressed data, was "iitkgp_erp_login-2.0.0.tar", last modified: Fri Jul 14 07:50:47 2023, max compression
```

## Comparing `iitkgp_erp_login-1.0.1.tar` & `iitkgp_erp_login-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.992432 iitkgp_erp_login-1.0.1/
--rw-r--r--   0 proffapt   (501) staff       (20)     1074 2023-07-09 19:05:06.000000 iitkgp_erp_login-1.0.1/LICENSE
--rw-r--r--   0 proffapt   (501) staff       (20)    13061 2023-07-10 21:19:19.992189 iitkgp_erp_login-1.0.1/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)    12503 2023-07-10 21:18:56.000000 iitkgp_erp_login-1.0.1/README.md
--rw-r--r--   0 proffapt   (501) staff       (20)      773 2023-07-10 21:19:15.000000 iitkgp_erp_login-1.0.1/pyproject.toml
--rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-10 21:19:19.992509 iitkgp_erp_login-1.0.1/setup.cfg
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.987967 iitkgp_erp_login-1.0.1/src/
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.990158 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/
--rw-r--r--   0 proffapt   (501) staff       (20)        0 2023-07-09 19:54:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 proffapt   (501) staff       (20)      403 2023-07-09 21:13:18.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 proffapt   (501) staff       (20)     2613 2023-07-09 21:13:45.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 proffapt   (501) staff       (20)     2373 2023-07-09 21:37:06.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/read_mail.py
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.991390 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 proffapt   (501) staff       (20)    13061 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 proffapt   (501) staff       (20)      394 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       92 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 proffapt   (501) staff       (20)       17 2023-07-10 21:19:19.000000 iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/top_level.txt
-drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-10 21:19:19.991578 iitkgp_erp_login-1.0.1/tests/
--rw-r--r--   0 proffapt   (501) staff       (20)      459 2023-07-09 20:54:15.000000 iitkgp_erp_login-1.0.1/tests/test.py
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.980011 iitkgp_erp_login-2.0.0/
+-rw-r--r--   0 proffapt   (501) staff       (20)     1074 2023-07-09 19:05:06.000000 iitkgp_erp_login-2.0.0/LICENSE
+-rw-r--r--   0 proffapt   (501) staff       (20)    13088 2023-07-14 07:50:47.979727 iitkgp_erp_login-2.0.0/PKG-INFO
+-rw-r--r--   0 proffapt   (501) staff       (20)    12530 2023-07-14 07:49:02.000000 iitkgp_erp_login-2.0.0/README.md
+-rw-r--r--   0 proffapt   (501) staff       (20)      773 2023-07-14 07:50:41.000000 iitkgp_erp_login-2.0.0/pyproject.toml
+-rw-r--r--   0 proffapt   (501) staff       (20)       38 2023-07-14 07:50:47.980085 iitkgp_erp_login-2.0.0/setup.cfg
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.975859 iitkgp_erp_login-2.0.0/src/
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.977877 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/
+-rw-r--r--   0 proffapt   (501) staff       (20)        0 2023-07-09 19:54:19.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 proffapt   (501) staff       (20)      403 2023-07-09 21:13:18.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 proffapt   (501) staff       (20)     3561 2023-07-13 22:50:20.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 proffapt   (501) staff       (20)     2373 2023-07-09 21:37:06.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/read_mail.py
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.979014 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 proffapt   (501) staff       (20)    13088 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 proffapt   (501) staff       (20)      394 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)        1 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)       92 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 proffapt   (501) staff       (20)       17 2023-07-14 07:50:47.000000 iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/top_level.txt
+drwxr-xr-x   0 proffapt   (501) staff       (20)        0 2023-07-14 07:50:47.979186 iitkgp_erp_login-2.0.0/tests/
+-rw-r--r--   0 proffapt   (501) staff       (20)      491 2023-07-13 21:24:40.000000 iitkgp_erp_login-2.0.0/tests/test.py
```

### Comparing `iitkgp_erp_login-1.0.1/LICENSE` & `iitkgp_erp_login-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-1.0.1/PKG-INFO` & `iitkgp_erp_login-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,42 @@
-Metadata-Version: 2.1
-Name: iitkgp_erp_login
-Version: 1.0.1
-Summary: A package to automate login process in ERP for IIT-KGP
-Author-email: Arpit Bhardwaj <proffapt@pm.me>
-Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
-Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ERP Login Module
 
 A python package/module to automate login process in ERP for IIT-KGP.
 
 <details>
   <summary>Table of Contents</summary>
    
 - <a href="#description">Description</a>
    - <a href="#endpoints">Endpoints</a>
       - <a href="#endpoints-about">About</a>
       - <a href="#endpoints-usage">Usage</a>
-      - <a href="#usage-in-login-workflow">Usage in login workflow</a>
    - <a href="#login">Login</a>
       - <a href="#login-input">Input</a>
       - <a href="#login-output">Output</a>
       - <a href="#login-usage">Usage</a>
    - <a href="#session-alive">Session status check</a>
       - <a href="#session-alive-input">Input</a>
       - <a href="#session-alive-output">Output</a>
       - <a href="#session-alive-usage">Usage</a>
-- <a href="#package-usage">Usage</a>
-   - <a href="#prerequisites">Prerequisites</a>
-      - <a href="#erpcreds">ERP credentials file</a>
-         - <a href="#erpcreds-creating">Creating</a>
-         - <a href="#erpcreds-using">Using</a>
-      - <a href="#token">Generating token for GMail enabled googleapi</a>
-   - <a href="#example">Example</a>
+- <a href="#example">Example</a>
    
 </details>
 
 <div id="description"></div>
 
 ## Description
 
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
    └── read_mail.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
 The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
@@ -79,75 +58,129 @@
 print(HOMEPAGE_URL)
 # Output: https://erp.iitkgp.ac.in/IIT_ERP3/
 
 print(LOGIN_URL)
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
-<div id="usage-in-login-workflow"></div>
-
-#### Usage in login workflow
-
-To automate the login process into ERP, the endpoints are hit in the following order:
-
-1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step establishes the initial session and retrieves `sessionToken`.
-2. Hit `SECRET_QUESTION_URL` using `session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)`. This step fetches the secret question required for authentication.
-3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests an OTP (One-Time Password) for authentication.
-4. Finally, hit `LOGIN_URL` using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step performs the actual ERP login with the provided login details and OTP.
-
-> **Note**  `session` = [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) is used to persist the session parameters throughout the workflow
-
 <div id="login"></div>
 
 ### Login
 
-ERP login workflow is implemented in `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
-The function requires following arguments:
-1. `headers`: Headers for the post requests. An example is given below.
+The function requires following _compulsory_ arguments:
+1. `headers`: Headers for the post requests.
     ```python
     headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
     }
     ``` 
-2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported into python file.
-    ```python
-    import erpcreds
-    ```
-3.  `OTP_WAIT_INTERVAL`: The interval after which the API continuously checks for new OTP mail.
-4.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+2.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
     ```python
     import requests
 
     session = requests.Session()
     ```
 
+The function can also be provided with these _optional_ arguments:
+
+<div id="erpcreds"></div>
+
+1.  `ERPCREDS`: ERP Login Credentials python file, which is imported into main python file.<br>
+    | Default Value | `None` |
+    |---|---|
+    | NOT Specified | The user is prompted to enter their credentials manually |
+    | Specified (`ERPCREDS=erpcreds`) | The credentials are retrieved from the `erpcreds.py` file |
+
+    > **Note** Here, `credentials` refer to the roll number, password, and security question.
+    <details>
+      <summary><b>Prerequisites - ERP credentials file</b></summary>
+      
+    - This file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
+    - Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
+      - You can choose any valid name for the file, adhering to Python's naming conventions.
+      - **Do not change the variable names**. Copy the format provided below & update the values inside the `double quotes` (").
+        ```python
+        # ERP Credentials
+        ROLL_NUMBER = "XXYYXXXXX"
+        PASSWORD = "**********"
+        SECURITY_QUESTIONS_ANSWERS = {
+            "Q1" : "A1",
+            "Q2" : "A2",
+            "Q3" : "A3",
+        }
+        ```
+      
+    </details>
+    
+<div id="token"></div>
+    
+2.  `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API continuously checks for new OTP emails.
+    | Default Value | `None` |
+    |---|---|
+    | NOT Specified | The user will be prompted to manually enter the received OTP |
+    | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and checked every `2 seconds` |
+  
+    <details>
+      <summary><b>Prerequisites - Token for GMail enabled googleapi</b></summary>
+
+    The token file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
+
+    1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
+       > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
+
+    2. To generate the `token.json` file, follow the steps below:
+        - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
+        - Import the required module, `google-auth-oauthlib`
+      
+          ```bash
+          pip install google-auth-oauthlib
+          ```
+        - Execute `gentokenjson.py` with the `readonly` argument
+   
+          ```bash
+          python3 gentokenjson.py readonly
+          ```
+        - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
+        - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
+           - Click on `Continue` instead of __Back To Safety__
+           - Then, press `Continue` again
+        - The `token.json` file will be generated in the same folder as the `credentials.json` file
+  
+        > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
+
+3.  `LOGGING`: Toggles **comprehensive logging**.
+    | Default value | `False` |
+    |---|---|
+    | NOT Specified | No Logging |
+    | Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+    
 <div id="login-output"></div>
 
 #### Output
-1. The function returns the following in the order of occurrence as here (`sessionToken, ssoToekn`):
+1. The function returns the following, in the order of occurrence as here (`return sessionToken, ssoToken`):
    1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
    2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
-2. It also modifies the `session` object, which now includes parameters for the logged-in session. These parameters can be utilized for further navigation within the ERP system.
-3. It incorporates **comprehensive logging**. It prints the status of each step, providing detailed information throughout the process.
+2. It also modifies the `session` object, which now includes parameters for the logged-in session. This `session` object can be utilized for further navigation within the ERP system.
 
 <div id="login-usage"></div>
 
 #### Usage
-It is recommended to use the `login` function in the following manner:
+It is recommended to use the `login` function in the following manner (optional arguments are _your_ choice):
 ```python
-# importing the erp.py file
+# Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
-# using the login function inside erp.py
-sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
+# Using the login function inside erp.py
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
@@ -156,25 +189,37 @@
 headers = {
    'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
-sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
-   
-print(sessionToken, ssoToken)
-```
+sessionToken, ssoToken = erp.login(headers, session)
+# Credentials: Manual | OTP: Manual | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds)
+# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2)
+# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, LOGGING=True)
+# Credentials: Manual | OTP: Manual | Logging: Yes
 
-> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5)
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+```
 
 <div id="session-alive"></div>
 
 ### Session status check
-The logic for checking the status of the session is implemented in the `session_alive(session)` function  n [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
+The logic for checking the status of the session is implemented in the `session_alive(session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
 The function requires following argument:
 
  -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
@@ -182,15 +227,19 @@
     import requests
 
     session = requests.Session()
      ```
 <div id="session-alive-output"></div>
 
 #### Output
-The `session_alive(session)` function returns the status of the session as a boolean value: **True** if it is alive and **False** if it is not.
+The `session_alive(session)` function returns the status of the session as a boolean value:
+| Status | Return Value |
+| ------ | :------------: |
+| Valid (`Alive`)  | `True` |
+| Not Valid (`Dead`) | `False` |
 
 <div id="session-alive-usage"></div>
 
 #### Usage
 It is recommended to use the `session_alive` function in the following manner:
 ```python
 # Importing the erp.py file
@@ -201,118 +250,43 @@
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function and `session_alive` function:
 
 ```python
 import requests
 import time
+
 import creds
+# Importing creds.py, which contains ERP credentials
+
 import iitkgp_erp_login.erp as erp
 
 headers = {
     'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
+print("Logging into ERP for:", creds.ROLL_NUMBER)
+
 while True:
     if not erp.session_alive(session):
-        erp.login(headers, creds, 2, session)
+        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
-> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
-
-<div id="package-usage"></div>
-
-## Usage
-
-<div id="prerequisites"></div>
-
-### Prerequisites
-
-The following scripts are required and **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported:
-
-- <a href="#erpcreds">erpcreds.py</a>
-- <a href="#token">token.json</a>
-
-<div id="erpcreds"></div>
-
-#### ERP credentials file
-
-<div id="erpcreds-creating"></div>
-
-##### Creating
-
-Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
-- You can choose any valid name for the file, adhering to Python's naming conventions.
-- **Do not change the variable names**. Simply copy the format provided below and update the values inside the `double quotes` (").
-  ```python
-  # ERP Credentials
-  ROLL_NUMBER = "XXYYXXXXX"
-  PASSWORD = "**********"
-  SECURITY_QUESTIONS_ANSWERS = {
-      "Q1" : "A1",
-      "Q2" : "A2",
-      "Q3" : "A3",
-  }
-  ```
-
-<div id="erpcreds-using"></div>
-
-##### Using
-
-Let's suppose you have saved the ERP credentials file as `erpcreds.py`. To use it, you can simply import it in your Python script using the following code:
-
-```python
-import erpcreds
-
-print(erpcreds.ROLL_NUMBER)
-# Output: XXYYXXXXX
-
-print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"])
-# Output: A2
-```
-
-<div id="token"></div>
-
-#### Generating token for GMail enabled googleapi
-
-1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
-   > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
-
-2. To generate the `token.json` file, follow the steps below:
-    - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
-    - Import the required module, `google-auth-oauthlib`
-      
-      ```bash
-      pip install google-auth-oauthlib
-      ```
-    - Execute `gentokenjson.py` with the `readonly` argument
-   
-      ```bash
-      python3 gentokenjson.py readonly
-      ```
-    - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
-    - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
-       - Click on `Continue` instead of __Back To Safety__
-       - Then, press `Continue` again
-    - The `token.json` file will be generated in the same folder as the `credentials.json` file
-  
-    > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
-
 <div id="example"></div>
 
-### Example
+## Example
 
-Now, we will create a script that opens the ERP system on your default browser with a logged-in session.
+Now, we will create a script that opens the ERP Homepage on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
    pip install iitkgp_erp_login
    ````
 2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
@@ -329,15 +303,15 @@
    headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
    }
 
    session = requests.Session()
 
-   _, ssoToken = erp.login(headers, erpcreds, 2, session)
+   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
 4. Run the script.
    ```bash
    python3 open_erp.py
```

#### html2text {}

```diff
@@ -1,26 +1,18 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 1.0.1 Summary: A package
-to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
-pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
-Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # ERP Login Module A python package/module to automate login process in
-ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
-Usage_in_login_workflow - Login - Input - Output - Usage - Session_status_check
-- Input - Output - Usage - Usage - Prerequisites - ERP_credentials_file -
-Creating - Using - Generating_token_for_GMail_enabled_googleapi - Example
+# ERP Login Module A python package/module to automate login process in ERP for
+IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage - Login -
+Input - Output - Usage - Session_status_check - Input - Output - Usage -
+Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
 erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
 iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
-implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various
+implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various
 helper functions. These functions are not intended to be used by _you_, the
 user. The only case where OTP is required is during the login process, which is
-handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
+handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
 abstraction for general users. If you want to modify the OTP fetching process,
 feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
 erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 ### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
@@ -30,124 +22,128 @@
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
 The URL of the welcome page, which is accessible only when the user is **NOT**
 logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
 is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
-#### Usage in login workflow To automate the login process into ERP, the
-endpoints are hit in the following order: 1. Hit `HOMEPAGE_URL` using
-`session.get(HOMEPAGE_URL)`. This step establishes the initial session and
-retrieves `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
-(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER},
-headers=headers)`. This step fetches the secret question required for
-authentication. 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee':
-'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests
-an OTP (One-Time Password) for authentication. 4. Finally, hit `LOGIN_URL`
-using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step
-performs the actual ERP login with the provided login details and OTP. >
-**Note** `session` = [requests.Session()](https://docs.python-requests.org/en/
-latest/_modules/requests/sessions/) is used to persist the session parameters
-throughout the workflow
-### Login ERP login workflow is implemented in `login(headers, erp_creds,
-OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
-output specifications for the function are mentioned below.
-#### Input The function requires following arguments: 1. `headers`: Headers for
-the post requests. An example is given below. ```python headers = { 'timeout':
+### Login ERP login workflow is implemented in `login(headers, session,
+ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py]
+(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
+iitkgp_erp_login/erp.py). The input and output specifications for the function
+are mentioned below.
+#### Input The function requires following _compulsory_ arguments: 1.
+`headers`: Headers for the post requests. ```python headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-``` 2. `erp_creds`: ERP_Login_Credentials_file, which is imported into python
-file. ```python import erpcreds ``` 3. `OTP_WAIT_INTERVAL`: The interval after
-which the API continuously checks for new OTP mail. 4. `session`: A
-[requests.Session()](https://docs.python-requests.org/en/latest/_modules/
-requests/sessions/) object, to persist the session parameters throughout the
-workflow. ```python import requests session = requests.Session() ```
-#### Output 1. The function returns the following in the order of occurrence as
-here (`sessionToken, ssoToekn`): 1. [sessionToken](https://en.wikipedia.org/
-wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
-It also modifies the `session` object, which now includes parameters for the
-logged-in session. These parameters can be utilized for further navigation
-within the ERP system. 3. It incorporates **comprehensive logging**. It prints
-the status of each step, providing detailed information throughout the process.
+``` 2. `session`: A [requests.Session()](https://docs.python-requests.org/en/
+latest/_modules/requests/sessions/) object, to persist the session parameters
+throughout the workflow. ```python import requests session = requests.Session()
+``` The function can also be provided with these _optional_ arguments:
+1. `ERPCREDS`: ERP Login Credentials python file, which is imported into main
+python file.
+| Default Value | `None` | |---|---| | NOT Specified | The user is prompted to
+enter their credentials manually | | Specified (`ERPCREDS=erpcreds`) | The
+credentials are retrieved from the `erpcreds.py` file | > **Note** Here,
+`credentials` refer to the roll number, password, and security question.
+Prerequisites - ERP credentials file - This file **MUST** be present in the
+same directory as the script where `iitkgp_erp_login` module is being imported.
+- Create a `.py` file with your ERP credentials stored in it. Please follow the
+instructions below to create this file: - You can choose any valid name for the
+file, adhering to Python's naming conventions. - **Do not change the variable
+names**. Copy the format provided below & update the values inside the `double
+quotes` ("). ```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD =
+"**********" SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" :
+"A3", } ```
+2. `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API
+continuously checks for new OTP emails. | Default Value | `None` | |---|---| |
+NOT Specified | The user will be prompted to manually enter the received OTP |
+| Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and
+checked every `2 seconds` |  Prerequisites - Token for GMail enabled googleapi
+The token file **MUST** be present in the same directory as the script where
+`iitkgp_erp_login` module is being imported. 1. Follow the steps in the [Gmail
+API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
+python) guide to obtain `credentials.json` file. > **Note** The
+`credentials.json` file is permanent unless you manually delete its reference
+in your Google Cloud Console. 2. To generate the `token.json` file, follow the
+steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
+adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
+contains the `credentials.json` file - Import the required module, `google-
+auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
+`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
+readonly ``` - A browser window will open, prompting you to select the Google
+account associated with receiving OTP for login. - Grant permission to the
+selected email address to utilize the newly enabled **Gmail API**. - Click on
+`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
+`token.json` file will be generated in the same folder as the
+`credentials.json` file > **Warning** The `token.json` file has an expiration
+time, so it's important to periodically check and refresh it in your projects
+to ensure uninterrupted access. 3. `LOGGING`: Toggles **comprehensive
+logging**. | Default value | `False` | |---|---| | NOT Specified | No Logging |
+| Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+#### Output 1. The function returns the following, in the order of occurrence
+as here (`return sessionToken, ssoToken`): 1. [sessionToken](https://
+en.wikipedia.org/wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/
+Single_sign-on) 2. It also modifies the `session` object, which now includes
+parameters for the logged-in session. This `session` object can be utilized for
+further navigation within the ERP system.
 #### Usage It is recommended to use the `login` function in the following
-manner: ```python # importing the erp.py file import iitkgp_erp_login.erp as
-erp # using the login function inside erp.py sessionToken, ssoToken = erp.login
-(headers, erpcreds, 2, session) ``` Here's an example combining all the aspects
-we have discussed so far about the `login` function: ```python import requests
-import erpcreds import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
-'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
-Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-session = requests.Session() sessionToken, ssoToken = erp.login(headers,
-erpcreds, 2, session) print(sessionToken, ssoToken) ``` > **Note** The code
-snippet above will not work unless the prerequisites are fulfilled
+manner (optional arguments are _your_ choice): ```python # Importing the erp.py
+file import iitkgp_erp_login.erp as erp # Using the login function inside
+erp.py sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, LOGGING=True) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function: ```python import
+requests import erpcreds import iitkgp_erp_login.erp as erp headers =
+{ 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/
+537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79
+Safari/537.36', } session = requests.Session() sessionToken, ssoToken =
+erp.login(headers, session) # Credentials: Manual | OTP: Manual | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds) #
+Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) #
+Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
+Credentials: Manual | OTP: Manual | Logging: Yes sessionToken, ssoToken =
+erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5) #
+Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5
+seconds | Logging: No sessionToken, ssoToken = erp.login(headers, session,
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic
+- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+```
 ### Session status check The logic for checking the status of the session is
-implemented in the `session_alive(session)` function n [erp.py](https://
+implemented in the `session_alive(session)` function in [erp.py](https://
 github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
 erp.py). This function determines whether the given session is valid/alive or
 not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
 requests/sessions/) object, to persist the session parameters throughout the
 workflow. ```python import requests session = requests.Session() ```
 #### Output The `session_alive(session)` function returns the status of the
-session as a boolean value: **True** if it is alive and **False** if it is not.
+session as a boolean value: | Status | Return Value | | ------ | :------------:
+| | Valid (`Alive`) | `True` | | Not Valid (`Dead`) | `False` |
 #### Usage It is recommended to use the `session_alive` function in the
 following manner: ```python # Importing the erp.py file import
 iitkgp_erp_login.erp as erp # Using the session_alive function inside erp.py
 print(erp.session_alive(session)) ``` Here's an example combining all the
 aspects we have discussed so far about the `login` function and `session_alive`
-function: ```python import requests import time import creds import
-iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
-requests.Session() while True: if not erp.session_alive(session): erp.login
-(headers, creds, 2, session) else: print("Session is alive.") time.sleep(2) ```
-> **Note** The code snippet above will not work unless the prerequisites are
-fulfilled
-## Usage
-### Prerequisites The following scripts are required and **MUST** be present in
-the same directory as the script where `iitkgp_erp_login` module is being
-imported: - erpcreds.py - token.json
-#### ERP credentials file
-##### Creating Create a `.py` file with your ERP credentials stored in it.
-Please follow the instructions below to create this file: - You can choose any
-valid name for the file, adhering to Python's naming conventions. - **Do not
-change the variable names**. Simply copy the format provided below and update
-the values inside the `double quotes` ("). ```python # ERP Credentials
-ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********" SECURITY_QUESTIONS_ANSWERS =
-{ "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
-##### Using Let's suppose you have saved the ERP credentials file as
-`erpcreds.py`. To use it, you can simply import it in your Python script using
-the following code: ```python import erpcreds print(erpcreds.ROLL_NUMBER) #
-Output: XXYYXXXXX print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2
-```
-#### Generating token for GMail enabled googleapi 1. Follow the steps in the
-[Gmail API - Python Quickstart](https://developers.google.com/gmail/api/
-quickstart/python) guide to obtain `credentials.json` file. > **Note** The
-`credentials.json` file is permanent unless you manually delete its reference
-in your Google Cloud Console. 2. To generate the `token.json` file, follow the
-steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
-adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
-contains the `credentials.json` file - Import the required module, `google-
-auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
-`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
-readonly ``` - A browser window will open, prompting you to select the Google
-account associated with receiving OTP for login. - Grant permission to the
-selected email address to utilize the newly enabled **Gmail API**. - Click on
-`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
-`token.json` file will be generated in the same folder as the
-`credentials.json` file > **Warning** The `token.json` file has an expiration
-time, so it's important to periodically check and refresh it in your projects
-to ensure uninterrupted access.
-### Example Now, we will create a script that opens the ERP system on your
+function: ```python import requests import time import creds # Importing
+creds.py, which contains ERP credentials import iitkgp_erp_login.erp as erp
+headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)
+AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/
+51.0.2704.79 Safari/537.36', } session = requests.Session() print("Logging into
+ERP for:", creds.ROLL_NUMBER) while True: if not erp.session_alive(session):
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
+else: print("Session is alive.") time.sleep(2) ```
+## Example Now, we will create a script that opens the ERP Homepage on your
 default browser with a logged-in session. 1. Install the package. ```bash pip
 install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
 exist in the same directory as the script we are about to create. 3. Create a
 file named `open_erp.py` and include the following code: ```python import
 requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
 from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-session = requests.Session() _, ssoToken = erp.login(headers, erpcreds, 2,
-session) logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open
-(logged_in_url) ``` 4. Run the script. ```bash python3 open_erp.py ```
+session = requests.Session() _, ssoToken = erp.login(headers, session,
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) logged_in_url = f"
+{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run
+the script. ```bash python3 open_erp.py ```
```

### Comparing `iitkgp_erp_login-1.0.1/README.md` & `iitkgp_erp_login-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,56 @@
+Metadata-Version: 2.1
+Name: iitkgp_erp_login
+Version: 2.0.0
+Summary: A package to automate login process in ERP for IIT-KGP
+Author-email: Arpit Bhardwaj <proffapt@pm.me>
+Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
+Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ERP Login Module
 
 A python package/module to automate login process in ERP for IIT-KGP.
 
 <details>
   <summary>Table of Contents</summary>
    
 - <a href="#description">Description</a>
    - <a href="#endpoints">Endpoints</a>
       - <a href="#endpoints-about">About</a>
       - <a href="#endpoints-usage">Usage</a>
-      - <a href="#usage-in-login-workflow">Usage in login workflow</a>
    - <a href="#login">Login</a>
       - <a href="#login-input">Input</a>
       - <a href="#login-output">Output</a>
       - <a href="#login-usage">Usage</a>
    - <a href="#session-alive">Session status check</a>
       - <a href="#session-alive-input">Input</a>
       - <a href="#session-alive-output">Output</a>
       - <a href="#session-alive-usage">Usage</a>
-- <a href="#package-usage">Usage</a>
-   - <a href="#prerequisites">Prerequisites</a>
-      - <a href="#erpcreds">ERP credentials file</a>
-         - <a href="#erpcreds-creating">Creating</a>
-         - <a href="#erpcreds-using">Using</a>
-      - <a href="#token">Generating token for GMail enabled googleapi</a>
-   - <a href="#example">Example</a>
+- <a href="#example">Example</a>
    
 </details>
 
 <div id="description"></div>
 
 ## Description
 
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
    └── read_mail.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
 The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
@@ -65,75 +72,129 @@
 print(HOMEPAGE_URL)
 # Output: https://erp.iitkgp.ac.in/IIT_ERP3/
 
 print(LOGIN_URL)
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
-<div id="usage-in-login-workflow"></div>
-
-#### Usage in login workflow
-
-To automate the login process into ERP, the endpoints are hit in the following order:
-
-1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step establishes the initial session and retrieves `sessionToken`.
-2. Hit `SECRET_QUESTION_URL` using `session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)`. This step fetches the secret question required for authentication.
-3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests an OTP (One-Time Password) for authentication.
-4. Finally, hit `LOGIN_URL` using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step performs the actual ERP login with the provided login details and OTP.
-
-> **Note**  `session` = [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) is used to persist the session parameters throughout the workflow
-
 <div id="login"></div>
 
 ### Login
 
-ERP login workflow is implemented in `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
-The function requires following arguments:
-1. `headers`: Headers for the post requests. An example is given below.
+The function requires following _compulsory_ arguments:
+1. `headers`: Headers for the post requests.
     ```python
     headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
     }
     ``` 
-2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported into python file.
-    ```python
-    import erpcreds
-    ```
-3.  `OTP_WAIT_INTERVAL`: The interval after which the API continuously checks for new OTP mail.
-4.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+2.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
     ```python
     import requests
 
     session = requests.Session()
     ```
 
+The function can also be provided with these _optional_ arguments:
+
+<div id="erpcreds"></div>
+
+1.  `ERPCREDS`: ERP Login Credentials python file, which is imported into main python file.<br>
+    | Default Value | `None` |
+    |---|---|
+    | NOT Specified | The user is prompted to enter their credentials manually |
+    | Specified (`ERPCREDS=erpcreds`) | The credentials are retrieved from the `erpcreds.py` file |
+
+    > **Note** Here, `credentials` refer to the roll number, password, and security question.
+    <details>
+      <summary><b>Prerequisites - ERP credentials file</b></summary>
+      
+    - This file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
+    - Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
+      - You can choose any valid name for the file, adhering to Python's naming conventions.
+      - **Do not change the variable names**. Copy the format provided below & update the values inside the `double quotes` (").
+        ```python
+        # ERP Credentials
+        ROLL_NUMBER = "XXYYXXXXX"
+        PASSWORD = "**********"
+        SECURITY_QUESTIONS_ANSWERS = {
+            "Q1" : "A1",
+            "Q2" : "A2",
+            "Q3" : "A3",
+        }
+        ```
+      
+    </details>
+    
+<div id="token"></div>
+    
+2.  `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API continuously checks for new OTP emails.
+    | Default Value | `None` |
+    |---|---|
+    | NOT Specified | The user will be prompted to manually enter the received OTP |
+    | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and checked every `2 seconds` |
+  
+    <details>
+      <summary><b>Prerequisites - Token for GMail enabled googleapi</b></summary>
+
+    The token file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
+
+    1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
+       > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
+
+    2. To generate the `token.json` file, follow the steps below:
+        - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
+        - Import the required module, `google-auth-oauthlib`
+      
+          ```bash
+          pip install google-auth-oauthlib
+          ```
+        - Execute `gentokenjson.py` with the `readonly` argument
+   
+          ```bash
+          python3 gentokenjson.py readonly
+          ```
+        - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
+        - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
+           - Click on `Continue` instead of __Back To Safety__
+           - Then, press `Continue` again
+        - The `token.json` file will be generated in the same folder as the `credentials.json` file
+  
+        > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
+
+3.  `LOGGING`: Toggles **comprehensive logging**.
+    | Default value | `False` |
+    |---|---|
+    | NOT Specified | No Logging |
+    | Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+    
 <div id="login-output"></div>
 
 #### Output
-1. The function returns the following in the order of occurrence as here (`sessionToken, ssoToekn`):
+1. The function returns the following, in the order of occurrence as here (`return sessionToken, ssoToken`):
    1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
    2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
-2. It also modifies the `session` object, which now includes parameters for the logged-in session. These parameters can be utilized for further navigation within the ERP system.
-3. It incorporates **comprehensive logging**. It prints the status of each step, providing detailed information throughout the process.
+2. It also modifies the `session` object, which now includes parameters for the logged-in session. This `session` object can be utilized for further navigation within the ERP system.
 
 <div id="login-usage"></div>
 
 #### Usage
-It is recommended to use the `login` function in the following manner:
+It is recommended to use the `login` function in the following manner (optional arguments are _your_ choice):
 ```python
-# importing the erp.py file
+# Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
-# using the login function inside erp.py
-sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
+# Using the login function inside erp.py
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
@@ -142,25 +203,37 @@
 headers = {
    'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
-sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
-   
-print(sessionToken, ssoToken)
-```
+sessionToken, ssoToken = erp.login(headers, session)
+# Credentials: Manual | OTP: Manual | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds)
+# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2)
+# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, LOGGING=True)
+# Credentials: Manual | OTP: Manual | Logging: Yes
 
-> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5)
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+```
 
 <div id="session-alive"></div>
 
 ### Session status check
-The logic for checking the status of the session is implemented in the `session_alive(session)` function  n [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
+The logic for checking the status of the session is implemented in the `session_alive(session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
 The function requires following argument:
 
  -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
@@ -168,15 +241,19 @@
     import requests
 
     session = requests.Session()
      ```
 <div id="session-alive-output"></div>
 
 #### Output
-The `session_alive(session)` function returns the status of the session as a boolean value: **True** if it is alive and **False** if it is not.
+The `session_alive(session)` function returns the status of the session as a boolean value:
+| Status | Return Value |
+| ------ | :------------: |
+| Valid (`Alive`)  | `True` |
+| Not Valid (`Dead`) | `False` |
 
 <div id="session-alive-usage"></div>
 
 #### Usage
 It is recommended to use the `session_alive` function in the following manner:
 ```python
 # Importing the erp.py file
@@ -187,118 +264,43 @@
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function and `session_alive` function:
 
 ```python
 import requests
 import time
+
 import creds
+# Importing creds.py, which contains ERP credentials
+
 import iitkgp_erp_login.erp as erp
 
 headers = {
     'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
+print("Logging into ERP for:", creds.ROLL_NUMBER)
+
 while True:
     if not erp.session_alive(session):
-        erp.login(headers, creds, 2, session)
+        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
-> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
-
-<div id="package-usage"></div>
-
-## Usage
-
-<div id="prerequisites"></div>
-
-### Prerequisites
-
-The following scripts are required and **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported:
-
-- <a href="#erpcreds">erpcreds.py</a>
-- <a href="#token">token.json</a>
-
-<div id="erpcreds"></div>
-
-#### ERP credentials file
-
-<div id="erpcreds-creating"></div>
-
-##### Creating
-
-Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
-- You can choose any valid name for the file, adhering to Python's naming conventions.
-- **Do not change the variable names**. Simply copy the format provided below and update the values inside the `double quotes` (").
-  ```python
-  # ERP Credentials
-  ROLL_NUMBER = "XXYYXXXXX"
-  PASSWORD = "**********"
-  SECURITY_QUESTIONS_ANSWERS = {
-      "Q1" : "A1",
-      "Q2" : "A2",
-      "Q3" : "A3",
-  }
-  ```
-
-<div id="erpcreds-using"></div>
-
-##### Using
-
-Let's suppose you have saved the ERP credentials file as `erpcreds.py`. To use it, you can simply import it in your Python script using the following code:
-
-```python
-import erpcreds
-
-print(erpcreds.ROLL_NUMBER)
-# Output: XXYYXXXXX
-
-print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"])
-# Output: A2
-```
-
-<div id="token"></div>
-
-#### Generating token for GMail enabled googleapi
-
-1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
-   > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
-
-2. To generate the `token.json` file, follow the steps below:
-    - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
-    - Import the required module, `google-auth-oauthlib`
-      
-      ```bash
-      pip install google-auth-oauthlib
-      ```
-    - Execute `gentokenjson.py` with the `readonly` argument
-   
-      ```bash
-      python3 gentokenjson.py readonly
-      ```
-    - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
-    - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
-       - Click on `Continue` instead of __Back To Safety__
-       - Then, press `Continue` again
-    - The `token.json` file will be generated in the same folder as the `credentials.json` file
-  
-    > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
-
 <div id="example"></div>
 
-### Example
+## Example
 
-Now, we will create a script that opens the ERP system on your default browser with a logged-in session.
+Now, we will create a script that opens the ERP Homepage on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
    pip install iitkgp_erp_login
    ````
 2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
@@ -315,15 +317,15 @@
    headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
    }
 
    session = requests.Session()
 
-   _, ssoToken = erp.login(headers, erpcreds, 2, session)
+   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
 4. Run the script.
    ```bash
    python3 open_erp.py
```

#### html2text {}

```diff
@@ -1,19 +1,25 @@
-# ERP Login Module A python package/module to automate login process in ERP for
-IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage - Usage
-in_login_workflow - Login - Input - Output - Usage - Session_status_check -
-Input - Output - Usage - Usage - Prerequisites - ERP_credentials_file -
-Creating - Using - Generating_token_for_GMail_enabled_googleapi - Example
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.0.0 Summary: A package
+to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
+pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
+Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # ERP Login Module A python package/module to automate login process in
+ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
+Login - Input - Output - Usage - Session_status_check - Input - Output - Usage
+- Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
 erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
 iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
-implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various
+implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various
 helper functions. These functions are not intended to be used by _you_, the
 user. The only case where OTP is required is during the login process, which is
-handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
+handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
 abstraction for general users. If you want to modify the OTP fetching process,
 feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
 erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 ### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
@@ -23,124 +29,128 @@
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
 The URL of the welcome page, which is accessible only when the user is **NOT**
 logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
 is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
-#### Usage in login workflow To automate the login process into ERP, the
-endpoints are hit in the following order: 1. Hit `HOMEPAGE_URL` using
-`session.get(HOMEPAGE_URL)`. This step establishes the initial session and
-retrieves `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
-(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER},
-headers=headers)`. This step fetches the secret question required for
-authentication. 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee':
-'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests
-an OTP (One-Time Password) for authentication. 4. Finally, hit `LOGIN_URL`
-using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step
-performs the actual ERP login with the provided login details and OTP. >
-**Note** `session` = [requests.Session()](https://docs.python-requests.org/en/
-latest/_modules/requests/sessions/) is used to persist the session parameters
-throughout the workflow
-### Login ERP login workflow is implemented in `login(headers, erp_creds,
-OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
-output specifications for the function are mentioned below.
-#### Input The function requires following arguments: 1. `headers`: Headers for
-the post requests. An example is given below. ```python headers = { 'timeout':
+### Login ERP login workflow is implemented in `login(headers, session,
+ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py]
+(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
+iitkgp_erp_login/erp.py). The input and output specifications for the function
+are mentioned below.
+#### Input The function requires following _compulsory_ arguments: 1.
+`headers`: Headers for the post requests. ```python headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-``` 2. `erp_creds`: ERP_Login_Credentials_file, which is imported into python
-file. ```python import erpcreds ``` 3. `OTP_WAIT_INTERVAL`: The interval after
-which the API continuously checks for new OTP mail. 4. `session`: A
-[requests.Session()](https://docs.python-requests.org/en/latest/_modules/
-requests/sessions/) object, to persist the session parameters throughout the
-workflow. ```python import requests session = requests.Session() ```
-#### Output 1. The function returns the following in the order of occurrence as
-here (`sessionToken, ssoToekn`): 1. [sessionToken](https://en.wikipedia.org/
-wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
-It also modifies the `session` object, which now includes parameters for the
-logged-in session. These parameters can be utilized for further navigation
-within the ERP system. 3. It incorporates **comprehensive logging**. It prints
-the status of each step, providing detailed information throughout the process.
+``` 2. `session`: A [requests.Session()](https://docs.python-requests.org/en/
+latest/_modules/requests/sessions/) object, to persist the session parameters
+throughout the workflow. ```python import requests session = requests.Session()
+``` The function can also be provided with these _optional_ arguments:
+1. `ERPCREDS`: ERP Login Credentials python file, which is imported into main
+python file.
+| Default Value | `None` | |---|---| | NOT Specified | The user is prompted to
+enter their credentials manually | | Specified (`ERPCREDS=erpcreds`) | The
+credentials are retrieved from the `erpcreds.py` file | > **Note** Here,
+`credentials` refer to the roll number, password, and security question.
+Prerequisites - ERP credentials file - This file **MUST** be present in the
+same directory as the script where `iitkgp_erp_login` module is being imported.
+- Create a `.py` file with your ERP credentials stored in it. Please follow the
+instructions below to create this file: - You can choose any valid name for the
+file, adhering to Python's naming conventions. - **Do not change the variable
+names**. Copy the format provided below & update the values inside the `double
+quotes` ("). ```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD =
+"**********" SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" :
+"A3", } ```
+2. `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API
+continuously checks for new OTP emails. | Default Value | `None` | |---|---| |
+NOT Specified | The user will be prompted to manually enter the received OTP |
+| Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and
+checked every `2 seconds` |  Prerequisites - Token for GMail enabled googleapi
+The token file **MUST** be present in the same directory as the script where
+`iitkgp_erp_login` module is being imported. 1. Follow the steps in the [Gmail
+API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
+python) guide to obtain `credentials.json` file. > **Note** The
+`credentials.json` file is permanent unless you manually delete its reference
+in your Google Cloud Console. 2. To generate the `token.json` file, follow the
+steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
+adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
+contains the `credentials.json` file - Import the required module, `google-
+auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
+`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
+readonly ``` - A browser window will open, prompting you to select the Google
+account associated with receiving OTP for login. - Grant permission to the
+selected email address to utilize the newly enabled **Gmail API**. - Click on
+`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
+`token.json` file will be generated in the same folder as the
+`credentials.json` file > **Warning** The `token.json` file has an expiration
+time, so it's important to periodically check and refresh it in your projects
+to ensure uninterrupted access. 3. `LOGGING`: Toggles **comprehensive
+logging**. | Default value | `False` | |---|---| | NOT Specified | No Logging |
+| Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+#### Output 1. The function returns the following, in the order of occurrence
+as here (`return sessionToken, ssoToken`): 1. [sessionToken](https://
+en.wikipedia.org/wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/
+Single_sign-on) 2. It also modifies the `session` object, which now includes
+parameters for the logged-in session. This `session` object can be utilized for
+further navigation within the ERP system.
 #### Usage It is recommended to use the `login` function in the following
-manner: ```python # importing the erp.py file import iitkgp_erp_login.erp as
-erp # using the login function inside erp.py sessionToken, ssoToken = erp.login
-(headers, erpcreds, 2, session) ``` Here's an example combining all the aspects
-we have discussed so far about the `login` function: ```python import requests
-import erpcreds import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
-'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
-Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-session = requests.Session() sessionToken, ssoToken = erp.login(headers,
-erpcreds, 2, session) print(sessionToken, ssoToken) ``` > **Note** The code
-snippet above will not work unless the prerequisites are fulfilled
+manner (optional arguments are _your_ choice): ```python # Importing the erp.py
+file import iitkgp_erp_login.erp as erp # Using the login function inside
+erp.py sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, LOGGING=True) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function: ```python import
+requests import erpcreds import iitkgp_erp_login.erp as erp headers =
+{ 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/
+537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79
+Safari/537.36', } session = requests.Session() sessionToken, ssoToken =
+erp.login(headers, session) # Credentials: Manual | OTP: Manual | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds) #
+Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) #
+Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
+Credentials: Manual | OTP: Manual | Logging: Yes sessionToken, ssoToken =
+erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5) #
+Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5
+seconds | Logging: No sessionToken, ssoToken = erp.login(headers, session,
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic
+- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+```
 ### Session status check The logic for checking the status of the session is
-implemented in the `session_alive(session)` function n [erp.py](https://
+implemented in the `session_alive(session)` function in [erp.py](https://
 github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
 erp.py). This function determines whether the given session is valid/alive or
 not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
 requests/sessions/) object, to persist the session parameters throughout the
 workflow. ```python import requests session = requests.Session() ```
 #### Output The `session_alive(session)` function returns the status of the
-session as a boolean value: **True** if it is alive and **False** if it is not.
+session as a boolean value: | Status | Return Value | | ------ | :------------:
+| | Valid (`Alive`) | `True` | | Not Valid (`Dead`) | `False` |
 #### Usage It is recommended to use the `session_alive` function in the
 following manner: ```python # Importing the erp.py file import
 iitkgp_erp_login.erp as erp # Using the session_alive function inside erp.py
 print(erp.session_alive(session)) ``` Here's an example combining all the
 aspects we have discussed so far about the `login` function and `session_alive`
-function: ```python import requests import time import creds import
-iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
-requests.Session() while True: if not erp.session_alive(session): erp.login
-(headers, creds, 2, session) else: print("Session is alive.") time.sleep(2) ```
-> **Note** The code snippet above will not work unless the prerequisites are
-fulfilled
-## Usage
-### Prerequisites The following scripts are required and **MUST** be present in
-the same directory as the script where `iitkgp_erp_login` module is being
-imported: - erpcreds.py - token.json
-#### ERP credentials file
-##### Creating Create a `.py` file with your ERP credentials stored in it.
-Please follow the instructions below to create this file: - You can choose any
-valid name for the file, adhering to Python's naming conventions. - **Do not
-change the variable names**. Simply copy the format provided below and update
-the values inside the `double quotes` ("). ```python # ERP Credentials
-ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********" SECURITY_QUESTIONS_ANSWERS =
-{ "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
-##### Using Let's suppose you have saved the ERP credentials file as
-`erpcreds.py`. To use it, you can simply import it in your Python script using
-the following code: ```python import erpcreds print(erpcreds.ROLL_NUMBER) #
-Output: XXYYXXXXX print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2
-```
-#### Generating token for GMail enabled googleapi 1. Follow the steps in the
-[Gmail API - Python Quickstart](https://developers.google.com/gmail/api/
-quickstart/python) guide to obtain `credentials.json` file. > **Note** The
-`credentials.json` file is permanent unless you manually delete its reference
-in your Google Cloud Console. 2. To generate the `token.json` file, follow the
-steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
-adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
-contains the `credentials.json` file - Import the required module, `google-
-auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
-`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
-readonly ``` - A browser window will open, prompting you to select the Google
-account associated with receiving OTP for login. - Grant permission to the
-selected email address to utilize the newly enabled **Gmail API**. - Click on
-`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
-`token.json` file will be generated in the same folder as the
-`credentials.json` file > **Warning** The `token.json` file has an expiration
-time, so it's important to periodically check and refresh it in your projects
-to ensure uninterrupted access.
-### Example Now, we will create a script that opens the ERP system on your
+function: ```python import requests import time import creds # Importing
+creds.py, which contains ERP credentials import iitkgp_erp_login.erp as erp
+headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)
+AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/
+51.0.2704.79 Safari/537.36', } session = requests.Session() print("Logging into
+ERP for:", creds.ROLL_NUMBER) while True: if not erp.session_alive(session):
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
+else: print("Session is alive.") time.sleep(2) ```
+## Example Now, we will create a script that opens the ERP Homepage on your
 default browser with a logged-in session. 1. Install the package. ```bash pip
 install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
 exist in the same directory as the script we are about to create. 3. Create a
 file named `open_erp.py` and include the following code: ```python import
 requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
 from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-session = requests.Session() _, ssoToken = erp.login(headers, erpcreds, 2,
-session) logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open
-(logged_in_url) ``` 4. Run the script. ```bash python3 open_erp.py ```
+session = requests.Session() _, ssoToken = erp.login(headers, session,
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) logged_in_url = f"
+{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run
+the script. ```bash python3 open_erp.py ```
```

### Comparing `iitkgp_erp_login-1.0.1/pyproject.toml` & `iitkgp_erp_login-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "1.0.1"
+version = "2.0.0"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/erp.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,64 +8,85 @@
 
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 logging.basicConfig(level=logging.INFO)
 
 class ErpLoginError(Exception):
     pass
 
-def login(headers, erp_creds, OTP_WAIT_INTERVAL, session):
+def login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False):
+    if ERPCREDS != None:
+        ROLL_NUMBER = ERPCREDS.ROLL_NUMBER
+        PASSWORD = ERPCREDS.PASSWORD
+    else:
+        import getpass
+        ROLL_NUMBER = input("Enter you Roll Number: ")
+        PASSWORD = getpass.getpass("Enter your ERP password: ")
+
     try:
         r = session.get(HOMEPAGE_URL)
         soup = bs(r.text, 'html.parser')
         sessionToken = soup.find(id='sessionToken')['value']
-        logging.info(" Generated session token")
+        logging.info(" Generated session token") if LOGGING else None
     except (requests.exceptions.RequestException, KeyError) as e:
         raise ErpLoginError(f"Failed to generate session token: {str(e)}")
     
     try:
-        r = session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)
+        r = session.post(SECRET_QUESTION_URL, data={'user_id': ROLL_NUMBER}, headers=headers)
         secret_question = r.text
-        secret_answer = erp_creds.SECURITY_QUESTIONS_ANSWERS[secret_question]
-        logging.info(" Fetched Security Question")
+        logging.info(" Fetched Security Question") if LOGGING else None
+
+        if ERPCREDS != None:
+            secret_answer = ERPCREDS.SECURITY_QUESTIONS_ANSWERS[secret_question]
+        else:
+            print ("Your secret question: " + secret_question)
+            secret_answer = getpass.getpass("Enter the answer to the secret question: ")
     except (requests.exceptions.RequestException, KeyError) as e:
         raise ErpLoginError(f"Failed to fetch Security Question: {str(e)}")
 
     try:
-        r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)
-        logging.info(" Requested OTP")
+        r = session.post(OTP_URL, data={'typeee': 'SI', 'loginid': ROLL_NUMBER}, headers=headers)
     except requests.exceptions.RequestException as e:
         raise ErpLoginError(f"Failed to request OTP: {str(e)}")
+    
+    login_details = {
+        'user_id': ROLL_NUMBER,
+        'password': PASSWORD,
+        'answer': secret_answer,
+        'sessionToken': sessionToken,
+        'requestedUrl': HOMEPAGE_URL,
+    }
+
+    if r.status_code == 200:
+        logging.info(" Requested OTP") if LOGGING else None
+        
+        if OTP_CHECK_INTERVAL != None:
+                try:
+                    logging.info(" Waiting for OTP...") if LOGGING else None
+                    otp = getOTP(OTP_CHECK_INTERVAL)
+                    logging.info(" Received OTP") if LOGGING else None
+                except Exception as e:
+                    raise ErpLoginError(f"Failed to receive OTP: {str(e)}")
+        else:
+            otp = input("Enter the OTP sent to your registered email address: ").strip()
+            
+        login_details['email_otp'] = otp
+    else:
+        logging.info(" OTP is not required :yay") if LOGGING else None
 
     try:
-        logging.info(" Waiting for OTP...")
-        otp = getOTP(OTP_WAIT_INTERVAL)
-        logging.info(" Received OTP")
-    except Exception as e:
-        raise ErpLoginError(f"Failed to receive OTP: {str(e)}")
-
-    try:
-        login_details = {
-            'user_id': erp_creds.ROLL_NUMBER,
-            'password': erp_creds.PASSWORD,
-            'answer': secret_answer,
-            'email_otp': otp,
-            'sessionToken': sessionToken,
-            'requestedUrl': HOMEPAGE_URL,
-        }
-
         r = session.post(LOGIN_URL, data=login_details, headers=headers)
         ssoToken = re.search(r'\?ssoToken=(.+)$', r.history[1].headers['Location'])
         if ssoToken is None:
-            raise ErpLoginError("Incorrect OTP")
+            raise ErpLoginError(f"Failed to generate ssoToken: {str(e)}")
         ssoToken = ssoToken.group(1)
-        logging.info(" Generated ssoToken")
+        logging.info(" Generated ssoToken") if LOGGING else None
     except (requests.exceptions.RequestException, IndexError) as e:
         raise ErpLoginError(f"ERP login failed: {str(e)}")
 
-    logging.info(" ERP login completed!")
+    logging.info(" ERP login completed!") if LOGGING else None
 
     return sessionToken, ssoToken
 
 
 def session_alive(session):
     r = session.get(WELCOMEPAGE_URL)
     return r.status_code == 404
```

### Comparing `iitkgp_erp_login-1.0.1/src/iitkgp_erp_login/read_mail.py` & `iitkgp_erp_login-2.0.0/src/iitkgp_erp_login/read_mail.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-1.0.1/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-2.0.0/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp-erp-login
-Version: 1.0.1
+Version: 2.0.0
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,45 +19,38 @@
 <details>
   <summary>Table of Contents</summary>
    
 - <a href="#description">Description</a>
    - <a href="#endpoints">Endpoints</a>
       - <a href="#endpoints-about">About</a>
       - <a href="#endpoints-usage">Usage</a>
-      - <a href="#usage-in-login-workflow">Usage in login workflow</a>
    - <a href="#login">Login</a>
       - <a href="#login-input">Input</a>
       - <a href="#login-output">Output</a>
       - <a href="#login-usage">Usage</a>
    - <a href="#session-alive">Session status check</a>
       - <a href="#session-alive-input">Input</a>
       - <a href="#session-alive-output">Output</a>
       - <a href="#session-alive-usage">Usage</a>
-- <a href="#package-usage">Usage</a>
-   - <a href="#prerequisites">Prerequisites</a>
-      - <a href="#erpcreds">ERP credentials file</a>
-         - <a href="#erpcreds-creating">Creating</a>
-         - <a href="#erpcreds-using">Using</a>
-      - <a href="#token">Generating token for GMail enabled googleapi</a>
-   - <a href="#example">Example</a>
+- <a href="#example">Example</a>
    
 </details>
 
 <div id="description"></div>
 
 ## Description
 
 ```graphql
 iitkgp_erp_login
    ├── endpoints.py
    ├── erp.py
    └── read_mail.py
 ```
 
-[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
+[read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various helper functions. These functions are not intended to be used by _you_, the user. The only case where OTP is required is during the login process, which is handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an abstraction for general users. If you want to modify the OTP fetching process, feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 
 <div id="endpoints"></div>
 
 ### Endpoints
 
 The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the necessary endpoints for the ERP login workflow.
 
@@ -79,75 +72,129 @@
 print(HOMEPAGE_URL)
 # Output: https://erp.iitkgp.ac.in/IIT_ERP3/
 
 print(LOGIN_URL)
 # Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm
 ```
 
-<div id="usage-in-login-workflow"></div>
-
-#### Usage in login workflow
-
-To automate the login process into ERP, the endpoints are hit in the following order:
-
-1. Hit `HOMEPAGE_URL` using `session.get(HOMEPAGE_URL)`. This step establishes the initial session and retrieves `sessionToken`.
-2. Hit `SECRET_QUESTION_URL` using `session.post(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER}, headers=headers)`. This step fetches the secret question required for authentication.
-3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee': 'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests an OTP (One-Time Password) for authentication.
-4. Finally, hit `LOGIN_URL` using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step performs the actual ERP login with the provided login details and OTP.
-
-> **Note**  `session` = [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) is used to persist the session parameters throughout the workflow
-
 <div id="login"></div>
 
 ### Login
 
-ERP login workflow is implemented in `login(headers, erp_creds, OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
+ERP login workflow is implemented in `login(headers, session, ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and output specifications for the function are mentioned below.
 
 <div id="login-input"></div>
 
 #### Input
-The function requires following arguments:
-1. `headers`: Headers for the post requests. An example is given below.
+The function requires following _compulsory_ arguments:
+1. `headers`: Headers for the post requests.
     ```python
     headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
     }
     ``` 
-2.  `erp_creds`: <a href="#erpcreds">ERP Login Credentials file</a>, which is imported into python file.
-    ```python
-    import erpcreds
-    ```
-3.  `OTP_WAIT_INTERVAL`: The interval after which the API continuously checks for new OTP mail.
-4.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
+2.  `session`: A [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
     ```python
     import requests
 
     session = requests.Session()
     ```
 
+The function can also be provided with these _optional_ arguments:
+
+<div id="erpcreds"></div>
+
+1.  `ERPCREDS`: ERP Login Credentials python file, which is imported into main python file.<br>
+    | Default Value | `None` |
+    |---|---|
+    | NOT Specified | The user is prompted to enter their credentials manually |
+    | Specified (`ERPCREDS=erpcreds`) | The credentials are retrieved from the `erpcreds.py` file |
+
+    > **Note** Here, `credentials` refer to the roll number, password, and security question.
+    <details>
+      <summary><b>Prerequisites - ERP credentials file</b></summary>
+      
+    - This file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
+    - Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
+      - You can choose any valid name for the file, adhering to Python's naming conventions.
+      - **Do not change the variable names**. Copy the format provided below & update the values inside the `double quotes` (").
+        ```python
+        # ERP Credentials
+        ROLL_NUMBER = "XXYYXXXXX"
+        PASSWORD = "**********"
+        SECURITY_QUESTIONS_ANSWERS = {
+            "Q1" : "A1",
+            "Q2" : "A2",
+            "Q3" : "A3",
+        }
+        ```
+      
+    </details>
+    
+<div id="token"></div>
+    
+2.  `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API continuously checks for new OTP emails.
+    | Default Value | `None` |
+    |---|---|
+    | NOT Specified | The user will be prompted to manually enter the received OTP |
+    | Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and checked every `2 seconds` |
+  
+    <details>
+      <summary><b>Prerequisites - Token for GMail enabled googleapi</b></summary>
+
+    The token file **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported.
+
+    1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
+       > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
+
+    2. To generate the `token.json` file, follow the steps below:
+        - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
+        - Import the required module, `google-auth-oauthlib`
+      
+          ```bash
+          pip install google-auth-oauthlib
+          ```
+        - Execute `gentokenjson.py` with the `readonly` argument
+   
+          ```bash
+          python3 gentokenjson.py readonly
+          ```
+        - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
+        - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
+           - Click on `Continue` instead of __Back To Safety__
+           - Then, press `Continue` again
+        - The `token.json` file will be generated in the same folder as the `credentials.json` file
+  
+        > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
+
+3.  `LOGGING`: Toggles **comprehensive logging**.
+    | Default value | `False` |
+    |---|---|
+    | NOT Specified | No Logging |
+    | Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+    
 <div id="login-output"></div>
 
 #### Output
-1. The function returns the following in the order of occurrence as here (`sessionToken, ssoToekn`):
+1. The function returns the following, in the order of occurrence as here (`return sessionToken, ssoToken`):
    1. [sessionToken](https://en.wikipedia.org/wiki/Session_ID)
    2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on)
-2. It also modifies the `session` object, which now includes parameters for the logged-in session. These parameters can be utilized for further navigation within the ERP system.
-3. It incorporates **comprehensive logging**. It prints the status of each step, providing detailed information throughout the process.
+2. It also modifies the `session` object, which now includes parameters for the logged-in session. This `session` object can be utilized for further navigation within the ERP system.
 
 <div id="login-usage"></div>
 
 #### Usage
-It is recommended to use the `login` function in the following manner:
+It is recommended to use the `login` function in the following manner (optional arguments are _your_ choice):
 ```python
-# importing the erp.py file
+# Importing the erp.py file
 import iitkgp_erp_login.erp as erp
 
-# using the login function inside erp.py
-sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
+# Using the login function inside erp.py
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function:
 
 ```python
 import requests
 import erpcreds
@@ -156,25 +203,37 @@
 headers = {
    'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
-sessionToken, ssoToken = erp.login(headers, erpcreds, 2, session)
-   
-print(sessionToken, ssoToken)
-```
+sessionToken, ssoToken = erp.login(headers, session)
+# Credentials: Manual | OTP: Manual | Logging: No
 
-> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds)
+# Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2)
+# Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, LOGGING=True)
+# Credentials: Manual | OTP: Manual | Logging: Yes
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5)
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5 seconds | Logging: No
+
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
+# Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+```
 
 <div id="session-alive"></div>
 
 ### Session status check
-The logic for checking the status of the session is implemented in the `session_alive(session)` function  n [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
+The logic for checking the status of the session is implemented in the `session_alive(session)` function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). This function determines whether the given session is valid/alive or not. The input and output specifications for the function are mentioned below.
 
 <div id="session-alive-input"></div>
 
 #### Input
 The function requires following argument:
 
  -  `session`: [requests.Session()](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) object, to persist the session parameters throughout the workflow.
@@ -182,15 +241,19 @@
     import requests
 
     session = requests.Session()
      ```
 <div id="session-alive-output"></div>
 
 #### Output
-The `session_alive(session)` function returns the status of the session as a boolean value: **True** if it is alive and **False** if it is not.
+The `session_alive(session)` function returns the status of the session as a boolean value:
+| Status | Return Value |
+| ------ | :------------: |
+| Valid (`Alive`)  | `True` |
+| Not Valid (`Dead`) | `False` |
 
 <div id="session-alive-usage"></div>
 
 #### Usage
 It is recommended to use the `session_alive` function in the following manner:
 ```python
 # Importing the erp.py file
@@ -201,118 +264,43 @@
 ```
 
 Here's an example combining all the aspects we have discussed so far about the `login` function and `session_alive` function:
 
 ```python
 import requests
 import time
+
 import creds
+# Importing creds.py, which contains ERP credentials
+
 import iitkgp_erp_login.erp as erp
 
 headers = {
     'timeout': '20',
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
 }
 
 session = requests.Session()
 
+print("Logging into ERP for:", creds.ROLL_NUMBER)
+
 while True:
     if not erp.session_alive(session):
-        erp.login(headers, creds, 2, session)
+        erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
     else:
         print("Session is alive.")
 
     time.sleep(2)
 ```
 
-> **Note** The code snippet above will not work unless the <a href="#prerequisites">prerequisites</a> are fulfilled
-
-<div id="package-usage"></div>
-
-## Usage
-
-<div id="prerequisites"></div>
-
-### Prerequisites
-
-The following scripts are required and **MUST** be present in the same directory as the script where `iitkgp_erp_login` module is being imported:
-
-- <a href="#erpcreds">erpcreds.py</a>
-- <a href="#token">token.json</a>
-
-<div id="erpcreds"></div>
-
-#### ERP credentials file
-
-<div id="erpcreds-creating"></div>
-
-##### Creating
-
-Create a `.py` file with your ERP credentials stored in it. Please follow the instructions below to create this file:
-- You can choose any valid name for the file, adhering to Python's naming conventions.
-- **Do not change the variable names**. Simply copy the format provided below and update the values inside the `double quotes` (").
-  ```python
-  # ERP Credentials
-  ROLL_NUMBER = "XXYYXXXXX"
-  PASSWORD = "**********"
-  SECURITY_QUESTIONS_ANSWERS = {
-      "Q1" : "A1",
-      "Q2" : "A2",
-      "Q3" : "A3",
-  }
-  ```
-
-<div id="erpcreds-using"></div>
-
-##### Using
-
-Let's suppose you have saved the ERP credentials file as `erpcreds.py`. To use it, you can simply import it in your Python script using the following code:
-
-```python
-import erpcreds
-
-print(erpcreds.ROLL_NUMBER)
-# Output: XXYYXXXXX
-
-print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"])
-# Output: A2
-```
-
-<div id="token"></div>
-
-#### Generating token for GMail enabled googleapi
-
-1. Follow the steps in the [Gmail API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/python) guide to obtain `credentials.json` file.
-   > **Note** The `credentials.json` file is permanent unless you manually delete its reference in your Google Cloud Console.
-
-2. To generate the `token.json` file, follow the steps below:
-    - Download the [gentokenjson.py](https://gist.github.com/proffapt/adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that contains the `credentials.json` file
-    - Import the required module, `google-auth-oauthlib`
-      
-      ```bash
-      pip install google-auth-oauthlib
-      ```
-    - Execute `gentokenjson.py` with the `readonly` argument
-   
-      ```bash
-      python3 gentokenjson.py readonly
-      ```
-    - A browser window will open, prompting you to select the Google account associated with receiving OTP for login.
-    - Grant permission to the selected email address to utilize the newly enabled **Gmail API**.
-       - Click on `Continue` instead of __Back To Safety__
-       - Then, press `Continue` again
-    - The `token.json` file will be generated in the same folder as the `credentials.json` file
-  
-    > **Warning** The `token.json` file has an expiration time, so it's important to periodically check and refresh it in your projects to ensure uninterrupted access.
-
 <div id="example"></div>
 
-### Example
+## Example
 
-Now, we will create a script that opens the ERP system on your default browser with a logged-in session.
+Now, we will create a script that opens the ERP Homepage on your default browser with a logged-in session.
 
 1. Install the package.
 
    ```bash
    pip install iitkgp_erp_login
    ````
 2. Make sure that <a href="#erpcreds">erpcreds.py</a> & <a href="#token">token.json</a> files exist in the same directory as the script we are about to create.
@@ -329,15 +317,15 @@
    headers = {
        'timeout': '20',
        'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36',
    }
 
    session = requests.Session()
 
-   _, ssoToken = erp.login(headers, erpcreds, 2, session)
+   _, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True)
 
    logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}"
    webbrowser.open(logged_in_url)
    ```
 4. Run the script.
    ```bash
    python3 open_erp.py
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 1.0.1 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp-erp-login Version: 2.0.0 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # ERP Login Module A python package/module to automate login process in
 ERP for IIT-KGP.  Table of Contents - Description - Endpoints - About - Usage -
-Usage_in_login_workflow - Login - Input - Output - Usage - Session_status_check
-- Input - Output - Usage - Usage - Prerequisites - ERP_credentials_file -
-Creating - Using - Generating_token_for_GMail_enabled_googleapi - Example
+Login - Input - Output - Usage - Session_status_check - Input - Output - Usage
+- Example
 ## Description ```graphql iitkgp_erp_login âââ endpoints.py âââ
 erp.py âââ read_mail.py ``` [read_mail.py](https://github.com/proffapt/
 iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) contains the
-implementation of the `getOTP(OTP_WAIT_INTERVAL)` function, along with various
+implementation of the `getOTP(OTP_CHECK_INTERVAL)` function, along with various
 helper functions. These functions are not intended to be used by _you_, the
 user. The only case where OTP is required is during the login process, which is
-handled by functions in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
+handled by function in [erp.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/erp.py). Hence, let this script serve as an
 abstraction for general users. If you want to modify the OTP fetching process,
 feel free to refer to the [read_mail.py](https://github.com/proffapt/iitkgp-
 erp-login-pypi/blob/main/src/iitkgp_erp_login/read_mail.py) script.
 ### Endpoints The [endpoints.py](https://github.com/proffapt/iitkgp-erp-login-
 pypi/blob/main/src/iitkgp_erp_login/endpoints.py) file includes all the
 necessary endpoints for the ERP login workflow.
@@ -30,124 +29,128 @@
 for authentication. - `LOGIN_URL`: The URL for ERP login. - `WELCOMEPAGE_URL`:
 The URL of the welcome page, which is accessible only when the user is **NOT**
 logged in, and behaves exactly like the `HOMEPAGE_URL`. However, when the user
 is logged in, it returns a `404` error.
 #### Usage ```python from iitkgp_erp_login.endpoints import * print
 (HOMEPAGE_URL) # Output: https://erp.iitkgp.ac.in/IIT_ERP3/ print(LOGIN_URL) #
 Output: https://erp.iitkgp.ac.in/SSOAdministration/auth.htm ```
-#### Usage in login workflow To automate the login process into ERP, the
-endpoints are hit in the following order: 1. Hit `HOMEPAGE_URL` using
-`session.get(HOMEPAGE_URL)`. This step establishes the initial session and
-retrieves `sessionToken`. 2. Hit `SECRET_QUESTION_URL` using `session.post
-(SECRET_QUESTION_URL, data={'user_id': erp_creds.ROLL_NUMBER},
-headers=headers)`. This step fetches the secret question required for
-authentication. 3. Hit `OTP_URL` using `session.post(OTP_URL, data={'typeee':
-'SI', 'loginid': erp_creds.ROLL_NUMBER}, headers=headers)`. This step requests
-an OTP (One-Time Password) for authentication. 4. Finally, hit `LOGIN_URL`
-using `session.post(LOGIN_URL, data=login_details, headers=headers)`. This step
-performs the actual ERP login with the provided login details and OTP. >
-**Note** `session` = [requests.Session()](https://docs.python-requests.org/en/
-latest/_modules/requests/sessions/) is used to persist the session parameters
-throughout the workflow
-### Login ERP login workflow is implemented in `login(headers, erp_creds,
-OTP_WAIT_INTERVAL, session)` function in [erp.py](https://github.com/proffapt/
-iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/erp.py). The input and
-output specifications for the function are mentioned below.
-#### Input The function requires following arguments: 1. `headers`: Headers for
-the post requests. An example is given below. ```python headers = { 'timeout':
+### Login ERP login workflow is implemented in `login(headers, session,
+ERPCREDS=None, OTP_CHECK_INTERVAL=None, LOGGING=False)` function in [erp.py]
+(https://github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/
+iitkgp_erp_login/erp.py). The input and output specifications for the function
+are mentioned below.
+#### Input The function requires following _compulsory_ arguments: 1.
+`headers`: Headers for the post requests. ```python headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-``` 2. `erp_creds`: ERP_Login_Credentials_file, which is imported into python
-file. ```python import erpcreds ``` 3. `OTP_WAIT_INTERVAL`: The interval after
-which the API continuously checks for new OTP mail. 4. `session`: A
-[requests.Session()](https://docs.python-requests.org/en/latest/_modules/
-requests/sessions/) object, to persist the session parameters throughout the
-workflow. ```python import requests session = requests.Session() ```
-#### Output 1. The function returns the following in the order of occurrence as
-here (`sessionToken, ssoToekn`): 1. [sessionToken](https://en.wikipedia.org/
-wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/Single_sign-on) 2.
-It also modifies the `session` object, which now includes parameters for the
-logged-in session. These parameters can be utilized for further navigation
-within the ERP system. 3. It incorporates **comprehensive logging**. It prints
-the status of each step, providing detailed information throughout the process.
+``` 2. `session`: A [requests.Session()](https://docs.python-requests.org/en/
+latest/_modules/requests/sessions/) object, to persist the session parameters
+throughout the workflow. ```python import requests session = requests.Session()
+``` The function can also be provided with these _optional_ arguments:
+1. `ERPCREDS`: ERP Login Credentials python file, which is imported into main
+python file.
+| Default Value | `None` | |---|---| | NOT Specified | The user is prompted to
+enter their credentials manually | | Specified (`ERPCREDS=erpcreds`) | The
+credentials are retrieved from the `erpcreds.py` file | > **Note** Here,
+`credentials` refer to the roll number, password, and security question.
+Prerequisites - ERP credentials file - This file **MUST** be present in the
+same directory as the script where `iitkgp_erp_login` module is being imported.
+- Create a `.py` file with your ERP credentials stored in it. Please follow the
+instructions below to create this file: - You can choose any valid name for the
+file, adhering to Python's naming conventions. - **Do not change the variable
+names**. Copy the format provided below & update the values inside the `double
+quotes` ("). ```python # ERP Credentials ROLL_NUMBER = "XXYYXXXXX" PASSWORD =
+"**********" SECURITY_QUESTIONS_ANSWERS = { "Q1" : "A1", "Q2" : "A2", "Q3" :
+"A3", } ```
+2. `OTP_CHECK_INTERVAL`: The interval, in seconds, after which the API
+continuously checks for new OTP emails. | Default Value | `None` | |---|---| |
+NOT Specified | The user will be prompted to manually enter the received OTP |
+| Specified (`OTP_CHECKINTERVAL=2`) | The OTP will be automatically fetched and
+checked every `2 seconds` |  Prerequisites - Token for GMail enabled googleapi
+The token file **MUST** be present in the same directory as the script where
+`iitkgp_erp_login` module is being imported. 1. Follow the steps in the [Gmail
+API - Python Quickstart](https://developers.google.com/gmail/api/quickstart/
+python) guide to obtain `credentials.json` file. > **Note** The
+`credentials.json` file is permanent unless you manually delete its reference
+in your Google Cloud Console. 2. To generate the `token.json` file, follow the
+steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
+adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
+contains the `credentials.json` file - Import the required module, `google-
+auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
+`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
+readonly ``` - A browser window will open, prompting you to select the Google
+account associated with receiving OTP for login. - Grant permission to the
+selected email address to utilize the newly enabled **Gmail API**. - Click on
+`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
+`token.json` file will be generated in the same folder as the
+`credentials.json` file > **Warning** The `token.json` file has an expiration
+time, so it's important to periodically check and refresh it in your projects
+to ensure uninterrupted access. 3. `LOGGING`: Toggles **comprehensive
+logging**. | Default value | `False` | |---|---| | NOT Specified | No Logging |
+| Specified (`LOGGING=True`) | Logs every step in an exhaustive manner |
+#### Output 1. The function returns the following, in the order of occurrence
+as here (`return sessionToken, ssoToken`): 1. [sessionToken](https://
+en.wikipedia.org/wiki/Session_ID) 2. [ssoToken](https://en.wikipedia.org/wiki/
+Single_sign-on) 2. It also modifies the `session` object, which now includes
+parameters for the logged-in session. This `session` object can be utilized for
+further navigation within the ERP system.
 #### Usage It is recommended to use the `login` function in the following
-manner: ```python # importing the erp.py file import iitkgp_erp_login.erp as
-erp # using the login function inside erp.py sessionToken, ssoToken = erp.login
-(headers, erpcreds, 2, session) ``` Here's an example combining all the aspects
-we have discussed so far about the `login` function: ```python import requests
-import erpcreds import iitkgp_erp_login.erp as erp headers = { 'timeout': '20',
-'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like
-Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-session = requests.Session() sessionToken, ssoToken = erp.login(headers,
-erpcreds, 2, session) print(sessionToken, ssoToken) ``` > **Note** The code
-snippet above will not work unless the prerequisites are fulfilled
+manner (optional arguments are _your_ choice): ```python # Importing the erp.py
+file import iitkgp_erp_login.erp as erp # Using the login function inside
+erp.py sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds,
+OTP_CHECK_INTERVAL=2, LOGGING=True) ``` Here's an example combining all the
+aspects we have discussed so far about the `login` function: ```python import
+requests import erpcreds import iitkgp_erp_login.erp as erp headers =
+{ 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/
+537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79
+Safari/537.36', } session = requests.Session() sessionToken, ssoToken =
+erp.login(headers, session) # Credentials: Manual | OTP: Manual | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, ERPCREDS=erpcreds) #
+Credentials: Automatic - from erpcreds.py | OTP: Manual | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, OTP_CHECK_INTERVAL=2) #
+Credentials: Manual | OTP: Automatic - checked every 2 seconds | Logging: No
+sessionToken, ssoToken = erp.login(headers, session, LOGGING=True) #
+Credentials: Manual | OTP: Manual | Logging: Yes sessionToken, ssoToken =
+erp.login(headers, session, ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=5) #
+Credentials: Automatic - from erpcreds.py | OTP: Automatic - checked every 5
+seconds | Logging: No sessionToken, ssoToken = erp.login(headers, session,
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) # Credentials: Automatic
+- from erpcreds.py | OTP: Automatic - checked every 2 seconds | Logging: Yes
+```
 ### Session status check The logic for checking the status of the session is
-implemented in the `session_alive(session)` function n [erp.py](https://
+implemented in the `session_alive(session)` function in [erp.py](https://
 github.com/proffapt/iitkgp-erp-login-pypi/blob/main/src/iitkgp_erp_login/
 erp.py). This function determines whether the given session is valid/alive or
 not. The input and output specifications for the function are mentioned below.
 #### Input The function requires following argument: - `session`:
 [requests.Session()](https://docs.python-requests.org/en/latest/_modules/
 requests/sessions/) object, to persist the session parameters throughout the
 workflow. ```python import requests session = requests.Session() ```
 #### Output The `session_alive(session)` function returns the status of the
-session as a boolean value: **True** if it is alive and **False** if it is not.
+session as a boolean value: | Status | Return Value | | ------ | :------------:
+| | Valid (`Alive`) | `True` | | Not Valid (`Dead`) | `False` |
 #### Usage It is recommended to use the `session_alive` function in the
 following manner: ```python # Importing the erp.py file import
 iitkgp_erp_login.erp as erp # Using the session_alive function inside erp.py
 print(erp.session_alive(session)) ``` Here's an example combining all the
 aspects we have discussed so far about the `login` function and `session_alive`
-function: ```python import requests import time import creds import
-iitkgp_erp_login.erp as erp headers = { 'timeout': '20', 'User-Agent':
-'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu
-Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', } session =
-requests.Session() while True: if not erp.session_alive(session): erp.login
-(headers, creds, 2, session) else: print("Session is alive.") time.sleep(2) ```
-> **Note** The code snippet above will not work unless the prerequisites are
-fulfilled
-## Usage
-### Prerequisites The following scripts are required and **MUST** be present in
-the same directory as the script where `iitkgp_erp_login` module is being
-imported: - erpcreds.py - token.json
-#### ERP credentials file
-##### Creating Create a `.py` file with your ERP credentials stored in it.
-Please follow the instructions below to create this file: - You can choose any
-valid name for the file, adhering to Python's naming conventions. - **Do not
-change the variable names**. Simply copy the format provided below and update
-the values inside the `double quotes` ("). ```python # ERP Credentials
-ROLL_NUMBER = "XXYYXXXXX" PASSWORD = "**********" SECURITY_QUESTIONS_ANSWERS =
-{ "Q1" : "A1", "Q2" : "A2", "Q3" : "A3", } ```
-##### Using Let's suppose you have saved the ERP credentials file as
-`erpcreds.py`. To use it, you can simply import it in your Python script using
-the following code: ```python import erpcreds print(erpcreds.ROLL_NUMBER) #
-Output: XXYYXXXXX print(erpcreds.SECURITY_QUESTIONS_ANSWERS["Q2"]) # Output: A2
-```
-#### Generating token for GMail enabled googleapi 1. Follow the steps in the
-[Gmail API - Python Quickstart](https://developers.google.com/gmail/api/
-quickstart/python) guide to obtain `credentials.json` file. > **Note** The
-`credentials.json` file is permanent unless you manually delete its reference
-in your Google Cloud Console. 2. To generate the `token.json` file, follow the
-steps below: - Download the [gentokenjson.py](https://gist.github.com/proffapt/
-adbc716a427c036f238e828d8995e1a3) file and place it in the same folder that
-contains the `credentials.json` file - Import the required module, `google-
-auth-oauthlib` ```bash pip install google-auth-oauthlib ``` - Execute
-`gentokenjson.py` with the `readonly` argument ```bash python3 gentokenjson.py
-readonly ``` - A browser window will open, prompting you to select the Google
-account associated with receiving OTP for login. - Grant permission to the
-selected email address to utilize the newly enabled **Gmail API**. - Click on
-`Continue` instead of __Back To Safety__ - Then, press `Continue` again - The
-`token.json` file will be generated in the same folder as the
-`credentials.json` file > **Warning** The `token.json` file has an expiration
-time, so it's important to periodically check and refresh it in your projects
-to ensure uninterrupted access.
-### Example Now, we will create a script that opens the ERP system on your
+function: ```python import requests import time import creds # Importing
+creds.py, which contains ERP credentials import iitkgp_erp_login.erp as erp
+headers = { 'timeout': '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64)
+AppleWebKit/537.36 (KHTML, like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/
+51.0.2704.79 Safari/537.36', } session = requests.Session() print("Logging into
+ERP for:", creds.ROLL_NUMBER) while True: if not erp.session_alive(session):
+erp.login(headers, session, ERPCREDS=creds, OTP_CHECK_TIMEOUT=2, LOGGING=True)
+else: print("Session is alive.") time.sleep(2) ```
+## Example Now, we will create a script that opens the ERP Homepage on your
 default browser with a logged-in session. 1. Install the package. ```bash pip
 install iitkgp_erp_login ```` 2. Make sure that erpcreds.py & token.json files
 exist in the same directory as the script we are about to create. 3. Create a
 file named `open_erp.py` and include the following code: ```python import
 requests import webbrowser import erpcreds import iitkgp_erp_login.erp as erp
 from iitkgp_erp_login.endpoints import HOMEPAGE_URL headers = { 'timeout':
 '20', 'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML,
 like Gecko) Ubuntu Chromium/51.0.2704.79 Chrome/51.0.2704.79 Safari/537.36', }
-session = requests.Session() _, ssoToken = erp.login(headers, erpcreds, 2,
-session) logged_in_url = f"{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open
-(logged_in_url) ``` 4. Run the script. ```bash python3 open_erp.py ```
+session = requests.Session() _, ssoToken = erp.login(headers, session,
+ERPCREDS=erpcreds, OTP_CHECK_INTERVAL=2, LOGGING=True) logged_in_url = f"
+{HOMEPAGE_URL}?ssoToken={ssoToken}" webbrowser.open(logged_in_url) ``` 4. Run
+the script. ```bash python3 open_erp.py ```
```

