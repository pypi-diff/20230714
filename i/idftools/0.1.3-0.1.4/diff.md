# Comparing `tmp/idftools-0.1.3.tar.gz` & `tmp/idftools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idftools-0.1.3.tar", last modified: Thu Jul 13 20:58:44 2023, max compression
+gzip compressed data, was "idftools-0.1.4.tar", last modified: Fri Jul 14 16:37:52 2023, max compression
```

## Comparing `idftools-0.1.3.tar` & `idftools-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-13 20:58:44.654091 idftools-0.1.3/
--rw-rw-r--   0 enio      (1000) enio      (1000)      233 2023-07-13 20:58:44.654091 idftools-0.1.3/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)       99 2023-07-13 20:22:47.000000 idftools-0.1.3/README.md
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-13 20:58:44.654091 idftools-0.1.3/idftools/
--rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.3/idftools/certificate.py
--rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.3/idftools/driversfactory.py
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-13 20:58:44.654091 idftools-0.1.3/idftools/idftools.egg-info/
--rw-rw-r--   0 enio      (1000) enio      (1000)      233 2023-07-13 20:58:44.000000 idftools-0.1.3/idftools/idftools.egg-info/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-13 20:58:44.000000 idftools-0.1.3/idftools/idftools.egg-info/SOURCES.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-13 20:58:44.000000 idftools-0.1.3/idftools/idftools.egg-info/dependency_links.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)      307 2023-07-13 20:58:44.000000 idftools-0.1.3/idftools/idftools.egg-info/requires.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-13 20:58:44.000000 idftools-0.1.3/idftools/idftools.egg-info/top_level.txt
--rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.3/idftools/utilities.py
--rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-13 20:58:44.654091 idftools-0.1.3/setup.cfg
--rw-rw-r--   0 enio      (1000) enio      (1000)      483 2023-07-13 20:54:49.000000 idftools-0.1.3/setup.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 16:37:52.343838 idftools-0.1.4/
+-rw-rw-r--   0 enio      (1000) enio      (1000)      668 2023-07-14 16:37:52.343838 idftools-0.1.4/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      249 2023-07-14 14:44:57.000000 idftools-0.1.4/README.md
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 16:37:52.343838 idftools-0.1.4/idftools/
+-rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.4/idftools/certificate.py
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.4/idftools/driversfactory.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 16:37:52.343838 idftools-0.1.4/idftools/idftools.egg-info/
+-rw-rw-r--   0 enio      (1000) enio      (1000)      668 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)      353 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/requires.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 16:37:52.000000 idftools-0.1.4/idftools/idftools.egg-info/top_level.txt
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.4/idftools/utilities.py
+-rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 16:37:52.343838 idftools-0.1.4/setup.cfg
+-rw-rw-r--   0 enio      (1000) enio      (1000)      819 2023-07-14 16:37:45.000000 idftools-0.1.4/setup.py
```

### Comparing `idftools-0.1.3/idftools/certificate.py` & `idftools-0.1.4/idftools/certificate.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.3/idftools/driversfactory.py` & `idftools-0.1.4/idftools/driversfactory.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.3/idftools/utilities.py` & `idftools-0.1.4/idftools/utilities.py`

 * *Files identical despite different names*

