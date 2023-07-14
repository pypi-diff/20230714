# Comparing `tmp/mkits-0.87.tar.gz` & `tmp/mkits-0.88-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkits-0.87.tar", last modified: Wed May 31 21:10:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

