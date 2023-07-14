# Comparing `tmp/basket-client-1.0.0.tar.gz` & `tmp/basket_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/basket-client-1.0.0.tar", last modified: Mon Jan  7 21:41:38 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `basket-client-1.0.0.tar` & `basket_client-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-07 21:41:38.000000 basket-client-1.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2019-01-07 21:41:06.000000 basket-client-1.0.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-07 21:41:38.000000 basket-client-1.0.0/basket_client.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2019-01-07 21:41:37.000000 basket-client-1.0.0/basket_client.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-07 21:41:37.000000 basket-client-1.0.0/basket_client.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2019-01-07 21:41:37.000000 basket-client-1.0.0/basket_client.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-01-07 21:41:37.000000 basket-client-1.0.0/basket_client.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-01-07 21:41:37.000000 basket-client-1.0.0/basket_client.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1743 2019-01-07 21:41:38.000000 basket-client-1.0.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-07 21:41:38.000000 basket-client-1.0.0/basket/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21315 2019-01-07 21:41:06.000000 basket-client-1.0.0/basket/tests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8946 2019-01-07 21:41:06.000000 basket-client-1.0.0/basket/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      376 2019-01-07 21:41:06.000000 basket-client-1.0.0/basket/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2019-01-07 21:41:06.000000 basket-client-1.0.0/basket/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2019-01-07 21:41:38.000000 basket-client-1.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2019-01-07 21:41:06.000000 basket-client-1.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      658 2019-01-07 21:41:06.000000 basket-client-1.0.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2019-01-07 21:41:06.000000 basket-client-1.0.0/setup.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/change_log.rst
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/install.rst
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 basket_client-1.1.0/docs/usage.rst
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 basket_client-1.1.0/src/basket/__init__.py
+-rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 basket_client-1.1.0/src/basket/base.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 basket_client-1.1.0/src/basket/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basket_client-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    19526 2020-02-02 00:00:00.000000 basket_client-1.1.0/tests/test_client.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 basket_client-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 basket_client-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 basket_client-1.1.0/README.rst
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 basket_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 basket_client-1.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `basket-client-1.0.0/basket_client.egg-info/PKG-INFO` & `basket_client-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,61 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: basket-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python client for Mozilla's basket service.
-Home-page: https://github.com/mozilla/basket-client
-Author: Michael Kelly and contributors
-Author-email: dev-mozilla-org@lists.mozilla.org
-License: BSD
-Description: =============
-        Basket Client
-        =============
-        
-        This is a client for Mozilla's email subscription service,
-        basket. Basket is not a real subscription service, but it talks to a
-        real one and we don't really care who/what it is.
-        
-        .. image:: https://travis-ci.org/mozilla/basket-client.svg?branch=master
-            :target: https://travis-ci.org/mozilla/basket-client
-        .. image:: https://img.shields.io/pypi/v/basket-client.svg
-            :target: https://pypi.python.org/pypi/basket-client
-        
-        
-        Docs
-        ----
-        
-        Documentation can be found at http://basket-client.rtfd.org/
-        
-        
-        License
-        -------
-        
-        This software is licensed under the BSD License. For more information, read the file ``LICENSE``.
-        
-Keywords: mozilla,basket
-Platform: UNKNOWN
+Project-URL: Documentation, https://github.com/mozilla/basket-client#readme
+Project-URL: Issues, https://github.com/mozilla/basket-client/issues
+Project-URL: Source, https://github.com/mozilla/basket-client
+Author: Michael Kelly
+Maintainer: Paul McLanahan, Rob Hudson
+License: BSD-3-Clause
+License-File: LICENSE
+Keywords: basket,mozilla
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.8
+Requires-Dist: requests<3.0.0
+Description-Content-Type: text/x-rst
+
+=============
+Basket Client
+=============
+
+This is a client for Mozilla's email subscription service,
+`basket <https://basket.mozilla.org/>`_. Basket is not a real subscription service, but it talks to a
+real one and we don't really care who/what it is.
+
+|latest-version| |python-support| |build-status|
+
+.. |latest-version| image:: https://img.shields.io/pypi/v/basket-client.svg
+   :target: https://pypi.org/project/basket-client/
+   :alt: Latest version on PyPI
+
+.. |python-support| image:: https://img.shields.io/pypi/pyversions/basket-client
+   :target: https://pypi.org/project/basket-client/
+   :alt: Supported Python versions
+
+.. |build-status| image:: https://github.com/mozilla/basket-client/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/mozilla/basket-client/actions/workflows/test.yml
+   :alt: Build Status
+
+Docs
+----
+
+Documentation can be found at http://basket-client.rtfd.org/
+
+
+License
+-------
+
+This software is licensed under the BSD License. For more information, read the file ``LICENSE``.
```

### Comparing `basket-client-1.0.0/basket/tests.py` & `basket_client-1.1.0/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 import json
+import unittest
+from unittest.mock import ANY, Mock, patch
 
 from requests.exceptions import ConnectionError, Timeout
-from mock import ANY, Mock, patch
 
-from basket import (BasketException, confirm, confirm_email_change, debug_user,
-                    errors, get_newsletters, lookup_user, request, send_recovery_message,
-                    start_email_change, subscribe, send_sms,
-                    unsubscribe, update_user, user)
+from basket import (
+    BasketException,
+    confirm,
+    confirm_email_change,
+    debug_user,
+    errors,
+    get_newsletters,
+    lookup_user,
+    request,
+    send_recovery_message,
+    send_sms,
+    start_email_change,
+    subscribe,
+    unsubscribe,
+    update_user,
+    user,
+)
 from basket.base import basket_url, get_env_or_setting, parse_response
 
