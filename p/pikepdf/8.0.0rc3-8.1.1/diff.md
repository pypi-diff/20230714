# Comparing `tmp/pikepdf-8.0.0rc3.tar.gz` & `tmp/pikepdf-8.1.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-8.0.0rc3.tar", last modified: Tue Jul 11 21:13:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

