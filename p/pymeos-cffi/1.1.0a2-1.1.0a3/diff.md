# Comparing `tmp/pymeos_cffi-1.1.0a2.tar.gz` & `tmp/pymeos_cffi-1.1.0a3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeos_cffi-1.1.0a2.tar", last modified: Thu Jul 13 09:00:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

