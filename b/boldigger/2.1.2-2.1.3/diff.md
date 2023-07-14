# Comparing `tmp/boldigger-2.1.2.tar.gz` & `tmp/boldigger-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boldigger-2.1.2.tar", last modified: Wed Mar 15 16:18:22 2023, max compression
+gzip compressed data, was "boldigger-2.1.3.tar", last modified: Fri Jul 14 04:42:50 2023, max compression
```

## Comparing `boldigger-2.1.2.tar` & `boldigger-2.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 16:18:22.502108 boldigger-2.1.2/
--rw-rw-rw-   0        0        0     1093 2022-09-16 05:40:35.000000 boldigger-2.1.2/LICENSE
--rw-rw-rw-   0        0        0      135 2022-09-16 05:40:35.000000 boldigger-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9459 2023-03-15 16:18:22.502108 boldigger-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8940 2022-09-16 05:40:35.000000 boldigger-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 16:18:22.484101 boldigger-2.1.2/boldigger/
--rw-rw-rw-   0        0        0        2 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/__init__.py
--rw-rw-rw-   0        0        0     8141 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/__main__.py
--rw-rw-rw-   0        0        0     7542 2023-03-15 16:12:44.000000 boldigger-2.1.2/boldigger/additional_data.py
--rw-rw-rw-   0        0        0     9538 2023-03-15 16:17:21.000000 boldigger-2.1.2/boldigger/api_verification.py
--rw-rw-rw-   0        0        0    11979 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/boldblast_coi.py
--rw-rw-rw-   0        0        0     9827 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/boldblast_its.py
--rw-rw-rw-   0        0        0     4655 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/boldblast_rbcl.py
--rw-rw-rw-   0        0        0     3829 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/check_fasta.py
-drwxrwxrwx   0        0        0        0 2023-03-15 16:18:22.501109 boldigger-2.1.2/boldigger/data/
--rw-rw-rw-   0        0        0     5188 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/data/certs.pem
--rw-rw-rw-   0        0        0      771 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/data/github.png
--rw-rw-rw-   0        0        0    16352 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/data/logo.png
--rw-rw-rw-   0        0        0       34 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/data/userdata
--rw-rw-rw-   0        0        0     9535 2023-03-15 16:12:44.000000 boldigger-2.1.2/boldigger/digger_sort.py
--rw-rw-rw-   0        0        0     3537 2023-03-15 16:12:44.000000 boldigger-2.1.2/boldigger/first_hit.py
--rw-rw-rw-   0        0        0     7408 2023-03-15 16:12:44.000000 boldigger-2.1.2/boldigger/jamp_hit.py
--rw-rw-rw-   0        0        0     2014 2022-09-16 05:40:35.000000 boldigger-2.1.2/boldigger/login.py
-drwxrwxrwx   0        0        0        0 2023-03-15 16:18:22.498107 boldigger-2.1.2/boldigger.egg-info/
--rw-rw-rw-   0        0        0     9459 2023-03-15 16:18:22.000000 boldigger-2.1.2/boldigger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-03-15 16:18:22.000000 boldigger-2.1.2/boldigger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 16:18:22.000000 boldigger-2.1.2/boldigger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-03-15 16:18:22.000000 boldigger-2.1.2/boldigger.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      274 2023-03-15 16:18:22.000000 boldigger-2.1.2/boldigger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-15 16:18:22.000000 boldigger-2.1.2/boldigger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 16:18:22.502108 boldigger-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1441 2023-03-15 16:17:43.000000 boldigger-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:42:50.227879 boldigger-2.1.3/
+-rw-rw-rw-   0        0        0     1093 2022-09-16 05:40:35.000000 boldigger-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0      135 2022-09-16 05:40:35.000000 boldigger-2.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9514 2023-07-14 04:42:50.227879 boldigger-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8995 2023-07-14 04:39:14.000000 boldigger-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 04:42:50.212877 boldigger-2.1.3/boldigger/
+-rw-rw-rw-   0        0        0        2 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/__init__.py
+-rw-rw-rw-   0        0        0     8141 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/__main__.py
+-rw-rw-rw-   0        0        0     7542 2023-03-15 16:12:44.000000 boldigger-2.1.3/boldigger/additional_data.py
+-rw-rw-rw-   0        0        0     9538 2023-03-15 16:17:21.000000 boldigger-2.1.3/boldigger/api_verification.py
+-rw-rw-rw-   0        0        0    11979 2023-07-14 04:39:57.000000 boldigger-2.1.3/boldigger/boldblast_coi.py
+-rw-rw-rw-   0        0        0    12000 2023-07-14 04:40:07.000000 boldigger-2.1.3/boldigger/boldblast_its.py
+-rw-rw-rw-   0        0        0     5339 2023-07-14 04:40:12.000000 boldigger-2.1.3/boldigger/boldblast_rbcl.py
+-rw-rw-rw-   0        0        0     3829 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/check_fasta.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:42:50.226879 boldigger-2.1.3/boldigger/data/
+-rw-rw-rw-   0        0        0     5188 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/data/certs.pem
+-rw-rw-rw-   0        0        0      771 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/data/github.png
+-rw-rw-rw-   0        0        0    16352 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/data/logo.png
+-rw-rw-rw-   0        0        0       34 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/data/userdata
+-rw-rw-rw-   0        0        0     9535 2023-03-15 16:12:44.000000 boldigger-2.1.3/boldigger/digger_sort.py
+-rw-rw-rw-   0        0        0     3537 2023-03-15 16:12:44.000000 boldigger-2.1.3/boldigger/first_hit.py
+-rw-rw-rw-   0        0        0     7408 2023-03-15 16:12:44.000000 boldigger-2.1.3/boldigger/jamp_hit.py
+-rw-rw-rw-   0        0        0     2014 2022-09-16 05:40:35.000000 boldigger-2.1.3/boldigger/login.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:42:50.222878 boldigger-2.1.3/boldigger.egg-info/
+-rw-rw-rw-   0        0        0     9514 2023-07-14 04:42:50.000000 boldigger-2.1.3/boldigger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-14 04:42:50.000000 boldigger-2.1.3/boldigger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:42:50.000000 boldigger-2.1.3/boldigger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-14 04:42:50.000000 boldigger-2.1.3/boldigger.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      274 2023-07-14 04:42:50.000000 boldigger-2.1.3/boldigger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 04:42:50.000000 boldigger-2.1.3/boldigger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:42:50.227879 boldigger-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2023-07-14 04:42:40.000000 boldigger-2.1.3/setup.py
```

### Comparing `boldigger-2.1.2/LICENSE` & `boldigger-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/PKG-INFO` & `boldigger-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boldigger
-Version: 2.1.2
+Version: 2.1.3
 Summary: A python package to query different databases of boldsystems.org
 Home-page: https://github.com/DominikBuchner/BOLDigger
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,7 +118,8 @@
 
 ## Still to do
 
 * Implement the identification engine API for quick analyses
 * rework the command-line version with the new methods - will take some time
 * Add a failsafe to detect fasta format (2line, line-wrapping) and correct it before starting the search
 * Add failsaves for its and rbcl downloads
