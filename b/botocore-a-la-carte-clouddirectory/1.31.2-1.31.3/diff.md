# Comparing `tmp/botocore-a-la-carte-clouddirectory-1.31.2.tar.gz` & `tmp/botocore_a_la_carte_clouddirectory-1.31.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-clouddirectory-1.31.2.tar", last modified: Wed Jul 12 01:44:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

