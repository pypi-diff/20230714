# Comparing `tmp/antgen-0.3.7.tar.gz` & `tmp/antgen-0.3.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\antgen-0.3.7.tar", last modified: Fri Jul 14 17:00:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

