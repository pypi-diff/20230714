# Comparing `tmp/omdbapi-0.6.0.tar.gz` & `tmp/omdbapi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omdbapi-0.6.0.tar", last modified: Sun Jun 20 14:16:28 2021, max compression
+gzip compressed data, was "omdbapi-0.7.0.tar", last modified: Fri Jul 14 11:02:09 2023, max compression
```

## Comparing `omdbapi-0.6.0.tar` & `omdbapi-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 diego      (501) staff       (20)        0 2021-06-20 14:16:28.000000 omdbapi-0.6.0/
--rw-r--r--   0 diego      (501) staff       (20)    34520 2019-10-20 10:57:37.000000 omdbapi-0.6.0/LICENSE
--rw-r--r--   0 diego      (501) staff       (20)       33 2018-05-20 12:28:33.000000 omdbapi-0.6.0/MANIFEST.in
--rw-r--r--   0 diego      (501) staff       (20)     6662 2021-06-20 14:16:28.000000 omdbapi-0.6.0/PKG-INFO
--rw-r--r--   0 diego      (501) staff       (20)     5033 2021-06-20 13:39:06.000000 omdbapi-0.6.0/README.md
-drwxr-xr-x   0 diego      (501) staff       (20)        0 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi/
--rw-r--r--   0 diego      (501) staff       (20)       22 2021-06-20 14:15:56.000000 omdbapi-0.6.0/omdbapi/__init__.py
--rw-r--r--   0 diego      (501) staff       (20)     1189 2021-06-20 14:11:40.000000 omdbapi-0.6.0/omdbapi/movie_search.py
--rw-r--r--   0 diego      (501) staff       (20)     1395 2019-06-16 10:45:49.000000 omdbapi-0.6.0/omdbapi/movie_search_OLD.py
-drwxr-xr-x   0 diego      (501) staff       (20)        0 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi/tests/
--rw-r--r--   0 diego      (501) staff       (20)        0 2019-02-06 17:15:43.000000 omdbapi-0.6.0/omdbapi/tests/__init__.py
--rw-r--r--   0 diego      (501) staff       (20)     1710 2021-06-20 14:13:14.000000 omdbapi-0.6.0/omdbapi/tests/test_movie.py
-drwxr-xr-x   0 diego      (501) staff       (20)        0 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi.egg-info/
--rw-r--r--   0 diego      (501) staff       (20)     6662 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi.egg-info/PKG-INFO
--rw-r--r--   0 diego      (501) staff       (20)      348 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi.egg-info/SOURCES.txt
--rw-r--r--   0 diego      (501) staff       (20)        1 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi.egg-info/dependency_links.txt
--rw-r--r--   0 diego      (501) staff       (20)        1 2019-10-20 10:56:55.000000 omdbapi-0.6.0/omdbapi.egg-info/not-zip-safe
--rw-r--r--   0 diego      (501) staff       (20)        9 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi.egg-info/requires.txt
--rw-r--r--   0 diego      (501) staff       (20)        8 2021-06-20 14:16:28.000000 omdbapi-0.6.0/omdbapi.egg-info/top_level.txt
--rw-r--r--   0 diego      (501) staff       (20)       38 2021-06-20 14:16:28.000000 omdbapi-0.6.0/setup.cfg
--rw-r--r--   0 diego      (501) staff       (20)     5028 2021-06-20 14:14:40.000000 omdbapi-0.6.0/setup.py
+drwxr-xr-x   0 diego      (501) staff       (20)        0 2023-07-14 11:02:09.955247 omdbapi-0.7.0/
+-rw-r--r--   0 diego      (501) staff       (20)    34520 2023-07-14 07:50:05.000000 omdbapi-0.7.0/LICENSE
+-rw-r--r--   0 diego      (501) staff       (20)       33 2023-07-14 07:50:05.000000 omdbapi-0.7.0/MANIFEST.in
+-rw-r--r--   0 diego      (501) staff       (20)     5283 2023-07-14 11:02:09.954686 omdbapi-0.7.0/PKG-INFO
+-rw-r--r--   0 diego      (501) staff       (20)     4527 2023-07-14 10:33:35.000000 omdbapi-0.7.0/README.md
+drwxr-xr-x   0 diego      (501) staff       (20)        0 2023-07-14 11:02:09.948289 omdbapi-0.7.0/omdbapi/
+-rw-r--r--   0 diego      (501) staff       (20)       22 2023-07-14 10:55:22.000000 omdbapi-0.7.0/omdbapi/__init__.py
+-rw-r--r--   0 diego      (501) staff       (20)     1417 2023-07-14 10:55:22.000000 omdbapi-0.7.0/omdbapi/movie_search.py
+drwxr-xr-x   0 diego      (501) staff       (20)        0 2023-07-14 11:02:09.954004 omdbapi-0.7.0/omdbapi/tests/
+-rw-r--r--   0 diego      (501) staff       (20)        0 2023-07-14 07:50:05.000000 omdbapi-0.7.0/omdbapi/tests/__init__.py
+-rw-r--r--   0 diego      (501) staff       (20)     2147 2023-07-14 10:26:21.000000 omdbapi-0.7.0/omdbapi/tests/test_movie.py
+drwxr-xr-x   0 diego      (501) staff       (20)        0 2023-07-14 11:02:09.953122 omdbapi-0.7.0/omdbapi.egg-info/
+-rw-r--r--   0 diego      (501) staff       (20)     5283 2023-07-14 11:02:09.000000 omdbapi-0.7.0/omdbapi.egg-info/PKG-INFO
+-rw-r--r--   0 diego      (501) staff       (20)      320 2023-07-14 11:02:09.000000 omdbapi-0.7.0/omdbapi.egg-info/SOURCES.txt
+-rw-r--r--   0 diego      (501) staff       (20)        1 2023-07-14 11:02:09.000000 omdbapi-0.7.0/omdbapi.egg-info/dependency_links.txt
+-rw-r--r--   0 diego      (501) staff       (20)        1 2023-07-14 11:02:09.000000 omdbapi-0.7.0/omdbapi.egg-info/not-zip-safe
+-rw-r--r--   0 diego      (501) staff       (20)        9 2023-07-14 11:02:09.000000 omdbapi-0.7.0/omdbapi.egg-info/requires.txt
+-rw-r--r--   0 diego      (501) staff       (20)        8 2023-07-14 11:02:09.000000 omdbapi-0.7.0/omdbapi.egg-info/top_level.txt
+-rw-r--r--   0 diego      (501) staff       (20)       38 2023-07-14 11:02:09.955361 omdbapi-0.7.0/setup.cfg
+-rw-r--r--   0 diego      (501) staff       (20)     5028 2023-07-14 07:50:05.000000 omdbapi-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `omdbapi-0.6.0/LICENSE` & `omdbapi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omdbapi-0.6.0/README.md` & `omdbapi-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # omdbapi python library.
 [![Build Status](https://travis-ci.org/dubirajara/omdbapi.svg?branch=master)](https://travis-ci.org/dubirajara/omdbapi)
-[![Updates](https://pyup.io/repos/github/dubirajara/omdbapi/shield.svg)](https://pyup.io/repos/github/dubirajara/omdbapi/)
-[![Python 3](https://pyup.io/repos/github/dubirajara/omdbapi/python-3-shield.svg)](https://pyup.io/repos/github/dubirajara/omdbapi/)
 [![codecov](https://codecov.io/gh/dubirajara/omdbapi/branch/master/graph/badge.svg)](https://codecov.io/gh/dubirajara/omdbapi)
 
-Python lib to get movie, series, episode data from the Open Movie Database (OMDb) api.
+Python wrap to get movie, series, episode data from the Open Movie Database (OMDb) api.
 Example build and distribution python projects - [Pytools](http://www.python.pro.br) course.
 
 Used [The Open Movie Database](http://www.omdbapi.com) api to build a python lib and distribution in [pypi](https://pypi.org/project/omdbapi/).
 
 ## How to use? 
 
 **IMPORTANT**: Requires Python 3.7 or newer. To works with python 3.6 must install the versión 0.5.1.
 
-#### Before, you must be request free the omdbapi api key [here](http://www.omdbapi.com/apikey.aspx?__EVENTTARGET=freeAcct&__EVENTARGUMENT=&__LASTFOCUS=&__VIEWSTATE=%2FwEPDwUKLTIwNDY4MTIzNQ9kFgYCAQ9kFgICBw8WAh4HVmlzaWJsZWhkAgIPFgIfAGhkAgMPFgIfAGhkGAEFHl9fQ29udHJvbHNSZXF1aXJlUG9zdEJhY2tLZXlfXxYDBQtwYXRyZW9uQWNjdAUIZnJlZUFjY3QFCGZyZWVBY2N0x0euvR%2FzVv1jLU3mGetH4R3kWtYKWACCaYcfoP1IY8g%3D&__VIEWSTATEGENERATOR=5E550F58&__EVENTVALIDATION=%2FwEdAAU5GG7XylwYou%2BzznFv7FbZmSzhXfnlWWVdWIamVouVTzfZJuQDpLVS6HZFWq5fYpioiDjxFjSdCQfbG0SWduXFd8BcWGH1ot0k0SO7CfuulN6vYN8IikxxqwtGWTciOwQ4e4xie4N992dlfbpyqd1D&at=freeAcct&Email=)
+#### Before, you must be request free the omdbapi api key [here](http://www.omdbapi.com/apikey.aspx)
 
 Install the library, Python 3.7 or newer:
 ```python
 >>> pip install omdbapi
 ```
 To works with python 3.6 must install the versión 0.5.1
 ```python