+* Add metadata async download to speed up the process
```

### Comparing `boldigger-2.1.2/README.md` & `boldigger-2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -103,7 +103,8 @@
 
 ## Still to do
 
 * Implement the identification engine API for quick analyses
 * rework the command-line version with the new methods - will take some time
 * Add a failsafe to detect fasta format (2line, line-wrapping) and correct it before starting the search
 * Add failsaves for its and rbcl downloads
+* Add metadata async download to speed up the process
```

### Comparing `boldigger-2.1.2/boldigger/__main__.py` & `boldigger-2.1.3/boldigger/__main__.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/additional_data.py` & `boldigger-2.1.3/boldigger/additional_data.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/api_verification.py` & `boldigger-2.1.3/boldigger/api_verification.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/boldblast_coi.py` & `boldigger-2.1.3/boldigger/boldblast_coi.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'tabtype': 'animalTabPane',
     'historicalDB': '',
     'searchdb': 'COX1',
     'sequence': query
     }
 
     ## send search request
-    r = session.post('https://boldsystems.org/index.php/IDS_IdentificationRequest', data = seq_data, timeout = 300)
+    r = session.post('https://boldsystems.org/index.php/IDS_IdentificationRequest', data = seq_data, timeout = 900)
 
     ## extract Top20 table links from the BOLD Result page
     soup = BSoup(r.text, 'html5lib')
     data = soup.find_all('span', style = 'text-decoration: none')
     data = ['http://boldsystems.org' + data[i].get('result') for i in range(len(data))]
 
     ## return the data
```

### Comparing `boldigger-2.1.2/boldigger/check_fasta.py` & `boldigger-2.1.3/boldigger/check_fasta.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/data/certs.pem` & `boldigger-2.1.3/boldigger/data/certs.pem`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/data/github.png` & `boldigger-2.1.3/boldigger/data/github.png`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/data/logo.png` & `boldigger-2.1.3/boldigger/data/logo.png`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/digger_sort.py` & `boldigger-2.1.3/boldigger/digger_sort.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/first_hit.py` & `boldigger-2.1.3/boldigger/first_hit.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/jamp_hit.py` & `boldigger-2.1.3/boldigger/jamp_hit.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger/login.py` & `boldigger-2.1.3/boldigger/login.py`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/boldigger.egg-info/PKG-INFO` & `boldigger-2.1.3/boldigger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boldigger
-Version: 2.1.2
+Version: 2.1.3
 Summary: A python package to query different databases of boldsystems.org
 Home-page: https://github.com/DominikBuchner/BOLDigger
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,7 +118,8 @@
 
 ## Still to do
 
 * Implement the identification engine API for quick analyses
 * rework the command-line version with the new methods - will take some time
 * Add a failsafe to detect fasta format (2line, line-wrapping) and correct it before starting the search
 * Add failsaves for its and rbcl downloads
+* Add metadata async download to speed up the process
```

### Comparing `boldigger-2.1.2/boldigger.egg-info/SOURCES.txt` & `boldigger-2.1.3/boldigger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boldigger-2.1.2/setup.py` & `boldigger-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="boldigger",
-    version="2.1.2",
+    version="2.1.3",
     author="Dominik Buchner",
     author_email="dominik.buchner524@googlemail.com",
     description="A python package to query different databases of boldsystems.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DominikBuchner/BOLDigger",
     packages=setuptools.find_packages(),
```

