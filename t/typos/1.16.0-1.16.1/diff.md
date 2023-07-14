# Comparing `tmp/typos-1.16.0.tar.gz` & `tmp/typos-1.16.1.tar.gz`

## Comparing `typos-1.16.0.tar` & `typos-1.16.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  7035769 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44720 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.16.0/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.16.0/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12622 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21859 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32621 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     6791 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123      207 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      123    53454 2023-07-10 15:05:23.000000 typos-1.16.0/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.16.0/PKG-INFO
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    46000 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    18950 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  7035769 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.16.1/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-07-14 19:29:01.000000 typos-1.16.1/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.16.1/pyproject.toml
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 typos-1.16.1/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12622 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21859 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32621 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     6791 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123      207 2023-07-14 19:29:01.000000 typos-1.16.1/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      123    53691 2023-07-14 19:29:01.000000 typos-1.16.1/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.16.1/PKG-INFO
```

### Comparing `typos-1.16.0/local_dependencies/typos-dict/Cargo.toml` & `typos-1.16.1/local_dependencies/typos-dict/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-dict"
-version = "0.10.6"
+version = "0.10.7"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.16.0/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.16.1/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/varcon-core/Cargo.toml` & `typos-1.16.1/local_dependencies/varcon-core/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "varcon-core"
-version = "2.2.12"
+version = "4.0.0"
 description = "Varcon-relevant data structures"
 readme = "../../README.md"
 categories = ["text-processing"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
 rust-version= "1.64.0"  # MSRV
@@ -16,16 +16,16 @@
   "README.md",
   "benches/**/*",
   "examples/**/*"
 ]
 
 [features]
 default = []
-parser = ["winnow"]
-flags = ["enumflags2"]
+parser = ["dep:winnow"]
+flags = ["dep:enumflags2"]
 
 [dependencies]
-winnow = { version = "0.4.6", optional = true }
+winnow = { version = "0.5.0", optional = true }
 enumflags2 = { version = "0.7", optional = true }
 
 [package.metadata.docs.rs]
 features = [ "parser", "flags" ]
```

### Comparing `typos-1.16.0/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.16.1/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/varcon-core/src/lib.rs` & `typos-1.16.1/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/dictgen/Cargo.toml` & `typos-1.16.1/local_dependencies/dictgen/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dictgen"
-version = "0.2.5"
+version = "0.2.6"
 description = "Compile-time case-insensitive map"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling", "no_std"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
 rust-version= "1.64.0"  # MSRV
@@ -17,15 +17,15 @@
   "benches/**/*",
   "examples/**/*"
 ]
 
 [features]
 default = ["std"]
 std = []
-codegen = ["std", "phf_codegen"]
-map = ["phf", "phf_shared"]
+codegen = ["std", "dep:phf_codegen"]
+map = ["dep:phf", "dep:phf_shared"]
 
 [dependencies]
 unicase = "2.6"
 phf = { version = "0.11", features = ["unicase"], optional = true }
 phf_codegen = { version = "0.11", optional = true }
 phf_shared = { version = "0.11", optional = true }
```

### Comparing `typos-1.16.0/local_dependencies/dictgen/src/map.rs` & `typos-1.16.1/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/dictgen/src/table.rs` & `typos-1.16.1/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/dictgen/src/trie.rs` & `typos-1.16.1/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/typos-vars/Cargo.toml` & `typos-1.16.1/local_dependencies/typos-vars/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-vars"
-version = "0.8.10"
+version = "0.8.11"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
@@ -18,8 +18,8 @@
   "benches/**/*",
   "examples/**/*"
 ]
 
 [dependencies]
 unicase = "2.6"
 dictgen = { version = "^0.2", path = "../dictgen" }
-varcon-core = { version = "^2.2", path = "../varcon-core", features = ["flags"] }
+varcon-core = { version = "^4.0", path = "../varcon-core", features = ["flags"] }
```

### Comparing `typos-1.16.0/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.16.1/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/typos/Cargo.toml` & `typos-1.16.1/local_dependencies/typos/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos"
-version = "0.10.14"
+version = "0.10.15"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
@@ -18,15 +18,15 @@
   "benches/**/*",
   "examples/**/*"
 ]
 
 [dependencies]
 anyhow = "1.0"
 thiserror = "1.0"
