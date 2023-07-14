# Comparing `tmp/blendedUx_Lang-1.0.0.tar.gz` & `tmp/blendedUx_Lang-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendedUx_Lang-1.0.0.tar", last modified: Thu Aug 25 05:57:07 2022, max compression
+gzip compressed data, was "blendedUx_Lang-1.1.0.tar", last modified: Fri Jul 14 05:41:50 2023, max compression
```

## Comparing `blendedUx_Lang-1.0.0.tar` & `blendedUx_Lang-1.1.0.tar`

### file list

```diff
@@ -1,66 +1,297 @@
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.824255 blendedUx_Lang-1.0.0/
--rw-rw-rw-   0        0        0     1107 2022-08-25 05:19:40.000000 blendedUx_Lang-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       29 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      193 2022-08-25 05:57:07.823257 blendedUx_Lang-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7318 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.730255 blendedUx_Lang-1.0.0/blendedUxLang/
--rw-rw-rw-   0        0        0      207 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.747938 blendedUx_Lang-1.0.0/blendedUxLang/blended/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/__init__.py
--rw-rw-rw-   0        0        0     3220 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/_compat.py
--rw-rw-rw-   0        0        0     4266 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/colormap.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.758380 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/__init__.py
--rw-rw-rw-   0        0        0       66 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/admin.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.760425 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/models.py
--rw-rw-rw-   0        0        0       63 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/tests.py
--rw-rw-rw-   0        0        0      232 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/urls.py
--rw-rw-rw-   0        0        0      776 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/views.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.767363 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/__init__.py
--rw-rw-rw-   0        0        0      372 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/jinjaenv.py
--rw-rw-rw-   0        0        0     9282 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/loader.py
--rw-rw-rw-   0        0        0     3116 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/models.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.771353 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/templatetags/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/templatetags/__init__.py
--rw-rw-rw-   0        0        0    25126 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/templatetags/blended_tags.py
--rw-rw-rw-   0        0        0    65214 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/tests.py
--rw-rw-rw-   0        0        0     1664 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/flask.py
--rw-rw-rw-   0        0        0     8383 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/functions.py
--rw-rw-rw-   0        0        0    28299 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/jinjaenv.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.778907 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.780902 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/__init__.py
--rw-rw-rw-   0        0        0     9720 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/blendedParserListener.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.788326 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py2/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py2/__init__.py
--rw-rw-rw-   0        0        0    38068 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py2/blendedLexer.py
--rw-rw-rw-   0        0        0   140728 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py2/blendedParser.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.792432 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py3/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py3/__init__.py
--rw-rw-rw-   0        0        0    37011 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py3/blendedLexer.py
--rw-rw-rw-   0        0        0   141316 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py3/blendedParser.py
--rw-rw-rw-   0        0        0     1065 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/lint.py
--rw-rw-rw-   0        0        0     1252 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/lintcommands.py
--rw-rw-rw-   0        0        0      405 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/listeners.py
--rw-rw-rw-   0        0        0     6165 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/sets.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.794466 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/
--rw-rw-rw-   0        0        0      260 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.803892 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0     3067 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      778 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/wsgi.py
--rw-rw-rw-   0        0        0    10880 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/blended/trimfloat.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.804892 blendedUx_Lang-1.0.0/blendedUxLang/tests/
--rw-rw-rw-   0        0        0      482 2022-08-25 05:16:00.000000 blendedUx_Lang-1.0.0/blendedUxLang/tests/parse_release_tags.py
-drwxrwxrwx   0        0        0        0 2022-08-25 05:57:07.822256 blendedUx_Lang-1.0.0/blendedUx_Lang.egg-info/
--rw-rw-rw-   0        0        0      193 2022-08-25 05:57:07.000000 blendedUx_Lang-1.0.0/blendedUx_Lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2057 2022-08-25 05:57:07.000000 blendedUx_Lang-1.0.0/blendedUx_Lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-25 05:57:07.000000 blendedUx_Lang-1.0.0/blendedUx_Lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-08-25 05:57:07.000000 blendedUx_Lang-1.0.0/blendedUx_Lang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-25 05:57:07.824255 blendedUx_Lang-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      261 2022-08-25 05:56:55.000000 blendedUx_Lang-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.297248 blendedUx_Lang-1.1.0/
+-rw-rw-rw-   0        0        0     1096 2023-03-02 07:43:08.000000 blendedUx_Lang-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       29 2023-03-02 07:43:08.000000 blendedUx_Lang-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-07-14 05:41:50.296253 blendedUx_Lang-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-13 13:41:32.000000 blendedUx_Lang-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.010924 blendedUx_Lang-1.1.0/blended/
+-rw-rw-rw-   0        0        0      161 2023-05-18 08:19:03.000000 blendedUx_Lang-1.1.0/blended/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.149248 blendedUx_Lang-1.1.0/blended/__pycache__/
+-rw-rw-rw-   0        0        0      476 2023-05-18 08:27:52.000000 blendedUx_Lang-1.1.0/blended/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      179 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1953 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/_compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1389 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/_compat.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6085 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/colormap.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3630 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/colormap.cpython-38.pyc
+-rw-rw-rw-   0        0        0    13894 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/functions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7972 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/functions.cpython-38.pyc
+-rw-rw-rw-   0        0        0    40556 2023-05-16 15:32:27.000000 blendedUx_Lang-1.1.0/blended/__pycache__/jinjaenv.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23364 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/jinjaenv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9976 2023-05-16 07:18:27.000000 blendedUx_Lang-1.1.0/blended/__pycache__/sets.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6132 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/sets.cpython-38.pyc
+-rw-rw-rw-   0        0        0    16848 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/trimfloat.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10880 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/trimfloat.cpython-38.pyc
+-rw-rw-rw-   0        0        0      849 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/_compat.py
+-rw-rw-rw-   0        0        0     4266 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/colormap.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.261474 blendedUx_Lang-1.1.0/blended/customtags/
+-rw-rw-rw-   0        0        0       79 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/customtags/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.518950 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/
+-rw-rw-rw-   0        0        0      329 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      289 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7101 2023-05-16 07:23:17.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4683 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_compat.cpython-38.pyc
+-rw-rw-rw-   0        0        0   210048 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_stringdefs.cpython-311.pyc
+-rw-rw-rw-   0        0        0   208260 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_stringdefs.cpython-38.pyc
+-rw-rw-rw-   0        0        0    49725 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/arguments.cpython-311.pyc
+-rw-rw-rw-   0        0        0    26381 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/arguments.cpython-38.pyc
+-rw-rw-rw-   0        0        0    14212 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/core.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7699 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/core.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5726 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/decorators.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3317 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/decorators.cpython-38.pyc
+-rw-rw-rw-   0        0        0     8652 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/exceptions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6336 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/exceptions.cpython-38.pyc
+-rw-rw-rw-   0        0        0    28436 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/expr_parser.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13562 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/expr_parser.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4256 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/helpers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2842 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/helpers.cpython-38.pyc
+-rw-rw-rw-   0        0        0    19689 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/lexer.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12473 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/lexer.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3181 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/middleware.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2053 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/middleware.cpython-38.pyc
+-rw-rw-rw-   0        0        0    37791 2023-05-16 07:26:21.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/nodes.cpython-311.pyc
+-rw-rw-rw-   0        0        0    22471 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/nodes.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6137 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/parser.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3264 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/parser.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7454 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/tokens.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4334 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/tokens.cpython-38.pyc
+-rw-rw-rw-   0        0        0    16901 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/trimfloat.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10891 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/trimfloat.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7096 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4613 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/utils.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7580 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/values.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5145 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/values.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4200 2023-05-16 07:23:12.000000 blendedUx_Lang-1.1.0/blended/customtags/_compat.py
+-rw-rw-rw-   0        0        0   404439 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/_stringdefs.py
+-rw-rw-rw-   0        0        0    33426 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/arguments.py
+-rw-rw-rw-   0        0        0     8682 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/core.py
+-rw-rw-rw-   0        0        0     4103 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/decorators.py
+-rw-rw-rw-   0        0        0     4939 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/exceptions.py
+-rw-rw-rw-   0        0        0    19676 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/expr_parser.py
+-rw-rw-rw-   0        0        0     2779 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/helpers.py
+-rw-rw-rw-   0        0        0    17134 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/lexer.py
+-rw-rw-rw-   0        0        0     2006 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/middleware.py
+-rw-rw-rw-   0        0        0    23316 2023-05-16 07:26:18.000000 blendedUx_Lang-1.1.0/blended/customtags/nodes.py
+-rw-rw-rw-   0        0        0     6091 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.543008 blendedUx_Lang-1.1.0/blended/customtags/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.559003 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      203 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      338 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/customtags.cpython-311.pyc
+-rw-rw-rw-   0        0        0      273 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/customtags.cpython-38.pyc
+-rw-rw-rw-   0        0        0       60 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/customtags.py
+-rw-rw-rw-   0        0        0     5689 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/tokens.py
+-rw-rw-rw-   0        0        0    10894 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/trimfloat.py
+-rw-rw-rw-   0        0        0     6021 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/utils.py
+-rw-rw-rw-   0        0        0     3986 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/values.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.573012 blendedUx_Lang-1.1.0/blended/djangolint/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.686154 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/
+-rw-rw-rw-   0        0        0      207 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      190 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      262 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/admin.cpython-311.pyc
+-rw-rw-rw-   0        0        0      231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/admin.cpython-38.pyc
+-rw-rw-rw-   0        0        0      259 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0      228 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/models.cpython-38.pyc
+-rw-rw-rw-   0        0        0      262 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/tests.cpython-311.pyc
+-rw-rw-rw-   0        0        0      231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/tests.cpython-38.pyc
+-rw-rw-rw-   0        0        0      537 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/urls.cpython-311.pyc
+-rw-rw-rw-   0        0        0      403 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/urls.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1405 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/views.cpython-311.pyc
+-rw-rw-rw-   0        0        0      909 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/views.cpython-38.pyc
+-rw-rw-rw-   0        0        0       66 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/admin.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.693132 blendedUx_Lang-1.1.0/blended/djangolint/migrations/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.699149 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      201 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0       60 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/models.py
+-rw-rw-rw-   0        0        0       63 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/tests.py
+-rw-rw-rw-   0        0        0      218 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/urls.py
+-rw-rw-rw-   0        0        0      762 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/views.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.713920 blendedUx_Lang-1.1.0/blended/djangotags/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.782221 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/
+-rw-rw-rw-   0        0        0      207 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      190 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      802 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/jinjaenv.cpython-311.pyc
+-rw-rw-rw-   0        0        0      576 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/jinjaenv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9257 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/loader.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4723 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/loader.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3985 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2991 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/models.cpython-38.pyc
+-rw-rw-rw-   0        0        0    77112 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/tests.cpython-311.pyc
+-rw-rw-rw-   0        0        0    42295 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/tests.cpython-38.pyc
+-rw-rw-rw-   0        0        0      345 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/jinjaenv.py
+-rw-rw-rw-   0        0        0    13279 2023-07-06 12:10:11.000000 blendedUx_Lang-1.1.0/blended/djangotags/loader.py
+-rw-rw-rw-   0        0        0     3349 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/models.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.811106 blendedUx_Lang-1.1.0/blended/djangotags/templates/
+-rw-rw-rw-   0        0        0     1127 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/colormacros.html
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.828106 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/
+-rw-rw-rw-   0        0        0       94 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/echotag.html
+-rw-rw-rw-   0        0        0       51 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/multilinecomment.html
+-rw-rw-rw-   0        0        0       76 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/multilinetag.html
+-rw-rw-rw-   0        0        0       15 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/multilinevariable.html
+-rw-rw-rw-   0        0        0       71 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/newline.html
+-rw-rw-rw-   0        0        0       48 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/whitespace.html
+-rw-rw-rw-   0        0        0      125 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/whitespace2.html
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.832115 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.850174 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      203 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    36018 2023-05-16 07:29:05.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17805 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-38.pyc
+-rw-rw-rw-   0        0        0    30325 2023-07-06 12:09:17.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/blended_tags.py
+-rw-rw-rw-   0        0        0    53307 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/tests.py
+-rw-rw-rw-   0        0        0     8530 2023-06-20 10:46:57.000000 blendedUx_Lang-1.1.0/blended/functions.py
+-rw-rw-rw-   0        0        0    31394 2023-05-16 08:25:59.000000 blendedUx_Lang-1.1.0/blended/jinjaenv.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.860134 blendedUx_Lang-1.1.0/blended/lint/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.892680 blendedUx_Lang-1.1.0/blended/lint/__pycache__/
+-rw-rw-rw-   0        0        0      201 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      184 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1662 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lint.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1065 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lint.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2418 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lintcommands.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1239 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lintcommands.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1335 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/listeners.cpython-311.pyc
+-rw-rw-rw-   0        0        0      893 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/listeners.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.905699 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.917981 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/
+-rw-rw-rw-   0        0        0      217 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      200 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    13027 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12185 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6261 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedLexer.g4
+-rw-rw-rw-   0        0        0     4992 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParser.g4
+-rw-rw-rw-   0        0        0     9720 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParserListener.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.929973 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.954983 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/
+-rw-rw-rw-   0        0        0      221 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      204 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    43111 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-311.pyc
+-rw-rw-rw-   0        0        0    22293 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-38.pyc
+-rw-rw-rw-   0        0        0   225659 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-311.pyc
+-rw-rw-rw-   0        0        0   118406 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-38.pyc
+-rw-rw-rw-   0        0        0    38068 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.tokens
+-rw-rw-rw-   0        0        0   140728 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.tokens
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.001682 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.030030 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/
+-rw-rw-rw-   0        0        0      221 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      204 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    42275 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-311.pyc
+-rw-rw-rw-   0        0        0    22035 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-38.pyc
+-rw-rw-rw-   0        0        0   227751 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-311.pyc
+-rw-rw-rw-   0        0        0   119493 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-38.pyc
+-rw-rw-rw-   0        0        0    37011 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.tokens
+-rw-rw-rw-   0        0        0   141316 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.tokens
+-rw-rw-rw-   0        0        0      995 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/lint.py
+-rw-rw-rw-   0        0        0     1238 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/lintcommands.py
+-rw-rw-rw-   0        0        0      405 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/listeners.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:48.929501 blendedUx_Lang-1.1.0/blended/lint/test_files/
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.087018 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/
+-rw-rw-rw-   0        0        0       16 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error.html
+-rw-rw-rw-   0        0        0      213 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_01_0_for_scope.html
+-rw-rw-rw-   0        0        0      114 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_01_1_for_scope.html
+-rw-rw-rw-   0        0        0      180 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_02_0_macro_scope.html
+-rw-rw-rw-   0        0        0      224 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_02_1_macro_scope.html
+-rw-rw-rw-   0        0        0      179 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_02_2_macro_scope.html
+-rw-rw-rw-   0        0        0      105 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_03_0_set_block.html
+-rw-rw-rw-   0        0        0      187 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_04_0_for_dict.html
+-rw-rw-rw-   0        0        0      108 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_05_0_tilde_expression.html
+-rw-rw-rw-   0        0        0       69 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_06_0_for_conditional.html
+-rw-rw-rw-   0        0        0      196 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_07_0_string_iter.html
+-rw-rw-rw-   0        0        0      158 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_09_0_extends_macro.html
+-rw-rw-rw-   0        0        0       40 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_10_0_filters_first.html
+-rw-rw-rw-   0        0        0      160 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_10_1_filters_scope.html
+-rw-rw-rw-   0        0        0       65 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_0_filter.html
+-rw-rw-rw-   0        0        0      122 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_1_filter_echo.html
+-rw-rw-rw-   0        0        0      158 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_2_filter_for.html
+-rw-rw-rw-   0        0        0      115 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_3_filter_sort.html
+-rw-rw-rw-   0        0        0      353 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_4_filter_macro.html
+-rw-rw-rw-   0        0        0       81 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_08_7_include_macro.html
+-rw-rw-rw-   0        0        0       62 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_08_8_macro_include.html
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.093008 blendedUx_Lang-1.1.0/blended/lint/test_files/expr_tests/
+-rw-rw-rw-   0        0        0       16 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/expr_tests/error.html
+-rw-rw-rw-   0        0        0      286 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/expr_tests/success.html
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.240654 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/
+-rw-rw-rw-   0        0        0       70 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/modeTest.html
+-rw-rw-rw-   0        0        0       93 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_0_extends_file.html
+-rw-rw-rw-   0        0        0       86 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_1_extends_object.html
+-rw-rw-rw-   0        0        0      101 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_2_extends_parent.html
+-rw-rw-rw-   0        0        0       91 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_3_extends_inner_block.html
+-rw-rw-rw-   0        0        0      104 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_4_extends_multiple.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_5_block_scoping.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_5_extends_macro.html
+-rw-rw-rw-   0        0        0      353 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_0_for_basic.html
+-rw-rw-rw-   0        0        0       68 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_1_for_expression.html
+-rw-rw-rw-   0        0        0      482 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_2_for_variables.html
+-rw-rw-rw-   0        0        0       93 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_4_for_else.html
+-rw-rw-rw-   0        0        0      199 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_6_for_macro.html
+-rw-rw-rw-   0        0        0       96 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_7_for_set.html
+-rw-rw-rw-   0        0        0      119 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_8_for_dict.html
+-rw-rw-rw-   0        0        0      140 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_0_if_basic.html
+-rw-rw-rw-   0        0        0      676 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_1_if_expressions.html
+-rw-rw-rw-   0        0        0       92 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_3_if_scope.html
+-rw-rw-rw-   0        0        0      127 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_05_0_set_basic.html
+-rw-rw-rw-   0        0        0      137 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_05_1_set_expression.html
+-rw-rw-rw-   0        0        0      121 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_05_3_set_macro.html
+-rw-rw-rw-   0        0        0       52 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_0_do_basic.html
+-rw-rw-rw-   0        0        0       49 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_1_do_expression.html
+-rw-rw-rw-   0        0        0       86 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_2_do_macro.html
+-rw-rw-rw-   0        0        0      213 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_3_do_assign.html
+-rw-rw-rw-   0        0        0       22 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_0_echo_basic.html
+-rw-rw-rw-   0        0        0       50 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_1_echo_expression.html
+-rw-rw-rw-   0        0        0      102 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_2_echo_macro.html
+-rw-rw-rw-   0        0        0      219 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_3_echo_macro_recur.html
+-rw-rw-rw-   0        0        0       37 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_0_include_string.html
+-rw-rw-rw-   0        0        0       33 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_1_include_variable.html
+-rw-rw-rw-   0        0        0      520 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_3_include_with.html
+-rw-rw-rw-   0        0        0       58 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_4_include_default_scope.html
+-rw-rw-rw-   0        0        0       45 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_5_include_ignore_missing.html
+-rw-rw-rw-   0        0        0       73 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_6_include_only.html
+-rw-rw-rw-   0        0        0       83 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_7_include_chain.html
+-rw-rw-rw-   0        0        0      114 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_8_include_scope.html
+-rw-rw-rw-   0        0        0      196 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_09_0_raw.html
+-rw-rw-rw-   0        0        0       14 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_10_0_variable_filters.html
+-rw-rw-rw-   0        0        0      115 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_10_1_comments.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_11_0_escaping.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_12_0_whitespace.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_12_1_string_interpolation.html
+-rw-rw-rw-   0        0        0     6340 2023-05-16 07:18:23.000000 blendedUx_Lang-1.1.0/blended/sets.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.244664 blendedUx_Lang-1.1.0/blended/testapp/
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.250657 blendedUx_Lang-1.1.0/blended/testapp/__pycache__/
+-rw-rw-rw-   0        0        0      586 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/__pycache__/manage.cpython-311.pyc
+-rw-rw-rw-   0        0        0      413 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/__pycache__/manage.cpython-38.pyc
+-rw-rw-rw-   0        0        0      260 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.261721 blendedUx_Lang-1.1.0/blended/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.294261 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/
+-rw-rw-rw-   0        0        0      212 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      195 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2596 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/settings.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/settings.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1123 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/urls.cpython-311.pyc
+-rw-rw-rw-   0        0        0      984 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/urls.cpython-38.pyc
+-rw-rw-rw-   0        0        0      734 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/wsgi.cpython-311.pyc
+-rw-rw-rw-   0        0        0      598 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/wsgi.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3067 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      778 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/wsgi.py
+-rw-rw-rw-   0        0        0    10880 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/trimfloat.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.110226 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13553 2023-07-14 05:41:48.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:41:50.298258 blendedUx_Lang-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      527 2023-07-14 05:35:03.000000 blendedUx_Lang-1.1.0/setup.py
```

### Comparing `blendedUx_Lang-1.0.0/LICENSE` & `blendedUx_Lang-1.1.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Cognam Technologies
+Copyright (c) 2016 agua-man
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/_compat.py` & `blendedUx_Lang-1.1.0/blended/customtags/_compat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-    jinja2._compat
+    customtags._compat
     ~~~~~~~~~~~~~~
 
     Some py2/py3 compatibility support based on a stripped down
     version of six so we don't have to depend on a specific version
     of it.
 
     :copyright: Copyright 2013 by the Jinja team, see AUTHORS.
