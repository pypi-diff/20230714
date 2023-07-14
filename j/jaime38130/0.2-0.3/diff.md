# Comparing `tmp/jaime38130-0.2.tar.gz` & `tmp/jaime38130-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaime38130-0.2.tar", last modified: Fri Jul 14 21:11:15 2023, max compression
+gzip compressed data, was "dist\jaime38130-0.3.tar", last modified: Fri Jul 14 21:30:16 2023, max compression
```

## Comparing `jaime38130-0.2.tar` & `jaime38130-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 21:11:15.000000 jaime38130-0.2/
--rw-rw-rw-   0        0        0      769 2023-07-14 21:11:15.000000 jaime38130-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 21:11:15.000000 jaime38130-0.2/jaime38130/
--rw-rw-rw-   0        0        0       49 2023-07-14 20:04:50.000000 jaime38130-0.2/jaime38130/__init__.py
--rw-rw-rw-   0        0        0     1223 2023-07-14 21:01:04.000000 jaime38130-0.2/jaime38130/script_python.py
--rw-rw-rw-   0        0        0       65 2023-07-14 20:16:59.000000 jaime38130-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1685 2023-07-14 21:08:14.000000 jaime38130-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:30:16.000000 jaime38130-0.3/
+-rw-rw-rw-   0        0        0      870 2023-07-14 21:30:16.000000 jaime38130-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 21:30:16.000000 jaime38130-0.3/jaime38130/
+-rw-rw-rw-   0        0        0       49 2023-07-14 20:04:50.000000 jaime38130-0.3/jaime38130/__init__.py
+-rw-rw-rw-   0        0        0     1223 2023-07-14 21:24:42.000000 jaime38130-0.3/jaime38130/script_python.py
+-rw-rw-rw-   0        0        0       65 2023-07-14 20:16:59.000000 jaime38130-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-07-14 21:29:54.000000 jaime38130-0.3/setup.py
```

### Comparing `jaime38130-0.2/jaime38130/script_python.py` & `jaime38130-0.3/jaime38130/script_python.py`

 * *Files identical despite different names*