-winnow = "0.4.6"
+winnow = "0.5.0"
 unicode-xid = "0.2.4"
 once_cell = "1.17.2"
 serde = { version = "1.0", features = ["derive"] }
 simdutf8 = "0.1.4"
 itertools = "0.10"
 unicode-segmentation = "1.10.1"
 bstr = "1.5"
```

### Comparing `typos-1.16.0/local_dependencies/typos/src/check.rs` & `typos-1.16.1/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/typos/src/dict.rs` & `typos-1.16.1/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/local_dependencies/typos/src/tokens.rs` & `typos-1.16.1/local_dependencies/typos/src/tokens.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use bstr::ByteSlice;
+use winnow::BStr;
 
 /// Define rules for tokenizaing a buffer.
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub struct TokenizerBuilder {
     unicode: bool,
 }
 
@@ -44,25 +45,27 @@
         TokenizerBuilder::default().build()
     }
 
     pub fn parse_str<'c>(&'c self, content: &'c str) -> impl Iterator<Item = Identifier<'c>> {
         let iter = if self.unicode && !ByteSlice::is_ascii(content.as_bytes()) {
             itertools::Either::Left(unicode_parser::iter_identifiers(content))
         } else {
-            itertools::Either::Right(ascii_parser::iter_identifiers(content.as_bytes()))
+            itertools::Either::Right(ascii_parser::iter_identifiers(BStr::new(
+                content.as_bytes(),
+            )))
         };
         iter.map(move |identifier| self.transform(identifier, content.as_bytes()))
     }
 
     pub fn parse_bytes<'c>(&'c self, content: &'c [u8]) -> impl Iterator<Item = Identifier<'c>> {
         let iter = if self.unicode && !ByteSlice::is_ascii(content) {
             let iter = Utf8Chunks::new(content).flat_map(unicode_parser::iter_identifiers);
             itertools::Either::Left(iter)
         } else {
-            itertools::Either::Right(ascii_parser::iter_identifiers(content))
+            itertools::Either::Right(ascii_parser::iter_identifiers(BStr::new(content)))
         };
         iter.map(move |identifier| self.transform(identifier, content))
     }
 
     fn transform<'i>(&self, identifier: &'i str, content: &[u8]) -> Identifier<'i> {
         debug_assert!(!identifier.is_empty());
 
@@ -122,192 +125,209 @@
             }
         }
     }
 }
 
 mod parser {
     use winnow::combinator::*;
+    use winnow::error::ParserError;
     use winnow::prelude::*;
     use winnow::stream::AsBStr;
     use winnow::stream::AsChar;
     use winnow::stream::SliceLen;
     use winnow::stream::Stream;
     use winnow::stream::StreamIsPartial;
     use winnow::token::*;
+    use winnow::trace::trace;
 
-    pub(crate) fn next_identifier<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    pub(crate) fn next_identifier<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         preceded(ignore, identifier).parse_next(input)
     }
 
-    fn identifier<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn identifier<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         // Generally a language would be `{XID_Start}{XID_Continue}*` but going with only
         // `{XID_Continue}+` because XID_Continue is a superset of XID_Start and rather catch odd
         // or unexpected cases than strip off start characters to a word since we aren't doing a
         // proper word boundary parse
-        take_while(1.., is_xid_continue).parse_next(input)
+        trace("identifier", take_while(1.., is_xid_continue)).parse_next(input)
     }
 
-    fn ignore<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn ignore<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        take_many0(alt((
-            // CAUTION: If adding an ignorable literal, if it doesn't start with `is_xid_continue`,
-            // - Update `is_ignore_char` to make sure `sep1` doesn't eat it all up
-            // - Make sure you always consume it
-            terminated(uuid_literal, peek(sep1)),
-            terminated(hash_literal, peek(sep1)),
-            terminated(base64_literal, peek(sep1)), // base64 should be quoted or something
-            terminated(ordinal_literal, peek(sep1)),
-            terminated(hex_literal, peek(sep1)),
-            terminated(dec_literal, peek(sep1)), // Allow digit-prefixed words
-            terminated(email_literal, peek(sep1)),
-            terminated(url_literal, peek(sep1)),
-            terminated(css_color, peek(sep1)),
-            c_escape,
-            printf,
-            other,
-        )))
+        trace(
+            "ignore",
+            take_many0(alt((
+                // CAUTION: If adding an ignorable literal, if it doesn't start with `is_xid_continue`,
+                // - Update `is_ignore_char` to make sure `sep1` doesn't eat it all up
+                // - Make sure you always consume it
+                terminated(uuid_literal, peek(sep1)),
+                terminated(hash_literal, peek(sep1)),
+                terminated(base64_literal, peek(sep1)), // base64 should be quoted or something
+                terminated(ordinal_literal, peek(sep1)),
+                terminated(hex_literal, peek(sep1)),
+                terminated(dec_literal, peek(sep1)), // Allow digit-prefixed words
+                terminated(email_literal, peek(sep1)),
+                terminated(url_literal, peek(sep1)),
+                terminated(css_color, peek(sep1)),
+                c_escape,
+                printf,
+                other,
+            ))),
+        )
         .parse_next(input)
     }
 
