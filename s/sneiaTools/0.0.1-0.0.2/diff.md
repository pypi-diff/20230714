# Comparing `tmp/sneiaTools-0.0.1.tar.gz` & `tmp/sneiaTools-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneiaTools-0.0.1.tar", last modified: Wed Jul 12 19:44:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

