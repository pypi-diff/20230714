# Comparing `tmp/pyDolarVenezuela-1.0.4.tar.gz` & `tmp/pyDolarVenezuela-1.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDolarVenezuela-1.0.4.tar", last modified: Mon Jul  3 23:10:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

