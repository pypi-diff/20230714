# Comparing `tmp/intel_extension_for_transformers-1.0b0.tar.gz` & `tmp/intel_extension_for_transformers-1.1-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_extension_for_transformers-1.0b0.tar", last modified: Sun Dec 11 05:19:15 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

