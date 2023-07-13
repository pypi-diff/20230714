# Comparing `tmp/search-me-3.0.0.tar.gz` & `tmp/search-me-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search-me-3.0.0.tar", last modified: Tue Jul  4 15:39:55 2023, max compression
+gzip compressed data, was "search-me-3.1.0.tar", last modified: Thu Jul 13 22:55:15 2023, max compression
```

## Comparing `search-me-3.0.0.tar` & `search-me-3.1.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.921924 search-me-3.0.0/
--rw-rw-rw-   0        0        0     1096 2023-07-04 15:26:23.000000 search-me-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     4485 2023-07-04 15:39:55.923925 search-me-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2795 2023-07-04 15:37:06.000000 search-me-3.0.0/README.md
--rw-rw-rw-   0        0        0     2087 2023-07-04 15:26:23.000000 search-me-3.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.854920 search-me-3.0.0/search_me/
-drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.917924 search-me-3.0.0/search_me/.engines/
--rw-rw-rw-   0        0        0     1892 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.domains
--rw-rw-rw-   0        0        0      248 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.formats
--rw-rw-rw-   0        0        0     1188 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.languages
--rw-rw-rw-   0        0        0      312 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.params
--rw-rw-rw-   0        0        0     1024 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.pass
--rw-rw-rw-   0        0        0      332 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.regex
--rw-rw-rw-   0        0        0     1024 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/.engines/.salt
--rw-rw-rw-   0        0        0      554 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/__init__.py
--rw-rw-rw-   0        0        0     4198 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/balancers.py
--rw-rw-rw-   0        0        0    12426 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/engines.py
--rw-rw-rw-   0        0        0     1932 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/exceptions.py
--rw-rw-rw-   0        0        0      389 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/models.py
--rw-rw-rw-   0        0        0     4846 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/storage.py
--rw-rw-rw-   0        0        0     2510 2023-07-04 15:26:23.000000 search-me-3.0.0/search_me/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:39:55.884922 search-me-3.0.0/search_me.egg-info/
--rw-rw-rw-   0        0        0     4485 2023-07-04 15:39:54.000000 search-me-3.0.0/search_me.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-04 15:39:54.000000 search-me-3.0.0/search_me.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 15:39:55.000000 search-me-3.0.0/search_me.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2895 2023-07-04 15:39:55.927925 search-me-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-07-04 15:26:23.000000 search-me-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:55:15.091151 search-me-3.1.0/
+-rw-rw-rw-   0        0        0     1096 2023-07-04 15:26:23.000000 search-me-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4486 2023-07-13 22:55:15.093151 search-me-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2796 2023-07-13 22:53:01.000000 search-me-3.1.0/README.md
+-rw-rw-rw-   0        0        0     2154 2023-07-13 14:48:34.000000 search-me-3.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-13 22:55:14.948142 search-me-3.1.0/search_me/
+drwxrwxrwx   0        0        0        0 2023-07-13 22:55:15.033147 search-me-3.1.0/search_me/.engines/
+-rw-rw-rw-   0        0        0     1892 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.domains
+-rw-rw-rw-   0        0        0      248 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.formats
+-rw-rw-rw-   0        0        0     1188 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.languages
+-rw-rw-rw-   0        0        0      312 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.params
+-rw-rw-rw-   0        0        0     1024 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.pass
+-rw-rw-rw-   0        0        0      332 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.regex
+-rw-rw-rw-   0        0        0     1024 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/.engines/.salt
+-rw-rw-rw-   0        0        0   218828 2023-07-12 17:46:27.000000 search-me-3.1.0/search_me/.engines/.useragents
+drwxrwxrwx   0        0        0        0 2023-07-13 22:55:15.086150 search-me-3.1.0/search_me/.osint/
+-rw-rw-rw-   0        0        0     4324 2023-07-13 20:05:53.000000 search-me-3.1.0/search_me/.osint/.code
+-rw-rw-rw-   0        0        0   455416 2023-07-13 20:05:54.000000 search-me-3.1.0/search_me/.osint/.dorks
+-rw-rw-rw-   0        0        0     2148 2023-07-13 20:05:54.000000 search-me-3.1.0/search_me/.osint/.gov
+-rw-rw-rw-   0        0        0    20664 2023-07-13 20:05:54.000000 search-me-3.1.0/search_me/.osint/.main
+-rw-rw-rw-   0        0        0      312 2023-07-13 20:05:54.000000 search-me-3.1.0/search_me/.osint/.swap
+-rw-rw-rw-   0        0        0      554 2023-07-13 22:21:38.000000 search-me-3.1.0/search_me/__init__.py
+-rw-rw-rw-   0        0        0     4198 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/balancers.py
+-rw-rw-rw-   0        0        0    12168 2023-07-13 07:15:11.000000 search-me-3.1.0/search_me/engines.py
+-rw-rw-rw-   0        0        0     2177 2023-07-13 07:06:27.000000 search-me-3.1.0/search_me/exceptions.py
+-rw-rw-rw-   0        0        0      389 2023-07-04 15:26:23.000000 search-me-3.1.0/search_me/models.py
+-rw-rw-rw-   0        0        0     9984 2023-07-13 19:52:42.000000 search-me-3.1.0/search_me/osint.py
+-rw-rw-rw-   0        0        0     2005 2023-07-13 07:16:03.000000 search-me-3.1.0/search_me/services.py
+-rw-rw-rw-   0        0        0     5038 2023-07-12 18:39:51.000000 search-me-3.1.0/search_me/storage.py
+-rw-rw-rw-   0        0        0     3393 2023-07-13 07:18:40.000000 search-me-3.1.0/search_me/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:55:14.982144 search-me-3.1.0/search_me.egg-info/
+-rw-rw-rw-   0        0        0     4486 2023-07-13 22:55:14.000000 search-me-3.1.0/search_me.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-07-13 22:55:14.000000 search-me-3.1.0/search_me.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 22:55:14.000000 search-me-3.1.0/search_me.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 22:55:14.000000 search-me-3.1.0/search_me.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      139 2023-07-13 22:55:14.000000 search-me-3.1.0/search_me.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 22:55:14.000000 search-me-3.1.0/search_me.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3029 2023-07-13 22:55:15.097151 search-me-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-07-04 15:26:23.000000 search-me-3.1.0/setup.py
```

### Comparing `search-me-3.0.0/LICENSE` & `search-me-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `search-me-3.0.0/PKG-INFO` & `search-me-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-me
-Version: 3.0.0
+Version: 3.1.0
 Summary: Search in Google, Bing, Brave, Mojeek, Moose, Yahoo, Searx
 Home-page: https://bit.ly/bitbucket-search-me
 Download-URL: https://bit.ly/search-me-dwnld
 Author: Michael R. Kisel
 Author-email: deploy-me@yandex.ru
 Maintainer: Michael R. Kisel <deploy-me@yandex.ru>
 Maintainer-email: deploy-me@yandex.ru
@@ -45,15 +45,15 @@
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/v/search-me.svg?style=flat-square&logo=appveyor" alt="Version"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/l/search-me.svg?style=flat-square&logo=appveyor&color=blueviolet" alt="License"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/pyversions/search-me.svg?style=flat-square&logo=appveyor" alt="Python"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/status/search-me.svg?style=flat-square&logo=appveyor" alt="Status"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/format/search-me.svg?style=flat-square&logo=appveyor&color=yellow" alt="Format"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/wheel/search-me.svg?style=flat-square&logo=appveyor&color=red" alt="Wheel"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/bitbucket/pipelines/deploy-me/search-me/master?style=flat-square&logo=appveyor" alt="Build"></a>
-    <a href="https://pypi.org/projectsearch-me"><img src="https://bit.ly/sm-cov" alt="Coverage"></a>
+    <a href="https://pypi.org/project/search-me"><img src="https://bit.ly/sm-cov" alt="Coverage"></a>
     <a href="https://pepy.tech/project/search-me"><img src="https://static.pepy.tech/personalized-badge/search-me?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
     <br><br><br>
 </p>
 
 # SEARCH-ME
 
 Search in Google, Bing, Brave, Mojeek, Moose, Yahoo, Searx. See more in [documentation](https://deploy-me.bitbucket.io/search-me/index.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: search-me Version: 3.0.0 Summary: Search in Google,
+Metadata-Version: 2.1 Name: search-me Version: 3.1.0 Summary: Search in Google,
 Bing, Brave, Mojeek, Moose, Yahoo, Searx Home-page: https://bit.ly/bitbucket-
 search-me Download-URL: https://bit.ly/search-me-dwnld Author: Michael R. Kisel
 Author-email: deploy-me@yandex.ru Maintainer: Michael R. Kisel
 yandex.ru> Maintainer-email: deploy-me@yandex.ru License: MIT Keywords:
 google,bing,brave,mojeek,moose,yahoo,searx,async,async search,aiohttp,web
 search,async scraper,osint Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Framework ::
```

