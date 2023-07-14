# Comparing `tmp/aiohttp_client_cache-0.8.1.tar.gz` & `tmp/aiohttp_client_cache-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_client_cache-0.8.1.tar", max compression
+gzip compressed data, was "aiohttp_client_cache-0.8.2.tar", max compression
```

## Comparing `aiohttp_client_cache-0.8.1.tar` & `aiohttp_client_cache-0.8.2.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0      247 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/.readthedocs.yml
--rw-r--r--   0        0        0     4628 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      992 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/CONTRIBUTORS.md
--rw-r--r--   0        0        0     6143 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/HISTORY.md
--rw-r--r--   0        0        0     1068 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/LICENSE
--rw-r--r--   0        0        0     1322 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/LICENSE_requests_cache.md
--rw-r--r--   0        0        0     4915 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/README.md
--rw-r--r--   0        0        0      297 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/__init__.py
--rw-r--r--   0        0        0     1858 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/__init__.py
--rw-r--r--   0        0        0    15142 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/base.py
--rw-r--r--   0        0        0     6672 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/dynamodb.py
--rw-r--r--   0        0        0     3872 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/filesystem.py
--rw-r--r--   0        0        0     3690 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/mongodb.py
--rw-r--r--   0        0        0     4148 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/redis.py
--rw-r--r--   0        0        0     8151 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/sqlite.py
--rw-r--r--   0        0        0     8913 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/cache_control.py
--rw-r--r--   0        0        0     2698 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/cache_keys.py
--rw-r--r--   0        0        0        0 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/py.typed
--rw-r--r--   0        0        0     9364 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/response.py
--rw-r--r--   0        0        0     3981 2023-01-05 17:44:56.166088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/session.py
--rw-r--r--   0        0        0    11235 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/aiohttp_client_cache/signatures.py
--rw-r--r--   0        0        0      889 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docker-compose.yml
--rw-r--r--   0        0        0      176 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/Dockerfile
--rw-r--r--   0        0        0      343 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/_static/collapsible_container.css
--rw-r--r--   0        0        0      401 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/_static/collapsible_container.js
--rw-r--r--   0        0        0      441 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/_static/table.css
--rw-r--r--   0        0        0      303 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/_templates/module.rst_t
--rw-r--r--   0        0        0      357 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/aiohttp_client_cache.session.md
--rw-r--r--   0        0        0     3460 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/backends.md
--rw-r--r--   0        0        0     4305 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/conf.py
--rw-r--r--   0        0        0       52 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/contributing.md
--rw-r--r--   0        0        0       36 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/contributors.md
--rw-r--r--   0        0        0      275 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/docker-compose.yml
--rw-r--r--   0        0        0      878 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/examples.md
--rw-r--r--   0        0        0       31 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/history.md
--rw-r--r--   0        0        0      233 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/index.md
--rw-r--r--   0        0        0      577 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/reference.md
--rw-r--r--   0        0        0      699 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/related_projects.md
--rw-r--r--   0        0        0     2492 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/security.md
--rw-r--r--   0        0        0    11466 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/docs/user_guide.md
--rw-r--r--   0        0        0      240 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/examples/README.md
--rw-r--r--   0        0        0     1714 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/examples/log_requests.py
--rw-r--r--   0        0        0     2598 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/examples/precache.py
--rw-r--r--   0        0        0     1392 2023-01-05 17:44:56.170088 aiohttp_client_cache-0.8.1/examples/url_patterns.py
--rw-r--r--   0        0        0     3849 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/__init__.py
--rw-r--r--   0        0        0     2299 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/conftest.py
--rw-r--r--   0        0        0      147 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/__init__.py
--rw-r--r--   0        0        0    12677 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/base_backend_test.py
--rw-r--r--   0        0        0     3751 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/base_storage_test.py
--rw-r--r--   0        0        0      172 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/test_dict.py
--rw-r--r--   0        0        0     1427 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/test_dynamodb.py
--rw-r--r--   0        0        0     1776 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/test_filesystem.py
--rw-r--r--   0        0        0     1461 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/test_mongodb.py
--rw-r--r--   0        0        0     1024 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/test_redis.py
--rw-r--r--   0        0        0     5495 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/integration/test_sqlite.py
--rw-r--r--   0        0        0        0 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/unit/__init__.py
--rw-r--r--   0        0        0     9151 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/unit/test_base_backend.py
--rw-r--r--   0        0        0     7180 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/unit/test_cache_control.py
--rw-r--r--   0        0        0     2508 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/unit/test_cache_keys.py
--rw-r--r--   0        0        0     7083 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/unit/test_response.py
--rw-r--r--   0        0        0     4658 2023-01-05 17:44:56.174088 aiohttp_client_cache-0.8.1/test/unit/test_session.py
--rw-r--r--   0        0        0     6618 1970-01-01 00:00:00.000000 aiohttp_client_cache-0.8.1/setup.py
--rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 aiohttp_client_cache-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/.readthedocs.yml
+-rw-r--r--   0        0        0     4628 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      992 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     6409 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/HISTORY.md
+-rw-r--r--   0        0        0     1068 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1322 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/LICENSE_requests_cache.md
+-rw-r--r--   0        0        0     4581 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/README.md
+-rw-r--r--   0        0        0      297 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/__init__.py
+-rw-r--r--   0        0        0     1858 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/__init__.py
+-rw-r--r--   0        0        0    15302 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/base.py
+-rw-r--r--   0        0        0     6687 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/dynamodb.py
+-rw-r--r--   0        0        0     3878 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/filesystem.py
+-rw-r--r--   0        0        0     3971 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/mongodb.py
+-rw-r--r--   0        0        0     4177 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/redis.py
+-rw-r--r--   0        0        0     8166 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/sqlite.py
+-rw-r--r--   0        0        0     8913 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/cache_control.py
+-rw-r--r--   0        0        0     2698 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/cache_keys.py
+-rw-r--r--   0        0        0        0 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/py.typed
+-rw-r--r--   0        0        0     9358 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/response.py
+-rw-r--r--   0        0        0     3948 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/session.py
+-rw-r--r--   0        0        0    11235 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/aiohttp_client_cache/signatures.py
+-rw-r--r--   0        0        0      988 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docker-compose.yml
+-rw-r--r--   0        0        0      176 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docs/Dockerfile
+-rw-r--r--   0        0        0      343 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docs/_static/collapsible_container.css
+-rw-r--r--   0        0        0      401 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docs/_static/collapsible_container.js
+-rw-r--r--   0        0        0      441 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docs/_static/table.css
+-rw-r--r--   0        0        0      303 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docs/_templates/module.rst_t
+-rw-r--r--   0        0        0      357 2023-07-14 19:33:54.809228 aiohttp_client_cache-0.8.2/docs/aiohttp_client_cache.session.md
+-rw-r--r--   0        0        0     3460 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/backends.md
+-rw-r--r--   0        0        0     4305 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/conf.py
+-rw-r--r--   0        0        0       52 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/contributing.md
+-rw-r--r--   0        0        0       36 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/contributors.md
+-rw-r--r--   0        0        0      275 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/docker-compose.yml
+-rw-r--r--   0        0        0      878 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/examples.md
+-rw-r--r--   0        0        0       31 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/history.md
+-rw-r--r--   0        0        0      233 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/index.md
+-rw-r--r--   0        0        0      577 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/reference.md
+-rw-r--r--   0        0        0      699 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/related_projects.md
+-rw-r--r--   0        0        0     2492 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/security.md
+-rw-r--r--   0        0        0    11466 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/docs/user_guide.md
+-rw-r--r--   0        0        0      240 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/examples/README.md
+-rw-r--r--   0        0        0     1714 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/examples/log_requests.py
+-rw-r--r--   0        0        0     2598 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/examples/precache.py
+-rw-r--r--   0        0        0     1392 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/examples/url_patterns.py
+-rw-r--r--   0        0        0     4320 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/__init__.py
+-rw-r--r--   0        0        0     2299 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/conftest.py
+-rw-r--r--   0        0        0      147 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/__init__.py
+-rw-r--r--   0        0        0    12675 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/base_backend_test.py
+-rw-r--r--   0        0        0     3751 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/base_storage_test.py
+-rw-r--r--   0        0        0      172 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/test_dict.py
+-rw-r--r--   0        0        0     1213 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/test_dynamodb.py
+-rw-r--r--   0        0        0     1776 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/test_filesystem.py
+-rw-r--r--   0        0        0     1761 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/test_mongodb.py
+-rw-r--r--   0        0        0     1024 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/test_redis.py
+-rw-r--r--   0        0        0     5495 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/integration/test_sqlite.py
+-rw-r--r--   0        0        0        0 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/unit/__init__.py
+-rw-r--r--   0        0        0     9151 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/unit/test_base_backend.py
+-rw-r--r--   0        0        0     7180 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/unit/test_cache_control.py
+-rw-r--r--   0        0        0     2508 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/unit/test_cache_keys.py
+-rw-r--r--   0        0        0     7077 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/unit/test_response.py
+-rw-r--r--   0        0        0     4658 2023-07-14 19:33:54.813228 aiohttp_client_cache-0.8.2/test/unit/test_session.py
+-rw-r--r--   0        0        0     7423 1970-01-01 00:00:00.000000 aiohttp_client_cache-0.8.2/PKG-INFO
```

### Comparing `aiohttp_client_cache-0.8.1/CONTRIBUTING.md` & `aiohttp_client_cache-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/CONTRIBUTORS.md` & `aiohttp_client_cache-0.8.2/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/HISTORY.md` & `aiohttp_client_cache-0.8.2/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.8.2 (2023-07-14)
+* Add some missing type annotations to backend classes
+* Fix passing connection parameters to MongoDB backend
+* Revert closing backend connections on session context exit
+* Fix `CachedResponse.close()` method to match `ClientResponse.close()`
+
 ## 0.8.1 (2023-01-05)
 * For SQLite backend, close database connection on `ClientSession` context exit
 
 ## 0.8.0 (2022-12-29)
 * Lazily initialize and reuse SQLite connection objects
 * Fix `AttributeError` when using a response cached with an older version of `attrs`
 * Fix concurrent usage of `SQLiteCache.bulk_commit()`
