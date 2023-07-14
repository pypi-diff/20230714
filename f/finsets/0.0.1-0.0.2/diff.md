# Comparing `tmp/finsets-0.0.1.tar.gz` & `tmp/finsets-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finsets-0.0.1.tar", last modified: Thu Jul 13 22:05:49 2023, max compression
+gzip compressed data, was "finsets-0.0.2.tar", last modified: Fri Jul 14 16:13:20 2023, max compression
```

## Comparing `finsets-0.0.1.tar` & `finsets-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.929661 finsets-0.0.1/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.797659 finsets-0.0.1/.github/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.837660 finsets-0.0.1/.github/workflows/
--rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 finsets-0.0.1/.github/workflows/deploy.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)      320 2023-07-10 02:37:15.000000 finsets-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-07-07 21:41:53.000000 finsets-0.0.1/.gitignore
--rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 finsets-0.0.1/LICENSE
--rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 finsets-0.0.1/MANIFEST.in
--rw-rw-r--   0 imb       (1000) imb       (1000)     3328 2023-07-13 22:05:49.929661 finsets-0.0.1/PKG-INFO
--rw-rw-r--   0 imb       (1000) imb       (1000)     2524 2023-07-12 22:25:43.000000 finsets-0.0.1/README.md
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.861660 finsets-0.0.1/finsets/
--rw-r--r--   0 imb       (1000) imb       (1000)       55 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)    14644 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/_modidx.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.889661 finsets-0.0.1/finsets/fred/
--rw-r--r--   0 imb       (1000) imb       (1000)       43 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/fred/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     5084 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/fred/fred.py
--rw-rw-r--   0 imb       (1000) imb       (1000)    19807 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/fred/fred_api.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.893661 finsets-0.0.1/finsets/papers/
--rw-r--r--   0 imb       (1000) imb       (1000)       38 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/papers/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     2731 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/papers/hassan_etal_2019.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.893661 finsets-0.0.1/finsets/wrds/
--rw-rw-r--   0 imb       (1000) imb       (1000)       45 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/wrds/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     9454 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/wrds/compa.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     3421 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/wrds/crspm.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     3243 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/wrds/linking.py
--rw-rw-r--   0 imb       (1000) imb       (1000)    26569 2023-07-12 22:52:36.000000 finsets-0.0.1/finsets/wrds/wrds_api.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.889661 finsets-0.0.1/finsets.egg-info/
--rw-r--r--   0 imb       (1000) imb       (1000)     3328 2023-07-13 22:05:49.000000 finsets-0.0.1/finsets.egg-info/PKG-INFO
--rw-r--r--   0 imb       (1000) imb       (1000)      689 2023-07-13 22:05:49.000000 finsets-0.0.1/finsets.egg-info/SOURCES.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-07-13 22:05:49.000000 finsets-0.0.1/finsets.egg-info/dependency_links.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       36 2023-07-13 22:05:49.000000 finsets-0.0.1/finsets.egg-info/entry_points.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-25 14:31:30.000000 finsets-0.0.1/finsets.egg-info/not-zip-safe
--rw-r--r--   0 imb       (1000) imb       (1000)       76 2023-07-13 22:05:49.000000 finsets-0.0.1/finsets.egg-info/requires.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        8 2023-07-13 22:05:49.000000 finsets-0.0.1/finsets.egg-info/top_level.txt
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-13 22:05:49.905661 finsets-0.0.1/nbs/
--rw-r--r--   0 imb       (1000) imb       (1000)      613 2023-07-12 22:35:51.000000 finsets-0.0.1/nbs/_quarto.yml
--rw-r--r--   0 imb       (1000) imb       (1000)     5437 2023-07-13 16:57:17.000000 finsets-0.0.1/nbs/index.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      258 2023-07-12 22:52:40.000000 finsets-0.0.1/nbs/nbdev.yml
--rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 finsets-0.0.1/nbs/styles.css
--rw-r--r--   0 imb       (1000) imb       (1000)     1060 2023-07-12 20:27:09.000000 finsets-0.0.1/settings.ini
--rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-07-13 22:05:49.929661 finsets-0.0.1/setup.cfg
--rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 finsets-0.0.1/setup.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.707991 finsets-0.0.2/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.699991 finsets-0.0.2/.github/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/.github/workflows/
+-rw-rw-r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 finsets-0.0.2/.github/workflows/deploy.yaml
+-rw-rw-r--   0 imb       (1000) imb       (1000)      320 2023-07-10 02:37:21.000000 finsets-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-07-07 21:41:53.000000 finsets-0.0.2/.gitignore
+-rw-rw-r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 finsets-0.0.2/LICENSE
+-rw-rw-r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 finsets-0.0.2/MANIFEST.in
+-rw-rw-r--   0 imb       (1000) imb       (1000)     5902 2023-07-14 16:13:20.703991 finsets-0.0.2/PKG-INFO
+-rw-rw-r--   0 imb       (1000) imb       (1000)     5098 2023-07-14 16:09:35.000000 finsets-0.0.2/README.md
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/data/
+-rw-r--r--   0 imb       (1000) imb       (1000)        0 2023-07-14 16:08:44.000000 finsets-0.0.2/data/.gitkeep
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/finsets/
+-rw-r--r--   0 imb       (1000) imb       (1000)       55 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/__init__.py
+-rw-rw-r--   0 imb       (1000) imb       (1000)    14755 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/_modidx.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/finsets/fred/
+-rw-r--r--   0 imb       (1000) imb       (1000)       43 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/fred/__init__.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     5547 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/fred/fred.py
+-rw-r--r--   0 imb       (1000) imb       (1000)    19807 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/fred/fred_api.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/finsets/papers/
+-rw-r--r--   0 imb       (1000) imb       (1000)       38 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/papers/__init__.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     2731 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/papers/hassan_etal_2019.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/finsets/wrds/
+-rw-r--r--   0 imb       (1000) imb       (1000)       45 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/wrds/__init__.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     9454 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/wrds/compa.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     3421 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/wrds/crspm.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     3243 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/wrds/linking.py
+-rw-r--r--   0 imb       (1000) imb       (1000)    26569 2023-07-14 16:08:43.000000 finsets-0.0.2/finsets/wrds/wrds_api.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/finsets.egg-info/
+-rw-r--r--   0 imb       (1000) imb       (1000)     5902 2023-07-14 16:13:20.000000 finsets-0.0.2/finsets.egg-info/PKG-INFO
+-rw-r--r--   0 imb       (1000) imb       (1000)      906 2023-07-14 16:13:20.000000 finsets-0.0.2/finsets.egg-info/SOURCES.txt
+-rw-rw-r--   0 imb       (1000) imb       (1000)        1 2023-07-14 16:13:20.000000 finsets-0.0.2/finsets.egg-info/dependency_links.txt
+-rw-rw-r--   0 imb       (1000) imb       (1000)       36 2023-07-14 16:13:20.000000 finsets-0.0.2/finsets.egg-info/entry_points.txt
+-rw-rw-r--   0 imb       (1000) imb       (1000)        1 2023-06-25 14:31:30.000000 finsets-0.0.2/finsets.egg-info/not-zip-safe
+-rw-r--r--   0 imb       (1000) imb       (1000)       76 2023-07-14 16:13:20.000000 finsets-0.0.2/finsets.egg-info/requires.txt
+-rw-rw-r--   0 imb       (1000) imb       (1000)        8 2023-07-14 16:13:20.000000 finsets-0.0.2/finsets.egg-info/top_level.txt
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/nbs/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/nbs/00_fred/
+-rw-r--r--   0 imb       (1000) imb       (1000)    44573 2023-07-14 16:08:48.000000 finsets-0.0.2/nbs/00_fred/00_fred.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)    24965 2023-07-10 22:15:45.000000 finsets-0.0.2/nbs/00_fred/01_fred_api.ipynb
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/nbs/01_wrds/
+-rw-r--r--   0 imb       (1000) imb       (1000)    49456 2023-07-14 13:10:54.000000 finsets-0.0.2/nbs/01_wrds/00_wrds_api.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)    15035 2023-07-12 22:25:27.000000 finsets-0.0.2/nbs/01_wrds/01_crspm.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)    36123 2023-07-12 22:25:27.000000 finsets-0.0.2/nbs/01_wrds/03_compa.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)    13414 2023-07-10 22:15:45.000000 finsets-0.0.2/nbs/01_wrds/linking.ipynb
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-07-14 16:13:20.703991 finsets-0.0.2/nbs/02_papers/
+-rw-r--r--   0 imb       (1000) imb       (1000)    39265 2023-07-12 22:25:27.000000 finsets-0.0.2/nbs/02_papers/hassan_etal_2019.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      613 2023-07-12 22:35:51.000000 finsets-0.0.2/nbs/_quarto.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)    10633 2023-07-14 16:08:48.000000 finsets-0.0.2/nbs/index.ipynb
+-rw-rw-r--   0 imb       (1000) imb       (1000)      258 2023-07-14 16:08:48.000000 finsets-0.0.2/nbs/nbdev.yml
+-rw-rw-r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 finsets-0.0.2/nbs/styles.css
+-rw-r--r--   0 imb       (1000) imb       (1000)      922 2023-07-14 16:08:38.000000 finsets-0.0.2/settings.ini
+-rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-07-14 16:13:20.707991 finsets-0.0.2/setup.cfg
+-rw-rw-r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 finsets-0.0.2/setup.py
```

### Comparing `finsets-0.0.1/.gitignore` & `finsets-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/LICENSE` & `finsets-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets/_modidx.py` & `finsets-0.0.2/finsets/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/finsets',
                 'doc_host': 'https://ionmihai.github.io',
                 'git_url': 'https://github.com/ionmihai/finsets',
                 'lib_path': 'finsets'},
