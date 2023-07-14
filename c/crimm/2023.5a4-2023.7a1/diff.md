# Comparing `tmp/crimm-2023.5a4.tar.gz` & `tmp/crimm-2023.7a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crimm-2023.5a4.tar", last modified: Thu Jun  1 00:02:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

