# Comparing `tmp/bastila_search-0.4.1.tar.gz` & `tmp/bastila_search-0.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.4.1.tar", last modified: Fri Jul 14 19:19:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

