# Comparing `tmp/element-sdk-0.2.5.tar.gz` & `tmp/element_sdk-0.2.6-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-sdk-0.2.5.tar", last modified: Thu Jul 13 14:13:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