### Comparing `search-me-3.0.0/README.md` & `search-me-3.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/v/search-me.svg?style=flat-square&logo=appveyor" alt="Version"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/l/search-me.svg?style=flat-square&logo=appveyor&color=blueviolet" alt="License"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/pyversions/search-me.svg?style=flat-square&logo=appveyor" alt="Python"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/status/search-me.svg?style=flat-square&logo=appveyor" alt="Status"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/format/search-me.svg?style=flat-square&logo=appveyor&color=yellow" alt="Format"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/wheel/search-me.svg?style=flat-square&logo=appveyor&color=red" alt="Wheel"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/bitbucket/pipelines/deploy-me/search-me/master?style=flat-square&logo=appveyor" alt="Build"></a>
-    <a href="https://pypi.org/projectsearch-me"><img src="https://bit.ly/sm-cov" alt="Coverage"></a>
+    <a href="https://pypi.org/project/search-me"><img src="https://bit.ly/sm-cov" alt="Coverage"></a>
     <a href="https://pepy.tech/project/search-me"><img src="https://static.pepy.tech/personalized-badge/search-me?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
     <br><br><br>
 </p>
 
 # SEARCH-ME
 
 Search in Google, Bing, Brave, Mojeek, Moose, Yahoo, Searx. See more in [documentation](https://deploy-me.bitbucket.io/search-me/index.html)
```

### Comparing `search-me-3.0.0/pyproject.toml` & `search-me-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "search-me"
-version = "3.0.0"
+version = "3.1.0"
 description = "Search in Google, Bing, Brave, Mojeek, Moose, Yahoo, Searx"
 license = "MIT"
 authors = ["Michael R. Kisel <deploy-me@yandex.ru>"]
 maintainers = ["Michael R. Kisel <deploy-me@yandex.ru>"]
 readme = "README.md"
 homepage = "https://bit.ly/bitbucket-search-me"
 documentation = "https://bit.ly/search-me-docs"
@@ -38,26 +38,28 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 aiohttp = "3.8.4"
 pandas = "2.0.2"
 cryptography = "41.0.1"
 bs4 = "0.0.1"
+jmespath = "1.0.1"
+tabulate = "0.9.0"
 importlib_resources = "*"
 
 [tool.poetry.dev-dependencies]
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.1.0"
 coverage-badge = "*"
 pylint = "2.17.4"
 pdoc3 = "*"
 twine = "*"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.coverage.run]