@@ -18,15 +18,14 @@
 
 
 if not PY2:
     unichr = chr
     range_type = range
     text_type = str
     string_types = (str,)
-    integer_types = (int,)
 
     iterkeys = lambda d: iter(d.keys())
     itervalues = lambda d: iter(d.values())
     iteritems = lambda d: iter(d.items())
 
     import pickle
     from io import BytesIO, StringIO
@@ -48,15 +47,14 @@
     get_next = lambda x: x.__next__
 
 else:
     unichr = unichr
     text_type = unicode
     range_type = xrange
     string_types = (str, unicode)
-    integer_types = (int, long)
 
     iterkeys = lambda d: d.iterkeys()
     itervalues = lambda d: d.itervalues()
     iteritems = lambda d: d.iteritems()
 
     import cPickle as pickle
     from cStringIO import StringIO as BytesIO, StringIO
@@ -80,14 +78,20 @@
     get_next = lambda x: x.next
 
     def encode_filename(filename):
         if isinstance(filename, unicode):
             return filename.encode('utf-8')
         return filename
 
+try:
+    next = next
+except NameError:
+    def next(it):
+        return it.next()
+
 
 def with_metaclass(meta, *bases):
     # This requires a bit of explanation: the basic idea is to make a
     # dummy metaclass for one level of class instanciation that replaces
     # itself with the actual metaclass.  Because of internal type checks
     # we also need to make sure that we downgrade the custom metaclass
     # for one level to something closer to type (that's why __call__ and
