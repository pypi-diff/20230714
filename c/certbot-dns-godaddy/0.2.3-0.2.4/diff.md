# Comparing `tmp/certbot_dns_godaddy-0.2.3.tar.gz` & `tmp/certbot_dns_godaddy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_dns_godaddy-0.2.3.tar", max compression
+gzip compressed data, was "certbot_dns_godaddy-0.2.4.tar", max compression
```

## Comparing `certbot_dns_godaddy-0.2.3.tar` & `certbot_dns_godaddy-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10786 2023-07-14 03:13:55.149754 certbot_dns_godaddy-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     5610 2023-07-14 03:13:55.149754 certbot_dns_godaddy-0.2.3/README.md
--rw-r--r--   0        0        0     4686 2023-07-14 03:13:55.149754 certbot_dns_godaddy-0.2.3/certbot_dns_godaddy.py
--rw-r--r--   0        0        0     1501 2023-07-14 03:13:55.153754 certbot_dns_godaddy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 certbot_dns_godaddy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10786 2023-07-14 05:49:16.095575 certbot_dns_godaddy-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     5610 2023-07-14 05:49:16.095575 certbot_dns_godaddy-0.2.4/README.md
+-rw-r--r--   0        0        0     4686 2023-07-14 05:49:16.095575 certbot_dns_godaddy-0.2.4/certbot_dns_godaddy.py
+-rw-r--r--   0        0        0     1501 2023-07-14 05:49:16.099575 certbot_dns_godaddy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 certbot_dns_godaddy-0.2.4/PKG-INFO
```

### Comparing `certbot_dns_godaddy-0.2.3/LICENSE.txt` & `certbot_dns_godaddy-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot_dns_godaddy-0.2.3/README.md` & `certbot_dns_godaddy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `certbot_dns_godaddy-0.2.3/certbot_dns_godaddy.py` & `certbot_dns_godaddy-0.2.4/certbot_dns_godaddy.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_godaddy-0.2.3/pyproject.toml` & `certbot_dns_godaddy-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "certbot-dns-godaddy"
-version = "0.2.3"
+version = "0.2.4"
 description = "A certbot plugin that implements letsencrypt dns wildcard support for godaddy using lexicon"
 authors = ["Dustyn Gibson <miigotu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/miigotu/certbot-dns-godaddy"
 
 packages = [{include = "certbot_dns_godaddy.py"}]
```

### Comparing `certbot_dns_godaddy-0.2.3/PKG-INFO` & `certbot_dns_godaddy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-godaddy
-Version: 0.2.3
+Version: 0.2.4
 Summary: A certbot plugin that implements letsencrypt dns wildcard support for godaddy using lexicon
 Home-page: https://github.com/miigotu/certbot-dns-godaddy
 License: Apache-2.0
 Author: Dustyn Gibson
 Author-email: miigotu@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 3 - Alpha
```