-import unittest
-
-
 # Warning: there are two request() methods, one in basket-client and
 # one in the requests library. Pay attention, it's very confusing.
 
-class TestBasketClient(unittest.TestCase):
 
+class TestBasketClient(unittest.TestCase):
     def test_basket_url_no_token(self):
         """Form basket URL properly when no token used"""
-        with patch('basket.base.BASKET_URL', new="BASKET_URL"):
+        with patch("basket.base.BASKET_URL", new="BASKET_URL"):
             result = basket_url("METHOD")
         self.assertEqual("BASKET_URL/news/METHOD/", result)
 
     def test_basket_url_with_token(self):
         """Form basket URL properly when token used"""
-        with patch('basket.base.BASKET_URL', new="BASKET_URL"):
+        with patch("basket.base.BASKET_URL", new="BASKET_URL"):
             result = basket_url("METHOD", "TOKEN")
         self.assertEqual("BASKET_URL/news/METHOD/TOKEN/", result)
 
     def test_response_not_200(self):
         """parse_response() raises exception on non-200 status code"""
         # and puts the status code on the exception
         res = Mock(status_code=666)
@@ -38,457 +49,407 @@
         except BasketException as e:
             self.assertEqual(666, e.status_code)
         else:
             self.fail("parse_response should have raised BasketException")
 
     def test_response_error(self):
         """parse_response() raises exception on status=error"""
-        content = json.dumps({'status': 'error', 'desc': 'ERROR', 'code': 3})
-        res = Mock(status_code=200, content=content,
-                   content_type='application/json')
+        content = json.dumps({"status": "error", "desc": "ERROR", "code": 3})
+        res = Mock(status_code=200, content=content, content_type="application/json")
         try:
             parse_response(res)
         except BasketException as e:
             self.assertEqual(3, e.code)
         else:
             self.fail("parse_response should have raised BasketException")
 
     def test_response_error_no_code(self):
         """if response has no code, and is error, then the code in
         the exception is the UNKNOWN code"""
-        content = json.dumps({'status': 'error', 'desc': 'ERROR'})
-        res = Mock(status_code=200, content=content,
-                   content_type='application/json')
+        content = json.dumps({"status": "error", "desc": "ERROR"})
+        res = Mock(status_code=200, content=content, content_type="application/json")
         try:
             parse_response(res)
         except BasketException as e:
             self.assertEqual(errors.BASKET_UNKNOWN_ERROR, e.code)
         else:
             self.fail("parse_response should have raised BasketException")
 
     def test_response_content(self):
         """parse_response() returns parsed response content if no error"""
-        data = {u'status': u'ok', u'foo': u'bar'}
+        data = {"status": "ok", "foo": "bar"}
         content = json.dumps(data)
-        res = Mock(status_code=200, content=content,
-                   content_type='application/json')
+        res = Mock(status_code=200, content=content, content_type="application/json")
         result = parse_response(res)
         self.assertEqual(data, result)
 
     def test_response_no_content_type(self):
         """parse_response() doesn't fail if the response is missing a content type"""
         # probably only an issue in testing, but still...
-        data = {u'status': u'ok', u'foo': u'bar'}
+        data = {"status": "ok", "foo": "bar"}
         content = json.dumps(data)
         res = Mock(status_code=200, content=content)
         result = parse_response(res)
         self.assertEqual(data, result)
 
     def test_request(self):
         """
         request() calls requests.request() with the expected parms
         if everything is normal, and returns the expected result.
         """
-        response_data = {u'status': u'ok', u'foo': u'bar'}
+        response_data = {"status": "ok", "foo": "bar"}
         action, method, token = "ACTION", "METHOD", "TOKEN"
         url = basket_url(action, token)
-        with patch('basket.base.requests.request', autospec=True) \
-                as request_call:
-            request_call.return_value = Mock(status_code=200,
-                                             content=json.dumps(response_data),
-                                             content_type='application/json')
-            result = request(method, action, data="DATA",
-                             token=token, params="PARAMS")
-
-        request_call.assert_called_with(method, url, data="DATA",
-                                        params="PARAMS", headers=None,
-                                        timeout=ANY)
+        with patch("basket.base.requests.request", autospec=True) as request_call:
+            request_call.return_value = Mock(status_code=200, content=json.dumps(response_data), content_type="application/json")
+            result = request(method, action, data="DATA", token=token, params="PARAMS")
+
+        request_call.assert_called_with(method, url, data="DATA", params="PARAMS", headers=None, timeout=ANY)
         self.assertEqual(response_data, result)
 
     def test_request_newsletters_string(self):
         """
         If request is passed newsletters as a string, newsletters is passed
         along unaltered.
         """
-        input_data = {'newsletters': 'one,two'}
+        input_data = {"newsletters": "one,two"}
         action, method, token = "ACTION", "METHOD", "TOKEN"
         url = basket_url(action, token)
-        content = {'one': 100, 'two': 200}
-        with patch('basket.base.requests.request', autospec=True) \
-                as request_call:
-            request_call.return_value = Mock(status_code=200,
-                                             content=json.dumps(content),
-                                             content_type='application/json')
-            result = request(method, action, data=input_data,
-                             token=token, params="PARAMS")
-
-        request_call.assert_called_with(method, url, data=input_data,
-                                        params="PARAMS", headers=None,
-                                        timeout=ANY)
+        content = {"one": 100, "two": 200}
+        with patch("basket.base.requests.request", autospec=True) as request_call:
+            request_call.return_value = Mock(status_code=200, content=json.dumps(content), content_type="application/json")
+            result = request(method, action, data=input_data, token=token, params="PARAMS")
+
+        request_call.assert_called_with(method, url, data=input_data, params="PARAMS", headers=None, timeout=ANY)
         self.assertEqual(content, result)
 
     def test_request_newsletters_non_string(self):
         """
         If request is passed newsletters as a non-string, newsletters is
         converted to a comma-separated string
         """