@@ -102,10 +106,45 @@
             if this_bases is None:
                 return type.__new__(cls, name, (), d)
             return meta(name, bases, d)
     return metaclass('temporary_class', None, {})
 
 
 try:
+    from collections.abc import Mapping as mapping_types
+except ImportError:
+    import UserDict
+    mapping_types = (UserDict.UserDict, UserDict.DictMixin, dict)
+
+
+# common types.  These do exist in the special types module too which however
+# does not exist in IronPython out of the box.  Also that way we don't have
+# to deal with implementation specific stuff here
+class _C(object):
+    def method(self): pass
+def _func():
+    yield None
+function_type = type(_func)
+generator_type = type(_func())
+method_type = type(_C().method)
+code_type = type(_C.method.__code__)
+try:
+    raise TypeError()
+except TypeError:
+    _tb = sys.exc_info()[2]
+    traceback_type = type(_tb)
+    frame_type = type(_tb.tb_frame)
+
+
+try:
     from urllib.parse import quote_from_bytes as url_quote
 except ImportError:
     from urllib import quote as url_quote
+
+
+try:
+    from thread import allocate_lock
+except ImportError:
+    try:
+        from threading import Lock as allocate_lock
+    except ImportError:
+        from dummy_thread import allocate_lock
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/colormap.py` & `blendedUx_Lang-1.1.0/blended/colormap.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/djangolint/views.py` & `blendedUx_Lang-1.1.0/blended/djangolint/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from django.http import HttpResponse
 from django.shortcuts import render
 from django.views.decorators.csrf import csrf_exempt
 
 from antlr4.InputStream import InputStream