-    fn sep1<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn sep1<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         alt((
             one_of(|c| !is_xid_continue(c)).recognize(),
             eof.map(|_| <T as Stream>::Slice::default()),
         ))
         .parse_next(input)
     }
 
-    fn other<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn other<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        (
-            one_of(|c| !is_xid_continue(c)),
-            take_while(0.., is_ignore_char),
+        trace(
+            "other",
+            (
+                one_of(|c| !is_xid_continue(c)),
+                take_while(0.., is_ignore_char),
+            )
+                .recognize(),
         )
-            .recognize()
-            .parse_next(input)
+        .parse_next(input)
     }
 
-    fn ordinal_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn ordinal_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         fn is_sep(c: impl AsChar) -> bool {
             let c = c.as_char();
             // Avoid markdown throwing off our ordinal detection
             ['_'].contains(&c)
         }
 
-        (
-            take_while(0.., is_sep),
-            take_while(1.., is_dec_digit),
-            alt((('s', 't'), ('n', 'd'), ('r', 'd'), ('t', 'h'))),
-            take_while(0.., is_sep),
+        trace(
+            "ordinal_literal",
+            (
+                take_while(0.., is_sep),
+                take_while(1.., is_dec_digit),
+                alt((('s', 't'), ('n', 'd'), ('r', 'd'), ('t', 'h'))),
+                take_while(0.., is_sep),
+            )
+                .recognize(),
         )
-            .recognize()
-            .parse_next(input)
+        .parse_next(input)
     }
 
-    fn dec_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn dec_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        take_while(1.., is_dec_digit_with_sep).parse_next(input)
+        trace("dec_literal", take_while(1.., is_dec_digit_with_sep)).parse_next(input)
     }
 
-    fn hex_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn hex_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         preceded(
             ('0', alt(('x', 'X'))),
             take_while(1.., is_hex_digit_with_sep),
         )
         .parse_next(input)
     }
 
-    fn css_color<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn css_color<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        preceded(
-            '#',
-            alt((
-                terminated(take_while(3..=8, is_lower_hex_digit), peek(sep1)),
-                terminated(take_while(3..=8, is_upper_hex_digit), peek(sep1)),
-            )),
+        trace(
+            "color",
+            preceded(
+                '#',
+                alt((
+                    terminated(take_while(3..=8, is_lower_hex_digit), peek(sep1)),
+                    terminated(take_while(3..=8, is_upper_hex_digit), peek(sep1)),
+                )),
+            ),
         )
         .parse_next(input)
     }
 
-    fn uuid_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn uuid_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        alt((
-            (
-                take_while(8, is_lower_hex_digit),
-                '-',
-                take_while(4, is_lower_hex_digit),
-                '-',
-                take_while(4, is_lower_hex_digit),
-                '-',
-                take_while(4, is_lower_hex_digit),
-                '-',
-                take_while(12, is_lower_hex_digit),
-            ),
-            (
-                take_while(8, is_upper_hex_digit),
-                '-',
-                take_while(4, is_upper_hex_digit),
-                '-',
-                take_while(4, is_upper_hex_digit),
-                '-',
-                take_while(4, is_upper_hex_digit),
-                '-',
-                take_while(12, is_upper_hex_digit),
-            ),
-        ))
-        .recognize()
+        trace(
+            "uuid",
+            alt((
+                (
+                    take_while(8, is_lower_hex_digit),
+                    '-',
+                    take_while(4, is_lower_hex_digit),
+                    '-',
+                    take_while(4, is_lower_hex_digit),
+                    '-',
+                    take_while(4, is_lower_hex_digit),
+                    '-',
+                    take_while(12, is_lower_hex_digit),
+                ),
+                (
+                    take_while(8, is_upper_hex_digit),
+                    '-',
+                    take_while(4, is_upper_hex_digit),
+                    '-',
+                    take_while(4, is_upper_hex_digit),
+                    '-',
+                    take_while(4, is_upper_hex_digit),
+                    '-',
+                    take_while(12, is_upper_hex_digit),
+                ),
+            ))
+            .recognize(),
+        )
         .parse_next(input)
     }
 