@@ -56,16 +54,15 @@
  'imdbrating': '8.6',
  'imdbvotes': '1,569,520',
  'imdbid': 'tt0816692',
  'type': 'movie',
  'dvd': '24 May 2016',
  'boxoffice': '$188,020,017',
  'production': 'Lynda Obst Productions, Syncopy',
- 'website': 'N/A',
- 'response': 'True'}
+ 'website': 'N/A'}
 
 ```
 Or can set full plot as parameter:
 ```python
 >>> movie.get_movie(title='Interstellar', plot='full')
 {'title': 'Interstellar',
  'year': '2014',
@@ -88,18 +85,29 @@
  'imdbrating': '8.6',
  'imdbvotes': '1,569,520',
  'imdbid': 'tt0816692',
  'type': 'movie',
  'dvd': '24 May 2016',
  'boxoffice': '$188,020,017',
  'production': 'Lynda Obst Productions, Syncopy',
- 'website': 'N/A',
- 'response': 'True'}
+ 'website': 'N/A'}
 
 ```
+Get value using class attributes:
+```python
+>>> movie.director
+'Christopher Nolan'
+
+>>> movie.poster
+'https://m.media-amazon.com/images/M/MV5BZjdkOTU3MDktN2IxOS00OGEyLWFmMjktY2FiMmZkNWIyODZiXkEyXkFqcGdeQXVyMTMxODk2OTU@._V1_SX300.jpg'
+
+>>> movie.awards
+'Won 1 Oscar. Another 43 wins & 148 nominations.'
+```
+
 
 Get values using keys as parameter:
 ```python
 >>> movie.get_data('director', 'actors', 'awards', 'plot')
 
 {'director': 'Christopher Nolan',
  'actors': 'Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow',
```

### Comparing `omdbapi-0.6.0/omdbapi/tests/test_movie.py` & `omdbapi-0.7.0/omdbapi/tests/test_movie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,73 @@
 from unittest.mock import Mock
 
 import pytest
 
 from omdbapi import movie_search
+from omdbapi.movie_search import GetMovieException
 
 
 @pytest.fixture
 def get_movie(mocker):
     resp_mock = Mock()
     resp_mock.json.return_value = {
         'Title': 'Star Wars: Episode IV - A New Hope',
         'Year': '1977',
         'Genre': 'Action, Adventure, Fantasy',
         'Director': 'George Lucas',
         'Writer': 'George Lucas',
         'Actors': 'Mark Hamill, Harrison Ford, Carrie Fisher, Peter Cushing',
         'Awards': 'Won 6 Oscars. Another 50 wins & 28 nominations.',
         'Response': 'True'
-         }
+    }
     get_mock = mocker.patch('omdbapi.movie_search.requests.get')
     get_mock.return_value = resp_mock
     movie = movie_search.GetMovie(api_key='12345')
     return movie
 
 
 @pytest.mark.parametrize(
     'expected',
-    ('title', 'awards', 'year', 'genre', 'writer', 'response', 'actors', 'director')
+    ('title', 'awards', 'year', 'genre', 'writer', 'actors', 'director')
 )
 def test_get_all_data(expected, get_movie):
     movie = get_movie.get_movie(title='star wars')
     assert expected in movie
 
 
 def test_repr():
     movie = movie_search.GetMovie(api_key='12345')