-from blendedUxLang.blended.lint.lint import lint
+from blended.lint.lint import lint
 
 
 @csrf_exempt
 def validate(request):
     """
     view to return error messages if passed string is invalid.
     """
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/models.py` & `blendedUx_Lang-1.1.0/blended/djangotags/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 By default (i.e. if it is unspecified), the AUTOESCAPE_DEFAULT is False, but it can be overridden
 in the settings.  If the original default Django functionality is required, set AUTOESCAPE_DEFAULT
 to True.
 """
 
 from django.conf import settings
-from blendedUxLang.blended.djangotags.templatetags.blended_tags import register
+from blended.djangotags.templatetags.blended_tags import register
 from django.template.context import Context, RequestContext
 
 TEMPLATES = getattr(settings, 'TEMPLATES', None)
 
 if TEMPLATES and ('OPTIONS' in TEMPLATES) and ('override_builtins' in TEMPLATES['OPTIONS']):
     OVERRIDE_BUILTINS = TEMPLATES['OPTIONS']['override_builtins']
 elif getattr(settings, 'OVERRIDE_BUILTINS', None):
@@ -37,16 +37,21 @@
     from django.template.base import builtins
     if OVERRIDE_BUILTINS:
         builtins.append(register)
 except ImportError:
     from django.template.engine import Engine
     if OVERRIDE_BUILTINS:
         Engine.default_builtins.append('blended.djangotags.templatetags.blended_tags')
-    
 
+'''
+Engine.default_builtins = 
+                        ['django.template.defaulttags', 'django.template.defaultfilters', 
+                        'django.template.loader_tags', 'blended.djangotags.templatetags.blended_tags']
+'''   
+# breakpoint()
 
 def wrap_context_init(__init__):
     def __wrapinit__(self, dict_=None, autoescape=None, **kwargs):
         if autoescape is None:
             autoescape = getattr(settings, 'AUTOESCAPE_DEFAULT', False)
         return __init__(self, dict_, autoescape=autoescape, **kwargs) 
     return __wrapinit__
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/djangotags/templatetags/blended_tags.py` & `blendedUx_Lang-1.1.0/blended/djangotags/templatetags/blended_tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
+import posixpath
 import sys
 import warnings
 import collections
 import datetime
-
+import json
 from copy import copy
 from numbers import Number
+from django.template.base import Parser as dj_parser
+from django.template.base import VariableDoesNotExist
 
 from django.template import Template
 from django.template import Library, Context, RequestContext, Variable, TemplateSyntaxError
 from django.template.loader import get_template
 from django.template.loader_tags import ExtendsNode, BlockNode
-from django.utils.safestring import mark_safe, EscapeText
-
+from django.utils.safestring import mark_safe
+from django.template.exceptions import TemplateDoesNotExist
 try:
     from django.template.defaultfilters import escape_filter
 except ImportError:
     from django.template.defaultfilters import escape as escape_filter
 try:
     from django.utils.encoding import force_text 
 except ImportError:
@@ -26,30 +29,31 @@
 try:
     from django.utils.deprecation import RemovedInDjango110Warning as DjangoDeprecationWarning
 except ImportError:
     DjangoDeprecationWarning = DeprecationWarning
 try:
     from django.utils.six import string_types
 except ImportError:
-    string_types = basestring
+    string_types = TypeError
 try:
     from django.template.base import Template as BaseTemplate
     template_types = (Template, BaseTemplate)
 except ImportError:
     template_types = Template
-try:
-    from django.template.base import render_value_in_context
-except ImportError:
-    from django.template.base import _render_value_in_context as render_value_in_context
 
-from customtags import core, arguments, utils
-from customtags._compat import text_type
-from customtags.trimfloat import trimfloat
-from blendedUxLang.blended.djangotags.loader import template_from_string
-from blendedUxLang.blended.functions import builtins as builtin_funcs
+from django.template.base import render_value_in_context
+
+
+from blended.customtags import core, arguments, utils
+from blended.customtags._compat import text_type
+from blended.customtags.trimfloat import trimfloat
+from blended.djangotags.loader import template_from_string
+from blended.functions import builtins as builtin_funcs
+from blended.customtags.exceptions import *
+
 
 register = Library()
 
 datetime_isoformat = "%Y-%m-%dT%H:%M:%SZ"
 numbers_default_string_format = "%g"
 PYTHON_MAJOR_VER = sys.version_info[0]
 
@@ -66,20 +70,14 @@
 class Parent(core.Tag):
     parent_var = Variable('block.super')
 
     def render_tag(self, context):
         return self.parent_var.resolve(context)
 
 
-class Print(core.Tag):
-    options = core.Options(arguments.Argument("expression"))
-
-    def render_tag(self, context, expression):
-        expression = '' if expression is None or (isinstance(expression, EscapeText) and expression == 'None') else expression
-        return render_value_in_context(expression, context)
 
 
 class Do(core.Tag):
     options = core.Options(arguments.Argument("expression"))
 
     def render_tag(self, context, expression):
          return ""
@@ -108,14 +106,15 @@
 
 
 class Autoescape(core.Tag):
     options = core.Options(
         arguments.Argument("autoescape_on"),
         arguments.NodeList("nodelist"),
         arguments.EndTag()
+
     )
 
     def render_tag(self, context, autoescape_on, nodelist):
         old_setting = context.autoescape
         context.autoescape = autoescape_on
         output = nodelist.render(context)
         context.autoescape = old_setting
@@ -135,29 +134,30 @@
     rc = context.render_context
     rc['macros'] = macro_context
 
 
 def get_new_context(context, initial_data=None):
     if not initial_data:
         initial_data = {}
-
     ## the request context will allow us to populate the context with all
     ## global/default data, but that is only available if we already have a 
     ## RequestContext via context processors 
-
+    # if isinstance(context, RequestContext):
+    #     new_context = RequestContext(context.request, initial_data, autoescape=context.autoescape)
     if isinstance(context, RequestContext):
         #new_context = RequestContext(context.request, initial_data, autoescape=context.autoescape)
         from copy import copy, deepcopy
         """
         Instantiating RequestContext constructure is causing
         all the context_processors to execute everytime this is being called.
         # deepcopy throwing TypeError("cannot serialize '_io.BufferedReader' object")
         """
         new_context = copy(context)
         new_context.update(builtin_funcs())
+
     ## If we don't have a RequestContext, then we need to invoke the builtins
     ## context processor directly.  User functions will not be available
     ## inside the macro body unless added originally to the macro context.
 
     else:
         new_context = Context(autoescape=context.autoescape)
         new_context.update(builtin_funcs())
@@ -174,42 +174,42 @@
                                      required=False, commas=True),
         arguments.Constant(")"),
         arguments.NodeList("nodelist"),
         arguments.EndTag()
     )
 
     def render_tag(self, context, macroname, arg_names, nodelist):
-        macro_context = get_macro_context(context)
-        
+
         def macro(*args):
             #if len(arg_names) != len(args):
             #    raise TypeError("Macro '%s' expects %s arguments, %s provided." % 
             #                    (macroname, len(arg_names), len(args)))
-
-            #macro_context = get_macro_context(context)
+                
+            macro_context = get_macro_context(context)
             macro_context.push()
 
             ## get a fully scoped context with the macros as initial data
             inner_context = get_new_context(context, copy(macro_context))
             set_macro_context(inner_context, macro_context)
+
             i = 0
             for arg_name in arg_names:
                 try:
                   inner_context[arg_name] = args[i]
                 except IndexError:
                   break
                 i += 1
             rendered = nodelist.render(inner_context)
             macro_context.pop()
             return rendered
         macro.is_macro = True
         macro.name = macroname
 
-        #macrocontext = get_macro_context(context)
-        macro_context[macroname] = context[macroname] = macro
+        macrocontext = get_macro_context(context)
+        macrocontext[macroname] = context[macroname] = macro
         return ""
 
 
 def import_macros(context, template):
 
     # Does this quack like a Template?
     if not callable(getattr(template, 'render', None)):
@@ -271,15 +271,60 @@
             name = nameobj['name']
             if name not in macros_dict:
                 raise ImportError("Macro name '%s' not found in template." % name)
             if 'asname' in nameobj:
                 context[nameobj['asname']] = macros_dict[nameobj['name']]
             else:
                 context[nameobj['name']] = macros_dict[nameobj['name']]
-        return ""
+        
+        return ''
+
+
+def construct_relative_path(current_template_name, relative_name):
+    """
+    Convert a relative path (starting with './' or '../') to the full template
+    name based on the current_template_name.
+    """
+    new_name = relative_name.strip("'\"")
+    # breakpoint()
+    if not new_name.startswith(("./", "../")):
+        # relative_name is a variable or a literal that doesn't contain a
+        # relative path.
+        return relative_name
+    new_name = posixpath.normpath(
+        posixpath.join(
+            posixpath.dirname(current_template_name.lstrip("/")),
+            new_name,
+        )
+    )
+
+    if new_name.startswith("../"):
+        if repr(relative_name).startswith("'\""):           # this will generate error for "extend tag" as Django wanted  
+            raise TemplateSyntaxError(
+                "The relative path '%s' points outside the file hierarchy that "
+                "template '%s' is in." % (relative_name, current_template_name)
+            )
+        else:           # this will generate error for "include tag" as Django wanted                   
+            raise TemplateSyntaxError(
+                "The relative path '%s' points outside the file hierarchy that "
+                "template '%s' is in." % (json.dumps(relative_name), current_template_name)
+            )
+    if current_template_name.lstrip("/") == new_name:
+        raise TemplateSyntaxError(
+            "The relative path '%s' was translated to template name '%s', the "
+            "same template in which the tag appears."
+            % (relative_name, current_template_name)
+        )
+    has_quotes = (
+        relative_name.startswith(('"', "'")) and relative_name[0] == relative_name[-1]
+    )
+    # if not get_template(new_name):
+    #     breakpoint()
+    return f'"{new_name}"' if has_quotes else new_name
+
 
 
 class Include(core.Tag):
     options = core.Options(
         arguments.Argument("template"),
         arguments.Optional(
             arguments.Constant("ignore"),
@@ -308,48 +353,83 @@
         ),
     )
 
     def render_tag(self, context, template, extra_context=None, isolation=False, ignore=False):
         try:
             extra_context = extra_context if extra_context else {}
 
-            if not isinstance(extra_context, collections.Mapping):
+            if not isinstance(extra_context, collections.abc.Mapping):
                 raise TemplateSyntaxError(
                     "Extra context passed to include tag must act like a dict.")
 
             # Does this quack like a Template?
+            # added as like in django == 4.1.7
             if not callable(getattr(template, 'render', None)):
                 # If not, we'll try get_template
-                template = context.template.engine.get_template(template)
+                # template = context.template.engine.get_template(template)
+                # if "./../three.html" in template:
+                #     breakpoint()
+                template_name = template
+                if isinstance(template_name, str):
+                    template_name = (
+                        construct_relative_path(
+                            self.origin.template_name,
+                            template_name,
+                        ),
+                    )
+                else:
+                    # this will handle the case if typeof template_name is Nonetype, can't iterate through NoneType
+                    if template_name == None:    
+                        raise TemplateDoesNotExist("No template names provided")
+                    
+                    template_name = tuple(template_name)
+                cache = context.render_context.dicts[0].setdefault(self, {})
+                template = cache.get(template_name)
+                if template is None:
+                    template = context.template.engine.select_template(template_name)
+                    cache[template_name] = template
+            elif hasattr(template, "template"):
+                template = template.template
+            
+    
             old_ae_setting = context.autoescape
             if old_ae_setting:
                 context.autoescape = not old_ae_setting
             if isolation:
                 rendered = template.render(get_new_context(context, extra_context))
                 context.autoescape = old_ae_setting
                 return rendered
 
             ## this should be implemented as 'with context.push(**extra_context)'
             ## but we can't do that because we are supporting old Django
+            
             context.update(extra_context)
             rendered = template.render(context)
             context.pop()
             context.autoescape = old_ae_setting
             return rendered
-
-        except Exception as e:
-            if hasattr(context, 'template'):
-                if context.template.engine.debug:
-                    raise
-                return ''
+        # modified the exception because Blended support for "ignore missing" argument with include tag
+        # Django remove the "ignore missing" functionalities from version 2.x
+        except TemplateDoesNotExist:
+            bits = self.token.split_contents()
+            if bits[-2] == "ignore" and bits[-1] == "missing":
+                if hasattr(context, 'template'):
+                    # print(context.template.name)
+                    if context.template.engine.debug:
+                        raise
+                    return ''
+                else:
+                    from django.conf import settings
+                    if settings.DEBUG:
+                        raise 
+                    return ''
+            elif template_name == None:
+                raise TemplateDoesNotExist("No template names provided")
             else:
-                from django.conf import settings
-                if settings.TEMPLATE_DEBUG:
-                    raise
-                return ''
+                raise TemplateDoesNotExist("".join(template_name))
 
 
 class If(core.Tag):
     options = core.Options(
         arguments.Argument('conditional'),
         arguments.NodeList('nodelist'),
         arguments.Repetition(
@@ -360,40 +440,45 @@
                 arguments.NodeList('nodelist', endtags=['elif','else','endif']),
             ),
         ),
         arguments.Optional(
             arguments.BlockTag('else'),
             arguments.NodeList('elsenodelist'),
         ),
+        
         arguments.EndTag()
     )
 
     def render_tag(self, context, conditional, nodelist, elifs, elsenodelist=None):
-        if conditional:
+        if conditional:                
             return nodelist.render(context)
         for block in elifs:
             if block['conditional']:
                 return block['nodelist'].render(context)
         if elsenodelist:
             return elsenodelist.render(context)
-        return ""
+        return ''
+
+        
+        
 
 class Ifblock(core.Tag):
     name = 'ifblock'
     options = core.Options(
         arguments.MultiValueArgument('block_names', resolve=False),
         arguments.NodeList('nodelist'),
         arguments.Optional(
             arguments.BlockTag('else'),
             arguments.NodeList('elsenodelist'),
         ),
         arguments.EndTag()        
     )
     
     def render_tag(self, context, block_names, nodelist, elsenodelist=None):
+        # breakpoint()
         nodes_list = context.template.nodelist.get_nodes_by_type(BlockNode)
         result = []
         for node in nodes_list:
             if node.name in block_names:
                 exp_value = node.render(context).strip()
             else:
                 exp_value = ''        
@@ -426,15 +511,14 @@
 
     def render_tag(self, context, loopvars, values, is_reversed, pre_empty, post_empty=None):
         if 'forloop' in context:
             parentloop = context['forloop']
         else:
             parentloop = {}
         #with context.push():
-
         context.push()
         if values is None:
             values = []
         if not hasattr(values, '__len__'):
             values = list(values)
         len_values = len(values)
         if len_values < 1:
@@ -463,25 +547,33 @@
                 if unpack:
                     # If there are multiple loop variables, unpack the item into
                     # them.
 
                     # To complete this deprecation, remove from here to the
                     # try/except block as well as the try/except itself,
                     # leaving `unpacked_vars = ...` and the "else" statements.
-                    if not isinstance(item, (list, tuple)):
+                    if isinstance(item, str):
+                        len_item = len(item)
+                    elif not isinstance(item, (list, tuple)):
                         len_item = 1
                     else:
                         len_item = len(item)
                     # Check loop variable count before unpacking
                     if num_loopvars != len_item:
+                        # breakpoint()
                         warnings.warn(
                             "Need {} values to unpack in for loop; got {}. "
                             "This will raise an exception in Django 1.10."
                             .format(num_loopvars, len_item),
                             DjangoDeprecationWarning)
+                        raise ValueError(                   
+                            "Need {} values to unpack in for loop; got {}. ".format(
+                                num_loopvars, len_item
+                            ),
+                        )
                     try:
                         unpacked_vars = dict(zip(loopvars, item))
                     except TypeError:
                         pass
                     else:
                         pop_context = True
                         context.update(unpacked_vars)
@@ -489,16 +581,15 @@
                     context[loopvars[0]] = item
                 # In debug mode provide the source of the node which raised
                 # the exception
                 try:
                     debug_mode = context.template.engine.debug
                 except:
                     from django.conf import settings
-                    debug_mode = settings.TEMPLATE_DEBUG
-
+                    debug_mode = settings.DEBUG
                 if debug_mode:
                     for node in pre_empty:
                         try:
                             nodelist.append(node.render(context))
                         except Exception as e:
                             if not hasattr(e, 'django_template_source'):
                                 e.django_template_source = node.source
@@ -510,38 +601,54 @@
                     # The loop variables were pushed on to the context so pop them
                     # off again. This is necessary because the tag lets the length
                     # of loopvars differ to the length of each set of items and we
                     # don't want to leave any vars from the previous loop on the
                     # context.
                     context.pop()
             retval = mark_safe(''.join(force_text(n) for n in nodelist))
-
+        
         context.pop()
         return retval
 
 
 extends_options = core.Options(arguments.Expression())
 extends_options.initialize('extends')
 
 def do_extends(parser, token):
+    bits = token.split_contents()
+    if len(bits) <= 1:
+        raise TemplateSyntaxError("'%s' takes one argument" % bits[0])
+
+    bits[1] = construct_relative_path(parser.origin.template_name, bits[1])
+    '''
+     I have to pass this bits[1] in value of '<StringValue(Const(value='./dir2/one.html'))>'
+     container.tag_args[0].var --> Const(value='./dir2/one.html')
+     container.tag_args[0].var.value --> './dir2/one.html'
 
+    '''
+    # breakpoint()
     container = utils.Container()
     extends_options.parse(parser, token, container)
+    if (bits[1] != token.split_contents()[-1]):
+        container.tag_args[0].var.value = bits[1].strip('"')
 
     parent_name = container.tag_args[0]
+
+    # breakpoint()
+    
     parent_name.token = token
     nodelist = parser.parse()
     if nodelist.get_nodes_by_type(ExtendsNode):
         raise TemplateSyntaxError(
             "'%s' cannot appear more than once in the same template" % bits[0])
     try:
         return ExtendsNode(nodelist, parent_name)
     except TypeError:
         return ExtendsNode(nodelist, None, parent_name)
-
+        
 
 def items_filter(dict_val):
     try:
         keys = sorted(dict_val.keys())
     except:
         keys = dict_val.keys() 
         keys.sort()
@@ -568,15 +675,16 @@
         return template_obj
     elif isinstance(template, template_types):
         return template
     else:
         #raise TypeError("The `template` filter must be applied only to strings or templates.")
         ## or just convert it to a string first:
         template_obj = template_from_string(str(template))
-        return template_obj
+        return template_obj 
+    
 
 
 def render_filter(template, context=None, autoescape=None):
     autoescape = False if autoescape is None else autoescape
 
     if context is None:
         context = {}
@@ -651,28 +759,43 @@
         if formatting:
             return datetime.datetime.strptime(obj, formatting)
         else:
             return datetime.datetime.strptime(obj, datetime_isoformat)
     elif isinstance(obj, list):
         return datetime.datetime(*map_func(int, obj), tzinfo=None)
 
+from django.utils.safestring import SafeText
+class Print(core.Tag):
+    options = core.Options(arguments.Argument("expression"))
+    def render_tag(self, context, expression):
+        expression = '' if expression is None or (isinstance(expression, SafeText) and expression == 'None') else expression
+        return render_value_in_context(expression, context)
+
+
+from django.template.defaultfilters import first
+
+
+# register.tag(Verbatim.as_tag())            #use verbatim default
+
+register.tag(If.as_tag())
+register.tag(Ifblock.as_tag())
 
+
+# # 
 register.tag(Parent.as_tag())
 register.tag(Print.as_tag())
 register.tag(Do.as_tag())
 register.tag(Set.as_tag())
-register.tag(Verbatim.as_tag())
-register.tag(Autoescape.as_tag())
-register.tag(Macro.as_tag())
 register.tag(Import.as_tag())
 register.tag(From.as_tag())
-register.tag(Include.as_tag())
-register.tag(If.as_tag())
-register.tag(Ifblock.as_tag())
 register.tag(For.as_tag())
+register.tag(Autoescape.as_tag())
+register.tag(Macro.as_tag())
+register.tag(Include.as_tag())
+# add due to blended
 register.tag('extends', do_extends)
 register.filter('items', items_filter)
 register.filter('number', number_filter)
 register.filter('e', escape_filter)
 register.filter('escape', escape_filter)
 register.filter('string', string_filter)
 register.filter('template', template_filter)
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/functions.py` & `blendedUx_Lang-1.1.0/blended/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import re
 import math
 import datetime
+from jinja2 import filters as flt
 
-from blendedUxLang.blended.sets import intersection, union,\
-     symmetric_difference, complement, cartisan_product
-from blendedUxLang.blended.colormap import color_map
-from blendedUxLang.blended._compat import string_types
 
+import re
+import math
+import datetime
+
+from blended.sets import intersection, union,\
+     symmetric_difference, complement, cartisan_product
+from blended.colormap import color_map
+from blended._compat import string_types
+from blended.trimfloat import trimfloat, trimint
 HEX_COLOR_RE = re.compile(r'^#([a-fA-F0-9]{3}|[a-fA-F0-9]{6})$')
 HEX_COLOR_RE_WITHOUT_HASH = re.compile(r'^([a-fA-F0-9]{3}|[a-fA-F0-9]{6})$')
 
 def float_range(start, end=None, increment=None):
     """Take float and integer value as input argument and return range.
     work same as python range.
     """
@@ -98,20 +104,21 @@
         return "argument in title function must be string, int or float"
     if isinstance(arg, str):
         return arg.title()
     return None
 
 def blendedround(number, precision=0):
     """rounds a number to the nearest whole number"""
-    if (number.__class__.__name__ == 'Markup'):
-        number = float(number.unescape().strip("'"))
-    try:
-        return round(number, precision)
-    except TypeError:
-        return round(float(str(number)), precision)
+    if isinstance(number, str):
+        return trimfloat(round(float(number), precision))
+    if isinstance(number, int):
+        return trimint(round(number, precision))     # include trimint
+    else:
+        return trimfloat(round(number, precision))   # include trimfloat 
+    
 
 def ceil(value):
     """Rounds the value up to the nearest int."""
     if not isinstance(value, float):
         value = float(value)
     if isinstance(value, float):
         return math.ceil(value)
@@ -234,14 +241,15 @@
 
 def now():
     """
     Return a datetime object for the current time of the day
     """
     return datetime.datetime.now()
 
+
 def builtins(request=None):
     """
     return builtin fucitons
     """
     return {
         'range':float_range,
         'cycle':cycle,
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/jinjaenv.py` & `blendedUx_Lang-1.1.0/blended/jinjaenv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,137 @@
+
+import os
+import re
+import sys
+import jinja2
+import unittest
+import json
+from jinja2.utils import htmlsafe_json_dumps as Markup    # add for Markup
+from unittest import TestCase
+from jinja2 import Environment, Template
+from jinja2.compiler import CodeGenerator
+from jinja2.runtime import Undefined 
+# from jinja2 import Undefined 
+from jinja2.sandbox import safe_range
+from jinja2.nodes import OverlayScope
+from collections.abc import Mapping
+import traceback
 import sys
 import re
 import datetime
-
-from collections import Mapping
+from jinja2.parser import Parser
 from numbers import Number
 from functools import reduce
 
 import jinja2
 import jinja2.ext
 import jinja2.sandbox
 
 from jinja2 import nodes
-from jinja2.runtime import Undefined, Macro
+from jinja2.runtime import  Macro
 from jinja2.environment import TemplateExpression
-from jinja2._compat import encode_filename, string_types, iteritems,\
+from blended._compat import encode_filename, string_types, iteritems,\
      text_type, imap
-from jinja2.utils import Markup
 from jinja2.defaults import BLOCK_START_STRING,\
     BLOCK_END_STRING, VARIABLE_START_STRING, VARIABLE_END_STRING,\
     COMMENT_START_STRING, COMMENT_END_STRING, LINE_STATEMENT_PREFIX,\
     LINE_COMMENT_PREFIX, TRIM_BLOCKS, NEWLINE_SEQUENCE,\
     KEEP_TRAILING_NEWLINE, LSTRIP_BLOCKS
 
-from blendedUxLang.blended.functions import builtins
-from blendedUxLang.blended.trimfloat import trimfloat, trimint
 
-datetime_isoformat = "%Y-%m-%dT%H:%M:%SZ"
-numbers_default_string_format = "%g"
+from blended.functions import builtins
+from blended.trimfloat import trimfloat, trimint
 
-class BlendedTemplate(jinja2.environment.Template):
-    """Template class for Blended"""
-    spontaneous_environments = jinja2.utils.LRUCache(10)
 
-    def __new__(cls, source,
-                block_start_string=BLOCK_START_STRING,
-                block_end_string=BLOCK_END_STRING,
-                variable_start_string=VARIABLE_START_STRING,
-                variable_end_string=VARIABLE_END_STRING,
-                comment_start_string=COMMENT_START_STRING,
-                comment_end_string=COMMENT_END_STRING,
-                line_statement_prefix=LINE_STATEMENT_PREFIX,
-                line_comment_prefix=LINE_COMMENT_PREFIX,
-                trim_blocks=TRIM_BLOCKS,
-                lstrip_blocks=LSTRIP_BLOCKS,
-                newline_sequence=NEWLINE_SEQUENCE,
-                keep_trailing_newline=KEEP_TRAILING_NEWLINE,
-                extensions=(),
-                optimized=True,
-                undefined=Undefined,
-                finalize=None,
-                autoescape=False,
-                trim_floats=True,
-                dict_attrs=False):
-        # only changed this to use BlendedEnvironment
-        env = cls.get_spontaneous_blended_environment(
-            block_start_string, block_end_string, variable_start_string,
-            variable_end_string, comment_start_string, comment_end_string,
-            line_statement_prefix, line_comment_prefix, trim_blocks,
-            lstrip_blocks, newline_sequence, keep_trailing_newline,
-            frozenset(extensions), optimized, undefined, finalize, autoescape,
-            trim_floats, dict_attrs, None, 0, False, None)
-        return env.from_string(source, template_class=cls)
+class BlendedParser(jinja2.parser.Parser):
+    """
+    This parser subclass overrides the parsing of the include tag, in order to provide
+    a local context feature.  It also overrides parse_primary to ensure that numbers are
+    printed without trailing zeros.
+    """
+    def _wrap_as_const(self, as_const):
+        """
+        """
+        def as_const_wrapper(eval_ctx=None):
+            """
+            """
+            value = as_const(eval_ctx)
+            if isinstance(value, Number):
+                return self.environment._trimfloat(value)
+            return value
+        return as_const_wrapper
 
-    @classmethod
-    def get_spontaneous_blended_environment(cls, *args):
-        """This is just implemented here to be able to use BlendedEnvironment"""
-        try:
-            env = cls.spontaneous_environments.get(args)
-        except TypeError:
-            return BlendedEnvironment(*args)
-        if env is not None:
-            return env
-        cls.spontaneous_environments[args] = env = BlendedEnvironment(*args)
-        env.shared = True
-        return env
+    def _wrap_parse(parse_method):
+        """
+        """
+        def parse_wrapper(self, *args, **kwargs):
+            """
+            """
+            node = parse_method(self, *args, **kwargs)
+            if node == None:              # add this because sometimes may be node is NoneType object
+                return node
+            node.as_const = self._wrap_as_const(node.as_const)
+            return node
+        
+        return parse_wrapper
 
-    def new_context(self, vars=None, shared=False, locals=None, args=None):
-        """Reimplementation of Template.new_context,
-        needed for handling Include node args.
+    parse_primary = _wrap_parse(jinja2.parser.Parser.parse_primary)
+    parse_filter = _wrap_parse(jinja2.parser.Parser.parse_filter)
+    
+    def parse_include(self):
         """
-        if args:
-            new_locals = dict(locals) if locals else {}
-            for key, value in iteritems(args):
-                new_locals['l_' + key] = value
+        Reimplementation of Parser.parse_include, necessary for new Include functionality
+        """
+        lineno = lineno = next(self.stream).lineno
+        node = nodes.Include(lineno=lineno)
+        node.fields = nodes.Include.fields + ('with_expression',) ## compiler needs this
+
+        node.template = self.parse_expression()
+        if self.stream.current.test('name:ignore') and\
+           self.stream.look().test('name:missing'):
+            node.ignore_missing = True
+            self.stream.skip(2)
         else:
