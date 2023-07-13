# Comparing `tmp/11x_wagtail_blog-0.1.0.tar.gz` & `tmp/11x_wagtail_blog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "11x_wagtail_blog-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "11x_wagtail_blog-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `11x_wagtail_blog-0.1.0.tar` & `11x_wagtail_blog-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0      242 2023-07-03 17:25:55.411469 11x_wagtail_blog-0.1.0/.gitignore
--rw-r--r--   0        0        0       22 2023-07-03 17:39:21.047490 11x_wagtail_blog-0.1.0/.python-version
--rw-r--r--   0        0        0     1087 2023-07-03 16:57:20.371425 11x_wagtail_blog-0.1.0/LICENSE
--rw-r--r--   0        0        0      186 2023-07-12 20:26:51.147945 11x_wagtail_blog-0.1.0/README.rst
--rw-r--r--   0        0        0      634 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     1788 2023-07-03 18:19:38.219552 11x_wagtail_blog-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      498 2023-07-03 18:22:21.651556 11x_wagtail_blog-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1608 2023-07-12 20:25:36.959943 11x_wagtail_blog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      697 2023-07-04 16:31:02.906578 11x_wagtail_blog-0.1.0/tox.ini
--rw-r--r--   0        0        0       38 2023-07-12 20:24:13.887941 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/__init__.py
--rw-r--r--   0        0        0      164 2023-07-03 18:43:43.887589 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/apps.py
--rw-r--r--   0        0        0     1153 2023-07-11 00:03:16.100737 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/fakers.py
--rw-r--r--   0        0        0     3962 2023-07-11 00:07:25.992743 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-10 22:20:08.564577 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/migrations/__init__.py
--rw-r--r--   0        0        0     3237 2023-07-12 15:33:06.386469 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/models.py
--rw-r--r--   0        0        0      229 2023-07-04 18:49:03.415909 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/about_the_author.html
--rw-r--r--   0        0        0      659 2023-07-04 17:26:31.071781 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/tests/testing_models/testing_article_page.html
--rw-r--r--   0        0        0        0 2023-07-04 17:12:17.795760 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templatetags/__init__.py
--rw-r--r--   0        0        0      612 2023-07-04 18:08:01.615846 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templatetags/x11x_wagtail_blog.py
--rw-r--r--   0        0        0        0 2023-07-10 23:48:47.780714 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/__init__.py
--rw-r--r--   0        0        0     5239 2023-07-12 15:37:19.206475 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/test_extensible_article_page.py
--rw-r--r--   0        0        0        0 2023-07-10 23:48:45.748714 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/__init__.py
--rw-r--r--   0        0        0      198 2023-07-10 23:53:51.440722 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/apps.py
--rw-r--r--   0        0        0      565 2023-07-10 23:50:54.984717 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/fakers.py
--rw-r--r--   0        0        0     1155 2023-07-10 23:54:08.428722 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-10 23:54:08.320722 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/migrations/__init__.py
--rw-r--r--   0        0        0      270 2023-07-11 00:01:20.236734 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/models.py
--rw-r--r--   0        0        0       63 2023-07-03 18:39:46.795583 11x_wagtail_blog-0.1.0/x11x_wagtail_blog/views.py
--rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 11x_wagtail_blog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-07-03 17:25:55.411469 11x_wagtail_blog-0.2.0/.gitignore
+-rw-r--r--   0        0        0       22 2023-07-03 17:39:21.047490 11x_wagtail_blog-0.2.0/.python-version
+-rw-r--r--   0        0        0      203 2023-07-13 23:26:11.752169 11x_wagtail_blog-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1087 2023-07-03 16:57:20.371425 11x_wagtail_blog-0.2.0/LICENSE
+-rw-r--r--   0        0        0      211 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/README.j2.rst
+-rw-r--r--   0        0        0     3081 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/README.rst
+-rw-r--r--   0        0        0      634 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     2111 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     1373 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-07-03 18:15:47.719546 11x_wagtail_blog-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0      528 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/docs/models.rst
+-rw-r--r--   0        0        0      158 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/docs/testing.rst
+-rw-r--r--   0        0        0     2165 2023-07-13 17:17:52.554462 11x_wagtail_blog-0.2.0/docs/update_readme.py
+-rw-r--r--   0        0        0     1608 2023-07-12 20:25:36.959943 11x_wagtail_blog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-07-04 16:31:02.906578 11x_wagtail_blog-0.2.0/tox.ini
+-rw-r--r--   0        0        0     2335 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-03 18:43:43.887589 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/apps.py
+-rw-r--r--   0        0        0     3033 2023-07-13 23:24:21.840166 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/fakers.py
+-rw-r--r--   0        0        0     3962 2023-07-11 00:07:25.992743 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:20:08.564577 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/migrations/__init__.py
+-rw-r--r--   0        0        0     5440 2023-07-13 23:24:21.844166 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/models.py
+-rw-r--r--   0        0        0      229 2023-07-04 18:49:03.415909 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/about_the_author.html
+-rw-r--r--   0        0        0      659 2023-07-04 17:26:31.071781 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/tests/testing_models/testing_article_page.html
+-rw-r--r--   0        0        0        0 2023-07-04 17:12:17.795760 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/templatetags/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-13 23:24:21.844166 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/templatetags/x11x_wagtail_blog.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:48:47.780714 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-13 23:24:21.844166 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/test_docs.py
+-rw-r--r--   0        0        0     5239 2023-07-12 15:37:19.206475 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/test_extensible_article_page.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:48:45.748714 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-10 23:53:51.440722 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/apps.py
+-rw-r--r--   0        0        0      565 2023-07-10 23:50:54.984717 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/fakers.py
+-rw-r--r--   0        0        0     1155 2023-07-10 23:54:08.428722 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:54:08.320722 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/migrations/__init__.py
+-rw-r--r--   0        0        0      270 2023-07-11 00:01:20.236734 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/models.py
+-rw-r--r--   0        0        0       63 2023-07-03 18:39:46.795583 11x_wagtail_blog-0.2.0/x11x_wagtail_blog/views.py
+-rw-r--r--   0        0        0     4540 1970-01-01 00:00:00.000000 11x_wagtail_blog-0.2.0/PKG-INFO
```

### Comparing `11x_wagtail_blog-0.1.0/LICENSE` & `11x_wagtail_blog-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/docs/Makefile` & `11x_wagtail_blog-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/docs/make.bat` & `11x_wagtail_blog-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/pyproject.toml` & `11x_wagtail_blog-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/tox.ini` & `11x_wagtail_blog-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/x11x_wagtail_blog/migrations/0001_initial.py` & `11x_wagtail_blog-0.2.0/x11x_wagtail_blog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/tests/testing_models/testing_article_page.html` & `11x_wagtail_blog-0.2.0/x11x_wagtail_blog/templates/x11x_wagtail_blog/tests/testing_models/testing_article_page.html`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/test_extensible_article_page.py` & `11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/test_extensible_article_page.py`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/fakers.py` & `11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/fakers.py`

 * *Files identical despite different names*

### Comparing `11x_wagtail_blog-0.1.0/x11x_wagtail_blog/tests/testing_models/migrations/0001_initial.py` & `11x_wagtail_blog-0.2.0/x11x_wagtail_blog/tests/testing_models/migrations/0001_initial.py`

 * *Files identical despite different names*