-    assert repr(movie) == "GetMovie(api_key='12345', values=None)"
+    assert repr(movie) == "GetMovie(api_key='12345', values={})"
 
 
 @pytest.mark.parametrize(
     'expected',
     ('title', 'awards', 'year')
 )
 def test_get_data(expected, get_movie):
     get_movie.get_movie(title='star wars')
     data_movie = get_movie.get_data('Title', 'Awards', 'Year')
     assert expected in data_movie
 
 
+@pytest.mark.parametrize(
+    'field, value',
+    [('title', 'Star Wars: Episode IV - A New Hope'),
+     ('director', 'George Lucas'),
+     ('genre', 'Action, Adventure, Fantasy')]
+)
+def test_get_data_by_attributes(field, value, get_movie):
+    get_movie.get_movie(title='star wars')
+    assert getattr(get_movie, field) == value
+
+
 def test_data_key_not_found(get_movie):
     get_movie.get_movie(title='star wars')
     data_movie = get_movie.get_data('Plot')
     assert data_movie['plot'] == 'key not found!'
 
 
 def test_get_data_invalid():
-    movie = movie_search.GetMovie(api_key='1111')
-    assert movie.get_movie(title='star wars') == 'Invalid API key!'
+    with pytest.raises(GetMovieException) as e:
+        movie = movie_search.GetMovie(api_key='1111')
+        movie.get_movie(title='star wars')
+    assert str(e.value) == 'Invalid API key!'
```

### Comparing `omdbapi-0.6.0/setup.py` & `omdbapi-0.7.0/setup.py`

 * *Files identical despite different names*