-  'syms': { 'finsets.fred.fred': { 'finsets.fred.fred.common_raw_vars': ('00_fred/fred.html#common_raw_vars', 'finsets/fred/fred.py'),
-                                   'finsets.fred.fred.get_series': ('00_fred/fred.html#get_series', 'finsets/fred/fred.py'),
+  'syms': { 'finsets.fred.fred': { 'finsets.fred.fred.clean': ('00_fred/fred.html#clean', 'finsets/fred/fred.py'),
+                                   'finsets.fred.fred.common_raw_vars': ('00_fred/fred.html#common_raw_vars', 'finsets/fred/fred.py'),
+                                   'finsets.fred.fred.download': ('00_fred/fred.html#download', 'finsets/fred/fred.py'),
                                    'finsets.fred.fred.get_series_info': ('00_fred/fred.html#get_series_info', 'finsets/fred/fred.py'),
                                    'finsets.fred.fred.search': ('00_fred/fred.html#search', 'finsets/fred/fred.py')},
             'finsets.fred.fred_api': { 'finsets.fred.fred_api.Fred': ('00_fred/fred_api.html#fred', 'finsets/fred/fred_api.py'),
                                        'finsets.fred.fred_api.Fred.__do_series_search': ( '00_fred/fred_api.html#fred.__do_series_search',
                                                                                           'finsets/fred/fred_api.py'),
                                        'finsets.fred.fred_api.Fred.__fetch_data': ( '00_fred/fred_api.html#fred.__fetch_data',
                                                                                     'finsets/fred/fred_api.py'),
```

### Comparing `finsets-0.0.1/finsets/fred/fred.py` & `finsets-0.0.2/finsets/fred/fred.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/00_fred/00_fred.ipynb.
 
 # %% auto 0
-__all__ = ['get_series', 'get_series_info', 'search', 'common_raw_vars']
+__all__ = ['download', 'clean', 'get_series_info', 'search', 'common_raw_vars']
 
 # %% ../../nbs/00_fred/00_fred.ipynb 4
 import os, time
 
 import pandas as pd
 from .fred_api import Fred
 
 import pandasmore as pdm
 
 # %% ../../nbs/00_fred/00_fred.ipynb 5
-def get_series(series: str=None, # FRED series name
+def download(series: str=None, # FRED series name
+               api_key: str=None # FRED api key. If None, will use os.getenv("FRED_API_KEY")
+               ) -> pd.DataFrame: 
+    """Retrieves series from FRED and returns it as a pd.DataFrame."""
+
+    if api_key is None: api_key = os.getenv("FRED_API_KEY")
+    api = Fred(api_key=api_key)
+    return api.get_series(series).to_frame(name=series)
+
+# %% ../../nbs/00_fred/00_fred.ipynb 7
+def clean(series: str=None, # FRED series name
                label: str=None, # Name you want to give to the series in the output DataFrame. If None, use lowercase of `series`
                api_key: str=None # FRED api key. If None, will use os.getenv("FRED_API_KEY")
                ) -> pd.DataFrame: 
     """Retrieves series from FRED, cleans the date and sets it as index"""
 
     if api_key is None: api_key = os.getenv("FRED_API_KEY")
     api = Fred(api_key=api_key)
     freq = api.get_series_info('GDP').frequency_short 
+    time.sleep(1)
     if label is None: label = str.lower(series)
-    df = api.get_series(series).to_frame(name=label).reset_index().rename({'index':'date'},axis=1)
+    df = download(series).rename(columns={series:label}).reset_index().rename({'index':'date'},axis=1)
     df = pdm.setup_tseries(df, freq=freq).drop('date', axis=1)
     return df 
 
-# %% ../../nbs/00_fred/00_fred.ipynb 7
+# %% ../../nbs/00_fred/00_fred.ipynb 9
 def get_series_info(series: str=None, # FRED series name
                     api_key: str=None # FRED api key. If None, will use os.getenv("FRED_API_KEY")
                     ) -> pd.Series:
     """Get metadata from FRED for given `series` from FRED"""
 
     if api_key is None: api_key = os.getenv("FRED_API_KEY")
     api = Fred(api_key=api_key)
     return api.get_series_info(series)
 
-# %% ../../nbs/00_fred/00_fred.ipynb 9
+# %% ../../nbs/00_fred/00_fred.ipynb 11
 def search(search_text: str=None, # What to search for
               order_by: str='popularity', # How to order search results; try `search_rank` if you don't find what you were looking for
               nr_results: int=10, # How many results to output
               api_key: str=None # FRED api key. If None, will use os.getenv("FRED_API_KEY")
               ) -> pd.DataFrame:
     """Search FRED for a given `search_text`, sort by popularity and return only the first `nr_results`"""
 
     if api_key is None: api_key = os.getenv("FRED_API_KEY")
     api = Fred(api_key=api_key)  
     return api.search(search_text, order_by=order_by)\
               .pipe(pdm.order_columns, ['title', 'popularity','frequency_short', 'observation_start', 'observation_end'])\
               .iloc[:nr_results]
               
 
-# %% ../../nbs/00_fred/00_fred.ipynb 12
+# %% ../../nbs/00_fred/00_fred.ipynb 14
 def common_raw_vars() -> pd.DataFrame:
     """List of FRED series commonly used in finance research"""
 
     vars = [
     ['TB3MS','yield_3mt','3-month treasury bill secondary market rate', 'M', 'NSA',1934],
     ['DTB3','yield_3mt','3-month treasury bill secondary market rate', 'D', 'NSA',1954],
     ['GS10','yield_10yt','10-year treasury constant maturity market yield', 'M', 'NSA',1953],
```

### Comparing `finsets-0.0.1/finsets/fred/fred_api.py` & `finsets-0.0.2/finsets/fred/fred_api.py`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets/papers/hassan_etal_2019.py` & `finsets-0.0.2/finsets/papers/hassan_etal_2019.py`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets/wrds/compa.py` & `finsets-0.0.2/finsets/wrds/compa.py`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets/wrds/crspm.py` & `finsets-0.0.2/finsets/wrds/crspm.py`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets/wrds/linking.py` & `finsets-0.0.2/finsets/wrds/linking.py`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets/wrds/wrds_api.py` & `finsets-0.0.2/finsets/wrds/wrds_api.py`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/finsets.egg-info/SOURCES.txt` & `finsets-0.0.2/finsets.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 .github/workflows/deploy.yaml
 .github/workflows/test.yaml
+data/.gitkeep
 finsets/__init__.py
 finsets/_modidx.py
 finsets.egg-info/PKG-INFO
 finsets.egg-info/SOURCES.txt
 finsets.egg-info/dependency_links.txt
 finsets.egg-info/entry_points.txt
 finsets.egg-info/not-zip-safe
@@ -24,8 +25,15 @@
 finsets/wrds/compa.py
 finsets/wrds/crspm.py
 finsets/wrds/linking.py
 finsets/wrds/wrds_api.py
 nbs/_quarto.yml
 nbs/index.ipynb
 nbs/nbdev.yml
-nbs/styles.css
+nbs/styles.css
+nbs/00_fred/00_fred.ipynb
+nbs/00_fred/01_fred_api.ipynb
+nbs/01_wrds/00_wrds_api.ipynb
+nbs/01_wrds/01_crspm.ipynb
+nbs/01_wrds/03_compa.ipynb
+nbs/01_wrds/linking.ipynb
+nbs/02_papers/hassan_etal_2019.ipynb
```

### Comparing `finsets-0.0.1/nbs/_quarto.yml` & `finsets-0.0.2/nbs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/nbs/styles.css` & `finsets-0.0.2/nbs/styles.css`

 * *Files identical despite different names*

### Comparing `finsets-0.0.1/settings.ini` & `finsets-0.0.2/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = finsets
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = finsets
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
-
-### nbdev ###
 doc_path = _docs
 lib_path = finsets
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = True
 custom_quarto_yml = True
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://ionmihai.github.io
+doc_baseurl = /finsets
+git_url = https://github.com/ionmihai/finsets
+title = finsets
 audience = Developers
 author = Mihai Ion
 author_email = mihaiion@email.arizona.edu
-copyright = 2023 onwards, %(author)s
+copyright = 2023 onwards, Mihai Ion
 description = Download and process datasets commonly used in finance research
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = ionmihai
-
-### Optional ###
 requirements = fastcore pandas numpy psycopg2-binary sqlalchemy<2 estout pandasmore
-# dev_requirements = 
-# console_scripts =
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `finsets-0.0.1/setup.py` & `finsets-0.0.2/setup.py`

 * *Files identical despite different names*

