# Comparing `tmp/tap_googlemeet-0.0.1.tar.gz` & `tmp/tap_googlemeet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_googlemeet-0.0.1.tar", max compression
+gzip compressed data, was "tap_googlemeet-0.0.2.tar", max compression
```

## Comparing `tap_googlemeet-0.0.1.tar` & `tap_googlemeet-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11344 2023-07-14 13:29:25.916144 tap_googlemeet-0.0.1/LICENSE
--rw-r--r--   0        0        0     3112 2023-07-14 13:29:25.911520 tap_googlemeet-0.0.1/README.md
--rw-r--r--   0        0        0     1297 2023-07-14 15:21:02.213123 tap_googlemeet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-14 13:29:25.923657 tap_googlemeet-0.0.1/tap_googlemeet/__init__.py
--rw-r--r--   0        0        0     3311 2023-07-14 15:53:05.470774 tap_googlemeet-0.0.1/tap_googlemeet/client.py
--rw-r--r--   0        0        0     4434 2023-07-14 14:42:43.146306 tap_googlemeet-0.0.1/tap_googlemeet/schemas/call_ended.json
--rw-r--r--   0        0        0      767 2023-07-14 15:33:31.082492 tap_googlemeet-0.0.1/tap_googlemeet/secrets_manager.py
--rw-r--r--   0        0        0      432 2023-07-14 14:32:59.890024 tap_googlemeet-0.0.1/tap_googlemeet/streams.py
--rw-r--r--   0        0        0     1110 2023-07-14 15:31:03.732556 tap_googlemeet-0.0.1/tap_googlemeet/tap.py
--rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 tap_googlemeet-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-07-14 13:29:25.916144 tap_googlemeet-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3112 2023-07-14 13:29:25.911520 tap_googlemeet-0.0.2/README.md
+-rw-r--r--   0        0        0     1297 2023-07-14 16:05:07.678068 tap_googlemeet-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-14 13:29:25.923657 tap_googlemeet-0.0.2/tap_googlemeet/__init__.py
+-rw-r--r--   0        0        0     3312 2023-07-14 16:04:49.092213 tap_googlemeet-0.0.2/tap_googlemeet/client.py
+-rw-r--r--   0        0        0     4434 2023-07-14 14:42:43.146306 tap_googlemeet-0.0.2/tap_googlemeet/schemas/call_ended.json
+-rw-r--r--   0        0        0      767 2023-07-14 15:33:31.082492 tap_googlemeet-0.0.2/tap_googlemeet/secrets_manager.py
+-rw-r--r--   0        0        0      432 2023-07-14 14:32:59.890024 tap_googlemeet-0.0.2/tap_googlemeet/streams.py
+-rw-r--r--   0        0        0     1110 2023-07-14 15:31:03.732556 tap_googlemeet-0.0.2/tap_googlemeet/tap.py
+-rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 tap_googlemeet-0.0.2/PKG-INFO
```

### Comparing `tap_googlemeet-0.0.1/LICENSE` & `tap_googlemeet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_googlemeet-0.0.1/README.md` & `tap_googlemeet-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_googlemeet-0.0.1/pyproject.toml` & `tap_googlemeet-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-googlemeet"
-version = "0.0.1"
+version = "0.0.2"
 description = "`tap-googlemeet` is a Singer tap for GoogleMeet, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Hidde Stokvis"]
 keywords = [
     "ELT",
     "GoogleMeet",
 ]
```

### Comparing `tap_googlemeet-0.0.1/tap_googlemeet/client.py` & `tap_googlemeet-0.0.2/tap_googlemeet/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     creds = Credentials.from_authorized_user_info(config, SCOPES)
     if not creds or not creds.valid:
         if creds and creds.expired and creds.refresh_token:
             creds.refresh(Request())
         else:
             flow = InstalledAppFlow.from_client_config(config, scopes=SCOPES)
             creds = flow.run_local_server(port=0)
-        update_secret(creds, sectret_id)
+        update_secret(config, sectret_id)
     return creds
 
 class GoogleMeetStream(Stream):
     """GoogleMeet stream class."""
     _credentials = None
 
     def get_records(self, context: dict | None):
```

### Comparing `tap_googlemeet-0.0.1/tap_googlemeet/schemas/call_ended.json` & `tap_googlemeet-0.0.2/tap_googlemeet/schemas/call_ended.json`

 * *Files identical despite different names*

### Comparing `tap_googlemeet-0.0.1/tap_googlemeet/secrets_manager.py` & `tap_googlemeet-0.0.2/tap_googlemeet/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `tap_googlemeet-0.0.1/tap_googlemeet/tap.py` & `tap_googlemeet-0.0.2/tap_googlemeet/tap.py`

 * *Files identical despite different names*

### Comparing `tap_googlemeet-0.0.1/PKG-INFO` & `tap_googlemeet-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-googlemeet
-Version: 0.0.1
+Version: 0.0.2
 Summary: `tap-googlemeet` is a Singer tap for GoogleMeet, built with the Meltano Singer SDK.
 License: Apache-2.0
 Keywords: ELT,GoogleMeet
 Author: Hidde Stokvis
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