-    fn hash_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn hash_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         // Size considerations:
         //   - 40 characters holds for a SHA-1 hash from older Git versions.
@@ -315,139 +335,160 @@
         //   - Git allows abbreviated hashes, but we need a good abbreviation
         //     that won't be mistaken for a variable name.
         //   - Through experimentation we've found that there is almost
         //     never any actual text inside a hex string of 32 characters
         //     or more.
 
         const IGNORE_HEX_MIN: usize = 32;
-        alt((
-            take_while(IGNORE_HEX_MIN.., is_lower_hex_digit),
-            take_while(IGNORE_HEX_MIN.., is_upper_hex_digit),
-        ))
+        trace(
+            "hash",
+            alt((
+                take_while(IGNORE_HEX_MIN.., is_lower_hex_digit),
+                take_while(IGNORE_HEX_MIN.., is_upper_hex_digit),
+            )),
+        )
         .parse_next(input)
     }
 
-    fn base64_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn base64_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        let (padding, captured) = take_while(1.., is_base64_digit).parse_next(input.clone())?;
+        trace("base64", move |input: &mut T| {
+            let start = input.checkpoint();
+            let captured = take_while(1.., is_base64_digit).parse_next(input)?;
 
-        const CHUNK: usize = 4;
-        let padding_offset = input.offset_to(&padding);
-        let mut padding_len = CHUNK - padding_offset % CHUNK;
-        if padding_len == CHUNK {
-            padding_len = 0;
-        }
+            const CHUNK: usize = 4;
+            let padding_offset = input.offset_from(&start);
+            let mut padding_len = CHUNK - padding_offset % CHUNK;
+            if padding_len == CHUNK {
+                padding_len = 0;
+            }
 
-        if captured.slice_len() < 90
-            && padding_len == 0
-            && captured
-                .as_bstr()
-                .iter()
-                .all(|c| !['/', '+'].contains(&c.as_char()))
-        {
-            return Err(winnow::error::ErrMode::Backtrack(
-                winnow::error::Error::new(input, winnow::error::ErrorKind::Slice),
-            ));
-        }
+            if captured.slice_len() < 90
+                && padding_len == 0
+                && captured
+                    .as_bstr()
+                    .iter()
+                    .all(|c| !['/', '+'].contains(&c.as_char()))
+            {
+                return Err(winnow::error::ErrMode::from_error_kind(
+                    input,
+                    winnow::error::ErrorKind::Slice,
+                ));
+            }
 
-        let (after, _) =
-            take_while(padding_len..=padding_len, is_base64_padding).parse_next(padding)?;
+            take_while(padding_len..=padding_len, is_base64_padding).parse_next(input)?;
 
-        let after_offset = input.offset_to(&after);
-        Ok(input.next_slice(after_offset))
+            let after_offset = input.offset_from(&start);
+            input.reset(start);
+            Ok(input.next_slice(after_offset))
+        })
+        .parse_next(input)
     }
 
-    fn email_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn email_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        (
-            take_while(1.., is_localport_char),
-            '@',
-            take_while(1.., is_domain_char),
+        trace(
+            "email",
+            (
+                take_while(1.., is_localport_char),
+                '@',
+                take_while(1.., is_domain_char),
+            )
+                .recognize(),
         )
-            .recognize()
-            .parse_next(input)
+        .parse_next(input)
     }
 
-    fn url_literal<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn url_literal<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        (
-            opt(terminated(
-                take_while(1.., is_scheme_char),
-                // HACK: Technically you can skip `//` if you don't have a domain but that would
-                // get messy to support.
-                (':', '/', '/'),
-            )),
+        trace(
+            "url",
             (
-                opt(terminated(url_userinfo, '@')),
-                take_while(1.., is_domain_char),
-                opt(preceded(':', take_while(1.., AsChar::is_dec_digit))),
-            ),
-            '/',
-            // HACK: Too lazy to enumerate
-            take_while(0.., is_path_query_fragment),
+                opt(terminated(
+                    take_while(1.., is_scheme_char),
+                    // HACK: Technically you can skip `//` if you don't have a domain but that would
+                    // get messy to support.
+                    (':', '/', '/'),
+                )),
+                (
+                    opt(terminated(url_userinfo, '@')),
+                    take_while(1.., is_domain_char),
+                    opt(preceded(':', take_while(1.., AsChar::is_dec_digit))),
+                ),
+                '/',
+                // HACK: Too lazy to enumerate
+                take_while(0.., is_path_query_fragment),
+            )
+                .recognize(),
         )
