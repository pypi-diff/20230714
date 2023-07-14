# Comparing `tmp/racplusplus-0.0.4.tar.gz` & `tmp/racplusplus-0.0.5-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racplusplus-0.0.4.tar", last modified: Sat Jun 24 01:12:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