-            new_locals = locals
+            node.ignore_missing = False
 
-        return jinja2.runtime.new_context(self.environment, self.name, self.blocks,
-                                          vars, shared, self.globals, new_locals)
+        node.with_expression = None
+        if self.stream.current.test_any('name:with', 'name:without') and\
+           self.stream.look().test('name:context'):
+            node.with_context = next(self.stream).value == 'with'
+            self.stream.skip()
+        elif self.stream.current.test('name:with'):
+            self.stream.skip()
+            node.with_expression = self.parse_expression()
+            if self.stream.current.test('name:only'):
+                node.with_context = False
+                self.stream.skip()
+            else:
+                node.with_context = True
 
-###
-### Extensions and Filters
-###
+        elif self.stream.current.test('name:only'):
+            node.with_context = False
+            self.stream.skip()
+        else:
+            node.with_context = True
+        return node
+
+
+# add custom extension
+class CommentExtension(jinja2.ext.Extension):
+    """Extension for comment tag."""
+    tags = set(['comment'])
+
+    def parse(self, parser):
+        token = parser.stream.current
+        lineno = next(parser.stream).lineno
+        if token.type == 'name' and token.value == 'comment':
+            parser.parse_statements(['name:endcomment'], drop_needle=True)
+            return nodes.Const("")
+        else:
+            jinja2.exceptions.TemplateSyntaxError("Expected token 'comment'")
 
 class ParentExtension(jinja2.ext.Extension):
     """Extension for Parent tag."""
     tags = set(['parent'])
 
     def parse(self, parser):
         """
@@ -121,17 +157,22 @@
         param_count = len(params)
 
         if param_count == 1:
             node.test = self.build_test(params[0], lineno)
         else:
             node.test = self.get_or_expr(params, param_count-1, lineno)
 
-        node.body = parser.parse_statements(('name:else', 'name:endifblock'))
+        node.body = parser.parse_statements(('name:elif','name:else', 'name:endifblock'))
+        node.elif_ = []
         token = next(parser.stream)
-        if token.test('name:else'):
+        if token.test("name:elif"):
+            node = nodes.If(lineno=self.stream.current.lineno)
+            result.elif_.append(node)
+
+        elif token.test('name:else'):
             node.else_ = parser.parse_statements(('name:endifblock',), drop_needle=True)
         else:
             node.else_ = []
         return result
 
     def get_or_expr(self, params, index, lineno):
         if index == 0:
@@ -152,73 +193,63 @@
             if (parser_stream.current.type == 'name'):
                 params.append(parser_stream.current.value)
                 next(parser_stream)
             else:
                 raise jinja2.exceptions.TemplateSyntaxError("Expected block name.")
         return params
 
-class CommentExtension(jinja2.ext.Extension):
-    """Extension for comment tag."""
-    tags = set(['comment'])
 
-    def parse(self, parser):
-        token = parser.stream.current
-        lineno = next(parser.stream).lineno
-        if token.type == 'name' and token.value == 'comment':
-            parser.parse_statements(['name:endcomment'], drop_needle=True)
-            return nodes.Const("")
-        else:
-            jinja2.exceptions.TemplateSyntaxError("Expected token 'comment'")
-
-def items_filter(dict_val):
-    """iterate over the given object and list of tuple in key, value
-    representation.
-    """
-    try:
-        keys = sorted(dict_val.keys())
-    except:
-        keys = dict_val.keys()
-        keys.sort()
-    return [(key, dict_val[key]) for key in keys]
 
 def number_filter(value, default=0):
     """Convert the value into an number. basically in float type
     """
     try:
         return float(value)
     except (TypeError, ValueError):
         return default
 
-@jinja2.evalcontextfilter
+
+@jinja2.pass_eval_context
 def render_filter(eval_ctx, template, context=None):
     """renders the context in the template object.
     """
     if context is None:
         context = {}
     elif not isinstance(context, dict):
         raise TypeError("The `render` filter can only be passed a dict as an argument.")
     if hasattr(template, 'render'):
         return template.render(context)
     else:
         raise TypeError("The `render` filter should only be "
                         "applied to objecst that implement `render`.")
 
+
+datetime_isoformat = "%Y-%m-%dT%H:%M:%SZ"
+numbers_default_string_format = "%g"
+# def datetime_filter(obj, formatting=None):
+#     """
+#     Return a datetime object for the current time of the day
+#     """
+#     return datetime.datetime.now()
+
 def datetime_filter(obj, formatting=None):
     """this filter accepts string, list or dates and return a datetime object.
     """
     if isinstance(obj, datetime.datetime):
         return obj
     elif isinstance(obj, text_type):
         if formatting:
             return datetime.datetime.strptime(obj, formatting)
         else:
             return datetime.datetime.strptime(obj, datetime_isoformat)
     elif isinstance(obj, list):
         return datetime.datetime(*imap(int, obj), tzinfo=None)
 
