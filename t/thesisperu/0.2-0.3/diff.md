# Comparing `tmp/thesisperu-0.2.tar.gz` & `tmp/thesisperu-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thesisperu-0.2.tar", last modified: Fri Jul 14 19:47:39 2023, max compression
+gzip compressed data, was "thesisperu-0.3.tar", last modified: Fri Jul 14 19:51:01 2023, max compression
```

## Comparing `thesisperu-0.2.tar` & `thesisperu-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:47:39.186401 thesisperu-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:47:28.000000 thesisperu-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:47:39.186401 thesisperu-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 19:47:28.000000 thesisperu-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:47:39.186401 thesisperu-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-14 19:47:28.000000 thesisperu-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:47:39.186401 thesisperu-0.2/thesisperu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:47:28.000000 thesisperu-0.2/thesisperu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-14 19:47:28.000000 thesisperu-0.2/thesisperu/scrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:47:28.000000 thesisperu-0.2/thesisperu/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:47:39.186401 thesisperu-0.2/thesisperu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:47:38.000000 thesisperu-0.2/thesisperu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 19:47:39.000000 thesisperu-0.2/thesisperu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:47:38.000000 thesisperu-0.2/thesisperu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 19:47:38.000000 thesisperu-0.2/thesisperu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 19:47:38.000000 thesisperu-0.2/thesisperu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:51:01.071411 thesisperu-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:50:50.000000 thesisperu-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:51:01.071411 thesisperu-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 19:50:50.000000 thesisperu-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:51:01.071411 thesisperu-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-14 19:50:50.000000 thesisperu-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:51:01.071411 thesisperu-0.3/thesisperu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:50:50.000000 thesisperu-0.3/thesisperu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-14 19:50:50.000000 thesisperu-0.3/thesisperu/scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:50:50.000000 thesisperu-0.3/thesisperu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:51:01.071411 thesisperu-0.3/thesisperu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:51:00.000000 thesisperu-0.3/thesisperu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 19:51:01.000000 thesisperu-0.3/thesisperu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:51:00.000000 thesisperu-0.3/thesisperu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 19:51:00.000000 thesisperu-0.3/thesisperu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 19:51:00.000000 thesisperu-0.3/thesisperu.egg-info/top_level.txt
```

### Comparing `thesisperu-0.2/thesisperu/scrapper.py` & `thesisperu-0.3/thesisperu/scrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def get_html(url, element='div', css = 'artifact-description'):
 	response = r.get(url, verify=False).content
 	html = bs(response, 'html.parser')
 	s_items = html.find_all(element, class_ = css)
 	# return a sublinks 
 	return s_items
 
-def get_main_items(self, sub_items, master_dir = '', prefix = None):
+def get_main_items(sub_items, master_dir = '', prefix = None):
 
 	if prefix is None:
 		raise "No Prefix provided"
 
 	urls, num_thesis, name_links = [], [], []
 	sub_items_df = pd.DataFrame()
```