-        response_data = {u'status': u'ok', u'foo': u'bar'}
-        input_data = {'newsletters': ['one', 'two'], 'thing': 1}
+        response_data = {"status": "ok", "foo": "bar"}
+        input_data = {"newsletters": ["one", "two"], "thing": 1}
         expected_input_data = input_data.copy()
-        newsletters = ','.join(input_data['newsletters'])
-        expected_input_data['newsletters'] = newsletters
+        newsletters = ",".join(input_data["newsletters"])
+        expected_input_data["newsletters"] = newsletters
         action, method, token = "ACTION", "METHOD", "TOKEN"
         url = basket_url(action, token)
-        with patch('basket.base.requests.request', autospec=True) \
-                as request_call:
-            request_call.return_value = Mock(status_code=200,
-                                             content=json.dumps(response_data),
-                                             content_type='application/json')
-            result = request(method, action, data=input_data,
-                             token=token, params="PARAMS")
-
-        request_call.assert_called_with(method, url, data=expected_input_data,
-                                        params="PARAMS", headers=None,
-                                        timeout=ANY)
+        with patch("basket.base.requests.request", autospec=True) as request_call:
+            request_call.return_value = Mock(status_code=200, content=json.dumps(response_data), content_type="application/json")
+            result = request(method, action, data=input_data, token=token, params="PARAMS")
+
+        request_call.assert_called_with(method, url, data=expected_input_data, params="PARAMS", headers=None, timeout=ANY)
         self.assertEqual(response_data, result)
 
     def test_request_conn_error(self):
         """
         If requests throws a ConnectionError, it's converted to
         a BasketException
         """
-        input_data = {'newsletters': ['one', 'two'], 'thing': 1}
+        input_data = {"newsletters": ["one", "two"], "thing": 1}
         expected_input_data = input_data.copy()
-        newsletters = ','.join(input_data['newsletters'])
-        expected_input_data['newsletters'] = newsletters
+        newsletters = ",".join(input_data["newsletters"])
+        expected_input_data["newsletters"] = newsletters
         action, method, token = "ACTION", "METHOD", "TOKEN"
-        with patch('basket.base.requests.request', autospec=True) \
-                as request_call:
+        with patch("basket.base.requests.request", autospec=True) as request_call:
             request_call.side_effect = ConnectionError
             with self.assertRaises(BasketException):
-                request(method, action, data=input_data,
-                        token=token, params="PARAMS")
+                request(method, action, data=input_data, token=token, params="PARAMS")
 
     def test_request_timeout(self):
         """
         If requests times out, it's converted to
         a BasketException
         """
-        input_data = {'newsletters': ['one', 'two'], 'thing': 1}
+        input_data = {"newsletters": ["one", "two"], "thing": 1}
         expected_input_data = input_data.copy()
-        newsletters = ','.join(input_data['newsletters'])
-        expected_input_data['newsletters'] = newsletters
+        newsletters = ",".join(input_data["newsletters"])
+        expected_input_data["newsletters"] = newsletters
         action, method, token = "ACTION", "METHOD", "TOKEN"
-        with patch('basket.base.requests.request', autospec=True) \
-                as request_call:
+        with patch("basket.base.requests.request", autospec=True) as request_call:
             request_call.side_effect = Timeout
             with self.assertRaises(BasketException):
-                request(method, action, data=input_data,
-                        token=token, params="PARAMS")
+                request(method, action, data=input_data, token=token, params="PARAMS")
 
     def test_subscribe(self):
         """
         subscribe calls request with the expected parms and returns the result
         """
         email = "user1@example.com"
-        newsletters = ['news1', 'news2']
+        newsletters = ["news1", "news2"]
         kwargs = {
-            'arg1': 100,
-            'arg2': 200,
+            "arg1": 100,
+            "arg2": 200,
         }
         expected_kwargs = kwargs.copy()
-        expected_kwargs['email'] = email
-        expected_kwargs['newsletters'] = newsletters
-        with patch('basket.base.request', autospec=True) as request_call:
+        expected_kwargs["email"] = email
+        expected_kwargs["newsletters"] = newsletters
+        with patch("basket.base.request", autospec=True) as request_call:
             result = subscribe(email, newsletters, **kwargs)
 
-        request_call.assert_called_with('post', 'subscribe',
-                                        data=expected_kwargs,
-                                        headers={})
+        request_call.assert_called_with("post", "subscribe", data=expected_kwargs, headers={})
         self.assertEqual(request_call.return_value, result)
 
     def test_subscribe_sync_y_api_key_in_args(self):
         """
         subscribe calls request with the expected parms and returns the result
         when sync='Y', adds the API key from the args to the headers
         """
-        api_key = 'foo_bar'
+        api_key = "foo_bar"
         email = "user1@example.com"
-        newsletters = ['news1', 'news2']
+        newsletters = ["news1", "news2"]
         kwargs = {
-            'arg1': 100,
-            'arg2': 200,
-            'sync': 'Y',
-            'api_key': api_key,
+            "arg1": 100,
+            "arg2": 200,
+            "sync": "Y",
+            "api_key": api_key,
         }
         expected_kwargs = kwargs.copy()
-        expected_kwargs['email'] = email
-        expected_kwargs['newsletters'] = newsletters
-        del expected_kwargs['api_key']
-        with patch('basket.base.request', autospec=True) as request_call:
+        expected_kwargs["email"] = email
+        expected_kwargs["newsletters"] = newsletters
+        del expected_kwargs["api_key"]
+        with patch("basket.base.request", autospec=True) as request_call:
             result = subscribe(email, newsletters, **kwargs)
 
