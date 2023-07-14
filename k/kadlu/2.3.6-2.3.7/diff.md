# Comparing `tmp/kadlu-2.3.6.tar.gz` & `tmp/kadlu-2.3.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kadlu-2.3.6.tar", last modified: Mon Jul 26 18:52:15 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