-omit = ["test_*", "fixtures.py", "exceptions.py"]
+omit = ["test_*", "fixtures.py", "exceptions.py", "osint.py", "services.py"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `search-me-3.0.0/search_me/.engines/.domains` & `search-me-3.1.0/search_me/.engines/.domains`

 * *Files identical despite different names*

### Comparing `search-me-3.0.0/search_me/.engines/.languages` & `search-me-3.1.0/search_me/.engines/.languages`

 * *Files identical despite different names*

### Comparing `search-me-3.0.0/search_me/.engines/.pass` & `search-me-3.1.0/search_me/.engines/.pass`

 * *Files identical despite different names*

### Comparing `search-me-3.0.0/search_me/.engines/.salt` & `search-me-3.1.0/search_me/.engines/.salt`

 * *Files identical despite different names*

### Comparing `search-me-3.0.0/search_me/__init__.py` & `search-me-3.1.0/search_me/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 __author__ = "Michael R. Kisel"
 __license__ = "MIT"
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 __maintainer__ = "Michael R. Kisel"
 __email__ = "deploy-me@yandex.ru"
 __status__ = "Stable"
 
 
 __all__ = (
     "Google", "Bing", "Brave", "Mojeek", "Moose", "Yahoo", "Searx", "Etools"
```

### Comparing `search-me-3.0.0/search_me/balancers.py` & `search-me-3.1.0/search_me/balancers.py`

 * *Files identical despite different names*

### Comparing `search-me-3.0.0/search_me/engines.py` & `search-me-3.1.0/search_me/engines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import logging
 import time
 from functools import cached_property
 from pathlib import Path
-try:
-    from importlib.resources import files
-except ImportError:
-    from importlib_resources import files
 from aiohttp.client_exceptions import ClientConnectorError
 from bs4 import BeautifulSoup
 from numpy import where
 from search_me.balancers import RR, DWRR
 from search_me.exceptions import (
     SearchEngineRequestError, SearchEngineAccessError, SearchEngineFormatError
 )
 from search_me.models import SearchResult as Response
 from search_me.storage import SafeStorage as Storage
-from search_me.tools import retry, check_params
+from search_me.tools import retry, check_params, get_current_dir
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class SearchEngine:
@@ -79,30 +75,26 @@
         """Load data from files
 
         Raises
         ------
         SearchEngineFormatError
             Raised if not found right format
         """
-        try:
-            root_dir = files("search_me")
-        except ModuleNotFoundError:
-            root_dir = Path(__file__).parent
-        cur_dir = root_dir / f".{Path(__file__).name.split('.')[0]}"
+        workdir = get_current_dir() / f".{Path(__file__).name.split('.')[0]}"
 
-        with Storage.load(cur_dir / ".salt", cur_dir / ".pass") as loader:
-            df_domains = loader.send(cur_dir / ".domains")
+        with Storage.load(workdir / ".salt", workdir / ".pass") as loader:
+            df_domains = loader.send(workdir / ".domains")
             next(loader)
-            df_languages = loader.send(cur_dir / ".languages")
+            df_languages = loader.send(workdir / ".languages")
             next(loader)
-            df_regex= loader.send(cur_dir / ".regex")
+            df_regex= loader.send(workdir / ".regex")
             next(loader)
-            df_formats = loader.send(cur_dir / ".formats")
+            df_formats = loader.send(workdir / ".formats")
             next(loader)
-            df_params = loader.send(cur_dir / ".params")
+            df_params = loader.send(workdir / ".params")
             next(loader)
 
         domains, languages, regex, output_format, default_params = (
             self.df_to_list_filter_by_engine(df_domains),
             self.df_to_list_filter_by_engine(df_languages),
             self.df_to_list_filter_by_engine(df_regex),
             self.df_to_list_filter_by_engine(df_formats),
@@ -404,18 +396,17 @@
             if status_code == 200:
                 if self.is_html:
                     content = await resp.text()
                 else:
                     content = await resp.json()
                 self.recalc_domain_weights(domain, 1)
                 return content
-            else:
-                self.recalc_domain_weights(domain, -1)
-                time.sleep(self.default_kwargs.get("delay", 0))
-                raise SearchEngineRequestError(domain, status_code)
+            self.recalc_domain_weights(domain, -1)
+            time.sleep(self.default_kwargs.get("delay", 0))
+            raise SearchEngineRequestError(domain, status_code)
 
     def recalc_domain_weights(self, domain, w):
         """Recalc weights for item
 
         Parameters
         ----------
         domain : str
```

### Comparing `search-me-3.0.0/search_me/exceptions.py` & `search-me-3.1.0/search_me/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,7 +81,22 @@
 
         Returns
         -------
         str
             String representation
         """
         return f"Set up params {self.params}"
+
+
+class ApiError(Exception):
+    """Api Error
+    """
+
+    def __str__(self):
+        """Str method
+
+        Returns
+        -------
+        str
+            String representation
+        """
+        return "Provide valid API key"
```

### Comparing `search-me-3.0.0/search_me/storage.py` & `search-me-3.1.0/search_me/storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import logging
 from base64 import urlsafe_b64encode
 from contextlib import contextmanager
 from io import BytesIO
-from os import urandom
+from os import urandom, path
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from pandas import read_json
 
 
 logger = logging.getLogger(__name__)
@@ -99,15 +99,17 @@
             Password path
 
         Yields
         ------
         None
             None
         """
-        __key__ = cls.load_key(cls.save_salt(filepath_pass), cls.save_salt(filepath_salt))
+        raw_pass = cls.load_salt(filepath_pass) if path.exists(filepath_pass) else cls.save_salt(filepath_pass)
+        raw_salt = cls.load_salt(filepath_salt) if path.exists(filepath_salt) else cls.save_salt(filepath_salt)
+        __key__ = cls.load_key(raw_pass, raw_salt)
         p1, p2 = None, None
         while True:
             df_path, df = yield p1, p2
             with BytesIO() as df_stream, open(df_path, "wb") as f:
                 df.to_json(df_stream, orient=cls.ORIENT, compression=cls.COMP)
                 df_stream.seek(0)
                 f.write(__key__.encrypt(df_stream.read()))
```

### Comparing `search-me-3.0.0/search_me/tools.py` & `search-me-3.1.0/search_me/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # -*- coding: utf-8 -*-
 import logging
 from functools import wraps
-from search_me.exceptions import SearchEngineParamsError
+try:
+    from importlib.resources import files
+except ImportError:
+    from importlib_resources import files
+from pathlib import Path
+from search_me.exceptions import SearchEngineParamsError, ApiError
 
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 def retry(exceptions):
@@ -99,7 +104,48 @@
     @wraps(func)
     def wrapper(*args, **kwargs):
         item = func(*args, **kwargs)
         if item:
             args[0].calls[item] += 1
         return item
     return wrapper
+
+
+def validate_api_key(func):
+    """Raise api error
+
+    Parameters
+    ----------
+    func : function
+        Function
+
+    Returns
+    -------
+    Any
+        Function result
+
+    Raises
+    ------
+    SearchMeApiError
+        If api key not valid
+    """
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except (ValueError, FileNotFoundError) as e:
+            raise ApiError() from e
+    return wrapper
+
+
+def get_current_dir():
+    """Get current dir
+
+    Returns
+    -------
+    str
+        Current dir
+    """
+    try:
+        return files(__package__)
+    except ModuleNotFoundError:
+        return Path(__file__).parent
```

### Comparing `search-me-3.0.0/search_me.egg-info/PKG-INFO` & `search-me-3.1.0/search_me.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: search-me
-Version: 3.0.0
+Version: 3.1.0
 Summary: Search in Google, Bing, Brave, Mojeek, Moose, Yahoo, Searx
 Home-page: https://bit.ly/bitbucket-search-me
 Download-URL: https://bit.ly/search-me-dwnld
 Author: Michael R. Kisel
 Author-email: deploy-me@yandex.ru
 Maintainer: Michael R. Kisel <deploy-me@yandex.ru>
 Maintainer-email: deploy-me@yandex.ru
@@ -45,15 +45,15 @@
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/v/search-me.svg?style=flat-square&logo=appveyor" alt="Version"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/l/search-me.svg?style=flat-square&logo=appveyor&color=blueviolet" alt="License"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/pyversions/search-me.svg?style=flat-square&logo=appveyor" alt="Python"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/status/search-me.svg?style=flat-square&logo=appveyor" alt="Status"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/format/search-me.svg?style=flat-square&logo=appveyor&color=yellow" alt="Format"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/pypi/wheel/search-me.svg?style=flat-square&logo=appveyor&color=red" alt="Wheel"></a>
     <a href="https://pypi.org/project/search-me"><img src="https://img.shields.io/bitbucket/pipelines/deploy-me/search-me/master?style=flat-square&logo=appveyor" alt="Build"></a>
-    <a href="https://pypi.org/projectsearch-me"><img src="https://bit.ly/sm-cov" alt="Coverage"></a>
+    <a href="https://pypi.org/project/search-me"><img src="https://bit.ly/sm-cov" alt="Coverage"></a>
     <a href="https://pepy.tech/project/search-me"><img src="https://static.pepy.tech/personalized-badge/search-me?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
     <br><br><br>
 </p>
 
 # SEARCH-ME
 
 Search in Google, Bing, Brave, Mojeek, Moose, Yahoo, Searx. See more in [documentation](https://deploy-me.bitbucket.io/search-me/index.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: search-me Version: 3.0.0 Summary: Search in Google,
+Metadata-Version: 2.1 Name: search-me Version: 3.1.0 Summary: Search in Google,
 Bing, Brave, Mojeek, Moose, Yahoo, Searx Home-page: https://bit.ly/bitbucket-
 search-me Download-URL: https://bit.ly/search-me-dwnld Author: Michael R. Kisel
 Author-email: deploy-me@yandex.ru Maintainer: Michael R. Kisel
 yandex.ru> Maintainer-email: deploy-me@yandex.ru License: MIT Keywords:
 google,bing,brave,mojeek,moose,yahoo,searx,async,async search,aiohttp,web
 search,async scraper,osint Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Framework ::
```

### Comparing `search-me-3.0.0/search_me.egg-info/SOURCES.txt` & `search-me-3.1.0/search_me.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,30 @@
 setup.cfg
 setup.py
 search_me/__init__.py
 search_me/balancers.py
 search_me/engines.py
 search_me/exceptions.py
 search_me/models.py
+search_me/osint.py
+search_me/services.py
 search_me/storage.py
 search_me/tools.py
 search_me.egg-info/PKG-INFO
 search_me.egg-info/SOURCES.txt
 search_me.egg-info/dependency_links.txt
 search_me.egg-info/not-zip-safe
 search_me.egg-info/requires.txt
 search_me.egg-info/top_level.txt
 search_me/.engines/.domains
 search_me/.engines/.formats
 search_me/.engines/.languages
 search_me/.engines/.params
 search_me/.engines/.pass
 search_me/.engines/.regex
-search_me/.engines/.salt
+search_me/.engines/.salt
+search_me/.engines/.useragents
+search_me/.osint/.code
+search_me/.osint/.dorks
+search_me/.osint/.gov
+search_me/.osint/.main
+search_me/.osint/.swap
```

### Comparing `search-me-3.0.0/setup.cfg` & `search-me-3.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6561 7263 682d 6d65 0d0a 7665   = search-me..ve
-00000020: 7273 696f 6e20 3d20 332e 302e 300d 0a75  rsion = 3.0.0..u
+00000020: 7273 696f 6e20 3d20 332e 312e 300d 0a75  rsion = 3.1.0..u
 00000030: 726c 203d 2068 7474 7073 3a2f 2f62 6974  rl = https://bit
 00000040: 2e6c 792f 6269 7462 7563 6b65 742d 7365  .ly/bitbucket-se
 00000050: 6172 6368 2d6d 650d 0a68 6f6d 655f 7061  arch-me..home_pa
 00000060: 6765 203d 2068 7474 7073 3a2f 2f62 6974  ge = https://bit
 00000070: 2e6c 792f 6269 7462 7563 6b65 742d 7365  .ly/bitbucket-se
 00000080: 6172 6368 2d6d 650d 0a64 6f77 6e6c 6f61  arch-me..downloa
 00000090: 645f 7572 6c20 3d20 6874 7470 733a 2f2f  d_url = https://
@@ -150,32 +150,41 @@
 00000950: 6e79 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  ny....[options].
 00000960: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
 00000970: 650d 0a69 6e73 7461 6c6c 5f72 6571 7569  e..install_requi
 00000980: 7265 7320 3d20 0d0a 0961 696f 6874 7470  res = ...aiohttp
 00000990: 3c34 2e30 2e30 0d0a 0970 616e 6461 733c  <4.0.0...pandas<
 000009a0: 3d32 2e30 2e32 0d0a 0963 7279 7074 6f67  =2.0.2...cryptog
 000009b0: 7261 7068 793c 3d34 312e 302e 310d 0a09  raphy<=41.0.1...
-000009c0: 6273 343c 3d30 2e30 2e31 0d0a 0969 6d70  bs4<=0.0.1...imp
-000009d0: 6f72 746c 6962 5f72 6573 6f75 7263 6573  ortlib_resources
-000009e0: 3b20 7079 7468 6f6e 5f76 6572 7369 6f6e  ; python_version
-000009f0: 203c 2022 332e 3922 0d0a 7079 7468 6f6e   < "3.9"..python
-00000a00: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000a10: 382c 203c 340d 0a69 6e63 6c75 6465 5f70  8, <4..include_p
-00000a20: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
-00000a30: 7565 0d0a 7061 636b 6167 6573 203d 2073  ue..packages = s
-00000a40: 6561 7263 685f 6d65 0d0a 0d0a 5b6f 7074  earch_me....[opt
-00000a50: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-00000a60: 615d 0d0a 7365 6172 6368 5f6d 6520 3d20  a]..search_me = 
-00000a70: 0d0a 092e 656e 6769 6e65 732f 2e64 6f6d  ....engines/.dom
-00000a80: 6169 6e73 0d0a 092e 656e 6769 6e65 732f  ains....engines/
-00000a90: 2e66 6f72 6d61 7473 0d0a 092e 656e 6769  .formats....engi
-00000aa0: 6e65 732f 2e6c 616e 6775 6167 6573 0d0a  nes/.languages..
-00000ab0: 092e 656e 6769 6e65 732f 2e70 6172 616d  ..engines/.param
-00000ac0: 730d 0a09 2e65 6e67 696e 6573 2f2e 7061  s....engines/.pa
-00000ad0: 7373 0d0a 092e 656e 6769 6e65 732f 2e72  ss....engines/.r
-00000ae0: 6567 6578 0d0a 092e 656e 6769 6e65 732f  egex....engines/
-00000af0: 2e73 616c 740d 0a0d 0a5b 6669 6c65 735d  .salt....[files]
-00000b00: 0d0a 7061 636b 6167 6573 203d 200d 0a09  ..packages = ...
-00000b10: 7365 7475 700d 0a09 7365 7475 702e 6366  setup...setup.cf
-00000b20: 670d 0a0d 0a5b 6567 675f 696e 666f 5d0d  g....[egg_info].
-00000b30: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000b40: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000009c0: 6273 343c 3d30 2e30 2e31 0d0a 096a 6d65  bs4<=0.0.1...jme
+000009d0: 7370 6174 683c 3d31 2e30 2e31 0d0a 0974  spath<=1.0.1...t
+000009e0: 6162 756c 6174 653c 3d30 2e39 2e30 0d0a  abulate<=0.9.0..
+000009f0: 0969 6d70 6f72 746c 6962 5f72 6573 6f75  .importlib_resou
+00000a00: 7263 6573 3b20 7079 7468 6f6e 5f76 6572  rces; python_ver
+00000a10: 7369 6f6e 203c 2022 332e 3922 0d0a 7079  sion < "3.9"..py
+00000a20: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000a30: 3e3d 332e 382c 203c 340d 0a69 6e63 6c75  >=3.8, <4..inclu
+00000a40: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+00000a50: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
+00000a60: 203d 2073 6561 7263 685f 6d65 0d0a 0d0a   = search_me....
+00000a70: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000a80: 5f64 6174 615d 0d0a 7365 6172 6368 5f6d  _data]..search_m
+00000a90: 6520 3d20 0d0a 092e 656e 6769 6e65 732f  e = ....engines/
+00000aa0: 2e64 6f6d 6169 6e73 0d0a 092e 656e 6769  .domains....engi
+00000ab0: 6e65 732f 2e66 6f72 6d61 7473 0d0a 092e  nes/.formats....
+00000ac0: 656e 6769 6e65 732f 2e6c 616e 6775 6167  engines/.languag
+00000ad0: 6573 0d0a 092e 656e 6769 6e65 732f 2e70  es....engines/.p
+00000ae0: 6172 616d 730d 0a09 2e65 6e67 696e 6573  arams....engines
+00000af0: 2f2e 7061 7373 0d0a 092e 656e 6769 6e65  /.pass....engine
+00000b00: 732f 2e72 6567 6578 0d0a 092e 656e 6769  s/.regex....engi
+00000b10: 6e65 732f 2e73 616c 740d 0a09 2e65 6e67  nes/.salt....eng
+00000b20: 696e 6573 2f2e 7573 6572 6167 656e 7473  ines/.useragents
+00000b30: 0d0a 092e 6f73 696e 742f 2e63 6f64 650d  ....osint/.code.
+00000b40: 0a09 2e6f 7369 6e74 2f2e 646f 726b 730d  ...osint/.dorks.
+00000b50: 0a09 2e6f 7369 6e74 2f2e 676f 760d 0a09  ...osint/.gov...
+00000b60: 2e6f 7369 6e74 2f2e 6d61 696e 0d0a 092e  .osint/.main....
+00000b70: 6f73 696e 742f 2e73 7761 700d 0a0d 0a5b  osint/.swap....[
+00000b80: 6669 6c65 735d 0d0a 7061 636b 6167 6573  files]..packages
+00000b90: 203d 200d 0a09 7365 7475 700d 0a09 7365   = ...setup...se
+00000ba0: 7475 702e 6366 670d 0a0d 0a5b 6567 675f  tup.cfg....[egg_
+00000bb0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000bc0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000bd0: 300d 0a0d 0a                             0....
```