-        request_call.assert_called_with('post', 'subscribe',
-                                        data=expected_kwargs,
-                                        headers={'x-api-key': api_key})
+        request_call.assert_called_with("post", "subscribe", data=expected_kwargs, headers={"x-api-key": api_key})
         self.assertEqual(request_call.return_value, result)
 
     def test_subscribe_sync_y_api_key_not_in_args(self):
         """
         subscribe calls request with the expected parms and returns the result
         when sync='Y', adds the API key from the settings to the headers
         """
-        api_key = 'foo_bar'
+        api_key = "foo_bar"
         email = "user1@example.com"
-        newsletters = ['news1', 'news2']
+        newsletters = ["news1", "news2"]
         kwargs = {
-            'arg1': 100,
-            'arg2': 200,
-            'sync': 'Y',
+            "arg1": 100,
+            "arg2": 200,
+            "sync": "Y",
         }
         expected_kwargs = kwargs.copy()
-        expected_kwargs['email'] = email
-        expected_kwargs['newsletters'] = newsletters
-        with patch('basket.base.request', autospec=True) as request_call:
-            with patch('basket.base.BASKET_API_KEY', api_key):
+        expected_kwargs["email"] = email
+        expected_kwargs["newsletters"] = newsletters
+        with patch("basket.base.request", autospec=True) as request_call:
+            with patch("basket.base.BASKET_API_KEY", api_key):
                 result = subscribe(email, newsletters, **kwargs)
 
-        request_call.assert_called_with('post', 'subscribe',
-                                        data=expected_kwargs,
-                                        headers={'x-api-key': api_key})
+        request_call.assert_called_with("post", "subscribe", data=expected_kwargs, headers={"x-api-key": api_key})
         self.assertEqual(request_call.return_value, result)
 
     def test_unsubscribe(self):
         """
         unsubscribe calls request with the expected parms, returns the result
         """
         email = "user1@example.com"
-        newsletters = ['news1', 'news2']
+        newsletters = ["news1", "news2"]
         token = "TOKEN"
         optout = False
         expected_data = {
-            'email': email,
-            'newsletters': newsletters,
+            "email": email,
+            "newsletters": newsletters,
         }
-        with patch('basket.base.request', autospec=True) as request_call:
+        with patch("basket.base.request", autospec=True) as request_call:
             result = unsubscribe(token, email, newsletters, optout)
 
-        request_call.assert_called_with('post', 'unsubscribe',
-                                        data=expected_data,
-                                        token=token)
+        request_call.assert_called_with("post", "unsubscribe", data=expected_data, token=token)
         self.assertEqual(request_call.return_value, result)
 
     def test_unsubscribe_optout(self):
         """
         unsubscribe calls request with the expected parms and returns the
         result. optout is passed if true, instead of newsletters.
         """
         email = "user1@example.com"
-        newsletters = ['news1', 'news2']
+        newsletters = ["news1", "news2"]
         token = "TOKEN"
         optout = True
-        expected_data = {
-            'email': email,
-            'optout': 'Y'
-        }
-        with patch('basket.base.request', autospec=True) as request_call:
+        expected_data = {"email": email, "optout": "Y"}
+        with patch("basket.base.request", autospec=True) as request_call:
             result = unsubscribe(token, email, newsletters, optout)
 
-        request_call.assert_called_with('post', 'unsubscribe',
-                                        data=expected_data,
-                                        token=token)
+        request_call.assert_called_with("post", "unsubscribe", data=expected_data, token=token)
         self.assertEqual(request_call.return_value, result)
 
     def test_unsubscribe_bad_args(self):
         """
         unsubscribe must be passed newsletters or optout, or it raises
         BasketException
         """
         email = "user1@example.com"
         newsletters = None
         token = "TOKEN"
         optout = None
-        with patch('basket.base.request', autospec=True):
+        with patch("basket.base.request", autospec=True):
             with self.assertRaises(BasketException):
                 unsubscribe(token, email, newsletters, optout)
 
     def test_user(self):
         """
         user passes the expected args to request() and returns the result.
         """
         token = "TOKEN"
-        with patch('basket.base.request', autospec=True) as request_call:
+        with patch("basket.base.request", autospec=True) as request_call:
             result = user(token)
-        request_call.assert_called_with('get', 'user', token=token)
+        request_call.assert_called_with("get", "user", token=token)
         self.assertEqual(request_call.return_value, result)
 
     def test_update_user(self):
         """
         update_user passes the expected args to request(), returns the result.
         """
         token = "TOKEN"
         kwargs = {
-            'one': 100,
-            'two': 200,
+            "one": 100,
+            "two": 200,
         }
-        with patch('basket.base.request', autospec=True) as request_call:
+        with patch("basket.base.request", autospec=True) as request_call:
             result = update_user(token, **kwargs)
-        request_call.assert_called_with('post', 'user', data=kwargs,
-                                        token=token)
+        request_call.assert_called_with("post", "user", data=kwargs, token=token)
         self.assertEqual(request_call.return_value, result)
 
     def test_debug_user(self):
         """
         debug_user passes the expected args to request(), returns the result.
         """
         email = "user@example.com"
         supertoken = "STOKEN"
-        params = {'email': email, 'supertoken': supertoken}
-        with patch('basket.base.request', autospec=True) as request_call:
+        params = {"email": email, "supertoken": supertoken}
+        with patch("basket.base.request", autospec=True) as request_call:
             result = debug_user(email, supertoken)