+
+
 class TemplateNull(object):
     """object of class represents 'null' which is replacing None in string_filter
     """
     def __repr__(self):
         return "null"
 
 class TemplateTrue(object):
@@ -233,28 +264,30 @@
     def __repr__(self):
         return "false"
 
 null = TemplateNull()
 true = TemplateTrue()
 false = TemplateFalse()
 
+# use custom string filter we can modified string wrt its format
+
 
 def string_filter(value, format=None, recursion=False):
 
     try:  # try except block to fix the absence of unicode in py3
-        if value and isinstance(value, unicode):
-            value = value.encode('utf-8')
+        if value and isinstance(value, str):
+            value = value
     except NameError:
         pass
-
+    # print(value)
     if format:
         if isinstance(value, Number) and not isinstance(value, bool):
             return format % value
         if isinstance(value, str):
-            return format % trimfloat(value)
+            return format % trimfloat(value)        #include  trimfloat
         elif isinstance(value, datetime.datetime):
             return datetime.datetime.strftime(value, format)
         elif isinstance(value, (list, tuple)):
             rendered = []
             for item in value:
                 rendered.append(string_filter(item))
             return format % tuple(rendered)
@@ -267,44 +300,118 @@
             return 'true' if value else 'false'
         elif isinstance(value, str):
             if recursion:
                 return "'%s'" % value
             else:
                 return "%s" % value
         elif isinstance(value, Number):
-            return str(trimfloat(value))
+            return str(trimfloat(value))              # include trimfloat
         elif isinstance(value, datetime.datetime):
             return datetime.datetime.strftime(value, datetime_isoformat)
         elif isinstance(value, (list, tuple)):
             rendered = []
             for item in value:
                 rendered.append(string_filter(item, recursion=True))
             return "[%s]" % ", ".join(rendered)
         elif isinstance(value, dict):
             rendered = []
             for key in sorted(value.keys()):
                 rendered_value = string_filter(value[key], recursion=True)
                 rendered.append('\'%s\': %s' % (key, rendered_value))
             return "{%s}" % ", ".join(rendered)
+        # elif isinstance(value, type):
+        #     return value.__class__
         else:
             raise TypeError("Type %s unsupported by string filter" % value.__class__)
 
-filters = {
+
+from jinja2.filters import do_dictsort
+filters_add = {
     "render": render_filter,
-    "items": items_filter,
-    "number": number_filter,
+    "items": do_dictsort,
     "string": string_filter,
+    "number": number_filter,
     "datetime": datetime_filter,
 }
+#
+
+
+class BlendedTemplate(jinja2.environment.Template):
+    """Template class for Blended"""
+    spontaneous_environments = jinja2.utils.LRUCache(10)
+
+    def __new__(cls, source,
+                block_start_string=BLOCK_START_STRING,
+                block_end_string=BLOCK_END_STRING,
+                variable_start_string=VARIABLE_START_STRING,
+                variable_end_string=VARIABLE_END_STRING,
+                comment_start_string=COMMENT_START_STRING,
+                comment_end_string=COMMENT_END_STRING,
+                line_statement_prefix=LINE_STATEMENT_PREFIX,
+                line_comment_prefix=LINE_COMMENT_PREFIX,
+                trim_blocks=TRIM_BLOCKS,
+                lstrip_blocks=LSTRIP_BLOCKS,
+                newline_sequence=NEWLINE_SEQUENCE,
+                keep_trailing_newline=KEEP_TRAILING_NEWLINE,
+                extensions=(),
+                optimized=True,
+                undefined=Undefined,
+                finalize=None,
+                autoescape=False,
+                trim_floats=True,
+                dict_attrs=False,
+                enable_async=False,
+                ):
+        # only changed this to use BlendedEnvironment
+        env = cls.get_spontaneous_blended_environment(
+            block_start_string, block_end_string, variable_start_string,
+            variable_end_string, comment_start_string, comment_end_string,
+            line_statement_prefix, line_comment_prefix, trim_blocks,
+            lstrip_blocks, newline_sequence, keep_trailing_newline,
+            frozenset(extensions), optimized, undefined, finalize, autoescape,
+            trim_floats, dict_attrs,enable_async, None, 0, False, None)
+        return env.from_string(source, template_class=cls)
+
+    @classmethod
+    def get_spontaneous_blended_environment(cls, *args):
+        """This is just implemented here to be able to use BlendedEnvironment"""
+        try:
+            env = cls.spontaneous_environments.get(args)
+        except TypeError:
+            return BlendedEnvironment(*args)
+        if env is not None:
+            return env
+        cls.spontaneous_environments[args] = env = BlendedEnvironment(*args)
+        env.shared = True
+        return env
+    
+    def new_context(self, vars=None, shared=False, locals=None, args=None):
+        """Reimplementation of Template.new_context,
+        needed for handling Include node args.
+        """
+        
+        if args:
+            new_locals = dict(locals, **args) if locals else {}
+            # for key, value in new_locals.items():
+            #     new_locals[key] = value
+        else:
+            new_locals = locals
+        return jinja2.runtime.new_context(self.environment, self.name, self.blocks,
+                                          vars, shared, self.globals, new_locals)
+    
+    
+              
+        
+
+# Adding new proper jinja environment with some additional features
 class BlendedEnvironment(jinja2.sandbox.SandboxedEnvironment):
-    """Environment class for blended.
-    """
-    template_class = BlendedTemplate
-    EXTENSIONS = [CommentExtension, ParentExtension, IfblockExtension,
-                  jinja2.ext.do, jinja2.ext.with_, jinja2.ext.autoescape]
+
+    template_class = BlendedTemplate                 # Blended template class
+    EXTENSIONS = [ ParentExtension, IfblockExtension, CommentExtension, jinja2.ext.i18n ]           
+    # jinja don't have ParentExtension, jinja use super() instead of parent
 
     def __init__(self,
                  block_start_string=BLOCK_START_STRING,
                  block_end_string=BLOCK_END_STRING,
                  variable_start_string=VARIABLE_START_STRING,
                  variable_end_string=VARIABLE_END_STRING,
                  comment_start_string=COMMENT_START_STRING,
@@ -315,29 +422,32 @@
                  lstrip_blocks=LSTRIP_BLOCKS,
                  newline_sequence=NEWLINE_SEQUENCE,
                  keep_trailing_newline=True,
                  extensions=(),
                  optimized=True,
                  undefined=Undefined,
                  finalize=None,
-                 autoescape=True,
+                 autoescape=False,
                  loader=None,
                  cache_size=400,
                  auto_reload=True,
                  bytecode_cache=None,
                  trim_floats=True,
                  sandboxed_access=True,
-                 dict_attrs=False):
+                 dict_attrs=False,
+                 enable_async=False,
+                 ):
         """
         The new extensions and functions are added to the environment here
         """
