# Comparing `tmp/thesisperu-0.4.tar.gz` & `tmp/thesisperu-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thesisperu-0.4.tar", last modified: Fri Jul 14 19:52:24 2023, max compression
+gzip compressed data, was "thesisperu-0.5.tar", last modified: Fri Jul 14 19:56:39 2023, max compression
```

## Comparing `thesisperu-0.4.tar` & `thesisperu-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:52:24.338403 thesisperu-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:52:15.000000 thesisperu-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:52:24.338403 thesisperu-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 19:52:15.000000 thesisperu-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:52:24.338403 thesisperu-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-14 19:52:15.000000 thesisperu-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:52:24.338403 thesisperu-0.4/thesisperu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:52:15.000000 thesisperu-0.4/thesisperu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-14 19:52:15.000000 thesisperu-0.4/thesisperu/scrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:52:15.000000 thesisperu-0.4/thesisperu/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:52:24.338403 thesisperu-0.4/thesisperu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:52:24.000000 thesisperu-0.4/thesisperu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 19:52:24.000000 thesisperu-0.4/thesisperu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:52:24.000000 thesisperu-0.4/thesisperu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 19:52:24.000000 thesisperu-0.4/thesisperu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 19:52:24.000000 thesisperu-0.4/thesisperu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:56:39.367410 thesisperu-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:56:26.000000 thesisperu-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:56:39.367410 thesisperu-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 19:56:26.000000 thesisperu-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:56:39.367410 thesisperu-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-14 19:56:26.000000 thesisperu-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:56:39.367410 thesisperu-0.5/thesisperu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:56:26.000000 thesisperu-0.5/thesisperu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-14 19:56:26.000000 thesisperu-0.5/thesisperu/scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:56:26.000000 thesisperu-0.5/thesisperu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:56:39.367410 thesisperu-0.5/thesisperu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 19:56:39.000000 thesisperu-0.5/thesisperu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 19:56:39.000000 thesisperu-0.5/thesisperu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:56:39.000000 thesisperu-0.5/thesisperu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 19:56:39.000000 thesisperu-0.5/thesisperu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 19:56:39.000000 thesisperu-0.5/thesisperu.egg-info/top_level.txt
```

### Comparing `thesisperu-0.4/thesisperu/scrapper.py` & `thesisperu-0.5/thesisperu/scrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,21 +46,21 @@
 
 	sub_items_df = sub_items_df.assign(
 		dir_name = name_links, num_thesis = num_thesis, urls = urls,
 		master_dir = master_dir
 	)
 	return sub_items_df
 
-def search_sub_items(main_items_df):
+def search_sub_items(main_items_df, prefix):
 	urls = main_items_df.urls.to_numpy()
 	name = main_items_df.dir_name.to_numpy()
 	sub_df = pd.DataFrame()
 
 	for i, url in tqdm.tqdm(enumerate(urls)):
-		sub_url_df = get_main_items(get_html(url), name[i])
+		sub_url_df = get_main_items(get_html(url), name[i], prefix=prefix)
 		sub_df = pd.concat((sub_df, sub_url_df))
 	return sub_df
 
 
 def get_thesis_metadata(url, master_dir='dir', sub_dir='sdir', prefix=None):
 	response = r.get(url, verify=False).content
 	meta_url = bs(response, 'html.parser')
```

