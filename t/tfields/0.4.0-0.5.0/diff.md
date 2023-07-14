# Comparing `tmp/tfields-0.4.0.tar.gz` & `tmp/tfields-0.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tfields-0.4.0.tar", last modified: Thu Dec  9 16:07:32 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