-
+        self.sandboxed = sandboxed_access       # adding the sandboxed parameter
         self.trim_floats = trim_floats
         self.dict_attrs = dict_attrs
         self.sandboxed_access = sandboxed_access
+        self.is_async = enable_async
         extensions = list(extensions)
         extensions.extend(self.EXTENSIONS)
         super(BlendedEnvironment, self).__init__(block_start_string,
                                                  block_end_string,
                                                  variable_start_string,
                                                  variable_end_string,
                                                  comment_start_string,
@@ -352,32 +462,37 @@
                                                  optimized,
                                                  undefined,
                                                  finalize,
                                                  autoescape,
                                                  loader,
                                                  cache_size,
                                                  auto_reload,
-                                                 bytecode_cache)
-
+                                                 bytecode_cache,
+                                                 enable_async        # by adding enable async at this point solve all test related to async_filters
+                                                 )
+        
         self.globals.update(builtins())
+        self.filters.update(filters_add)
         self.globals.update({"null": None})
+        self.globals["range"] = safe_range      # By adding "safe_range" then in this env, only iterate 10000 times in loop
+        
+        
 
         def template_filter(template):
             """filter to create template from the string"""
             if isinstance(template, jinja2.environment.Template):
                 return template
             elif isinstance(template, string_types):
                 return self.from_string(template)
             else:
                 raise TypeError("The `template` filter must only operate on "
                                 "strings or template instances.")
 
         self.filters['template'] = template_filter
-        self.filters.update(filters)
-
+        self.filters.update(filters_add)
     def __substitute(self, val):
         """Substitution of verbaim to raw performs here
         """
         if re.match(r'''{%\s*verbatim\s*%}(.*?){%\s*endverbatim\s*%}''',
                     val.group(0), re.S):
             return "{%% raw %%}%s{%% endraw %%}" % val.group(1)
         elif re.match(r'''{%\s*verbatim\s*%}''', val.group(0)):
@@ -397,70 +512,47 @@
 
     def preprocess(self, source, name=None, filename=None):
         """Preprocesses the source with all extensions.  This is automatically
         called for all parsing and compiling methods but *not* for :meth:`lex`
         because there you usually only want the actual source tokenized.
         Regex for conversion of verbatim to raw tag.
         """
-
         if self.trim_blocks:
             source = re.sub(r'''{%\s*endverbatim\s*%}(\n.*?)''', self.__add_newline, source, re.S)
         ptrn = r'''(?s)(?:{%\s*verbatim\s*%}(.*?))?{%\s*endverbatim\s*%}|{%\s*verbatim\s*%}'''
         source = re.sub(ptrn, self.__substitute, source, re.S)
 
         return reduce(lambda s, e: e.preprocess(s, name, filename),
                       self.iter_extensions(), text_type(source))
 
     def _parse(self, source, name, filename):
         """overridden to change Parser to BlendedParser"""
         return BlendedParser(self, source, name, encode_filename(filename)).parse()
 
-    def _generate(self, source, name, filename, defer_init=False):
+    def _generate(self, source, name, filename, defer_init=False, optimized=True):
         """
         Should be same algorithm as superclass, but with BlendedCodeGenerator instead.
         This is the place to look at the compiled code.
         """
         if not isinstance(source, nodes.Template):
             raise TypeError('Can\'t compile non template nodes')
 
-        generator = BlendedCodeGenerator(self, name, filename, defer_init=defer_init)
+        generator = BlendedCodeGenerator(self, name, filename, defer_init=defer_init, optimized=optimized)
         generator.visit(source)
         result = generator.stream.getvalue()
-
         return result
-
-    def compile_expression(self, source, undefined_to_none=True):
-        """Should be same algorithm as superclass, but with BlendedParser instead"""
-        ## Is this ever called ?
-        parser = BlendedParser(self, source, state='variable')
-        exc_info = None
-        try:
-            expr = parser.parse_expression()
-            if not parser.stream.eos:
-                raise jinja2.exceptions.TemplateSyntaxError('chunk after expression',
-                                                            parser.stream.current.lineno,
-                                                            None, None)
-            expr.set_environment(self)
-        except jinja2.exceptions.TemplateSyntaxError:
-            exc_info = sys.exc_info()
-        if exc_info is not None:
-            self.handle_exception(exc_info, source_hint=source)
-        body = [nodes.Assign(nodes.Name('result', 'store'), expr, lineno=1)]
-        template = self.from_string(nodes.Template(body, lineno=1))
-        return TemplateExpression(template, undefined_to_none)
-
     def _trimfloat(self, value):
         """
         trimfloat method to remove fractional part from float value.
         """
         if self.trim_floats and isinstance(value, Number) and not (isinstance(value, bool) or isinstance(value, complex)):
             if isinstance(value, int):
-                return trimint(value)
+                return trimint(value)     # include trimint
             else:
-                return trimfloat(value)
+                return trimfloat(value)   # include trimfloat
         return value
 
     def getattr(self, obj, attribute):
         """
         """
         if not self.dict_attrs and isinstance(obj, Mapping):
             try:
@@ -481,30 +573,14 @@
         if not self.dict_attrs and isinstance(obj, Mapping):
             try:
                 return self._trimfloat(obj[argument])
             except (TypeError, LookupError):
                 return self.undefined(obj=obj, name=argument)
         return self._trimfloat(super(BlendedEnvironment, self).getitem(obj, argument))
 
-    def call(__self, __context, __obj, *args, **kwargs):
-        """
-        """
-        result = super(BlendedEnvironment, __self).call(__context, __obj, *args, **kwargs)
-        if isinstance(__obj, Macro) and not isinstance(result, Markup):
-            result = Markup(result)
-        return __self._trimfloat(result)
-
-    def call_filter(self, name, value, args=None, kwargs=None, context=None, eval_ctx=None):
-        """
-        """
-        ## Does this ever get called?
-        value = super(BlendedEnvironment, self).call_filter(name, value, args, kwargs,
-                                                            context, eval_ctx)
-        return self._trimfloat(value)
-
 
 class BlendedImmutableEnvironment(BlendedEnvironment):
     '''
 
     '''
     def __init__(self,
                  block_start_string=BLOCK_START_STRING,
@@ -526,142 +602,69 @@
                  autoescape=False,
                  loader=None,
                  cache_size=400,
                  auto_reload=True,
                  bytecode_cache=None,
                  trim_floats=True,
                  sandboxed_access=True,
-                 dict_attrs=True):
+                 dict_attrs=True,
+                 enable_async=False,
+                 ):
                  
         super(BlendedImmutableEnvironment, self).__init__(block_start_string,
                  block_end_string, variable_start_string, variable_end_string,
                  comment_start_string, comment_end_string, line_statement_prefix,
                  line_comment_prefix, trim_blocks, lstrip_blocks, newline_sequence,
                  keep_trailing_newline, extensions, optimized, undefined,
                  finalize, autoescape, loader, cache_size, auto_reload,
-                 bytecode_cache,trim_floats,sandboxed_access,dict_attrs)
+                 bytecode_cache,trim_floats,sandboxed_access,dict_attrs,enable_async)
     
     def is_safe_attribute(self, obj, attr, value):
         if not super(BlendedEnvironment, self).is_safe_attribute(obj, attr, value):
             return False
         return not jinja2.sandbox.modifies_known_mutable(obj, attr)
 
-
-class BlendedParser(jinja2.parser.Parser):
-    """
-    This parser subclass overrides the parsing of the include tag, in order to provide
-    a local context feature.  It also overrides parse_primary to ensure that numbers are
-    printed without trailing zeros.
-    """
-
-    def _wrap_as_const(self, as_const):
-        """
-        """
-        def as_const_wrapper(eval_ctx=None):
-            """
-            """
-            value = as_const(eval_ctx)
-            if isinstance(value, Number):
-                return self.environment._trimfloat(value)
-            return value
-        return as_const_wrapper
-
-    def _wrap_parse(parse_method):
-        """
-        """
-        def parse_wrapper(self, *args, **kwargs):
-            """
-            """
-            node = parse_method(self, *args, **kwargs)
-            node.as_const = self._wrap_as_const(node.as_const)
-            return node
-        return parse_wrapper
-
-    parse_primary = _wrap_parse(jinja2.parser.Parser.parse_primary)
-    parse_filter = _wrap_parse(jinja2.parser.Parser.parse_filter)
-
-    def parse_include(self):
-        """
-        Reimplementation of Parser.parse_include, necessary for new Include functionality
-        """
-        lineno = lineno = next(self.stream).lineno
-        node = nodes.Include(lineno=lineno)
-        node.fields = nodes.Include.fields + ('with_expression',) ## compiler needs this
-
-        node.template = self.parse_expression()
-        if self.stream.current.test('name:ignore') and\
-           self.stream.look().test('name:missing'):
-            node.ignore_missing = True
-            self.stream.skip(2)
-        else:
-            node.ignore_missing = False
-
-        node.with_expression = None
-        if self.stream.current.test_any('name:with', 'name:without') and\
-           self.stream.look().test('name:context'):
-            node.with_context = next(self.stream).value == 'with'
-            self.stream.skip()
-        elif self.stream.current.test('name:with'):
-            self.stream.skip()
-            node.with_expression = self.parse_expression()
-            if self.stream.current.test('name:only'):
-                node.with_context = False
-                self.stream.skip()
-            else:
-                node.with_context = True
-
-        elif self.stream.current.test('name:only'):
-            node.with_context = False
-            self.stream.skip()
-        else:
-            node.with_context = True
-        return node
-
-
 class BlendedCodeGenerator(jinja2.compiler.CodeGenerator):
     """
     This subclass does a couple of things: it helps standardize all numbers in Jinja
     as floats, but with the feature that trailing zeroes are not printed; it also adds
     functionality to the include tag.
 
     What is added to include is the ability to pass specific arguments into the tag.
 
     .. sourcecode:: jinja
 
         {% include "included_file.html" with { "arg1": strval, "arg2": numval } %}
     """
 
-    def pull_locals(self, frame):
-        """
-        """
-        for name in frame.identifiers.undeclared:
-            self.writeline('l_%s = environment._trimfloat(context.resolve(%r))' % (name, name))
 
     def visit_Const(self, node, frame):
         """
         """
-        val = node.value
+        # val = node.value
+        val = node.as_const(frame.eval_ctx)
         if isinstance(val, Number):
             self.write('environment._trimfloat(' + str(val) + ')')
         else:
             self.write(repr(val))