-            .recognize()
-            .parse_next(input)
+        .parse_next(input)
     }
 
-    fn url_userinfo<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn url_userinfo<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        (
-            take_while(1.., is_localport_char),
-            opt(preceded(':', take_while(0.., is_localport_char))),
+        trace(
+            "userinfo",
+            (
+                take_while(1.., is_localport_char),
+                opt(preceded(':', take_while(0.., is_localport_char))),
+            )
+                .recognize(),
         )
-            .recognize()
-            .parse_next(input)
+        .parse_next(input)
     }
 
-    fn c_escape<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn c_escape<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
         // We don't know whether the string we are parsing is a literal string (no escaping) or
         // regular string that does escaping. The escaped letter might be part of a word, or it
         // might not be. Rather than guess and be wrong part of the time and correct people's words
         // incorrectly, we opt for just not evaluating it at all.
-        preceded(take_while(1.., is_escape), take_while(0.., is_xid_continue)).parse_next(input)
+        trace(
+            "escape",
+            preceded(take_while(1.., is_escape), take_while(0.., is_xid_continue)),
+        )
+        .parse_next(input)
     }
 
-    fn printf<T>(input: T) -> IResult<T, <T as Stream>::Slice>
+    fn printf<T>(input: &mut T) -> PResult<<T as Stream>::Slice, ()>
     where
         T: Stream + StreamIsPartial + PartialEq,
         <T as Stream>::Slice: AsBStr + SliceLen + Default,
         <T as Stream>::Token: AsChar + Copy,
     {
-        preceded('%', take_while(1.., is_xid_continue)).parse_next(input)
+        trace("printf", preceded('%', take_while(1.., is_xid_continue))).parse_next(input)
     }
 
-    fn take_many0<I, E, F>(mut f: F) -> impl FnMut(I) -> IResult<I, <I as Stream>::Slice, E>
+    fn take_many0<I, E, F>(mut f: F) -> impl Parser<I, <I as Stream>::Slice, E>
     where
         I: Stream,
