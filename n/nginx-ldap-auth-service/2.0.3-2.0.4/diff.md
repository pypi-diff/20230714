# Comparing `tmp/nginx-ldap-auth-service-2.0.3.tar.gz` & `tmp/nginx-ldap-auth-service-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-ldap-auth-service-2.0.3.tar", last modified: Wed Jul 12 00:22:45 2023, max compression
+gzip compressed data, was "nginx-ldap-auth-service-2.0.4.tar", last modified: Fri Jul 14 17:39:23 2023, max compression
```

## Comparing `nginx-ldap-auth-service-2.0.3.tar` & `nginx-ldap-auth-service-2.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.348319 nginx-ldap-auth-service-2.0.3/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.3/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.3/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     1645 2023-07-12 00:22:38.000000 nginx-ldap-auth-service-2.0.3/Makefile
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-12 00:22:45.349052 nginx-ldap-auth-service-2.0.3/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.3/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.307444 nginx-ldap-auth-service-2.0.3/etc/
--rw-r--r--   0 cmalek     (501) admin       (80)      687 2023-07-12 00:20:30.000000 nginx-ldap-auth-service-2.0.3/etc/environment.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.308999 nginx-ldap-auth-service-2.0.3/etc/nginx/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.312670 nginx-ldap-auth-service-2.0.3/etc/nginx/certs/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.crt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.key
--rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.3/etc/nginx/nginx.conf
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.325183 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/
--rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-12 00:22:38.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.332287 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/
--rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3635 2023-07-12 00:14:38.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     7143 2023-07-12 00:14:51.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/main.py
--rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/middleware.py
--rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-12 00:21:31.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/models.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.338088 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/
--rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/cli.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-12 00:06:35.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/server.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/ldap.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/logging.py
--rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/main.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4522 2023-07-11 20:24:02.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/types.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-12 00:22:45.346622 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-12 00:22:45.000000 nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      628 2023-05-26 19:08:43.000000 nginx-ldap-auth-service-2.0.3/requirements.dev.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-12 00:22:45.355388 nginx-ldap-auth-service-2.0.3/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-12 00:22:38.000000 nginx-ldap-auth-service-2.0.3/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.255685 nginx-ldap-auth-service-2.0.4/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1453 2023-05-26 19:55:10.000000 nginx-ldap-auth-service-2.0.4/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       54 2023-05-25 16:57:03.000000 nginx-ldap-auth-service-2.0.4/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1706 2023-07-14 17:39:18.000000 nginx-ldap-auth-service-2.0.4/Makefile
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-14 17:39:23.256192 nginx-ldap-auth-service-2.0.4/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      568 2023-07-11 23:13:44.000000 nginx-ldap-auth-service-2.0.4/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.226056 nginx-ldap-auth-service-2.0.4/etc/
+-rw-r--r--   0 cmalek     (501) admin       (80)      716 2023-07-14 17:10:58.000000 nginx-ldap-auth-service-2.0.4/etc/environment.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.227427 nginx-ldap-auth-service-2.0.4/etc/nginx/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.229831 nginx-ldap-auth-service-2.0.4/etc/nginx/certs/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1127 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.crt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1708 2023-05-25 17:12:21.000000 nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.key
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4599 2023-07-11 20:39:31.000000 nginx-ldap-auth-service-2.0.4/etc/nginx/nginx.conf
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.237480 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      217 2023-07-14 17:39:18.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.243909 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/
+-rw-rw-r--   0 cmalek     (501) admin       (80)        0 2023-05-25 15:43:10.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3635 2023-07-12 00:14:38.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     7601 2023-07-14 17:31:00.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/main.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     4706 2023-07-07 23:31:10.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/middleware.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     9652 2023-07-12 00:21:31.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/models.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.248676 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       74 2023-05-25 15:49:09.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      419 2023-07-10 16:58:38.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/cli.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2198 2023-07-12 00:06:35.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/server.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     3378 2023-07-08 00:06:11.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/ldap.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5010 2023-07-10 23:25:53.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/logging.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      179 2023-07-10 17:22:33.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/main.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5746 2023-07-14 17:23:15.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      147 2023-05-25 18:28:56.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/types.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-14 17:39:23.254953 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1624 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)      865 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       62 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      270 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       16 2023-07-14 17:39:23.000000 nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      634 2023-07-12 16:14:11.000000 nginx-ldap-auth-service-2.0.4/requirements.dev.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      518 2023-07-14 17:39:23.259392 nginx-ldap-auth-service-2.0.4/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1927 2023-07-14 17:39:18.000000 nginx-ldap-auth-service-2.0.4/setup.py
```

### Comparing `nginx-ldap-auth-service-2.0.3/LICENSE.txt` & `nginx-ldap-auth-service-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/Makefile` & `nginx-ldap-auth-service-2.0.4/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = 2.0.3
+VERSION = 2.0.4
 
 PACKAGE = nginx-ldap-auth-service
 
 DOCKER_REGISTRY = caltechads
 #======================================================================
 
 
