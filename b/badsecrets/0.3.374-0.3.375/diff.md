# Comparing `tmp/badsecrets-0.3.374.tar.gz` & `tmp/badsecrets-0.3.375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.3.374.tar", max compression
+gzip compressed data, was "badsecrets-0.3.375.tar", max compression
```

## Comparing `badsecrets-0.3.374.tar` & `badsecrets-0.3.375.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    35149 2023-07-11 04:16:58.264845 badsecrets-0.3.374/LICENSE
--rw-r--r--   0        0        0    31849 2023-07-11 04:16:58.264845 badsecrets-0.3.374/README.md
--rw-r--r--   0        0        0      711 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/__init__.py
--rw-r--r--   0        0        0     6986 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4210 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     7875 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3544 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     5076 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0    10204 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0      986 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2022 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0     1057 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     4057 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    14819 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2172 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1931 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3077 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2932 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4949 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     3718 2023-07-11 04:16:58.264845 badsecrets-0.3.374/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654096 2023-07-11 04:16:58.272845 badsecrets-0.3.374/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-07-11 04:16:58.272845 badsecrets-0.3.374/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-07-11 04:16:58.272845 badsecrets-0.3.374/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-07-11 04:16:58.292845 badsecrets-0.3.374/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      957 2023-07-11 04:17:28.720888 badsecrets-0.3.374/pyproject.toml
--rw-r--r--   0        0        0    32703 1970-01-01 00:00:00.000000 badsecrets-0.3.374/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 15:15:16.938012 badsecrets-0.3.375/LICENSE
+-rw-r--r--   0        0        0    31950 2023-07-14 15:15:16.938012 badsecrets-0.3.375/README.md
+-rw-r--r--   0        0        0      711 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/__init__.py
+-rw-r--r--   0        0        0     6986 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4210 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     7875 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     5076 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0    10204 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0      986 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2022 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/express_signedcookies.py
+-rw-r--r--   0        0        0     1057 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4057 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14819 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2172 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1931 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3077 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2932 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     4949 2023-07-14 15:15:16.938012 badsecrets-0.3.375/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3718 2023-07-14 15:15:16.942012 badsecrets-0.3.375/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654096 2023-07-14 15:15:16.946012 badsecrets-0.3.375/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-07-14 15:15:16.946012 badsecrets-0.3.375/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-07-14 15:15:16.946012 badsecrets-0.3.375/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-07-14 15:15:16.962013 badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-07-14 15:15:16.966013 badsecrets-0.3.375/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-07-14 15:15:39.318575 badsecrets-0.3.375/pyproject.toml
+-rw-r--r--   0        0        0    32804 1970-01-01 00:00:00.000000 badsecrets-0.3.375/PKG-INFO
```

### Comparing `badsecrets-0.3.374/LICENSE` & `badsecrets-0.3.375/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/README.md` & `badsecrets-0.3.375/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 <p align="left"><img width="300" height="300" src="https://user-images.githubusercontent.com/24899338/223151619-6859bc93-1fe2-47c7-86a6-ecaa6b495ece.png"></p>
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![License](https://img.shields.io/badge/license-GPLv3-f126ea.svg)
 ![Tests](https://github.com/blacklanternsecurity/badsecrets/actions/workflows/tests.yaml/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/blacklanternsecurity/badsecrets/branch/main/graph/badge.svg?token=2PAE7NUM07)](https://codecov.io/gh/blacklanternsecurity/badsecrets)
+[![Pypi Downloads](https://img.shields.io/pypi/dm/badsecrets)](https://pypi.org/project/badsecrets)
+
 
 A pure python library for identifying the use of known or very weak cryptographic secrets across a variety of platforms. The project is designed to be both a repository of various "known secrets" (for example, ASP.NET machine keys found in examples in tutorials), and to provide a language-agnostic abstraction layer for identifying their use.  
 
 Knowing when a 'bad secret' was used is usually a matter of examining some cryptographic product in which the secret was used: for example, a cookie which is signed with a keyed hashing algorithm. Things can get complicated when you dive into the individual implementation oddities each platform provides, which this library aims to alleviate. 
 
 Check out our full [blog post](https://blog.blacklanternsecurity.com/p/introducing-badsecrets) on the Black Lantern Security blog!
```

### Comparing `badsecrets-0.3.374/badsecrets/__init__.py` & `badsecrets-0.3.375/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/base.py` & `badsecrets-0.3.375/badsecrets/base.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/examples/blacklist3r.py` & `badsecrets-0.3.375/badsecrets/examples/blacklist3r.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/examples/cli.py` & `badsecrets-0.3.375/badsecrets/examples/cli.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/examples/symfony_knownkey.py` & `badsecrets-0.3.375/badsecrets/examples/symfony_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.3.375/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/helpers.py` & `badsecrets-0.3.375/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.3.375/badsecrets/modules/aspnet_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.3.375/badsecrets/modules/django_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.3.375/badsecrets/modules/express_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.3.375/badsecrets/modules/flask_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/generic_jwt.py` & `badsecrets-0.3.375/badsecrets/modules/generic_jwt.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.3.375/badsecrets/modules/jsf_viewstate.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.3.375/badsecrets/modules/laravel_signedcookies.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/peoplesoft_pstoken.py` & `badsecrets-0.3.375/badsecrets/modules/peoplesoft_pstoken.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.3.375/badsecrets/modules/rails_secretkeybase.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.3.375/badsecrets/modules/symfony_signedurl.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.3.375/badsecrets/modules/telerik_encryptionkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.3.375/badsecrets/modules/telerik_hashkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.3.375/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.3.375/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.3.375/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.3.375/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.3.375/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.3.375/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.3.375/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.3.375/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.3.375/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.3.375/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.3.375/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.3.375/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.3.375/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.3.374/pyproject.toml` & `badsecrets-0.3.375/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.3.374"
+version = "v0.3.375"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
```

### Comparing `badsecrets-0.3.374/PKG-INFO` & `badsecrets-0.3.375/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.3.374
+Version: 0.3.375
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -24,14 +24,16 @@
 
 <p align="left"><img width="300" height="300" src="https://user-images.githubusercontent.com/24899338/223151619-6859bc93-1fe2-47c7-86a6-ecaa6b495ece.png"></p>
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![License](https://img.shields.io/badge/license-GPLv3-f126ea.svg)
 ![Tests](https://github.com/blacklanternsecurity/badsecrets/actions/workflows/tests.yaml/badge.svg?branch=main)
 [![codecov](https://codecov.io/gh/blacklanternsecurity/badsecrets/branch/main/graph/badge.svg?token=2PAE7NUM07)](https://codecov.io/gh/blacklanternsecurity/badsecrets)
+[![Pypi Downloads](https://img.shields.io/pypi/dm/badsecrets)](https://pypi.org/project/badsecrets)
+
 
 A pure python library for identifying the use of known or very weak cryptographic secrets across a variety of platforms. The project is designed to be both a repository of various "known secrets" (for example, ASP.NET machine keys found in examples in tutorials), and to provide a language-agnostic abstraction layer for identifying their use.  
 
 Knowing when a 'bad secret' was used is usually a matter of examining some cryptographic product in which the secret was used: for example, a cookie which is signed with a keyed hashing algorithm. Things can get complicated when you dive into the individual implementation oddities each platform provides, which this library aims to alleviate. 
 
 Check out our full [blog post](https://blog.blacklanternsecurity.com/p/introducing-badsecrets) on the Black Lantern Security blog!
```

