# Comparing `tmp/marlowe-0.1.0-cp311-none-win_amd64.whl.zip` & `tmp/marlowe-0.1.1-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 816371 bytes, number of entries: 5
--rw-r--r--  4.6 unx     1061 b- defN 23-Jul-14 20:40 marlowe-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Jul-14 20:40 marlowe-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      111 b- defN 23-Jul-14 20:40 marlowe/__init__.py
--rwxr-xr-x  4.6 unx  2411520 b- defN 23-Jul-14 20:40 marlowe/marlowe.cp311-win_amd64.pyd
--rw-r--r--  4.6 unx      376 b- defN 23-Jul-14 20:40 marlowe-0.1.0.dist-info/RECORD
-5 files, 2413163 bytes uncompressed, 815679 bytes compressed:  66.2%
+Zip file size: 816455 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     1400 b- defN 23-Jul-14 21:35 marlowe-0.1.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jul-14 21:35 marlowe-0.1.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx      111 b- defN 23-Jul-14 21:35 marlowe/__init__.py
+-rwxr-xr-x  4.6 unx  2411520 b- defN 23-Jul-14 21:35 marlowe/marlowe.cp311-win_amd64.pyd
+-rw-r--r--  4.6 unx      376 b- defN 23-Jul-14 21:35 marlowe-0.1.1.dist-info/RECORD
+5 files, 2413502 bytes uncompressed, 815763 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: marlowe-0.1.0.dist-info/METADATA
+Filename: marlowe-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: marlowe-0.1.0.dist-info/WHEEL
+Filename: marlowe-0.1.1.dist-info/WHEEL
 Comment: 
 
 Filename: marlowe/__init__.py
 Comment: 
 
 Filename: marlowe/marlowe.cp311-win_amd64.pyd
 Comment: 
 
-Filename: marlowe-0.1.0.dist-info/RECORD
+Filename: marlowe-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `marlowe-0.1.0.dist-info/METADATA` & `marlowe-0.1.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: marlowe
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Summary: marlowe-rs bindings for using cardano marlowe in python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ## MARLOWE-PY
 
 **Python bindings for Marlowe_Lang [marlowe-rs](https://github.com/OlofBlomqvist/marlowe-rs).**
 
@@ -21,19 +22,27 @@
 ### Project goals
 
 - Provide easy to use API's for everything marlowe-rs supports.
 - Provide easy to use way of designing Marlowe contracts in Python.
 
 ### How to install
 
-No package has been published to PyPi yet - for now, you need download and pip install marlowepy.gz
+```bash
+pip install marlowe
+```
+
+Or pip install wlh files directly:
+- release versions: https://github.com/OlofBlomqvist/marlowe-py/releases
+- latest builds artifact: https://github.com/OlofBlomqvist/marlowe-py/actions/workflows/wheely.yml
+
 
 ### How to use
 
-- See the notebook for example usage.
+See the example notebook [here](https://github.com/OlofBlomqvist/marlowe-py/blob/main/example.ipynb).
+
 
-### How to build
+### Building from source
 
-- See [development.md](./development.md)
+- See [development.md](https://github.com/OlofBlomqvist/marlowe-py/blob/main/development.md)
```

