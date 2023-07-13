# Comparing `tmp/adafri-0.0.18.tar.gz` & `tmp/adafri-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.18.tar", last modified: Thu Jul 13 22:03:34 2023, max compression
+gzip compressed data, was "adafri-0.0.19.tar", last modified: Thu Jul 13 22:31:39 2023, max compression
```

## Comparing `adafri-0.0.18.tar` & `adafri-0.0.19.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.396331 adafri-0.0.18/
--rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 22:03:34.395977 adafri-0.0.18/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.368210 adafri-0.0.18/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.18/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.373690 adafri-0.0.18/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.18/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.18/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.18/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.374560 adafri-0.0.18/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.18/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.375683 adafri-0.0.18/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.18/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.378416 adafri-0.0.18/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.18/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.18/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.18/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.379344 adafri-0.0.18/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.18/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.381029 adafri-0.0.18/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.18/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.18/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.381849 adafri-0.0.18/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.18/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.382207 adafri-0.0.18/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.18/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.389332 adafri-0.0.18/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6354 2023-07-13 21:14:52.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9437 2023-07-13 22:02:43.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9023 2023-07-13 21:53:10.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.18/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.391456 adafri-0.0.18/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.18/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.18/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.392206 adafri-0.0.18/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.18/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.394993 adafri-0.0.18/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.18/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.18/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.18/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:03:34.371198 adafri-0.0.18/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 22:03:34.000000 adafri-0.0.18/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 22:03:34.000000 adafri-0.0.18/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 22:03:34.000000 adafri-0.0.18/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 22:03:34.000000 adafri-0.0.18/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 22:03:34.396523 adafri-0.0.18/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 22:03:27.000000 adafri-0.0.18/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.342717 adafri-0.0.19/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 22:31:39.342179 adafri-0.0.19/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.316654 adafri-0.0.19/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.19/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.321310 adafri-0.0.19/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.322122 adafri-0.0.19/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.19/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.322905 adafri-0.0.19/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.325386 adafri-0.0.19/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.326331 adafri-0.0.19/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.19/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.327809 adafri-0.0.19/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.328849 adafri-0.0.19/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.329234 adafri-0.0.19/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.19/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.334887 adafri-0.0.19/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6354 2023-07-13 21:14:52.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9437 2023-07-13 22:02:43.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9027 2023-07-13 22:31:10.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.336907 adafri-0.0.19/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.337785 adafri-0.0.19/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.340682 adafri-0.0.19/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-13 22:31:39.319043 adafri-0.0.19/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      493 2023-07-13 22:31:39.000000 adafri-0.0.19/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-13 22:31:39.000000 adafri-0.0.19/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-13 22:31:39.000000 adafri-0.0.19/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-13 22:31:39.000000 adafri-0.0.19/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-13 22:31:39.342890 adafri-0.0.19/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1007 2023-07-13 22:31:32.000000 adafri-0.0.19/setup.py
```

### Comparing `adafri-0.0.18/adafri/utils/response.py` & `adafri-0.0.19/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/utils/utils.py` & `adafri-0.0.19/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/account/models/account.py` & `adafri-0.0.19/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19/adafri/v1/auth/oauth/models/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("name required","INVALID_REQUEST", 1));
 
         token_model.id = Crypto().generate_id(token_model.access_token+"~"+token_model.client_id);
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, token_model, None);
     
 
     def save(self, token, request):
-        model = {**token, "client_id": request.client.client_id, "uid": request.user.uid}
+        model = {**token, "client_id": request.client.client_id, "uid": request.client.uid}
         token_generate = OAuthToken.generate(**model);
         if token_generate.status == ResponseStatus.ERROR:
             return token_generate
         docRef = OAuthToken(token_generate.data.to_json()).document_reference();
         if docRef.get().exists:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Location with name {token_generate.data.id} already exist","INVALID_REQUEST", 1));
         
@@ -183,13 +183,13 @@
 DEFAULT_EXPIRES_IN = 3600
 class TokenGenerator(BearerTokenGenerator):
     @staticmethod
     def generate(grant_type, client, user=None, scope=None, expires_in=None, include_refresh_token=True):
         if expires_in is None:
             expires_in = DEFAULT_EXPIRES_IN
         expires_at = datetime.now() + timedelta(seconds=DEFAULT_EXPIRES_IN)
-        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": user.uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
+        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": client.uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
         access_token = Crypto().generate_token("access_token~"+json.dumps(token));
         token['access_token'] = access_token;
         if include_refresh_token:
             token['refresh_token'] = Crypto().generate_token("refresh_token~"+json.dumps(token));
         return token
```

### Comparing `adafri-0.0.18/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/user/models/user.py` & `adafri-0.0.19/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.18/setup.py` & `adafri-0.0.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.18' 
+VERSION = '0.0.19' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

