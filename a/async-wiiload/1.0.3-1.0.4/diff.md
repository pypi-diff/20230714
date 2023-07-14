# Comparing `tmp/async-wiiload-1.0.3.tar.gz` & `tmp/async-wiiload-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-wiiload-1.0.3.tar", last modified: Thu Jul 13 10:19:48 2023, max compression
+gzip compressed data, was "async-wiiload-1.0.4.tar", last modified: Fri Jul 14 09:25:27 2023, max compression
```

## Comparing `async-wiiload-1.0.3.tar` & `async-wiiload-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.github/workflows/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/requirements-setuptools.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.857669 async-wiiload-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/src/async_wiiload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/async_wiiload.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/src/wiiload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/src/wiiload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/src/wiiload/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/src/wiiload/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 10:19:48.000000 async-wiiload-1.0.3/src/wiiload/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:19:48.861669 async-wiiload-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-13 10:19:38.000000 async-wiiload-1.0.3/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.281033 async-wiiload-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.277033 async-wiiload-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.277033 async-wiiload-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/.github/workflows/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-07-14 09:25:27.281033 async-wiiload-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/requirements-setuptools.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:25:27.281033 async-wiiload-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.277033 async-wiiload-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.277033 async-wiiload-1.0.4/src/async_wiiload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-07-14 09:25:27.000000 async-wiiload-1.0.4/src/async_wiiload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-14 09:25:27.000000 async-wiiload-1.0.4/src/async_wiiload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:25:27.000000 async-wiiload-1.0.4/src/async_wiiload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 09:25:27.000000 async-wiiload-1.0.4/src/async_wiiload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 09:25:27.000000 async-wiiload-1.0.4/src/async_wiiload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.281033 async-wiiload-1.0.4/src/wiiload/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/src/wiiload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/src/wiiload/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/src/wiiload/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 09:25:27.000000 async-wiiload-1.0.4/src/wiiload/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:25:27.281033 async-wiiload-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-14 09:25:18.000000 async-wiiload-1.0.4/tests/test_upload.py
```

### Comparing `async-wiiload-1.0.3/.github/dependabot.yml` & `async-wiiload-1.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/.github/workflows/ci.yml` & `async-wiiload-1.0.4/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -67,34 +67,32 @@
         shell: bash
 
       - name: run pytest
         run: python -m pytest --cov
 
       - name: codecov
         uses: codecov/codecov-action@v3
-        with:
-          fail_ci_if_error: true
 
   pypi:
     runs-on: 'ubuntu-latest'
     needs:
       - test
 
+    permissions:
+      id-token: write
+
     steps:
       - name: Download all the dists
         uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Publish 📦 to TestPyPI
         if: ${{ github.ref == 'refs/heads/main' }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.testpypi_password }}
           repository_url: https://test.pypi.org/legacy/
       
       - name: Publish 📦 to PyPI
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
```

### Comparing `async-wiiload-1.0.3/.github/workflows/dependabot.yml` & `async-wiiload-1.0.4/.github/workflows/dependabot.yml`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/.gitignore` & `async-wiiload-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/LICENSE` & `async-wiiload-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/PKG-INFO` & `async-wiiload-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wiiload
-Version: 1.0.3
+Version: 1.0.4
 Summary: library for sending executables to Wii's Homebrew Channel
 Author: Henrique Gemignani Passos Lima
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `async-wiiload-1.0.3/pyproject.toml` & `async-wiiload-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/src/async_wiiload.egg-info/PKG-INFO` & `async-wiiload-1.0.4/src/async_wiiload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wiiload
-Version: 1.0.3
+Version: 1.0.4
 Summary: library for sending executables to Wii's Homebrew Channel
 Author: Henrique Gemignani Passos Lima
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `async-wiiload-1.0.3/src/async_wiiload.egg-info/SOURCES.txt` & `async-wiiload-1.0.4/src/async_wiiload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/src/wiiload/__main__.py` & `async-wiiload-1.0.4/src/wiiload/__main__.py`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/src/wiiload/upload.py` & `async-wiiload-1.0.4/src/wiiload/upload.py`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/tests/test_main.py` & `async-wiiload-1.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `async-wiiload-1.0.3/tests/test_upload.py` & `async-wiiload-1.0.4/tests/test_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import io
 from unittest.mock import AsyncMock, MagicMock
 
-from wiiload import upload
+import wiiload
 
 
 async def test_upload_bytes(unused_tcp_port, mocker):
     result = io.BytesIO()
 
     reader = AsyncMock()
     writer = AsyncMock()
@@ -18,15 +18,15 @@
     )
 
     expected_data = (
         b"HAXX\x00\x05\x00\x08\x00\x00\x00\x0c\x00\x00\x00\x04x\x9c3426\x01\x00"
         b"\x01\xf8\x00\xcbme\x00that\x00"
     )
 
-    await upload.upload_bytes(b"1234", ["me", "that"], "localhost", unused_tcp_port)
+    await wiiload.upload_bytes(b"1234", ["me", "that"], "localhost", unused_tcp_port)
     assert result.getvalue() == expected_data
 
     mock_open_connection.assert_awaited_once_with("localhost", unused_tcp_port)
     writer.drain.assert_awaited_once_with()
     writer.close.assert_called_once_with()
     writer.wait_closed.assert_awaited_once_with()
 
@@ -36,13 +36,13 @@
         "wiiload.upload.upload_bytes", new_callable=AsyncMock
     )
 
     path = tmp_path.joinpath("somewhere.bin")
     path.write_bytes(b"foobar")
 
     # Run
-    await upload.upload_file(path, ["foo"], "localhost")
+    await wiiload.upload_file(path, ["foo"], "localhost")
 
     # Assert
     mock_upload_bytes.assert_awaited_once_with(
         b"foobar", ["somewhere.bin", "foo"], "localhost", 4299
     )
```

