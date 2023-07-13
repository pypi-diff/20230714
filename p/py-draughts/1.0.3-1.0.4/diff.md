# Comparing `tmp/py-draughts-1.0.3.tar.gz` & `tmp/py-draughts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.0.3.tar", last modified: Thu Jul 13 19:34:38 2023, max compression
+gzip compressed data, was "py-draughts-1.0.4.tar", last modified: Thu Jul 13 22:44:46 2023, max compression
```

## Comparing `py-draughts-1.0.3.tar` & `py-draughts-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.927326 py-draughts-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6266 2023-07-13 19:34:38.926325 py-draughts-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4848 2023-07-13 18:25:28.000000 py-draughts-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.890324 py-draughts-1.0.3/draughts/
--rw-rw-rw-   0        0        0      964 2023-07-13 19:34:17.000000 py-draughts-1.0.3/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-13 18:02:36.000000 py-draughts-1.0.3/draughts/american.py
--rw-rw-rw-   0        0        0    11486 2023-07-13 19:30:01.000000 py-draughts-1.0.3/draughts/base.py
--rw-rw-rw-   0        0        0      671 2023-07-13 17:34:05.000000 py-draughts-1.0.3/draughts/models.py
--rw-rw-rw-   0        0        0     4197 2023-07-13 18:10:29.000000 py-draughts-1.0.3/draughts/move.py
--rw-rw-rw-   0        0        0     5323 2023-07-13 19:34:18.000000 py-draughts-1.0.3/draughts/server.py
--rw-rw-rw-   0        0        0     5989 2023-07-13 18:10:31.000000 py-draughts-1.0.3/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.837328 py-draughts-1.0.3/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.893324 py-draughts-1.0.3/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.0.3/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.896323 py-draughts-1.0.3/draughts/static/js/
--rw-rw-rw-   0        0        0     5993 2023-07-13 18:16:53.000000 py-draughts-1.0.3/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.904328 py-draughts-1.0.3/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.0.3/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2860 2023-07-13 18:13:53.000000 py-draughts-1.0.3/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-1.0.3/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.918327 py-draughts-1.0.3/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     6266 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 19:34:38.000000 py-draughts-1.0.3/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 19:34:38.928325 py-draughts-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:34:38.925324 py-draughts-1.0.3/test/
--rw-rw-rw-   0        0        0     1123 2023-07-13 17:33:45.000000 py-draughts-1.0.3/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.0.3/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.404502 py-draughts-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-07-13 22:43:03.000000 py-draughts-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-13 22:43:03.000000 py-draughts-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6258 2023-07-13 22:44:46.396414 py-draughts-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4841 2023-07-13 22:43:03.000000 py-draughts-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.103001 py-draughts-1.0.4/draughts/
+-rw-rw-rw-   0        0        0      964 2023-07-13 22:43:20.000000 py-draughts-1.0.4/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/american.py
+-rw-rw-rw-   0        0        0    11486 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/base.py
+-rw-rw-rw-   0        0        0      671 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/models.py
+-rw-rw-rw-   0        0        0     4197 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/move.py
+-rw-rw-rw-   0        0        0     5323 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/server.py
+-rw-rw-rw-   0        0        0     5989 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:45.790761 py-draughts-1.0.4/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.135020 py-draughts-1.0.4/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.196396 py-draughts-1.0.4/draughts/static/js/
+-rw-rw-rw-   0        0        0     5993 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.278271 py-draughts-1.0.4/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2860 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-13 22:43:03.000000 py-draughts-1.0.4/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.330852 py-draughts-1.0.4/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     6258 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 22:44:45.000000 py-draughts-1.0.4/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 22:43:03.000000 py-draughts-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 22:44:46.404502 py-draughts-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1905 2023-07-13 22:43:10.000000 py-draughts-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:44:46.388892 py-draughts-1.0.4/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-13 22:43:03.000000 py-draughts-1.0.4/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-13 22:43:03.000000 py-draughts-1.0.4/test/test_board.py
```

### Comparing `py-draughts-1.0.3/LICENSE` & `py-draughts-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/PKG-INFO` & `py-draughts-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.3
+Version: 1.0.4
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -19,22 +19,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
 ## Installation
 
@@ -160,25 +161,23 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e1caeb3f-2744-4198-a426-76ad184a448a" width="800" />
-
 <img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
 
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e6ae7861-624d-497a-b617-e499d817f6a3" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4deead2a-adf1-4a7a-9422-c8da43f31a53" width="800" />
 
 
 ### testing best moves finding methods:
 
-[Example](examples/engine.py)
+[Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
 
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
```

### Comparing `py-draughts-1.0.3/README.md` & `py-draughts-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
 ## Installation
 
@@ -131,25 +132,23 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e1caeb3f-2744-4198-a426-76ad184a448a" width="800" />
-
 <img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
 
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e6ae7861-624d-497a-b617-e499d817f6a3" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4deead2a-adf1-4a7a-9422-c8da43f31a53" width="800" />
 
 
 ### testing best moves finding methods:
 
-[Example](examples/engine.py)
+[Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
 
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
```

### Comparing `py-draughts-1.0.3/draughts/__init__.py` & `py-draughts-1.0.4/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-1.0.3/draughts/american.py` & `py-draughts-1.0.4/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/base.py` & `py-draughts-1.0.4/draughts/base.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/models.py` & `py-draughts-1.0.4/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/move.py` & `py-draughts-1.0.4/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/server.py` & `py-draughts-1.0.4/draughts/server.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/standard.py` & `py-draughts-1.0.4/draughts/standard.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/static/css/style.css` & `py-draughts-1.0.4/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/static/js/script.js` & `py-draughts-1.0.4/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/templates/base.html` & `py-draughts-1.0.4/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/templates/index.html` & `py-draughts-1.0.4/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/draughts/utils.py` & `py-draughts-1.0.4/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.0.4/py_draughts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.0.3
+Version: 1.0.4
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -19,22 +19,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-draughts
 
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/py-draughts)
 
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
 ## Installation
 
@@ -160,25 +161,23 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e1caeb3f-2744-4198-a426-76ad184a448a" width="800" />
-
 <img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b5b3c1fe-3e08-4114-b73b-2b136e3c1c9b" width="800" />
 
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/e6ae7861-624d-497a-b617-e499d817f6a3" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/4deead2a-adf1-4a7a-9422-c8da43f31a53" width="800" />
 
 
 ### testing best moves finding methods:
 
-[Example](examples/engine.py)
+[Example](https://github.com/michalskibinski109/py-draughts/blob/main/examples/engine.py)
 
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
```

### Comparing `py-draughts-1.0.3/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.0.4/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/setup.py` & `py-draughts-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,9 +42,9 @@
         "Topic :: Games/Entertainment :: Turn Based Strategy",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Typing :: Typed",
     ],
     project_urls={
         "Documentation": "https://michalskibinski109.github.io/draughts/index.html",
     },
-    python_requires=">=3.10",
+    python_requires=">=3.8",
 )
```

### Comparing `py-draughts-1.0.3/test/test_american_board.py` & `py-draughts-1.0.4/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.0.3/test/test_board.py` & `py-draughts-1.0.4/test/test_board.py`

 * *Files identical despite different names*

