# Comparing `tmp/tidytweets-0.1.tar.gz` & `tmp/tidytweets-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tidytweets-0.1.tar", last modified: Thu Jun 29 13:59:13 2023, max compression
+gzip compressed data, was "dist\tidytweets-0.15.tar", last modified: Fri Jul 14 00:08:38 2023, max compression
```

## Comparing `tidytweets-0.1.tar` & `tidytweets-0.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:59:13.789218 tidytweets-0.1/
--rw-rw-rw-   0        0        0     1094 2023-06-29 13:28:11.000000 tidytweets-0.1/LICENSE.rst
--rw-rw-rw-   0        0        0      630 2023-06-29 13:59:13.789714 tidytweets-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      146 2023-06-29 13:28:11.000000 tidytweets-0.1/README.md
--rw-rw-rw-   0        0        0      115 2023-06-29 13:59:13.790706 tidytweets-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1261 2023-06-29 13:54:34.000000 tidytweets-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:59:13.772849 tidytweets-0.1/tests/
--rw-rw-rw-   0        0        0      161 2023-06-29 13:28:11.000000 tidytweets-0.1/tests/test_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:59:13.765409 tidytweets-0.1/tidytweets/
-drwxrwxrwx   0        0        0        0 2023-06-29 13:59:13.788722 tidytweets-0.1/tidytweets/tidytweets.egg-info/
--rw-rw-rw-   0        0        0      630 2023-06-29 13:59:13.000000 tidytweets-0.1/tidytweets/tidytweets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-06-29 13:59:13.000000 tidytweets-0.1/tidytweets/tidytweets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:59:13.000000 tidytweets-0.1/tidytweets/tidytweets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-06-29 13:59:13.000000 tidytweets-0.1/tidytweets/tidytweets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:59:13.000000 tidytweets-0.1/tidytweets/tidytweets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 00:08:38.931465 tidytweets-0.15/
+-rw-rw-rw-   0        0        0     1094 2023-06-29 13:28:11.000000 tidytweets-0.15/LICENSE.rst
+-rw-rw-rw-   0        0        0      631 2023-07-14 00:08:38.931465 tidytweets-0.15/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2023-06-29 13:28:11.000000 tidytweets-0.15/README.md
+-rw-rw-rw-   0        0        0      115 2023-07-14 00:08:38.934937 tidytweets-0.15/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2023-07-14 00:06:36.000000 tidytweets-0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:08:38.918571 tidytweets-0.15/tests/
+-rw-rw-rw-   0        0        0      161 2023-06-29 13:28:11.000000 tidytweets-0.15/tests/test_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:08:38.915097 tidytweets-0.15/tidytweets/
+drwxrwxrwx   0        0        0        0 2023-07-14 00:08:38.930472 tidytweets-0.15/tidytweets/tidytweets.egg-info/
+-rw-rw-rw-   0        0        0      631 2023-07-14 00:08:38.000000 tidytweets-0.15/tidytweets/tidytweets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-07-14 00:08:38.000000 tidytweets-0.15/tidytweets/tidytweets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:08:38.000000 tidytweets-0.15/tidytweets/tidytweets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-07-14 00:08:38.000000 tidytweets-0.15/tidytweets/tidytweets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:08:38.000000 tidytweets-0.15/tidytweets/tidytweets.egg-info/top_level.txt
```

### Comparing `tidytweets-0.1/LICENSE.rst` & `tidytweets-0.15/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `tidytweets-0.1/PKG-INFO` & `tidytweets-0.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytweets
-Version: 0.1
+Version: 0.15
 Summary: Clean tweets to perform various NLP tasks such as topic analysis, word embeddings, sentiment analysis, etc.
 Home-page: https://github.com/lgomezt/Tidytweets
 Author: Lucas Gómez Tobón, Jose Fernando Barrera
 Author-email: lucasgomeztobon@hotmail.com, jf.barrera10@uniandes.edu.co
 License: MIT
 Keywords: NLP Text processing Twitter API processing data cleaning
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidytweets-0.1/setup.py` & `tidytweets-0.15/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name = 'tidytweets',
     packages = find_packages('tidytweets',include = ['tidytweets']),
-    version = '0.1',
+    version = '0.15',
     description = 'Clean tweets to perform various NLP tasks such as topic analysis, word embeddings, sentiment analysis, etc.',
     author = 'Lucas Gómez Tobón, Jose Fernando Barrera',
     author_email  = "lucasgomeztobon@hotmail.com, jf.barrera10@uniandes.edu.co",
     license = 'MIT',
     package_dir={'': 'tidytweets'},
     url='https://github.com/lgomezt/Tidytweets',
     keywords='NLP Text processing Twitter API processing data cleaning',
@@ -18,13 +18,13 @@
     ],
     python_requires = ">=3.6",
     setup_requires = ['pytest-runner'],
     tests_require = ['pytest'],
     install_requires = [
         'pandas','numpy','nltk','spacy','gensim','textblob','tweepy',
         'emoji','unidecode','scikit-learn','matplotlib','seaborn','wordcloud',
-        'plotly','pyLDAvis','thefuzz'
+        'plotly','pyLDAvis','thefuzz','tqdm','spacy_spanish_lemmatizer'
     ],
     # Running `python setup.py pytest`
     # will execute all tests stored in the "tests" folder.
     test_suite = 'tests',
 )
```

### Comparing `tidytweets-0.1/tidytweets/tidytweets.egg-info/PKG-INFO` & `tidytweets-0.15/tidytweets/tidytweets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytweets
-Version: 0.1
+Version: 0.15
 Summary: Clean tweets to perform various NLP tasks such as topic analysis, word embeddings, sentiment analysis, etc.
 Home-page: https://github.com/lgomezt/Tidytweets
 Author: Lucas Gómez Tobón, Jose Fernando Barrera
 Author-email: lucasgomeztobon@hotmail.com, jf.barrera10@uniandes.edu.co
 License: MIT
 Keywords: NLP Text processing Twitter API processing data cleaning
 Classifier: Programming Language :: Python :: 3
```