-        request_call.assert_called_with('get', 'debug-user', params=params)
+        request_call.assert_called_with("get", "debug-user", params=params)
         self.assertEqual(request_call.return_value, result)
 
     def test_get_newsletters(self):
         """
         get_newsletters passes the expected args to request() and returns
         the 'newsletters' part of what it returns
         """
-        with patch('basket.base.request', autospec=True) as request_call:
-            request_call.return_value = {'newsletters': 'FOO BAR'}
+        with patch("basket.base.request", autospec=True) as request_call:
+            request_call.return_value = {"newsletters": "FOO BAR"}
             result = get_newsletters()
-        request_call.assert_called_with('get', 'newsletters')
-        self.assertEqual('FOO BAR', result)
+        request_call.assert_called_with("get", "newsletters")
+        self.assertEqual("FOO BAR", result)
 
     def test_confirm(self):
         """
         confirm() passes the expected args to request, and returns the result.
         """
         token = "TOKEN"
-        with patch('basket.base.request', autospec=True) as request_call:
+        with patch("basket.base.request", autospec=True) as request_call:
             result = confirm(token)
-        request_call.assert_called_with('post', 'confirm', token=token)
+        request_call.assert_called_with("post", "confirm", token=token)
         self.assertEqual(request_call.return_value, result)
 
     def test_send_recovery_email(self):
         """
         send_recovery_email() passes the expected args to request,
         and returns the result.
         """
         email = "dude@example.com"
-        with patch('basket.base.request', autospec=True) as mock_request:
+        with patch("basket.base.request", autospec=True) as mock_request:
             result = send_recovery_message(email)
-        data = {'email': email}
-        mock_request.assert_called_with('post', 'recover', data=data)
+        data = {"email": email}
+        mock_request.assert_called_with("post", "recover", data=data)
         self.assertEqual(mock_request.return_value, result)
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_lookup_user_token(self, mock_request):
         """Calling lookup_user with a token should not require an API key."""
-        lookup_user(token='TOKEN')
-        mock_request.assert_called_with('get', 'lookup-user',
-                                        params={'token': 'TOKEN'})
+        lookup_user(token="TOKEN")
+        mock_request.assert_called_with("get", "lookup-user", params={"token": "TOKEN"})
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_lookup_user_email(self, mock_request):
         """Calling lookup_user with email and api key should succeed."""
-        api_key = 'There is only XUL!'
-        email = 'dana@example.com'
+        api_key = "There is only XUL!"
+        email = "dana@example.com"
         lookup_user(email=email, api_key=api_key)
-        mock_request.assert_called_with('get', 'lookup-user',
-                                        params={'email': email},
-                                        headers={'x-api-key': api_key})
+        mock_request.assert_called_with("get", "lookup-user", params={"email": email}, headers={"x-api-key": api_key})
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_lookup_user_email_setting(self, mock_request):
         """Calling lookup_user with email and api key setting should succeed."""
-        api_key = 'There is only XUL!'
-        email = 'dana@example.com'
-        with patch('basket.base.BASKET_API_KEY', api_key):
+        api_key = "There is only XUL!"
+        email = "dana@example.com"
+        with patch("basket.base.BASKET_API_KEY", api_key):
             lookup_user(email=email)
-        mock_request.assert_called_with('get', 'lookup-user',
-                                        params={'email': email},
-                                        headers={'x-api-key': api_key})
+        mock_request.assert_called_with("get", "lookup-user", params={"email": email}, headers={"x-api-key": api_key})
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_lookup_user_no_api_key(self, mock_request):
         """Calling lookup_user with email and no api key raises an exception."""
         with self.assertRaises(BasketException):
-            lookup_user(email='dana@example.com')
+            lookup_user(email="dana@example.com")
 
         self.assertFalse(mock_request.called)
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_lookup_user_no_args(self, mock_request):
         """Calling lookup_user with no email or token raises an exception."""
         with self.assertRaises(BasketException):
             lookup_user()
 
         self.assertFalse(mock_request.called)
 
-    @patch('basket.base.settings',
-           type('X', (object,), {'TESTING_SETTINGS': True}))
+    @patch("basket.base.settings", type("X", (object,), {"TESTING_SETTINGS": True}))
     def test_gets_setting(self):
         """Should return the setting if it exists."""
-        self.assertEqual(get_env_or_setting('TESTING_SETTINGS'), True)
-        self.assertEqual(get_env_or_setting('DOES_NOT_EXIST'), None)
+        self.assertEqual(get_env_or_setting("TESTING_SETTINGS"), True)
+        self.assertEqual(get_env_or_setting("DOES_NOT_EXIST"), None)
 
     def test_get_setting_from_env(self):
         """Should always return the value from the env if it exists."""
-        self.assertEqual(get_env_or_setting('TESTING_SETTINGS'), None)
-        with patch('basket.base.settings',
-                   type('X', (object,), {'TESTING_SETTINGS': 'DUDE'})):
-            self.assertEqual(get_env_or_setting('TESTING_SETTINGS'), 'DUDE')
-            with patch.dict('os.environ', {'TESTING_SETTINGS': 'WALTER'}):
-                self.assertEqual(get_env_or_setting('TESTING_SETTINGS'),
-                                 'WALTER')
+        self.assertEqual(get_env_or_setting("TESTING_SETTINGS"), None)
+        with patch("basket.base.settings", type("X", (object,), {"TESTING_SETTINGS": "DUDE"})):
+            self.assertEqual(get_env_or_setting("TESTING_SETTINGS"), "DUDE")
+            with patch.dict("os.environ", {"TESTING_SETTINGS": "WALTER"}):
+                self.assertEqual(get_env_or_setting("TESTING_SETTINGS"), "WALTER")
 
     def test_start_email_change(self):
         """
         start_email_change() passes the expected args to request, and returns the result.
         """
         token = "TOKEN"
         new_email = "NEW EMAIL"
