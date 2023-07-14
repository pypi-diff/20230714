# Comparing `tmp/vtype-1.1.1.tar.gz` & `tmp/vtype-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtype-1.1.1.tar", last modified: Sun Jul  9 14:39:10 2023, max compression
+gzip compressed data, was "vtype-1.1.2.tar", last modified: Fri Jul 14 17:49:46 2023, max compression
```

## Comparing `vtype-1.1.1.tar` & `vtype-1.1.2.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:26:56.463941 vtype-1.1.1/LICENSE
--rw-r--r--   0        0        0      320 2023-07-09 14:39:02.248047 vtype-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-09 14:37:16.500843 vtype-1.1.1/vtype.py
--rw-r--r--   0        0        0      172 1970-01-01 00:00:00.000000 vtype-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.601742 vtype-1.1.2/LICENSE
+-rw-r--r--   0        0        0      426 2023-07-14 16:35:39.816109 vtype-1.1.2/README.md
+-rw-r--r--   0        0        0      521 2023-07-14 17:49:46.433367 vtype-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-07-13 08:30:36.887445 vtype-1.1.2/vtype/__init__.py
+-rw-r--r--   0        0        0    10283 2023-07-14 17:14:22.785588 vtype-1.1.2/vtype/_core.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 vtype-1.1.2/PKG-INFO
```

### Comparing `vtype-1.1.1/LICENSE` & `vtype-1.1.2/LICENSE`

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