-
+    
+    
     def visit_Filter(self, node, frame):
         """
         """
         self.write('environment._trimfloat(')
         super(BlendedCodeGenerator, self).visit_Filter(node, frame)
         self.write(')')
 
+
     def visit_Include(self, node, frame):
         """
         Handles includes. Overrides base functionality to add new Include node functionality
         """
-        if node.with_context:
-            self.unoptimize_scope(frame)
+        
         if node.ignore_missing:
             self.writeline('try:')
             self.indent()
 
         func_name = 'get_or_select_template'
         if isinstance(node.template, nodes.Const):
             if isinstance(node.template.value, string_types):
@@ -678,32 +681,127 @@
             self.outdent()
             self.writeline('except TemplateNotFound:')
             self.indent()
             self.writeline('pass')
             self.outdent()
             self.writeline('else:')
             self.indent()
-
+        
+        skip_event_yield = False
         if node.with_expression:
+            # breakpoint()
             self.writeline('args = dict(')
             self.visit(node.with_expression, frame)
             self.write(')')
-
+            
             if node.with_context:
                 self.writeline('vars = dict(context.parent)')
                 self.writeline('ctxt = template.new_context(vars, True, locals(), args)')
             else:
                 self.writeline('ctxt = template.new_context(args, True)')
             self.writeline('for event in template.root_render_func(ctxt):')
         else:
+            
             if node.with_context:
-                self.writeline('ctxt = template.new_context(context.parent, True, locals())')
-                self.writeline('for event in template.root_render_func(ctxt):')
+                self.writeline(
+                f"{self.choose_async()}for event in template.root_render_func("
+                "template.new_context(context.get_all(), True,"
+                f" {self.dump_local_context(frame)})):"
+            )
+            
+            elif self.environment.is_async:
+                self.writeline(
+                    "for event in (await template._get_default_module_async())"
+                    "._body_stream:"
+                )
             else:
-                self.writeline('for event in template.module._body_stream:')
-
-        self.indent()
-        self.simple_write('event', frame)
-        self.outdent()
+                self.writeline("yield from template._get_default_module()._body_stream")
+                skip_event_yield = True
+                
+        if not skip_event_yield:
+            self.indent()
+            self.simple_write("event", frame)
+            self.outdent()
 
         if node.ignore_missing:
             self.outdent()
+    
+
+# NativeEnvironment for Blended
+'''
+The default Environment renders templates to strings. 
+With NativeEnvironment, rendering a template produces a native Python type.
+====
+env = NativeEnvironment()
+env_t = env.from_string('{{ x + y }}')
+result = env_t.render(x=4, y=2)
+print(result)     ---> 6
+print(type(result))   ---> int      [ if we don't use NativeEnvironment then type is 'str' ]
+
+'''
+from jinja2.nativetypes import native_concat, NativeCodeGenerator, NativeTemplate, NativeEnvironment
+from jinja2.compiler import has_safe_repr
+import typing as t
+
+class Blended_NativeCodeGenerator(BlendedCodeGenerator):
+    @staticmethod
+    def _default_finalize(value):
+        return value
+
+    def _output_const_repr(self, group) -> str:
+        return repr("".join([str(v) for v in group]))
+
+    def _output_child_to_const(
+        self, node: nodes.Expr, frame, finalize: BlendedCodeGenerator._FinalizeInfo
+    ):
+        const = node.as_const(frame.eval_ctx)
+
+        if not has_safe_repr(const):
+            raise nodes.Impossible()
+
+        if isinstance(node, nodes.TemplateData):
+            return const
+
+        return finalize.const(const)  # type: ignore
+
+    def _output_child_pre(
+        self, node: nodes.Expr, frame, finalize: BlendedCodeGenerator._FinalizeInfo
+    ) -> None:
+        if finalize.src is not None:
+            self.write(finalize.src)
+
+    def _output_child_post(
+        self, node: nodes.Expr, frame, finalize: BlendedCodeGenerator._FinalizeInfo
+    ) -> None:
+        if finalize.src is not None:
+            self.write(")")
+
+class Blended_NativeEnvironment(BlendedEnvironment):
+    
+    code_generator_class = Blended_NativeCodeGenerator
+    concat = staticmethod(native_concat)
+    
+
+
+class Blended_NativeTemplate(BlendedTemplate):
+    environment_class = Blended_NativeEnvironment
+    def render(self, *args, **kwargs):
+        """Render the template to produce a native Python type. If the
+        result is a single node, its value is returned. Otherwise, the
+        nodes are concatenated as strings. If the result can be parsed
+        with :func:`ast.literal_eval`, the parsed value is returned.
+        Otherwise, the string is returned.
+        """
+        ctx = self.new_context(dict(*args, **kwargs))
+
+        try:
+            # temp = self.environment_class.concat(self.root_render_func(ctx))
+            # if temp not in [False, True]:
+            return self.environment_class.concat(  # type: ignore
+                self.root_render_func(ctx)  # type: ignore
+            ) 
+        except Exception:
+            return self.environment.handle_exception()
+
+Blended_NativeEnvironment.template_class = Blended_NativeTemplate
+
+
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/blendedParserListener.py` & `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParserListener.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py2/blendedLexer.py` & `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py2/blendedParser.py` & `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py3/blendedLexer.py` & `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/blended_grammar/py3/blendedParser.py` & `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/lint.py` & `blendedUx_Lang-1.1.0/blended/lint/lint.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from antlr4.tree.Trees import Trees
 
 from antlr4.error.ErrorListener import ErrorListener
 
 is_py3k = sys.version_info[0] > 2
 
 if is_py3k:
-    from blendedUxLang.blended.lint.blended_grammar.py3.blendedLexer import blendedLexer
-    from blendedUxLang.blended.lint.blended_grammar.py3.blendedParser import blendedParser
+    from blended.lint.blended_grammar.py3.blendedLexer import blendedLexer
+    from blended.lint.blended_grammar.py3.blendedParser import blendedParser
 else:
-    from blendedUxLang.blended.lint.blended_grammar.py2.blendedLexer import blendedLexer
-    from blendedUxLang.blended.lint.blended_grammar.py2.blendedParser import blendedParser
+    from blended.lint.blended_grammar.py2.blendedLexer import blendedLexer
+    from blended.lint.blended_grammar.py2.blendedParser import blendedParser
 
 
-from blendedUxLang.blended.lint.listeners import BlendedErrorListener
+from blended.lint.listeners import BlendedErrorListener
     
 def lint(input):
     error_listener = BlendedErrorListener() 
 
     lexer = blendedLexer(input)
     lexer.removeErrorListeners()
     lexer.addErrorListener(error_listener)
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/lint/lintcommands.py` & `blendedUx_Lang-1.1.0/blended/lint/lintcommands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import click
 
 from antlr4 import FileStream
 
-from blendedUxLang.blended.lint.lint import lint
+from blended.lint.lint import lint
 
 @click.command()
 @click.argument('filename', nargs=-1)
 def blended_lint(filename):
     
     working_directory = os.getcwd()
     errors = {}
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/sets.py` & `blendedUx_Lang-1.1.0/blended/sets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 import json
 import sys
 import functools
 import collections
-
-from jinja2._compat import imap
+from collections.abc import MutableSet
+# from collections.abc import MutableMapping
 
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
 PY34 = sys.version_info[0:2] >= (3, 4)
 
-class OrderedSet(collections.MutableSet):
+class OrderedSet(MutableSet):
     """
     Order set class to created a Ordered set list.
     """
 
     def __init__(self, iterable=None):
         """
         initialization of OrderSet
@@ -151,56 +151,61 @@
     Returns cartisan product of two lists.
     """
     result = [[x, y]  for x in list1 for y in list2]
     if PY2:
         cartisan_product_list = _byteify(result)
     elif PY3 or PY34:
         cartisan_product_list = result
-    cartisan_product_result_list = list(imap(functools.partial(
+    cartisan_product_result_list = list(map(functools.partial(
         json.dumps, sort_keys=True), cartisan_product_list))
     cartisan_product_set = set(cartisan_product_result_list)
     if PY3 or PY34:
-        cartisan_product_result = list(imap(functools.partial(
-            json.loads, encoding="utf-8"), cartisan_product_set))
+        # cartisan_product_result = list(map(functools.partial(
+        #     json.loads, encoding="utf-8"), cartisan_product_set))
+        cartisan_product_result = list(map(json.loads, cartisan_product_set))
     elif PY2:
-        cartisan_product_result = list(imap(json_loads_byteified, cartisan_product_set))
+        cartisan_product_result = list(map(json_loads_byteified, cartisan_product_set))
     return cartisan_product_result
 
 def mapped_list(list1, list2):
     """
     Returns list mapped in json string.
     """
-    mapped_list1 = list(imap(functools.partial(json.dumps, sort_keys=True), list1))
-    mapped_list2 = list(imap(functools.partial(json.dumps, sort_keys=True), list2))
+    mapped_list1 = list(map(functools.partial(json.dumps, sort_keys=True), list1))
+    mapped_list2 = list(map(functools.partial(json.dumps, sort_keys=True), list2))
     return mapped_list1, mapped_list2
 
 def result_set(set_obj):
     """
     Take set object as argument and return a list object for the given set
     """
+    # breakpoint()
+    # a = map(functools.partial(json.loads, encoding="utf-8"), set_obj)
+
     if PY3 or PY34:
-        result = list(imap(functools.partial(json.loads, encoding="utf-8"), set_obj))
+        result = list(map(json.loads, set_obj))
     elif PY2:
-        result = list(imap(json_loads_byteified, set_obj))
+        result = list(map(json_loads_byteified, set_obj))
     return result
+    
 
 def json_loads_byteified(json_text):
     """
     returns byteified of the give data in json representation of data
     """
     return _byteify(
         json.loads(json_text, object_hook=_byteify),
         ignore_dicts=True)
 
 def _byteify(data, ignore_dicts=False):
     """
     byteify the unicode in python2.
     """
     # if this is a unicode string, return its string representation
-    if isinstance(data, unicode):
+    if isinstance(data, str):
         return data.encode('utf-8')
     # if this is a list of values, return list of byteified values
     if isinstance(data, list):
         return [_byteify(item, ignore_dicts=False) for item in data]
     # if this is a dictionary, return dictionary of byteified keys and values
     # but only if we haven't already byteified it
     if isinstance(data, dict) and not ignore_dicts:
```

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/settings.py` & `blendedUx_Lang-1.1.0/blended/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/testapp/testapp/urls.py` & `blendedUx_Lang-1.1.0/blended/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.0.0/blendedUxLang/blended/trimfloat.py` & `blendedUx_Lang-1.1.0/blended/trimfloat.py`

 * *Files identical despite different names*