-        with patch('basket.base.request', autospec=True) as request_call:
+        with patch("basket.base.request", autospec=True) as request_call:
             result = start_email_change(token, new_email)
-        request_call.assert_called_with('post', 'start-email-change', token=token, data={'email': new_email})
+        request_call.assert_called_with("post", "start-email-change", token=token, data={"email": new_email})
         self.assertEqual(request_call.return_value, result)
 
     def test_confirm_email_change(self):
         """
         confirm_email_change() passes the expected args to request, and returns the result.
         """
         change_key = "CHANGE KEY"
-        with patch('basket.base.request', autospec=True) as request_call:
+        with patch("basket.base.request", autospec=True) as request_call:
             result = confirm_email_change(change_key)
-        request_call.assert_called_with('post', 'confirm-email-change', token=change_key)
+        request_call.assert_called_with("post", "confirm-email-change", token=change_key)
         self.assertEqual(request_call.return_value, result)
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_subscribe_source_ip(self, mock_request):
-        subscribe('dude@example.com', 'abiding-times', source_ip='1.1.1.1')
-        mock_request.assert_called_with('post', 'subscribe',
-                                        data={'email': 'dude@example.com',
-                                              'newsletters': 'abiding-times'},
-                                        headers={'x-source-ip': '1.1.1.1'})
+        subscribe("dude@example.com", "abiding-times", source_ip="1.1.1.1")
+        mock_request.assert_called_with(
+            "post", "subscribe", data={"email": "dude@example.com", "newsletters": "abiding-times"}, headers={"x-source-ip": "1.1.1.1"}
+        )
 
-    @patch('basket.base.request')
+    @patch("basket.base.request")
     def test_send_sms_source_ip(self, mock_request):
-        send_sms('5558675309', 'abide', source_ip='1.1.1.1')
-        mock_request.assert_called_with('post', 'subscribe_sms',
-                                        data={'mobile_number': '5558675309',
-                                              'msg_name': 'abide',
-                                              'optin': 'N'},
-                                        headers={'x-source-ip': '1.1.1.1'})
+        send_sms("5558675309", "abide", source_ip="1.1.1.1")
+        mock_request.assert_called_with(
+            "post", "subscribe_sms", data={"mobile_number": "5558675309", "msg_name": "abide", "optin": "N"}, headers={"x-source-ip": "1.1.1.1"}
+        )
 
-    @patch('basket.base.requests')
+    @patch("basket.base.requests")
     def test_mock_success(self, mock_requests):
-        result = subscribe('success@example.com', 'abiding-times')
-        self.assertEqual(result, {'status': 'ok'})
+        result = subscribe("success@example.com", "abiding-times")
+        self.assertEqual(result, {"status": "ok"})
         self.assertFalse(mock_requests.request.called)
 
-    @patch('basket.base.requests')
+    @patch("basket.base.requests")
     def test_mock_failure(self, mock_requests):
         with self.assertRaises(BasketException) as exc:
-            subscribe('failure@example.com', 'abiding-times')
+            subscribe("failure@example.com", "abiding-times")
         self.assertEqual(exc.exception.code, errors.BASKET_MOCK_FAILURE)
         self.assertFalse(mock_requests.request.called)
```

### Comparing `basket-client-1.0.0/basket/base.py` & `basket_client-1.1.0/src/basket/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import os
-import six
 
 # Use Django settings for BASKET_URL if available, but fall back to
 # env var or default if not. This lets us test without all the setup
 # that we'd otherwise need for Django.
 try:
     from django.conf import settings
 except (ImportError, AttributeError):
@@ -16,26 +15,25 @@
         # Django installed but not initialized
         settings = None
 
 import requests
 
 import basket.errors as errors
 
-
 log = logging.getLogger(__name__)
 
 
 def get_env_or_setting(name, default=None):
     """Return the value of name from an env var, a Django setting, or default"""
     return os.getenv(name, getattr(settings, name, default))
 
 
-BASKET_URL = get_env_or_setting('BASKET_URL', 'http://localhost:8000')
-BASKET_API_KEY = get_env_or_setting('BASKET_API_KEY', '')
-BASKET_TIMEOUT = get_env_or_setting('BASKET_TIMEOUT', 10)
+BASKET_URL = get_env_or_setting("BASKET_URL", "http://localhost:8000")
+BASKET_API_KEY = get_env_or_setting("BASKET_API_KEY", "")
+BASKET_TIMEOUT = get_env_or_setting("BASKET_TIMEOUT", 10)
 
 
 class BasketException(Exception):
     def __init__(self, *args, **kwargs):
         # Required kwargs:
         #
         # :param code: Basket error code (from basket/errors.py)
@@ -45,224 +43,211 @@
         # :param: First arg can be an English description of the error
         #
         # Optional kwargs:
         #
         # :param status_code: HTTP status code (e.g. 200, 400)
         # :param result: Whole decoded result from Basket
         #
-        self.status_code = kwargs.pop('status_code', 0)
+        self.status_code = kwargs.pop("status_code", 0)
         # `code` is a required kwarg, but if it's not there, better to
         # fake it and report the error than to blow up in the middle of error
         # handling.
-        self.code = kwargs.pop('code', errors.BASKET_UNKNOWN_ERROR)
-        self.result = kwargs.pop('result', {})
+        self.code = kwargs.pop("code", errors.BASKET_UNKNOWN_ERROR)
+        self.result = kwargs.pop("result", {})
         if args:
             self.desc = args[0]
         else:
