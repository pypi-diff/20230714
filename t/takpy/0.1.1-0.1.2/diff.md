# Comparing `tmp/takpy-0.1.1.tar.gz` & `tmp/takpy-0.1.2.tar.gz`

## Comparing `takpy-0.1.1.tar` & `takpy-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 takpy-0.1.1/Cargo.toml
--rw-r--r--   0        0        0     5856 2023-07-13 13:00:30.000000 takpy-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       38 2023-07-13 13:28:26.000000 takpy-0.1.1/.gitignore
--rw-r--r--   0        0        0      681 2023-07-13 12:49:07.000000 takpy-0.1.1/README.md
--rw-r--r--   0        0        0      379 2023-07-13 12:51:42.000000 takpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6045 2023-07-13 13:27:13.000000 takpy-0.1.1/src/lib.rs
--rw-r--r--   0        0        0     7848 2023-07-13 13:27:21.000000 takpy-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 takpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 takpy-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0     5856 2023-07-13 13:00:30.000000 takpy-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       38 2023-07-13 13:28:26.000000 takpy-0.1.2/.gitignore
+-rw-r--r--   0        0        0      681 2023-07-13 12:49:07.000000 takpy-0.1.2/README.md
+-rw-r--r--   0        0        0      379 2023-07-13 12:51:42.000000 takpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6045 2023-07-13 13:27:13.000000 takpy-0.1.2/src/lib.rs
+-rw-r--r--   0        0        0     7848 2023-07-14 21:35:56.000000 takpy-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 takpy-0.1.2/PKG-INFO
```

### Comparing `takpy-0.1.1/.github/workflows/ci.yml` & `takpy-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `takpy-0.1.1/README.md` & `takpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `takpy-0.1.1/src/lib.rs` & `takpy-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `takpy-0.1.1/Cargo.lock` & `takpy-0.1.2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "fast-tak"
-version = "0.2.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b46fb8bb70168f596656201e0dae58726b286e121fd803250e69669da37eb776"
+checksum = "96f3bd65bba65ddc17f8477b88478d4d81048aba469315272d4928bfaffd6573"
 dependencies = [
  "takparse",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
@@ -203,15 +203,15 @@
 name = "takparse"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "616bf8626a329585beb63e0bb03a5d809318da9d41d7bfb694222ded8b0f4846"
 
 [[package]]
 name = "takpy"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "fast-tak",
  "pyo3",
 ]
 
 [[package]]
 name = "target-lexicon"
```

### Comparing `takpy-0.1.1/PKG-INFO` & `takpy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: takpy
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # takpy
```