-        F: winnow::Parser<I, <I as Stream>::Slice, E>,
-        E: winnow::error::ParseError<I>,
+        F: Parser<I, <I as Stream>::Slice, E>,
+        E: ParserError<I>,
     {
-        move |i: I| {
+        move |i: &mut I| {
             repeat(0.., f.by_ref())
                 .map(|()| ())
                 .recognize()
                 .parse_next(i)
         }
     }
 
@@ -577,32 +618,32 @@
     }
 }
 
 mod unicode_parser {
     use super::parser::next_identifier;
 
     pub(crate) fn iter_identifiers(mut input: &str) -> impl Iterator<Item = &str> {
-        std::iter::from_fn(move || match next_identifier(input) {
-            Ok((i, o)) => {
-                input = i;
+        std::iter::from_fn(move || match next_identifier(&mut input) {
+            Ok(o) => {
                 debug_assert_ne!(o, "");
                 Some(o)
             }
             _ => None,
         })
     }
 }
 
 mod ascii_parser {
     use super::parser::next_identifier;
 
-    pub(crate) fn iter_identifiers(mut input: &[u8]) -> impl Iterator<Item = &str> {
-        std::iter::from_fn(move || match next_identifier(input) {
-            Ok((i, o)) => {
-                input = i;
+    use winnow::BStr;
+
+    pub(crate) fn iter_identifiers(mut input: &BStr) -> impl Iterator<Item = &str> {
+        std::iter::from_fn(move || match next_identifier(&mut input) {
+            Ok(o) => {
                 debug_assert_ne!(o, b"");
                 // This is safe because we've checked that the strings are a subset of ASCII
                 // characters.
                 let o = unsafe { std::str::from_utf8_unchecked(o) };
                 Some(o)
             }
             _ => None,
```

### Comparing `typos-1.16.0/rust_src/typos-cli/Cargo.toml` & `typos-1.16.1/rust_src/typos-cli/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.16.0"
+version = "1.16.1"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
@@ -36,26 +36,26 @@
   {file="../../action/entrypoint.sh", search="VERSION=.*", replace="VERSION={{version}}", min=1},
   {file="../../docs/pre-commit.md", search="rev: .*", replace="rev: {{tag_name}}", exactly=1},
   {file="../../setup.py", search="TYPOS_VERSION = .*", replace="TYPOS_VERSION = '{{version}}'", exactly=1},
 ]
 
 [features]
 default = ["dict", "vars"]
-dict = ["typos-dict"]
-vars = ["typos-vars"]
+dict = ["dep:typos-dict"]
+vars = ["dep:typos-vars"]
 
 
 [[bin]]
 name = "typos"
 path = "src/bin/typos-cli/main.rs"
 doc = false
 
 [dependencies]
 typos = { version = "^0.10", path = "../../local_dependencies/typos" }
-varcon-core = { version = "^2.2.12", path = "../../local_dependencies/varcon-core" }
+varcon-core = { version = "^4.0.0", path = "../../local_dependencies/varcon-core" }
 typos-dict = { version = "^0.10", path = "../../local_dependencies/typos-dict", optional = true }
 typos-vars = { version = "^0.8", path = "../../local_dependencies/typos-vars", optional = true }
 unicase = "2.6"
 anyhow = "1.0"
 clap = { version = "4.3.0", features = ["derive"] }
 clap-verbosity-flag = "2.0"
 ignore = "0.4"
```

### Comparing `typos-1.16.0/rust_src/typos-cli/benches/checks.rs` & `typos-1.16.1/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/benches/corrections.rs` & `typos-1.16.1/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/benches/data.rs` & `typos-1.16.1/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.16.1/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.16.1/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/config.rs` & `typos-1.16.1/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/default_types.rs` & `typos-1.16.1/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/dict.rs` & `typos-1.16.1/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/file.rs` & `typos-1.16.1/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/file_type.rs` & `typos-1.16.1/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/policy.rs` & `typos-1.16.1/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/rust_src/typos-cli/src/report.rs` & `typos-1.16.1/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.16.0/Cargo.lock` & `typos-1.16.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dictgen"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "phf",
  "phf_codegen",
  "phf_shared",
  "unicase",
 ]
 
@@ -1606,15 +1606,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
 dependencies = [
  "indexmap 1.9.2",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "winnow",
+ "winnow 0.4.9",
 ]
 
 [[package]]
 name = "trycmd"
 version = "0.14.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2925e71868a12b173c1eb166018c2d2f9dfaedfcaec747bdb6ea2246785d258e"
@@ -1633,31 +1633,31 @@
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typos"
-version = "0.10.14"
+version = "0.10.15"
 dependencies = [
  "anyhow",
  "bstr",
  "itertools",
  "once_cell",
  "serde",
  "simdutf8",
  "thiserror",
  "unicode-segmentation",
  "unicode-xid",
- "winnow",
+ "winnow 0.5.0",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.16.0"
+version = "1.16.1"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
@@ -1697,30 +1697,30 @@
  "unicode-segmentation",
  "unicode-width",
  "varcon-core",
 ]
 
 [[package]]
 name = "typos-dict"
-version = "0.10.6"
+version = "0.10.7"
 dependencies = [
  "codegenrs",
  "csv",
  "dictgen",
  "edit-distance",
  "indexmap 2.0.0",
  "itertools",
  "snapbox",
  "unicase",
  "varcon",
 ]
 
 [[package]]
 name = "typos-vars"
-version = "0.8.10"
+version = "0.8.11"
 dependencies = [
  "codegenrs",
  "dictgen",
  "itertools",
  "snapbox",
  "typos",
  "unicase",
@@ -1815,27 +1815,27 @@
 checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "varcon"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "codegenrs",
  "snapbox",
  "varcon-core",
 ]
 
 [[package]]
 name = "varcon-core"
-version = "2.2.12"
+version = "4.0.0"
 dependencies = [
  "enumflags2",
- "winnow",
+ "winnow 0.5.0",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
@@ -2117,13 +2117,22 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.6"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81a2094c43cc94775293eaa0e499fbc30048a6d824ac82c0351a8c0bf9112529"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "winnow"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
+checksum = "81fac9742fd1ad1bd9643b991319f72dd031016d44b77039a26977eb667141e7"
 dependencies = [
  "memchr",
 ]
```

### Comparing `typos-1.16.0/PKG-INFO` & `typos-1.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.16.0
+Version: 1.16.1
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