```

### Comparing `aiohttp_client_cache-0.8.1/LICENSE` & `aiohttp_client_cache-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/LICENSE_requests_cache.md` & `aiohttp_client_cache-0.8.2/LICENSE_requests_cache.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/README.md` & `aiohttp_client_cache-0.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,14 @@
 * **Customization:** Works out of the box with little to no config, but with plenty of options
   available for customizing cache
   [expiration](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html#cache-expiration)
   and other [behavior](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html#cache-options)
 * **Persistence:** Includes several [storage backends](https://aiohttp-client-cache.readthedocs.io/en/latest/backends.html):
   SQLite, DynamoDB, MongoDB, and Redis.
 
-# Development Status
-**This library is a work in progress!**
-
-Breaking changes should be expected until a `1.0` release, so version pinning is recommended.
-
-My goal for this library is to eventually have a similar (but not identical) feature set as
-`requests-cache`, and also contribute new features from this library back to `requests-cache`.
-If there is a feature you want, if you've discovered a bug, or if you have other general feedback, please
-[create an issue](https://github.com/requests-cache/aiohttp-client-cache/issues/new/choose) for it!
-
 # Quickstart
 First, install with pip (python 3.7+ required):
 ```bash
 pip install aiohttp-client-cache
 ```
 
 ## Basic Usage
@@ -83,7 +73,11 @@
 
 # More Info
 To learn more, see:
 * [User Guide](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html)
 * [Cache Backends](https://aiohttp-client-cache.readthedocs.io/en/latest/backends.html)
 * [API Reference](https://aiohttp-client-cache.readthedocs.io/en/latest/reference.html)
 * [Examples](https://aiohttp-client-cache.readthedocs.io/en/latest/examples.html)
+
+# Feedback
+If there is a feature you want, if you've discovered a bug, or if you have other general feedback, please
+[create an issue](https://github.com/requests-cache/aiohttp-client-cache/issues/new/choose) for it!
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/__init__.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/base.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import inspect
 import pickle
 from abc import ABCMeta, abstractmethod
 from collections import UserDict
 from datetime import datetime
 from logging import getLogger
-from typing import AsyncIterable, Callable, Iterable, Optional, Tuple, Union
+from typing import Any, AsyncIterable, Awaitable, Callable, Iterable, Optional, Tuple, Union
 
 from aiohttp import ClientResponse
 from aiohttp.typedefs import StrOrURL
 
 from aiohttp_client_cache.cache_control import CacheActions, ExpirationPatterns, ExpirationTime
 from aiohttp_client_cache.cache_keys import create_key
 from aiohttp_client_cache.response import AnyResponse, CachedResponse
 from aiohttp_client_cache.signatures import extend_init_signature
 
 ResponseOrKey = Union[CachedResponse, bytes, str, None]
+_FilterFn = Union[
+    Callable[[AnyResponse], bool],
+    Callable[[AnyResponse], Awaitable[bool]],
+]
+
 logger = getLogger(__name__)
 
 
 class CacheBackend:
     """Base class for cache backends; includes a non-persistent, in-memory cache.
 
     This manages higher-level cache operations, including cache expiration, generating cache keys,
@@ -31,21 +36,21 @@
     """
 
     def __init__(
         self,
         cache_name: str = 'aiohttp-cache',
         expire_after: ExpirationTime = -1,
         urls_expire_after: Optional[ExpirationPatterns] = None,
-        allowed_codes: tuple = (200,),
-        allowed_methods: tuple = ('GET', 'HEAD'),
+        allowed_codes: Tuple[int, ...] = (200,),
+        allowed_methods: Tuple[str, ...] = ('GET', 'HEAD'),
         include_headers: bool = False,
-        ignored_params: Optional[Iterable] = None,
+        ignored_params: Optional[Iterable[str]] = None,
         cache_control: bool = False,
-        filter_fn: Callable = lambda r: True,
-        **kwargs,
+        filter_fn: _FilterFn = lambda r: True,
+        **kwargs: Any,
     ):
         """
         Args:
             cache_name: Cache prefix or namespace, depending on backend
             expire_after: Time after which a cache entry will be expired; see
                 :ref:`user_guide:cache expiration` for possible formats
             urls_expire_after: Expiration times to apply for different URL patterns
@@ -213,25 +218,25 @@
             response = await self.responses.read(key)
             if response and response.is_expired or not self.filter_fn(response):
                 keys_to_delete.add(key)
 
         logger.debug(f'Deleting {len(keys_to_delete)} expired cache entries')
         await self.bulk_delete(keys_to_delete)
 
-    def create_key(self, method: str, url: StrOrURL, **kwargs):
+    def create_key(self, method: str, url: StrOrURL, **kwargs: Any):
         """Create a unique cache key based on request details"""
         return create_key(
             method,
             url,
             include_headers=self.include_headers,
             ignored_params=self.ignored_params,
             **kwargs,
         )
 
-    async def delete_url(self, url: StrOrURL, method: str = 'GET', **kwargs):
+    async def delete_url(self, url: StrOrURL, method: str = 'GET', **kwargs: Any):
         """Delete cached response associated with `url`, along with its history (if applicable)"""
         key = self.create_key(url=url, method=method, **kwargs)
         await self.delete(key)
 
     async def has_url(self, url: StrOrURL, method: str = 'GET', **kwargs) -> bool:
         """Returns `True` if cache has `url`, `False` otherwise"""
         key = self.create_key(method=method, url=url, **kwargs)
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/dynamodb.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from contextlib import asynccontextmanager
-from typing import AsyncIterable, Dict
+from typing import Any, AsyncIterable, Dict
 
 import aioboto3
 from aioboto3.session import ResourceCreatorContext
 from aioboto3.session import Session as AWSSession
 from botocore.exceptions import ClientError
 
 from aiohttp_client_cache.backends import BaseCache, CacheBackend, ResponseOrKey, get_valid_kwargs
@@ -23,15 +23,15 @@
     def __init__(
         self,
         cache_name: str = 'aiohttp-cache',
         key_attr_name: str = 'k',
         val_attr_name: str = 'v',
         create_if_not_exists: bool = False,
         context: ResourceCreatorContext = None,
-        **kwargs,
+        **kwargs: Any,
     ):
         """
         Args:
             cache_name: Table name to use
             key_attr_name: The name of the field to use for keys in the DynamoDB document
             val_attr_name: The name of the field to use for values in the DynamoDB document
             create_if_not_exists: Whether or not to attempt to create the DynamoDB table
@@ -70,15 +70,15 @@
         self,
         table_name: str,
         namespace: str,
         key_attr_name: str = 'k',
         val_attr_name: str = 'v',
         create_if_not_exists: bool = False,
         context: ResourceCreatorContext = None,
-        **kwargs,
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.table_name = table_name
         self.namespace = namespace
         self.key_attr_name = key_attr_name
         self.val_attr_name = val_attr_name
         self.create_if_not_exists = create_if_not_exists
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/filesystem.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/filesystem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import contextmanager
 from os import listdir, makedirs
 from os.path import abspath, dirname, expanduser, isabs, isfile, join
 from pathlib import Path
 from pickle import PickleError
 from shutil import rmtree
 from tempfile import gettempdir
-from typing import AsyncIterable, Union
+from typing import Any, AsyncIterable, Union
 
 import aiofiles
 import aiofiles.os
 
 from aiohttp_client_cache.backends import BaseCache, CacheBackend, ResponseOrKey
 from aiohttp_client_cache.backends.sqlite import SQLiteCache
 
@@ -22,35 +22,35 @@
     Args:
         cache_name: Base directory for cache files
         use_temp: Store cache files in a temp directory (e.g., ``/tmp/http_cache/``).
             Note: if ``cache_name`` is an absolute path, this option will be ignored.
     """
 
     def __init__(
-        self, cache_name: Union[Path, str] = 'http_cache', use_temp: bool = False, **kwargs
+        self, cache_name: Union[Path, str] = 'http_cache', use_temp: bool = False, **kwargs: Any
     ):
         super().__init__(**kwargs)
         self.responses = FileCache(cache_name, use_temp=use_temp, **kwargs)
         db_path = join(dirname(self.responses.cache_dir), 'redirects.sqlite')
         self.redirects = SQLiteCache(db_path, 'redirects', **kwargs)
 
 
 class FileCache(BaseCache):
     """A dictionary-like interface to files on the local filesystem"""
 
-    def __init__(self, cache_name, use_temp: bool = False, **kwargs):
+    def __init__(self, cache_name, use_temp: bool = False, **kwargs: Any):
         super().__init__(**kwargs)
         self.cache_dir = _get_cache_dir(cache_name, use_temp)
 
     @contextmanager
     def _try_io(self, ignore_errors: bool = True):
         """Attempt an I/O operation, and either ignore errors or re-raise them as KeyErrors"""
         try:
             yield
-        except (IOError, OSError, PickleError):
+        except (OSError, PickleError):
             if not ignore_errors:
                 raise
 
     def _join(self, key):
         return join(self.cache_dir, str(key))
 
     async def clear(self):
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/mongodb.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/mongodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from typing import AsyncIterable
+from typing import Any, AsyncIterable
 
 from motor.motor_asyncio import AsyncIOMotorClient
+from pymongo import MongoClient
 
 from aiohttp_client_cache.backends import BaseCache, CacheBackend, ResponseOrKey, get_valid_kwargs
 from aiohttp_client_cache.signatures import extend_init_signature, mongo_template
 
 
 @extend_init_signature(CacheBackend, mongo_template)
 class MongoDBBackend(CacheBackend):
     """Async cache backend for `MongoDB <https://www.mongodb.com>`_
     (requires `motor <https://motor.readthedocs.io>`_)
     """
 
     def __init__(
-        self, cache_name: str = 'aiohttp-cache', connection: AsyncIOMotorClient = None, **kwargs
+        self,
+        cache_name: str = 'aiohttp-cache',
+        connection: AsyncIOMotorClient = None,
+        **kwargs: Any
     ):
         """
         Args:
             cache_name: Database name
             connection: Optional client object to use instead of creating a new one
         """
         super().__init__(cache_name=cache_name, **kwargs)
@@ -32,18 +36,27 @@
         db_name: database name (be careful with production databases)
         collection_name: collection name
         connection: MongoDB connection instance to use instead of creating a new one
         kwargs: Additional keyword args for :py:class:`~motor.motor_asyncio.AsyncIOMotorClient`
     """
 
     def __init__(
-        self, db_name: str, collection_name: str, connection: AsyncIOMotorClient = None, **kwargs
+        self,
+        db_name: str,
+        collection_name: str,
+        connection: AsyncIOMotorClient = None,
+        **kwargs: Any
     ):
         super().__init__(**kwargs)
-        connection_kwargs = get_valid_kwargs(AsyncIOMotorClient.__init__, kwargs)
+
+        # Motor accepts the same arguments as pymongo, plus one additional argument
+        connection_kwargs = get_valid_kwargs(MongoClient.__init__, kwargs)
+        if kwargs.get('io_loop'):
+            connection_kwargs['io_loop'] = kwargs.pop('io_loop')
+
         self.connection = connection or AsyncIOMotorClient(**connection_kwargs)
         self.db = self.connection[db_name]
         self.collection = self.db[collection_name]
 
     async def clear(self):
         await self.collection.drop()
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/redis.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterable, Optional
+from typing import Any, AsyncIterable, Optional
 
 from redis.asyncio import Connection, Redis, from_url
 
 from aiohttp_client_cache.backends import BaseCache, CacheBackend, ResponseOrKey, get_valid_kwargs
 from aiohttp_client_cache.signatures import extend_init_signature, redis_template
 
 DEFAULT_ADDRESS = 'redis://localhost'
@@ -10,15 +10,17 @@
 
 @extend_init_signature(CacheBackend, redis_template)
 class RedisBackend(CacheBackend):
     """Async cache backend for `Redis <https://redis.io>`_
     (requires `redis-py <https://redis-py.readthedocs.io>`_)
     """
 
-    def __init__(self, cache_name: str = 'aiohttp-cache', address: str = DEFAULT_ADDRESS, **kwargs):
+    def __init__(
+        self, cache_name: str = 'aiohttp-cache', address: str = DEFAULT_ADDRESS, **kwargs: Any
+    ):
         """
         Args:
             cache_name: Used as a namespace (prefix for hash key)
             address: Redis server URI
         """
         super().__init__(cache_name=cache_name, **kwargs)
         self.responses = RedisCache(cache_name, 'responses', address=address, **kwargs)
@@ -45,15 +47,15 @@
 
     def __init__(
         self,
         namespace: str,
         collection_name: str,
         address: str = DEFAULT_ADDRESS,
         connection: Optional[Redis] = None,
-        **kwargs,
+        **kwargs: Any,
     ):
         # Pop off BaseCache kwargs and use the rest as Redis connection kwargs
         super().__init__(**kwargs)
         self.address = address
         self._connection = connection
         self.connection_kwargs = get_valid_kwargs(Connection.__init__, kwargs)
         self.hash_key = f'{namespace}:{collection_name}'
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/backends/sqlite.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/backends/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sqlite3
 from contextlib import asynccontextmanager
 from contextvars import ContextVar
 from os import makedirs
 from os.path import abspath, basename, dirname, expanduser, isabs, join
 from pathlib import Path
 from tempfile import gettempdir
-from typing import AsyncIterable, AsyncIterator, Optional, Union
+from typing import Any, AsyncIterable, AsyncIterator, Optional, Union
 
 import aiosqlite
 
 from aiohttp_client_cache.backends import BaseCache, CacheBackend, ResponseOrKey, get_valid_kwargs
 from aiohttp_client_cache.signatures import extend_init_signature, sqlite_template
 
 bulk_commit_var: ContextVar[bool] = ContextVar('bulk_commit', default=False)
@@ -33,15 +33,15 @@
     """
 
     def __init__(
         self,
         cache_name: str = 'aiohttp-cache',
         use_temp: bool = False,
         fast_save: bool = False,
-        **kwargs,
+        **kwargs: Any,
     ):
         super().__init__(cache_name=cache_name, **kwargs)
         self.responses = SQLitePickleCache(
             cache_name, 'responses', use_temp=use_temp, fast_save=fast_save, **kwargs
         )
         self.redirects = SQLiteCache(cache_name, 'redirects', use_temp=use_temp, **kwargs)
 
@@ -65,15 +65,15 @@
 
     def __init__(
         self,
         filename: str,
         table_name: str = 'aiohttp-cache',
         use_temp: bool = False,
         fast_save: bool = False,
-        **kwargs,
+        **kwargs: Any,
     ):
         super().__init__(**kwargs)
         self.connection_kwargs = get_valid_kwargs(sqlite_template, kwargs)
         self.fast_save = fast_save
         self.filename = _get_cache_filename(filename, use_temp)
         self.table_name = table_name
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/cache_control.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/cache_control.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/cache_keys.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/cache_keys.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/response.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     @property
     def connection(self):
         return None
 
     async def __aenter__(self) -> 'CachedResponse':
         return self
 
-    async def close(self):
+    def close(self):
         pass
 
     async def wait_for_close(self):
         pass
 
     def release(self):
         pass
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/session.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
             if await self.cache.is_cacheable(new_response, actions):
                 await self.cache.save_response(new_response, actions.key, actions.expires)
             return set_response_defaults(new_response)
 
     async def close(self):
         """Close both aiohttp connector and any backend connection(s) on contextmanager exit"""
         await super().close()
-        await self.cache.close()
 
     @asynccontextmanager
     async def disabled(self):
         """Temporarily disable the cache
 
         Example:
```

### Comparing `aiohttp_client_cache-0.8.1/aiohttp_client_cache/signatures.py` & `aiohttp_client_cache-0.8.2/aiohttp_client_cache/signatures.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docker-compose.yml` & `aiohttp_client_cache-0.8.2/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,17 @@
   dynamodb:
     image: amazon/dynamodb-local
     hostname: dynamodb-local
     container_name: dynamodb-local
     ports:
       - 8000:8000
     command: '-jar DynamoDBLocal.jar -inMemory'
+    environment:
+      AWS_ACCESS_KEY_ID: 'placeholder'
+      AWS_SECRET_ACCESS_KEY: 'placeholder'
     working_dir: /home/dynamodblocal
 
   mongo:
     image: mongo
     container_name: mongo
     environment:
       MONGO_INITDB_DATABASE: aiohttp_client_cache_pytest
```

### Comparing `aiohttp_client_cache-0.8.1/docs/backends.md` & `aiohttp_client_cache-0.8.2/docs/backends.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docs/conf.py` & `aiohttp_client_cache-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docs/examples.md` & `aiohttp_client_cache-0.8.2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docs/reference.md` & `aiohttp_client_cache-0.8.2/docs/reference.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docs/related_projects.md` & `aiohttp_client_cache-0.8.2/docs/related_projects.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docs/security.md` & `aiohttp_client_cache-0.8.2/docs/security.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/docs/user_guide.md` & `aiohttp_client_cache-0.8.2/docs/user_guide.md`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/examples/log_requests.py` & `aiohttp_client_cache-0.8.2/examples/log_requests.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/examples/precache.py` & `aiohttp_client_cache-0.8.2/examples/precache.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/examples/url_patterns.py` & `aiohttp_client_cache-0.8.2/examples/url_patterns.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/conftest.py` & `aiohttp_client_cache-0.8.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/integration/base_backend_test.py` & `aiohttp_client_cache-0.8.2/test/integration/base_backend_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
             await asyncio.sleep(1)
             response = await session.get(httpbin('get'), expire_after=1)
             print(response.expires)
             assert response.from_cache is False
 
     async def test_delete_expired_responses(self):
         async with self.init_session(expire_after=1) as session:
-
             # Populate the cache with several responses that should expire immediately
             for response_format in HTTPBIN_FORMATS:
                 await session.get(httpbin(response_format))
             await session.get(httpbin('redirect/1'))
             await asyncio.sleep(1)
 
             # Cache a response and some redirects, which should be the only non-expired cache items
@@ -238,15 +237,14 @@
             await session.get(httpbin('cache/0'))
             response = await session.get(httpbin('cache/0'))
 
             assert response.from_cache is False
             assert await session.cache.responses.size() == 0
 
     async def test_cookies_with_redirect(self):
-
         async with self.init_session(cache_control=True) as session:
             await session.get(httpbin('cookies/set?test_cookie=value'))
             session.cookie_jar.clear()
             await session.get(httpbin('cookies/set?test_cookie=value'))
 
         cookies = session.cookie_jar.filter_cookies(httpbin())
         assert cookies['test_cookie'].value == 'value'
```

### Comparing `aiohttp_client_cache-0.8.1/test/integration/base_storage_test.py` & `aiohttp_client_cache-0.8.2/test/integration/base_storage_test.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/integration/test_dynamodb.py` & `aiohttp_client_cache-0.8.2/test/integration/test_dynamodb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-import asyncio
 from typing import Any, Dict
 
-import aioboto3
 import pytest
 
 from aiohttp_client_cache.backends.dynamodb import DynamoDBBackend, DynamoDbCache
 from test.integration import BaseBackendTest, BaseStorageTest
 
-resource_kwargs = {
-    'region_name': 'region',
-    'aws_access_key_id': 'access_key_id',
-    'aws_secret_access_key': 'secret_access_key',
+AWS_OPTIONS = {
     'endpoint_url': 'http://localhost:8000',
+    'region_name': 'us-east-1',
+    'aws_access_key_id': 'placeholder',
+    'aws_secret_access_key': 'placeholder',
 }
 
 
 def is_dynamodb_running():
     """Test if a DynamoDB service is running locally"""
-
-    async def check_dynamodb():
-        session = aioboto3.Session()
-        async with session.resource('dynamodb', **resource_kwargs) as resource:
-            client = resource.meta.client
-            await client.describe_limits()
+    import boto3
 
     try:
-        asyncio.run(check_dynamodb())
+        client = boto3.client('dynamodb', **AWS_OPTIONS)
+        client.describe_limits()
         return True
     except OSError:
         return False
 
 
 pytestmark = [
     pytest.mark.asyncio,
@@ -42,14 +36,14 @@
 class TestDynamoDbCache(BaseStorageTest):
     storage_class = DynamoDbCache
     picklable = True
     init_kwargs = {
         'create_if_not_exists': True,
         'key_attr_name': 'k',
         'val_attr_name': 'v',
-        **resource_kwargs,
+        **AWS_OPTIONS,
     }
 
 
 class TestDynamoDBBackend(BaseBackendTest):
     backend_class = DynamoDBBackend
-    init_kwargs: Dict[str, Any] = {'create_if_not_exists': True, **resource_kwargs}
+    init_kwargs: Dict[str, Any] = {'create_if_not_exists': True, **AWS_OPTIONS}
```

### Comparing `aiohttp_client_cache-0.8.1/test/integration/test_filesystem.py` & `aiohttp_client_cache-0.8.2/test/integration/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/integration/test_redis.py` & `aiohttp_client_cache-0.8.2/test/integration/test_redis.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/integration/test_sqlite.py` & `aiohttp_client_cache-0.8.2/test/integration/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/unit/test_base_backend.py` & `aiohttp_client_cache-0.8.2/test/unit/test_base_backend.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/unit/test_cache_control.py` & `aiohttp_client_cache-0.8.2/test/unit/test_cache_control.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/unit/test_cache_keys.py` & `aiohttp_client_cache-0.8.2/test/unit/test_cache_keys.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/test/unit/test_response.py` & `aiohttp_client_cache-0.8.2/test/unit/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,12 +191,12 @@
 
 async def test_no_ops(aiohttp_client):
     # Just make sure CachedResponse doesn't explode if extra ClientResponse methods are called
     response = await get_test_response(aiohttp_client)
 
     await response.start()
     response.release()
-    await response.close()
+    response.close()
     await response.wait_for_close()
     await response.terminate()
     assert response.connection is None
     assert response._released is True
```

### Comparing `aiohttp_client_cache-0.8.1/test/unit/test_session.py` & `aiohttp_client_cache-0.8.2/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_cache-0.8.1/setup.py` & `aiohttp_client_cache-0.8.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,137 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['aiohttp_client_cache', 'aiohttp_client_cache.backends']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8,<4.0',
- 'attrs>=21.2',
- 'itsdangerous>=2.0',
- 'python-forge>=18.6,<19.0',
- 'url-normalize>=1.4,<2.0']
-
-extras_require = \
-{'all': ['aioboto3>=9.0',
-         'aiobotocore>=2.0',
-         'aiofiles>=0.6.0',
-         'aiosqlite>=0.16',
-         'motor>=3.1',
-         'redis>=4.2'],
- 'docs': ['furo>=2022.1.2',
-          'linkify-it-py>=1.0.1,<2.0.0',
-          'myst-parser>=0.15.1,<0.16.0',
-          'sphinx>=4.5.0,<5.0.0',
-          'sphinx-automodapi>=0.14',
-          'sphinx-autodoc-typehints>=1.11,<2.0',
-          'sphinx-copybutton>=0.3,<0.4',
-          'sphinxcontrib-apidoc>=0.3,<0.4'],
- 'docs:python_version >= "3.8"': ['sphinx-inline-tabs>=2022.1.2b11,<2023.0.0'],
- 'dynamodb': ['aioboto3>=9.0', 'aiobotocore>=2.0'],
- 'filesystem': ['aiofiles>=0.6.0', 'aiosqlite>=0.16'],
- 'mongodb': ['motor>=3.1'],
- 'redis': ['redis>=4.2'],
- 'sqlite': ['aiosqlite>=0.16']}
-
-setup_kwargs = {
-    'name': 'aiohttp-client-cache',
-    'version': '0.8.1',
-    'description': 'Persistent cache for aiohttp requests',
-    'long_description': "# aiohttp-client-cache\n\n[![Build status](https://github.com/requests-cache/aiohttp-client-cache/workflows/Build/badge.svg)](https://github.com/requests-cache/aiohttp-client-cache/actions)\n[![Documentation Status](https://img.shields.io/readthedocs/aiohttp-client-cache/stable?label=docs)](https://aiohttp-client-cache.readthedocs.io/en/latest/)\n[![Codecov](https://codecov.io/gh/requests-cache/aiohttp-client-cache/branch/main/graph/badge.svg?token=I6PNLYTILM)](https://codecov.io/gh/requests-cache/aiohttp-client-cache)\n[![PyPI](https://img.shields.io/pypi/v/aiohttp-client-cache?color=blue)](https://pypi.org/project/aiohttp-client-cache)\n[![Conda](https://img.shields.io/conda/vn/conda-forge/aiohttp-client-cache?color=blue)](https://anaconda.org/conda-forge/aiohttp-client-cache)\n[![PyPI - Python Versions](https://img.shields.io/pypi/pyversions/aiohttp-client-cache)](https://pypi.org/project/aiohttp-client-cache)\n[![PyPI - Format](https://img.shields.io/pypi/format/aiohttp-client-cache?color=blue)](https://pypi.org/project/aiohttp-client-cache)\n\n**aiohttp-client-cache** is an async persistent cache for [aiohttp](https://docs.aiohttp.org)\nclient requests, based on [requests-cache](https://github.com/reclosedev/requests-cache).\n\n# Features\n* **Ease of use:** Use as a [drop-in replacement](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html)\n  for `aiohttp.ClientSession`\n* **Customization:** Works out of the box with little to no config, but with plenty of options\n  available for customizing cache\n  [expiration](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html#cache-expiration)\n  and other [behavior](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html#cache-options)\n* **Persistence:** Includes several [storage backends](https://aiohttp-client-cache.readthedocs.io/en/latest/backends.html):\n  SQLite, DynamoDB, MongoDB, and Redis.\n\n# Development Status\n**This library is a work in progress!**\n\nBreaking changes should be expected until a `1.0` release, so version pinning is recommended.\n\nMy goal for this library is to eventually have a similar (but not identical) feature set as\n`requests-cache`, and also contribute new features from this library back to `requests-cache`.\nIf there is a feature you want, if you've discovered a bug, or if you have other general feedback, please\n[create an issue](https://github.com/requests-cache/aiohttp-client-cache/issues/new/choose) for it!\n\n# Quickstart\nFirst, install with pip (python 3.7+ required):\n```bash\npip install aiohttp-client-cache\n```\n\n## Basic Usage\nNext, use [aiohttp_client_cache.CachedSession](https://aiohttp-client-cache.readthedocs.io/en/latest/modules/aiohttp_client_cache.session.html#aiohttp_client_cache.session.CachedSession)\nin place of [aiohttp.ClientSession](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.ClientSession).\nTo briefly demonstrate how to use it:\n\n**Replace this:**\n```python\nfrom aiohttp import ClientSession\n\nasync with ClientSession() as session:\n    await session.get('http://httpbin.org/delay/1')\n```\n\n**With this:**\n```python\nfrom aiohttp_client_cache import CachedSession, SQLiteBackend\n\nasync with CachedSession(cache=SQLiteBackend('demo_cache')) as session:\n    await session.get('http://httpbin.org/delay/1')\n```\n\nThe URL in this example adds a delay of 1 second, simulating a slow or rate-limited website.\nWith caching, the response will be fetched once, saved to `demo_cache.sqlite`, and subsequent\nrequests will return the cached response near-instantly.\n\n## Configuration\nSeveral options are available to customize caching behavior. This example demonstrates a few of them:\n\n```python\n# fmt: off\nfrom aiohttp_client_cache import SQLiteBackend\n\ncache = SQLiteBackend(\n    cache_name='~/.cache/aiohttp-requests.db',  # For SQLite, this will be used as the filename\n    expire_after=60*60,                         # By default, cached responses expire in an hour\n    urls_expire_after={'*.fillmurray.com': -1}, # Requests for any subdomain on this site will never expire\n    allowed_codes=(200, 418),                   # Cache responses with these status codes\n    allowed_methods=['GET', 'POST'],            # Cache requests with these HTTP methods\n    include_headers=True,                       # Cache requests with different headers separately\n    ignored_params=['auth_token'],              # Keep using the cached response even if this param changes\n    timeout=2.5,                                # Connection timeout for SQLite backend\n)\n```\n\n# More Info\nTo learn more, see:\n* [User Guide](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html)\n* [Cache Backends](https://aiohttp-client-cache.readthedocs.io/en/latest/backends.html)\n* [API Reference](https://aiohttp-client-cache.readthedocs.io/en/latest/reference.html)\n* [Examples](https://aiohttp-client-cache.readthedocs.io/en/latest/examples.html)\n",
-    'author': 'Jordan Cook',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/requests-cache/aiohttp-client-cache',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: aiohttp-client-cache
+Version: 0.8.2
+Summary: Persistent cache for aiohttp requests
+Home-page: https://github.com/requests-cache/aiohttp-client-cache
+License: MIT
+Keywords: aiohttp,async,asyncio,cache,cache-backends,client,http,persistence,requests,sqlite,redis,mongodb,dynamodb
+Author: Jordan Cook
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: aiohttp
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Provides-Extra: all
+Provides-Extra: docs
+Provides-Extra: dynamodb
+Provides-Extra: filesystem
+Provides-Extra: mongodb
+Provides-Extra: redis
+Provides-Extra: sqlite
+Requires-Dist: aioboto3 (>=9.0) ; extra == "all" or extra == "dynamodb"
+Requires-Dist: aiobotocore (>=2.0) ; extra == "all" or extra == "dynamodb"
+Requires-Dist: aiofiles (>=0.6.0) ; extra == "all" or extra == "filesystem"
+Requires-Dist: aiohttp (>=3.8,<4.0)
+Requires-Dist: aiosqlite (>=0.16) ; extra == "all" or extra == "filesystem" or extra == "sqlite"
+Requires-Dist: attrs (>=21.2)
+Requires-Dist: furo (>=2022.1.2) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: itsdangerous (>=2.0)
+Requires-Dist: linkify-it-py (>=2.0) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: markdown-it-py (>=2.2) ; python_version >= "3.8"
+Requires-Dist: motor (>=3.1) ; extra == "all" or extra == "mongodb"
+Requires-Dist: myst-parser (>=2.0) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: python-forge (>=18.6,<19.0)
+Requires-Dist: redis (>=4.2) ; extra == "all" or extra == "redis"
+Requires-Dist: sphinx (>=6.2,<7.0) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: sphinx-autodoc-typehints (>=1.23,<2.0) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: sphinx-automodapi (>=0.15) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: sphinx-copybutton (>=0.3,<0.4) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: sphinx-inline-tabs (>=2023.4) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: sphinxcontrib-apidoc (>=0.3) ; (python_version >= "3.8") and (extra == "docs")
+Requires-Dist: url-normalize (>=1.4,<2.0)
+Project-URL: Documentation, https://aiohttp-client-cache.readthedocs.io
+Project-URL: Repository, https://github.com/requests-cache/aiohttp-client-cache
+Description-Content-Type: text/markdown
+
+# aiohttp-client-cache
+
+[![Build status](https://github.com/requests-cache/aiohttp-client-cache/workflows/Build/badge.svg)](https://github.com/requests-cache/aiohttp-client-cache/actions)
+[![Documentation Status](https://img.shields.io/readthedocs/aiohttp-client-cache/stable?label=docs)](https://aiohttp-client-cache.readthedocs.io/en/latest/)
+[![Codecov](https://codecov.io/gh/requests-cache/aiohttp-client-cache/branch/main/graph/badge.svg?token=I6PNLYTILM)](https://codecov.io/gh/requests-cache/aiohttp-client-cache)
+[![PyPI](https://img.shields.io/pypi/v/aiohttp-client-cache?color=blue)](https://pypi.org/project/aiohttp-client-cache)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/aiohttp-client-cache?color=blue)](https://anaconda.org/conda-forge/aiohttp-client-cache)
+[![PyPI - Python Versions](https://img.shields.io/pypi/pyversions/aiohttp-client-cache)](https://pypi.org/project/aiohttp-client-cache)
+[![PyPI - Format](https://img.shields.io/pypi/format/aiohttp-client-cache?color=blue)](https://pypi.org/project/aiohttp-client-cache)
+
+**aiohttp-client-cache** is an async persistent cache for [aiohttp](https://docs.aiohttp.org)
+client requests, based on [requests-cache](https://github.com/reclosedev/requests-cache).
+
+# Features
+* **Ease of use:** Use as a [drop-in replacement](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html)
+  for `aiohttp.ClientSession`
+* **Customization:** Works out of the box with little to no config, but with plenty of options
+  available for customizing cache
+  [expiration](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html#cache-expiration)
+  and other [behavior](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html#cache-options)
+* **Persistence:** Includes several [storage backends](https://aiohttp-client-cache.readthedocs.io/en/latest/backends.html):
+  SQLite, DynamoDB, MongoDB, and Redis.
+
+# Quickstart
+First, install with pip (python 3.7+ required):
+```bash
+pip install aiohttp-client-cache
+```
+
+## Basic Usage
+Next, use [aiohttp_client_cache.CachedSession](https://aiohttp-client-cache.readthedocs.io/en/latest/modules/aiohttp_client_cache.session.html#aiohttp_client_cache.session.CachedSession)
+in place of [aiohttp.ClientSession](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.ClientSession).
+To briefly demonstrate how to use it:
+
+**Replace this:**
+```python
+from aiohttp import ClientSession
+
+async with ClientSession() as session:
+    await session.get('http://httpbin.org/delay/1')
+```
+
+**With this:**
+```python
+from aiohttp_client_cache import CachedSession, SQLiteBackend
+
+async with CachedSession(cache=SQLiteBackend('demo_cache')) as session:
+    await session.get('http://httpbin.org/delay/1')
+```
+
+The URL in this example adds a delay of 1 second, simulating a slow or rate-limited website.
+With caching, the response will be fetched once, saved to `demo_cache.sqlite`, and subsequent
+requests will return the cached response near-instantly.
+
+## Configuration
+Several options are available to customize caching behavior. This example demonstrates a few of them:
+
+```python
+# fmt: off
+from aiohttp_client_cache import SQLiteBackend
+
+cache = SQLiteBackend(
+    cache_name='~/.cache/aiohttp-requests.db',  # For SQLite, this will be used as the filename
+    expire_after=60*60,                         # By default, cached responses expire in an hour
+    urls_expire_after={'*.fillmurray.com': -1}, # Requests for any subdomain on this site will never expire
+    allowed_codes=(200, 418),                   # Cache responses with these status codes
+    allowed_methods=['GET', 'POST'],            # Cache requests with these HTTP methods
+    include_headers=True,                       # Cache requests with different headers separately
+    ignored_params=['auth_token'],              # Keep using the cached response even if this param changes
+    timeout=2.5,                                # Connection timeout for SQLite backend
+)
+```
+
+# More Info
+To learn more, see:
+* [User Guide](https://aiohttp-client-cache.readthedocs.io/en/latest/user_guide.html)
+* [Cache Backends](https://aiohttp-client-cache.readthedocs.io/en/latest/backends.html)
+* [API Reference](https://aiohttp-client-cache.readthedocs.io/en/latest/reference.html)
+* [Examples](https://aiohttp-client-cache.readthedocs.io/en/latest/examples.html)
+
+# Feedback
+If there is a feature you want, if you've discovered a bug, or if you have other general feedback, please
+[create an issue](https://github.com/requests-cache/aiohttp-client-cache/issues/new/choose) for it!
```

