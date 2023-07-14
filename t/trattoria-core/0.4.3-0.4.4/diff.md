# Comparing `tmp/trattoria_core-0.4.3.tar.gz` & `tmp/trattoria_core-0.4.4.tar.gz`

## Comparing `trattoria_core-0.4.3.tar` & `trattoria_core-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 trattoria_core-0.4.3/Cargo.toml
--rw-r--r--   0     1001      121     3337 2021-08-06 16:02:51.000000 trattoria_core-0.4.3/.github/workflows/ci.yml
--rw-r--r--   0     1001      121       52 2021-08-06 16:02:51.000000 trattoria_core-0.4.3/.gitignore
--rw-r--r--   0     1001      121      152 2021-08-06 16:02:51.000000 trattoria_core-0.4.3/README.md
--rw-r--r--   0     1001      121     7195 2021-08-06 16:02:51.000000 trattoria_core-0.4.3/poetry.lock
--rw-r--r--   0     1001      121      394 2021-08-06 16:02:51.000000 trattoria_core-0.4.3/pyproject.toml
--rw-r--r--   0     1001      121    17405 2021-08-06 16:02:51.000000 trattoria_core-0.4.3/src/lib.rs
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 trattoria_core-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 trattoria_core-0.4.4/Cargo.toml
+-rw-r--r--   0        0        0     1319 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1523 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/.github/workflows/ci_windows.yml
+-rw-r--r--   0        0        0      469 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/.github/workflows/linting.yml
+-rw-r--r--   0        0        0       70 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/.gitignore
+-rw-r--r--   0        0        0      154 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/README.md
+-rw-r--r--   0        0        0      417 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    17985 2023-07-14 09:22:05.000000 trattoria_core-0.4.4/src/lib.rs
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 trattoria_core-0.4.4/PKG-INFO
```

### Comparing `trattoria_core-0.4.3/Cargo.toml` & `trattoria_core-0.4.4/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [package]
 name = "trattoria-core"
-version = "0.4.3"
+version = "0.4.4"
 authors = ["Guillem Ballesteros <dev+crate@maxwellrules.com>"]
 description = "PyO3 wrapper for TTTR-Toolbox"
 edition = "2018"
 license = "MIT"
 keywords = ["scientific-computing", "python", "science"]
-
+
 [lib]
 name = "trattoria_core"
 crate-type = ["cdylib"]
-
+
 [dependencies]
-tttr-toolbox = "0.4.3"
+tttr-toolbox = "0.4.4"
 #tttr-toolbox = { path = "../tttr-toolbox/tttr-toolbox" }
 numpy = "0.13.2"
 ndarray = "0.15.2"
-
+
 [profile.release]
 lto="fat"
 codegen-units = 1
 debug = false
 incremental = false
-
+
 [dependencies.pyo3]
 version = "0.13.2"
 features = ["extension-module"]
-
+
 [package.metadata.maturin]
 requires-dist = ["numpy>=1.16"]
 classifier = ["Programming Language :: Python", "Topic :: Scientific/Engineering", "Topic :: Scientific/Engineering :: Physics"]
```

