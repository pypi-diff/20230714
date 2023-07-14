# Comparing `tmp/racplusplus-0.0.4.tar.gz` & `tmp/racplusplus-0.0.5-cp311-cp311-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racplusplus-0.0.4.tar", last modified: Sat Jun 24 01:12:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