-            self.desc = ''
-        super(BasketException, self).__init__(*args, **kwargs)
+            self.desc = ""
+        super().__init__(*args, **kwargs)
 
 
 class BasketNetworkException(BasketException):
     """Used on error connecting to basket"""
+
     def __init__(self, *args, **kwargs):
-        if 'code' not in kwargs:
-            kwargs['code'] = errors.BASKET_NETWORK_FAILURE
-        super(BasketNetworkException, self).__init__(*args, **kwargs)
+        if "code" not in kwargs:
+            kwargs["code"] = errors.BASKET_NETWORK_FAILURE
+        super().__init__(*args, **kwargs)
 
 
 def basket_url(method, token=None):
     """Form a basket API url. If the request requires a user-specific
     token, it is suffixed as the last part of the URL."""
 
-    token = '%s/' % token if token else ''
+    token = f"{token}/" if token else ""
 
-    return '%s/news/%s/%s' % (BASKET_URL, method, token)
+    return f"{BASKET_URL}/news/{method}/{token}"
 
 
 def parse_response(res):
     """Parse the result of a basket API call, raise exception on error"""
 
     # Parse the json and check for errors
     # We assume all basket calls respond with JSON (they're supposed to)
     result = {}
     try:
         result = json.loads(res.content)
     except Exception:
-        log.exception("Error parsing JSON returned by basket (%s)" % res.content)
+        log.exception(f"Error parsing JSON returned by basket ({res.content})")
 
-    if res.status_code != 200 or result.get('status', '') == 'error':
-        desc = result.get('desc', '%s request returned from basket: %s' %
-                                  (res.status_code, res.content))
-        raise BasketException(desc,
-                              status_code=res.status_code,
-                              code=result.get('code', errors.BASKET_UNKNOWN_ERROR),
-                              result=result)
+    if res.status_code != 200 or result.get("status", "") == "error":
+        desc = result.get("desc", f"{res.status_code} request returned from basket: {res.content}")
+        raise BasketException(desc, status_code=res.status_code, code=result.get("code", errors.BASKET_UNKNOWN_ERROR), result=result)
 
     return result
 
 
 def request(method, action, data=None, token=None, params=None, headers=None):
     """Call the basket API with the supplied http method and data."""
     # send mock response for testing email addresses (bug 1261886)
-    if data and 'email' in data:
-        if data['email'] == 'success@example.com':
-            return {'status': 'ok'}
-        elif data['email'] == 'failure@example.com':
-            raise BasketException('mock failure',
-                                  status_code=400,
-                                  code=errors.BASKET_MOCK_FAILURE)
+    if data and "email" in data:
+        if data["email"] == "success@example.com":
+            return {"status": "ok"}
+        elif data["email"] == "failure@example.com":
+            raise BasketException("mock failure", status_code=400, code=errors.BASKET_MOCK_FAILURE)
 
     # newsletters should be comma-delimited
-    if data and 'newsletters' in data:
-        if not isinstance(data['newsletters'], six.string_types):
-            data['newsletters'] = ','.join(data['newsletters'])
+    if data and "newsletters" in data:
+        if not isinstance(data["newsletters"], str):
+            data["newsletters"] = ",".join(data["newsletters"])
 
     try:
-        res = requests.request(method,
-                               basket_url(action, token),
-                               data=data,
-                               params=params,
-                               headers=headers,
-                               timeout=BASKET_TIMEOUT)
+        res = requests.request(method, basket_url(action, token), data=data, params=params, headers=headers, timeout=BASKET_TIMEOUT)
     except requests.exceptions.ConnectionError:
         raise BasketNetworkException("Error connecting to basket")
     except requests.exceptions.Timeout:
         raise BasketNetworkException("Timeout connecting to basket")
     return parse_response(res)
 
 
 # Public API methods
 
+
 def confirm(token):
     """
     Confirm a user.  token is required.
     """
-    return request('post', 'confirm', token=token)
+    return request("post", "confirm", token=token)
 
 
 def subscribe(email, newsletters, **kwargs):
     """Subscribe an email through basket to `newsletters`, which can
     be string or an array of newsletter names. Additional parameters
     should be passed as keyword arguments."""
 
     kwargs.update(email=email, newsletters=newsletters)
     headers = {}
-    if kwargs.get('sync', 'N') == 'Y':
-        api_key = kwargs.pop('api_key', BASKET_API_KEY)
+    if kwargs.get("sync", "N") == "Y":
+        api_key = kwargs.pop("api_key", BASKET_API_KEY)
         if not api_key:
-            raise BasketException('API key required for email lookup.',
-                                  code=errors.BASKET_AUTH_ERROR)
-        headers['x-api-key'] = api_key
+            raise BasketException("API key required for email lookup.", code=errors.BASKET_AUTH_ERROR)
+        headers["x-api-key"] = api_key
 
-    source_ip = kwargs.pop('source_ip', None)
+    source_ip = kwargs.pop("source_ip", None)
     if source_ip:
-        headers['x-source-ip'] = source_ip
+        headers["x-source-ip"] = source_ip
 
-    return request('post', 'subscribe', data=kwargs, headers=headers)
+    return request("post", "subscribe", data=kwargs, headers=headers)
 
 
 def send_sms(mobile_number, msg_name, optin=False, source_ip=None):
     """
     Send SMS message `msg_name` to `mobile_number` and optionally add the
     number to a list for future messages.
     """
     headers = {}
     if source_ip:
-        headers['x-source-ip'] = source_ip
+        headers["x-source-ip"] = source_ip
 