@@ -24,15 +24,16 @@
 	docker tag ${PACKAGE}:${VERSION} ${PACKAGE}:latest
 
 tag:
 	docker tag ${PACKAGE}:${VERSION} ${DOCKER_REGISTRY}/${PACKAGE}:${VERSION}
 	docker tag ${PACKAGE}:latest ${DOCKER_REGISTRY}/${PACKAGE}:latest
 
 push: tag
-	docker push ${DOCKER_REGISTRY}/${PACKAGE}
+	docker push ${DOCKER_REGISTRY}/${PACKAGE}:latest
+	docker push ${DOCKER_REGISTRY}/${PACKAGE}:${VERSION}
 
 pull:
 	docker pull ${DOCKER_REGISTRY}/${PACKAGE}:${VERSION}
 
 dev:
 	docker-compose up
```

### Comparing `nginx-ldap-auth-service-2.0.3/PKG-INFO` & `nginx-ldap-auth-service-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.3
+Version: 2.0.4
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.3/README.md` & `nginx-ldap-auth-service-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/etc/environment.txt` & `nginx-ldap-auth-service-2.0.4/etc/environment.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LDAP_BINDDN=__LDAP_BINDDN__
 LDAP_PASSWORD=__LDAP_PASSWORD__
 LDAP_BASEDN=ou=users,dc=example,dc=com
 # SENTRY_URL=None
 
 # COOKIE_NAME=nginxauth
 # SESSION_MAX_AGE=0
+# USE_ROLLING_SESSIONS=False
 # SESSION_BACKEND=memory
 # REDIS_URL=redis://localhost
 # REDIS_PREFIX=nginx_ldap_auth.
 # LDAP_STARTTLS=True
 # LDAP_DISABLE_REFERRALS=False
 # LDAP_USERNAME_ATTRIBUTE=uid
 # LDAP_FULL_NAME_ATTRIBUTE=cn
