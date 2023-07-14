# Comparing `tmp/coolfunc-1.1.3.tar.gz` & `tmp/coolfunc-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolfunc-1.1.3.tar", last modified: Sun Jul  9 14:37:41 2023, max compression
+gzip compressed data, was "coolfunc-1.1.4.tar", last modified: Fri Jul 14 17:49:57 2023, max compression
```

## Comparing `coolfunc-1.1.3.tar` & `coolfunc-1.1.4.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:26:56.463941 coolfunc-1.1.3/LICENSE
--rw-r--r--   0        0        0       13 2023-07-09 14:37:16.500843 coolfunc-1.1.3/coolfunc.py
--rw-r--r--   0        0        0      323 2023-07-09 14:37:28.579340 coolfunc-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      175 1970-01-01 00:00:00.000000 coolfunc-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.598742 coolfunc-1.1.4/LICENSE
+-rw-r--r--   0        0        0      420 2023-07-14 16:18:55.765669 coolfunc-1.1.4/README.md
+-rw-r--r--   0        0        0      269 2023-07-13 08:32:43.018342 coolfunc-1.1.4/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2838 2023-07-14 17:14:22.785588 coolfunc-1.1.4/coolfunc/_core.py
+-rw-r--r--   0        0        0      531 2023-07-14 17:49:57.441762 coolfunc-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 coolfunc-1.1.4/PKG-INFO
```

### Comparing `coolfunc-1.1.3/LICENSE` & `coolfunc-1.1.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -170,18 +170,22 @@
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
-   
+
 
    Copyright [2023] [lcctoor.com]
 
+   author: lcctoor.com
+   domain-name: lcctoor.com
+   email: lcctoor@outlook.com
+
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
```

