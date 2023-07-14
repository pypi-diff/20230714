# Comparing `tmp/blacksheep-2.0a8.tar.gz` & `tmp/blacksheep-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksheep-2.0a8.tar", last modified: Sun Jul  2 11:25:56 2023, max compression
+gzip compressed data, was "blacksheep-2.0a9.tar", last modified: Fri Jul 14 18:59:53 2023, max compression
```

## Comparing `blacksheep-2.0a8.tar` & `blacksheep-2.0a9.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.362078 blacksheep-2.0a8/
--rw-r--r--   0 runner     (501) staff       (20)     1072 2023-07-02 11:25:29.000000 blacksheep-2.0a8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      233 2023-07-02 11:25:29.000000 blacksheep-2.0a8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    10983 2023-07-02 11:25:56.361600 blacksheep-2.0a8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    10098 2023-07-02 11:25:29.000000 blacksheep-2.0a8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.300331 blacksheep-2.0a8/blacksheep/
--rw-r--r--   0 runner     (501) staff       (20)     4219 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      433 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/asgi.pyi
--rw-r--r--   0 runner     (501) staff       (20)   710094 2023-07-02 11:25:47.000000 blacksheep-2.0a8/blacksheep/baseapp.c
--rw-r--r--   0 runner     (501) staff       (20)      567 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/baseapp.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1535 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/baseapp.pyi
--rw-r--r--   0 runner     (501) staff       (20)     6169 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/baseapp.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.305564 blacksheep-2.0a8/blacksheep/client/
--rw-r--r--   0 runner     (501) staff       (20)      396 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/client/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13126 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/client/connection.py
--rw-r--r--   0 runner     (501) staff       (20)    10499 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/client/cookies.py
--rw-r--r--   0 runner     (501) staff       (20)     2004 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/client/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)     4753 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/client/pool.py
--rw-r--r--   0 runner     (501) staff       (20)    15045 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/client/session.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.306495 blacksheep-2.0a8/blacksheep/common/
--rw-r--r--   0 runner     (501) staff       (20)      397 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/common/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.308404 blacksheep-2.0a8/blacksheep/common/files/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/common/files/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3371 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/common/files/asyncfs.py
--rw-r--r--   0 runner     (501) staff       (20)      938 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/common/files/info.py
--rwxr-xr-x   0 runner     (501) staff       (20)      679 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/common/files/pathsutils.py
--rw-r--r--   0 runner     (501) staff       (20)     1457 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/common/types.py
--rw-r--r--   0 runner     (501) staff       (20)   984100 2023-07-02 11:25:44.000000 blacksheep-2.0a8/blacksheep/contents.c
--rw-r--r--   0 runner     (501) staff       (20)     1042 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/contents.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3101 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/contents.pyi
--rw-r--r--   0 runner     (501) staff       (20)     7614 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/contents.pyx
--rw-r--r--   0 runner     (501) staff       (20)   709913 2023-07-02 11:25:43.000000 blacksheep-2.0a8/blacksheep/cookies.c
--rw-r--r--   0 runner     (501) staff       (20)      981 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/cookies.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1332 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/cookies.pyi
--rw-r--r--   0 runner     (501) staff       (20)     6498 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/cookies.pyx
--rw-r--r--   0 runner     (501) staff       (20)   700175 2023-07-02 11:25:42.000000 blacksheep-2.0a8/blacksheep/exceptions.c
--rw-r--r--   0 runner     (501) staff       (20)      421 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/exceptions.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1707 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/exceptions.pyi
--rw-r--r--   0 runner     (501) staff       (20)     1774 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/exceptions.pyx
--rw-r--r--   0 runner     (501) staff       (20)   589286 2023-07-02 11:25:42.000000 blacksheep-2.0a8/blacksheep/headers.c
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/headers.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1876 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/headers.pyi
--rw-r--r--   0 runner     (501) staff       (20)     5660 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/headers.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.308861 blacksheep-2.0a8/blacksheep/includes/
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/includes/consts.pxi
--rw-r--r--   0 runner     (501) staff       (20)  1193377 2023-07-02 11:25:45.000000 blacksheep-2.0a8/blacksheep/messages.c
--rw-r--r--   0 runner     (501) staff       (20)     2123 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/messages.pxd
--rw-r--r--   0 runner     (501) staff       (20)     5566 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/messages.pyi
--rw-r--r--   0 runner     (501) staff       (20)    18791 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/messages.pyx
--rw-r--r--   0 runner     (501) staff       (20)      587 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/middlewares.py
--rw-r--r--   0 runner     (501) staff       (20)     3320 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/multipart.py
--rw-r--r--   0 runner     (501) staff       (20)      434 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/normalization.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/py.typed
--rw-r--r--   0 runner     (501) staff       (20)     5564 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/ranges.py
--rw-r--r--   0 runner     (501) staff       (20)   649740 2023-07-02 11:25:46.000000 blacksheep-2.0a8/blacksheep/scribe.c
--rw-r--r--   0 runner     (501) staff       (20)      753 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/scribe.pxd
--rw-r--r--   0 runner     (501) staff       (20)      841 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/scribe.pyi
--rw-r--r--   0 runner     (501) staff       (20)    10605 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/scribe.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.317551 blacksheep-2.0a8/blacksheep/server/
--rw-r--r--   0 runner     (501) staff       (20)      180 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    29634 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/application.py
--rw-r--r--   0 runner     (501) staff       (20)     2537 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/asgi.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.319472 blacksheep-2.0a8/blacksheep/server/authentication/
--rw-r--r--   0 runner     (501) staff       (20)     1838 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/authentication/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4376 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/authentication/cookie.py
--rw-r--r--   0 runner     (501) staff       (20)     5275 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/authentication/jwt.py
--rw-r--r--   0 runner     (501) staff       (20)    37888 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/authentication/oidc.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.320098 blacksheep-2.0a8/blacksheep/server/authorization/
--rw-r--r--   0 runner     (501) staff       (20)     3540 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/authorization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    27359 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/bindings.py
--rw-r--r--   0 runner     (501) staff       (20)     4337 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/compression.py
--rw-r--r--   0 runner     (501) staff       (20)    13325 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/controllers.py
--rw-r--r--   0 runner     (501) staff       (20)    11679 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/cors.py
--rw-r--r--   0 runner     (501) staff       (20)    13278 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/csrf.py
--rw-r--r--   0 runner     (501) staff       (20)     1581 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/dataprotection.py
--rw-r--r--   0 runner     (501) staff       (20)     1932 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/di.py
--rw-r--r--   0 runner     (501) staff       (20)     1316 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/env.py
--rw-r--r--   0 runner     (501) staff       (20)     1679 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/errors.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.321507 blacksheep-2.0a8/blacksheep/server/files/
--rw-r--r--   0 runner     (501) staff       (20)     9368 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/files/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8717 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/files/dynamic.py
--rw-r--r--   0 runner     (501) staff       (20)     1134 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/files/static.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.322435 blacksheep-2.0a8/blacksheep/server/headers/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/headers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11234 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/headers/cache.py
--rw-r--r--   0 runner     (501) staff       (20)    19420 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/normalization.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.325514 blacksheep-2.0a8/blacksheep/server/openapi/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/openapi/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13395 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/openapi/common.py
--rw-r--r--   0 runner     (501) staff       (20)    16431 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/openapi/docstrings.py
--rw-r--r--   0 runner     (501) staff       (20)      428 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/openapi/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)     2831 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/openapi/ui.py
--rw-r--r--   0 runner     (501) staff       (20)    42810 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/openapi/v3.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.327037 blacksheep-2.0a8/blacksheep/server/remotes/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/remotes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13119 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/remotes/forwarding.py
--rw-r--r--   0 runner     (501) staff       (20)      963 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/remotes/hosts.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.328939 blacksheep-2.0a8/blacksheep/server/rendering/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/rendering/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      765 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/rendering/abc.py
--rw-r--r--   0 runner     (501) staff       (20)     4016 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/rendering/jinja2.py
--rw-r--r--   0 runner     (501) staff       (20)      417 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/rendering/models.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.332010 blacksheep-2.0a8/blacksheep/server/res/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/res/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1356 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/res/error.css
--rw-r--r--   0 runner     (501) staff       (20)     1028 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/res/error.html
--rw-r--r--   0 runner     (501) staff       (20)      331 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/res/fileslist.html
--rw-r--r--   0 runner     (501) staff       (20)      590 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/res/redoc-ui.html
--rw-r--r--   0 runner     (501) staff       (20)      841 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/res/swagger-ui.html
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/resources.py
--rw-r--r--   0 runner     (501) staff       (20)    10477 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/responses.py
--rw-r--r--   0 runner     (501) staff       (20)    26805 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/routing.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.332925 blacksheep-2.0a8/blacksheep/server/security/
--rw-r--r--   0 runner     (501) staff       (20)      417 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/security/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      848 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/security/hsts.py
--rw-r--r--   0 runner     (501) staff       (20)     5352 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/server/websocket.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.333572 blacksheep-2.0a8/blacksheep/sessions/
--rw-r--r--   0 runner     (501) staff       (20)     5399 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/sessions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.335715 blacksheep-2.0a8/blacksheep/settings/
--rw-r--r--   0 runner     (501) staff       (20)       76 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/settings/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      538 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/settings/di.py
--rw-r--r--   0 runner     (501) staff       (20)     1073 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/settings/html.py
--rw-r--r--   0 runner     (501) staff       (20)      894 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/settings/json.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.338354 blacksheep-2.0a8/blacksheep/testing/
--rw-r--r--   0 runner     (501) staff       (20)      398 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/testing/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4379 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/testing/client.py
--rw-r--r--   0 runner     (501) staff       (20)     3755 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/testing/helpers.py
--rw-r--r--   0 runner     (501) staff       (20)     1440 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/testing/messages.py
--rw-r--r--   0 runner     (501) staff       (20)     2659 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/testing/simulator.py
--rw-r--r--   0 runner     (501) staff       (20)   418255 2023-07-02 11:25:41.000000 blacksheep-2.0a8/blacksheep/url.c
--rw-r--r--   0 runner     (501) staff       (20)      751 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/url.pxd
--rw-r--r--   0 runner     (501) staff       (20)      707 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/url.pyi
--rw-r--r--   0 runner     (501) staff       (20)     4061 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/url.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.339866 blacksheep-2.0a8/blacksheep/utils/
--rw-r--r--   0 runner     (501) staff       (20)     1115 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2733 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/utils/aio.py
--rw-r--r--   0 runner     (501) staff       (20)      712 2023-07-02 11:25:29.000000 blacksheep-2.0a8/blacksheep/utils/meta.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.302695 blacksheep-2.0a8/blacksheep.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    10983 2023-07-02 11:25:56.000000 blacksheep-2.0a8/blacksheep.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4301 2023-07-02 11:25:56.000000 blacksheep-2.0a8/blacksheep.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-02 11:25:56.000000 blacksheep-2.0a8/blacksheep.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      276 2023-07-02 11:25:56.000000 blacksheep-2.0a8/blacksheep.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       11 2023-07-02 11:25:56.000000 blacksheep-2.0a8/blacksheep.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1435 2023-07-02 11:25:29.000000 blacksheep-2.0a8/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-02 11:25:56.362189 blacksheep-2.0a8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1275 2023-07-02 11:25:29.000000 blacksheep-2.0a8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 11:25:56.360957 blacksheep-2.0a8/tests/
--rw-r--r--   0 runner     (501) staff       (20)   113290 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_application.py
--rw-r--r--   0 runner     (501) staff       (20)    18883 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_auth.py
--rw-r--r--   0 runner     (501) staff       (20)     2294 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_auth_cookie.py
--rw-r--r--   0 runner     (501) staff       (20)    19745 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)     3540 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_caching.py
--rw-r--r--   0 runner     (501) staff       (20)     9781 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_contents.py
--rw-r--r--   0 runner     (501) staff       (20)    26270 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_controllers.py
--rw-r--r--   0 runner     (501) staff       (20)     7424 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_cookies.py
--rw-r--r--   0 runner     (501) staff       (20)    21883 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_cors.py
--rw-r--r--   0 runner     (501) staff       (20)    21340 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_csrf.py
--rw-r--r--   0 runner     (501) staff       (20)     1427 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_dataprotection.py
--rw-r--r--   0 runner     (501) staff       (20)      464 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_env.py
--rw-r--r--   0 runner     (501) staff       (20)     5565 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_files_handler.py
--rw-r--r--   0 runner     (501) staff       (20)    25887 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_files_serving.py
--rw-r--r--   0 runner     (501) staff       (20)    20844 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_forwarding.py
--rw-r--r--   0 runner     (501) staff       (20)     3531 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_gzip.py
--rw-r--r--   0 runner     (501) staff       (20)     6298 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_headers.py
--rw-r--r--   0 runner     (501) staff       (20)     5620 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_multipart.py
--rw-r--r--   0 runner     (501) staff       (20)    19342 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_normalization.py
--rw-r--r--   0 runner     (501) staff       (20)    28307 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_openapi_docstrings.py
--rw-r--r--   0 runner     (501) staff       (20)    82998 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_openapi_v3.py
--rw-r--r--   0 runner     (501) staff       (20)     1141 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_pathutils.py
--rw-r--r--   0 runner     (501) staff       (20)     5288 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_ranges.py
--rw-r--r--   0 runner     (501) staff       (20)    17798 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_requests.py
--rw-r--r--   0 runner     (501) staff       (20)    28976 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_responses.py
--rw-r--r--   0 runner     (501) staff       (20)    26915 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_router.py
--rw-r--r--   0 runner     (501) staff       (20)     8607 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_sessions.py
--rw-r--r--   0 runner     (501) staff       (20)     8666 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_templating.py
--rw-r--r--   0 runner     (501) staff       (20)     7043 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_testing.py
--rw-r--r--   0 runner     (501) staff       (20)     3220 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_url.py
--rw-r--r--   0 runner     (501) staff       (20)     1401 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    12812 2023-07-02 11:25:29.000000 blacksheep-2.0a8/tests/test_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.016225 blacksheep-2.0a9/
+-rw-rw-rw-   0        0        0     1072 2023-07-14 18:59:12.000000 blacksheep-2.0a9/LICENSE
+-rw-rw-rw-   0        0        0      233 2023-07-14 18:59:12.000000 blacksheep-2.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11293 2023-07-14 18:59:53.016225 blacksheep-2.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0    10098 2023-07-14 18:59:12.000000 blacksheep-2.0a9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:51.654176 blacksheep-2.0a9/blacksheep/
+-rw-rw-rw-   0        0        0     4219 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/asgi.pyi
+-rw-rw-rw-   0        0        0   710271 2023-07-14 18:59:37.000000 blacksheep-2.0a9/blacksheep/baseapp.c
+-rw-rw-rw-   0        0        0      567 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/baseapp.pxd
+-rw-rw-rw-   0        0        0     1535 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/baseapp.pyi
+-rw-rw-rw-   0        0        0     6169 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/baseapp.pyx
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.499864 blacksheep-2.0a9/blacksheep/client/
+-rw-rw-rw-   0        0        0      396 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/client/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/client/connection.py
+-rw-rw-rw-   0        0        0    10499 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/client/cookies.py
+-rw-rw-rw-   0        0        0     2004 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/client/exceptions.py
+-rw-rw-rw-   0        0        0     4753 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/client/pool.py
+-rw-rw-rw-   0        0        0    15045 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/client/session.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.499864 blacksheep-2.0a9/blacksheep/common/
+-rw-rw-rw-   0        0        0      397 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.499864 blacksheep-2.0a9/blacksheep/common/files/
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/common/files/__init__.py
+-rw-rw-rw-   0        0        0     3371 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/common/files/asyncfs.py
+-rw-rw-rw-   0        0        0      938 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/common/files/info.py
+-rw-rw-rw-   0        0        0      679 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/common/files/pathsutils.py
+-rw-rw-rw-   0        0        0     1457 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/common/types.py
+-rw-rw-rw-   0        0        0   995944 2023-07-14 18:59:35.000000 blacksheep-2.0a9/blacksheep/contents.c
+-rw-rw-rw-   0        0        0     1048 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/contents.pxd
+-rw-rw-rw-   0        0        0     3101 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/contents.pyi
+-rw-rw-rw-   0        0        0     7620 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/contents.pyx
+-rw-rw-rw-   0        0        0   710103 2023-07-14 18:59:34.000000 blacksheep-2.0a9/blacksheep/cookies.c
+-rw-rw-rw-   0        0        0      981 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/cookies.pxd
+-rw-rw-rw-   0        0        0     1332 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/cookies.pyi
+-rw-rw-rw-   0        0        0     6498 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/cookies.pyx
+-rw-rw-rw-   0        0        0   700393 2023-07-14 18:59:33.000000 blacksheep-2.0a9/blacksheep/exceptions.c
+-rw-rw-rw-   0        0        0      421 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/exceptions.pxd
+-rw-rw-rw-   0        0        0     1707 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/exceptions.pyi
+-rw-rw-rw-   0        0        0     1774 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/exceptions.pyx
+-rw-rw-rw-   0        0        0   589462 2023-07-14 18:59:34.000000 blacksheep-2.0a9/blacksheep/headers.c
+-rw-rw-rw-   0        0        0      798 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/headers.pxd
+-rw-rw-rw-   0        0        0     1876 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/headers.pyi
+-rw-rw-rw-   0        0        0     5660 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/headers.pyx
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.499864 blacksheep-2.0a9/blacksheep/includes/
+-rw-rw-rw-   0        0        0       44 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/includes/consts.pxi
+-rw-rw-rw-   0        0        0  1193798 2023-07-14 18:59:36.000000 blacksheep-2.0a9/blacksheep/messages.c
+-rw-rw-rw-   0        0        0     2123 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/messages.pxd
+-rw-rw-rw-   0        0        0     5566 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/messages.pyi
+-rw-rw-rw-   0        0        0    18791 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/messages.pyx
+-rw-rw-rw-   0        0        0      587 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/middlewares.py
+-rw-rw-rw-   0        0        0     3320 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/multipart.py
+-rw-rw-rw-   0        0        0      434 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/normalization.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/py.typed
+-rw-rw-rw-   0        0        0     5564 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/ranges.py
+-rw-rw-rw-   0        0        0   651653 2023-07-14 18:59:37.000000 blacksheep-2.0a9/blacksheep/scribe.c
+-rw-rw-rw-   0        0        0      753 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/scribe.pxd
+-rw-rw-rw-   0        0        0      841 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/scribe.pyi
+-rw-rw-rw-   0        0        0    10605 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/scribe.pyx
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/
+-rw-rw-rw-   0        0        0      180 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/__init__.py
+-rw-rw-rw-   0        0        0    29634 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/application.py
+-rw-rw-rw-   0        0        0     2537 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/asgi.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/authentication/
+-rw-rw-rw-   0        0        0     1838 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/authentication/__init__.py
+-rw-rw-rw-   0        0        0     4376 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/authentication/cookie.py
+-rw-rw-rw-   0        0        0     5275 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/authentication/jwt.py
+-rw-rw-rw-   0        0        0    37888 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/authentication/oidc.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/authorization/
+-rw-rw-rw-   0        0        0     3540 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/authorization/__init__.py
+-rw-rw-rw-   0        0        0    27359 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/bindings.py
+-rw-rw-rw-   0        0        0     4337 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/compression.py
+-rw-rw-rw-   0        0        0    13325 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/controllers.py
+-rw-rw-rw-   0        0        0    11679 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/cors.py
+-rw-rw-rw-   0        0        0    13278 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/csrf.py
+-rw-rw-rw-   0        0        0     1581 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/dataprotection.py
+-rw-rw-rw-   0        0        0     1932 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/di.py
+-rw-rw-rw-   0        0        0     1316 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/env.py
+-rw-rw-rw-   0        0        0     1679 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/files/
+-rw-rw-rw-   0        0        0     9368 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/files/__init__.py
+-rw-rw-rw-   0        0        0     8717 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/files/dynamic.py
+-rw-rw-rw-   0        0        0     1134 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/files/static.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/headers/
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/headers/__init__.py
+-rw-rw-rw-   0        0        0    11234 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/headers/cache.py
+-rw-rw-rw-   0        0        0    19420 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/normalization.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/openapi/
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/openapi/__init__.py
+-rw-rw-rw-   0        0        0    13395 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/openapi/common.py
+-rw-rw-rw-   0        0        0    16431 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/openapi/docstrings.py
+-rw-rw-rw-   0        0        0      428 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/openapi/exceptions.py
+-rw-rw-rw-   0        0        0     2831 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/openapi/ui.py
+-rw-rw-rw-   0        0        0    42810 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/openapi/v3.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.515481 blacksheep-2.0a9/blacksheep/server/remotes/
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/remotes/__init__.py
+-rw-rw-rw-   0        0        0    13119 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/remotes/forwarding.py
+-rw-rw-rw-   0        0        0      963 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/remotes/hosts.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/server/rendering/
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/rendering/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/rendering/abc.py
+-rw-rw-rw-   0        0        0     4016 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/rendering/jinja2.py
+-rw-rw-rw-   0        0        0      417 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/rendering/models.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/server/res/
+-rw-rw-rw-   0        0        0        0 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/res/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/res/error.css
+-rw-rw-rw-   0        0        0     1028 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/res/error.html
+-rw-rw-rw-   0        0        0      331 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/res/fileslist.html
+-rw-rw-rw-   0        0        0      590 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/res/redoc-ui.html
+-rw-rw-rw-   0        0        0      841 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/res/swagger-ui.html
+-rw-rw-rw-   0        0        0      263 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/resources.py
+-rw-rw-rw-   0        0        0    10477 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/responses.py
+-rw-rw-rw-   0        0        0    26805 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/routing.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/server/security/
+-rw-rw-rw-   0        0        0      417 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/security/__init__.py
+-rw-rw-rw-   0        0        0      848 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/security/hsts.py
+-rw-rw-rw-   0        0        0     5352 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/server/websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/sessions/
+-rw-rw-rw-   0        0        0     5399 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/settings/
+-rw-rw-rw-   0        0        0       76 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/settings/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/settings/di.py
+-rw-rw-rw-   0        0        0     1073 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/settings/html.py
+-rw-rw-rw-   0        0        0      894 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/settings/json.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/testing/
+-rw-rw-rw-   0        0        0      398 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/testing/__init__.py
+-rw-rw-rw-   0        0        0     4379 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/testing/client.py
+-rw-rw-rw-   0        0        0     3755 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/testing/helpers.py
+-rw-rw-rw-   0        0        0     1440 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/testing/messages.py
+-rw-rw-rw-   0        0        0     2659 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/testing/simulator.py
+-rw-rw-rw-   0        0        0   418432 2023-07-14 18:59:32.000000 blacksheep-2.0a9/blacksheep/url.c
+-rw-rw-rw-   0        0        0      751 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/url.pxd
+-rw-rw-rw-   0        0        0      707 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/url.pyi
+-rw-rw-rw-   0        0        0     4061 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/url.pyx
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.000610 blacksheep-2.0a9/blacksheep/utils/
+-rw-rw-rw-   0        0        0     1115 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/utils/__init__.py
+-rw-rw-rw-   0        0        0     2733 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/utils/aio.py
+-rw-rw-rw-   0        0        0      712 2023-07-14 18:59:12.000000 blacksheep-2.0a9/blacksheep/utils/meta.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:52.499864 blacksheep-2.0a9/blacksheep.egg-info/
+-rw-rw-rw-   0        0        0    11293 2023-07-14 18:59:51.000000 blacksheep-2.0a9/blacksheep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4301 2023-07-14 18:59:51.000000 blacksheep-2.0a9/blacksheep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:59:51.000000 blacksheep-2.0a9/blacksheep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2023-07-14 18:59:51.000000 blacksheep-2.0a9/blacksheep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 18:59:51.000000 blacksheep-2.0a9/blacksheep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1435 2023-07-14 18:59:12.000000 blacksheep-2.0a9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 18:59:53.016225 blacksheep-2.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-14 18:59:12.000000 blacksheep-2.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:59:53.016225 blacksheep-2.0a9/tests/
+-rw-rw-rw-   0        0        0   113290 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_application.py
+-rw-rw-rw-   0        0        0    18883 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_auth.py
+-rw-rw-rw-   0        0        0     2294 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_auth_cookie.py
+-rw-rw-rw-   0        0        0    19745 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_bindings.py
+-rw-rw-rw-   0        0        0     3540 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_caching.py
+-rw-rw-rw-   0        0        0     9964 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_contents.py
+-rw-rw-rw-   0        0        0    26270 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_controllers.py
+-rw-rw-rw-   0        0        0     7424 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_cookies.py
+-rw-rw-rw-   0        0        0    21883 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_cors.py
+-rw-rw-rw-   0        0        0    21340 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_csrf.py
+-rw-rw-rw-   0        0        0     1427 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_dataprotection.py
+-rw-rw-rw-   0        0        0      464 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_env.py
+-rw-rw-rw-   0        0        0     5565 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_files_handler.py
+-rw-rw-rw-   0        0        0    25887 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_files_serving.py
+-rw-rw-rw-   0        0        0    20844 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_forwarding.py
+-rw-rw-rw-   0        0        0     3531 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_gzip.py
+-rw-rw-rw-   0        0        0     6298 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_headers.py
+-rw-rw-rw-   0        0        0     5620 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_multipart.py
+-rw-rw-rw-   0        0        0    19342 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_normalization.py
+-rw-rw-rw-   0        0        0    28307 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_openapi_docstrings.py
+-rw-rw-rw-   0        0        0    82998 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_openapi_v3.py
+-rw-rw-rw-   0        0        0     1141 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_pathutils.py
+-rw-rw-rw-   0        0        0     5288 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_ranges.py
+-rw-rw-rw-   0        0        0    17798 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_requests.py
+-rw-rw-rw-   0        0        0    28976 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_responses.py
+-rw-rw-rw-   0        0        0    26915 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_router.py
+-rw-rw-rw-   0        0        0     8607 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_sessions.py
+-rw-rw-rw-   0        0        0     8666 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_templating.py
+-rw-rw-rw-   0        0        0     7043 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_testing.py
+-rw-rw-rw-   0        0        0     3220 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_url.py
+-rw-rw-rw-   0        0        0     1401 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_utils.py
+-rw-rw-rw-   0        0        0    12812 2023-07-14 18:59:12.000000 blacksheep-2.0a9/tests/test_websocket.py
```

### Comparing `blacksheep-2.0a8/LICENSE` & `blacksheep-2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/PKG-INFO` & `blacksheep-2.0a9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,687 +1,706 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 626c 6163  : 2.1.Name: blac
-00000020: 6b73 6865 6570 0a56 6572 7369 6f6e 3a20  ksheep.Version: 
-00000030: 322e 3061 380a 5375 6d6d 6172 793a 2046  2.0a8.Summary: F
-00000040: 6173 7420 7765 6220 6672 616d 6577 6f72  ast web framewor
-00000050: 6b20 666f 7220 5079 7468 6f6e 2061 7379  k for Python asy
-00000060: 6e63 696f 0a41 7574 686f 722d 656d 6169  ncio.Author-emai
-00000070: 6c3a 2052 6f62 6572 746f 2050 7265 7661  l: Roberto Preva
-00000080: 746f 203c 726f 6265 7274 6f2e 7072 6576  to <roberto.prev
-00000090: 6174 6f40 676d 6169 6c2e 636f 6d3e 0a50  ato@gmail.com>.P
-000000a0: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
-000000b0: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
-000000c0: 7468 7562 2e63 6f6d 2f4e 656f 7465 726f  thub.com/Neotero
-000000d0: 692f 426c 6163 6b53 6865 6570 0a50 726f  i/BlackSheep.Pro
-000000e0: 6a65 6374 2d55 524c 3a20 4275 6720 5472  ject-URL: Bug Tr
-000000f0: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
-00000100: 6974 6875 622e 636f 6d2f 4e65 6f74 6572  ithub.com/Neoter
-00000110: 6f69 2f42 6c61 636b 5368 6565 702f 6973  oi/BlackSheep/is
-00000120: 7375 6573 0a4b 6579 776f 7264 733a 2062  sues.Keywords: b
-00000130: 6c61 636b 7368 6565 702c 7765 6220 6672  lacksheep,web fr
-00000140: 616d 6577 6f72 6b2c 6173 796e 6369 6f0a  amework,asyncio.
-00000150: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
-00000160: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000170: 3a20 3320 2d20 416c 7068 610a 436c 6173  : 3 - Alpha.Clas
-00000180: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000190: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001a0: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
-000001b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-000001e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000001f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000200: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000210: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-00000220: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000230: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000240: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-00000250: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000260: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000270: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-00000280: 6965 723a 2045 6e76 6972 6f6e 6d65 6e74  ier: Environment
-00000290: 203a 3a20 5765 6220 456e 7669 726f 6e6d   :: Web Environm
-000002a0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-000002b0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000002c0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000002d0: 6e74 0a43 6c61 7373 6966 6965 723a 2046  nt.Classifier: F
-000002e0: 7261 6d65 776f 726b 203a 3a20 4173 796e  ramework :: Asyn
-000002f0: 6349 4f0a 5265 7175 6972 6573 2d50 7974  cIO.Requires-Pyt
-00000300: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
-00000310: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000320: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000330: 776e 0a50 726f 7669 6465 732d 4578 7472  wn.Provides-Extr
-00000340: 613a 206a 696e 6a61 0a50 726f 7669 6465  a: jinja.Provide
-00000350: 732d 4578 7472 613a 2066 756c 6c0a 4c69  s-Extra: full.Li
-00000360: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000370: 4e53 450a 0a5b 215b 4275 696c 645d 2868  NSE..[![Build](h
-00000380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000390: 6d2f 4e65 6f74 6572 6f69 2f42 6c61 636b  m/Neoteroi/Black
-000003a0: 5368 6565 702f 776f 726b 666c 6f77 732f  Sheep/workflows/
-000003b0: 4d61 696e 2f62 6164 6765 2e73 7667 295d  Main/badge.svg)]
-000003c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000003d0: 636f 6d2f 4e65 6f74 6572 6f69 2f42 6c61  com/Neoteroi/Bla
-000003e0: 636b 5368 6565 702f 6163 7469 6f6e 7329  ckSheep/actions)
-000003f0: 0a5b 215b 7079 7069 5d28 6874 7470 733a  .[![pypi](https:
-00000400: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000410: 2f70 7970 692f 762f 426c 6163 6b53 6865  /pypi/v/BlackShe
-00000420: 6570 2e73 7667 3f63 6f6c 6f72 3d62 6c75  ep.svg?color=blu
-00000430: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
-00000440: 2e6f 7267 2f70 726f 6a65 6374 2f42 6c61  .org/project/Bla
-00000450: 636b 5368 6565 702f 290a 5b21 5b76 6572  ckSheep/).[![ver
-00000460: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
-00000470: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000480: 7069 2f70 7976 6572 7369 6f6e 732f 626c  pi/pyversions/bl
-00000490: 6163 6b73 6865 6570 2e73 7667 295d 2868  acksheep.svg)](h
-000004a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000004b0: 6d2f 726f 6265 7274 6f70 7265 7661 746f  m/robertoprevato
-000004c0: 2f62 6c61 636b 7368 6565 7029 0a5b 215b  /blacksheep).[![
-000004d0: 636f 6465 636f 765d 2868 7474 7073 3a2f  codecov](https:/
-000004e0: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f4e  /codecov.io/gh/N
-000004f0: 656f 7465 726f 692f 426c 6163 6b53 6865  eoteroi/BlackShe
-00000500: 6570 2f62 7261 6e63 682f 6d61 7374 6572  ep/branch/master
-00000510: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-00000520: 3f74 6f6b 656e 3d4e 7a69 3239 4c30 4567  ?token=Nzi29L0Eg
-00000530: 3129 5d28 6874 7470 733a 2f2f 636f 6465  1)](https://code
-00000540: 636f 762e 696f 2f67 682f 4e65 6f74 6572  cov.io/gh/Neoter
-00000550: 6f69 2f42 6c61 636b 5368 6565 7029 0a5b  oi/BlackSheep).[
-00000560: 215b 6c69 6365 6e73 655d 2868 7474 7073  ![license](https
-00000570: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000580: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00000590: 2f4e 656f 7465 726f 692f 626c 6163 6b73  /Neoteroi/blacks
-000005a0: 6865 6570 2e73 7667 295d 2868 7474 7073  heep.svg)](https
-000005b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e65  ://github.com/Ne
-000005c0: 6f74 6572 6f69 2f62 6c61 636b 7368 6565  oteroi/blackshee
-000005d0: 702f 626c 6f62 2f6d 6169 6e2f 4c49 4345  p/blob/main/LICE
-000005e0: 4e53 4529 205b 215b 4a6f 696e 2074 6865  NSE) [![Join the
-000005f0: 2063 6861 7420 6174 2068 7474 7073 3a2f   chat at https:/
-00000600: 2f67 6974 7465 722e 696d 2f4e 656f 7465  /gitter.im/Neote
-00000610: 726f 692f 426c 6163 6b53 6865 6570 5d28  roi/BlackSheep](
-00000620: 6874 7470 733a 2f2f 6261 6467 6573 2e67  https://badges.g
-00000630: 6974 7465 722e 696d 2f4e 656f 7465 726f  itter.im/Neotero
-00000640: 692f 426c 6163 6b53 6865 6570 2e73 7667  i/BlackSheep.svg
-00000650: 295d 2868 7474 7073 3a2f 2f67 6974 7465  )](https://gitte
-00000660: 722e 696d 2f4e 656f 7465 726f 692f 426c  r.im/Neoteroi/Bl
-00000670: 6163 6b53 6865 6570 3f75 746d 5f73 6f75  ackSheep?utm_sou
-00000680: 7263 653d 6261 6467 6526 7574 6d5f 6d65  rce=badge&utm_me
-00000690: 6469 756d 3d62 6164 6765 2675 746d 5f63  dium=badge&utm_c
-000006a0: 616d 7061 6967 6e3d 7072 2d62 6164 6765  ampaign=pr-badge
-000006b0: 2675 746d 5f63 6f6e 7465 6e74 3d62 6164  &utm_content=bad
-000006c0: 6765 2920 5b21 5b64 6f63 756d 656e 7461  ge) [![documenta
-000006d0: 7469 6f6e 5d28 6874 7470 733a 2f2f 696d  tion](https://im
-000006e0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000006f0: 6765 2ff0 9f93 962d 646f 6373 2d70 7572  ge/....-docs-pur
-00000700: 706c 6529 5d28 6874 7470 733a 2f2f 7777  ple)](https://ww
-00000710: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
-00000720: 6c61 636b 7368 6565 702f 290a 0a23 2042  lacksheep/)..# B
-00000730: 6c61 636b 5368 6565 700a 426c 6163 6b53  lackSheep.BlackS
-00000740: 6865 6570 2069 7320 616e 2061 7379 6e63  heep is an async
-00000750: 6872 6f6e 6f75 7320 7765 6220 6672 616d  hronous web fram
-00000760: 6577 6f72 6b20 746f 2062 7569 6c64 2065  ework to build e
-00000770: 7665 6e74 2062 6173 6564 2077 6562 0a61  vent based web.a
-00000780: 7070 6c69 6361 7469 6f6e 7320 7769 7468  pplications with
-00000790: 2050 7974 686f 6e2e 2049 7420 6973 2069   Python. It is i
-000007a0: 6e73 7069 7265 6420 6279 0a5b 466c 6173  nspired by.[Flas
-000007b0: 6b5d 2868 7474 7073 3a2f 2f70 616c 6c65  k](https://palle
-000007c0: 7473 7072 6f6a 6563 7473 2e63 6f6d 2f70  tsprojects.com/p
-000007d0: 2f66 6c61 736b 2f29 2c20 5b41 5350 2e4e  /flask/), [ASP.N
-000007e0: 4554 0a43 6f72 655d 2868 7474 7073 3a2f  ET.Core](https:/
-000007f0: 2f64 6f63 732e 6d69 6372 6f73 6f66 742e  /docs.microsoft.
-00000800: 636f 6d2f 656e 2d75 732f 6173 706e 6574  com/en-us/aspnet
-00000810: 2f63 6f72 652f 292c 2061 6e64 2074 6865  /core/), and the
-00000820: 2077 6f72 6b20 6279 205b 5975 7279 0a53   work by [Yury.S
-00000830: 656c 6976 616e 6f76 5d28 6874 7470 733a  elivanov](https:
-00000840: 2f2f 6d61 6769 632e 696f 2f62 6c6f 672f  //magic.io/blog/
-00000850: 7576 6c6f 6f70 2d62 6c61 7a69 6e67 2d66  uvloop-blazing-f
-00000860: 6173 742d 7079 7468 6f6e 2d6e 6574 776f  ast-python-netwo
-00000870: 726b 696e 672f 292e 0a0a 3c70 2061 6c69  rking/)...<p ali
-00000880: 676e 3d22 6c65 6674 223e 0a20 203c 6120  gn="left">.  <a 
-00000890: 6872 6566 3d22 2362 6c61 636b 7368 6565  href="#blackshee
-000008a0: 7022 3e3c 696d 6720 7769 6474 683d 2233  p"><img width="3
-000008b0: 3230 2220 6865 6967 6874 3d22 3237 3122  20" height="271"
-000008c0: 2073 7263 3d22 6874 7470 733a 2f2f 7777   src="https://ww
-000008d0: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
-000008e0: 6c61 636b 7368 6565 702f 696d 672f 626c  lacksheep/img/bl
-000008f0: 6163 6b73 6865 6570 2e70 6e67 2220 616c  acksheep.png" al
-00000900: 743d 2242 6c61 636b 2053 6865 6570 223e  t="Black Sheep">
-00000910: 3c2f 613e 0a3c 2f70 3e0a 0a60 6060 6261  </a>.</p>..```ba
-00000920: 7368 0a70 6970 2069 6e73 7461 6c6c 2062  sh.pip install b
-00000930: 6c61 636b 7368 6565 700a 6060 600a 0a2d  lacksheep.```..-
-00000940: 2d2d 0a0a 6060 6070 7974 686f 6e0a 6672  --..```python.fr
-00000950: 6f6d 2064 6174 6574 696d 6520 696d 706f  om datetime impo
-00000960: 7274 2064 6174 6574 696d 650a 0a66 726f  rt datetime..fro
-00000970: 6d20 626c 6163 6b73 6865 6570 2069 6d70  m blacksheep imp
-00000980: 6f72 7420 4170 706c 6963 6174 696f 6e0a  ort Application.
-00000990: 0a0a 6170 7020 3d20 4170 706c 6963 6174  ..app = Applicat
-000009a0: 696f 6e28 290a 0a40 6170 702e 726f 7574  ion()..@app.rout
-000009b0: 6528 222f 2229 0a61 7379 6e63 2064 6566  e("/").async def
-000009c0: 2068 6f6d 6528 293a 0a20 2020 2072 6574   home():.    ret
-000009d0: 7572 6e20 6622 4865 6c6c 6f2c 2057 6f72  urn f"Hello, Wor
-000009e0: 6c64 2120 7b64 6174 6574 696d 652e 7574  ld! {datetime.ut
-000009f0: 636e 6f77 2829 2e69 736f 666f 726d 6174  cnow().isoformat
-00000a00: 2829 7d22 0a0a 6060 600a 0a23 2320 4765  ()}"..```..## Ge
-00000a10: 7474 696e 6720 7374 6172 7465 6420 7573  tting started us
-00000a20: 696e 6720 7468 6520 434c 4920 e29c a80a  ing the CLI ....
-00000a30: 0a42 6c61 636b 5368 6565 7020 6f66 6665  .BlackSheep offe
-00000a40: 7273 2061 2043 4c49 2074 6f20 626f 6f74  rs a CLI to boot
-00000a50: 7374 7261 7020 6e65 7720 7072 6f6a 6563  strap new projec
-00000a60: 7473 2072 6170 6964 6c79 2e0a 546f 2074  ts rapidly..To t
-00000a70: 7279 2069 742c 2066 6972 7374 2069 6e73  ry it, first ins
-00000a80: 7461 6c6c 2074 6865 2060 626c 6163 6b73  tall the `blacks
-00000a90: 6865 6570 2d63 6c69 6020 7061 636b 6167  heep-cli` packag
-00000aa0: 653a 0a0a 6060 6062 6173 680a 7069 7020  e:..```bash.pip 
-00000ab0: 696e 7374 616c 6c20 626c 6163 6b73 6865  install blackshe
-00000ac0: 6570 2d63 6c69 0a60 6060 0a0a 5468 656e  ep-cli.```..Then
-00000ad0: 2075 7365 2074 6865 2060 626c 6163 6b73   use the `blacks
-00000ae0: 6865 6570 2063 7265 6174 6560 2063 6f6d  heep create` com
-00000af0: 6d61 6e64 2074 6f20 626f 6f74 7374 7261  mand to bootstra
-00000b00: 7020 6120 7072 6f6a 6563 740a 7573 696e  p a project.usin
-00000b10: 6720 6f6e 6520 6f66 2074 6865 2073 7570  g one of the sup
-00000b20: 706f 7274 6564 2074 656d 706c 6174 6573  ported templates
-00000b30: 2e0a 0a21 5b62 6c61 636b 7368 6565 7020  ...![blacksheep 
-00000b40: 6372 6561 7465 2063 6f6d 6d61 6e64 5d28  create command](
-00000b50: 6874 7470 733a 2f2f 6769 7374 2e67 6974  https://gist.git
-00000b60: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000b70: 6f6d 2f52 6f62 6572 746f 5072 6576 6174  om/RobertoPrevat
-00000b80: 6f2f 3338 6130 3539 3862 3531 3561 3266  o/38a0598b515a2f
-00000b90: 3732 3537 6336 3134 3933 3838 3433 6239  7257c614938843b9
-00000ba0: 3962 2f72 6177 2f36 3764 3135 6261 3333  9b/raw/67d15ba33
-00000bb0: 3764 6539 3463 3266 3530 6439 3830 6137  7de94c2f50d980a7
-00000bc0: 6238 3932 3461 3734 3732 3539 3235 342f  b8924a747259254/
-00000bd0: 626c 6163 6b73 6865 6570 2d63 7265 6174  blacksheep-creat
-00000be0: 652d 6465 6d6f 2e67 6966 290a 0a54 6865  e-demo.gif)..The
-00000bf0: 2043 4c49 2069 6e63 6c75 6465 7320 6120   CLI includes a 
-00000c00: 6865 6c70 2c20 616e 6420 7375 7070 6f72  help, and suppor
-00000c10: 7473 2063 7573 746f 6d20 7465 6d70 6c61  ts custom templa
-00000c20: 7465 732c 2075 7369 6e67 2074 6865 0a73  tes, using the.s
-00000c30: 616d 6520 736f 7572 6365 7320 7375 7070  ame sources supp
-00000c40: 6f72 7465 6420 6279 2060 436f 6f6b 6965  orted by `Cookie
-00000c50: 6375 7474 6572 602e 0a0a 2323 2047 6574  cutter`...## Get
-00000c60: 7469 6e67 2073 7461 7274 6564 2077 6974  ting started wit
-00000c70: 6820 7468 6520 646f 6375 6d65 6e74 6174  h the documentat
-00000c80: 696f 6e0a 0a54 6865 2064 6f63 756d 656e  ion..The documen
-00000c90: 7461 7469 6f6e 206f 6666 6572 7320 6765  tation offers ge
-00000ca0: 7474 696e 6720 7374 6172 7465 6420 7475  tting started tu
-00000cb0: 746f 7269 616c 733a 0a2a 205b 4765 7474  torials:.* [Gett
-00000cc0: 696e 6720 7374 6172 7465 643a 0a20 2062  ing started:.  b
-00000cd0: 6173 6963 735d 2868 7474 7073 3a2f 2f77  asics](https://w
-00000ce0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00000cf0: 626c 6163 6b73 6865 6570 2f67 6574 7469  blacksheep/getti
-00000d00: 6e67 2d73 7461 7274 6564 2f29 0a2a 205b  ng-started/).* [
-00000d10: 4765 7474 696e 6720 7374 6172 7465 643a  Getting started:
-00000d20: 2074 6865 204d 5643 2070 726f 6a65 6374   the MVC project
-00000d30: 0a20 2074 656d 706c 6174 655d 2868 7474  .  template](htt
-00000d40: 7073 3a2f 2f77 7777 2e6e 656f 7465 726f  ps://www.neotero
-00000d50: 692e 6465 762f 626c 6163 6b73 6865 6570  i.dev/blacksheep
-00000d60: 2f6d 7663 2d70 726f 6a65 6374 2d74 656d  /mvc-project-tem
-00000d70: 706c 6174 652f 290a 0a54 6865 7365 2070  plate/)..These p
-00000d80: 726f 6a65 6374 2074 656d 706c 6174 6573  roject templates
-00000d90: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00000da0: 7374 6172 7420 6e65 7720 6170 706c 6963  start new applic
-00000db0: 6174 696f 6e73 2066 6173 7465 723a 0a0a  ations faster:..
-00000dc0: 2a20 5b4d 5643 2070 726f 6a65 6374 0a20  * [MVC project. 
-00000dd0: 2074 656d 706c 6174 655d 2868 7474 7073   template](https
-00000de0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e65  ://github.com/Ne
-00000df0: 6f74 6572 6f69 2f42 6c61 636b 5368 6565  oteroi/BlackShee
-00000e00: 704d 5643 290a 2a20 5b45 6d70 7479 2070  pMVC).* [Empty p
-00000e10: 726f 6a65 6374 0a20 2074 656d 706c 6174  roject.  templat
-00000e20: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000e30: 622e 636f 6d2f 4e65 6f74 6572 6f69 2f42  b.com/Neoteroi/B
-00000e40: 6c61 636b 5368 6565 7045 6d70 7479 5072  lackSheepEmptyPr
-00000e50: 6f6a 6563 7429 0a0a 2323 2052 6571 7569  oject)..## Requi
-00000e60: 7265 6d65 6e74 730a 0a5b 5079 7468 6f6e  rements..[Python
-00000e70: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
-00000e80: 7468 6f6e 2e6f 7267 293a 2061 6e79 2076  thon.org): any v
-00000e90: 6572 7369 6f6e 206c 6973 7465 6420 696e  ersion listed in
-00000ea0: 2074 6865 2070 726f 6a65 6374 2773 0a63   the project's.c
-00000eb0: 6c61 7373 6966 6965 7273 2e20 5468 6520  lassifiers. The 
-00000ec0: 6375 7272 656e 7420 6c69 7374 2069 733a  current list is:
-00000ed0: 0a0a 5b21 5b76 6572 7369 6f6e 735d 2868  ..[![versions](h
-00000ee0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000ef0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000f00: 7369 6f6e 732f 626c 6163 6b73 6865 6570  sions/blacksheep
-00000f10: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000f20: 6974 6875 622e 636f 6d2f 726f 6265 7274  ithub.com/robert
-00000f30: 6f70 7265 7661 746f 2f62 6c61 636b 7368  oprevato/blacksh
-00000f40: 6565 7029 0a0a 0a42 6c61 636b 5368 6565  eep)...BlackShee
-00000f50: 7020 6265 6c6f 6e67 7320 746f 2074 6865  p belongs to the
-00000f60: 2063 6174 6567 6f72 7920 6f66 0a5b 4153   category of.[AS
-00000f70: 4749 5d28 6874 7470 733a 2f2f 6173 6769  GI](https://asgi
-00000f80: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000f90: 656e 2f6c 6174 6573 742f 2920 7765 6220  en/latest/) web 
-00000fa0: 6672 616d 6577 6f72 6b73 2c20 736f 2069  frameworks, so i
-00000fb0: 7420 7265 7175 6972 6573 0a61 6e20 4153  t requires.an AS
-00000fc0: 4749 2048 5454 5020 7365 7276 6572 2074  GI HTTP server t
-00000fd0: 6f20 7275 6e2c 2073 7563 6820 6173 205b  o run, such as [
-00000fe0: 7576 6963 6f72 6e5d 2868 7474 703a 2f2f  uvicorn](http://
-00000ff0: 7777 772e 7576 6963 6f72 6e2e 6f72 672f  www.uvicorn.org/
-00001000: 292c 206f 720a 5b68 7970 6572 636f 726e  ), or.[hypercorn
-00001010: 5d28 6874 7470 733a 2f2f 7067 6a6f 6e65  ](https://pgjone
-00001020: 732e 6769 746c 6162 2e69 6f2f 6879 7065  s.gitlab.io/hype
-00001030: 7263 6f72 6e2f 292e 2046 6f72 2065 7861  rcorn/). For exa
-00001040: 6d70 6c65 2c20 746f 2075 7365 2069 7420  mple, to use it 
-00001050: 7769 7468 0a75 7669 636f 726e 3a0a 0a60  with.uvicorn:..`
-00001060: 6060 6261 7368 0a24 2070 6970 2069 6e73  ``bash.$ pip ins
-00001070: 7461 6c6c 2075 7669 636f 726e 0a60 6060  tall uvicorn.```
-00001080: 0a0a 546f 2072 756e 2061 6e20 6170 706c  ..To run an appl
-00001090: 6963 6174 696f 6e20 6c69 6b65 2069 6e20  ication like in 
-000010a0: 7468 6520 6578 616d 706c 6520 6162 6f76  the example abov
-000010b0: 652c 2075 7365 2074 6865 206d 6574 686f  e, use the metho
-000010c0: 6473 2070 726f 7669 6465 6420 6279 0a74  ds provided by.t
-000010d0: 6865 2041 5347 4920 4854 5450 2053 6572  he ASGI HTTP Ser
-000010e0: 7665 723a 0a0a 6060 6062 6173 680a 2320  ver:..```bash.# 
-000010f0: 6966 2074 6865 2042 6c61 636b 5368 6565  if the BlackShee
-00001100: 7020 6170 7020 6973 2064 6566 696e 6564  p app is defined
-00001110: 2069 6e20 6120 6669 6c65 2060 7365 7276   in a file `serv
-00001120: 6572 2e70 7960 0a0a 2420 7576 6963 6f72  er.py`..$ uvicor
-00001130: 6e20 7365 7276 6572 3a61 7070 0a60 6060  n server:app.```
-00001140: 0a0a 546f 2072 756e 2066 6f72 2070 726f  ..To run for pro
-00001150: 6475 6374 696f 6e2c 2072 6566 6572 2074  duction, refer t
-00001160: 6f20 7468 6520 646f 6375 6d65 6e74 6174  o the documentat
-00001170: 696f 6e20 6f66 2074 6865 2063 686f 7365  ion of the chose
-00001180: 6e20 4153 4749 2073 6572 7665 720a 2869  n ASGI server.(i
-00001190: 2e65 2e20 666f 7220 5b75 7669 636f 726e  .e. for [uvicorn
-000011a0: 5d28 6874 7470 733a 2f2f 7777 772e 7576  ](https://www.uv
-000011b0: 6963 6f72 6e2e 6f72 672f 2372 756e 6e69  icorn.org/#runni
-000011c0: 6e67 2d77 6974 682d 6775 6e69 636f 726e  ng-with-gunicorn
-000011d0: 2929 2e0a 0a23 2320 4175 746f 6d61 7469  ))...## Automati
-000011e0: 6320 6269 6e64 696e 6773 2061 6e64 2064  c bindings and d
-000011f0: 6570 656e 6465 6e63 7920 696e 6a65 6374  ependency inject
-00001200: 696f 6e0a 426c 6163 6b53 6865 6570 2073  ion.BlackSheep s
-00001210: 7570 706f 7274 7320 6175 746f 6d61 7469  upports automati
-00001220: 6320 6269 6e64 696e 6720 6f66 2076 616c  c binding of val
-00001230: 7565 7320 666f 7220 7265 7175 6573 7420  ues for request 
-00001240: 6861 6e64 6c65 7273 2c20 6279 2074 7970  handlers, by typ
-00001250: 650a 616e 6e6f 7461 7469 6f6e 206f 7220  e.annotation or 
-00001260: 6279 2063 6f6e 7665 6e74 696f 6e73 2e20  by conventions. 
-00001270: 5365 6520 5b6d 6f72 650a 6865 7265 5d28  See [more.here](
-00001280: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
-00001290: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
-000012a0: 6565 702f 7265 7175 6573 7473 2f29 2e0a  eep/requests/)..
-000012b0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-000012c0: 6461 7461 636c 6173 7365 7320 696d 706f  dataclasses impo
-000012d0: 7274 2064 6174 6163 6c61 7373 0a0a 6672  rt dataclass..fr
-000012e0: 6f6d 2062 6c61 636b 7368 6565 7020 696d  om blacksheep im
-000012f0: 706f 7274 2041 7070 6c69 6361 7469 6f6e  port Application
-00001300: 2c20 4672 6f6d 4a53 4f4e 2c20 4672 6f6d  , FromJSON, From
-00001310: 5175 6572 790a 0a0a 6170 7020 3d20 4170  Query...app = Ap
-00001320: 706c 6963 6174 696f 6e28 290a 0a0a 4064  plication()...@d
-00001330: 6174 6163 6c61 7373 0a63 6c61 7373 2043  ataclass.class C
-00001340: 7265 6174 6543 6174 496e 7075 743a 0a20  reateCatInput:. 
-00001350: 2020 206e 616d 653a 2073 7472 0a0a 0a40     name: str...@
-00001360: 6170 702e 726f 7574 6572 2e70 6f73 7428  app.router.post(
-00001370: 222f 6170 692f 6361 7473 2229 0a61 7379  "/api/cats").asy
-00001380: 6e63 2064 6566 2065 7861 6d70 6c65 2864  nc def example(d
-00001390: 6174 613a 2046 726f 6d4a 534f 4e5b 4372  ata: FromJSON[Cr
-000013a0: 6561 7465 4361 7449 6e70 7574 5d29 3a0a  eateCatInput]):.
-000013b0: 2020 2020 2320 696e 2074 6869 7320 6578      # in this ex
-000013c0: 616d 706c 652c 2064 6174 6120 6973 2062  ample, data is b
-000013d0: 6f75 6e64 2061 7574 6f6d 6174 6963 616c  ound automatical
-000013e0: 6c79 2072 6561 6469 6e67 2074 6865 204a  ly reading the J
-000013f0: 534f 4e0a 2020 2020 2320 7061 796c 6f61  SON.    # payloa
-00001400: 6420 616e 6420 6372 6561 7469 6e67 2061  d and creating a
-00001410: 6e20 696e 7374 616e 6365 206f 6620 6043  n instance of `C
-00001420: 7265 6174 6543 6174 496e 7075 7460 0a20  reateCatInput`. 
-00001430: 2020 202e 2e2e 0a0a 0a40 6170 702e 726f     ......@app.ro
-00001440: 7574 6572 2e67 6574 2822 2f3a 6375 6c74  uter.get("/:cult
-00001450: 7572 655f 636f 6465 2f3a 6172 6561 2229  ure_code/:area")
-00001460: 0a61 7379 6e63 2064 6566 2068 6f6d 6528  .async def home(
-00001470: 6375 6c74 7572 655f 636f 6465 2c20 6172  culture_code, ar
-00001480: 6561 293a 0a20 2020 2023 2069 6e20 7468  ea):.    # in th
-00001490: 6973 2065 7861 6d70 6c65 2c20 626f 7468  is example, both
-000014a0: 2070 6172 616d 6574 6572 7320 6172 6520   parameters are 
-000014b0: 6f62 7461 696e 6564 2066 726f 6d20 726f  obtained from ro
-000014c0: 7574 6573 2077 6974 680a 2020 2020 2320  utes with.    # 
-000014d0: 6d61 7463 6869 6e67 206e 616d 6573 0a20  matching names. 
-000014e0: 2020 2072 6574 7572 6e20 6622 5265 7175     return f"Requ
-000014f0: 6573 7420 666f 723a 207b 6375 6c74 7572  est for: {cultur
-00001500: 655f 636f 6465 7d20 7b61 7265 617d 220a  e_code} {area}".
-00001510: 0a0a 4061 7070 2e72 6f75 7465 722e 6765  ..@app.router.ge
-00001520: 7428 222f 6170 692f 7072 6f64 7563 7473  t("/api/products
-00001530: 2229 0a64 6566 2067 6574 5f70 726f 6475  ").def get_produ
-00001540: 6374 7328 0a20 2020 2070 6167 653a 2069  cts(.    page: i
-00001550: 6e74 203d 2031 2c0a 2020 2020 7369 7a65  nt = 1,.    size
-00001560: 3a20 696e 7420 3d20 3330 2c0a 2020 2020  : int = 30,.    
-00001570: 7365 6172 6368 3a20 7374 7220 3d20 2222  search: str = ""
-00001580: 2c0a 293a 0a20 2020 2023 2074 6869 7320  ,.):.    # this 
-00001590: 6578 616d 706c 6520 696c 6c75 7374 7261  example illustra
-000015a0: 7465 7320 7375 7070 6f72 7420 666f 7220  tes support for 
-000015b0: 696d 706c 6963 6974 2071 7565 7279 2070  implicit query p
-000015c0: 6172 616d 6574 6572 7320 7769 7468 0a20  arameters with. 
-000015d0: 2020 2023 2064 6566 6175 6c74 2076 616c     # default val
-000015e0: 7565 730a 2020 2020 2320 7369 6e63 6520  ues.    # since 
-000015f0: 7468 6520 736f 7572 6365 206f 6620 7061  the source of pa
-00001600: 6765 2c20 7369 7a65 2c20 616e 6420 7365  ge, size, and se
-00001610: 6172 6368 2069 7320 6e6f 7420 7370 6563  arch is not spec
-00001620: 6966 6965 6420 616e 6420 6e6f 0a20 2020  ified and no.   
-00001630: 2023 2072 6f75 7465 2070 6172 616d 6574   # route paramet
-00001640: 6572 206d 6174 6368 6573 2074 6865 6972  er matches their
-00001650: 206e 616d 652c 2074 6865 7920 6172 6520   name, they are 
-00001660: 6f62 7461 696e 6564 2066 726f 6d20 7175  obtained from qu
-00001670: 6572 7920 7374 7269 6e67 0a20 2020 202e  ery string.    .
-00001680: 2e2e 0a0a 0a40 6170 702e 726f 7574 6572  .....@app.router
-00001690: 2e67 6574 2822 2f61 7069 2f70 726f 6475  .get("/api/produ
-000016a0: 6374 7332 2229 0a64 6566 2067 6574 5f70  cts2").def get_p
-000016b0: 726f 6475 6374 7332 280a 2020 2020 7061  roducts2(.    pa
-000016c0: 6765 3a20 4672 6f6d 5175 6572 795b 696e  ge: FromQuery[in
-000016d0: 745d 203d 2046 726f 6d51 7565 7279 2831  t] = FromQuery(1
-000016e0: 292c 0a20 2020 2073 697a 653a 2046 726f  ),.    size: Fro
-000016f0: 6d51 7565 7279 5b69 6e74 5d20 3d20 4672  mQuery[int] = Fr
-00001700: 6f6d 5175 6572 7928 3330 292c 0a20 2020  omQuery(30),.   
-00001710: 2073 6561 7263 683a 2046 726f 6d51 7565   search: FromQue
-00001720: 7279 5b73 7472 5d20 3d20 4672 6f6d 5175  ry[str] = FromQu
-00001730: 6572 7928 2222 292c 0a29 3a0a 2020 2020  ery(""),.):.    
-00001740: 2320 7468 6973 2065 7861 6d70 6c65 2069  # this example i
-00001750: 6c6c 7573 7472 6174 6573 2073 7570 706f  llustrates suppo
-00001760: 7274 2066 6f72 2065 7870 6c69 6369 7420  rt for explicit 
-00001770: 7175 6572 7920 7061 7261 6d65 7465 7273  query parameters
-00001780: 2077 6974 680a 2020 2020 2320 6465 6661   with.    # defa
-00001790: 756c 7420 7661 6c75 6573 0a20 2020 2023  ult values.    #
-000017a0: 2069 6e20 7468 6973 2063 6173 652c 2070   in this case, p
-000017b0: 6172 616d 6574 6572 7320 6172 6520 6578  arameters are ex
-000017c0: 706c 6963 6974 6c79 2072 6561 6420 6672  plicitly read fr
-000017d0: 6f6d 2071 7565 7279 2073 7472 696e 670a  om query string.
-000017e0: 2020 2020 2e2e 2e0a 0a60 6060 0a0a 4974      .....```..It
-000017f0: 2061 6c73 6f20 7375 7070 6f72 7473 205b   also supports [
-00001800: 6465 7065 6e64 656e 6379 0a69 6e6a 6563  dependency.injec
-00001810: 7469 6f6e 5d28 6874 7470 733a 2f2f 7777  tion](https://ww
-00001820: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
-00001830: 6c61 636b 7368 6565 702f 6465 7065 6e64  lacksheep/depend
-00001840: 656e 6379 2d69 6e6a 6563 7469 6f6e 2f29  ency-injection/)
-00001850: 2c20 610a 6665 6174 7572 6520 7468 6174  , a.feature that
-00001860: 2070 726f 7669 6465 7320 6120 636f 6e73   provides a cons
-00001870: 6973 7465 6e74 2061 6e64 2063 6c65 616e  istent and clean
-00001880: 2077 6179 2074 6f20 7573 6520 6465 7065   way to use depe
-00001890: 6e64 656e 6369 6573 2069 6e20 7265 7175  ndencies in requ
-000018a0: 6573 740a 6861 6e64 6c65 7273 2e0a 0a23  est.handlers...#
-000018b0: 2320 4765 6e65 7261 7469 6f6e 206f 6620  # Generation of 
-000018c0: 4f70 656e 4150 4920 446f 6375 6d65 6e74  OpenAPI Document
-000018d0: 6174 696f 6e0a 5b47 656e 6572 6174 696f  ation.[Generatio
-000018e0: 6e20 6f66 204f 7065 6e41 5049 2044 6f63  n of OpenAPI Doc
-000018f0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00001900: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
-00001910: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
-00001920: 6f70 656e 6170 692f 292e 0a0a 2323 2053  openapi/)...## S
-00001930: 7472 6174 6567 6965 7320 746f 2068 616e  trategies to han
-00001940: 646c 6520 6175 7468 656e 7469 6361 7469  dle authenticati
-00001950: 6f6e 2061 6e64 2061 7574 686f 7269 7a61  on and authoriza
-00001960: 7469 6f6e 0a42 6c61 636b 5368 6565 7020  tion.BlackSheep 
-00001970: 696d 706c 656d 656e 7473 2073 7472 6174  implements strat
-00001980: 6567 6965 7320 746f 2068 616e 646c 6520  egies to handle 
-00001990: 6175 7468 656e 7469 6361 7469 6f6e 2061  authentication a
-000019a0: 6e64 2061 7574 686f 7269 7a61 7469 6f6e  nd authorization
-000019b0: 2e0a 5468 6573 6520 6665 6174 7572 6573  ..These features
-000019c0: 2061 7265 2064 6f63 756d 656e 7465 6420   are documented 
-000019d0: 6865 7265 3a0a 0a2a 205b 4175 7468 656e  here:..* [Authen
-000019e0: 7469 6361 7469 6f6e 5d28 6874 7470 733a  tication](https:
-000019f0: 2f2f 7777 772e 6e65 6f74 6572 6f69 2e64  //www.neoteroi.d
-00001a00: 6576 2f62 6c61 636b 7368 6565 702f 6175  ev/blacksheep/au
-00001a10: 7468 656e 7469 6361 7469 6f6e 2f29 0a2a  thentication/).*
-00001a20: 205b 4175 7468 6f72 697a 6174 696f 6e5d   [Authorization]
-00001a30: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
-00001a40: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
-00001a50: 6865 6570 2f61 7574 686f 7269 7a61 7469  heep/authorizati
-00001a60: 6f6e 2f29 0a0a 6060 6070 7974 686f 6e0a  on/)..```python.
-00001a70: 6170 702e 7573 655f 6175 7468 656e 7469  app.use_authenti
-00001a80: 6361 7469 6f6e 2829 5c0a 2020 2020 2e61  cation()\.    .a
-00001a90: 6464 2845 7861 6d70 6c65 4175 7468 656e  dd(ExampleAuthen
-00001aa0: 7469 6361 7469 6f6e 4861 6e64 6c65 7228  ticationHandler(
-00001ab0: 2929 0a0a 0a61 7070 2e75 7365 5f61 7574  ))...app.use_aut
-00001ac0: 686f 7269 7a61 7469 6f6e 2829 5c0a 2020  horization()\.  
-00001ad0: 2020 2e61 6464 2841 646d 696e 7350 6f6c    .add(AdminsPol
-00001ae0: 6963 7928 2929 0a0a 0a40 6175 7468 2822  icy())...@auth("
-00001af0: 6164 6d69 6e22 290a 4061 7070 2e72 6f75  admin").@app.rou
-00001b00: 7465 722e 6765 7428 222f 2229 0a61 7379  ter.get("/").asy
-00001b10: 6e63 2064 6566 206f 6e6c 795f 666f 725f  nc def only_for_
-00001b20: 6164 6d69 6e73 2829 3a0a 2020 2020 2e2e  admins():.    ..
-00001b30: 2e0a 0a0a 4061 7574 6828 290a 4061 7070  ....@auth().@app
-00001b40: 2e72 6f75 7465 722e 6765 7428 222f 2229  .router.get("/")
-00001b50: 0a61 7379 6e63 2064 6566 206f 6e6c 795f  .async def only_
-00001b60: 666f 725f 6175 7468 656e 7469 6361 7465  for_authenticate
-00001b70: 645f 7573 6572 7328 293a 0a20 2020 202e  d_users():.    .
-00001b80: 2e2e 0a60 6060 0a0a 5369 6e63 6520 7665  ...```..Since ve
-00001b90: 7273 696f 6e20 6031 2e32 2e31 602c 2042  rsion `1.2.1`, B
-00001ba0: 6c61 636b 5368 6565 7020 696d 706c 656d  lackSheep implem
-00001bb0: 656e 7473 3a0a 0a2a 205b 4275 696c 742d  ents:..* [Built-
-00001bc0: 696e 2073 7570 706f 7274 2066 6f72 204f  in support for O
-00001bd0: 7065 6e49 4420 436f 6e6e 6563 7420 6175  penID Connect au
-00001be0: 7468 656e 7469 6361 7469 6f6e 5d28 6874  thentication](ht
-00001bf0: 7470 733a 2f2f 7777 772e 6e65 6f74 6572  tps://www.neoter
-00001c00: 6f69 2e64 6576 2f62 6c61 636b 7368 6565  oi.dev/blackshee
-00001c10: 702f 6175 7468 656e 7469 6361 7469 6f6e  p/authentication
-00001c20: 2f23 6f69 6463 290a 2a20 5b42 7569 6c74  /#oidc).* [Built
-00001c30: 2d69 6e20 7375 7070 6f72 7420 666f 7220  -in support for 
-00001c40: 4a57 5420 4265 6172 6572 2061 7574 6865  JWT Bearer authe
-00001c50: 6e74 6963 6174 696f 6e5d 2868 7474 7073  ntication](https
-00001c60: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-00001c70: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
-00001c80: 7574 6865 6e74 6963 6174 696f 6e2f 236a  uthentication/#j
-00001c90: 7774 2d62 6561 7265 7229 0a0a 4d65 616e  wt-bearer)..Mean
-00001ca0: 696e 6720 7468 6174 2069 7420 6973 2065  ing that it is e
-00001cb0: 6173 7920 746f 2069 6e74 6567 7261 7465  asy to integrate
-00001cc0: 2077 6974 6820 7365 7276 6963 6573 2073   with services s
-00001cd0: 7563 6820 6173 3a0a 2a20 5b41 7574 6830  uch as:.* [Auth0
-00001ce0: 5d28 6874 7470 733a 2f2f 6175 7468 302e  ](https://auth0.
-00001cf0: 636f 6d29 0a2a 205b 417a 7572 6520 4163  com).* [Azure Ac
-00001d00: 7469 7665 2044 6972 6563 746f 7279 5d28  tive Directory](
-00001d10: 6874 7470 733a 2f2f 617a 7572 652e 6d69  https://azure.mi
-00001d20: 6372 6f73 6f66 742e 636f 6d2f 656e 2d75  crosoft.com/en-u
-00001d30: 732f 7365 7276 6963 6573 2f61 6374 6976  s/services/activ
-00001d40: 652d 6469 7265 6374 6f72 792f 290a 2a20  e-directory/).* 
-00001d50: 5b41 7a75 7265 2041 6374 6976 6520 4469  [Azure Active Di
-00001d60: 7265 6374 6f72 7920 4232 435d 2868 7474  rectory B2C](htt
-00001d70: 7073 3a2f 2f64 6f63 732e 6d69 6372 6f73  ps://docs.micros
-00001d80: 6f66 742e 636f 6d2f 656e 2d75 732f 617a  oft.com/en-us/az
-00001d90: 7572 652f 6163 7469 7665 2d64 6972 6563  ure/active-direc
-00001da0: 746f 7279 2d62 3263 2f6f 7665 7276 6965  tory-b2c/overvie
-00001db0: 7729 0a2a 205b 4f6b 7461 5d28 6874 7470  w).* [Okta](http
-00001dc0: 733a 2f2f 7777 772e 6f6b 7461 2e63 6f6d  s://www.okta.com
-00001dd0: 290a 0a52 6566 6572 2074 6f20 7468 6520  )..Refer to the 
-00001de0: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00001df0: 7220 6d6f 7265 2064 6574 6169 6c73 2061  r more details a
-00001e00: 6e64 2065 7861 6d70 6c65 732e 0a0a 2323  nd examples...##
-00001e10: 2057 6562 2066 7261 6d65 776f 726b 2066   Web framework f
-00001e20: 6561 7475 7265 730a 0a2a 205b 4153 4749  eatures..* [ASGI
-00001e30: 2063 6f6d 7061 7469 6269 6c69 7479 5d28   compatibility](
-00001e40: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
-00001e50: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
-00001e60: 6565 702f 6173 6769 2f29 0a2a 205b 526f  eep/asgi/).* [Ro
-00001e70: 7574 696e 675d 2868 7474 7073 3a2f 2f77  uting](https://w
-00001e80: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00001e90: 626c 6163 6b73 6865 6570 2f72 6f75 7469  blacksheep/routi
-00001ea0: 6e67 2f29 0a2a 2052 6571 7565 7374 2068  ng/).* Request h
-00001eb0: 616e 646c 6572 7320 6361 6e20 6265 205b  andlers can be [
-00001ec0: 6465 6669 6e65 6420 6173 0a20 2066 756e  defined as.  fun
-00001ed0: 6374 696f 6e73 5d28 6874 7470 733a 2f2f  ctions](https://
-00001ee0: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-00001ef0: 2f62 6c61 636b 7368 6565 702f 7265 7175  /blacksheep/requ
-00001f00: 6573 742d 6861 6e64 6c65 7273 2f29 2c20  est-handlers/), 
-00001f10: 6f72 205b 636c 6173 730a 2020 6d65 7468  or [class.  meth
-00001f20: 6f64 735d 2868 7474 7073 3a2f 2f77 7777  ods](https://www
-00001f30: 2e6e 656f 7465 726f 692e 6465 762f 626c  .neoteroi.dev/bl
-00001f40: 6163 6b73 6865 6570 2f63 6f6e 7472 6f6c  acksheep/control
-00001f50: 6c65 7273 2f29 0a2a 205b 4d69 6464 6c65  lers/).* [Middle
-00001f60: 7761 7265 735d 2868 7474 7073 3a2f 2f77  wares](https://w
-00001f70: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00001f80: 626c 6163 6b73 6865 6570 2f6d 6964 646c  blacksheep/middl
-00001f90: 6577 6172 6573 2f29 0a2a 205b 5765 6253  ewares/).* [WebS
-00001fa0: 6f63 6b65 745d 2868 7474 7073 3a2f 2f77  ocket](https://w
-00001fb0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00001fc0: 626c 6163 6b73 6865 6570 2f77 6562 736f  blacksheep/webso
-00001fd0: 636b 6574 2f29 0a2a 205b 4275 696c 742d  cket/).* [Built-
-00001fe0: 696e 2073 7570 706f 7274 2066 6f72 2064  in support for d
-00001ff0: 6570 656e 6465 6e63 790a 2020 696e 6a65  ependency.  inje
-00002000: 6374 696f 6e5d 2868 7474 7073 3a2f 2f77  ction](https://w
-00002010: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00002020: 626c 6163 6b73 6865 6570 2f64 6570 656e  blacksheep/depen
-00002030: 6465 6e63 792d 696e 6a65 6374 696f 6e2f  dency-injection/
-00002040: 290a 2a20 5b53 7570 706f 7274 2066 6f72  ).* [Support for
-00002050: 2061 7574 6f6d 6174 6963 2062 696e 6469   automatic bindi
-00002060: 6e67 206f 6620 726f 7574 6520 616e 6420  ng of route and 
-00002070: 7175 6572 7920 7061 7261 6d65 7465 7273  query parameters
-00002080: 2074 6f20 7265 7175 6573 740a 2020 6861   to request.  ha
-00002090: 6e64 6c65 7273 206d 6574 686f 6473 0a20  ndlers methods. 
-000020a0: 2063 616c 6c73 5d28 6874 7470 733a 2f2f   calls](https://
-000020b0: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-000020c0: 2f62 6c61 636b 7368 6565 702f 6765 7474  /blacksheep/gett
-000020d0: 696e 672d 7374 6172 7465 642f 2368 616e  ing-started/#han
-000020e0: 646c 696e 672d 726f 7574 652d 7061 7261  dling-route-para
-000020f0: 6d65 7465 7273 290a 2a20 5b53 7472 6174  meters).* [Strat
-00002100: 6567 7920 746f 2068 616e 646c 650a 2020  egy to handle.  
-00002110: 6578 6365 7074 696f 6e73 5d28 6874 7470  exceptions](http
-00002120: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
-00002130: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
-00002140: 6170 706c 6963 6174 696f 6e2f 2363 6f6e  application/#con
-00002150: 6669 6775 7269 6e67 2d65 7863 6570 7469  figuring-excepti
-00002160: 6f6e 732d 6861 6e64 6c65 7273 290a 2a20  ons-handlers).* 
-00002170: 5b53 7472 6174 6567 7920 746f 2068 616e  [Strategy to han
-00002180: 646c 6520 6175 7468 656e 7469 6361 7469  dle authenticati
-00002190: 6f6e 2061 6e64 0a20 2061 7574 686f 7269  on and.  authori
-000021a0: 7a61 7469 6f6e 5d28 6874 7470 733a 2f2f  zation](https://
-000021b0: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-000021c0: 2f62 6c61 636b 7368 6565 702f 6175 7468  /blacksheep/auth
-000021d0: 656e 7469 6361 7469 6f6e 2f29 0a2a 205b  entication/).* [
-000021e0: 4275 696c 742d 696e 2073 7570 706f 7274  Built-in support
-000021f0: 2066 6f72 204f 7065 6e49 4420 436f 6e6e   for OpenID Conn
-00002200: 6563 7420 6175 7468 656e 7469 6361 7469  ect authenticati
-00002210: 6f6e 2075 7369 6e67 204f 4944 430a 2020  on using OIDC.  
-00002220: 6469 7363 6f76 6572 795d 2868 7474 7073  discovery](https
-00002230: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-00002240: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
-00002250: 7574 6865 6e74 6963 6174 696f 6e2f 236f  uthentication/#o
-00002260: 6964 6329 0a2a 205b 4275 696c 742d 696e  idc).* [Built-in
-00002270: 2073 7570 706f 7274 2066 6f72 204a 5754   support for JWT
-00002280: 2042 6561 7265 7220 6175 7468 656e 7469   Bearer authenti
-00002290: 6361 7469 6f6e 2075 7369 6e67 204f 4944  cation using OID
-000022a0: 4320 6469 7363 6f76 6572 7920 616e 640a  C discovery and.
-000022b0: 2020 6f74 6865 7220 736f 7572 6365 7320    other sources 
-000022c0: 6f66 0a20 204a 574b 535d 2868 7474 7073  of.  JWKS](https
-000022d0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-000022e0: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
-000022f0: 7574 6865 6e74 6963 6174 696f 6e2f 236a  uthentication/#j
-00002300: 7774 2d62 6561 7265 7229 0a2a 205b 4861  wt-bearer).* [Ha
-00002310: 6e64 6c65 7273 0a20 206e 6f72 6d61 6c69  ndlers.  normali
-00002320: 7a61 7469 6f6e 5d28 6874 7470 733a 2f2f  zation](https://
-00002330: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-00002340: 2f62 6c61 636b 7368 6565 702f 7265 7175  /blacksheep/requ
-00002350: 6573 742d 6861 6e64 6c65 7273 2f29 0a2a  est-handlers/).*
-00002360: 205b 5365 7276 696e 6720 7374 6174 6963   [Serving static
-00002370: 0a20 2066 696c 6573 5d28 6874 7470 733a  .  files](https:
-00002380: 2f2f 7777 772e 6e65 6f74 6572 6f69 2e64  //www.neoteroi.d
-00002390: 6576 2f62 6c61 636b 7368 6565 702f 7374  ev/blacksheep/st
-000023a0: 6174 6963 2d66 696c 6573 2f29 0a2a 205b  atic-files/).* [
-000023b0: 496e 7465 6772 6174 696f 6e20 7769 7468  Integration with
-000023c0: 0a20 204a 696e 6a61 325d 2868 7474 7073  .  Jinja2](https
-000023d0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-000023e0: 6465 762f 626c 6163 6b73 6865 6570 2f74  dev/blacksheep/t
-000023f0: 656d 706c 6174 696e 672f 290a 2a20 5b53  emplating/).* [S
-00002400: 7570 706f 7274 2066 6f72 2073 6572 7669  upport for servi
-00002410: 6e67 2053 5041 7320 7468 6174 2075 7365  ng SPAs that use
-00002420: 2048 544d 4c35 2048 6973 746f 7279 2041   HTML5 History A
-00002430: 5049 2066 6f72 2063 6c69 656e 7420 7369  PI for client si
-00002440: 6465 0a20 2072 6f75 7469 6e67 5d28 6874  de.  routing](ht
-00002450: 7470 733a 2f2f 7777 772e 6e65 6f74 6572  tps://www.neoter
-00002460: 6f69 2e64 6576 2f62 6c61 636b 7368 6565  oi.dev/blackshee
-00002470: 702f 7374 6174 6963 2d66 696c 6573 2f23  p/static-files/#
-00002480: 686f 772d 746f 2d73 6572 7665 2d73 7061  how-to-serve-spa
-00002490: 732d 7468 6174 2d75 7365 2d68 746d 6c35  s-that-use-html5
-000024a0: 2d68 6973 746f 7279 2d61 7069 290a 2a20  -history-api).* 
-000024b0: 5b53 7570 706f 7274 2066 6f72 2061 7574  [Support for aut
-000024c0: 6f6d 6174 6963 2067 656e 6572 6174 696f  omatic generatio
-000024d0: 6e20 6f66 204f 7065 6e41 5049 0a20 2044  n of OpenAPI.  D
-000024e0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000024f0: 7470 733a 2f2f 7777 772e 6e65 6f74 6572  tps://www.neoter
-00002500: 6f69 2e64 6576 2f62 6c61 636b 7368 6565  oi.dev/blackshee
-00002510: 702f 6f70 656e 6170 692f 290a 2a20 5b53  p/openapi/).* [S
-00002520: 7472 6174 6567 7920 746f 2068 616e 646c  trategy to handl
-00002530: 6520 434f 5253 2073 6574 7469 6e67 735d  e CORS settings]
-00002540: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
-00002550: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
-00002560: 6865 6570 2f63 6f72 732f 290a 2a20 5b53  heep/cors/).* [S
-00002570: 6573 7369 6f6e 735d 2868 7474 7073 3a2f  essions](https:/
-00002580: 2f77 7777 2e6e 656f 7465 726f 692e 6465  /www.neoteroi.de
-00002590: 762f 626c 6163 6b73 6865 6570 2f73 6573  v/blacksheep/ses
-000025a0: 7369 6f6e 732f 290a 2a20 5375 7070 6f72  sions/).* Suppor
-000025b0: 7420 666f 7220 6175 746f 6d61 7469 6320  t for automatic 
-000025c0: 6269 6e64 696e 6720 6f66 2060 6461 7461  binding of `data
-000025d0: 636c 6173 7365 7360 2061 6e64 0a20 205b  classes` and.  [
-000025e0: 6070 7964 616e 7469 6360 5d28 6874 7470  `pydantic`](http
-000025f0: 733a 2f2f 7079 6461 6e74 6963 2d64 6f63  s://pydantic-doc
-00002600: 732e 6865 6c70 6d61 6e75 616c 2e69 6f29  s.helpmanual.io)
-00002610: 206d 6f64 656c 7320 746f 2068 616e 646c   models to handl
-00002620: 6520 7468 650a 2020 7265 7175 6573 7420  e the.  request 
-00002630: 626f 6479 2070 6179 6c6f 6164 2065 7870  body payload exp
-00002640: 6563 7465 6420 6279 2072 6571 7565 7374  ected by request
-00002650: 2068 616e 646c 6572 730a 2a20 5b60 5465   handlers.* [`Te
-00002660: 7374 436c 6965 6e74 6020 636c 6173 7320  stClient` class 
-00002670: 746f 2073 696d 706c 6966 7920 7465 7374  to simplify test
-00002680: 696e 6720 6f66 2061 7070 6c69 6361 7469  ing of applicati
-00002690: 6f6e 735d 2868 7474 7073 3a2f 2f77 7777  ons](https://www
-000026a0: 2e6e 656f 7465 726f 692e 6465 762f 626c  .neoteroi.dev/bl
-000026b0: 6163 6b73 6865 6570 2f74 6573 7469 6e67  acksheep/testing
-000026c0: 2f29 0a2a 205b 416e 7469 2046 6f72 6765  /).* [Anti Forge
-000026d0: 7279 2076 616c 6964 6174 696f 6e5d 2868  ry validation](h
-000026e0: 7474 7073 3a2f 2f77 7777 2e6e 656f 7465  ttps://www.neote
-000026f0: 726f 692e 6465 762f 626c 6163 6b73 6865  roi.dev/blackshe
-00002700: 6570 2f61 6e74 692d 7265 7175 6573 742d  ep/anti-request-
-00002710: 666f 7267 6572 7929 2074 6f20 7072 6f74  forgery) to prot
-00002720: 6563 7420 6167 6169 6e73 7420 4372 6f73  ect against Cros
-00002730: 732d 5369 7465 2052 6571 7565 7374 2046  s-Site Request F
-00002740: 6f72 6765 7279 2028 5853 5246 2f43 5352  orgery (XSRF/CSR
-00002750: 4629 2061 7474 6163 6b73 0a0a 2323 2043  F) attacks..## C
-00002760: 6c69 656e 7420 6665 6174 7572 6573 0a0a  lient features..
-00002770: 426c 6163 6b53 6865 6570 2069 6e63 6c75  BlackSheep inclu
-00002780: 6465 7320 616e 2048 5454 5020 436c 6965  des an HTTP Clie
-00002790: 6e74 2e0a 0a2a 2a45 7861 6d70 6c65 3a2a  nt...**Example:*
-000027a0: 2a0a 6060 6070 7974 686f 6e0a 696d 706f  *.```python.impo
-000027b0: 7274 2061 7379 6e63 696f 0a0a 6672 6f6d  rt asyncio..from
-000027c0: 2062 6c61 636b 7368 6565 702e 636c 6965   blacksheep.clie
-000027d0: 6e74 2069 6d70 6f72 7420 436c 6965 6e74  nt import Client
-000027e0: 5365 7373 696f 6e0a 0a0a 6173 796e 6320  Session...async 
-000027f0: 6465 6620 636c 6965 6e74 5f65 7861 6d70  def client_examp
-00002800: 6c65 2829 3a0a 2020 2020 6173 796e 6320  le():.    async 
-00002810: 7769 7468 2043 6c69 656e 7453 6573 7369  with ClientSessi
-00002820: 6f6e 2829 2061 7320 636c 6965 6e74 3a0a  on() as client:.
-00002830: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00002840: 203d 2061 7761 6974 2063 6c69 656e 742e   = await client.
-00002850: 6765 7428 2268 7474 7073 3a2f 2f64 6f63  get("https://doc
-00002860: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f22  s.python.org/3/"
-00002870: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00002880: 7420 7265 7370 6f6e 7365 2069 7320 6e6f  t response is no
-00002890: 7420 4e6f 6e65 0a20 2020 2020 2020 2074  t None.        t
-000028a0: 6578 7420 3d20 6177 6169 7420 7265 7370  ext = await resp
-000028b0: 6f6e 7365 2e74 6578 7428 290a 2020 2020  onse.text().    
-000028c0: 2020 2020 7072 696e 7428 7465 7874 290a      print(text).
-000028d0: 0a0a 6173 796e 6369 6f2e 7275 6e28 636c  ..asyncio.run(cl
-000028e0: 6965 6e74 5f65 7861 6d70 6c65 2829 290a  ient_example()).
-000028f0: 6060 600a 0a23 2320 5375 7070 6f72 7465  ```..## Supporte
-00002900: 6420 706c 6174 666f 726d 7320 616e 6420  d platforms and 
-00002910: 7275 6e74 696d 6573 0a2a 2050 7974 686f  runtimes.* Pytho
-00002920: 6e3a 2061 6c6c 2076 6572 7369 6f6e 7320  n: all versions 
-00002930: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
-00002940: 6275 696c 6420 6d61 7472 6978 0a2a 2055  build matrix.* U
-00002950: 6275 6e74 750a 2a20 5769 6e64 6f77 7320  buntu.* Windows 
-00002960: 3130 0a2a 206d 6163 4f53 0a0a 2323 2044  10.* macOS..## D
-00002970: 6f63 756d 656e 7461 7469 6f6e 0a50 6c65  ocumentation.Ple
-00002980: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
-00002990: 205b 646f 6375 6d65 6e74 6174 696f 6e20   [documentation 
-000029a0: 7765 6273 6974 655d 2868 7474 7073 3a2f  website](https:/
-000029b0: 2f77 7777 2e6e 656f 7465 726f 692e 6465  /www.neoteroi.de
-000029c0: 762f 626c 6163 6b73 6865 6570 2f29 2e0a  v/blacksheep/)..
-000029d0: 0a23 2320 436f 6d6d 756e 6963 6174 696f  .## Communicatio
-000029e0: 6e0a 5b42 6c61 636b 5368 6565 7020 636f  n.[BlackSheep co
-000029f0: 6d6d 756e 6974 7920 696e 2047 6974 7465  mmunity in Gitte
-00002a00: 725d 2868 7474 7073 3a2f 2f67 6974 7465  r](https://gitte
-00002a10: 722e 696d 2f4e 656f 7465 726f 692f 426c  r.im/Neoteroi/Bl
-00002a20: 6163 6b53 6865 6570 292e 0a0a 2323 2042  ackSheep)...## B
-00002a30: 7261 6e63 6865 730a 5468 6520 5f6d 6169  ranches.The _mai
-00002a40: 6e5f 2062 7261 6e63 6820 636f 6e74 6169  n_ branch contai
-00002a50: 6e73 2074 6865 2063 7572 7265 6e74 6c79  ns the currently
-00002a60: 2064 6576 656c 6f70 6564 2076 6572 7369   developed versi
-00002a70: 6f6e 2c20 7768 6963 6820 6973 2076 6572  on, which is ver
-00002a80: 7369 6f6e 2032 0a61 6c70 6861 2e20 5468  sion 2.alpha. Th
-00002a90: 6520 5f76 315f 2062 7261 6e63 6820 636f  e _v1_ branch co
-00002aa0: 6e74 6169 6e73 2076 6572 7369 6f6e 2031  ntains version 1
-00002ab0: 206f 6620 7468 6520 7765 6220 6672 616d   of the web fram
-00002ac0: 6577 6f72 6b2c 2066 6f72 2062 7567 7320  ework, for bugs 
-00002ad0: 6669 7865 730a 616e 6420 6d61 696e 7465  fixes.and mainte
-00002ae0: 6e61 6e63 652e 0a                        nance..
+00000010: 3a20 322e 310d 0a4e 616d 653a 2062 6c61  : 2.1..Name: bla
+00000020: 636b 7368 6565 700d 0a56 6572 7369 6f6e  cksheep..Version
+00000030: 3a20 322e 3061 390d 0a53 756d 6d61 7279  : 2.0a9..Summary
+00000040: 3a20 4661 7374 2077 6562 2066 7261 6d65  : Fast web frame
+00000050: 776f 726b 2066 6f72 2050 7974 686f 6e20  work for Python 
+00000060: 6173 796e 6369 6f0d 0a41 7574 686f 722d  asyncio..Author-
+00000070: 656d 6169 6c3a 2052 6f62 6572 746f 2050  email: Roberto P
+00000080: 7265 7661 746f 203c 726f 6265 7274 6f2e  revato <roberto.
+00000090: 7072 6576 6174 6f40 676d 6169 6c2e 636f  prevato@gmail.co
+000000a0: 6d3e 0d0a 5072 6f6a 6563 742d 5552 4c3a  m>..Project-URL:
+000000b0: 2048 6f6d 6570 6167 652c 2068 7474 7073   Homepage, https
+000000c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e65  ://github.com/Ne
+000000d0: 6f74 6572 6f69 2f42 6c61 636b 5368 6565  oteroi/BlackShee
+000000e0: 700d 0a50 726f 6a65 6374 2d55 524c 3a20  p..Project-URL: 
+000000f0: 4275 6720 5472 6163 6b65 722c 2068 7474  Bug Tracker, htt
+00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000110: 4e65 6f74 6572 6f69 2f42 6c61 636b 5368  Neoteroi/BlackSh
+00000120: 6565 702f 6973 7375 6573 0d0a 4b65 7977  eep/issues..Keyw
+00000130: 6f72 6473 3a20 626c 6163 6b73 6865 6570  ords: blacksheep
+00000140: 2c77 6562 2066 7261 6d65 776f 726b 2c61  ,web framework,a
+00000150: 7379 6e63 696f 0d0a 436c 6173 7369 6669  syncio..Classifi
+00000160: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+00000170: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
+00000180: 7068 610d 0a43 6c61 7373 6966 6965 723a  pha..Classifier:
+00000190: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+000001a0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000001b0: 4c69 6365 6e73 650d 0a43 6c61 7373 6966  License..Classif
+000001c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001e0: 686f 6e20 3a3a 2033 2e38 0d0a 436c 6173  hon :: 3.8..Clas
+000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000210: 5079 7468 6f6e 203a 3a20 332e 390d 0a43  Python :: 3.9..C
+00000220: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000250: 300d 0a43 6c61 7373 6966 6965 723a 2050  0..Classifier: P
+00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000280: 2033 2e31 310d 0a43 6c61 7373 6966 6965   3.11..Classifie
+00000290: 723a 2045 6e76 6972 6f6e 6d65 6e74 203a  r: Environment :
+000002a0: 3a20 5765 6220 456e 7669 726f 6e6d 656e  : Web Environmen
+000002b0: 740d 0a43 6c61 7373 6966 6965 723a 204f  t..Classifier: O
+000002c0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000002d0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000002e0: 740d 0a43 6c61 7373 6966 6965 723a 2046  t..Classifier: F
+000002f0: 7261 6d65 776f 726b 203a 3a20 4173 796e  ramework :: Asyn
+00000300: 6349 4f0d 0a52 6571 7569 7265 732d 5079  cIO..Requires-Py
+00000310: 7468 6f6e 3a20 3e3d 332e 370d 0a44 6573  thon: >=3.7..Des
+00000320: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000330: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000340: 646f 776e 0d0a 5072 6f76 6964 6573 2d45  down..Provides-E
+00000350: 7874 7261 3a20 6a69 6e6a 610d 0a50 726f  xtra: jinja..Pro
+00000360: 7669 6465 732d 4578 7472 613a 2066 756c  vides-Extra: ful
+00000370: 6c0d 0a4c 6963 656e 7365 2d46 696c 653a  l..License-File:
+00000380: 204c 4943 454e 5345 0d0a 0d0a 5b21 5b42   LICENSE....[![B
+00000390: 7569 6c64 5d28 6874 7470 733a 2f2f 6769  uild](https://gi
+000003a0: 7468 7562 2e63 6f6d 2f4e 656f 7465 726f  thub.com/Neotero
+000003b0: 692f 426c 6163 6b53 6865 6570 2f77 6f72  i/BlackSheep/wor
+000003c0: 6b66 6c6f 7773 2f4d 6169 6e2f 6261 6467  kflows/Main/badg
+000003d0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000003e0: 6769 7468 7562 2e63 6f6d 2f4e 656f 7465  github.com/Neote
+000003f0: 726f 692f 426c 6163 6b53 6865 6570 2f61  roi/BlackSheep/a
+00000400: 6374 696f 6e73 290d 0a5b 215b 7079 7069  ctions)..[![pypi
+00000410: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000420: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000430: 426c 6163 6b53 6865 6570 2e73 7667 3f63  BlackSheep.svg?c
+00000440: 6f6c 6f72 3d62 6c75 6529 5d28 6874 7470  olor=blue)](http
+00000450: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000460: 6a65 6374 2f42 6c61 636b 5368 6565 702f  ject/BlackSheep/
+00000470: 290d 0a5b 215b 7665 7273 696f 6e73 5d28  )..[![versions](
+00000480: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000490: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+000004a0: 7273 696f 6e73 2f62 6c61 636b 7368 6565  rsions/blackshee
+000004b0: 702e 7376 6729 5d28 6874 7470 733a 2f2f  p.svg)](https://
+000004c0: 6769 7468 7562 2e63 6f6d 2f72 6f62 6572  github.com/rober
+000004d0: 746f 7072 6576 6174 6f2f 626c 6163 6b73  toprevato/blacks
+000004e0: 6865 6570 290d 0a5b 215b 636f 6465 636f  heep)..[![codeco
+000004f0: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000500: 6f76 2e69 6f2f 6768 2f4e 656f 7465 726f  ov.io/gh/Neotero
+00000510: 692f 426c 6163 6b53 6865 6570 2f62 7261  i/BlackSheep/bra
+00000520: 6e63 682f 6d61 7374 6572 2f67 7261 7068  nch/master/graph
+00000530: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00000540: 3d4e 7a69 3239 4c30 4567 3129 5d28 6874  =Nzi29L0Eg1)](ht
+00000550: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000560: 2f67 682f 4e65 6f74 6572 6f69 2f42 6c61  /gh/Neoteroi/Bla
+00000570: 636b 5368 6565 7029 0d0a 5b21 5b6c 6963  ckSheep)..[![lic
+00000580: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
+00000590: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000005a0: 6875 622f 6c69 6365 6e73 652f 4e65 6f74  hub/license/Neot
+000005b0: 6572 6f69 2f62 6c61 636b 7368 6565 702e  eroi/blacksheep.
+000005c0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+000005d0: 7468 7562 2e63 6f6d 2f4e 656f 7465 726f  thub.com/Neotero
+000005e0: 692f 626c 6163 6b73 6865 6570 2f62 6c6f  i/blacksheep/blo
+000005f0: 622f 6d61 696e 2f4c 4943 454e 5345 2920  b/main/LICENSE) 
+00000600: 5b21 5b4a 6f69 6e20 7468 6520 6368 6174  [![Join the chat
+00000610: 2061 7420 6874 7470 733a 2f2f 6769 7474   at https://gitt
+00000620: 6572 2e69 6d2f 4e65 6f74 6572 6f69 2f42  er.im/Neoteroi/B
+00000630: 6c61 636b 5368 6565 705d 2868 7474 7073  lackSheep](https
+00000640: 3a2f 2f62 6164 6765 732e 6769 7474 6572  ://badges.gitter
+00000650: 2e69 6d2f 4e65 6f74 6572 6f69 2f42 6c61  .im/Neoteroi/Bla
+00000660: 636b 5368 6565 702e 7376 6729 5d28 6874  ckSheep.svg)](ht
+00000670: 7470 733a 2f2f 6769 7474 6572 2e69 6d2f  tps://gitter.im/
+00000680: 4e65 6f74 6572 6f69 2f42 6c61 636b 5368  Neoteroi/BlackSh
+00000690: 6565 703f 7574 6d5f 736f 7572 6365 3d62  eep?utm_source=b
+000006a0: 6164 6765 2675 746d 5f6d 6564 6975 6d3d  adge&utm_medium=
+000006b0: 6261 6467 6526 7574 6d5f 6361 6d70 6169  badge&utm_campai
+000006c0: 676e 3d70 722d 6261 6467 6526 7574 6d5f  gn=pr-badge&utm_
+000006d0: 636f 6e74 656e 743d 6261 6467 6529 205b  content=badge) [
+000006e0: 215b 646f 6375 6d65 6e74 6174 696f 6e5d  ![documentation]
+000006f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000700: 656c 6473 2e69 6f2f 6261 6467 652f f09f  elds.io/badge/..
+00000710: 9396 2d64 6f63 732d 7075 7270 6c65 295d  ..-docs-purple)]
+00000720: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00000730: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+00000740: 6865 6570 2f29 0d0a 0d0a 2320 426c 6163  heep/)....# Blac
+00000750: 6b53 6865 6570 0d0a 426c 6163 6b53 6865  kSheep..BlackShe
+00000760: 6570 2069 7320 616e 2061 7379 6e63 6872  ep is an asynchr
+00000770: 6f6e 6f75 7320 7765 6220 6672 616d 6577  onous web framew
+00000780: 6f72 6b20 746f 2062 7569 6c64 2065 7665  ork to build eve
+00000790: 6e74 2062 6173 6564 2077 6562 0d0a 6170  nt based web..ap
+000007a0: 706c 6963 6174 696f 6e73 2077 6974 6820  plications with 
+000007b0: 5079 7468 6f6e 2e20 4974 2069 7320 696e  Python. It is in
+000007c0: 7370 6972 6564 2062 790d 0a5b 466c 6173  spired by..[Flas
+000007d0: 6b5d 2868 7474 7073 3a2f 2f70 616c 6c65  k](https://palle
+000007e0: 7473 7072 6f6a 6563 7473 2e63 6f6d 2f70  tsprojects.com/p
+000007f0: 2f66 6c61 736b 2f29 2c20 5b41 5350 2e4e  /flask/), [ASP.N
+00000800: 4554 0d0a 436f 7265 5d28 6874 7470 733a  ET..Core](https:
+00000810: 2f2f 646f 6373 2e6d 6963 726f 736f 6674  //docs.microsoft
+00000820: 2e63 6f6d 2f65 6e2d 7573 2f61 7370 6e65  .com/en-us/aspne
+00000830: 742f 636f 7265 2f29 2c20 616e 6420 7468  t/core/), and th
+00000840: 6520 776f 726b 2062 7920 5b59 7572 790d  e work by [Yury.
+00000850: 0a53 656c 6976 616e 6f76 5d28 6874 7470  .Selivanov](http
+00000860: 733a 2f2f 6d61 6769 632e 696f 2f62 6c6f  s://magic.io/blo
+00000870: 672f 7576 6c6f 6f70 2d62 6c61 7a69 6e67  g/uvloop-blazing
+00000880: 2d66 6173 742d 7079 7468 6f6e 2d6e 6574  -fast-python-net
+00000890: 776f 726b 696e 672f 292e 0d0a 0d0a 3c70  working/).....<p
+000008a0: 2061 6c69 676e 3d22 6c65 6674 223e 0d0a   align="left">..
+000008b0: 2020 3c61 2068 7265 663d 2223 626c 6163    <a href="#blac
+000008c0: 6b73 6865 6570 223e 3c69 6d67 2077 6964  ksheep"><img wid
+000008d0: 7468 3d22 3332 3022 2068 6569 6768 743d  th="320" height=
+000008e0: 2232 3731 2220 7372 633d 2268 7474 7073  "271" src="https
+000008f0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
+00000900: 6465 762f 626c 6163 6b73 6865 6570 2f69  dev/blacksheep/i
+00000910: 6d67 2f62 6c61 636b 7368 6565 702e 706e  mg/blacksheep.pn
+00000920: 6722 2061 6c74 3d22 426c 6163 6b20 5368  g" alt="Black Sh
+00000930: 6565 7022 3e3c 2f61 3e0d 0a3c 2f70 3e0d  eep"></a>..</p>.
+00000940: 0a0d 0a60 6060 6261 7368 0d0a 7069 7020  ...```bash..pip 
+00000950: 696e 7374 616c 6c20 626c 6163 6b73 6865  install blackshe
+00000960: 6570 0d0a 6060 600d 0a0d 0a2d 2d2d 0d0a  ep..```....---..
+00000970: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
+00000980: 6d20 6461 7465 7469 6d65 2069 6d70 6f72  m datetime impor
+00000990: 7420 6461 7465 7469 6d65 0d0a 0d0a 6672  t datetime....fr
+000009a0: 6f6d 2062 6c61 636b 7368 6565 7020 696d  om blacksheep im
+000009b0: 706f 7274 2041 7070 6c69 6361 7469 6f6e  port Application
+000009c0: 0d0a 0d0a 0d0a 6170 7020 3d20 4170 706c  ......app = Appl
+000009d0: 6963 6174 696f 6e28 290d 0a0d 0a40 6170  ication()....@ap
+000009e0: 702e 726f 7574 6528 222f 2229 0d0a 6173  p.route("/")..as
+000009f0: 796e 6320 6465 6620 686f 6d65 2829 3a0d  ync def home():.
+00000a00: 0a20 2020 2072 6574 7572 6e20 6622 4865  .    return f"He
+00000a10: 6c6c 6f2c 2057 6f72 6c64 2120 7b64 6174  llo, World! {dat
+00000a20: 6574 696d 652e 7574 636e 6f77 2829 2e69  etime.utcnow().i
+00000a30: 736f 666f 726d 6174 2829 7d22 0d0a 0d0a  soformat()}"....
+00000a40: 6060 600d 0a0d 0a23 2320 4765 7474 696e  ```....## Gettin
+00000a50: 6720 7374 6172 7465 6420 7573 696e 6720  g started using 
+00000a60: 7468 6520 434c 4920 e29c a80d 0a0d 0a42  the CLI .......B
+00000a70: 6c61 636b 5368 6565 7020 6f66 6665 7273  lackSheep offers
+00000a80: 2061 2043 4c49 2074 6f20 626f 6f74 7374   a CLI to bootst
+00000a90: 7261 7020 6e65 7720 7072 6f6a 6563 7473  rap new projects
+00000aa0: 2072 6170 6964 6c79 2e0d 0a54 6f20 7472   rapidly...To tr
+00000ab0: 7920 6974 2c20 6669 7273 7420 696e 7374  y it, first inst
+00000ac0: 616c 6c20 7468 6520 6062 6c61 636b 7368  all the `blacksh
+00000ad0: 6565 702d 636c 6960 2070 6163 6b61 6765  eep-cli` package
+00000ae0: 3a0d 0a0d 0a60 6060 6261 7368 0d0a 7069  :....```bash..pi
+00000af0: 7020 696e 7374 616c 6c20 626c 6163 6b73  p install blacks
+00000b00: 6865 6570 2d63 6c69 0d0a 6060 600d 0a0d  heep-cli..```...
+00000b10: 0a54 6865 6e20 7573 6520 7468 6520 6062  .Then use the `b
+00000b20: 6c61 636b 7368 6565 7020 6372 6561 7465  lacksheep create
+00000b30: 6020 636f 6d6d 616e 6420 746f 2062 6f6f  ` command to boo
+00000b40: 7473 7472 6170 2061 2070 726f 6a65 6374  tstrap a project
+00000b50: 0d0a 7573 696e 6720 6f6e 6520 6f66 2074  ..using one of t
+00000b60: 6865 2073 7570 706f 7274 6564 2074 656d  he supported tem
+00000b70: 706c 6174 6573 2e0d 0a0d 0a21 5b62 6c61  plates.....![bla
+00000b80: 636b 7368 6565 7020 6372 6561 7465 2063  cksheep create c
+00000b90: 6f6d 6d61 6e64 5d28 6874 7470 733a 2f2f  ommand](https://
+00000ba0: 6769 7374 2e67 6974 6875 6275 7365 7263  gist.githubuserc
+00000bb0: 6f6e 7465 6e74 2e63 6f6d 2f52 6f62 6572  ontent.com/Rober
+00000bc0: 746f 5072 6576 6174 6f2f 3338 6130 3539  toPrevato/38a059
+00000bd0: 3862 3531 3561 3266 3732 3537 6336 3134  8b515a2f7257c614
+00000be0: 3933 3838 3433 6239 3962 2f72 6177 2f36  938843b99b/raw/6
+00000bf0: 3764 3135 6261 3333 3764 6539 3463 3266  7d15ba337de94c2f
+00000c00: 3530 6439 3830 6137 6238 3932 3461 3734  50d980a7b8924a74
+00000c10: 3732 3539 3235 342f 626c 6163 6b73 6865  7259254/blackshe
+00000c20: 6570 2d63 7265 6174 652d 6465 6d6f 2e67  ep-create-demo.g
+00000c30: 6966 290d 0a0d 0a54 6865 2043 4c49 2069  if)....The CLI i
+00000c40: 6e63 6c75 6465 7320 6120 6865 6c70 2c20  ncludes a help, 
+00000c50: 616e 6420 7375 7070 6f72 7473 2063 7573  and supports cus
+00000c60: 746f 6d20 7465 6d70 6c61 7465 732c 2075  tom templates, u
+00000c70: 7369 6e67 2074 6865 0d0a 7361 6d65 2073  sing the..same s
+00000c80: 6f75 7263 6573 2073 7570 706f 7274 6564  ources supported
+00000c90: 2062 7920 6043 6f6f 6b69 6563 7574 7465   by `Cookiecutte
+00000ca0: 7260 2e0d 0a0d 0a23 2320 4765 7474 696e  r`.....## Gettin
+00000cb0: 6720 7374 6172 7465 6420 7769 7468 2074  g started with t
+00000cc0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00000cd0: 0d0a 0d0a 5468 6520 646f 6375 6d65 6e74  ....The document
+00000ce0: 6174 696f 6e20 6f66 6665 7273 2067 6574  ation offers get
+00000cf0: 7469 6e67 2073 7461 7274 6564 2074 7574  ting started tut
+00000d00: 6f72 6961 6c73 3a0d 0a2a 205b 4765 7474  orials:..* [Gett
+00000d10: 696e 6720 7374 6172 7465 643a 0d0a 2020  ing started:..  
+00000d20: 6261 7369 6373 5d28 6874 7470 733a 2f2f  basics](https://
+00000d30: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
+00000d40: 2f62 6c61 636b 7368 6565 702f 6765 7474  /blacksheep/gett
+00000d50: 696e 672d 7374 6172 7465 642f 290d 0a2a  ing-started/)..*
+00000d60: 205b 4765 7474 696e 6720 7374 6172 7465   [Getting starte
+00000d70: 643a 2074 6865 204d 5643 2070 726f 6a65  d: the MVC proje
+00000d80: 6374 0d0a 2020 7465 6d70 6c61 7465 5d28  ct..  template](
+00000d90: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
+00000da0: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
+00000db0: 6565 702f 6d76 632d 7072 6f6a 6563 742d  eep/mvc-project-
+00000dc0: 7465 6d70 6c61 7465 2f29 0d0a 0d0a 5468  template/)....Th
+00000dd0: 6573 6520 7072 6f6a 6563 7420 7465 6d70  ese project temp
+00000de0: 6c61 7465 7320 6361 6e20 6265 2075 7365  lates can be use
+00000df0: 6420 746f 2073 7461 7274 206e 6577 2061  d to start new a
+00000e00: 7070 6c69 6361 7469 6f6e 7320 6661 7374  pplications fast
+00000e10: 6572 3a0d 0a0d 0a2a 205b 4d56 4320 7072  er:....* [MVC pr
+00000e20: 6f6a 6563 740d 0a20 2074 656d 706c 6174  oject..  templat
+00000e30: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000e40: 622e 636f 6d2f 4e65 6f74 6572 6f69 2f42  b.com/Neoteroi/B
+00000e50: 6c61 636b 5368 6565 704d 5643 290d 0a2a  lackSheepMVC)..*
+00000e60: 205b 456d 7074 7920 7072 6f6a 6563 740d   [Empty project.
+00000e70: 0a20 2074 656d 706c 6174 655d 2868 7474  .  template](htt
+00000e80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e90: 4e65 6f74 6572 6f69 2f42 6c61 636b 5368  Neoteroi/BlackSh
+00000ea0: 6565 7045 6d70 7479 5072 6f6a 6563 7429  eepEmptyProject)
+00000eb0: 0d0a 0d0a 2323 2052 6571 7569 7265 6d65  ....## Requireme
+00000ec0: 6e74 730d 0a0d 0a5b 5079 7468 6f6e 5d28  nts....[Python](
+00000ed0: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
+00000ee0: 6f6e 2e6f 7267 293a 2061 6e79 2076 6572  on.org): any ver
+00000ef0: 7369 6f6e 206c 6973 7465 6420 696e 2074  sion listed in t
+00000f00: 6865 2070 726f 6a65 6374 2773 0d0a 636c  he project's..cl
+00000f10: 6173 7369 6669 6572 732e 2054 6865 2063  assifiers. The c
+00000f20: 7572 7265 6e74 206c 6973 7420 6973 3a0d  urrent list is:.
+00000f30: 0a0d 0a5b 215b 7665 7273 696f 6e73 5d28  ...[![versions](
+00000f40: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000f50: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000f60: 7273 696f 6e73 2f62 6c61 636b 7368 6565  rsions/blackshee
+00000f70: 702e 7376 6729 5d28 6874 7470 733a 2f2f  p.svg)](https://
+00000f80: 6769 7468 7562 2e63 6f6d 2f72 6f62 6572  github.com/rober
+00000f90: 746f 7072 6576 6174 6f2f 626c 6163 6b73  toprevato/blacks
+00000fa0: 6865 6570 290d 0a0d 0a0d 0a42 6c61 636b  heep)......Black
+00000fb0: 5368 6565 7020 6265 6c6f 6e67 7320 746f  Sheep belongs to
+00000fc0: 2074 6865 2063 6174 6567 6f72 7920 6f66   the category of
+00000fd0: 0d0a 5b41 5347 495d 2868 7474 7073 3a2f  ..[ASGI](https:/
+00000fe0: 2f61 7367 692e 7265 6164 7468 6564 6f63  /asgi.readthedoc
+00000ff0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f29  s.io/en/latest/)
+00001000: 2077 6562 2066 7261 6d65 776f 726b 732c   web frameworks,
+00001010: 2073 6f20 6974 2072 6571 7569 7265 730d   so it requires.
+00001020: 0a61 6e20 4153 4749 2048 5454 5020 7365  .an ASGI HTTP se
+00001030: 7276 6572 2074 6f20 7275 6e2c 2073 7563  rver to run, suc
+00001040: 6820 6173 205b 7576 6963 6f72 6e5d 2868  h as [uvicorn](h
+00001050: 7474 703a 2f2f 7777 772e 7576 6963 6f72  ttp://www.uvicor
+00001060: 6e2e 6f72 672f 292c 206f 720d 0a5b 6879  n.org/), or..[hy
+00001070: 7065 7263 6f72 6e5d 2868 7474 7073 3a2f  percorn](https:/
+00001080: 2f70 676a 6f6e 6573 2e67 6974 6c61 622e  /pgjones.gitlab.
+00001090: 696f 2f68 7970 6572 636f 726e 2f29 2e20  io/hypercorn/). 
+000010a0: 466f 7220 6578 616d 706c 652c 2074 6f20  For example, to 
+000010b0: 7573 6520 6974 2077 6974 680d 0a75 7669  use it with..uvi
+000010c0: 636f 726e 3a0d 0a0d 0a60 6060 6261 7368  corn:....```bash
+000010d0: 0d0a 2420 7069 7020 696e 7374 616c 6c20  ..$ pip install 
+000010e0: 7576 6963 6f72 6e0d 0a60 6060 0d0a 0d0a  uvicorn..```....
+000010f0: 546f 2072 756e 2061 6e20 6170 706c 6963  To run an applic
+00001100: 6174 696f 6e20 6c69 6b65 2069 6e20 7468  ation like in th
+00001110: 6520 6578 616d 706c 6520 6162 6f76 652c  e example above,
+00001120: 2075 7365 2074 6865 206d 6574 686f 6473   use the methods
+00001130: 2070 726f 7669 6465 6420 6279 0d0a 7468   provided by..th
+00001140: 6520 4153 4749 2048 5454 5020 5365 7276  e ASGI HTTP Serv
+00001150: 6572 3a0d 0a0d 0a60 6060 6261 7368 0d0a  er:....```bash..
+00001160: 2320 6966 2074 6865 2042 6c61 636b 5368  # if the BlackSh
+00001170: 6565 7020 6170 7020 6973 2064 6566 696e  eep app is defin
+00001180: 6564 2069 6e20 6120 6669 6c65 2060 7365  ed in a file `se
+00001190: 7276 6572 2e70 7960 0d0a 0d0a 2420 7576  rver.py`....$ uv
+000011a0: 6963 6f72 6e20 7365 7276 6572 3a61 7070  icorn server:app
+000011b0: 0d0a 6060 600d 0a0d 0a54 6f20 7275 6e20  ..```....To run 
+000011c0: 666f 7220 7072 6f64 7563 7469 6f6e 2c20  for production, 
+000011d0: 7265 6665 7220 746f 2074 6865 2064 6f63  refer to the doc
+000011e0: 756d 656e 7461 7469 6f6e 206f 6620 7468  umentation of th
+000011f0: 6520 6368 6f73 656e 2041 5347 4920 7365  e chosen ASGI se
+00001200: 7276 6572 0d0a 2869 2e65 2e20 666f 7220  rver..(i.e. for 
+00001210: 5b75 7669 636f 726e 5d28 6874 7470 733a  [uvicorn](https:
+00001220: 2f2f 7777 772e 7576 6963 6f72 6e2e 6f72  //www.uvicorn.or
+00001230: 672f 2372 756e 6e69 6e67 2d77 6974 682d  g/#running-with-
+00001240: 6775 6e69 636f 726e 2929 2e0d 0a0d 0a23  gunicorn)).....#
+00001250: 2320 4175 746f 6d61 7469 6320 6269 6e64  # Automatic bind
+00001260: 696e 6773 2061 6e64 2064 6570 656e 6465  ings and depende
+00001270: 6e63 7920 696e 6a65 6374 696f 6e0d 0a42  ncy injection..B
+00001280: 6c61 636b 5368 6565 7020 7375 7070 6f72  lackSheep suppor
+00001290: 7473 2061 7574 6f6d 6174 6963 2062 696e  ts automatic bin
+000012a0: 6469 6e67 206f 6620 7661 6c75 6573 2066  ding of values f
+000012b0: 6f72 2072 6571 7565 7374 2068 616e 646c  or request handl
+000012c0: 6572 732c 2062 7920 7479 7065 0d0a 616e  ers, by type..an
+000012d0: 6e6f 7461 7469 6f6e 206f 7220 6279 2063  notation or by c
+000012e0: 6f6e 7665 6e74 696f 6e73 2e20 5365 6520  onventions. See 
+000012f0: 5b6d 6f72 650d 0a68 6572 655d 2868 7474  [more..here](htt
+00001300: 7073 3a2f 2f77 7777 2e6e 656f 7465 726f  ps://www.neotero
+00001310: 692e 6465 762f 626c 6163 6b73 6865 6570  i.dev/blacksheep
+00001320: 2f72 6571 7565 7374 732f 292e 0d0a 0d0a  /requests/).....
+00001330: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00001340: 6461 7461 636c 6173 7365 7320 696d 706f  dataclasses impo
+00001350: 7274 2064 6174 6163 6c61 7373 0d0a 0d0a  rt dataclass....
+00001360: 6672 6f6d 2062 6c61 636b 7368 6565 7020  from blacksheep 
+00001370: 696d 706f 7274 2041 7070 6c69 6361 7469  import Applicati
+00001380: 6f6e 2c20 4672 6f6d 4a53 4f4e 2c20 4672  on, FromJSON, Fr
+00001390: 6f6d 5175 6572 790d 0a0d 0a0d 0a61 7070  omQuery......app
+000013a0: 203d 2041 7070 6c69 6361 7469 6f6e 2829   = Application()
+000013b0: 0d0a 0d0a 0d0a 4064 6174 6163 6c61 7373  ......@dataclass
+000013c0: 0d0a 636c 6173 7320 4372 6561 7465 4361  ..class CreateCa
+000013d0: 7449 6e70 7574 3a0d 0a20 2020 206e 616d  tInput:..    nam
+000013e0: 653a 2073 7472 0d0a 0d0a 0d0a 4061 7070  e: str......@app
+000013f0: 2e72 6f75 7465 722e 706f 7374 2822 2f61  .router.post("/a
+00001400: 7069 2f63 6174 7322 290d 0a61 7379 6e63  pi/cats")..async
+00001410: 2064 6566 2065 7861 6d70 6c65 2864 6174   def example(dat
+00001420: 613a 2046 726f 6d4a 534f 4e5b 4372 6561  a: FromJSON[Crea
+00001430: 7465 4361 7449 6e70 7574 5d29 3a0d 0a20  teCatInput]):.. 
+00001440: 2020 2023 2069 6e20 7468 6973 2065 7861     # in this exa
+00001450: 6d70 6c65 2c20 6461 7461 2069 7320 626f  mple, data is bo
+00001460: 756e 6420 6175 746f 6d61 7469 6361 6c6c  und automaticall
+00001470: 7920 7265 6164 696e 6720 7468 6520 4a53  y reading the JS
+00001480: 4f4e 0d0a 2020 2020 2320 7061 796c 6f61  ON..    # payloa
+00001490: 6420 616e 6420 6372 6561 7469 6e67 2061  d and creating a
+000014a0: 6e20 696e 7374 616e 6365 206f 6620 6043  n instance of `C
+000014b0: 7265 6174 6543 6174 496e 7075 7460 0d0a  reateCatInput`..
+000014c0: 2020 2020 2e2e 2e0d 0a0d 0a0d 0a40 6170      .........@ap
+000014d0: 702e 726f 7574 6572 2e67 6574 2822 2f3a  p.router.get("/:
+000014e0: 6375 6c74 7572 655f 636f 6465 2f3a 6172  culture_code/:ar
+000014f0: 6561 2229 0d0a 6173 796e 6320 6465 6620  ea")..async def 
+00001500: 686f 6d65 2863 756c 7475 7265 5f63 6f64  home(culture_cod
+00001510: 652c 2061 7265 6129 3a0d 0a20 2020 2023  e, area):..    #
+00001520: 2069 6e20 7468 6973 2065 7861 6d70 6c65   in this example
+00001530: 2c20 626f 7468 2070 6172 616d 6574 6572  , both parameter
+00001540: 7320 6172 6520 6f62 7461 696e 6564 2066  s are obtained f
+00001550: 726f 6d20 726f 7574 6573 2077 6974 680d  rom routes with.
+00001560: 0a20 2020 2023 206d 6174 6368 696e 6720  .    # matching 
+00001570: 6e61 6d65 730d 0a20 2020 2072 6574 7572  names..    retur
+00001580: 6e20 6622 5265 7175 6573 7420 666f 723a  n f"Request for:
+00001590: 207b 6375 6c74 7572 655f 636f 6465 7d20   {culture_code} 
+000015a0: 7b61 7265 617d 220d 0a0d 0a0d 0a40 6170  {area}"......@ap
+000015b0: 702e 726f 7574 6572 2e67 6574 2822 2f61  p.router.get("/a
+000015c0: 7069 2f70 726f 6475 6374 7322 290d 0a64  pi/products")..d
+000015d0: 6566 2067 6574 5f70 726f 6475 6374 7328  ef get_products(
+000015e0: 0d0a 2020 2020 7061 6765 3a20 696e 7420  ..    page: int 
+000015f0: 3d20 312c 0d0a 2020 2020 7369 7a65 3a20  = 1,..    size: 
+00001600: 696e 7420 3d20 3330 2c0d 0a20 2020 2073  int = 30,..    s
+00001610: 6561 7263 683a 2073 7472 203d 2022 222c  earch: str = "",
+00001620: 0d0a 293a 0d0a 2020 2020 2320 7468 6973  ..):..    # this
+00001630: 2065 7861 6d70 6c65 2069 6c6c 7573 7472   example illustr
+00001640: 6174 6573 2073 7570 706f 7274 2066 6f72  ates support for
+00001650: 2069 6d70 6c69 6369 7420 7175 6572 7920   implicit query 
+00001660: 7061 7261 6d65 7465 7273 2077 6974 680d  parameters with.
+00001670: 0a20 2020 2023 2064 6566 6175 6c74 2076  .    # default v
+00001680: 616c 7565 730d 0a20 2020 2023 2073 696e  alues..    # sin
+00001690: 6365 2074 6865 2073 6f75 7263 6520 6f66  ce the source of
+000016a0: 2070 6167 652c 2073 697a 652c 2061 6e64   page, size, and
+000016b0: 2073 6561 7263 6820 6973 206e 6f74 2073   search is not s
+000016c0: 7065 6369 6669 6564 2061 6e64 206e 6f0d  pecified and no.
+000016d0: 0a20 2020 2023 2072 6f75 7465 2070 6172  .    # route par
+000016e0: 616d 6574 6572 206d 6174 6368 6573 2074  ameter matches t
+000016f0: 6865 6972 206e 616d 652c 2074 6865 7920  heir name, they 
+00001700: 6172 6520 6f62 7461 696e 6564 2066 726f  are obtained fro
+00001710: 6d20 7175 6572 7920 7374 7269 6e67 0d0a  m query string..
+00001720: 2020 2020 2e2e 2e0d 0a0d 0a0d 0a40 6170      .........@ap
+00001730: 702e 726f 7574 6572 2e67 6574 2822 2f61  p.router.get("/a
+00001740: 7069 2f70 726f 6475 6374 7332 2229 0d0a  pi/products2")..
+00001750: 6465 6620 6765 745f 7072 6f64 7563 7473  def get_products
+00001760: 3228 0d0a 2020 2020 7061 6765 3a20 4672  2(..    page: Fr
+00001770: 6f6d 5175 6572 795b 696e 745d 203d 2046  omQuery[int] = F
+00001780: 726f 6d51 7565 7279 2831 292c 0d0a 2020  romQuery(1),..  
+00001790: 2020 7369 7a65 3a20 4672 6f6d 5175 6572    size: FromQuer
+000017a0: 795b 696e 745d 203d 2046 726f 6d51 7565  y[int] = FromQue
+000017b0: 7279 2833 3029 2c0d 0a20 2020 2073 6561  ry(30),..    sea
+000017c0: 7263 683a 2046 726f 6d51 7565 7279 5b73  rch: FromQuery[s
+000017d0: 7472 5d20 3d20 4672 6f6d 5175 6572 7928  tr] = FromQuery(
+000017e0: 2222 292c 0d0a 293a 0d0a 2020 2020 2320  ""),..):..    # 
+000017f0: 7468 6973 2065 7861 6d70 6c65 2069 6c6c  this example ill
+00001800: 7573 7472 6174 6573 2073 7570 706f 7274  ustrates support
+00001810: 2066 6f72 2065 7870 6c69 6369 7420 7175   for explicit qu
+00001820: 6572 7920 7061 7261 6d65 7465 7273 2077  ery parameters w
+00001830: 6974 680d 0a20 2020 2023 2064 6566 6175  ith..    # defau
+00001840: 6c74 2076 616c 7565 730d 0a20 2020 2023  lt values..    #
+00001850: 2069 6e20 7468 6973 2063 6173 652c 2070   in this case, p
+00001860: 6172 616d 6574 6572 7320 6172 6520 6578  arameters are ex
+00001870: 706c 6963 6974 6c79 2072 6561 6420 6672  plicitly read fr
+00001880: 6f6d 2071 7565 7279 2073 7472 696e 670d  om query string.
+00001890: 0a20 2020 202e 2e2e 0d0a 0d0a 6060 600d  .    .......```.
+000018a0: 0a0d 0a49 7420 616c 736f 2073 7570 706f  ...It also suppo
+000018b0: 7274 7320 5b64 6570 656e 6465 6e63 790d  rts [dependency.
+000018c0: 0a69 6e6a 6563 7469 6f6e 5d28 6874 7470  .injection](http
+000018d0: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
+000018e0: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
+000018f0: 6465 7065 6e64 656e 6379 2d69 6e6a 6563  dependency-injec
+00001900: 7469 6f6e 2f29 2c20 610d 0a66 6561 7475  tion/), a..featu
+00001910: 7265 2074 6861 7420 7072 6f76 6964 6573  re that provides
+00001920: 2061 2063 6f6e 7369 7374 656e 7420 616e   a consistent an
+00001930: 6420 636c 6561 6e20 7761 7920 746f 2075  d clean way to u
+00001940: 7365 2064 6570 656e 6465 6e63 6965 7320  se dependencies 
+00001950: 696e 2072 6571 7565 7374 0d0a 6861 6e64  in request..hand
+00001960: 6c65 7273 2e0d 0a0d 0a23 2320 4765 6e65  lers.....## Gene
+00001970: 7261 7469 6f6e 206f 6620 4f70 656e 4150  ration of OpenAP
+00001980: 4920 446f 6375 6d65 6e74 6174 696f 6e0d  I Documentation.
+00001990: 0a5b 4765 6e65 7261 7469 6f6e 206f 6620  .[Generation of 
+000019a0: 4f70 656e 4150 4920 446f 6375 6d65 6e74  OpenAPI Document
+000019b0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f77  ation](https://w
+000019c0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+000019d0: 626c 6163 6b73 6865 6570 2f6f 7065 6e61  blacksheep/opena
+000019e0: 7069 2f29 2e0d 0a0d 0a23 2320 5374 7261  pi/).....## Stra
+000019f0: 7465 6769 6573 2074 6f20 6861 6e64 6c65  tegies to handle
+00001a00: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
+00001a10: 616e 6420 6175 7468 6f72 697a 6174 696f  and authorizatio
+00001a20: 6e0d 0a42 6c61 636b 5368 6565 7020 696d  n..BlackSheep im
+00001a30: 706c 656d 656e 7473 2073 7472 6174 6567  plements strateg
+00001a40: 6965 7320 746f 2068 616e 646c 6520 6175  ies to handle au
+00001a50: 7468 656e 7469 6361 7469 6f6e 2061 6e64  thentication and
+00001a60: 2061 7574 686f 7269 7a61 7469 6f6e 2e0d   authorization..
+00001a70: 0a54 6865 7365 2066 6561 7475 7265 7320  .These features 
+00001a80: 6172 6520 646f 6375 6d65 6e74 6564 2068  are documented h
+00001a90: 6572 653a 0d0a 0d0a 2a20 5b41 7574 6865  ere:....* [Authe
+00001aa0: 6e74 6963 6174 696f 6e5d 2868 7474 7073  ntication](https
+00001ab0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
+00001ac0: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
+00001ad0: 7574 6865 6e74 6963 6174 696f 6e2f 290d  uthentication/).
+00001ae0: 0a2a 205b 4175 7468 6f72 697a 6174 696f  .* [Authorizatio
+00001af0: 6e5d 2868 7474 7073 3a2f 2f77 7777 2e6e  n](https://www.n
+00001b00: 656f 7465 726f 692e 6465 762f 626c 6163  eoteroi.dev/blac
+00001b10: 6b73 6865 6570 2f61 7574 686f 7269 7a61  ksheep/authoriza
+00001b20: 7469 6f6e 2f29 0d0a 0d0a 6060 6070 7974  tion/)....```pyt
+00001b30: 686f 6e0d 0a61 7070 2e75 7365 5f61 7574  hon..app.use_aut
+00001b40: 6865 6e74 6963 6174 696f 6e28 295c 0d0a  hentication()\..
+00001b50: 2020 2020 2e61 6464 2845 7861 6d70 6c65      .add(Example
+00001b60: 4175 7468 656e 7469 6361 7469 6f6e 4861  AuthenticationHa
+00001b70: 6e64 6c65 7228 2929 0d0a 0d0a 0d0a 6170  ndler())......ap
+00001b80: 702e 7573 655f 6175 7468 6f72 697a 6174  p.use_authorizat
+00001b90: 696f 6e28 295c 0d0a 2020 2020 2e61 6464  ion()\..    .add
+00001ba0: 2841 646d 696e 7350 6f6c 6963 7928 2929  (AdminsPolicy())
+00001bb0: 0d0a 0d0a 0d0a 4061 7574 6828 2261 646d  ......@auth("adm
+00001bc0: 696e 2229 0d0a 4061 7070 2e72 6f75 7465  in")..@app.route
+00001bd0: 722e 6765 7428 222f 2229 0d0a 6173 796e  r.get("/")..asyn
+00001be0: 6320 6465 6620 6f6e 6c79 5f66 6f72 5f61  c def only_for_a
+00001bf0: 646d 696e 7328 293a 0d0a 2020 2020 2e2e  dmins():..    ..
+00001c00: 2e0d 0a0d 0a0d 0a40 6175 7468 2829 0d0a  .......@auth()..
+00001c10: 4061 7070 2e72 6f75 7465 722e 6765 7428  @app.router.get(
+00001c20: 222f 2229 0d0a 6173 796e 6320 6465 6620  "/")..async def 
+00001c30: 6f6e 6c79 5f66 6f72 5f61 7574 6865 6e74  only_for_authent
+00001c40: 6963 6174 6564 5f75 7365 7273 2829 3a0d  icated_users():.
+00001c50: 0a20 2020 202e 2e2e 0d0a 6060 600d 0a0d  .    .....```...
+00001c60: 0a53 696e 6365 2076 6572 7369 6f6e 2060  .Since version `
+00001c70: 312e 322e 3160 2c20 426c 6163 6b53 6865  1.2.1`, BlackShe
+00001c80: 6570 2069 6d70 6c65 6d65 6e74 733a 0d0a  ep implements:..
+00001c90: 0d0a 2a20 5b42 7569 6c74 2d69 6e20 7375  ..* [Built-in su
+00001ca0: 7070 6f72 7420 666f 7220 4f70 656e 4944  pport for OpenID
+00001cb0: 2043 6f6e 6e65 6374 2061 7574 6865 6e74   Connect authent
+00001cc0: 6963 6174 696f 6e5d 2868 7474 7073 3a2f  ication](https:/
+00001cd0: 2f77 7777 2e6e 656f 7465 726f 692e 6465  /www.neoteroi.de
+00001ce0: 762f 626c 6163 6b73 6865 6570 2f61 7574  v/blacksheep/aut
+00001cf0: 6865 6e74 6963 6174 696f 6e2f 236f 6964  hentication/#oid
+00001d00: 6329 0d0a 2a20 5b42 7569 6c74 2d69 6e20  c)..* [Built-in 
+00001d10: 7375 7070 6f72 7420 666f 7220 4a57 5420  support for JWT 
+00001d20: 4265 6172 6572 2061 7574 6865 6e74 6963  Bearer authentic
+00001d30: 6174 696f 6e5d 2868 7474 7073 3a2f 2f77  ation](https://w
+00001d40: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+00001d50: 626c 6163 6b73 6865 6570 2f61 7574 6865  blacksheep/authe
+00001d60: 6e74 6963 6174 696f 6e2f 236a 7774 2d62  ntication/#jwt-b
+00001d70: 6561 7265 7229 0d0a 0d0a 4d65 616e 696e  earer)....Meanin
+00001d80: 6720 7468 6174 2069 7420 6973 2065 6173  g that it is eas
+00001d90: 7920 746f 2069 6e74 6567 7261 7465 2077  y to integrate w
+00001da0: 6974 6820 7365 7276 6963 6573 2073 7563  ith services suc
+00001db0: 6820 6173 3a0d 0a2a 205b 4175 7468 305d  h as:..* [Auth0]
+00001dc0: 2868 7474 7073 3a2f 2f61 7574 6830 2e63  (https://auth0.c
+00001dd0: 6f6d 290d 0a2a 205b 417a 7572 6520 4163  om)..* [Azure Ac
+00001de0: 7469 7665 2044 6972 6563 746f 7279 5d28  tive Directory](
+00001df0: 6874 7470 733a 2f2f 617a 7572 652e 6d69  https://azure.mi
+00001e00: 6372 6f73 6f66 742e 636f 6d2f 656e 2d75  crosoft.com/en-u
+00001e10: 732f 7365 7276 6963 6573 2f61 6374 6976  s/services/activ
+00001e20: 652d 6469 7265 6374 6f72 792f 290d 0a2a  e-directory/)..*
+00001e30: 205b 417a 7572 6520 4163 7469 7665 2044   [Azure Active D
+00001e40: 6972 6563 746f 7279 2042 3243 5d28 6874  irectory B2C](ht
+00001e50: 7470 733a 2f2f 646f 6373 2e6d 6963 726f  tps://docs.micro
+00001e60: 736f 6674 2e63 6f6d 2f65 6e2d 7573 2f61  soft.com/en-us/a
+00001e70: 7a75 7265 2f61 6374 6976 652d 6469 7265  zure/active-dire
+00001e80: 6374 6f72 792d 6232 632f 6f76 6572 7669  ctory-b2c/overvi
+00001e90: 6577 290d 0a2a 205b 4f6b 7461 5d28 6874  ew)..* [Okta](ht
+00001ea0: 7470 733a 2f2f 7777 772e 6f6b 7461 2e63  tps://www.okta.c
+00001eb0: 6f6d 290d 0a0d 0a52 6566 6572 2074 6f20  om)....Refer to 
+00001ec0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00001ed0: 6e20 666f 7220 6d6f 7265 2064 6574 6169  n for more detai
+00001ee0: 6c73 2061 6e64 2065 7861 6d70 6c65 732e  ls and examples.
+00001ef0: 0d0a 0d0a 2323 2057 6562 2066 7261 6d65  ....## Web frame
+00001f00: 776f 726b 2066 6561 7475 7265 730d 0a0d  work features...
+00001f10: 0a2a 205b 4153 4749 2063 6f6d 7061 7469  .* [ASGI compati
+00001f20: 6269 6c69 7479 5d28 6874 7470 733a 2f2f  bility](https://
+00001f30: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
+00001f40: 2f62 6c61 636b 7368 6565 702f 6173 6769  /blacksheep/asgi
+00001f50: 2f29 0d0a 2a20 5b52 6f75 7469 6e67 5d28  /)..* [Routing](
+00001f60: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
+00001f70: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
+00001f80: 6565 702f 726f 7574 696e 672f 290d 0a2a  eep/routing/)..*
+00001f90: 2052 6571 7565 7374 2068 616e 646c 6572   Request handler
+00001fa0: 7320 6361 6e20 6265 205b 6465 6669 6e65  s can be [define
+00001fb0: 6420 6173 0d0a 2020 6675 6e63 7469 6f6e  d as..  function
+00001fc0: 735d 2868 7474 7073 3a2f 2f77 7777 2e6e  s](https://www.n
+00001fd0: 656f 7465 726f 692e 6465 762f 626c 6163  eoteroi.dev/blac
+00001fe0: 6b73 6865 6570 2f72 6571 7565 7374 2d68  ksheep/request-h
+00001ff0: 616e 646c 6572 732f 292c 206f 7220 5b63  andlers/), or [c
+00002000: 6c61 7373 0d0a 2020 6d65 7468 6f64 735d  lass..  methods]
+00002010: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00002020: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+00002030: 6865 6570 2f63 6f6e 7472 6f6c 6c65 7273  heep/controllers
+00002040: 2f29 0d0a 2a20 5b4d 6964 646c 6577 6172  /)..* [Middlewar
+00002050: 6573 5d28 6874 7470 733a 2f2f 7777 772e  es](https://www.
+00002060: 6e65 6f74 6572 6f69 2e64 6576 2f62 6c61  neoteroi.dev/bla
+00002070: 636b 7368 6565 702f 6d69 6464 6c65 7761  cksheep/middlewa
+00002080: 7265 732f 290d 0a2a 205b 5765 6253 6f63  res/)..* [WebSoc
+00002090: 6b65 745d 2868 7474 7073 3a2f 2f77 7777  ket](https://www
+000020a0: 2e6e 656f 7465 726f 692e 6465 762f 626c  .neoteroi.dev/bl
+000020b0: 6163 6b73 6865 6570 2f77 6562 736f 636b  acksheep/websock
+000020c0: 6574 2f29 0d0a 2a20 5b42 7569 6c74 2d69  et/)..* [Built-i
+000020d0: 6e20 7375 7070 6f72 7420 666f 7220 6465  n support for de
+000020e0: 7065 6e64 656e 6379 0d0a 2020 696e 6a65  pendency..  inje
+000020f0: 6374 696f 6e5d 2868 7474 7073 3a2f 2f77  ction](https://w
+00002100: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+00002110: 626c 6163 6b73 6865 6570 2f64 6570 656e  blacksheep/depen
+00002120: 6465 6e63 792d 696e 6a65 6374 696f 6e2f  dency-injection/
+00002130: 290d 0a2a 205b 5375 7070 6f72 7420 666f  )..* [Support fo
+00002140: 7220 6175 746f 6d61 7469 6320 6269 6e64  r automatic bind
+00002150: 696e 6720 6f66 2072 6f75 7465 2061 6e64  ing of route and
+00002160: 2071 7565 7279 2070 6172 616d 6574 6572   query parameter
+00002170: 7320 746f 2072 6571 7565 7374 0d0a 2020  s to request..  
+00002180: 6861 6e64 6c65 7273 206d 6574 686f 6473  handlers methods
+00002190: 0d0a 2020 6361 6c6c 735d 2868 7474 7073  ..  calls](https
+000021a0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
+000021b0: 6465 762f 626c 6163 6b73 6865 6570 2f67  dev/blacksheep/g
+000021c0: 6574 7469 6e67 2d73 7461 7274 6564 2f23  etting-started/#
+000021d0: 6861 6e64 6c69 6e67 2d72 6f75 7465 2d70  handling-route-p
+000021e0: 6172 616d 6574 6572 7329 0d0a 2a20 5b53  arameters)..* [S
+000021f0: 7472 6174 6567 7920 746f 2068 616e 646c  trategy to handl
+00002200: 650d 0a20 2065 7863 6570 7469 6f6e 735d  e..  exceptions]
+00002210: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00002220: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+00002230: 6865 6570 2f61 7070 6c69 6361 7469 6f6e  heep/application
+00002240: 2f23 636f 6e66 6967 7572 696e 672d 6578  /#configuring-ex
+00002250: 6365 7074 696f 6e73 2d68 616e 646c 6572  ceptions-handler
+00002260: 7329 0d0a 2a20 5b53 7472 6174 6567 7920  s)..* [Strategy 
+00002270: 746f 2068 616e 646c 6520 6175 7468 656e  to handle authen
+00002280: 7469 6361 7469 6f6e 2061 6e64 0d0a 2020  tication and..  
+00002290: 6175 7468 6f72 697a 6174 696f 6e5d 2868  authorization](h
+000022a0: 7474 7073 3a2f 2f77 7777 2e6e 656f 7465  ttps://www.neote
+000022b0: 726f 692e 6465 762f 626c 6163 6b73 6865  roi.dev/blackshe
+000022c0: 6570 2f61 7574 6865 6e74 6963 6174 696f  ep/authenticatio
+000022d0: 6e2f 290d 0a2a 205b 4275 696c 742d 696e  n/)..* [Built-in
+000022e0: 2073 7570 706f 7274 2066 6f72 204f 7065   support for Ope
+000022f0: 6e49 4420 436f 6e6e 6563 7420 6175 7468  nID Connect auth
+00002300: 656e 7469 6361 7469 6f6e 2075 7369 6e67  entication using
+00002310: 204f 4944 430d 0a20 2064 6973 636f 7665   OIDC..  discove
+00002320: 7279 5d28 6874 7470 733a 2f2f 7777 772e  ry](https://www.
+00002330: 6e65 6f74 6572 6f69 2e64 6576 2f62 6c61  neoteroi.dev/bla
+00002340: 636b 7368 6565 702f 6175 7468 656e 7469  cksheep/authenti
+00002350: 6361 7469 6f6e 2f23 6f69 6463 290d 0a2a  cation/#oidc)..*
+00002360: 205b 4275 696c 742d 696e 2073 7570 706f   [Built-in suppo
+00002370: 7274 2066 6f72 204a 5754 2042 6561 7265  rt for JWT Beare
+00002380: 7220 6175 7468 656e 7469 6361 7469 6f6e  r authentication
+00002390: 2075 7369 6e67 204f 4944 4320 6469 7363   using OIDC disc
+000023a0: 6f76 6572 7920 616e 640d 0a20 206f 7468  overy and..  oth
+000023b0: 6572 2073 6f75 7263 6573 206f 660d 0a20  er sources of.. 
+000023c0: 204a 574b 535d 2868 7474 7073 3a2f 2f77   JWKS](https://w
+000023d0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+000023e0: 626c 6163 6b73 6865 6570 2f61 7574 6865  blacksheep/authe
+000023f0: 6e74 6963 6174 696f 6e2f 236a 7774 2d62  ntication/#jwt-b
+00002400: 6561 7265 7229 0d0a 2a20 5b48 616e 646c  earer)..* [Handl
+00002410: 6572 730d 0a20 206e 6f72 6d61 6c69 7a61  ers..  normaliza
+00002420: 7469 6f6e 5d28 6874 7470 733a 2f2f 7777  tion](https://ww
+00002430: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
+00002440: 6c61 636b 7368 6565 702f 7265 7175 6573  lacksheep/reques
+00002450: 742d 6861 6e64 6c65 7273 2f29 0d0a 2a20  t-handlers/)..* 
+00002460: 5b53 6572 7669 6e67 2073 7461 7469 630d  [Serving static.
+00002470: 0a20 2066 696c 6573 5d28 6874 7470 733a  .  files](https:
+00002480: 2f2f 7777 772e 6e65 6f74 6572 6f69 2e64  //www.neoteroi.d
+00002490: 6576 2f62 6c61 636b 7368 6565 702f 7374  ev/blacksheep/st
+000024a0: 6174 6963 2d66 696c 6573 2f29 0d0a 2a20  atic-files/)..* 
+000024b0: 5b49 6e74 6567 7261 7469 6f6e 2077 6974  [Integration wit
+000024c0: 680d 0a20 204a 696e 6a61 325d 2868 7474  h..  Jinja2](htt
+000024d0: 7073 3a2f 2f77 7777 2e6e 656f 7465 726f  ps://www.neotero
+000024e0: 692e 6465 762f 626c 6163 6b73 6865 6570  i.dev/blacksheep
+000024f0: 2f74 656d 706c 6174 696e 672f 290d 0a2a  /templating/)..*
+00002500: 205b 5375 7070 6f72 7420 666f 7220 7365   [Support for se
+00002510: 7276 696e 6720 5350 4173 2074 6861 7420  rving SPAs that 
+00002520: 7573 6520 4854 4d4c 3520 4869 7374 6f72  use HTML5 Histor
+00002530: 7920 4150 4920 666f 7220 636c 6965 6e74  y API for client
+00002540: 2073 6964 650d 0a20 2072 6f75 7469 6e67   side..  routing
+00002550: 5d28 6874 7470 733a 2f2f 7777 772e 6e65  ](https://www.ne
+00002560: 6f74 6572 6f69 2e64 6576 2f62 6c61 636b  oteroi.dev/black
+00002570: 7368 6565 702f 7374 6174 6963 2d66 696c  sheep/static-fil
+00002580: 6573 2f23 686f 772d 746f 2d73 6572 7665  es/#how-to-serve
+00002590: 2d73 7061 732d 7468 6174 2d75 7365 2d68  -spas-that-use-h
+000025a0: 746d 6c35 2d68 6973 746f 7279 2d61 7069  tml5-history-api
+000025b0: 290d 0a2a 205b 5375 7070 6f72 7420 666f  )..* [Support fo
+000025c0: 7220 6175 746f 6d61 7469 6320 6765 6e65  r automatic gene
+000025d0: 7261 7469 6f6e 206f 6620 4f70 656e 4150  ration of OpenAP
+000025e0: 490d 0a20 2044 6f63 756d 656e 7461 7469  I..  Documentati
+000025f0: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
+00002600: 6e65 6f74 6572 6f69 2e64 6576 2f62 6c61  neoteroi.dev/bla
+00002610: 636b 7368 6565 702f 6f70 656e 6170 692f  cksheep/openapi/
+00002620: 290d 0a2a 205b 5374 7261 7465 6779 2074  )..* [Strategy t
+00002630: 6f20 6861 6e64 6c65 2043 4f52 5320 7365  o handle CORS se
+00002640: 7474 696e 6773 5d28 6874 7470 733a 2f2f  ttings](https://
+00002650: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
+00002660: 2f62 6c61 636b 7368 6565 702f 636f 7273  /blacksheep/cors
+00002670: 2f29 0d0a 2a20 5b53 6573 7369 6f6e 735d  /)..* [Sessions]
+00002680: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00002690: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+000026a0: 6865 6570 2f73 6573 7369 6f6e 732f 290d  heep/sessions/).
+000026b0: 0a2a 2053 7570 706f 7274 2066 6f72 2061  .* Support for a
+000026c0: 7574 6f6d 6174 6963 2062 696e 6469 6e67  utomatic binding
+000026d0: 206f 6620 6064 6174 6163 6c61 7373 6573   of `dataclasses
+000026e0: 6020 616e 640d 0a20 205b 6070 7964 616e  ` and..  [`pydan
+000026f0: 7469 6360 5d28 6874 7470 733a 2f2f 7079  tic`](https://py
+00002700: 6461 6e74 6963 2d64 6f63 732e 6865 6c70  dantic-docs.help
+00002710: 6d61 6e75 616c 2e69 6f29 206d 6f64 656c  manual.io) model
+00002720: 7320 746f 2068 616e 646c 6520 7468 650d  s to handle the.
+00002730: 0a20 2072 6571 7565 7374 2062 6f64 7920  .  request body 
+00002740: 7061 796c 6f61 6420 6578 7065 6374 6564  payload expected
+00002750: 2062 7920 7265 7175 6573 7420 6861 6e64   by request hand
+00002760: 6c65 7273 0d0a 2a20 5b60 5465 7374 436c  lers..* [`TestCl
+00002770: 6965 6e74 6020 636c 6173 7320 746f 2073  ient` class to s
+00002780: 696d 706c 6966 7920 7465 7374 696e 6720  implify testing 
+00002790: 6f66 2061 7070 6c69 6361 7469 6f6e 735d  of applications]
+000027a0: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+000027b0: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+000027c0: 6865 6570 2f74 6573 7469 6e67 2f29 0d0a  heep/testing/)..
+000027d0: 2a20 5b41 6e74 6920 466f 7267 6572 7920  * [Anti Forgery 
+000027e0: 7661 6c69 6461 7469 6f6e 5d28 6874 7470  validation](http
+000027f0: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
+00002800: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
+00002810: 616e 7469 2d72 6571 7565 7374 2d66 6f72  anti-request-for
+00002820: 6765 7279 2920 746f 2070 726f 7465 6374  gery) to protect
+00002830: 2061 6761 696e 7374 2043 726f 7373 2d53   against Cross-S
+00002840: 6974 6520 5265 7175 6573 7420 466f 7267  ite Request Forg
+00002850: 6572 7920 2858 5352 462f 4353 5246 2920  ery (XSRF/CSRF) 
+00002860: 6174 7461 636b 730d 0a0d 0a23 2320 436c  attacks....## Cl
+00002870: 6965 6e74 2066 6561 7475 7265 730d 0a0d  ient features...
+00002880: 0a42 6c61 636b 5368 6565 7020 696e 636c  .BlackSheep incl
+00002890: 7564 6573 2061 6e20 4854 5450 2043 6c69  udes an HTTP Cli
+000028a0: 656e 742e 0d0a 0d0a 2a2a 4578 616d 706c  ent.....**Exampl
+000028b0: 653a 2a2a 0d0a 6060 6070 7974 686f 6e0d  e:**..```python.
+000028c0: 0a69 6d70 6f72 7420 6173 796e 6369 6f0d  .import asyncio.
+000028d0: 0a0d 0a66 726f 6d20 626c 6163 6b73 6865  ...from blackshe
+000028e0: 6570 2e63 6c69 656e 7420 696d 706f 7274  ep.client import
+000028f0: 2043 6c69 656e 7453 6573 7369 6f6e 0d0a   ClientSession..
+00002900: 0d0a 0d0a 6173 796e 6320 6465 6620 636c  ....async def cl
+00002910: 6965 6e74 5f65 7861 6d70 6c65 2829 3a0d  ient_example():.
+00002920: 0a20 2020 2061 7379 6e63 2077 6974 6820  .    async with 
+00002930: 436c 6965 6e74 5365 7373 696f 6e28 2920  ClientSession() 
+00002940: 6173 2063 6c69 656e 743a 0d0a 2020 2020  as client:..    
+00002950: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+00002960: 7761 6974 2063 6c69 656e 742e 6765 7428  wait client.get(
+00002970: 2268 7474 7073 3a2f 2f64 6f63 732e 7079  "https://docs.py
+00002980: 7468 6f6e 2e6f 7267 2f33 2f22 290d 0a0d  thon.org/3/")...
+00002990: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000029a0: 7265 7370 6f6e 7365 2069 7320 6e6f 7420  response is not 
+000029b0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7465  None..        te
+000029c0: 7874 203d 2061 7761 6974 2072 6573 706f  xt = await respo
+000029d0: 6e73 652e 7465 7874 2829 0d0a 2020 2020  nse.text()..    
+000029e0: 2020 2020 7072 696e 7428 7465 7874 290d      print(text).
+000029f0: 0a0d 0a0d 0a61 7379 6e63 696f 2e72 756e  .....asyncio.run
+00002a00: 2863 6c69 656e 745f 6578 616d 706c 6528  (client_example(
+00002a10: 2929 0d0a 6060 600d 0a0d 0a23 2320 5375  ))..```....## Su
+00002a20: 7070 6f72 7465 6420 706c 6174 666f 726d  pported platform
+00002a30: 7320 616e 6420 7275 6e74 696d 6573 0d0a  s and runtimes..
+00002a40: 2a20 5079 7468 6f6e 3a20 616c 6c20 7665  * Python: all ve
+00002a50: 7273 696f 6e73 2069 6e63 6c75 6465 6420  rsions included 
+00002a60: 696e 2074 6865 2062 7569 6c64 206d 6174  in the build mat
+00002a70: 7269 780d 0a2a 2055 6275 6e74 750d 0a2a  rix..* Ubuntu..*
+00002a80: 2057 696e 646f 7773 2031 300d 0a2a 206d   Windows 10..* m
+00002a90: 6163 4f53 0d0a 0d0a 2323 2044 6f63 756d  acOS....## Docum
+00002aa0: 656e 7461 7469 6f6e 0d0a 506c 6561 7365  entation..Please
+00002ab0: 2072 6566 6572 2074 6f20 7468 6520 5b64   refer to the [d
+00002ac0: 6f63 756d 656e 7461 7469 6f6e 2077 6562  ocumentation web
+00002ad0: 7369 7465 5d28 6874 7470 733a 2f2f 7777  site](https://ww
+00002ae0: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
+00002af0: 6c61 636b 7368 6565 702f 292e 0d0a 0d0a  lacksheep/).....
+00002b00: 2323 2043 6f6d 6d75 6e69 6361 7469 6f6e  ## Communication
+00002b10: 0d0a 5b42 6c61 636b 5368 6565 7020 636f  ..[BlackSheep co
+00002b20: 6d6d 756e 6974 7920 696e 2047 6974 7465  mmunity in Gitte
+00002b30: 725d 2868 7474 7073 3a2f 2f67 6974 7465  r](https://gitte
+00002b40: 722e 696d 2f4e 656f 7465 726f 692f 426c  r.im/Neoteroi/Bl
+00002b50: 6163 6b53 6865 6570 292e 0d0a 0d0a 2323  ackSheep).....##
+00002b60: 2042 7261 6e63 6865 730d 0a54 6865 205f   Branches..The _
+00002b70: 6d61 696e 5f20 6272 616e 6368 2063 6f6e  main_ branch con
+00002b80: 7461 696e 7320 7468 6520 6375 7272 656e  tains the curren
+00002b90: 746c 7920 6465 7665 6c6f 7065 6420 7665  tly developed ve
+00002ba0: 7273 696f 6e2c 2077 6869 6368 2069 7320  rsion, which is 
+00002bb0: 7665 7273 696f 6e20 320d 0a61 6c70 6861  version 2..alpha
+00002bc0: 2e20 5468 6520 5f76 315f 2062 7261 6e63  . The _v1_ branc
+00002bd0: 6820 636f 6e74 6169 6e73 2076 6572 7369  h contains versi
+00002be0: 6f6e 2031 206f 6620 7468 6520 7765 6220  on 1 of the web 
+00002bf0: 6672 616d 6577 6f72 6b2c 2066 6f72 2062  framework, for b
+00002c00: 7567 7320 6669 7865 730d 0a61 6e64 206d  ugs fixes..and m
+00002c10: 6169 6e74 656e 616e 6365 2e0d 0a         aintenance...
```

### Comparing `blacksheep-2.0a8/README.md` & `blacksheep-2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/__init__.py` & `blacksheep-2.0a9/blacksheep/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Root module of the framework. This module re-exports the most commonly
 used types to reduce the verbosity of the imports statements.
 """
 __author__ = "Roberto Prevato <roberto.prevato@gmail.com>"
-__version__ = "2.0a8"
+__version__ = "2.0a9"
 
 from .contents import Content as Content
 from .contents import FormContent as FormContent
 from .contents import FormPart as FormPart
 from .contents import HTMLContent as HTMLContent
 from .contents import JSONContent as JSONContent
 from .contents import MultiPartFormData as MultiPartFormData
```

### Comparing `blacksheep-2.0a8/blacksheep/baseapp.c` & `blacksheep-2.0a9/blacksheep/baseapp.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -953,24 +955,24 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/baseapp.pyx",
-  "blacksheep/baseapp.pxd",
+  "blacksheep\\baseapp.pyx",
+  "blacksheep\\baseapp.pxd",
   "stringsource",
   "datetime.pxd",
-  "blacksheep/exceptions.pxd",
-  "blacksheep/contents.pxd",
+  "blacksheep\\exceptions.pxd",
+  "blacksheep\\contents.pxd",
   "type.pxd",
-  "blacksheep/cookies.pxd",
-  "blacksheep/url.pxd",
-  "blacksheep/messages.pxd",
+  "blacksheep\\cookies.pxd",
+  "blacksheep\\url.pxd",
+  "blacksheep\\messages.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_10exceptions_MessageAborted;
 struct __pyx_obj_10blacksheep_10exceptions_HTTPException;
 struct __pyx_obj_10blacksheep_10exceptions_BadRequest;
 struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat;
@@ -1110,15 +1112,15 @@
  *     cdef readonly bytes type
  *     cdef readonly bytes body
  */
 struct __pyx_obj_10blacksheep_8contents_Content {
   PyObject_HEAD
   PyObject *type;
   PyObject *body;
-  int length;
+  PY_LONG_LONG length;
 };
 
 
 /* "contents.pxd":14
  * 
  * 
  * cdef class StreamedContent(Content):             # <<<<<<<<<<<<<<
@@ -2150,30 +2152,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -2231,15 +2233,15 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_f_10blacksheep_7baseapp_15BaseApplication_get_http_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception); /* proto*/
 static PyObject *__pyx_f_10blacksheep_7baseapp_15BaseApplication_get_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_exception); /* proto*/
 
@@ -2398,15 +2400,15 @@
 static const char __pyx_k_handle_bad_request[] = "handle_bad_request";
 static const char __pyx_k_show_error_details[] = "show_error_details";
 static const char __pyx_k_Handled_error_s_s_s[] = "Handled error: \"%s %s\". %s";
 static const char __pyx_k_Internal_Server_Error[] = "Internal Server Error";
 static const char __pyx_k_Internal_server_error[] = "Internal server error.";
 static const char __pyx_k_handle_http_exception[] = "handle_http_exception";
 static const char __pyx_k_BaseApplication_handle[] = "BaseApplication.handle";
-static const char __pyx_k_blacksheep_baseapp_pyx[] = "blacksheep/baseapp.pyx";
+static const char __pyx_k_blacksheep_baseapp_pyx[] = "blacksheep\\baseapp.pyx";
 static const char __pyx_k_Unhandled_exception_s_s[] = "Unhandled exception - \"%s %s\"";
 static const char __pyx_k_apply_exception_handler[] = "_apply_exception_handler";
 static const char __pyx_k_init_exceptions_handlers[] = "init_exceptions_handlers";
 static const char __pyx_k_get_class_instance_hierarchy[] = "get_class_instance_hierarchy";
 static const char __pyx_k_handle_internal_server_error[] = "handle_internal_server_error";
 static const char __pyx_k_pyx_unpickle_BaseApplication[] = "__pyx_unpickle_BaseApplication";
 static const char __pyx_k_server_error_details_handler[] = "server_error_details_handler";
@@ -9925,15 +9927,15 @@
   p->exceptions_handlers = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_7baseapp_BaseApplication(PyObject *o) {
   struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *p = (struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->router);
   Py_CLEAR(p->logger);
   Py_CLEAR(p->exceptions_handlers);
@@ -11937,70 +11939,70 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(4, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(4, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(4, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(4, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(4, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(4, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(4, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(4, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(4, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(4, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(4, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(4, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(4, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(5, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(5, 14, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(5, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(5, 14, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(5, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8contents_ASGIContent = (struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8contents_ASGIContent->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8contents_ASGIContent)) __PYX_ERR(5, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(5, 23, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(5, 27, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(5, 31, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(5, 35, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(5, 39, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(5, 47, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(5, 23, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(5, 27, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(5, 31, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(5, 35, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(5, 39, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(5, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(7, 17, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(7, 17, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7cookies_Cookie = (struct __pyx_vtabstruct_10blacksheep_7cookies_Cookie*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7cookies_Cookie->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7cookies_Cookie)) __PYX_ERR(7, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_3url_URL = (struct __pyx_vtabstruct_10blacksheep_3url_URL*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_3url_URL->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_3url_URL)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.messages"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Message),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(9, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8messages_Message),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(9, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Message = (struct __pyx_vtabstruct_10blacksheep_8messages_Message*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Message->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Message)) __PYX_ERR(9, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Request),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(9, 45, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8messages_Request),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(9, 45, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Request = (struct __pyx_vtabstruct_10blacksheep_8messages_Request*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Request->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Request)) __PYX_ERR(9, 45, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Response),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(9, 58, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8messages_Response),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(9, 58, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Response = (struct __pyx_vtabstruct_10blacksheep_8messages_Response*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Response->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Response)) __PYX_ERR(9, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -12021,21 +12023,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -15423,18 +15425,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -15480,22 +15482,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -16379,17 +16381,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
-#define __PYX_HAVE_RT_ImportFunction_0_29_35
-static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `blacksheep-2.0a8/blacksheep/baseapp.pxd` & `blacksheep-2.0a9/blacksheep/baseapp.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/baseapp.pyi` & `blacksheep-2.0a9/blacksheep/baseapp.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/baseapp.pyx` & `blacksheep-2.0a9/blacksheep/baseapp.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/client/connection.py` & `blacksheep-2.0a9/blacksheep/client/connection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/client/cookies.py` & `blacksheep-2.0a9/blacksheep/client/cookies.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/client/exceptions.py` & `blacksheep-2.0a9/blacksheep/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/client/pool.py` & `blacksheep-2.0a9/blacksheep/client/pool.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/client/session.py` & `blacksheep-2.0a9/blacksheep/client/session.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/common/files/asyncfs.py` & `blacksheep-2.0a9/blacksheep/common/files/asyncfs.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/common/files/info.py` & `blacksheep-2.0a9/blacksheep/common/files/info.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/common/files/pathsutils.py` & `blacksheep-2.0a9/blacksheep/common/files/pathsutils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/common/types.py` & `blacksheep-2.0a9/blacksheep/common/types.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/contents.c` & `blacksheep-2.0a9/blacksheep/contents.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -950,18 +952,18 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/contents.pyx",
-  "blacksheep/contents.pxd",
+  "blacksheep\\contents.pyx",
+  "blacksheep\\contents.pxd",
   "stringsource",
-  "blacksheep/exceptions.pxd",
+  "blacksheep\\exceptions.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_10exceptions_MessageAborted;
 struct __pyx_obj_10blacksheep_10exceptions_HTTPException;
 struct __pyx_obj_10blacksheep_10exceptions_BadRequest;
 struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat;
@@ -1076,15 +1078,15 @@
  *     cdef readonly bytes type
  *     cdef readonly bytes body
  */
 struct __pyx_obj_10blacksheep_8contents_Content {
   PyObject_HEAD
   PyObject *type;
   PyObject *body;
-  int length;
+  PY_LONG_LONG length;
 };
 
 
 /* "blacksheep/contents.pxd":14
  * 
  * 
  * cdef class StreamedContent(Content):             # <<<<<<<<<<<<<<
@@ -1899,30 +1901,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* PatchInspect.proto */
 static PyObject* __Pyx_patch_inspect(PyObject* module);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -1952,25 +1954,28 @@
 
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
@@ -2351,15 +2356,15 @@
 static int __pyx_pf_10blacksheep_8contents_7Content___init__(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self, PyObject *__pyx_v_content_type, PyObject *__pyx_v_data); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_7Content_2read(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_7Content_4type___get__(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_7Content_4body___get__(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_7Content_6length___get__(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_7Content_5__reduce_cython__(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_7Content_7__setstate_cython__(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_10blacksheep_8contents_15StreamedContent___init__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self, PyObject *__pyx_v_content_type, PyObject *__pyx_v_data_provider, int __pyx_v_data_length); /* proto */
+static int __pyx_pf_10blacksheep_8contents_15StreamedContent___init__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self, PyObject *__pyx_v_content_type, PyObject *__pyx_v_data_provider, PY_LONG_LONG __pyx_v_data_length); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_15StreamedContent_2read(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_15StreamedContent_5stream(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_15StreamedContent_8get_parts(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_15StreamedContent_9generator___get__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_15StreamedContent_11__reduce_cython__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8contents_15StreamedContent_13__setstate_cython__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_10blacksheep_8contents_11ASGIContent___init__(struct __pyx_obj_10blacksheep_8contents_ASGIContent *__pyx_v_self, PyObject *__pyx_v_receive); /* proto */
@@ -2724,15 +2729,15 @@
 }
 
 /* "blacksheep/contents.pxd":9
  * 
  * cdef class Content:
  *     cdef readonly bytes type             # <<<<<<<<<<<<<<
  *     cdef readonly bytes body
- *     cdef readonly int length
+ *     cdef readonly long long length
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10blacksheep_8contents_7Content_4type_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_10blacksheep_8contents_7Content_4type_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2760,15 +2765,15 @@
   return __pyx_r;
 }
 
 /* "blacksheep/contents.pxd":10
  * cdef class Content:
  *     cdef readonly bytes type
  *     cdef readonly bytes body             # <<<<<<<<<<<<<<
- *     cdef readonly int length
+ *     cdef readonly long long length
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10blacksheep_8contents_7Content_4body_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_10blacksheep_8contents_7Content_4body_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
@@ -2796,15 +2801,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "blacksheep/contents.pxd":11
  *     cdef readonly bytes type
  *     cdef readonly bytes body
- *     cdef readonly int length             # <<<<<<<<<<<<<<
+ *     cdef readonly long long length             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10blacksheep_8contents_7Content_6length_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_10blacksheep_8contents_7Content_6length_1__get__(PyObject *__pyx_v_self) {
@@ -2823,15 +2828,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 11, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2883,15 +2888,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.length, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->body);
   __Pyx_GIVEREF(__pyx_v_self->body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->body);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -3165,15 +3170,15 @@
  */
 
 /* Python wrapper */
 static int __pyx_pw_10blacksheep_8contents_15StreamedContent_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_10blacksheep_8contents_15StreamedContent_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_content_type = 0;
   PyObject *__pyx_v_data_provider = 0;
-  int __pyx_v_data_length;
+  PY_LONG_LONG __pyx_v_data_length;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
@@ -3222,17 +3227,17 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_content_type = ((PyObject*)values[0]);
     __pyx_v_data_provider = values[1];
     if (values[2]) {
-      __pyx_v_data_length = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_data_length == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
+      __pyx_v_data_length = __Pyx_PyInt_As_PY_LONG_LONG(values[2]); if (unlikely((__pyx_v_data_length == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
     } else {
-      __pyx_v_data_length = ((int)-1);
+      __pyx_v_data_length = ((PY_LONG_LONG)-1LL);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 30, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.contents.StreamedContent.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -3247,29 +3252,29 @@
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_10blacksheep_8contents_15StreamedContent___init__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self, PyObject *__pyx_v_content_type, PyObject *__pyx_v_data_provider, int __pyx_v_data_length) {
+static int __pyx_pf_10blacksheep_8contents_15StreamedContent___init__(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v_self, PyObject *__pyx_v_content_type, PyObject *__pyx_v_data_provider, PY_LONG_LONG __pyx_v_data_length) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "blacksheep/contents.pyx":36
- *         int data_length = -1
+ *         long long data_length = -1
  *     ):
  *         self.type = content_type             # <<<<<<<<<<<<<<
  *         self.body = None
  *         self.length = data_length
  */
   __Pyx_INCREF(__pyx_v_content_type);
   __Pyx_GIVEREF(__pyx_v_content_type);
@@ -4136,15 +4141,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.generator, self.length, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_INCREF(__pyx_v_self->generator);
@@ -4514,15 +4519,15 @@
   /* "blacksheep/contents.pyx":68
  *         self.type = None
  *         self.body = None
  *         self.length = -1             # <<<<<<<<<<<<<<
  *         self.receive = receive
  * 
  */
-  __pyx_v_self->__pyx_base.length = -1;
+  __pyx_v_self->__pyx_base.length = -1LL;
 
   /* "blacksheep/contents.pyx":69
  *         self.body = None
  *         self.length = -1
  *         self.receive = receive             # <<<<<<<<<<<<<<
  * 
  *     cpdef void dispose(self):
@@ -5409,15 +5414,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.length, self.receive, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -5911,15 +5916,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.length, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -6403,15 +6408,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.length, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -6935,15 +6940,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.length, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -9148,15 +9153,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.length, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_t_1);
@@ -10829,15 +10834,15 @@
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.body, self.boundary, self.length, self.parts, self.type)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_self->__pyx_base.length); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyTuple_New(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_self->__pyx_base.body);
   __Pyx_GIVEREF(__pyx_v_self->__pyx_base.body);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_self->__pyx_base.body);
   __Pyx_INCREF(__pyx_v_self->boundary);
@@ -11622,15 +11627,15 @@
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_Content__set_state(struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -11660,15 +11665,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -12046,15 +12051,15 @@
  *     if len(__pyx_state) > 4 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_StreamedContent__set_state(struct __pyx_obj_10blacksheep_8contents_StreamedContent *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -12095,15 +12100,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -12481,15 +12486,15 @@
  *     if len(__pyx_state) > 4 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_ASGIContent__set_state(struct __pyx_obj_10blacksheep_8contents_ASGIContent *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -12519,15 +12524,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -12916,15 +12921,15 @@
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_TextContent__set_state(struct __pyx_obj_10blacksheep_8contents_TextContent *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -12954,15 +12959,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -13340,15 +13345,15 @@
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_HTMLContent__set_state(struct __pyx_obj_10blacksheep_8contents_HTMLContent *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -13378,15 +13383,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -13764,15 +13769,15 @@
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_JSONContent__set_state(struct __pyx_obj_10blacksheep_8contents_JSONContent *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -13802,15 +13807,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -14188,15 +14193,15 @@
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_FormContent__set_state(struct __pyx_obj_10blacksheep_8contents_FormContent *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -14226,15 +14231,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -15062,15 +15067,15 @@
  *     if len(__pyx_state) > 5 and hasattr(__pyx_result, '__dict__'):
  */
 
 static PyObject *__pyx_f_10blacksheep_8contents___pyx_unpickle_MultiPartFormData__set_state(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
@@ -15112,15 +15117,15 @@
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v___pyx_result->__pyx_base.length = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(2, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
@@ -15247,15 +15252,15 @@
   p->body = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8contents_Content(PyObject *o) {
   struct __pyx_obj_10blacksheep_8contents_Content *p = (struct __pyx_obj_10blacksheep_8contents_Content *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->type);
   Py_CLEAR(p->body);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -15366,15 +15371,15 @@
   p->generator = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8contents_StreamedContent(PyObject *o) {
   struct __pyx_obj_10blacksheep_8contents_StreamedContent *p = (struct __pyx_obj_10blacksheep_8contents_StreamedContent *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->generator);
   if (PyType_IS_GC(__pyx_ptype_10blacksheep_8contents_Content)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_10blacksheep_8contents_Content(o);
@@ -15500,15 +15505,15 @@
   p->receive = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8contents_ASGIContent(PyObject *o) {
   struct __pyx_obj_10blacksheep_8contents_ASGIContent *p = (struct __pyx_obj_10blacksheep_8contents_ASGIContent *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->receive);
   if (PyType_IS_GC(__pyx_ptype_10blacksheep_8contents_Content)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_10blacksheep_8contents_Content(o);
@@ -15968,15 +15973,15 @@
   p->charset = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8contents_FormPart(PyObject *o) {
   struct __pyx_obj_10blacksheep_8contents_FormPart *p = (struct __pyx_obj_10blacksheep_8contents_FormPart *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->name);
   Py_CLEAR(p->data);
   Py_CLEAR(p->content_type);
   Py_CLEAR(p->file_name);
@@ -16122,15 +16127,15 @@
   p->boundary = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8contents_MultiPartFormData(PyObject *o) {
   struct __pyx_obj_10blacksheep_8contents_MultiPartFormData *p = (struct __pyx_obj_10blacksheep_8contents_MultiPartFormData *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->parts);
   Py_CLEAR(p->boundary);
   if (PyType_IS_GC(__pyx_ptype_10blacksheep_8contents_Content)) PyObject_GC_Track(o);
@@ -17463,21 +17468,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(3, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(3, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(3, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(3, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(3, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21498,18 +21503,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -21555,22 +21560,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -21853,208 +21858,208 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(PY_LONG_LONG),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
+        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (int) val;
+            return (PY_LONG_LONG) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
+                case  0: return (PY_LONG_LONG) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) >= 2 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) >= 3 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (int) -1;
+                    return (PY_LONG_LONG) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
+            if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
+                case  0: return (PY_LONG_LONG) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) - 1 > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) ((((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) ((((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) ((((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
+            if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
 #if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
                             "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
 #else
-            int val;
+            PY_LONG_LONG val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -22066,32 +22071,32 @@
                                               bytes, sizeof(val),
                                               is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
 #endif
-            return (int) -1;
+            return (PY_LONG_LONG) -1;
         }
     } else {
-        int val;
+        PY_LONG_LONG val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (int) -1;
-        val = __Pyx_PyInt_As_int(tmp);
+        if (!tmp) return (PY_LONG_LONG) -1;
+        val = __Pyx_PyInt_As_PY_LONG_LONG(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to int");
-    return (int) -1;
+        "value too large to convert to PY_LONG_LONG");
+    return (PY_LONG_LONG) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to int");
-    return (int) -1;
+        "can't convert negative value to PY_LONG_LONG");
+    return (PY_LONG_LONG) -1;
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
@@ -22320,14 +22325,210 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntFromPy */
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if (sizeof(int) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (int) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (int) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
+                case 2:
+                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
+                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
+                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
+                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        }
+                    }
+                    break;
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (int) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if (sizeof(int) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (int) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
+                case -2:
+                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        }
+                    }
+                    break;
+                case 2:
+                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        }
+                    }
+                    break;
+                case -3:
+                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        }
+                    }
+                    break;
+                case -4:
+                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        }
+                    }
+                    break;
+            }
+#endif
+            if (sizeof(int) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+#else
+            int val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+ #if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+ #endif
+            if (likely(v)) {
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+#endif
+            return (int) -1;
+        }
+    } else {
+        int val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (int) -1;
+        val = __Pyx_PyInt_As_int(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to int");
+    return (int) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to int");
+    return (int) -1;
+}
+
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
@@ -22516,28 +22717,38 @@
     return PyUnicode_FromFormat("<async_generator object %S at %p>",
                                 o->gi_qualname ? o->gi_qualname : Py_None, o);
 }
 #if PY_VERSION_HEX >= 0x030600B0
 static int
 __Pyx_async_gen_init_hooks(__pyx_PyAsyncGenObject *o)
 {
+#if !CYTHON_COMPILING_IN_PYPY
     PyThreadState *tstate;
+#endif
     PyObject *finalizer;
     PyObject *firstiter;
     if (o->ag_hooks_inited) {
         return 0;
     }
     o->ag_hooks_inited = 1;
+#if CYTHON_COMPILING_IN_PYPY
+    finalizer = _PyEval_GetAsyncGenFinalizer();
+#else
     tstate = __Pyx_PyThreadState_Current;
     finalizer = tstate->async_gen_finalizer;
+#endif
     if (finalizer) {
         Py_INCREF(finalizer);
         o->ag_finalizer = finalizer;
     }
+#if CYTHON_COMPILING_IN_PYPY
+    firstiter = _PyEval_GetAsyncGenFirstiter();
+#else
     firstiter = tstate->async_gen_firstiter;
+#endif
     if (firstiter) {
         PyObject *res;
 #if CYTHON_UNPACK_METHODS
         PyObject *self;
 #endif
         Py_INCREF(firstiter);
 #if CYTHON_UNPACK_METHODS
```

### Comparing `blacksheep-2.0a8/blacksheep/contents.pxd` & `blacksheep-2.0a9/blacksheep/contents.pxd`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This module is part of BlackSheep and is released under
 # the MIT License https://opensource.org/licenses/MIT
 
 
 cdef class Content:
     cdef readonly bytes type
     cdef readonly bytes body
-    cdef readonly int length
+    cdef readonly long long length
 
 
 cdef class StreamedContent(Content):
     cdef readonly object generator
 
 
 cdef class ASGIContent(Content):
```

### Comparing `blacksheep-2.0a8/blacksheep/contents.pyi` & `blacksheep-2.0a9/blacksheep/contents.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/contents.pyx` & `blacksheep-2.0a9/blacksheep/contents.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 cdef class StreamedContent(Content):
 
     def __init__(
         self,
         bytes content_type,
         object data_provider,
-        int data_length = -1
+        long long data_length = -1
     ):
         self.type = content_type
         self.body = None
         self.length = data_length
         self.generator = data_provider
 
         if not isasyncgenfunction(data_provider):
```

### Comparing `blacksheep-2.0a8/blacksheep/cookies.c` & `blacksheep-2.0a9/blacksheep/cookies.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -953,17 +955,17 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/cookies.pyx",
+  "blacksheep\\cookies.pyx",
   "stringsource",
-  "blacksheep/cookies.pxd",
+  "blacksheep\\cookies.pxd",
   "datetime.pxd",
   "type.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_7cookies_Cookie;
 struct __pyx_obj_10blacksheep_7cookies_CookieError;
@@ -1576,30 +1578,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
@@ -11426,15 +11428,15 @@
   p->path = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_7cookies_Cookie(PyObject *o) {
   struct __pyx_obj_10blacksheep_7cookies_Cookie *p = (struct __pyx_obj_10blacksheep_7cookies_Cookie *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_name);
   Py_CLEAR(p->_value);
   Py_CLEAR(p->expires);
@@ -11702,15 +11704,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_7cookies_CookieError(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
@@ -11892,15 +11894,15 @@
   PyObject *o = (&PyType_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc___Pyx_EnumMeta(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&PyType_Type)->tp_dealloc(o);
 }
@@ -12441,29 +12443,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -15172,18 +15174,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -15229,22 +15231,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `blacksheep-2.0a8/blacksheep/cookies.pxd` & `blacksheep-2.0a9/blacksheep/cookies.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/cookies.pyi` & `blacksheep-2.0a9/blacksheep/cookies.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/cookies.pyx` & `blacksheep-2.0a9/blacksheep/cookies.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/exceptions.c` & `blacksheep-2.0a9/blacksheep/exceptions.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -950,17 +952,17 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/exceptions.pyx",
+  "blacksheep\\exceptions.pyx",
   "stringsource",
-  "blacksheep/exceptions.pxd",
+  "blacksheep\\exceptions.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_10exceptions_MessageAborted;
 struct __pyx_obj_10blacksheep_10exceptions_HTTPException;
 struct __pyx_obj_10blacksheep_10exceptions_BadRequest;
 struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat;
@@ -11923,15 +11925,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_10exceptions_MessageAborted(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
@@ -12029,15 +12031,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_10exceptions_HTTPException(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
@@ -12242,15 +12244,15 @@
   p->inner_exception = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_10exceptions_BadRequestFormat(PyObject *o) {
   struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat *p = (struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->inner_exception);
   PyObject_GC_Track(o);
   __pyx_tp_dealloc_10blacksheep_10exceptions_HTTPException(o);
@@ -12460,15 +12462,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_10exceptions_InvalidArgument(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
@@ -12566,15 +12568,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_10exceptions_InvalidOperation(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
```

### Comparing `blacksheep-2.0a8/blacksheep/exceptions.pyi` & `blacksheep-2.0a9/blacksheep/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/exceptions.pyx` & `blacksheep-2.0a9/blacksheep/exceptions.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/headers.c` & `blacksheep-2.0a9/blacksheep/headers.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -950,15 +952,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/headers.pyx",
+  "blacksheep\\headers.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_7headers_Header;
 struct __pyx_obj_10blacksheep_7headers_Headers;
 struct __pyx_obj_10blacksheep_7headers___pyx_scope_struct____iter__;
@@ -1768,15 +1770,15 @@
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_blacksheep_headers[] = "blacksheep.headers";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_pyx_unpickle_Header[] = "__pyx_unpickle_Header";
 static const char __pyx_k_pyx_unpickle_Headers[] = "__pyx_unpickle_Headers";
-static const char __pyx_k_blacksheep_headers_pyx[] = "blacksheep/headers.pyx";
+static const char __pyx_k_blacksheep_headers_pyx[] = "blacksheep\\headers.pyx";
 static const char __pyx_k_Cannot_add_an_invalid_tuple[] = "Cannot add, an invalid tuple ";
 static const char __pyx_k_values_must_be_Dict_bytes_bytes[] = "values must be Dict[bytes, bytes] or List[Header]";
 static const char __pyx_k_Headers_contains_more_than_one_h[] = "Headers contains more than one header with the given key";
 static const char __pyx_k_Headers_does_not_contain_one_hea[] = "Headers does not contain one header with the given key";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xfa7a105, 0xaaf55bf, 0xe891e3f) = (name, value))";
 static const char __pyx_k_The_sequence_contains_invalid_el[] = "The sequence contains invalid elements: cannot add ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0xf09cc7e, 0x89445ea, 0x048b0cb) = (values))";
@@ -9009,15 +9011,15 @@
   p->value = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_7headers_Header(PyObject *o) {
   struct __pyx_obj_10blacksheep_7headers_Header *p = (struct __pyx_obj_10blacksheep_7headers_Header *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->name);
   Py_CLEAR(p->value);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -9151,15 +9153,15 @@
   p->values = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_7headers_Headers(PyObject *o) {
   struct __pyx_obj_10blacksheep_7headers_Headers *p = (struct __pyx_obj_10blacksheep_7headers_Headers *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->values);
   (*Py_TYPE(o)->tp_free)(o);
 }
```

### Comparing `blacksheep-2.0a8/blacksheep/headers.pxd` & `blacksheep-2.0a9/blacksheep/headers.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/headers.pyi` & `blacksheep-2.0a9/blacksheep/headers.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/headers.pyx` & `blacksheep-2.0a9/blacksheep/headers.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/messages.c` & `blacksheep-2.0a9/blacksheep/messages.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -953,24 +955,24 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/messages.pyx",
-  "blacksheep/messages.pxd",
+  "blacksheep\\messages.pyx",
+  "blacksheep\\messages.pxd",
   "stringsource",
   "datetime.pxd",
-  "blacksheep/contents.pxd",
+  "blacksheep\\contents.pxd",
   "type.pxd",
-  "blacksheep/cookies.pxd",
-  "blacksheep/exceptions.pxd",
-  "blacksheep/url.pxd",
-  "blacksheep/headers.pxd",
+  "blacksheep\\cookies.pxd",
+  "blacksheep\\exceptions.pxd",
+  "blacksheep\\url.pxd",
+  "blacksheep\\headers.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_8contents_Content;
 struct __pyx_obj_10blacksheep_8contents_StreamedContent;
 struct __pyx_obj_10blacksheep_8contents_ASGIContent;
 struct __pyx_obj_10blacksheep_8contents_TextContent;
@@ -1022,15 +1024,15 @@
  *     cdef readonly bytes type
  *     cdef readonly bytes body
  */
 struct __pyx_obj_10blacksheep_8contents_Content {
   PyObject_HEAD
   PyObject *type;
   PyObject *body;
-  int length;
+  PY_LONG_LONG length;
 };
 
 
 /* "contents.pxd":14
  * 
  * 
  * cdef class StreamedContent(Content):             # <<<<<<<<<<<<<<
@@ -2268,30 +2270,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* ClassMethod.proto */
 #include "descrobject.h"
@@ -2379,15 +2381,15 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static struct __pyx_obj_10blacksheep_8messages_Message *__pyx_f_10blacksheep_8messages_7Message_with_content(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_content, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_10blacksheep_8messages_7Message_get_first_header(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_key, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_10blacksheep_8messages_7Message_get_headers(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_key, int __pyx_skip_dispatch); /* proto*/
@@ -20389,15 +20391,15 @@
   p->content = ((struct __pyx_obj_10blacksheep_8contents_Content *)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8messages_Message(PyObject *o) {
   struct __pyx_obj_10blacksheep_8messages_Message *p = (struct __pyx_obj_10blacksheep_8messages_Message *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   if (p->__weakref__) PyObject_ClearWeakRefs(o);
   Py_CLEAR(p->__pyx___headers);
   Py_CLEAR(p->content);
@@ -20572,15 +20574,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8messages_Request(PyObject *o) {
   struct __pyx_obj_10blacksheep_8messages_Request *p = (struct __pyx_obj_10blacksheep_8messages_Request *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   if (p->__dict__) PyDict_Clear(p->__dict__);
   Py_CLEAR(p->method);
   Py_CLEAR(p->_url);
@@ -20983,15 +20985,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_8messages_Response(PyObject *o) {
   struct __pyx_obj_10blacksheep_8messages_Response *p = (struct __pyx_obj_10blacksheep_8messages_Response *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   if (p->__dict__) PyDict_Clear(p->__dict__);
   Py_CLEAR(p->__dict__);
   PyObject_GC_Track(o);
@@ -22566,67 +22568,67 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(4, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(4, 14, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(4, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(4, 14, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(4, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8contents_ASGIContent = (struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8contents_ASGIContent->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8contents_ASGIContent)) __PYX_ERR(4, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(4, 23, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(4, 27, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(4, 31, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(4, 35, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(4, 39, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(4, 47, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(4, 23, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(4, 27, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(4, 31, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(4, 35, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(4, 39, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(4, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(6, 17, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(6, 17, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7cookies_Cookie = (struct __pyx_vtabstruct_10blacksheep_7cookies_Cookie*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7cookies_Cookie->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7cookies_Cookie)) __PYX_ERR(6, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(7, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(7, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(7, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(7, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(7, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(7, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(7, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(7, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(7, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(7, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(7, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(7, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(7, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(7, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_3url_URL = (struct __pyx_vtabstruct_10blacksheep_3url_URL*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_3url_URL->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_3url_URL)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.headers"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7headers_Header = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.headers", "Header", sizeof(struct __pyx_obj_10blacksheep_7headers_Header), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7headers_Header),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7headers_Header) __PYX_ERR(9, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_7headers_Headers = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.headers", "Headers", sizeof(struct __pyx_obj_10blacksheep_7headers_Headers), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7headers_Headers),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7headers_Headers) __PYX_ERR(9, 13, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7headers_Header = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.headers", "Header", sizeof(struct __pyx_obj_10blacksheep_7headers_Header), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_7headers_Header),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_7headers_Header) __PYX_ERR(9, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7headers_Headers = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.headers", "Headers", sizeof(struct __pyx_obj_10blacksheep_7headers_Headers), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_7headers_Headers),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_7headers_Headers) __PYX_ERR(9, 13, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7headers_Headers = (struct __pyx_vtabstruct_10blacksheep_7headers_Headers*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7headers_Headers->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7headers_Headers)) __PYX_ERR(9, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -22647,27 +22649,27 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "multiparts_to_dictionary", (void (**)(void))&__pyx_f_10blacksheep_8contents_multiparts_to_dictionary, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "multiparts_to_dictionary", (void (**)(void))&__pyx_f_10blacksheep_8contents_multiparts_to_dictionary, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "split_value", (void (**)(void))&__pyx_f_10blacksheep_7cookies_split_value, "PyObject *(PyObject *, PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "split_value", (void (**)(void))&__pyx_f_10blacksheep_7cookies_split_value, "PyObject *(PyObject *, PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "build_absolute_url", (void (**)(void))&__pyx_f_10blacksheep_3url_build_absolute_url, "struct __pyx_obj_10blacksheep_3url_URL *(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "build_absolute_url", (void (**)(void))&__pyx_f_10blacksheep_3url_build_absolute_url, "struct __pyx_obj_10blacksheep_3url_URL *(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -27069,18 +27071,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -27126,22 +27128,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -28043,28 +28045,38 @@
     return PyUnicode_FromFormat("<async_generator object %S at %p>",
                                 o->gi_qualname ? o->gi_qualname : Py_None, o);
 }
 #if PY_VERSION_HEX >= 0x030600B0
 static int
 __Pyx_async_gen_init_hooks(__pyx_PyAsyncGenObject *o)
 {
+#if !CYTHON_COMPILING_IN_PYPY
     PyThreadState *tstate;
+#endif
     PyObject *finalizer;
     PyObject *firstiter;
     if (o->ag_hooks_inited) {
         return 0;
     }
     o->ag_hooks_inited = 1;
+#if CYTHON_COMPILING_IN_PYPY
+    finalizer = _PyEval_GetAsyncGenFinalizer();
+#else
     tstate = __Pyx_PyThreadState_Current;
     finalizer = tstate->async_gen_finalizer;
+#endif
     if (finalizer) {
         Py_INCREF(finalizer);
         o->ag_finalizer = finalizer;
     }
+#if CYTHON_COMPILING_IN_PYPY
+    firstiter = _PyEval_GetAsyncGenFirstiter();
+#else
     firstiter = tstate->async_gen_firstiter;
+#endif
     if (firstiter) {
         PyObject *res;
 #if CYTHON_UNPACK_METHODS
         PyObject *self;
 #endif
         Py_INCREF(firstiter);
 #if CYTHON_UNPACK_METHODS
@@ -28905,17 +28917,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
-#define __PYX_HAVE_RT_ImportFunction_0_29_35
-static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `blacksheep-2.0a8/blacksheep/messages.pxd` & `blacksheep-2.0a9/blacksheep/messages.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/messages.pyi` & `blacksheep-2.0a9/blacksheep/messages.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/messages.pyx` & `blacksheep-2.0a9/blacksheep/messages.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/middlewares.py` & `blacksheep-2.0a9/blacksheep/middlewares.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/multipart.py` & `blacksheep-2.0a9/blacksheep/multipart.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/ranges.py` & `blacksheep-2.0a9/blacksheep/ranges.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/scribe.c` & `blacksheep-2.0a9/blacksheep/scribe.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -953,22 +955,22 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/scribe.pyx",
+  "blacksheep\\scribe.pyx",
   "datetime.pxd",
-  "blacksheep/contents.pxd",
+  "blacksheep\\contents.pxd",
   "type.pxd",
-  "blacksheep/cookies.pxd",
-  "blacksheep/exceptions.pxd",
-  "blacksheep/url.pxd",
-  "blacksheep/messages.pxd",
+  "blacksheep\\cookies.pxd",
+  "blacksheep\\exceptions.pxd",
+  "blacksheep\\url.pxd",
+  "blacksheep\\messages.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_8contents_Content;
 struct __pyx_obj_10blacksheep_8contents_StreamedContent;
 struct __pyx_obj_10blacksheep_8contents_ASGIContent;
 struct __pyx_obj_10blacksheep_8contents_TextContent;
@@ -1018,15 +1020,15 @@
  *     cdef readonly bytes type
  *     cdef readonly bytes body
  */
 struct __pyx_obj_10blacksheep_8contents_Content {
   PyObject_HEAD
   PyObject *type;
   PyObject *body;
-  int length;
+  PY_LONG_LONG length;
 };
 
 
 /* "contents.pxd":14
  * 
  * 
  * cdef class StreamedContent(Content):             # <<<<<<<<<<<<<<
@@ -2008,30 +2010,30 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2072,14 +2074,17 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -2146,15 +2151,15 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'blacksheep.contents' */
 static PyTypeObject *__pyx_ptype_10blacksheep_8contents_Content = 0;
@@ -2314,15 +2319,15 @@
 static const char __pyx_k_write_response[] = "write_response";
 static const char __pyx_k_blacksheep_scribe[] = "blacksheep.scribe";
 static const char __pyx_k_transfer_encoding[] = "transfer-encoding";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_http_response_body[] = "http.response.body";
 static const char __pyx_k_send_asgi_response[] = "send_asgi_response";
 static const char __pyx_k_http_response_start[] = "http.response.start";
-static const char __pyx_k_blacksheep_scribe_pyx[] = "blacksheep/scribe.pyx";
+static const char __pyx_k_blacksheep_scribe_pyx[] = "blacksheep\\scribe.pyx";
 static const char __pyx_k_write_response_content[] = "write_response_content";
 static const char __pyx_k_Missing_request_content[] = "Missing request content";
 static const char __pyx_k_write_request_body_only[] = "write_request_body_only";
 static const char __pyx_k_application_octet_stream[] = "application/octet-stream";
 static PyObject *__pyx_kp_b_;
 static PyObject *__pyx_kp_b_0;
 static PyObject *__pyx_kp_b_0_2;
@@ -3436,15 +3441,15 @@
  *         message._add_header(b'transfer-encoding', b'chunked')
  *     else:
  *         message._add_header(b'content-length', str(content.length).encode())             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_content->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_content->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_4), NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -3595,15 +3600,15 @@
  *         message._add_header_if_missing(b'transfer-encoding', b'chunked')
  *     else:
  *         message._add_header_if_missing(b'content-length', str(content.length).encode())             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_content->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_content->length); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = PyUnicode_AsEncodedString(((PyObject*)__pyx_t_4), NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -10677,70 +10682,70 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(2, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(2, 14, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(2, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(2, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(2, 14, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(2, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8contents_ASGIContent = (struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8contents_ASGIContent->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8contents_ASGIContent)) __PYX_ERR(2, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(2, 23, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(2, 27, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(2, 31, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(2, 35, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(2, 39, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(2, 47, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(2, 23, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(2, 27, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(2, 31, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(2, 35, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(2, 39, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(2, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(1, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(1, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(1, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(1, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(1, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(1, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_36(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(4, 17, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(4, 17, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7cookies_Cookie = (struct __pyx_vtabstruct_10blacksheep_7cookies_Cookie*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7cookies_Cookie->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7cookies_Cookie)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(5, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(5, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(5, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(5, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(5, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(5, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(5, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(5, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(5, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(5, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(5, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(5, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(5, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(6, 8, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_3url_URL = (struct __pyx_vtabstruct_10blacksheep_3url_URL*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_3url_URL->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_3url_URL)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.messages"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Message),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(7, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8messages_Message),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(7, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Message = (struct __pyx_vtabstruct_10blacksheep_8messages_Message*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Message->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Message)) __PYX_ERR(7, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Request),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(7, 45, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8messages_Request),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(7, 45, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Request = (struct __pyx_vtabstruct_10blacksheep_8messages_Request*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Request->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Request)) __PYX_ERR(7, 45, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Response),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(7, 58, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType_0_29_36(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10blacksheep_8messages_Response),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(7, 58, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Response = (struct __pyx_vtabstruct_10blacksheep_8messages_Response*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Response->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Response)) __PYX_ERR(7, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -10761,21 +10766,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_36(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -14116,18 +14121,18 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -14173,22 +14178,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -14802,14 +14807,52 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(PY_LONG_LONG),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -15236,28 +15279,38 @@
     return PyUnicode_FromFormat("<async_generator object %S at %p>",
                                 o->gi_qualname ? o->gi_qualname : Py_None, o);
 }
 #if PY_VERSION_HEX >= 0x030600B0
 static int
 __Pyx_async_gen_init_hooks(__pyx_PyAsyncGenObject *o)
 {
+#if !CYTHON_COMPILING_IN_PYPY
     PyThreadState *tstate;
+#endif
     PyObject *finalizer;
     PyObject *firstiter;
     if (o->ag_hooks_inited) {
         return 0;
     }
     o->ag_hooks_inited = 1;
+#if CYTHON_COMPILING_IN_PYPY
+    finalizer = _PyEval_GetAsyncGenFinalizer();
+#else
     tstate = __Pyx_PyThreadState_Current;
     finalizer = tstate->async_gen_finalizer;
+#endif
     if (finalizer) {
         Py_INCREF(finalizer);
         o->ag_finalizer = finalizer;
     }
+#if CYTHON_COMPILING_IN_PYPY
+    firstiter = _PyEval_GetAsyncGenFirstiter();
+#else
     firstiter = tstate->async_gen_firstiter;
+#endif
     if (firstiter) {
         PyObject *res;
 #if CYTHON_UNPACK_METHODS
         PyObject *self;
 #endif
         Py_INCREF(firstiter);
 #if CYTHON_UNPACK_METHODS
@@ -16204,17 +16257,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
-#define __PYX_HAVE_RT_ImportFunction_0_29_35
-static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_36
+#define __PYX_HAVE_RT_ImportFunction_0_29_36
+static int __Pyx_ImportFunction_0_29_36(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `blacksheep-2.0a8/blacksheep/scribe.pxd` & `blacksheep-2.0a9/blacksheep/scribe.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/scribe.pyi` & `blacksheep-2.0a9/blacksheep/scribe.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/scribe.pyx` & `blacksheep-2.0a9/blacksheep/scribe.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/application.py` & `blacksheep-2.0a9/blacksheep/server/application.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/asgi.py` & `blacksheep-2.0a9/blacksheep/server/asgi.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/authentication/__init__.py` & `blacksheep-2.0a9/blacksheep/server/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/authentication/cookie.py` & `blacksheep-2.0a9/blacksheep/server/authentication/cookie.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/authentication/jwt.py` & `blacksheep-2.0a9/blacksheep/server/authentication/jwt.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/authentication/oidc.py` & `blacksheep-2.0a9/blacksheep/server/authentication/oidc.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/authorization/__init__.py` & `blacksheep-2.0a9/blacksheep/server/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/bindings.py` & `blacksheep-2.0a9/blacksheep/server/bindings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/compression.py` & `blacksheep-2.0a9/blacksheep/server/compression.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/controllers.py` & `blacksheep-2.0a9/blacksheep/server/controllers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/cors.py` & `blacksheep-2.0a9/blacksheep/server/cors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/csrf.py` & `blacksheep-2.0a9/blacksheep/server/csrf.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/dataprotection.py` & `blacksheep-2.0a9/blacksheep/server/dataprotection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/di.py` & `blacksheep-2.0a9/blacksheep/server/di.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/env.py` & `blacksheep-2.0a9/blacksheep/server/env.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/errors.py` & `blacksheep-2.0a9/blacksheep/server/errors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/files/__init__.py` & `blacksheep-2.0a9/blacksheep/server/files/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/files/dynamic.py` & `blacksheep-2.0a9/blacksheep/server/files/dynamic.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/files/static.py` & `blacksheep-2.0a9/blacksheep/server/files/static.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/headers/cache.py` & `blacksheep-2.0a9/blacksheep/server/headers/cache.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/normalization.py` & `blacksheep-2.0a9/blacksheep/server/normalization.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/openapi/common.py` & `blacksheep-2.0a9/blacksheep/server/openapi/common.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/openapi/docstrings.py` & `blacksheep-2.0a9/blacksheep/server/openapi/docstrings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/openapi/ui.py` & `blacksheep-2.0a9/blacksheep/server/openapi/ui.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/openapi/v3.py` & `blacksheep-2.0a9/blacksheep/server/openapi/v3.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/remotes/forwarding.py` & `blacksheep-2.0a9/blacksheep/server/remotes/forwarding.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/remotes/hosts.py` & `blacksheep-2.0a9/blacksheep/server/remotes/hosts.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/rendering/abc.py` & `blacksheep-2.0a9/blacksheep/server/rendering/abc.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/rendering/jinja2.py` & `blacksheep-2.0a9/blacksheep/server/rendering/jinja2.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/res/error.css` & `blacksheep-2.0a9/blacksheep/server/res/error.css`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/res/error.html` & `blacksheep-2.0a9/blacksheep/server/res/error.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/res/redoc-ui.html` & `blacksheep-2.0a9/blacksheep/server/res/redoc-ui.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/res/swagger-ui.html` & `blacksheep-2.0a9/blacksheep/server/res/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/responses.py` & `blacksheep-2.0a9/blacksheep/server/responses.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/routing.py` & `blacksheep-2.0a9/blacksheep/server/routing.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/security/hsts.py` & `blacksheep-2.0a9/blacksheep/server/security/hsts.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/server/websocket.py` & `blacksheep-2.0a9/blacksheep/server/websocket.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/sessions/__init__.py` & `blacksheep-2.0a9/blacksheep/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/settings/di.py` & `blacksheep-2.0a9/blacksheep/settings/di.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/settings/html.py` & `blacksheep-2.0a9/blacksheep/settings/html.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/settings/json.py` & `blacksheep-2.0a9/blacksheep/settings/json.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/testing/client.py` & `blacksheep-2.0a9/blacksheep/testing/client.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/testing/helpers.py` & `blacksheep-2.0a9/blacksheep/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/testing/messages.py` & `blacksheep-2.0a9/blacksheep/testing/messages.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/testing/simulator.py` & `blacksheep-2.0a9/blacksheep/testing/simulator.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/url.c` & `blacksheep-2.0a9/blacksheep/url.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -81,15 +81,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -365,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -445,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -950,17 +952,17 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "blacksheep/url.pyx",
+  "blacksheep\\url.pyx",
   "stringsource",
-  "blacksheep/url.pxd",
+  "blacksheep\\url.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10blacksheep_3url_URL;
 struct __pyx_obj_10blacksheep_3url_InvalidURL;
 
 /* "blacksheep/url.pxd":8
@@ -1586,15 +1588,15 @@
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_NotImplemented[] = "NotImplemented";
 static const char __pyx_k_blacksheep_url[] = "blacksheep.url";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_httptools_parser[] = "httptools.parser";
 static const char __pyx_k_pyx_unpickle_URL[] = "__pyx_unpickle_URL";
-static const char __pyx_k_blacksheep_url_pyx[] = "blacksheep/url.pyx";
+static const char __pyx_k_blacksheep_url_pyx[] = "blacksheep\\url.pyx";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_pyx_unpickle_InvalidURL[] = "__pyx_unpickle_InvalidURL";
 static const char __pyx_k_HttpParserInvalidURLError[] = "HttpParserInvalidURLError";
 static const char __pyx_k_Cannot_concatenate_a_URL_with_qu[] = "Cannot concatenate a URL with query or fragment to another URL portion";
 static const char __pyx_k_Cannot_concatenate_to_an_absolut[] = "Cannot concatenate to an absolute URL (";
 static const char __pyx_k_Cannot_generate_a_URL_from_a_par[] = "Cannot generate a URL from a partial URL";
 static const char __pyx_k_Expected_http_or_https_schema_go[] = "Expected http or https schema; got instead ";
@@ -6418,15 +6420,15 @@
   p->fragment = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_3url_URL(PyObject *o) {
   struct __pyx_obj_10blacksheep_3url_URL *p = (struct __pyx_obj_10blacksheep_3url_URL *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->value);
   Py_CLEAR(p->schema);
   Py_CLEAR(p->host);
   Py_CLEAR(p->path);
@@ -6650,15 +6652,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_10blacksheep_3url_InvalidURL(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
```

### Comparing `blacksheep-2.0a8/blacksheep/url.pxd` & `blacksheep-2.0a9/blacksheep/url.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/url.pyi` & `blacksheep-2.0a9/blacksheep/url.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/url.pyx` & `blacksheep-2.0a9/blacksheep/url.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/utils/__init__.py` & `blacksheep-2.0a9/blacksheep/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/utils/aio.py` & `blacksheep-2.0a9/blacksheep/utils/aio.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep/utils/meta.py` & `blacksheep-2.0a9/blacksheep/utils/meta.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/blacksheep.egg-info/PKG-INFO` & `blacksheep-2.0a9/blacksheep.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,687 +1,706 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 626c 6163  : 2.1.Name: blac
-00000020: 6b73 6865 6570 0a56 6572 7369 6f6e 3a20  ksheep.Version: 
-00000030: 322e 3061 380a 5375 6d6d 6172 793a 2046  2.0a8.Summary: F
-00000040: 6173 7420 7765 6220 6672 616d 6577 6f72  ast web framewor
-00000050: 6b20 666f 7220 5079 7468 6f6e 2061 7379  k for Python asy
-00000060: 6e63 696f 0a41 7574 686f 722d 656d 6169  ncio.Author-emai
-00000070: 6c3a 2052 6f62 6572 746f 2050 7265 7661  l: Roberto Preva
-00000080: 746f 203c 726f 6265 7274 6f2e 7072 6576  to <roberto.prev
-00000090: 6174 6f40 676d 6169 6c2e 636f 6d3e 0a50  ato@gmail.com>.P
-000000a0: 726f 6a65 6374 2d55 524c 3a20 486f 6d65  roject-URL: Home
-000000b0: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
-000000c0: 7468 7562 2e63 6f6d 2f4e 656f 7465 726f  thub.com/Neotero
-000000d0: 692f 426c 6163 6b53 6865 6570 0a50 726f  i/BlackSheep.Pro
-000000e0: 6a65 6374 2d55 524c 3a20 4275 6720 5472  ject-URL: Bug Tr
-000000f0: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
-00000100: 6974 6875 622e 636f 6d2f 4e65 6f74 6572  ithub.com/Neoter
-00000110: 6f69 2f42 6c61 636b 5368 6565 702f 6973  oi/BlackSheep/is
-00000120: 7375 6573 0a4b 6579 776f 7264 733a 2062  sues.Keywords: b
-00000130: 6c61 636b 7368 6565 702c 7765 6220 6672  lacksheep,web fr
-00000140: 616d 6577 6f72 6b2c 6173 796e 6369 6f0a  amework,asyncio.
-00000150: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
-00000160: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-00000170: 3a20 3320 2d20 416c 7068 610a 436c 6173  : 3 - Alpha.Clas
-00000180: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000190: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001a0: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
-000001b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-000001e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000001f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000200: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000210: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-00000220: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000230: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000240: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
-00000250: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000260: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000270: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-00000280: 6965 723a 2045 6e76 6972 6f6e 6d65 6e74  ier: Environment
-00000290: 203a 3a20 5765 6220 456e 7669 726f 6e6d   :: Web Environm
-000002a0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-000002b0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000002c0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000002d0: 6e74 0a43 6c61 7373 6966 6965 723a 2046  nt.Classifier: F
-000002e0: 7261 6d65 776f 726b 203a 3a20 4173 796e  ramework :: Asyn
-000002f0: 6349 4f0a 5265 7175 6972 6573 2d50 7974  cIO.Requires-Pyt
-00000300: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
-00000310: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000320: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000330: 776e 0a50 726f 7669 6465 732d 4578 7472  wn.Provides-Extr
-00000340: 613a 206a 696e 6a61 0a50 726f 7669 6465  a: jinja.Provide
-00000350: 732d 4578 7472 613a 2066 756c 6c0a 4c69  s-Extra: full.Li
-00000360: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000370: 4e53 450a 0a5b 215b 4275 696c 645d 2868  NSE..[![Build](h
-00000380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000390: 6d2f 4e65 6f74 6572 6f69 2f42 6c61 636b  m/Neoteroi/Black
-000003a0: 5368 6565 702f 776f 726b 666c 6f77 732f  Sheep/workflows/
-000003b0: 4d61 696e 2f62 6164 6765 2e73 7667 295d  Main/badge.svg)]
-000003c0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000003d0: 636f 6d2f 4e65 6f74 6572 6f69 2f42 6c61  com/Neoteroi/Bla
-000003e0: 636b 5368 6565 702f 6163 7469 6f6e 7329  ckSheep/actions)
-000003f0: 0a5b 215b 7079 7069 5d28 6874 7470 733a  .[![pypi](https:
-00000400: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000410: 2f70 7970 692f 762f 426c 6163 6b53 6865  /pypi/v/BlackShe
-00000420: 6570 2e73 7667 3f63 6f6c 6f72 3d62 6c75  ep.svg?color=blu
-00000430: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
-00000440: 2e6f 7267 2f70 726f 6a65 6374 2f42 6c61  .org/project/Bla
-00000450: 636b 5368 6565 702f 290a 5b21 5b76 6572  ckSheep/).[![ver
-00000460: 7369 6f6e 735d 2868 7474 7073 3a2f 2f69  sions](https://i
-00000470: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000480: 7069 2f70 7976 6572 7369 6f6e 732f 626c  pi/pyversions/bl
-00000490: 6163 6b73 6865 6570 2e73 7667 295d 2868  acksheep.svg)](h
-000004a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000004b0: 6d2f 726f 6265 7274 6f70 7265 7661 746f  m/robertoprevato
-000004c0: 2f62 6c61 636b 7368 6565 7029 0a5b 215b  /blacksheep).[![
-000004d0: 636f 6465 636f 765d 2868 7474 7073 3a2f  codecov](https:/
-000004e0: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f4e  /codecov.io/gh/N
-000004f0: 656f 7465 726f 692f 426c 6163 6b53 6865  eoteroi/BlackShe
-00000500: 6570 2f62 7261 6e63 682f 6d61 7374 6572  ep/branch/master
-00000510: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-00000520: 3f74 6f6b 656e 3d4e 7a69 3239 4c30 4567  ?token=Nzi29L0Eg
-00000530: 3129 5d28 6874 7470 733a 2f2f 636f 6465  1)](https://code
-00000540: 636f 762e 696f 2f67 682f 4e65 6f74 6572  cov.io/gh/Neoter
-00000550: 6f69 2f42 6c61 636b 5368 6565 7029 0a5b  oi/BlackSheep).[
-00000560: 215b 6c69 6365 6e73 655d 2868 7474 7073  ![license](https
-00000570: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000580: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00000590: 2f4e 656f 7465 726f 692f 626c 6163 6b73  /Neoteroi/blacks
-000005a0: 6865 6570 2e73 7667 295d 2868 7474 7073  heep.svg)](https
-000005b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e65  ://github.com/Ne
-000005c0: 6f74 6572 6f69 2f62 6c61 636b 7368 6565  oteroi/blackshee
-000005d0: 702f 626c 6f62 2f6d 6169 6e2f 4c49 4345  p/blob/main/LICE
-000005e0: 4e53 4529 205b 215b 4a6f 696e 2074 6865  NSE) [![Join the
-000005f0: 2063 6861 7420 6174 2068 7474 7073 3a2f   chat at https:/
-00000600: 2f67 6974 7465 722e 696d 2f4e 656f 7465  /gitter.im/Neote
-00000610: 726f 692f 426c 6163 6b53 6865 6570 5d28  roi/BlackSheep](
-00000620: 6874 7470 733a 2f2f 6261 6467 6573 2e67  https://badges.g
-00000630: 6974 7465 722e 696d 2f4e 656f 7465 726f  itter.im/Neotero
-00000640: 692f 426c 6163 6b53 6865 6570 2e73 7667  i/BlackSheep.svg
-00000650: 295d 2868 7474 7073 3a2f 2f67 6974 7465  )](https://gitte
-00000660: 722e 696d 2f4e 656f 7465 726f 692f 426c  r.im/Neoteroi/Bl
-00000670: 6163 6b53 6865 6570 3f75 746d 5f73 6f75  ackSheep?utm_sou
-00000680: 7263 653d 6261 6467 6526 7574 6d5f 6d65  rce=badge&utm_me
-00000690: 6469 756d 3d62 6164 6765 2675 746d 5f63  dium=badge&utm_c
-000006a0: 616d 7061 6967 6e3d 7072 2d62 6164 6765  ampaign=pr-badge
-000006b0: 2675 746d 5f63 6f6e 7465 6e74 3d62 6164  &utm_content=bad
-000006c0: 6765 2920 5b21 5b64 6f63 756d 656e 7461  ge) [![documenta
-000006d0: 7469 6f6e 5d28 6874 7470 733a 2f2f 696d  tion](https://im
-000006e0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000006f0: 6765 2ff0 9f93 962d 646f 6373 2d70 7572  ge/....-docs-pur
-00000700: 706c 6529 5d28 6874 7470 733a 2f2f 7777  ple)](https://ww
-00000710: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
-00000720: 6c61 636b 7368 6565 702f 290a 0a23 2042  lacksheep/)..# B
-00000730: 6c61 636b 5368 6565 700a 426c 6163 6b53  lackSheep.BlackS
-00000740: 6865 6570 2069 7320 616e 2061 7379 6e63  heep is an async
-00000750: 6872 6f6e 6f75 7320 7765 6220 6672 616d  hronous web fram
-00000760: 6577 6f72 6b20 746f 2062 7569 6c64 2065  ework to build e
-00000770: 7665 6e74 2062 6173 6564 2077 6562 0a61  vent based web.a
-00000780: 7070 6c69 6361 7469 6f6e 7320 7769 7468  pplications with
-00000790: 2050 7974 686f 6e2e 2049 7420 6973 2069   Python. It is i
-000007a0: 6e73 7069 7265 6420 6279 0a5b 466c 6173  nspired by.[Flas
-000007b0: 6b5d 2868 7474 7073 3a2f 2f70 616c 6c65  k](https://palle
-000007c0: 7473 7072 6f6a 6563 7473 2e63 6f6d 2f70  tsprojects.com/p
-000007d0: 2f66 6c61 736b 2f29 2c20 5b41 5350 2e4e  /flask/), [ASP.N
-000007e0: 4554 0a43 6f72 655d 2868 7474 7073 3a2f  ET.Core](https:/
-000007f0: 2f64 6f63 732e 6d69 6372 6f73 6f66 742e  /docs.microsoft.
-00000800: 636f 6d2f 656e 2d75 732f 6173 706e 6574  com/en-us/aspnet
-00000810: 2f63 6f72 652f 292c 2061 6e64 2074 6865  /core/), and the
-00000820: 2077 6f72 6b20 6279 205b 5975 7279 0a53   work by [Yury.S
-00000830: 656c 6976 616e 6f76 5d28 6874 7470 733a  elivanov](https:
-00000840: 2f2f 6d61 6769 632e 696f 2f62 6c6f 672f  //magic.io/blog/
-00000850: 7576 6c6f 6f70 2d62 6c61 7a69 6e67 2d66  uvloop-blazing-f
-00000860: 6173 742d 7079 7468 6f6e 2d6e 6574 776f  ast-python-netwo
-00000870: 726b 696e 672f 292e 0a0a 3c70 2061 6c69  rking/)...<p ali
-00000880: 676e 3d22 6c65 6674 223e 0a20 203c 6120  gn="left">.  <a 
-00000890: 6872 6566 3d22 2362 6c61 636b 7368 6565  href="#blackshee
-000008a0: 7022 3e3c 696d 6720 7769 6474 683d 2233  p"><img width="3
-000008b0: 3230 2220 6865 6967 6874 3d22 3237 3122  20" height="271"
-000008c0: 2073 7263 3d22 6874 7470 733a 2f2f 7777   src="https://ww
-000008d0: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
-000008e0: 6c61 636b 7368 6565 702f 696d 672f 626c  lacksheep/img/bl
-000008f0: 6163 6b73 6865 6570 2e70 6e67 2220 616c  acksheep.png" al
-00000900: 743d 2242 6c61 636b 2053 6865 6570 223e  t="Black Sheep">
-00000910: 3c2f 613e 0a3c 2f70 3e0a 0a60 6060 6261  </a>.</p>..```ba
-00000920: 7368 0a70 6970 2069 6e73 7461 6c6c 2062  sh.pip install b
-00000930: 6c61 636b 7368 6565 700a 6060 600a 0a2d  lacksheep.```..-
-00000940: 2d2d 0a0a 6060 6070 7974 686f 6e0a 6672  --..```python.fr
-00000950: 6f6d 2064 6174 6574 696d 6520 696d 706f  om datetime impo
-00000960: 7274 2064 6174 6574 696d 650a 0a66 726f  rt datetime..fro
-00000970: 6d20 626c 6163 6b73 6865 6570 2069 6d70  m blacksheep imp
-00000980: 6f72 7420 4170 706c 6963 6174 696f 6e0a  ort Application.
-00000990: 0a0a 6170 7020 3d20 4170 706c 6963 6174  ..app = Applicat
-000009a0: 696f 6e28 290a 0a40 6170 702e 726f 7574  ion()..@app.rout
-000009b0: 6528 222f 2229 0a61 7379 6e63 2064 6566  e("/").async def
-000009c0: 2068 6f6d 6528 293a 0a20 2020 2072 6574   home():.    ret
-000009d0: 7572 6e20 6622 4865 6c6c 6f2c 2057 6f72  urn f"Hello, Wor
-000009e0: 6c64 2120 7b64 6174 6574 696d 652e 7574  ld! {datetime.ut
-000009f0: 636e 6f77 2829 2e69 736f 666f 726d 6174  cnow().isoformat
-00000a00: 2829 7d22 0a0a 6060 600a 0a23 2320 4765  ()}"..```..## Ge
-00000a10: 7474 696e 6720 7374 6172 7465 6420 7573  tting started us
-00000a20: 696e 6720 7468 6520 434c 4920 e29c a80a  ing the CLI ....
-00000a30: 0a42 6c61 636b 5368 6565 7020 6f66 6665  .BlackSheep offe
-00000a40: 7273 2061 2043 4c49 2074 6f20 626f 6f74  rs a CLI to boot
-00000a50: 7374 7261 7020 6e65 7720 7072 6f6a 6563  strap new projec
-00000a60: 7473 2072 6170 6964 6c79 2e0a 546f 2074  ts rapidly..To t
-00000a70: 7279 2069 742c 2066 6972 7374 2069 6e73  ry it, first ins
-00000a80: 7461 6c6c 2074 6865 2060 626c 6163 6b73  tall the `blacks
-00000a90: 6865 6570 2d63 6c69 6020 7061 636b 6167  heep-cli` packag
-00000aa0: 653a 0a0a 6060 6062 6173 680a 7069 7020  e:..```bash.pip 
-00000ab0: 696e 7374 616c 6c20 626c 6163 6b73 6865  install blackshe
-00000ac0: 6570 2d63 6c69 0a60 6060 0a0a 5468 656e  ep-cli.```..Then
-00000ad0: 2075 7365 2074 6865 2060 626c 6163 6b73   use the `blacks
-00000ae0: 6865 6570 2063 7265 6174 6560 2063 6f6d  heep create` com
-00000af0: 6d61 6e64 2074 6f20 626f 6f74 7374 7261  mand to bootstra
-00000b00: 7020 6120 7072 6f6a 6563 740a 7573 696e  p a project.usin
-00000b10: 6720 6f6e 6520 6f66 2074 6865 2073 7570  g one of the sup
-00000b20: 706f 7274 6564 2074 656d 706c 6174 6573  ported templates
-00000b30: 2e0a 0a21 5b62 6c61 636b 7368 6565 7020  ...![blacksheep 
-00000b40: 6372 6561 7465 2063 6f6d 6d61 6e64 5d28  create command](
-00000b50: 6874 7470 733a 2f2f 6769 7374 2e67 6974  https://gist.git
-00000b60: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000b70: 6f6d 2f52 6f62 6572 746f 5072 6576 6174  om/RobertoPrevat
-00000b80: 6f2f 3338 6130 3539 3862 3531 3561 3266  o/38a0598b515a2f
-00000b90: 3732 3537 6336 3134 3933 3838 3433 6239  7257c614938843b9
-00000ba0: 3962 2f72 6177 2f36 3764 3135 6261 3333  9b/raw/67d15ba33
-00000bb0: 3764 6539 3463 3266 3530 6439 3830 6137  7de94c2f50d980a7
-00000bc0: 6238 3932 3461 3734 3732 3539 3235 342f  b8924a747259254/
-00000bd0: 626c 6163 6b73 6865 6570 2d63 7265 6174  blacksheep-creat
-00000be0: 652d 6465 6d6f 2e67 6966 290a 0a54 6865  e-demo.gif)..The
-00000bf0: 2043 4c49 2069 6e63 6c75 6465 7320 6120   CLI includes a 
-00000c00: 6865 6c70 2c20 616e 6420 7375 7070 6f72  help, and suppor
-00000c10: 7473 2063 7573 746f 6d20 7465 6d70 6c61  ts custom templa
-00000c20: 7465 732c 2075 7369 6e67 2074 6865 0a73  tes, using the.s
-00000c30: 616d 6520 736f 7572 6365 7320 7375 7070  ame sources supp
-00000c40: 6f72 7465 6420 6279 2060 436f 6f6b 6965  orted by `Cookie
-00000c50: 6375 7474 6572 602e 0a0a 2323 2047 6574  cutter`...## Get
-00000c60: 7469 6e67 2073 7461 7274 6564 2077 6974  ting started wit
-00000c70: 6820 7468 6520 646f 6375 6d65 6e74 6174  h the documentat
-00000c80: 696f 6e0a 0a54 6865 2064 6f63 756d 656e  ion..The documen
-00000c90: 7461 7469 6f6e 206f 6666 6572 7320 6765  tation offers ge
-00000ca0: 7474 696e 6720 7374 6172 7465 6420 7475  tting started tu
-00000cb0: 746f 7269 616c 733a 0a2a 205b 4765 7474  torials:.* [Gett
-00000cc0: 696e 6720 7374 6172 7465 643a 0a20 2062  ing started:.  b
-00000cd0: 6173 6963 735d 2868 7474 7073 3a2f 2f77  asics](https://w
-00000ce0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00000cf0: 626c 6163 6b73 6865 6570 2f67 6574 7469  blacksheep/getti
-00000d00: 6e67 2d73 7461 7274 6564 2f29 0a2a 205b  ng-started/).* [
-00000d10: 4765 7474 696e 6720 7374 6172 7465 643a  Getting started:
-00000d20: 2074 6865 204d 5643 2070 726f 6a65 6374   the MVC project
-00000d30: 0a20 2074 656d 706c 6174 655d 2868 7474  .  template](htt
-00000d40: 7073 3a2f 2f77 7777 2e6e 656f 7465 726f  ps://www.neotero
-00000d50: 692e 6465 762f 626c 6163 6b73 6865 6570  i.dev/blacksheep
-00000d60: 2f6d 7663 2d70 726f 6a65 6374 2d74 656d  /mvc-project-tem
-00000d70: 706c 6174 652f 290a 0a54 6865 7365 2070  plate/)..These p
-00000d80: 726f 6a65 6374 2074 656d 706c 6174 6573  roject templates
-00000d90: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00000da0: 7374 6172 7420 6e65 7720 6170 706c 6963  start new applic
-00000db0: 6174 696f 6e73 2066 6173 7465 723a 0a0a  ations faster:..
-00000dc0: 2a20 5b4d 5643 2070 726f 6a65 6374 0a20  * [MVC project. 
-00000dd0: 2074 656d 706c 6174 655d 2868 7474 7073   template](https
-00000de0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e65  ://github.com/Ne
-00000df0: 6f74 6572 6f69 2f42 6c61 636b 5368 6565  oteroi/BlackShee
-00000e00: 704d 5643 290a 2a20 5b45 6d70 7479 2070  pMVC).* [Empty p
-00000e10: 726f 6a65 6374 0a20 2074 656d 706c 6174  roject.  templat
-00000e20: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-00000e30: 622e 636f 6d2f 4e65 6f74 6572 6f69 2f42  b.com/Neoteroi/B
-00000e40: 6c61 636b 5368 6565 7045 6d70 7479 5072  lackSheepEmptyPr
-00000e50: 6f6a 6563 7429 0a0a 2323 2052 6571 7569  oject)..## Requi
-00000e60: 7265 6d65 6e74 730a 0a5b 5079 7468 6f6e  rements..[Python
-00000e70: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
-00000e80: 7468 6f6e 2e6f 7267 293a 2061 6e79 2076  thon.org): any v
-00000e90: 6572 7369 6f6e 206c 6973 7465 6420 696e  ersion listed in
-00000ea0: 2074 6865 2070 726f 6a65 6374 2773 0a63   the project's.c
-00000eb0: 6c61 7373 6966 6965 7273 2e20 5468 6520  lassifiers. The 
-00000ec0: 6375 7272 656e 7420 6c69 7374 2069 733a  current list is:
-00000ed0: 0a0a 5b21 5b76 6572 7369 6f6e 735d 2868  ..[![versions](h
-00000ee0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000ef0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-00000f00: 7369 6f6e 732f 626c 6163 6b73 6865 6570  sions/blacksheep
-00000f10: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000f20: 6974 6875 622e 636f 6d2f 726f 6265 7274  ithub.com/robert
-00000f30: 6f70 7265 7661 746f 2f62 6c61 636b 7368  oprevato/blacksh
-00000f40: 6565 7029 0a0a 0a42 6c61 636b 5368 6565  eep)...BlackShee
-00000f50: 7020 6265 6c6f 6e67 7320 746f 2074 6865  p belongs to the
-00000f60: 2063 6174 6567 6f72 7920 6f66 0a5b 4153   category of.[AS
-00000f70: 4749 5d28 6874 7470 733a 2f2f 6173 6769  GI](https://asgi
-00000f80: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000f90: 656e 2f6c 6174 6573 742f 2920 7765 6220  en/latest/) web 
-00000fa0: 6672 616d 6577 6f72 6b73 2c20 736f 2069  frameworks, so i
-00000fb0: 7420 7265 7175 6972 6573 0a61 6e20 4153  t requires.an AS
-00000fc0: 4749 2048 5454 5020 7365 7276 6572 2074  GI HTTP server t
-00000fd0: 6f20 7275 6e2c 2073 7563 6820 6173 205b  o run, such as [
-00000fe0: 7576 6963 6f72 6e5d 2868 7474 703a 2f2f  uvicorn](http://
-00000ff0: 7777 772e 7576 6963 6f72 6e2e 6f72 672f  www.uvicorn.org/
-00001000: 292c 206f 720a 5b68 7970 6572 636f 726e  ), or.[hypercorn
-00001010: 5d28 6874 7470 733a 2f2f 7067 6a6f 6e65  ](https://pgjone
-00001020: 732e 6769 746c 6162 2e69 6f2f 6879 7065  s.gitlab.io/hype
-00001030: 7263 6f72 6e2f 292e 2046 6f72 2065 7861  rcorn/). For exa
-00001040: 6d70 6c65 2c20 746f 2075 7365 2069 7420  mple, to use it 
-00001050: 7769 7468 0a75 7669 636f 726e 3a0a 0a60  with.uvicorn:..`
-00001060: 6060 6261 7368 0a24 2070 6970 2069 6e73  ``bash.$ pip ins
-00001070: 7461 6c6c 2075 7669 636f 726e 0a60 6060  tall uvicorn.```
-00001080: 0a0a 546f 2072 756e 2061 6e20 6170 706c  ..To run an appl
-00001090: 6963 6174 696f 6e20 6c69 6b65 2069 6e20  ication like in 
-000010a0: 7468 6520 6578 616d 706c 6520 6162 6f76  the example abov
-000010b0: 652c 2075 7365 2074 6865 206d 6574 686f  e, use the metho
-000010c0: 6473 2070 726f 7669 6465 6420 6279 0a74  ds provided by.t
-000010d0: 6865 2041 5347 4920 4854 5450 2053 6572  he ASGI HTTP Ser
-000010e0: 7665 723a 0a0a 6060 6062 6173 680a 2320  ver:..```bash.# 
-000010f0: 6966 2074 6865 2042 6c61 636b 5368 6565  if the BlackShee
-00001100: 7020 6170 7020 6973 2064 6566 696e 6564  p app is defined
-00001110: 2069 6e20 6120 6669 6c65 2060 7365 7276   in a file `serv
-00001120: 6572 2e70 7960 0a0a 2420 7576 6963 6f72  er.py`..$ uvicor
-00001130: 6e20 7365 7276 6572 3a61 7070 0a60 6060  n server:app.```
-00001140: 0a0a 546f 2072 756e 2066 6f72 2070 726f  ..To run for pro
-00001150: 6475 6374 696f 6e2c 2072 6566 6572 2074  duction, refer t
-00001160: 6f20 7468 6520 646f 6375 6d65 6e74 6174  o the documentat
-00001170: 696f 6e20 6f66 2074 6865 2063 686f 7365  ion of the chose
-00001180: 6e20 4153 4749 2073 6572 7665 720a 2869  n ASGI server.(i
-00001190: 2e65 2e20 666f 7220 5b75 7669 636f 726e  .e. for [uvicorn
-000011a0: 5d28 6874 7470 733a 2f2f 7777 772e 7576  ](https://www.uv
-000011b0: 6963 6f72 6e2e 6f72 672f 2372 756e 6e69  icorn.org/#runni
-000011c0: 6e67 2d77 6974 682d 6775 6e69 636f 726e  ng-with-gunicorn
-000011d0: 2929 2e0a 0a23 2320 4175 746f 6d61 7469  ))...## Automati
-000011e0: 6320 6269 6e64 696e 6773 2061 6e64 2064  c bindings and d
-000011f0: 6570 656e 6465 6e63 7920 696e 6a65 6374  ependency inject
-00001200: 696f 6e0a 426c 6163 6b53 6865 6570 2073  ion.BlackSheep s
-00001210: 7570 706f 7274 7320 6175 746f 6d61 7469  upports automati
-00001220: 6320 6269 6e64 696e 6720 6f66 2076 616c  c binding of val
-00001230: 7565 7320 666f 7220 7265 7175 6573 7420  ues for request 
-00001240: 6861 6e64 6c65 7273 2c20 6279 2074 7970  handlers, by typ
-00001250: 650a 616e 6e6f 7461 7469 6f6e 206f 7220  e.annotation or 
-00001260: 6279 2063 6f6e 7665 6e74 696f 6e73 2e20  by conventions. 
-00001270: 5365 6520 5b6d 6f72 650a 6865 7265 5d28  See [more.here](
-00001280: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
-00001290: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
-000012a0: 6565 702f 7265 7175 6573 7473 2f29 2e0a  eep/requests/)..
-000012b0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-000012c0: 6461 7461 636c 6173 7365 7320 696d 706f  dataclasses impo
-000012d0: 7274 2064 6174 6163 6c61 7373 0a0a 6672  rt dataclass..fr
-000012e0: 6f6d 2062 6c61 636b 7368 6565 7020 696d  om blacksheep im
-000012f0: 706f 7274 2041 7070 6c69 6361 7469 6f6e  port Application
-00001300: 2c20 4672 6f6d 4a53 4f4e 2c20 4672 6f6d  , FromJSON, From
-00001310: 5175 6572 790a 0a0a 6170 7020 3d20 4170  Query...app = Ap
-00001320: 706c 6963 6174 696f 6e28 290a 0a0a 4064  plication()...@d
-00001330: 6174 6163 6c61 7373 0a63 6c61 7373 2043  ataclass.class C
-00001340: 7265 6174 6543 6174 496e 7075 743a 0a20  reateCatInput:. 
-00001350: 2020 206e 616d 653a 2073 7472 0a0a 0a40     name: str...@
-00001360: 6170 702e 726f 7574 6572 2e70 6f73 7428  app.router.post(
-00001370: 222f 6170 692f 6361 7473 2229 0a61 7379  "/api/cats").asy
-00001380: 6e63 2064 6566 2065 7861 6d70 6c65 2864  nc def example(d
-00001390: 6174 613a 2046 726f 6d4a 534f 4e5b 4372  ata: FromJSON[Cr
-000013a0: 6561 7465 4361 7449 6e70 7574 5d29 3a0a  eateCatInput]):.
-000013b0: 2020 2020 2320 696e 2074 6869 7320 6578      # in this ex
-000013c0: 616d 706c 652c 2064 6174 6120 6973 2062  ample, data is b
-000013d0: 6f75 6e64 2061 7574 6f6d 6174 6963 616c  ound automatical
-000013e0: 6c79 2072 6561 6469 6e67 2074 6865 204a  ly reading the J
-000013f0: 534f 4e0a 2020 2020 2320 7061 796c 6f61  SON.    # payloa
-00001400: 6420 616e 6420 6372 6561 7469 6e67 2061  d and creating a
-00001410: 6e20 696e 7374 616e 6365 206f 6620 6043  n instance of `C
-00001420: 7265 6174 6543 6174 496e 7075 7460 0a20  reateCatInput`. 
-00001430: 2020 202e 2e2e 0a0a 0a40 6170 702e 726f     ......@app.ro
-00001440: 7574 6572 2e67 6574 2822 2f3a 6375 6c74  uter.get("/:cult
-00001450: 7572 655f 636f 6465 2f3a 6172 6561 2229  ure_code/:area")
-00001460: 0a61 7379 6e63 2064 6566 2068 6f6d 6528  .async def home(
-00001470: 6375 6c74 7572 655f 636f 6465 2c20 6172  culture_code, ar
-00001480: 6561 293a 0a20 2020 2023 2069 6e20 7468  ea):.    # in th
-00001490: 6973 2065 7861 6d70 6c65 2c20 626f 7468  is example, both
-000014a0: 2070 6172 616d 6574 6572 7320 6172 6520   parameters are 
-000014b0: 6f62 7461 696e 6564 2066 726f 6d20 726f  obtained from ro
-000014c0: 7574 6573 2077 6974 680a 2020 2020 2320  utes with.    # 
-000014d0: 6d61 7463 6869 6e67 206e 616d 6573 0a20  matching names. 
-000014e0: 2020 2072 6574 7572 6e20 6622 5265 7175     return f"Requ
-000014f0: 6573 7420 666f 723a 207b 6375 6c74 7572  est for: {cultur
-00001500: 655f 636f 6465 7d20 7b61 7265 617d 220a  e_code} {area}".
-00001510: 0a0a 4061 7070 2e72 6f75 7465 722e 6765  ..@app.router.ge
-00001520: 7428 222f 6170 692f 7072 6f64 7563 7473  t("/api/products
-00001530: 2229 0a64 6566 2067 6574 5f70 726f 6475  ").def get_produ
-00001540: 6374 7328 0a20 2020 2070 6167 653a 2069  cts(.    page: i
-00001550: 6e74 203d 2031 2c0a 2020 2020 7369 7a65  nt = 1,.    size
-00001560: 3a20 696e 7420 3d20 3330 2c0a 2020 2020  : int = 30,.    
-00001570: 7365 6172 6368 3a20 7374 7220 3d20 2222  search: str = ""
-00001580: 2c0a 293a 0a20 2020 2023 2074 6869 7320  ,.):.    # this 
-00001590: 6578 616d 706c 6520 696c 6c75 7374 7261  example illustra
-000015a0: 7465 7320 7375 7070 6f72 7420 666f 7220  tes support for 
-000015b0: 696d 706c 6963 6974 2071 7565 7279 2070  implicit query p
-000015c0: 6172 616d 6574 6572 7320 7769 7468 0a20  arameters with. 
-000015d0: 2020 2023 2064 6566 6175 6c74 2076 616c     # default val
-000015e0: 7565 730a 2020 2020 2320 7369 6e63 6520  ues.    # since 
-000015f0: 7468 6520 736f 7572 6365 206f 6620 7061  the source of pa
-00001600: 6765 2c20 7369 7a65 2c20 616e 6420 7365  ge, size, and se
-00001610: 6172 6368 2069 7320 6e6f 7420 7370 6563  arch is not spec
-00001620: 6966 6965 6420 616e 6420 6e6f 0a20 2020  ified and no.   
-00001630: 2023 2072 6f75 7465 2070 6172 616d 6574   # route paramet
-00001640: 6572 206d 6174 6368 6573 2074 6865 6972  er matches their
-00001650: 206e 616d 652c 2074 6865 7920 6172 6520   name, they are 
-00001660: 6f62 7461 696e 6564 2066 726f 6d20 7175  obtained from qu
-00001670: 6572 7920 7374 7269 6e67 0a20 2020 202e  ery string.    .
-00001680: 2e2e 0a0a 0a40 6170 702e 726f 7574 6572  .....@app.router
-00001690: 2e67 6574 2822 2f61 7069 2f70 726f 6475  .get("/api/produ
-000016a0: 6374 7332 2229 0a64 6566 2067 6574 5f70  cts2").def get_p
-000016b0: 726f 6475 6374 7332 280a 2020 2020 7061  roducts2(.    pa
-000016c0: 6765 3a20 4672 6f6d 5175 6572 795b 696e  ge: FromQuery[in
-000016d0: 745d 203d 2046 726f 6d51 7565 7279 2831  t] = FromQuery(1
-000016e0: 292c 0a20 2020 2073 697a 653a 2046 726f  ),.    size: Fro
-000016f0: 6d51 7565 7279 5b69 6e74 5d20 3d20 4672  mQuery[int] = Fr
-00001700: 6f6d 5175 6572 7928 3330 292c 0a20 2020  omQuery(30),.   
-00001710: 2073 6561 7263 683a 2046 726f 6d51 7565   search: FromQue
-00001720: 7279 5b73 7472 5d20 3d20 4672 6f6d 5175  ry[str] = FromQu
-00001730: 6572 7928 2222 292c 0a29 3a0a 2020 2020  ery(""),.):.    
-00001740: 2320 7468 6973 2065 7861 6d70 6c65 2069  # this example i
-00001750: 6c6c 7573 7472 6174 6573 2073 7570 706f  llustrates suppo
-00001760: 7274 2066 6f72 2065 7870 6c69 6369 7420  rt for explicit 
-00001770: 7175 6572 7920 7061 7261 6d65 7465 7273  query parameters
-00001780: 2077 6974 680a 2020 2020 2320 6465 6661   with.    # defa
-00001790: 756c 7420 7661 6c75 6573 0a20 2020 2023  ult values.    #
-000017a0: 2069 6e20 7468 6973 2063 6173 652c 2070   in this case, p
-000017b0: 6172 616d 6574 6572 7320 6172 6520 6578  arameters are ex
-000017c0: 706c 6963 6974 6c79 2072 6561 6420 6672  plicitly read fr
-000017d0: 6f6d 2071 7565 7279 2073 7472 696e 670a  om query string.
-000017e0: 2020 2020 2e2e 2e0a 0a60 6060 0a0a 4974      .....```..It
-000017f0: 2061 6c73 6f20 7375 7070 6f72 7473 205b   also supports [
-00001800: 6465 7065 6e64 656e 6379 0a69 6e6a 6563  dependency.injec
-00001810: 7469 6f6e 5d28 6874 7470 733a 2f2f 7777  tion](https://ww
-00001820: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
-00001830: 6c61 636b 7368 6565 702f 6465 7065 6e64  lacksheep/depend
-00001840: 656e 6379 2d69 6e6a 6563 7469 6f6e 2f29  ency-injection/)
-00001850: 2c20 610a 6665 6174 7572 6520 7468 6174  , a.feature that
-00001860: 2070 726f 7669 6465 7320 6120 636f 6e73   provides a cons
-00001870: 6973 7465 6e74 2061 6e64 2063 6c65 616e  istent and clean
-00001880: 2077 6179 2074 6f20 7573 6520 6465 7065   way to use depe
-00001890: 6e64 656e 6369 6573 2069 6e20 7265 7175  ndencies in requ
-000018a0: 6573 740a 6861 6e64 6c65 7273 2e0a 0a23  est.handlers...#
-000018b0: 2320 4765 6e65 7261 7469 6f6e 206f 6620  # Generation of 
-000018c0: 4f70 656e 4150 4920 446f 6375 6d65 6e74  OpenAPI Document
-000018d0: 6174 696f 6e0a 5b47 656e 6572 6174 696f  ation.[Generatio
-000018e0: 6e20 6f66 204f 7065 6e41 5049 2044 6f63  n of OpenAPI Doc
-000018f0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
-00001900: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
-00001910: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
-00001920: 6f70 656e 6170 692f 292e 0a0a 2323 2053  openapi/)...## S
-00001930: 7472 6174 6567 6965 7320 746f 2068 616e  trategies to han
-00001940: 646c 6520 6175 7468 656e 7469 6361 7469  dle authenticati
-00001950: 6f6e 2061 6e64 2061 7574 686f 7269 7a61  on and authoriza
-00001960: 7469 6f6e 0a42 6c61 636b 5368 6565 7020  tion.BlackSheep 
-00001970: 696d 706c 656d 656e 7473 2073 7472 6174  implements strat
-00001980: 6567 6965 7320 746f 2068 616e 646c 6520  egies to handle 
-00001990: 6175 7468 656e 7469 6361 7469 6f6e 2061  authentication a
-000019a0: 6e64 2061 7574 686f 7269 7a61 7469 6f6e  nd authorization
-000019b0: 2e0a 5468 6573 6520 6665 6174 7572 6573  ..These features
-000019c0: 2061 7265 2064 6f63 756d 656e 7465 6420   are documented 
-000019d0: 6865 7265 3a0a 0a2a 205b 4175 7468 656e  here:..* [Authen
-000019e0: 7469 6361 7469 6f6e 5d28 6874 7470 733a  tication](https:
-000019f0: 2f2f 7777 772e 6e65 6f74 6572 6f69 2e64  //www.neoteroi.d
-00001a00: 6576 2f62 6c61 636b 7368 6565 702f 6175  ev/blacksheep/au
-00001a10: 7468 656e 7469 6361 7469 6f6e 2f29 0a2a  thentication/).*
-00001a20: 205b 4175 7468 6f72 697a 6174 696f 6e5d   [Authorization]
-00001a30: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
-00001a40: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
-00001a50: 6865 6570 2f61 7574 686f 7269 7a61 7469  heep/authorizati
-00001a60: 6f6e 2f29 0a0a 6060 6070 7974 686f 6e0a  on/)..```python.
-00001a70: 6170 702e 7573 655f 6175 7468 656e 7469  app.use_authenti
-00001a80: 6361 7469 6f6e 2829 5c0a 2020 2020 2e61  cation()\.    .a
-00001a90: 6464 2845 7861 6d70 6c65 4175 7468 656e  dd(ExampleAuthen
-00001aa0: 7469 6361 7469 6f6e 4861 6e64 6c65 7228  ticationHandler(
-00001ab0: 2929 0a0a 0a61 7070 2e75 7365 5f61 7574  ))...app.use_aut
-00001ac0: 686f 7269 7a61 7469 6f6e 2829 5c0a 2020  horization()\.  
-00001ad0: 2020 2e61 6464 2841 646d 696e 7350 6f6c    .add(AdminsPol
-00001ae0: 6963 7928 2929 0a0a 0a40 6175 7468 2822  icy())...@auth("
-00001af0: 6164 6d69 6e22 290a 4061 7070 2e72 6f75  admin").@app.rou
-00001b00: 7465 722e 6765 7428 222f 2229 0a61 7379  ter.get("/").asy
-00001b10: 6e63 2064 6566 206f 6e6c 795f 666f 725f  nc def only_for_
-00001b20: 6164 6d69 6e73 2829 3a0a 2020 2020 2e2e  admins():.    ..
-00001b30: 2e0a 0a0a 4061 7574 6828 290a 4061 7070  ....@auth().@app
-00001b40: 2e72 6f75 7465 722e 6765 7428 222f 2229  .router.get("/")
-00001b50: 0a61 7379 6e63 2064 6566 206f 6e6c 795f  .async def only_
-00001b60: 666f 725f 6175 7468 656e 7469 6361 7465  for_authenticate
-00001b70: 645f 7573 6572 7328 293a 0a20 2020 202e  d_users():.    .
-00001b80: 2e2e 0a60 6060 0a0a 5369 6e63 6520 7665  ...```..Since ve
-00001b90: 7273 696f 6e20 6031 2e32 2e31 602c 2042  rsion `1.2.1`, B
-00001ba0: 6c61 636b 5368 6565 7020 696d 706c 656d  lackSheep implem
-00001bb0: 656e 7473 3a0a 0a2a 205b 4275 696c 742d  ents:..* [Built-
-00001bc0: 696e 2073 7570 706f 7274 2066 6f72 204f  in support for O
-00001bd0: 7065 6e49 4420 436f 6e6e 6563 7420 6175  penID Connect au
-00001be0: 7468 656e 7469 6361 7469 6f6e 5d28 6874  thentication](ht
-00001bf0: 7470 733a 2f2f 7777 772e 6e65 6f74 6572  tps://www.neoter
-00001c00: 6f69 2e64 6576 2f62 6c61 636b 7368 6565  oi.dev/blackshee
-00001c10: 702f 6175 7468 656e 7469 6361 7469 6f6e  p/authentication
-00001c20: 2f23 6f69 6463 290a 2a20 5b42 7569 6c74  /#oidc).* [Built
-00001c30: 2d69 6e20 7375 7070 6f72 7420 666f 7220  -in support for 
-00001c40: 4a57 5420 4265 6172 6572 2061 7574 6865  JWT Bearer authe
-00001c50: 6e74 6963 6174 696f 6e5d 2868 7474 7073  ntication](https
-00001c60: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-00001c70: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
-00001c80: 7574 6865 6e74 6963 6174 696f 6e2f 236a  uthentication/#j
-00001c90: 7774 2d62 6561 7265 7229 0a0a 4d65 616e  wt-bearer)..Mean
-00001ca0: 696e 6720 7468 6174 2069 7420 6973 2065  ing that it is e
-00001cb0: 6173 7920 746f 2069 6e74 6567 7261 7465  asy to integrate
-00001cc0: 2077 6974 6820 7365 7276 6963 6573 2073   with services s
-00001cd0: 7563 6820 6173 3a0a 2a20 5b41 7574 6830  uch as:.* [Auth0
-00001ce0: 5d28 6874 7470 733a 2f2f 6175 7468 302e  ](https://auth0.
-00001cf0: 636f 6d29 0a2a 205b 417a 7572 6520 4163  com).* [Azure Ac
-00001d00: 7469 7665 2044 6972 6563 746f 7279 5d28  tive Directory](
-00001d10: 6874 7470 733a 2f2f 617a 7572 652e 6d69  https://azure.mi
-00001d20: 6372 6f73 6f66 742e 636f 6d2f 656e 2d75  crosoft.com/en-u
-00001d30: 732f 7365 7276 6963 6573 2f61 6374 6976  s/services/activ
-00001d40: 652d 6469 7265 6374 6f72 792f 290a 2a20  e-directory/).* 
-00001d50: 5b41 7a75 7265 2041 6374 6976 6520 4469  [Azure Active Di
-00001d60: 7265 6374 6f72 7920 4232 435d 2868 7474  rectory B2C](htt
-00001d70: 7073 3a2f 2f64 6f63 732e 6d69 6372 6f73  ps://docs.micros
-00001d80: 6f66 742e 636f 6d2f 656e 2d75 732f 617a  oft.com/en-us/az
-00001d90: 7572 652f 6163 7469 7665 2d64 6972 6563  ure/active-direc
-00001da0: 746f 7279 2d62 3263 2f6f 7665 7276 6965  tory-b2c/overvie
-00001db0: 7729 0a2a 205b 4f6b 7461 5d28 6874 7470  w).* [Okta](http
-00001dc0: 733a 2f2f 7777 772e 6f6b 7461 2e63 6f6d  s://www.okta.com
-00001dd0: 290a 0a52 6566 6572 2074 6f20 7468 6520  )..Refer to the 
-00001de0: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00001df0: 7220 6d6f 7265 2064 6574 6169 6c73 2061  r more details a
-00001e00: 6e64 2065 7861 6d70 6c65 732e 0a0a 2323  nd examples...##
-00001e10: 2057 6562 2066 7261 6d65 776f 726b 2066   Web framework f
-00001e20: 6561 7475 7265 730a 0a2a 205b 4153 4749  eatures..* [ASGI
-00001e30: 2063 6f6d 7061 7469 6269 6c69 7479 5d28   compatibility](
-00001e40: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
-00001e50: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
-00001e60: 6565 702f 6173 6769 2f29 0a2a 205b 526f  eep/asgi/).* [Ro
-00001e70: 7574 696e 675d 2868 7474 7073 3a2f 2f77  uting](https://w
-00001e80: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00001e90: 626c 6163 6b73 6865 6570 2f72 6f75 7469  blacksheep/routi
-00001ea0: 6e67 2f29 0a2a 2052 6571 7565 7374 2068  ng/).* Request h
-00001eb0: 616e 646c 6572 7320 6361 6e20 6265 205b  andlers can be [
-00001ec0: 6465 6669 6e65 6420 6173 0a20 2066 756e  defined as.  fun
-00001ed0: 6374 696f 6e73 5d28 6874 7470 733a 2f2f  ctions](https://
-00001ee0: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-00001ef0: 2f62 6c61 636b 7368 6565 702f 7265 7175  /blacksheep/requ
-00001f00: 6573 742d 6861 6e64 6c65 7273 2f29 2c20  est-handlers/), 
-00001f10: 6f72 205b 636c 6173 730a 2020 6d65 7468  or [class.  meth
-00001f20: 6f64 735d 2868 7474 7073 3a2f 2f77 7777  ods](https://www
-00001f30: 2e6e 656f 7465 726f 692e 6465 762f 626c  .neoteroi.dev/bl
-00001f40: 6163 6b73 6865 6570 2f63 6f6e 7472 6f6c  acksheep/control
-00001f50: 6c65 7273 2f29 0a2a 205b 4d69 6464 6c65  lers/).* [Middle
-00001f60: 7761 7265 735d 2868 7474 7073 3a2f 2f77  wares](https://w
-00001f70: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00001f80: 626c 6163 6b73 6865 6570 2f6d 6964 646c  blacksheep/middl
-00001f90: 6577 6172 6573 2f29 0a2a 205b 5765 6253  ewares/).* [WebS
-00001fa0: 6f63 6b65 745d 2868 7474 7073 3a2f 2f77  ocket](https://w
-00001fb0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00001fc0: 626c 6163 6b73 6865 6570 2f77 6562 736f  blacksheep/webso
-00001fd0: 636b 6574 2f29 0a2a 205b 4275 696c 742d  cket/).* [Built-
-00001fe0: 696e 2073 7570 706f 7274 2066 6f72 2064  in support for d
-00001ff0: 6570 656e 6465 6e63 790a 2020 696e 6a65  ependency.  inje
-00002000: 6374 696f 6e5d 2868 7474 7073 3a2f 2f77  ction](https://w
-00002010: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
-00002020: 626c 6163 6b73 6865 6570 2f64 6570 656e  blacksheep/depen
-00002030: 6465 6e63 792d 696e 6a65 6374 696f 6e2f  dency-injection/
-00002040: 290a 2a20 5b53 7570 706f 7274 2066 6f72  ).* [Support for
-00002050: 2061 7574 6f6d 6174 6963 2062 696e 6469   automatic bindi
-00002060: 6e67 206f 6620 726f 7574 6520 616e 6420  ng of route and 
-00002070: 7175 6572 7920 7061 7261 6d65 7465 7273  query parameters
-00002080: 2074 6f20 7265 7175 6573 740a 2020 6861   to request.  ha
-00002090: 6e64 6c65 7273 206d 6574 686f 6473 0a20  ndlers methods. 
-000020a0: 2063 616c 6c73 5d28 6874 7470 733a 2f2f   calls](https://
-000020b0: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-000020c0: 2f62 6c61 636b 7368 6565 702f 6765 7474  /blacksheep/gett
-000020d0: 696e 672d 7374 6172 7465 642f 2368 616e  ing-started/#han
-000020e0: 646c 696e 672d 726f 7574 652d 7061 7261  dling-route-para
-000020f0: 6d65 7465 7273 290a 2a20 5b53 7472 6174  meters).* [Strat
-00002100: 6567 7920 746f 2068 616e 646c 650a 2020  egy to handle.  
-00002110: 6578 6365 7074 696f 6e73 5d28 6874 7470  exceptions](http
-00002120: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
-00002130: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
-00002140: 6170 706c 6963 6174 696f 6e2f 2363 6f6e  application/#con
-00002150: 6669 6775 7269 6e67 2d65 7863 6570 7469  figuring-excepti
-00002160: 6f6e 732d 6861 6e64 6c65 7273 290a 2a20  ons-handlers).* 
-00002170: 5b53 7472 6174 6567 7920 746f 2068 616e  [Strategy to han
-00002180: 646c 6520 6175 7468 656e 7469 6361 7469  dle authenticati
-00002190: 6f6e 2061 6e64 0a20 2061 7574 686f 7269  on and.  authori
-000021a0: 7a61 7469 6f6e 5d28 6874 7470 733a 2f2f  zation](https://
-000021b0: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-000021c0: 2f62 6c61 636b 7368 6565 702f 6175 7468  /blacksheep/auth
-000021d0: 656e 7469 6361 7469 6f6e 2f29 0a2a 205b  entication/).* [
-000021e0: 4275 696c 742d 696e 2073 7570 706f 7274  Built-in support
-000021f0: 2066 6f72 204f 7065 6e49 4420 436f 6e6e   for OpenID Conn
-00002200: 6563 7420 6175 7468 656e 7469 6361 7469  ect authenticati
-00002210: 6f6e 2075 7369 6e67 204f 4944 430a 2020  on using OIDC.  
-00002220: 6469 7363 6f76 6572 795d 2868 7474 7073  discovery](https
-00002230: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-00002240: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
-00002250: 7574 6865 6e74 6963 6174 696f 6e2f 236f  uthentication/#o
-00002260: 6964 6329 0a2a 205b 4275 696c 742d 696e  idc).* [Built-in
-00002270: 2073 7570 706f 7274 2066 6f72 204a 5754   support for JWT
-00002280: 2042 6561 7265 7220 6175 7468 656e 7469   Bearer authenti
-00002290: 6361 7469 6f6e 2075 7369 6e67 204f 4944  cation using OID
-000022a0: 4320 6469 7363 6f76 6572 7920 616e 640a  C discovery and.
-000022b0: 2020 6f74 6865 7220 736f 7572 6365 7320    other sources 
-000022c0: 6f66 0a20 204a 574b 535d 2868 7474 7073  of.  JWKS](https
-000022d0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-000022e0: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
-000022f0: 7574 6865 6e74 6963 6174 696f 6e2f 236a  uthentication/#j
-00002300: 7774 2d62 6561 7265 7229 0a2a 205b 4861  wt-bearer).* [Ha
-00002310: 6e64 6c65 7273 0a20 206e 6f72 6d61 6c69  ndlers.  normali
-00002320: 7a61 7469 6f6e 5d28 6874 7470 733a 2f2f  zation](https://
-00002330: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
-00002340: 2f62 6c61 636b 7368 6565 702f 7265 7175  /blacksheep/requ
-00002350: 6573 742d 6861 6e64 6c65 7273 2f29 0a2a  est-handlers/).*
-00002360: 205b 5365 7276 696e 6720 7374 6174 6963   [Serving static
-00002370: 0a20 2066 696c 6573 5d28 6874 7470 733a  .  files](https:
-00002380: 2f2f 7777 772e 6e65 6f74 6572 6f69 2e64  //www.neoteroi.d
-00002390: 6576 2f62 6c61 636b 7368 6565 702f 7374  ev/blacksheep/st
-000023a0: 6174 6963 2d66 696c 6573 2f29 0a2a 205b  atic-files/).* [
-000023b0: 496e 7465 6772 6174 696f 6e20 7769 7468  Integration with
-000023c0: 0a20 204a 696e 6a61 325d 2868 7474 7073  .  Jinja2](https
-000023d0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
-000023e0: 6465 762f 626c 6163 6b73 6865 6570 2f74  dev/blacksheep/t
-000023f0: 656d 706c 6174 696e 672f 290a 2a20 5b53  emplating/).* [S
-00002400: 7570 706f 7274 2066 6f72 2073 6572 7669  upport for servi
-00002410: 6e67 2053 5041 7320 7468 6174 2075 7365  ng SPAs that use
-00002420: 2048 544d 4c35 2048 6973 746f 7279 2041   HTML5 History A
-00002430: 5049 2066 6f72 2063 6c69 656e 7420 7369  PI for client si
-00002440: 6465 0a20 2072 6f75 7469 6e67 5d28 6874  de.  routing](ht
-00002450: 7470 733a 2f2f 7777 772e 6e65 6f74 6572  tps://www.neoter
-00002460: 6f69 2e64 6576 2f62 6c61 636b 7368 6565  oi.dev/blackshee
-00002470: 702f 7374 6174 6963 2d66 696c 6573 2f23  p/static-files/#
-00002480: 686f 772d 746f 2d73 6572 7665 2d73 7061  how-to-serve-spa
-00002490: 732d 7468 6174 2d75 7365 2d68 746d 6c35  s-that-use-html5
-000024a0: 2d68 6973 746f 7279 2d61 7069 290a 2a20  -history-api).* 
-000024b0: 5b53 7570 706f 7274 2066 6f72 2061 7574  [Support for aut
-000024c0: 6f6d 6174 6963 2067 656e 6572 6174 696f  omatic generatio
-000024d0: 6e20 6f66 204f 7065 6e41 5049 0a20 2044  n of OpenAPI.  D
-000024e0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000024f0: 7470 733a 2f2f 7777 772e 6e65 6f74 6572  tps://www.neoter
-00002500: 6f69 2e64 6576 2f62 6c61 636b 7368 6565  oi.dev/blackshee
-00002510: 702f 6f70 656e 6170 692f 290a 2a20 5b53  p/openapi/).* [S
-00002520: 7472 6174 6567 7920 746f 2068 616e 646c  trategy to handl
-00002530: 6520 434f 5253 2073 6574 7469 6e67 735d  e CORS settings]
-00002540: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
-00002550: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
-00002560: 6865 6570 2f63 6f72 732f 290a 2a20 5b53  heep/cors/).* [S
-00002570: 6573 7369 6f6e 735d 2868 7474 7073 3a2f  essions](https:/
-00002580: 2f77 7777 2e6e 656f 7465 726f 692e 6465  /www.neoteroi.de
-00002590: 762f 626c 6163 6b73 6865 6570 2f73 6573  v/blacksheep/ses
-000025a0: 7369 6f6e 732f 290a 2a20 5375 7070 6f72  sions/).* Suppor
-000025b0: 7420 666f 7220 6175 746f 6d61 7469 6320  t for automatic 
-000025c0: 6269 6e64 696e 6720 6f66 2060 6461 7461  binding of `data
-000025d0: 636c 6173 7365 7360 2061 6e64 0a20 205b  classes` and.  [
-000025e0: 6070 7964 616e 7469 6360 5d28 6874 7470  `pydantic`](http
-000025f0: 733a 2f2f 7079 6461 6e74 6963 2d64 6f63  s://pydantic-doc
-00002600: 732e 6865 6c70 6d61 6e75 616c 2e69 6f29  s.helpmanual.io)
-00002610: 206d 6f64 656c 7320 746f 2068 616e 646c   models to handl
-00002620: 6520 7468 650a 2020 7265 7175 6573 7420  e the.  request 
-00002630: 626f 6479 2070 6179 6c6f 6164 2065 7870  body payload exp
-00002640: 6563 7465 6420 6279 2072 6571 7565 7374  ected by request
-00002650: 2068 616e 646c 6572 730a 2a20 5b60 5465   handlers.* [`Te
-00002660: 7374 436c 6965 6e74 6020 636c 6173 7320  stClient` class 
-00002670: 746f 2073 696d 706c 6966 7920 7465 7374  to simplify test
-00002680: 696e 6720 6f66 2061 7070 6c69 6361 7469  ing of applicati
-00002690: 6f6e 735d 2868 7474 7073 3a2f 2f77 7777  ons](https://www
-000026a0: 2e6e 656f 7465 726f 692e 6465 762f 626c  .neoteroi.dev/bl
-000026b0: 6163 6b73 6865 6570 2f74 6573 7469 6e67  acksheep/testing
-000026c0: 2f29 0a2a 205b 416e 7469 2046 6f72 6765  /).* [Anti Forge
-000026d0: 7279 2076 616c 6964 6174 696f 6e5d 2868  ry validation](h
-000026e0: 7474 7073 3a2f 2f77 7777 2e6e 656f 7465  ttps://www.neote
-000026f0: 726f 692e 6465 762f 626c 6163 6b73 6865  roi.dev/blackshe
-00002700: 6570 2f61 6e74 692d 7265 7175 6573 742d  ep/anti-request-
-00002710: 666f 7267 6572 7929 2074 6f20 7072 6f74  forgery) to prot
-00002720: 6563 7420 6167 6169 6e73 7420 4372 6f73  ect against Cros
-00002730: 732d 5369 7465 2052 6571 7565 7374 2046  s-Site Request F
-00002740: 6f72 6765 7279 2028 5853 5246 2f43 5352  orgery (XSRF/CSR
-00002750: 4629 2061 7474 6163 6b73 0a0a 2323 2043  F) attacks..## C
-00002760: 6c69 656e 7420 6665 6174 7572 6573 0a0a  lient features..
-00002770: 426c 6163 6b53 6865 6570 2069 6e63 6c75  BlackSheep inclu
-00002780: 6465 7320 616e 2048 5454 5020 436c 6965  des an HTTP Clie
-00002790: 6e74 2e0a 0a2a 2a45 7861 6d70 6c65 3a2a  nt...**Example:*
-000027a0: 2a0a 6060 6070 7974 686f 6e0a 696d 706f  *.```python.impo
-000027b0: 7274 2061 7379 6e63 696f 0a0a 6672 6f6d  rt asyncio..from
-000027c0: 2062 6c61 636b 7368 6565 702e 636c 6965   blacksheep.clie
-000027d0: 6e74 2069 6d70 6f72 7420 436c 6965 6e74  nt import Client
-000027e0: 5365 7373 696f 6e0a 0a0a 6173 796e 6320  Session...async 
-000027f0: 6465 6620 636c 6965 6e74 5f65 7861 6d70  def client_examp
-00002800: 6c65 2829 3a0a 2020 2020 6173 796e 6320  le():.    async 
-00002810: 7769 7468 2043 6c69 656e 7453 6573 7369  with ClientSessi
-00002820: 6f6e 2829 2061 7320 636c 6965 6e74 3a0a  on() as client:.
-00002830: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00002840: 203d 2061 7761 6974 2063 6c69 656e 742e   = await client.
-00002850: 6765 7428 2268 7474 7073 3a2f 2f64 6f63  get("https://doc
-00002860: 732e 7079 7468 6f6e 2e6f 7267 2f33 2f22  s.python.org/3/"
-00002870: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00002880: 7420 7265 7370 6f6e 7365 2069 7320 6e6f  t response is no
-00002890: 7420 4e6f 6e65 0a20 2020 2020 2020 2074  t None.        t
-000028a0: 6578 7420 3d20 6177 6169 7420 7265 7370  ext = await resp
-000028b0: 6f6e 7365 2e74 6578 7428 290a 2020 2020  onse.text().    
-000028c0: 2020 2020 7072 696e 7428 7465 7874 290a      print(text).
-000028d0: 0a0a 6173 796e 6369 6f2e 7275 6e28 636c  ..asyncio.run(cl
-000028e0: 6965 6e74 5f65 7861 6d70 6c65 2829 290a  ient_example()).
-000028f0: 6060 600a 0a23 2320 5375 7070 6f72 7465  ```..## Supporte
-00002900: 6420 706c 6174 666f 726d 7320 616e 6420  d platforms and 
-00002910: 7275 6e74 696d 6573 0a2a 2050 7974 686f  runtimes.* Pytho
-00002920: 6e3a 2061 6c6c 2076 6572 7369 6f6e 7320  n: all versions 
-00002930: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
-00002940: 6275 696c 6420 6d61 7472 6978 0a2a 2055  build matrix.* U
-00002950: 6275 6e74 750a 2a20 5769 6e64 6f77 7320  buntu.* Windows 
-00002960: 3130 0a2a 206d 6163 4f53 0a0a 2323 2044  10.* macOS..## D
-00002970: 6f63 756d 656e 7461 7469 6f6e 0a50 6c65  ocumentation.Ple
-00002980: 6173 6520 7265 6665 7220 746f 2074 6865  ase refer to the
-00002990: 205b 646f 6375 6d65 6e74 6174 696f 6e20   [documentation 
-000029a0: 7765 6273 6974 655d 2868 7474 7073 3a2f  website](https:/
-000029b0: 2f77 7777 2e6e 656f 7465 726f 692e 6465  /www.neoteroi.de
-000029c0: 762f 626c 6163 6b73 6865 6570 2f29 2e0a  v/blacksheep/)..
-000029d0: 0a23 2320 436f 6d6d 756e 6963 6174 696f  .## Communicatio
-000029e0: 6e0a 5b42 6c61 636b 5368 6565 7020 636f  n.[BlackSheep co
-000029f0: 6d6d 756e 6974 7920 696e 2047 6974 7465  mmunity in Gitte
-00002a00: 725d 2868 7474 7073 3a2f 2f67 6974 7465  r](https://gitte
-00002a10: 722e 696d 2f4e 656f 7465 726f 692f 426c  r.im/Neoteroi/Bl
-00002a20: 6163 6b53 6865 6570 292e 0a0a 2323 2042  ackSheep)...## B
-00002a30: 7261 6e63 6865 730a 5468 6520 5f6d 6169  ranches.The _mai
-00002a40: 6e5f 2062 7261 6e63 6820 636f 6e74 6169  n_ branch contai
-00002a50: 6e73 2074 6865 2063 7572 7265 6e74 6c79  ns the currently
-00002a60: 2064 6576 656c 6f70 6564 2076 6572 7369   developed versi
-00002a70: 6f6e 2c20 7768 6963 6820 6973 2076 6572  on, which is ver
-00002a80: 7369 6f6e 2032 0a61 6c70 6861 2e20 5468  sion 2.alpha. Th
-00002a90: 6520 5f76 315f 2062 7261 6e63 6820 636f  e _v1_ branch co
-00002aa0: 6e74 6169 6e73 2076 6572 7369 6f6e 2031  ntains version 1
-00002ab0: 206f 6620 7468 6520 7765 6220 6672 616d   of the web fram
-00002ac0: 6577 6f72 6b2c 2066 6f72 2062 7567 7320  ework, for bugs 
-00002ad0: 6669 7865 730a 616e 6420 6d61 696e 7465  fixes.and mainte
-00002ae0: 6e61 6e63 652e 0a                        nance..
+00000010: 3a20 322e 310d 0a4e 616d 653a 2062 6c61  : 2.1..Name: bla
+00000020: 636b 7368 6565 700d 0a56 6572 7369 6f6e  cksheep..Version
+00000030: 3a20 322e 3061 390d 0a53 756d 6d61 7279  : 2.0a9..Summary
+00000040: 3a20 4661 7374 2077 6562 2066 7261 6d65  : Fast web frame
+00000050: 776f 726b 2066 6f72 2050 7974 686f 6e20  work for Python 
+00000060: 6173 796e 6369 6f0d 0a41 7574 686f 722d  asyncio..Author-
+00000070: 656d 6169 6c3a 2052 6f62 6572 746f 2050  email: Roberto P
+00000080: 7265 7661 746f 203c 726f 6265 7274 6f2e  revato <roberto.
+00000090: 7072 6576 6174 6f40 676d 6169 6c2e 636f  prevato@gmail.co
+000000a0: 6d3e 0d0a 5072 6f6a 6563 742d 5552 4c3a  m>..Project-URL:
+000000b0: 2048 6f6d 6570 6167 652c 2068 7474 7073   Homepage, https
+000000c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e65  ://github.com/Ne
+000000d0: 6f74 6572 6f69 2f42 6c61 636b 5368 6565  oteroi/BlackShee
+000000e0: 700d 0a50 726f 6a65 6374 2d55 524c 3a20  p..Project-URL: 
+000000f0: 4275 6720 5472 6163 6b65 722c 2068 7474  Bug Tracker, htt
+00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000110: 4e65 6f74 6572 6f69 2f42 6c61 636b 5368  Neoteroi/BlackSh
+00000120: 6565 702f 6973 7375 6573 0d0a 4b65 7977  eep/issues..Keyw
+00000130: 6f72 6473 3a20 626c 6163 6b73 6865 6570  ords: blacksheep
+00000140: 2c77 6562 2066 7261 6d65 776f 726b 2c61  ,web framework,a
+00000150: 7379 6e63 696f 0d0a 436c 6173 7369 6669  syncio..Classifi
+00000160: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+00000170: 5374 6174 7573 203a 3a20 3320 2d20 416c  Status :: 3 - Al
+00000180: 7068 610d 0a43 6c61 7373 6966 6965 723a  pha..Classifier:
+00000190: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+000001a0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000001b0: 4c69 6365 6e73 650d 0a43 6c61 7373 6966  License..Classif
+000001c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001e0: 686f 6e20 3a3a 2033 2e38 0d0a 436c 6173  hon :: 3.8..Clas
+000001f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000210: 5079 7468 6f6e 203a 3a20 332e 390d 0a43  Python :: 3.9..C
+00000220: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000250: 300d 0a43 6c61 7373 6966 6965 723a 2050  0..Classifier: P
+00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000280: 2033 2e31 310d 0a43 6c61 7373 6966 6965   3.11..Classifie
+00000290: 723a 2045 6e76 6972 6f6e 6d65 6e74 203a  r: Environment :
+000002a0: 3a20 5765 6220 456e 7669 726f 6e6d 656e  : Web Environmen
+000002b0: 740d 0a43 6c61 7373 6966 6965 723a 204f  t..Classifier: O
+000002c0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000002d0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000002e0: 740d 0a43 6c61 7373 6966 6965 723a 2046  t..Classifier: F
+000002f0: 7261 6d65 776f 726b 203a 3a20 4173 796e  ramework :: Asyn
+00000300: 6349 4f0d 0a52 6571 7569 7265 732d 5079  cIO..Requires-Py
+00000310: 7468 6f6e 3a20 3e3d 332e 370d 0a44 6573  thon: >=3.7..Des
+00000320: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000330: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000340: 646f 776e 0d0a 5072 6f76 6964 6573 2d45  down..Provides-E
+00000350: 7874 7261 3a20 6a69 6e6a 610d 0a50 726f  xtra: jinja..Pro
+00000360: 7669 6465 732d 4578 7472 613a 2066 756c  vides-Extra: ful
+00000370: 6c0d 0a4c 6963 656e 7365 2d46 696c 653a  l..License-File:
+00000380: 204c 4943 454e 5345 0d0a 0d0a 5b21 5b42   LICENSE....[![B
+00000390: 7569 6c64 5d28 6874 7470 733a 2f2f 6769  uild](https://gi
+000003a0: 7468 7562 2e63 6f6d 2f4e 656f 7465 726f  thub.com/Neotero
+000003b0: 692f 426c 6163 6b53 6865 6570 2f77 6f72  i/BlackSheep/wor
+000003c0: 6b66 6c6f 7773 2f4d 6169 6e2f 6261 6467  kflows/Main/badg
+000003d0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000003e0: 6769 7468 7562 2e63 6f6d 2f4e 656f 7465  github.com/Neote
+000003f0: 726f 692f 426c 6163 6b53 6865 6570 2f61  roi/BlackSheep/a
+00000400: 6374 696f 6e73 290d 0a5b 215b 7079 7069  ctions)..[![pypi
+00000410: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000420: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000430: 426c 6163 6b53 6865 6570 2e73 7667 3f63  BlackSheep.svg?c
+00000440: 6f6c 6f72 3d62 6c75 6529 5d28 6874 7470  olor=blue)](http
+00000450: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000460: 6a65 6374 2f42 6c61 636b 5368 6565 702f  ject/BlackSheep/
+00000470: 290d 0a5b 215b 7665 7273 696f 6e73 5d28  )..[![versions](
+00000480: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000490: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+000004a0: 7273 696f 6e73 2f62 6c61 636b 7368 6565  rsions/blackshee
+000004b0: 702e 7376 6729 5d28 6874 7470 733a 2f2f  p.svg)](https://
+000004c0: 6769 7468 7562 2e63 6f6d 2f72 6f62 6572  github.com/rober
+000004d0: 746f 7072 6576 6174 6f2f 626c 6163 6b73  toprevato/blacks
+000004e0: 6865 6570 290d 0a5b 215b 636f 6465 636f  heep)..[![codeco
+000004f0: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000500: 6f76 2e69 6f2f 6768 2f4e 656f 7465 726f  ov.io/gh/Neotero
+00000510: 692f 426c 6163 6b53 6865 6570 2f62 7261  i/BlackSheep/bra
+00000520: 6e63 682f 6d61 7374 6572 2f67 7261 7068  nch/master/graph
+00000530: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00000540: 3d4e 7a69 3239 4c30 4567 3129 5d28 6874  =Nzi29L0Eg1)](ht
+00000550: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000560: 2f67 682f 4e65 6f74 6572 6f69 2f42 6c61  /gh/Neoteroi/Bla
+00000570: 636b 5368 6565 7029 0d0a 5b21 5b6c 6963  ckSheep)..[![lic
+00000580: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
+00000590: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000005a0: 6875 622f 6c69 6365 6e73 652f 4e65 6f74  hub/license/Neot
+000005b0: 6572 6f69 2f62 6c61 636b 7368 6565 702e  eroi/blacksheep.
+000005c0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+000005d0: 7468 7562 2e63 6f6d 2f4e 656f 7465 726f  thub.com/Neotero
+000005e0: 692f 626c 6163 6b73 6865 6570 2f62 6c6f  i/blacksheep/blo
+000005f0: 622f 6d61 696e 2f4c 4943 454e 5345 2920  b/main/LICENSE) 
+00000600: 5b21 5b4a 6f69 6e20 7468 6520 6368 6174  [![Join the chat
+00000610: 2061 7420 6874 7470 733a 2f2f 6769 7474   at https://gitt
+00000620: 6572 2e69 6d2f 4e65 6f74 6572 6f69 2f42  er.im/Neoteroi/B
+00000630: 6c61 636b 5368 6565 705d 2868 7474 7073  lackSheep](https
+00000640: 3a2f 2f62 6164 6765 732e 6769 7474 6572  ://badges.gitter
+00000650: 2e69 6d2f 4e65 6f74 6572 6f69 2f42 6c61  .im/Neoteroi/Bla
+00000660: 636b 5368 6565 702e 7376 6729 5d28 6874  ckSheep.svg)](ht
+00000670: 7470 733a 2f2f 6769 7474 6572 2e69 6d2f  tps://gitter.im/
+00000680: 4e65 6f74 6572 6f69 2f42 6c61 636b 5368  Neoteroi/BlackSh
+00000690: 6565 703f 7574 6d5f 736f 7572 6365 3d62  eep?utm_source=b
+000006a0: 6164 6765 2675 746d 5f6d 6564 6975 6d3d  adge&utm_medium=
+000006b0: 6261 6467 6526 7574 6d5f 6361 6d70 6169  badge&utm_campai
+000006c0: 676e 3d70 722d 6261 6467 6526 7574 6d5f  gn=pr-badge&utm_
+000006d0: 636f 6e74 656e 743d 6261 6467 6529 205b  content=badge) [
+000006e0: 215b 646f 6375 6d65 6e74 6174 696f 6e5d  ![documentation]
+000006f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000700: 656c 6473 2e69 6f2f 6261 6467 652f f09f  elds.io/badge/..
+00000710: 9396 2d64 6f63 732d 7075 7270 6c65 295d  ..-docs-purple)]
+00000720: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00000730: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+00000740: 6865 6570 2f29 0d0a 0d0a 2320 426c 6163  heep/)....# Blac
+00000750: 6b53 6865 6570 0d0a 426c 6163 6b53 6865  kSheep..BlackShe
+00000760: 6570 2069 7320 616e 2061 7379 6e63 6872  ep is an asynchr
+00000770: 6f6e 6f75 7320 7765 6220 6672 616d 6577  onous web framew
+00000780: 6f72 6b20 746f 2062 7569 6c64 2065 7665  ork to build eve
+00000790: 6e74 2062 6173 6564 2077 6562 0d0a 6170  nt based web..ap
+000007a0: 706c 6963 6174 696f 6e73 2077 6974 6820  plications with 
+000007b0: 5079 7468 6f6e 2e20 4974 2069 7320 696e  Python. It is in
+000007c0: 7370 6972 6564 2062 790d 0a5b 466c 6173  spired by..[Flas
+000007d0: 6b5d 2868 7474 7073 3a2f 2f70 616c 6c65  k](https://palle
+000007e0: 7473 7072 6f6a 6563 7473 2e63 6f6d 2f70  tsprojects.com/p
+000007f0: 2f66 6c61 736b 2f29 2c20 5b41 5350 2e4e  /flask/), [ASP.N
+00000800: 4554 0d0a 436f 7265 5d28 6874 7470 733a  ET..Core](https:
+00000810: 2f2f 646f 6373 2e6d 6963 726f 736f 6674  //docs.microsoft
+00000820: 2e63 6f6d 2f65 6e2d 7573 2f61 7370 6e65  .com/en-us/aspne
+00000830: 742f 636f 7265 2f29 2c20 616e 6420 7468  t/core/), and th
+00000840: 6520 776f 726b 2062 7920 5b59 7572 790d  e work by [Yury.
+00000850: 0a53 656c 6976 616e 6f76 5d28 6874 7470  .Selivanov](http
+00000860: 733a 2f2f 6d61 6769 632e 696f 2f62 6c6f  s://magic.io/blo
+00000870: 672f 7576 6c6f 6f70 2d62 6c61 7a69 6e67  g/uvloop-blazing
+00000880: 2d66 6173 742d 7079 7468 6f6e 2d6e 6574  -fast-python-net
+00000890: 776f 726b 696e 672f 292e 0d0a 0d0a 3c70  working/).....<p
+000008a0: 2061 6c69 676e 3d22 6c65 6674 223e 0d0a   align="left">..
+000008b0: 2020 3c61 2068 7265 663d 2223 626c 6163    <a href="#blac
+000008c0: 6b73 6865 6570 223e 3c69 6d67 2077 6964  ksheep"><img wid
+000008d0: 7468 3d22 3332 3022 2068 6569 6768 743d  th="320" height=
+000008e0: 2232 3731 2220 7372 633d 2268 7474 7073  "271" src="https
+000008f0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
+00000900: 6465 762f 626c 6163 6b73 6865 6570 2f69  dev/blacksheep/i
+00000910: 6d67 2f62 6c61 636b 7368 6565 702e 706e  mg/blacksheep.pn
+00000920: 6722 2061 6c74 3d22 426c 6163 6b20 5368  g" alt="Black Sh
+00000930: 6565 7022 3e3c 2f61 3e0d 0a3c 2f70 3e0d  eep"></a>..</p>.
+00000940: 0a0d 0a60 6060 6261 7368 0d0a 7069 7020  ...```bash..pip 
+00000950: 696e 7374 616c 6c20 626c 6163 6b73 6865  install blackshe
+00000960: 6570 0d0a 6060 600d 0a0d 0a2d 2d2d 0d0a  ep..```....---..
+00000970: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
+00000980: 6d20 6461 7465 7469 6d65 2069 6d70 6f72  m datetime impor
+00000990: 7420 6461 7465 7469 6d65 0d0a 0d0a 6672  t datetime....fr
+000009a0: 6f6d 2062 6c61 636b 7368 6565 7020 696d  om blacksheep im
+000009b0: 706f 7274 2041 7070 6c69 6361 7469 6f6e  port Application
+000009c0: 0d0a 0d0a 0d0a 6170 7020 3d20 4170 706c  ......app = Appl
+000009d0: 6963 6174 696f 6e28 290d 0a0d 0a40 6170  ication()....@ap
+000009e0: 702e 726f 7574 6528 222f 2229 0d0a 6173  p.route("/")..as
+000009f0: 796e 6320 6465 6620 686f 6d65 2829 3a0d  ync def home():.
+00000a00: 0a20 2020 2072 6574 7572 6e20 6622 4865  .    return f"He
+00000a10: 6c6c 6f2c 2057 6f72 6c64 2120 7b64 6174  llo, World! {dat
+00000a20: 6574 696d 652e 7574 636e 6f77 2829 2e69  etime.utcnow().i
+00000a30: 736f 666f 726d 6174 2829 7d22 0d0a 0d0a  soformat()}"....
+00000a40: 6060 600d 0a0d 0a23 2320 4765 7474 696e  ```....## Gettin
+00000a50: 6720 7374 6172 7465 6420 7573 696e 6720  g started using 
+00000a60: 7468 6520 434c 4920 e29c a80d 0a0d 0a42  the CLI .......B
+00000a70: 6c61 636b 5368 6565 7020 6f66 6665 7273  lackSheep offers
+00000a80: 2061 2043 4c49 2074 6f20 626f 6f74 7374   a CLI to bootst
+00000a90: 7261 7020 6e65 7720 7072 6f6a 6563 7473  rap new projects
+00000aa0: 2072 6170 6964 6c79 2e0d 0a54 6f20 7472   rapidly...To tr
+00000ab0: 7920 6974 2c20 6669 7273 7420 696e 7374  y it, first inst
+00000ac0: 616c 6c20 7468 6520 6062 6c61 636b 7368  all the `blacksh
+00000ad0: 6565 702d 636c 6960 2070 6163 6b61 6765  eep-cli` package
+00000ae0: 3a0d 0a0d 0a60 6060 6261 7368 0d0a 7069  :....```bash..pi
+00000af0: 7020 696e 7374 616c 6c20 626c 6163 6b73  p install blacks
+00000b00: 6865 6570 2d63 6c69 0d0a 6060 600d 0a0d  heep-cli..```...
+00000b10: 0a54 6865 6e20 7573 6520 7468 6520 6062  .Then use the `b
+00000b20: 6c61 636b 7368 6565 7020 6372 6561 7465  lacksheep create
+00000b30: 6020 636f 6d6d 616e 6420 746f 2062 6f6f  ` command to boo
+00000b40: 7473 7472 6170 2061 2070 726f 6a65 6374  tstrap a project
+00000b50: 0d0a 7573 696e 6720 6f6e 6520 6f66 2074  ..using one of t
+00000b60: 6865 2073 7570 706f 7274 6564 2074 656d  he supported tem
+00000b70: 706c 6174 6573 2e0d 0a0d 0a21 5b62 6c61  plates.....![bla
+00000b80: 636b 7368 6565 7020 6372 6561 7465 2063  cksheep create c
+00000b90: 6f6d 6d61 6e64 5d28 6874 7470 733a 2f2f  ommand](https://
+00000ba0: 6769 7374 2e67 6974 6875 6275 7365 7263  gist.githubuserc
+00000bb0: 6f6e 7465 6e74 2e63 6f6d 2f52 6f62 6572  ontent.com/Rober
+00000bc0: 746f 5072 6576 6174 6f2f 3338 6130 3539  toPrevato/38a059
+00000bd0: 3862 3531 3561 3266 3732 3537 6336 3134  8b515a2f7257c614
+00000be0: 3933 3838 3433 6239 3962 2f72 6177 2f36  938843b99b/raw/6
+00000bf0: 3764 3135 6261 3333 3764 6539 3463 3266  7d15ba337de94c2f
+00000c00: 3530 6439 3830 6137 6238 3932 3461 3734  50d980a7b8924a74
+00000c10: 3732 3539 3235 342f 626c 6163 6b73 6865  7259254/blackshe
+00000c20: 6570 2d63 7265 6174 652d 6465 6d6f 2e67  ep-create-demo.g
+00000c30: 6966 290d 0a0d 0a54 6865 2043 4c49 2069  if)....The CLI i
+00000c40: 6e63 6c75 6465 7320 6120 6865 6c70 2c20  ncludes a help, 
+00000c50: 616e 6420 7375 7070 6f72 7473 2063 7573  and supports cus
+00000c60: 746f 6d20 7465 6d70 6c61 7465 732c 2075  tom templates, u
+00000c70: 7369 6e67 2074 6865 0d0a 7361 6d65 2073  sing the..same s
+00000c80: 6f75 7263 6573 2073 7570 706f 7274 6564  ources supported
+00000c90: 2062 7920 6043 6f6f 6b69 6563 7574 7465   by `Cookiecutte
+00000ca0: 7260 2e0d 0a0d 0a23 2320 4765 7474 696e  r`.....## Gettin
+00000cb0: 6720 7374 6172 7465 6420 7769 7468 2074  g started with t
+00000cc0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+00000cd0: 0d0a 0d0a 5468 6520 646f 6375 6d65 6e74  ....The document
+00000ce0: 6174 696f 6e20 6f66 6665 7273 2067 6574  ation offers get
+00000cf0: 7469 6e67 2073 7461 7274 6564 2074 7574  ting started tut
+00000d00: 6f72 6961 6c73 3a0d 0a2a 205b 4765 7474  orials:..* [Gett
+00000d10: 696e 6720 7374 6172 7465 643a 0d0a 2020  ing started:..  
+00000d20: 6261 7369 6373 5d28 6874 7470 733a 2f2f  basics](https://
+00000d30: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
+00000d40: 2f62 6c61 636b 7368 6565 702f 6765 7474  /blacksheep/gett
+00000d50: 696e 672d 7374 6172 7465 642f 290d 0a2a  ing-started/)..*
+00000d60: 205b 4765 7474 696e 6720 7374 6172 7465   [Getting starte
+00000d70: 643a 2074 6865 204d 5643 2070 726f 6a65  d: the MVC proje
+00000d80: 6374 0d0a 2020 7465 6d70 6c61 7465 5d28  ct..  template](
+00000d90: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
+00000da0: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
+00000db0: 6565 702f 6d76 632d 7072 6f6a 6563 742d  eep/mvc-project-
+00000dc0: 7465 6d70 6c61 7465 2f29 0d0a 0d0a 5468  template/)....Th
+00000dd0: 6573 6520 7072 6f6a 6563 7420 7465 6d70  ese project temp
+00000de0: 6c61 7465 7320 6361 6e20 6265 2075 7365  lates can be use
+00000df0: 6420 746f 2073 7461 7274 206e 6577 2061  d to start new a
+00000e00: 7070 6c69 6361 7469 6f6e 7320 6661 7374  pplications fast
+00000e10: 6572 3a0d 0a0d 0a2a 205b 4d56 4320 7072  er:....* [MVC pr
+00000e20: 6f6a 6563 740d 0a20 2074 656d 706c 6174  oject..  templat
+00000e30: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000e40: 622e 636f 6d2f 4e65 6f74 6572 6f69 2f42  b.com/Neoteroi/B
+00000e50: 6c61 636b 5368 6565 704d 5643 290d 0a2a  lackSheepMVC)..*
+00000e60: 205b 456d 7074 7920 7072 6f6a 6563 740d   [Empty project.
+00000e70: 0a20 2074 656d 706c 6174 655d 2868 7474  .  template](htt
+00000e80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e90: 4e65 6f74 6572 6f69 2f42 6c61 636b 5368  Neoteroi/BlackSh
+00000ea0: 6565 7045 6d70 7479 5072 6f6a 6563 7429  eepEmptyProject)
+00000eb0: 0d0a 0d0a 2323 2052 6571 7569 7265 6d65  ....## Requireme
+00000ec0: 6e74 730d 0a0d 0a5b 5079 7468 6f6e 5d28  nts....[Python](
+00000ed0: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
+00000ee0: 6f6e 2e6f 7267 293a 2061 6e79 2076 6572  on.org): any ver
+00000ef0: 7369 6f6e 206c 6973 7465 6420 696e 2074  sion listed in t
+00000f00: 6865 2070 726f 6a65 6374 2773 0d0a 636c  he project's..cl
+00000f10: 6173 7369 6669 6572 732e 2054 6865 2063  assifiers. The c
+00000f20: 7572 7265 6e74 206c 6973 7420 6973 3a0d  urrent list is:.
+00000f30: 0a0d 0a5b 215b 7665 7273 696f 6e73 5d28  ...[![versions](
+00000f40: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000f50: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000f60: 7273 696f 6e73 2f62 6c61 636b 7368 6565  rsions/blackshee
+00000f70: 702e 7376 6729 5d28 6874 7470 733a 2f2f  p.svg)](https://
+00000f80: 6769 7468 7562 2e63 6f6d 2f72 6f62 6572  github.com/rober
+00000f90: 746f 7072 6576 6174 6f2f 626c 6163 6b73  toprevato/blacks
+00000fa0: 6865 6570 290d 0a0d 0a0d 0a42 6c61 636b  heep)......Black
+00000fb0: 5368 6565 7020 6265 6c6f 6e67 7320 746f  Sheep belongs to
+00000fc0: 2074 6865 2063 6174 6567 6f72 7920 6f66   the category of
+00000fd0: 0d0a 5b41 5347 495d 2868 7474 7073 3a2f  ..[ASGI](https:/
+00000fe0: 2f61 7367 692e 7265 6164 7468 6564 6f63  /asgi.readthedoc
+00000ff0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f29  s.io/en/latest/)
+00001000: 2077 6562 2066 7261 6d65 776f 726b 732c   web frameworks,
+00001010: 2073 6f20 6974 2072 6571 7569 7265 730d   so it requires.
+00001020: 0a61 6e20 4153 4749 2048 5454 5020 7365  .an ASGI HTTP se
+00001030: 7276 6572 2074 6f20 7275 6e2c 2073 7563  rver to run, suc
+00001040: 6820 6173 205b 7576 6963 6f72 6e5d 2868  h as [uvicorn](h
+00001050: 7474 703a 2f2f 7777 772e 7576 6963 6f72  ttp://www.uvicor
+00001060: 6e2e 6f72 672f 292c 206f 720d 0a5b 6879  n.org/), or..[hy
+00001070: 7065 7263 6f72 6e5d 2868 7474 7073 3a2f  percorn](https:/
+00001080: 2f70 676a 6f6e 6573 2e67 6974 6c61 622e  /pgjones.gitlab.
+00001090: 696f 2f68 7970 6572 636f 726e 2f29 2e20  io/hypercorn/). 
+000010a0: 466f 7220 6578 616d 706c 652c 2074 6f20  For example, to 
+000010b0: 7573 6520 6974 2077 6974 680d 0a75 7669  use it with..uvi
+000010c0: 636f 726e 3a0d 0a0d 0a60 6060 6261 7368  corn:....```bash
+000010d0: 0d0a 2420 7069 7020 696e 7374 616c 6c20  ..$ pip install 
+000010e0: 7576 6963 6f72 6e0d 0a60 6060 0d0a 0d0a  uvicorn..```....
+000010f0: 546f 2072 756e 2061 6e20 6170 706c 6963  To run an applic
+00001100: 6174 696f 6e20 6c69 6b65 2069 6e20 7468  ation like in th
+00001110: 6520 6578 616d 706c 6520 6162 6f76 652c  e example above,
+00001120: 2075 7365 2074 6865 206d 6574 686f 6473   use the methods
+00001130: 2070 726f 7669 6465 6420 6279 0d0a 7468   provided by..th
+00001140: 6520 4153 4749 2048 5454 5020 5365 7276  e ASGI HTTP Serv
+00001150: 6572 3a0d 0a0d 0a60 6060 6261 7368 0d0a  er:....```bash..
+00001160: 2320 6966 2074 6865 2042 6c61 636b 5368  # if the BlackSh
+00001170: 6565 7020 6170 7020 6973 2064 6566 696e  eep app is defin
+00001180: 6564 2069 6e20 6120 6669 6c65 2060 7365  ed in a file `se
+00001190: 7276 6572 2e70 7960 0d0a 0d0a 2420 7576  rver.py`....$ uv
+000011a0: 6963 6f72 6e20 7365 7276 6572 3a61 7070  icorn server:app
+000011b0: 0d0a 6060 600d 0a0d 0a54 6f20 7275 6e20  ..```....To run 
+000011c0: 666f 7220 7072 6f64 7563 7469 6f6e 2c20  for production, 
+000011d0: 7265 6665 7220 746f 2074 6865 2064 6f63  refer to the doc
+000011e0: 756d 656e 7461 7469 6f6e 206f 6620 7468  umentation of th
+000011f0: 6520 6368 6f73 656e 2041 5347 4920 7365  e chosen ASGI se
+00001200: 7276 6572 0d0a 2869 2e65 2e20 666f 7220  rver..(i.e. for 
+00001210: 5b75 7669 636f 726e 5d28 6874 7470 733a  [uvicorn](https:
+00001220: 2f2f 7777 772e 7576 6963 6f72 6e2e 6f72  //www.uvicorn.or
+00001230: 672f 2372 756e 6e69 6e67 2d77 6974 682d  g/#running-with-
+00001240: 6775 6e69 636f 726e 2929 2e0d 0a0d 0a23  gunicorn)).....#
+00001250: 2320 4175 746f 6d61 7469 6320 6269 6e64  # Automatic bind
+00001260: 696e 6773 2061 6e64 2064 6570 656e 6465  ings and depende
+00001270: 6e63 7920 696e 6a65 6374 696f 6e0d 0a42  ncy injection..B
+00001280: 6c61 636b 5368 6565 7020 7375 7070 6f72  lackSheep suppor
+00001290: 7473 2061 7574 6f6d 6174 6963 2062 696e  ts automatic bin
+000012a0: 6469 6e67 206f 6620 7661 6c75 6573 2066  ding of values f
+000012b0: 6f72 2072 6571 7565 7374 2068 616e 646c  or request handl
+000012c0: 6572 732c 2062 7920 7479 7065 0d0a 616e  ers, by type..an
+000012d0: 6e6f 7461 7469 6f6e 206f 7220 6279 2063  notation or by c
+000012e0: 6f6e 7665 6e74 696f 6e73 2e20 5365 6520  onventions. See 
+000012f0: 5b6d 6f72 650d 0a68 6572 655d 2868 7474  [more..here](htt
+00001300: 7073 3a2f 2f77 7777 2e6e 656f 7465 726f  ps://www.neotero
+00001310: 692e 6465 762f 626c 6163 6b73 6865 6570  i.dev/blacksheep
+00001320: 2f72 6571 7565 7374 732f 292e 0d0a 0d0a  /requests/).....
+00001330: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00001340: 6461 7461 636c 6173 7365 7320 696d 706f  dataclasses impo
+00001350: 7274 2064 6174 6163 6c61 7373 0d0a 0d0a  rt dataclass....
+00001360: 6672 6f6d 2062 6c61 636b 7368 6565 7020  from blacksheep 
+00001370: 696d 706f 7274 2041 7070 6c69 6361 7469  import Applicati
+00001380: 6f6e 2c20 4672 6f6d 4a53 4f4e 2c20 4672  on, FromJSON, Fr
+00001390: 6f6d 5175 6572 790d 0a0d 0a0d 0a61 7070  omQuery......app
+000013a0: 203d 2041 7070 6c69 6361 7469 6f6e 2829   = Application()
+000013b0: 0d0a 0d0a 0d0a 4064 6174 6163 6c61 7373  ......@dataclass
+000013c0: 0d0a 636c 6173 7320 4372 6561 7465 4361  ..class CreateCa
+000013d0: 7449 6e70 7574 3a0d 0a20 2020 206e 616d  tInput:..    nam
+000013e0: 653a 2073 7472 0d0a 0d0a 0d0a 4061 7070  e: str......@app
+000013f0: 2e72 6f75 7465 722e 706f 7374 2822 2f61  .router.post("/a
+00001400: 7069 2f63 6174 7322 290d 0a61 7379 6e63  pi/cats")..async
+00001410: 2064 6566 2065 7861 6d70 6c65 2864 6174   def example(dat
+00001420: 613a 2046 726f 6d4a 534f 4e5b 4372 6561  a: FromJSON[Crea
+00001430: 7465 4361 7449 6e70 7574 5d29 3a0d 0a20  teCatInput]):.. 
+00001440: 2020 2023 2069 6e20 7468 6973 2065 7861     # in this exa
+00001450: 6d70 6c65 2c20 6461 7461 2069 7320 626f  mple, data is bo
+00001460: 756e 6420 6175 746f 6d61 7469 6361 6c6c  und automaticall
+00001470: 7920 7265 6164 696e 6720 7468 6520 4a53  y reading the JS
+00001480: 4f4e 0d0a 2020 2020 2320 7061 796c 6f61  ON..    # payloa
+00001490: 6420 616e 6420 6372 6561 7469 6e67 2061  d and creating a
+000014a0: 6e20 696e 7374 616e 6365 206f 6620 6043  n instance of `C
+000014b0: 7265 6174 6543 6174 496e 7075 7460 0d0a  reateCatInput`..
+000014c0: 2020 2020 2e2e 2e0d 0a0d 0a0d 0a40 6170      .........@ap
+000014d0: 702e 726f 7574 6572 2e67 6574 2822 2f3a  p.router.get("/:
+000014e0: 6375 6c74 7572 655f 636f 6465 2f3a 6172  culture_code/:ar
+000014f0: 6561 2229 0d0a 6173 796e 6320 6465 6620  ea")..async def 
+00001500: 686f 6d65 2863 756c 7475 7265 5f63 6f64  home(culture_cod
+00001510: 652c 2061 7265 6129 3a0d 0a20 2020 2023  e, area):..    #
+00001520: 2069 6e20 7468 6973 2065 7861 6d70 6c65   in this example
+00001530: 2c20 626f 7468 2070 6172 616d 6574 6572  , both parameter
+00001540: 7320 6172 6520 6f62 7461 696e 6564 2066  s are obtained f
+00001550: 726f 6d20 726f 7574 6573 2077 6974 680d  rom routes with.
+00001560: 0a20 2020 2023 206d 6174 6368 696e 6720  .    # matching 
+00001570: 6e61 6d65 730d 0a20 2020 2072 6574 7572  names..    retur
+00001580: 6e20 6622 5265 7175 6573 7420 666f 723a  n f"Request for:
+00001590: 207b 6375 6c74 7572 655f 636f 6465 7d20   {culture_code} 
+000015a0: 7b61 7265 617d 220d 0a0d 0a0d 0a40 6170  {area}"......@ap
+000015b0: 702e 726f 7574 6572 2e67 6574 2822 2f61  p.router.get("/a
+000015c0: 7069 2f70 726f 6475 6374 7322 290d 0a64  pi/products")..d
+000015d0: 6566 2067 6574 5f70 726f 6475 6374 7328  ef get_products(
+000015e0: 0d0a 2020 2020 7061 6765 3a20 696e 7420  ..    page: int 
+000015f0: 3d20 312c 0d0a 2020 2020 7369 7a65 3a20  = 1,..    size: 
+00001600: 696e 7420 3d20 3330 2c0d 0a20 2020 2073  int = 30,..    s
+00001610: 6561 7263 683a 2073 7472 203d 2022 222c  earch: str = "",
+00001620: 0d0a 293a 0d0a 2020 2020 2320 7468 6973  ..):..    # this
+00001630: 2065 7861 6d70 6c65 2069 6c6c 7573 7472   example illustr
+00001640: 6174 6573 2073 7570 706f 7274 2066 6f72  ates support for
+00001650: 2069 6d70 6c69 6369 7420 7175 6572 7920   implicit query 
+00001660: 7061 7261 6d65 7465 7273 2077 6974 680d  parameters with.
+00001670: 0a20 2020 2023 2064 6566 6175 6c74 2076  .    # default v
+00001680: 616c 7565 730d 0a20 2020 2023 2073 696e  alues..    # sin
+00001690: 6365 2074 6865 2073 6f75 7263 6520 6f66  ce the source of
+000016a0: 2070 6167 652c 2073 697a 652c 2061 6e64   page, size, and
+000016b0: 2073 6561 7263 6820 6973 206e 6f74 2073   search is not s
+000016c0: 7065 6369 6669 6564 2061 6e64 206e 6f0d  pecified and no.
+000016d0: 0a20 2020 2023 2072 6f75 7465 2070 6172  .    # route par
+000016e0: 616d 6574 6572 206d 6174 6368 6573 2074  ameter matches t
+000016f0: 6865 6972 206e 616d 652c 2074 6865 7920  heir name, they 
+00001700: 6172 6520 6f62 7461 696e 6564 2066 726f  are obtained fro
+00001710: 6d20 7175 6572 7920 7374 7269 6e67 0d0a  m query string..
+00001720: 2020 2020 2e2e 2e0d 0a0d 0a0d 0a40 6170      .........@ap
+00001730: 702e 726f 7574 6572 2e67 6574 2822 2f61  p.router.get("/a
+00001740: 7069 2f70 726f 6475 6374 7332 2229 0d0a  pi/products2")..
+00001750: 6465 6620 6765 745f 7072 6f64 7563 7473  def get_products
+00001760: 3228 0d0a 2020 2020 7061 6765 3a20 4672  2(..    page: Fr
+00001770: 6f6d 5175 6572 795b 696e 745d 203d 2046  omQuery[int] = F
+00001780: 726f 6d51 7565 7279 2831 292c 0d0a 2020  romQuery(1),..  
+00001790: 2020 7369 7a65 3a20 4672 6f6d 5175 6572    size: FromQuer
+000017a0: 795b 696e 745d 203d 2046 726f 6d51 7565  y[int] = FromQue
+000017b0: 7279 2833 3029 2c0d 0a20 2020 2073 6561  ry(30),..    sea
+000017c0: 7263 683a 2046 726f 6d51 7565 7279 5b73  rch: FromQuery[s
+000017d0: 7472 5d20 3d20 4672 6f6d 5175 6572 7928  tr] = FromQuery(
+000017e0: 2222 292c 0d0a 293a 0d0a 2020 2020 2320  ""),..):..    # 
+000017f0: 7468 6973 2065 7861 6d70 6c65 2069 6c6c  this example ill
+00001800: 7573 7472 6174 6573 2073 7570 706f 7274  ustrates support
+00001810: 2066 6f72 2065 7870 6c69 6369 7420 7175   for explicit qu
+00001820: 6572 7920 7061 7261 6d65 7465 7273 2077  ery parameters w
+00001830: 6974 680d 0a20 2020 2023 2064 6566 6175  ith..    # defau
+00001840: 6c74 2076 616c 7565 730d 0a20 2020 2023  lt values..    #
+00001850: 2069 6e20 7468 6973 2063 6173 652c 2070   in this case, p
+00001860: 6172 616d 6574 6572 7320 6172 6520 6578  arameters are ex
+00001870: 706c 6963 6974 6c79 2072 6561 6420 6672  plicitly read fr
+00001880: 6f6d 2071 7565 7279 2073 7472 696e 670d  om query string.
+00001890: 0a20 2020 202e 2e2e 0d0a 0d0a 6060 600d  .    .......```.
+000018a0: 0a0d 0a49 7420 616c 736f 2073 7570 706f  ...It also suppo
+000018b0: 7274 7320 5b64 6570 656e 6465 6e63 790d  rts [dependency.
+000018c0: 0a69 6e6a 6563 7469 6f6e 5d28 6874 7470  .injection](http
+000018d0: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
+000018e0: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
+000018f0: 6465 7065 6e64 656e 6379 2d69 6e6a 6563  dependency-injec
+00001900: 7469 6f6e 2f29 2c20 610d 0a66 6561 7475  tion/), a..featu
+00001910: 7265 2074 6861 7420 7072 6f76 6964 6573  re that provides
+00001920: 2061 2063 6f6e 7369 7374 656e 7420 616e   a consistent an
+00001930: 6420 636c 6561 6e20 7761 7920 746f 2075  d clean way to u
+00001940: 7365 2064 6570 656e 6465 6e63 6965 7320  se dependencies 
+00001950: 696e 2072 6571 7565 7374 0d0a 6861 6e64  in request..hand
+00001960: 6c65 7273 2e0d 0a0d 0a23 2320 4765 6e65  lers.....## Gene
+00001970: 7261 7469 6f6e 206f 6620 4f70 656e 4150  ration of OpenAP
+00001980: 4920 446f 6375 6d65 6e74 6174 696f 6e0d  I Documentation.
+00001990: 0a5b 4765 6e65 7261 7469 6f6e 206f 6620  .[Generation of 
+000019a0: 4f70 656e 4150 4920 446f 6375 6d65 6e74  OpenAPI Document
+000019b0: 6174 696f 6e5d 2868 7474 7073 3a2f 2f77  ation](https://w
+000019c0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+000019d0: 626c 6163 6b73 6865 6570 2f6f 7065 6e61  blacksheep/opena
+000019e0: 7069 2f29 2e0d 0a0d 0a23 2320 5374 7261  pi/).....## Stra
+000019f0: 7465 6769 6573 2074 6f20 6861 6e64 6c65  tegies to handle
+00001a00: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
+00001a10: 616e 6420 6175 7468 6f72 697a 6174 696f  and authorizatio
+00001a20: 6e0d 0a42 6c61 636b 5368 6565 7020 696d  n..BlackSheep im
+00001a30: 706c 656d 656e 7473 2073 7472 6174 6567  plements strateg
+00001a40: 6965 7320 746f 2068 616e 646c 6520 6175  ies to handle au
+00001a50: 7468 656e 7469 6361 7469 6f6e 2061 6e64  thentication and
+00001a60: 2061 7574 686f 7269 7a61 7469 6f6e 2e0d   authorization..
+00001a70: 0a54 6865 7365 2066 6561 7475 7265 7320  .These features 
+00001a80: 6172 6520 646f 6375 6d65 6e74 6564 2068  are documented h
+00001a90: 6572 653a 0d0a 0d0a 2a20 5b41 7574 6865  ere:....* [Authe
+00001aa0: 6e74 6963 6174 696f 6e5d 2868 7474 7073  ntication](https
+00001ab0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
+00001ac0: 6465 762f 626c 6163 6b73 6865 6570 2f61  dev/blacksheep/a
+00001ad0: 7574 6865 6e74 6963 6174 696f 6e2f 290d  uthentication/).
+00001ae0: 0a2a 205b 4175 7468 6f72 697a 6174 696f  .* [Authorizatio
+00001af0: 6e5d 2868 7474 7073 3a2f 2f77 7777 2e6e  n](https://www.n
+00001b00: 656f 7465 726f 692e 6465 762f 626c 6163  eoteroi.dev/blac
+00001b10: 6b73 6865 6570 2f61 7574 686f 7269 7a61  ksheep/authoriza
+00001b20: 7469 6f6e 2f29 0d0a 0d0a 6060 6070 7974  tion/)....```pyt
+00001b30: 686f 6e0d 0a61 7070 2e75 7365 5f61 7574  hon..app.use_aut
+00001b40: 6865 6e74 6963 6174 696f 6e28 295c 0d0a  hentication()\..
+00001b50: 2020 2020 2e61 6464 2845 7861 6d70 6c65      .add(Example
+00001b60: 4175 7468 656e 7469 6361 7469 6f6e 4861  AuthenticationHa
+00001b70: 6e64 6c65 7228 2929 0d0a 0d0a 0d0a 6170  ndler())......ap
+00001b80: 702e 7573 655f 6175 7468 6f72 697a 6174  p.use_authorizat
+00001b90: 696f 6e28 295c 0d0a 2020 2020 2e61 6464  ion()\..    .add
+00001ba0: 2841 646d 696e 7350 6f6c 6963 7928 2929  (AdminsPolicy())
+00001bb0: 0d0a 0d0a 0d0a 4061 7574 6828 2261 646d  ......@auth("adm
+00001bc0: 696e 2229 0d0a 4061 7070 2e72 6f75 7465  in")..@app.route
+00001bd0: 722e 6765 7428 222f 2229 0d0a 6173 796e  r.get("/")..asyn
+00001be0: 6320 6465 6620 6f6e 6c79 5f66 6f72 5f61  c def only_for_a
+00001bf0: 646d 696e 7328 293a 0d0a 2020 2020 2e2e  dmins():..    ..
+00001c00: 2e0d 0a0d 0a0d 0a40 6175 7468 2829 0d0a  .......@auth()..
+00001c10: 4061 7070 2e72 6f75 7465 722e 6765 7428  @app.router.get(
+00001c20: 222f 2229 0d0a 6173 796e 6320 6465 6620  "/")..async def 
+00001c30: 6f6e 6c79 5f66 6f72 5f61 7574 6865 6e74  only_for_authent
+00001c40: 6963 6174 6564 5f75 7365 7273 2829 3a0d  icated_users():.
+00001c50: 0a20 2020 202e 2e2e 0d0a 6060 600d 0a0d  .    .....```...
+00001c60: 0a53 696e 6365 2076 6572 7369 6f6e 2060  .Since version `
+00001c70: 312e 322e 3160 2c20 426c 6163 6b53 6865  1.2.1`, BlackShe
+00001c80: 6570 2069 6d70 6c65 6d65 6e74 733a 0d0a  ep implements:..
+00001c90: 0d0a 2a20 5b42 7569 6c74 2d69 6e20 7375  ..* [Built-in su
+00001ca0: 7070 6f72 7420 666f 7220 4f70 656e 4944  pport for OpenID
+00001cb0: 2043 6f6e 6e65 6374 2061 7574 6865 6e74   Connect authent
+00001cc0: 6963 6174 696f 6e5d 2868 7474 7073 3a2f  ication](https:/
+00001cd0: 2f77 7777 2e6e 656f 7465 726f 692e 6465  /www.neoteroi.de
+00001ce0: 762f 626c 6163 6b73 6865 6570 2f61 7574  v/blacksheep/aut
+00001cf0: 6865 6e74 6963 6174 696f 6e2f 236f 6964  hentication/#oid
+00001d00: 6329 0d0a 2a20 5b42 7569 6c74 2d69 6e20  c)..* [Built-in 
+00001d10: 7375 7070 6f72 7420 666f 7220 4a57 5420  support for JWT 
+00001d20: 4265 6172 6572 2061 7574 6865 6e74 6963  Bearer authentic
+00001d30: 6174 696f 6e5d 2868 7474 7073 3a2f 2f77  ation](https://w
+00001d40: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+00001d50: 626c 6163 6b73 6865 6570 2f61 7574 6865  blacksheep/authe
+00001d60: 6e74 6963 6174 696f 6e2f 236a 7774 2d62  ntication/#jwt-b
+00001d70: 6561 7265 7229 0d0a 0d0a 4d65 616e 696e  earer)....Meanin
+00001d80: 6720 7468 6174 2069 7420 6973 2065 6173  g that it is eas
+00001d90: 7920 746f 2069 6e74 6567 7261 7465 2077  y to integrate w
+00001da0: 6974 6820 7365 7276 6963 6573 2073 7563  ith services suc
+00001db0: 6820 6173 3a0d 0a2a 205b 4175 7468 305d  h as:..* [Auth0]
+00001dc0: 2868 7474 7073 3a2f 2f61 7574 6830 2e63  (https://auth0.c
+00001dd0: 6f6d 290d 0a2a 205b 417a 7572 6520 4163  om)..* [Azure Ac
+00001de0: 7469 7665 2044 6972 6563 746f 7279 5d28  tive Directory](
+00001df0: 6874 7470 733a 2f2f 617a 7572 652e 6d69  https://azure.mi
+00001e00: 6372 6f73 6f66 742e 636f 6d2f 656e 2d75  crosoft.com/en-u
+00001e10: 732f 7365 7276 6963 6573 2f61 6374 6976  s/services/activ
+00001e20: 652d 6469 7265 6374 6f72 792f 290d 0a2a  e-directory/)..*
+00001e30: 205b 417a 7572 6520 4163 7469 7665 2044   [Azure Active D
+00001e40: 6972 6563 746f 7279 2042 3243 5d28 6874  irectory B2C](ht
+00001e50: 7470 733a 2f2f 646f 6373 2e6d 6963 726f  tps://docs.micro
+00001e60: 736f 6674 2e63 6f6d 2f65 6e2d 7573 2f61  soft.com/en-us/a
+00001e70: 7a75 7265 2f61 6374 6976 652d 6469 7265  zure/active-dire
+00001e80: 6374 6f72 792d 6232 632f 6f76 6572 7669  ctory-b2c/overvi
+00001e90: 6577 290d 0a2a 205b 4f6b 7461 5d28 6874  ew)..* [Okta](ht
+00001ea0: 7470 733a 2f2f 7777 772e 6f6b 7461 2e63  tps://www.okta.c
+00001eb0: 6f6d 290d 0a0d 0a52 6566 6572 2074 6f20  om)....Refer to 
+00001ec0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00001ed0: 6e20 666f 7220 6d6f 7265 2064 6574 6169  n for more detai
+00001ee0: 6c73 2061 6e64 2065 7861 6d70 6c65 732e  ls and examples.
+00001ef0: 0d0a 0d0a 2323 2057 6562 2066 7261 6d65  ....## Web frame
+00001f00: 776f 726b 2066 6561 7475 7265 730d 0a0d  work features...
+00001f10: 0a2a 205b 4153 4749 2063 6f6d 7061 7469  .* [ASGI compati
+00001f20: 6269 6c69 7479 5d28 6874 7470 733a 2f2f  bility](https://
+00001f30: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
+00001f40: 2f62 6c61 636b 7368 6565 702f 6173 6769  /blacksheep/asgi
+00001f50: 2f29 0d0a 2a20 5b52 6f75 7469 6e67 5d28  /)..* [Routing](
+00001f60: 6874 7470 733a 2f2f 7777 772e 6e65 6f74  https://www.neot
+00001f70: 6572 6f69 2e64 6576 2f62 6c61 636b 7368  eroi.dev/blacksh
+00001f80: 6565 702f 726f 7574 696e 672f 290d 0a2a  eep/routing/)..*
+00001f90: 2052 6571 7565 7374 2068 616e 646c 6572   Request handler
+00001fa0: 7320 6361 6e20 6265 205b 6465 6669 6e65  s can be [define
+00001fb0: 6420 6173 0d0a 2020 6675 6e63 7469 6f6e  d as..  function
+00001fc0: 735d 2868 7474 7073 3a2f 2f77 7777 2e6e  s](https://www.n
+00001fd0: 656f 7465 726f 692e 6465 762f 626c 6163  eoteroi.dev/blac
+00001fe0: 6b73 6865 6570 2f72 6571 7565 7374 2d68  ksheep/request-h
+00001ff0: 616e 646c 6572 732f 292c 206f 7220 5b63  andlers/), or [c
+00002000: 6c61 7373 0d0a 2020 6d65 7468 6f64 735d  lass..  methods]
+00002010: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00002020: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+00002030: 6865 6570 2f63 6f6e 7472 6f6c 6c65 7273  heep/controllers
+00002040: 2f29 0d0a 2a20 5b4d 6964 646c 6577 6172  /)..* [Middlewar
+00002050: 6573 5d28 6874 7470 733a 2f2f 7777 772e  es](https://www.
+00002060: 6e65 6f74 6572 6f69 2e64 6576 2f62 6c61  neoteroi.dev/bla
+00002070: 636b 7368 6565 702f 6d69 6464 6c65 7761  cksheep/middlewa
+00002080: 7265 732f 290d 0a2a 205b 5765 6253 6f63  res/)..* [WebSoc
+00002090: 6b65 745d 2868 7474 7073 3a2f 2f77 7777  ket](https://www
+000020a0: 2e6e 656f 7465 726f 692e 6465 762f 626c  .neoteroi.dev/bl
+000020b0: 6163 6b73 6865 6570 2f77 6562 736f 636b  acksheep/websock
+000020c0: 6574 2f29 0d0a 2a20 5b42 7569 6c74 2d69  et/)..* [Built-i
+000020d0: 6e20 7375 7070 6f72 7420 666f 7220 6465  n support for de
+000020e0: 7065 6e64 656e 6379 0d0a 2020 696e 6a65  pendency..  inje
+000020f0: 6374 696f 6e5d 2868 7474 7073 3a2f 2f77  ction](https://w
+00002100: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+00002110: 626c 6163 6b73 6865 6570 2f64 6570 656e  blacksheep/depen
+00002120: 6465 6e63 792d 696e 6a65 6374 696f 6e2f  dency-injection/
+00002130: 290d 0a2a 205b 5375 7070 6f72 7420 666f  )..* [Support fo
+00002140: 7220 6175 746f 6d61 7469 6320 6269 6e64  r automatic bind
+00002150: 696e 6720 6f66 2072 6f75 7465 2061 6e64  ing of route and
+00002160: 2071 7565 7279 2070 6172 616d 6574 6572   query parameter
+00002170: 7320 746f 2072 6571 7565 7374 0d0a 2020  s to request..  
+00002180: 6861 6e64 6c65 7273 206d 6574 686f 6473  handlers methods
+00002190: 0d0a 2020 6361 6c6c 735d 2868 7474 7073  ..  calls](https
+000021a0: 3a2f 2f77 7777 2e6e 656f 7465 726f 692e  ://www.neoteroi.
+000021b0: 6465 762f 626c 6163 6b73 6865 6570 2f67  dev/blacksheep/g
+000021c0: 6574 7469 6e67 2d73 7461 7274 6564 2f23  etting-started/#
+000021d0: 6861 6e64 6c69 6e67 2d72 6f75 7465 2d70  handling-route-p
+000021e0: 6172 616d 6574 6572 7329 0d0a 2a20 5b53  arameters)..* [S
+000021f0: 7472 6174 6567 7920 746f 2068 616e 646c  trategy to handl
+00002200: 650d 0a20 2065 7863 6570 7469 6f6e 735d  e..  exceptions]
+00002210: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00002220: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+00002230: 6865 6570 2f61 7070 6c69 6361 7469 6f6e  heep/application
+00002240: 2f23 636f 6e66 6967 7572 696e 672d 6578  /#configuring-ex
+00002250: 6365 7074 696f 6e73 2d68 616e 646c 6572  ceptions-handler
+00002260: 7329 0d0a 2a20 5b53 7472 6174 6567 7920  s)..* [Strategy 
+00002270: 746f 2068 616e 646c 6520 6175 7468 656e  to handle authen
+00002280: 7469 6361 7469 6f6e 2061 6e64 0d0a 2020  tication and..  
+00002290: 6175 7468 6f72 697a 6174 696f 6e5d 2868  authorization](h
+000022a0: 7474 7073 3a2f 2f77 7777 2e6e 656f 7465  ttps://www.neote
+000022b0: 726f 692e 6465 762f 626c 6163 6b73 6865  roi.dev/blackshe
+000022c0: 6570 2f61 7574 6865 6e74 6963 6174 696f  ep/authenticatio
+000022d0: 6e2f 290d 0a2a 205b 4275 696c 742d 696e  n/)..* [Built-in
+000022e0: 2073 7570 706f 7274 2066 6f72 204f 7065   support for Ope
+000022f0: 6e49 4420 436f 6e6e 6563 7420 6175 7468  nID Connect auth
+00002300: 656e 7469 6361 7469 6f6e 2075 7369 6e67  entication using
+00002310: 204f 4944 430d 0a20 2064 6973 636f 7665   OIDC..  discove
+00002320: 7279 5d28 6874 7470 733a 2f2f 7777 772e  ry](https://www.
+00002330: 6e65 6f74 6572 6f69 2e64 6576 2f62 6c61  neoteroi.dev/bla
+00002340: 636b 7368 6565 702f 6175 7468 656e 7469  cksheep/authenti
+00002350: 6361 7469 6f6e 2f23 6f69 6463 290d 0a2a  cation/#oidc)..*
+00002360: 205b 4275 696c 742d 696e 2073 7570 706f   [Built-in suppo
+00002370: 7274 2066 6f72 204a 5754 2042 6561 7265  rt for JWT Beare
+00002380: 7220 6175 7468 656e 7469 6361 7469 6f6e  r authentication
+00002390: 2075 7369 6e67 204f 4944 4320 6469 7363   using OIDC disc
+000023a0: 6f76 6572 7920 616e 640d 0a20 206f 7468  overy and..  oth
+000023b0: 6572 2073 6f75 7263 6573 206f 660d 0a20  er sources of.. 
+000023c0: 204a 574b 535d 2868 7474 7073 3a2f 2f77   JWKS](https://w
+000023d0: 7777 2e6e 656f 7465 726f 692e 6465 762f  ww.neoteroi.dev/
+000023e0: 626c 6163 6b73 6865 6570 2f61 7574 6865  blacksheep/authe
+000023f0: 6e74 6963 6174 696f 6e2f 236a 7774 2d62  ntication/#jwt-b
+00002400: 6561 7265 7229 0d0a 2a20 5b48 616e 646c  earer)..* [Handl
+00002410: 6572 730d 0a20 206e 6f72 6d61 6c69 7a61  ers..  normaliza
+00002420: 7469 6f6e 5d28 6874 7470 733a 2f2f 7777  tion](https://ww
+00002430: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
+00002440: 6c61 636b 7368 6565 702f 7265 7175 6573  lacksheep/reques
+00002450: 742d 6861 6e64 6c65 7273 2f29 0d0a 2a20  t-handlers/)..* 
+00002460: 5b53 6572 7669 6e67 2073 7461 7469 630d  [Serving static.
+00002470: 0a20 2066 696c 6573 5d28 6874 7470 733a  .  files](https:
+00002480: 2f2f 7777 772e 6e65 6f74 6572 6f69 2e64  //www.neoteroi.d
+00002490: 6576 2f62 6c61 636b 7368 6565 702f 7374  ev/blacksheep/st
+000024a0: 6174 6963 2d66 696c 6573 2f29 0d0a 2a20  atic-files/)..* 
+000024b0: 5b49 6e74 6567 7261 7469 6f6e 2077 6974  [Integration wit
+000024c0: 680d 0a20 204a 696e 6a61 325d 2868 7474  h..  Jinja2](htt
+000024d0: 7073 3a2f 2f77 7777 2e6e 656f 7465 726f  ps://www.neotero
+000024e0: 692e 6465 762f 626c 6163 6b73 6865 6570  i.dev/blacksheep
+000024f0: 2f74 656d 706c 6174 696e 672f 290d 0a2a  /templating/)..*
+00002500: 205b 5375 7070 6f72 7420 666f 7220 7365   [Support for se
+00002510: 7276 696e 6720 5350 4173 2074 6861 7420  rving SPAs that 
+00002520: 7573 6520 4854 4d4c 3520 4869 7374 6f72  use HTML5 Histor
+00002530: 7920 4150 4920 666f 7220 636c 6965 6e74  y API for client
+00002540: 2073 6964 650d 0a20 2072 6f75 7469 6e67   side..  routing
+00002550: 5d28 6874 7470 733a 2f2f 7777 772e 6e65  ](https://www.ne
+00002560: 6f74 6572 6f69 2e64 6576 2f62 6c61 636b  oteroi.dev/black
+00002570: 7368 6565 702f 7374 6174 6963 2d66 696c  sheep/static-fil
+00002580: 6573 2f23 686f 772d 746f 2d73 6572 7665  es/#how-to-serve
+00002590: 2d73 7061 732d 7468 6174 2d75 7365 2d68  -spas-that-use-h
+000025a0: 746d 6c35 2d68 6973 746f 7279 2d61 7069  tml5-history-api
+000025b0: 290d 0a2a 205b 5375 7070 6f72 7420 666f  )..* [Support fo
+000025c0: 7220 6175 746f 6d61 7469 6320 6765 6e65  r automatic gene
+000025d0: 7261 7469 6f6e 206f 6620 4f70 656e 4150  ration of OpenAP
+000025e0: 490d 0a20 2044 6f63 756d 656e 7461 7469  I..  Documentati
+000025f0: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
+00002600: 6e65 6f74 6572 6f69 2e64 6576 2f62 6c61  neoteroi.dev/bla
+00002610: 636b 7368 6565 702f 6f70 656e 6170 692f  cksheep/openapi/
+00002620: 290d 0a2a 205b 5374 7261 7465 6779 2074  )..* [Strategy t
+00002630: 6f20 6861 6e64 6c65 2043 4f52 5320 7365  o handle CORS se
+00002640: 7474 696e 6773 5d28 6874 7470 733a 2f2f  ttings](https://
+00002650: 7777 772e 6e65 6f74 6572 6f69 2e64 6576  www.neoteroi.dev
+00002660: 2f62 6c61 636b 7368 6565 702f 636f 7273  /blacksheep/cors
+00002670: 2f29 0d0a 2a20 5b53 6573 7369 6f6e 735d  /)..* [Sessions]
+00002680: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+00002690: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+000026a0: 6865 6570 2f73 6573 7369 6f6e 732f 290d  heep/sessions/).
+000026b0: 0a2a 2053 7570 706f 7274 2066 6f72 2061  .* Support for a
+000026c0: 7574 6f6d 6174 6963 2062 696e 6469 6e67  utomatic binding
+000026d0: 206f 6620 6064 6174 6163 6c61 7373 6573   of `dataclasses
+000026e0: 6020 616e 640d 0a20 205b 6070 7964 616e  ` and..  [`pydan
+000026f0: 7469 6360 5d28 6874 7470 733a 2f2f 7079  tic`](https://py
+00002700: 6461 6e74 6963 2d64 6f63 732e 6865 6c70  dantic-docs.help
+00002710: 6d61 6e75 616c 2e69 6f29 206d 6f64 656c  manual.io) model
+00002720: 7320 746f 2068 616e 646c 6520 7468 650d  s to handle the.
+00002730: 0a20 2072 6571 7565 7374 2062 6f64 7920  .  request body 
+00002740: 7061 796c 6f61 6420 6578 7065 6374 6564  payload expected
+00002750: 2062 7920 7265 7175 6573 7420 6861 6e64   by request hand
+00002760: 6c65 7273 0d0a 2a20 5b60 5465 7374 436c  lers..* [`TestCl
+00002770: 6965 6e74 6020 636c 6173 7320 746f 2073  ient` class to s
+00002780: 696d 706c 6966 7920 7465 7374 696e 6720  implify testing 
+00002790: 6f66 2061 7070 6c69 6361 7469 6f6e 735d  of applications]
+000027a0: 2868 7474 7073 3a2f 2f77 7777 2e6e 656f  (https://www.neo
+000027b0: 7465 726f 692e 6465 762f 626c 6163 6b73  teroi.dev/blacks
+000027c0: 6865 6570 2f74 6573 7469 6e67 2f29 0d0a  heep/testing/)..
+000027d0: 2a20 5b41 6e74 6920 466f 7267 6572 7920  * [Anti Forgery 
+000027e0: 7661 6c69 6461 7469 6f6e 5d28 6874 7470  validation](http
+000027f0: 733a 2f2f 7777 772e 6e65 6f74 6572 6f69  s://www.neoteroi
+00002800: 2e64 6576 2f62 6c61 636b 7368 6565 702f  .dev/blacksheep/
+00002810: 616e 7469 2d72 6571 7565 7374 2d66 6f72  anti-request-for
+00002820: 6765 7279 2920 746f 2070 726f 7465 6374  gery) to protect
+00002830: 2061 6761 696e 7374 2043 726f 7373 2d53   against Cross-S
+00002840: 6974 6520 5265 7175 6573 7420 466f 7267  ite Request Forg
+00002850: 6572 7920 2858 5352 462f 4353 5246 2920  ery (XSRF/CSRF) 
+00002860: 6174 7461 636b 730d 0a0d 0a23 2320 436c  attacks....## Cl
+00002870: 6965 6e74 2066 6561 7475 7265 730d 0a0d  ient features...
+00002880: 0a42 6c61 636b 5368 6565 7020 696e 636c  .BlackSheep incl
+00002890: 7564 6573 2061 6e20 4854 5450 2043 6c69  udes an HTTP Cli
+000028a0: 656e 742e 0d0a 0d0a 2a2a 4578 616d 706c  ent.....**Exampl
+000028b0: 653a 2a2a 0d0a 6060 6070 7974 686f 6e0d  e:**..```python.
+000028c0: 0a69 6d70 6f72 7420 6173 796e 6369 6f0d  .import asyncio.
+000028d0: 0a0d 0a66 726f 6d20 626c 6163 6b73 6865  ...from blackshe
+000028e0: 6570 2e63 6c69 656e 7420 696d 706f 7274  ep.client import
+000028f0: 2043 6c69 656e 7453 6573 7369 6f6e 0d0a   ClientSession..
+00002900: 0d0a 0d0a 6173 796e 6320 6465 6620 636c  ....async def cl
+00002910: 6965 6e74 5f65 7861 6d70 6c65 2829 3a0d  ient_example():.
+00002920: 0a20 2020 2061 7379 6e63 2077 6974 6820  .    async with 
+00002930: 436c 6965 6e74 5365 7373 696f 6e28 2920  ClientSession() 
+00002940: 6173 2063 6c69 656e 743a 0d0a 2020 2020  as client:..    
+00002950: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+00002960: 7761 6974 2063 6c69 656e 742e 6765 7428  wait client.get(
+00002970: 2268 7474 7073 3a2f 2f64 6f63 732e 7079  "https://docs.py
+00002980: 7468 6f6e 2e6f 7267 2f33 2f22 290d 0a0d  thon.org/3/")...
+00002990: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000029a0: 7265 7370 6f6e 7365 2069 7320 6e6f 7420  response is not 
+000029b0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7465  None..        te
+000029c0: 7874 203d 2061 7761 6974 2072 6573 706f  xt = await respo
+000029d0: 6e73 652e 7465 7874 2829 0d0a 2020 2020  nse.text()..    
+000029e0: 2020 2020 7072 696e 7428 7465 7874 290d      print(text).
+000029f0: 0a0d 0a0d 0a61 7379 6e63 696f 2e72 756e  .....asyncio.run
+00002a00: 2863 6c69 656e 745f 6578 616d 706c 6528  (client_example(
+00002a10: 2929 0d0a 6060 600d 0a0d 0a23 2320 5375  ))..```....## Su
+00002a20: 7070 6f72 7465 6420 706c 6174 666f 726d  pported platform
+00002a30: 7320 616e 6420 7275 6e74 696d 6573 0d0a  s and runtimes..
+00002a40: 2a20 5079 7468 6f6e 3a20 616c 6c20 7665  * Python: all ve
+00002a50: 7273 696f 6e73 2069 6e63 6c75 6465 6420  rsions included 
+00002a60: 696e 2074 6865 2062 7569 6c64 206d 6174  in the build mat
+00002a70: 7269 780d 0a2a 2055 6275 6e74 750d 0a2a  rix..* Ubuntu..*
+00002a80: 2057 696e 646f 7773 2031 300d 0a2a 206d   Windows 10..* m
+00002a90: 6163 4f53 0d0a 0d0a 2323 2044 6f63 756d  acOS....## Docum
+00002aa0: 656e 7461 7469 6f6e 0d0a 506c 6561 7365  entation..Please
+00002ab0: 2072 6566 6572 2074 6f20 7468 6520 5b64   refer to the [d
+00002ac0: 6f63 756d 656e 7461 7469 6f6e 2077 6562  ocumentation web
+00002ad0: 7369 7465 5d28 6874 7470 733a 2f2f 7777  site](https://ww
+00002ae0: 772e 6e65 6f74 6572 6f69 2e64 6576 2f62  w.neoteroi.dev/b
+00002af0: 6c61 636b 7368 6565 702f 292e 0d0a 0d0a  lacksheep/).....
+00002b00: 2323 2043 6f6d 6d75 6e69 6361 7469 6f6e  ## Communication
+00002b10: 0d0a 5b42 6c61 636b 5368 6565 7020 636f  ..[BlackSheep co
+00002b20: 6d6d 756e 6974 7920 696e 2047 6974 7465  mmunity in Gitte
+00002b30: 725d 2868 7474 7073 3a2f 2f67 6974 7465  r](https://gitte
+00002b40: 722e 696d 2f4e 656f 7465 726f 692f 426c  r.im/Neoteroi/Bl
+00002b50: 6163 6b53 6865 6570 292e 0d0a 0d0a 2323  ackSheep).....##
+00002b60: 2042 7261 6e63 6865 730d 0a54 6865 205f   Branches..The _
+00002b70: 6d61 696e 5f20 6272 616e 6368 2063 6f6e  main_ branch con
+00002b80: 7461 696e 7320 7468 6520 6375 7272 656e  tains the curren
+00002b90: 746c 7920 6465 7665 6c6f 7065 6420 7665  tly developed ve
+00002ba0: 7273 696f 6e2c 2077 6869 6368 2069 7320  rsion, which is 
+00002bb0: 7665 7273 696f 6e20 320d 0a61 6c70 6861  version 2..alpha
+00002bc0: 2e20 5468 6520 5f76 315f 2062 7261 6e63  . The _v1_ branc
+00002bd0: 6820 636f 6e74 6169 6e73 2076 6572 7369  h contains versi
+00002be0: 6f6e 2031 206f 6620 7468 6520 7765 6220  on 1 of the web 
+00002bf0: 6672 616d 6577 6f72 6b2c 2066 6f72 2062  framework, for b
+00002c00: 7567 7320 6669 7865 730d 0a61 6e64 206d  ugs fixes..and m
+00002c10: 6169 6e74 656e 616e 6365 2e0d 0a         aintenance...
```

### Comparing `blacksheep-2.0a8/blacksheep.egg-info/SOURCES.txt` & `blacksheep-2.0a9/blacksheep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/pyproject.toml` & `blacksheep-2.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/setup.py` & `blacksheep-2.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_application.py` & `blacksheep-2.0a9/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_auth.py` & `blacksheep-2.0a9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_auth_cookie.py` & `blacksheep-2.0a9/tests/test_auth_cookie.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_bindings.py` & `blacksheep-2.0a9/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_caching.py` & `blacksheep-2.0a9/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_contents.py` & `blacksheep-2.0a9/tests/test_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import List
 
 import pytest
 
-from blacksheep import JSONContent, Request, StreamedContent
+from blacksheep import JSONContent, Request
 from blacksheep.contents import (
     FormPart,
     HTMLContent,
     MultiPartFormData,
+    StreamedContent,
     TextContent,
     parse_www_form,
     write_www_form_urlencoded,
 )
 from blacksheep.multipart import (
     get_boundary_from_header,
     parse_content_disposition_values,
@@ -319,7 +320,15 @@
 async def test_write_request_body_only(req: Request, expected_chunks: List[bytes]):
     received_chunks = []
 
     async for chunk in write_request_body_only(req):
         received_chunks.append(chunk)
 
     assert received_chunks == expected_chunks
+
+
+@pytest.mark.parametrize("size", [0, 2000, 2147483647, 9e18])
+def test_content_size(size):
+    async def gen():
+        yield b""
+
+    StreamedContent(b"text/plain", gen, size)
```

### Comparing `blacksheep-2.0a8/tests/test_controllers.py` & `blacksheep-2.0a9/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_cookies.py` & `blacksheep-2.0a9/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_cors.py` & `blacksheep-2.0a9/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_csrf.py` & `blacksheep-2.0a9/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_dataprotection.py` & `blacksheep-2.0a9/tests/test_dataprotection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_files_handler.py` & `blacksheep-2.0a9/tests/test_files_handler.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_files_serving.py` & `blacksheep-2.0a9/tests/test_files_serving.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_forwarding.py` & `blacksheep-2.0a9/tests/test_forwarding.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_gzip.py` & `blacksheep-2.0a9/tests/test_gzip.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_headers.py` & `blacksheep-2.0a9/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_multipart.py` & `blacksheep-2.0a9/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_normalization.py` & `blacksheep-2.0a9/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_openapi_docstrings.py` & `blacksheep-2.0a9/tests/test_openapi_docstrings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_openapi_v3.py` & `blacksheep-2.0a9/tests/test_openapi_v3.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_pathutils.py` & `blacksheep-2.0a9/tests/test_pathutils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_ranges.py` & `blacksheep-2.0a9/tests/test_ranges.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_requests.py` & `blacksheep-2.0a9/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_responses.py` & `blacksheep-2.0a9/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_router.py` & `blacksheep-2.0a9/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_sessions.py` & `blacksheep-2.0a9/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_templating.py` & `blacksheep-2.0a9/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_testing.py` & `blacksheep-2.0a9/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_url.py` & `blacksheep-2.0a9/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_utils.py` & `blacksheep-2.0a9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a8/tests/test_websocket.py` & `blacksheep-2.0a9/tests/test_websocket.py`

 * *Files identical despite different names*