-    return request('post', 'subscribe_sms', data={
-        'mobile_number': mobile_number,
-        'msg_name': msg_name,
-        'optin': 'Y' if optin else 'N',
-    }, headers=headers)
+    return request(
+        "post",
+        "subscribe_sms",
+        data={
+            "mobile_number": mobile_number,
+            "msg_name": msg_name,
+            "optin": "Y" if optin else "N",
+        },
+        headers=headers,
+    )
 
 
 def unsubscribe(token, email, newsletters=None, optout=False):
     """Unsubscribe an email from certain newsletters, or all of them
     if `optout` is passed. Requires a token."""
 
-    data = {'email': email}
+    data = {"email": email}
 
     if optout:
-        data['optout'] = 'Y'
+        data["optout"] = "Y"
     elif newsletters:
-        data['newsletters'] = newsletters
+        data["newsletters"] = newsletters
     else:
-        raise BasketException('unsubscribe requires either a newsletters '
-                              'or optout parameter',
-                              code=errors.BASKET_USAGE_ERROR)
+        raise BasketException("unsubscribe requires either a newsletters or optout parameter", code=errors.BASKET_USAGE_ERROR)
 
-    return request('post', 'unsubscribe', data=data, token=token)
+    return request("post", "unsubscribe", data=data, token=token)
 
 
 def user(token):
     """Get all the information about a user. Requires a token."""
-    return request('get', 'user', token=token)
+    return request("get", "user", token=token)
 
 
 def update_user(token, **kwargs):
     """Update any fields for a user. Requires a token. If newsletters
     is passed, the user is only subscribed to those specific
     newsletters."""
 
-    return request('post', 'user', data=kwargs, token=token)
+    return request("post", "user", data=kwargs, token=token)
 
 
 def lookup_user(email=None, token=None, api_key=None):
     """Get a user's information using an API key or the user's token."""
     # prefer token
     if token:
-        return request('get', 'lookup-user', params={'token': token})
+        return request("get", "lookup-user", params={"token": token})
 
     if email:
         api_key = api_key or BASKET_API_KEY
         if not api_key:
-            raise BasketException('API key required for email lookup.',
-                                  code=errors.BASKET_AUTH_ERROR)
-        return request('get', 'lookup-user',
-                       params={'email': email},
-                       headers={'x-api-key': api_key})
+            raise BasketException("API key required for email lookup.", code=errors.BASKET_AUTH_ERROR)
+        return request("get", "lookup-user", params={"email": email}, headers={"x-api-key": api_key})
 
-    raise BasketException('Either token or email are required.',
-                          code=errors.BASKET_USAGE_ERROR)
+    raise BasketException("Either token or email are required.", code=errors.BASKET_USAGE_ERROR)
 
 
 def debug_user(email, supertoken):
     """Get a user's information using a supertoken only known by devs,
     useful for ensuring that data is being posted correctly"""
 
-    return request('get', 'debug-user',
-                   params={'email': email,
-                           'supertoken': supertoken})
+    return request("get", "debug-user", params={"email": email, "supertoken": supertoken})
 
 
 def send_recovery_message(email):
     """Send recovery message for this email"""
-    return request('post', 'recover', data={'email': email})
+    return request("post", "recover", data={"email": email})
 
 
 def get_newsletters():
     """Returns data about the newsletters that basket knows about.
     Format is a list of dictionaries.
     """
-    return request('get', 'newsletters')['newsletters']
+    return request("get", "newsletters")["newsletters"]
 
 
 def start_email_change(token, new_email):
     """
     Start the process of changing the email address for a user.
 
     :param token: User's subscriber token
     :param new_email: Desired new email address
     """
-    return request('post', 'start-email-change', data={'email': new_email}, token=token)
+    return request("post", "start-email-change", data={"email": new_email}, token=token)
 
 
 def confirm_email_change(change_key):
     """
     Confirm email change.
 
     Call this when a user hits the link they were given to confirm changing
     their email. The link includes the change_key in it.
     """
-    return request('post', 'confirm-email-change', token=change_key)
+    return request("post", "confirm-email-change", token=change_key)
```

### Comparing `basket-client-1.0.0/LICENSE` & `basket_client-1.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2011, Mozilla.
+Copyright (c) 2011, Mozilla Foundation.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice,
        this list of conditions and the following disclaimer.
```

### Comparing `basket-client-1.0.0/README.rst` & `basket_client-1.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 =============
 Basket Client
 =============
 
 This is a client for Mozilla's email subscription service,
-basket. Basket is not a real subscription service, but it talks to a
+`basket <https://basket.mozilla.org/>`_. Basket is not a real subscription service, but it talks to a
 real one and we don't really care who/what it is.
 
-.. image:: https://travis-ci.org/mozilla/basket-client.svg?branch=master
-    :target: https://travis-ci.org/mozilla/basket-client
-.. image:: https://img.shields.io/pypi/v/basket-client.svg
-    :target: https://pypi.python.org/pypi/basket-client
+|latest-version| |python-support| |build-status|
 
+.. |latest-version| image:: https://img.shields.io/pypi/v/basket-client.svg
+   :target: https://pypi.org/project/basket-client/
+   :alt: Latest version on PyPI
+
+.. |python-support| image:: https://img.shields.io/pypi/pyversions/basket-client
+   :target: https://pypi.org/project/basket-client/
+   :alt: Supported Python versions
+
+.. |build-status| image:: https://github.com/mozilla/basket-client/actions/workflows/test.yml/badge.svg
+   :target: https://github.com/mozilla/basket-client/actions/workflows/test.yml
+   :alt: Build Status
 
 Docs
 ----
 
 Documentation can be found at http://basket-client.rtfd.org/
```