```

### Comparing `nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.crt` & `nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.crt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/etc/nginx/certs/localhost.key` & `nginx-ldap-auth-service-2.0.4/etc/nginx/certs/localhost.key`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/etc/nginx/nginx.conf` & `nginx-ldap-auth-service-2.0.4/etc/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/forms.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/forms.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/main.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import os
+from typing import cast
 
 from fastapi import FastAPI, Request, Response, status
 from fastapi.responses import HTMLResponse, RedirectResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
+from pydantic import AnyUrl
 from starsessions import (
     InMemoryStore,
     SessionStore,
     load_session,
     get_session_handler,
 )
 from starsessions.stores.redis import RedisStore
@@ -34,25 +36,28 @@
 
 # --------------------------------------
 # Session Store
 # --------------------------------------
 
 if settings.session_backend == "memory":
     store: SessionStore = InMemoryStore()
+    get_logger().info("session.store", backend=settings.session_backend)
 elif settings.session_backend == "redis":
     store = RedisStore(
-        settings.redis_url,
+        str(settings.redis_url),
         prefix=settings.redis_prefix,
         gc_ttl=settings.session_max_age
     )
+    redis_url = cast(AnyUrl, settings.redis_url)
     get_logger().info(
         "session.store",
         backend=settings.session_backend,
-        server=settings.redis_url,
-        max_age=settings.session_max_age
+        server=redis_url.host,
+        port=redis_url.port,
+        db=redis_url.path,
     )
 
 
 # --------------------------------------
 # The FastAPI app
 # --------------------------------------
 
@@ -64,14 +69,22 @@
 app.mount("/auth/static", StaticFiles(directory=static_dir), name="static")
 app.add_middleware(
     SessionMiddleware,
     store=store,
     cookie_name=settings.cookie_name,
     lifetime=settings.session_max_age
 )
+get_logger().info(
+    "session.setup.complete",
+    backend=settings.session_backend,
+    cookie_name=settings.cookie_name,
+    cookie_domain=settings.cookie_domain,
+    max_age=settings.session_max_age,
+    rolling=settings.use_rolling_session
+)
 templates = Jinja2Templates(directory=templates_dir)
 
 
 # --------------------------------------
 # Startup and Shutdown Events
 # --------------------------------------
 
@@ -218,15 +231,15 @@
         await load_session(request)
         if request.session.get("username"):
             # We have a valid session
             if not await User.objects.get(request.session["username"]):
                 # The user does not exist in LDAP; log them out
                 await kill_session(request)
             if not await User.objects.is_authorized(request.session["username"]):
-                # The user is not authorized
+                # The user is no longer authorized; log them out
                 await kill_session(request)
             return {}
         else:
             # Destroy the session because it is not valid
             await kill_session(request)
     # Force the user to authenticate
     response.headers["Cache-Control"] = "no-cache"
```

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/middleware.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/middleware.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/app/models.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/app/models.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/cli/server.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/cli/server.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/ldap.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/ldap.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth/logging.py` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth/logging.py`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/PKG-INFO` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-ldap-auth-service
-Version: 2.0.3
+Version: 2.0.4
 Summary: A FastAPI app that authenticates users via LDAP and sets a cookie for nginx
 Home-page: https://github.com/caltechads/nginx-ldap-auth-service
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: nginx,ldap,auth,fastapi,devops
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nginx-ldap-auth-service-2.0.3/nginx_ldap_auth_service.egg-info/SOURCES.txt` & `nginx-ldap-auth-service-2.0.4/nginx_ldap_auth_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/requirements.dev.txt` & `nginx-ldap-auth-service-2.0.4/requirements.dev.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 -e .
 -r doc/requirements.txt
 
 # Deployment
 # ------------------------------------------------------------------------------
 bumpversion==0.6.0                            # https://github.com/peritus/bumpversion
+twine
 
 # Development
 # ------------------------------------------------------------------------------
 flake8                                        # https://github.com/PyCQA/flake8
 pylint                                        # https://github.com/pylint-dev/pylint
 mypy                                          # https://github.com/python/mypy
 black                                         # https://github.com/psf/black
```

### Comparing `nginx-ldap-auth-service-2.0.3/setup.cfg` & `nginx-ldap-auth-service-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nginx-ldap-auth-service-2.0.3/setup.py` & `nginx-ldap-auth-service-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setup(
     name="nginx-ldap-auth-service",
-    version="2.0.3",
+    version="2.0.4",
     description="A FastAPI app that authenticates users via LDAP and sets a cookie for nginx",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     url="https://github.com/caltechads/nginx-ldap-auth-service",
     packages=find_packages(exclude=["bin"]),
     install_requires=[
         "aiodogstatsd==0.16.0.post0",
```

