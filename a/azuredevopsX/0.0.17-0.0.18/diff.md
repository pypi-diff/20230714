# Comparing `tmp/azuredevopsX-0.0.17.tar.gz` & `tmp/azuredevopsX-0.0.18-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azuredevopsX-0.0.17.tar", last modified: Wed Feb 15 13:18:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

