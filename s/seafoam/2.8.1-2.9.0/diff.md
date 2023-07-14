# Comparing `tmp/seafoam-2.8.1.tar.gz` & `tmp/seafoam-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seafoam-2.8.1.tar", last modified: Mon Jun 12 00:16:10 2023, max compression
+gzip compressed data, was "seafoam-2.9.0.tar", last modified: Fri Jul 14 18:15:21 2023, max compression
```

## Comparing `seafoam-2.8.1.tar` & `seafoam-2.9.0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.708976 seafoam-2.8.1/
--rw-rw-rw-   0        0        0     1133 2021-06-29 04:21:34.000000 seafoam-2.8.1/LICENSE.txt
--rw-rw-rw-   0        0        0      180 2021-07-05 16:41:31.000000 seafoam-2.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0    30291 2023-06-12 00:16:10.709977 seafoam-2.8.1/PKG-INFO
--rw-rw-rw-   0        0        0    28868 2023-06-11 23:27:14.000000 seafoam-2.8.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.445990 seafoam-2.8.1/docs/
--rw-rw-rw-   0        0        0     9539 2023-06-11 23:49:16.000000 seafoam-2.8.1/docs/CHANGELOG.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.382944 seafoam-2.8.1/pelican/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.383946 seafoam-2.8.1/pelican/plugins/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.454987 seafoam-2.8.1/pelican/plugins/seafoam/
--rw-rw-rw-   0        0        0      829 2021-07-05 17:37:19.000000 seafoam-2.8.1/pelican/plugins/seafoam/__init__.py
--rw-rw-rw-   0        0        0      502 2023-06-12 00:16:05.000000 seafoam-2.8.1/pelican/plugins/seafoam/constants.py
--rw-rw-rw-   0        0        0     1005 2021-07-05 02:52:25.000000 seafoam-2.8.1/pelican/plugins/seafoam/formatting.py
--rw-rw-rw-   0        0        0     7606 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/initialize.py
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.388948 seafoam-2.8.1/pelican/plugins/seafoam/static/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.458984 seafoam-2.8.1/pelican/plugins/seafoam/static/css/
--rw-rw-rw-   0        0        0   236390 2023-06-11 23:48:08.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
--rw-rw-rw-   0        0        0   235993 2023-06-11 23:48:09.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.479979 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/
--rw-rw-rw-   0        0        0   134808 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.520980 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/
--rw-rw-rw-   0        0        0     2104 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
--rw-rw-rw-   0        0        0     4460 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
--rw-rw-rw-   0        0        0    18413 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
--rw-rw-rw-   0        0        0    50449 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
--rw-rw-rw-   0        0        0    35472 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    19444 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
--rw-rw-rw-   0        0        0    15168 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    19294 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0    56250 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    35176 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    20280 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    15856 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    19408 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
--rw-rw-rw-   0        0        0    56028 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    35356 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    20416 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    16020 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    18842 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
--rw-rw-rw-   0        0        0    50436 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    35700 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    19916 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    15476 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.555978 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/
--rw-rw-rw-   0        0        0    24884 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
--rw-rw-rw-   0        0        0   128830 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
--rw-rw-rw-   0        0        0    49124 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    25788 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
--rw-rw-rw-   0        0        0    21932 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    25468 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0   128299 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    47480 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    26508 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    22480 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    23567 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
--rw-rw-rw-   0        0        0   127687 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    47032 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    24808 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    21020 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    23239 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
--rw-rw-rw-   0        0        0   128551 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    48900 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    24304 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    20512 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.565976 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/
--rw-rw-rw-   0        0        0     4499 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
--rw-rw-rw-   0        0        0    11207 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
--rw-rw-rw-   0        0        0    60057 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
--rw-rw-rw-   0        0        0    18564 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
--rw-rw-rw-   0        0        0    13008 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
--rw-rw-rw-   0        0        0    10084 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
--rw-rw-rw-   0        0        0   165742 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0    20127 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   109025 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.574980 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/
--rw-rw-rw-   0        0        0    30028 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
--rw-rw-rw-   0        0        0    81305 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
--rw-rw-rw-   0        0        0    78804 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
--rw-rw-rw-   0        0        0    36788 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
--rw-rw-rw-   0        0        0    30116 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.587981 seafoam-2.8.1/pelican/plugins/seafoam/static/js/
--rw-rw-rw-   0        0        0    72084 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.js
--rw-rw-rw-   0        0        0    37051 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     2512 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/comments.js
--rw-rw-rw-   0        0        0     1520 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/github.js
--rw-rw-rw-   0        0        0     2558 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/jXHR.js
--rw-rw-rw-   0        0        0    86713 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/jquery.min.js
--rw-rw-rw-   0        0        0     4381 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/js/respond.min.js
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.595982 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.596979 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/img/
--rw-rw-rw-   0        0        0      368 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/img/search.png
--rw-rw-rw-   0        0        0     5734 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
--rw-rw-rw-   0        0        0    33779 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
--rw-rw-rw-   0        0        0    10697 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
--rw-rw-rw-   0        0        0     4537 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
--rw-rw-rw-   0        0        0     3670 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.621976 seafoam-2.8.1/pelican/plugins/seafoam/templates/
--rw-rw-rw-   0        0        0     1110 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/404.html
--rw-rw-rw-   0        0        0     5399 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/archives.html
--rw-rw-rw-   0        0        0     4597 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/article.html
--rw-rw-rw-   0        0        0     1508 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/article_list.html
--rw-rw-rw-   0        0        0      761 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/author.html
--rw-rw-rw-   0        0        0      857 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/authors.html
--rw-rw-rw-   0        0        0    14081 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/base.html
--rw-rw-rw-   0        0        0     2053 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/categories.html
--rw-rw-rw-   0        0        0      738 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/category.html
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.664984 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/
--rw-rw-rw-   0        0        0      196 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/aboutme.html
--rw-rw-rw-   0        0        0      618 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/addthis.html
--rw-rw-rw-   0        0        0     1481 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_info.html
--rw-rw-rw-   0        0        0     2665 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_listing.html
--rw-rw-rw-   0        0        0      978 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/assets-css.html
--rw-rw-rw-   0        0        0      219 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/assets-js.html
--rw-rw-rw-   0        0        0     4405 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/cc-license.html
--rw-rw-rw-   0        0        0      553 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comment_count.html
--rw-rw-rw-   0        0        0     1291 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments-js.html
--rw-rw-rw-   0        0        0     5874 2022-04-30 21:08:37.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments.html
--rw-rw-rw-   0        0        0      741 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/disqus_script.html
--rw-rw-rw-   0        0        0     3364 2021-06-29 04:36:51.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/footer.html
--rw-rw-rw-   0        0        0     1818 2023-06-11 23:27:14.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/ga.html
--rw-rw-rw-   0        0        0     1308 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/github-js.html
--rw-rw-rw-   0        0        0      442 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/github.html
--rw-rw-rw-   0        0        0      434 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/links.html
--rw-rw-rw-   0        0        0     1991 2022-03-21 04:06:10.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/neighbors.html
--rw-rw-rw-   0        0        0     2955 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/pagination.html
--rw-rw-rw-   0        0        0      872 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/piwik.html
--rw-rw-rw-   0        0        0      486 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/prjct.html
--rw-rw-rw-   0        0        0      357 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/related-posts.html
--rw-rw-rw-   0        0        0     3520 2021-10-24 02:08:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/sidebar.html
--rw-rw-rw-   0        0        0      276 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/taglist.html
--rw-rw-rw-   0        0        0      296 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/translations.html
--rw-rw-rw-   0        0        0      703 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
--rw-rw-rw-   0        0        0      808 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/index.html
--rw-rw-rw-   0        0        0     2473 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/page.html
--rw-rw-rw-   0        0        0     7104 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/period_archives.html
--rw-rw-rw-   0        0        0     4517 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/prjct.html
--rw-rw-rw-   0        0        0     1507 2021-06-27 05:13:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.667984 seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/
--rw-rw-rw-   0        0        0     8939 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
--rw-rw-rw-   0        0        0     5443 2023-06-10 17:35:59.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/pricing.html
--rw-rw-rw-   0        0        0      795 2021-10-24 02:08:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/tag.html
--rw-rw-rw-   0        0        0     2036 2021-10-24 02:08:02.000000 seafoam-2.8.1/pelican/plugins/seafoam/templates/tags.html
--rw-rw-rw-   0        0        0      429 2022-03-21 04:06:10.000000 seafoam-2.8.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-12 00:16:10.706979 seafoam-2.8.1/seafoam.egg-info/
--rw-rw-rw-   0        0        0    30291 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8286 2023-06-12 00:16:10.000000 seafoam-2.8.1/seafoam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-06-12 00:16:09.000000 seafoam-2.8.1/seafoam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-06-12 00:16:10.716977 seafoam-2.8.1/setup.cfg
--rw-rw-rw-   0        0        0     4767 2023-06-10 17:35:59.000000 seafoam-2.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.965345 seafoam-2.9.0/
+-rw-rw-rw-   0        0        0     1133 2023-07-11 04:35:00.000000 seafoam-2.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      180 2023-07-11 04:35:00.000000 seafoam-2.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    30907 2023-07-14 18:15:21.965345 seafoam-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    29488 2023-07-14 18:03:53.000000 seafoam-2.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.087271 seafoam-2.9.0/docs/
+-rw-rw-rw-   0        0        0    10154 2023-07-14 18:13:02.000000 seafoam-2.9.0/docs/CHANGELOG.rst
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.076732 seafoam-2.9.0/pelican/
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.076732 seafoam-2.9.0/pelican/plugins/
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.087271 seafoam-2.9.0/pelican/plugins/seafoam/
+-rw-rw-rw-   0        0        0      829 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-14 18:15:10.000000 seafoam-2.9.0/pelican/plugins/seafoam/constants.py
+-rw-rw-rw-   0        0        0     1005 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/formatting.py
+-rw-rw-rw-   0        0        0     7606 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/initialize.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.076732 seafoam-2.9.0/pelican/plugins/seafoam/static/
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.107939 seafoam-2.9.0/pelican/plugins/seafoam/static/css/
+-rw-rw-rw-   0        0        0   236433 2023-07-12 04:11:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
+-rw-rw-rw-   0        0        0   236036 2023-07-12 04:11:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.169936 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.295853 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/
+-rw-rw-rw-   0        0        0     2104 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
+-rw-rw-rw-   0        0        0     4460 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
+-rw-rw-rw-   0        0        0    18413 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
+-rw-rw-rw-   0        0        0    50449 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    35472 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    19444 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    15168 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    19294 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0    56250 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    35176 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    20280 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    15856 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    19408 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0    56028 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    35356 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    20416 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    16020 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    18842 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0    50436 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    35700 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    19916 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    15476 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.420648 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/
+-rw-rw-rw-   0        0        0    24884 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
+-rw-rw-rw-   0        0        0   128830 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    49124 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    25788 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    21932 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    25468 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0   128299 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    47480 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    26508 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    22480 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    23567 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0   127687 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    47032 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    24808 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    21020 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    23239 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0   128551 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    48900 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    24304 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    20512 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.451440 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/
+-rw-rw-rw-   0        0        0     4499 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
+-rw-rw-rw-   0        0        0    11207 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
+-rw-rw-rw-   0        0        0    60057 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
+-rw-rw-rw-   0        0        0    18564 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
+-rw-rw-rw-   0        0        0    13008 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
+-rw-rw-rw-   0        0        0    10084 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
+-rw-rw-rw-   0        0        0   165742 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0    20127 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   109025 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.482697 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/
+-rw-rw-rw-   0        0        0    30028 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
+-rw-rw-rw-   0        0        0    81305 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
+-rw-rw-rw-   0        0        0    78804 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
+-rw-rw-rw-   0        0        0    36788 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
+-rw-rw-rw-   0        0        0    30116 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.597449 seafoam-2.9.0/pelican/plugins/seafoam/static/js/
+-rw-rw-rw-   0        0        0    72084 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.js
+-rw-rw-rw-   0        0        0    37051 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     2512 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/comments.js
+-rw-rw-rw-   0        0        0     1520 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/github.js
+-rw-rw-rw-   0        0        0     2558 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/jXHR.js
+-rw-rw-rw-   0        0        0    86713 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/jquery.min.js
+-rw-rw-rw-   0        0        0     4381 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/respond.min.js
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.649899 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.660435 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/img/
+-rw-rw-rw-   0        0        0      368 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/img/search.png
+-rw-rw-rw-   0        0        0     5734 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
+-rw-rw-rw-   0        0        0    33779 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
+-rw-rw-rw-   0        0        0    10697 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
+-rw-rw-rw-   0        0        0     4537 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
+-rw-rw-rw-   0        0        0     3670 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.744268 seafoam-2.9.0/pelican/plugins/seafoam/templates/
+-rw-rw-rw-   0        0        0     1110 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/404.html
+-rw-rw-rw-   0        0        0     5875 2023-07-12 01:08:09.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/archives.html
+-rw-rw-rw-   0        0        0     4657 2023-07-13 02:13:40.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/article.html
+-rw-rw-rw-   0        0        0     1551 2023-07-12 03:05:35.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/article_list.html
+-rw-rw-rw-   0        0        0      761 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/author.html
+-rw-rw-rw-   0        0        0      857 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/authors.html
+-rw-rw-rw-   0        0        0    15825 2023-07-13 02:15:55.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/base.html
+-rw-rw-rw-   0        0        0     2053 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/categories.html
+-rw-rw-rw-   0        0        0      738 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/category.html
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.923061 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/
+-rw-rw-rw-   0        0        0      196 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/aboutme.html
+-rw-rw-rw-   0        0        0      618 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/addthis.html
+-rw-rw-rw-   0        0        0     1481 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_info.html
+-rw-rw-rw-   0        0        0     3389 2023-07-12 04:29:59.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_listing.html
+-rw-rw-rw-   0        0        0      978 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/assets-css.html
+-rw-rw-rw-   0        0        0      219 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/assets-js.html
+-rw-rw-rw-   0        0        0     4405 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/cc-license.html
+-rw-rw-rw-   0        0        0      553 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comment_count.html
+-rw-rw-rw-   0        0        0     1291 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comments-js.html
+-rw-rw-rw-   0        0        0     5874 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comments.html
+-rw-rw-rw-   0        0        0      741 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/disqus_script.html
+-rw-rw-rw-   0        0        0     3869 2023-07-12 00:31:05.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/footer.html
+-rw-rw-rw-   0        0        0     1818 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/ga.html
+-rw-rw-rw-   0        0        0     1308 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/github-js.html
+-rw-rw-rw-   0        0        0      442 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/github.html
+-rw-rw-rw-   0        0        0      434 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/links.html
+-rw-rw-rw-   0        0        0     1991 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/neighbors.html
+-rw-rw-rw-   0        0        0     2955 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/pagination.html
+-rw-rw-rw-   0        0        0      872 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/piwik.html
+-rw-rw-rw-   0        0        0      486 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/prjct.html
+-rw-rw-rw-   0        0        0      357 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/related-posts.html
+-rw-rw-rw-   0        0        0     3520 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/sidebar.html
+-rw-rw-rw-   0        0        0      276 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/taglist.html
+-rw-rw-rw-   0        0        0      296 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/translations.html
+-rw-rw-rw-   0        0        0      703 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
+-rw-rw-rw-   0        0        0      796 2023-07-12 03:06:56.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/index.html
+-rw-rw-rw-   0        0        0     2474 2023-07-13 02:04:28.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/page.html
+-rw-rw-rw-   0        0        0     7104 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/period_archives.html
+-rw-rw-rw-   0        0        0     4517 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/prjct.html
+-rw-rw-rw-   0        0        0     1507 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.933608 seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/
+-rw-rw-rw-   0        0        0     8939 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
+-rw-rw-rw-   0        0        0     5443 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/pricing.html
+-rw-rw-rw-   0        0        0      795 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/tag.html
+-rw-rw-rw-   0        0        0     2036 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/tags.html
+-rw-rw-rw-   0        0        0      429 2023-07-11 04:35:00.000000 seafoam-2.9.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.965345 seafoam-2.9.0/seafoam.egg-info/
+-rw-rw-rw-   0        0        0    30907 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8286 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-14 18:15:21.965345 seafoam-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     4767 2023-07-11 04:35:00.000000 seafoam-2.9.0/setup.py
```

### Comparing `seafoam-2.8.1/LICENSE.txt` & `seafoam-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/PKG-INFO` & `seafoam-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.8.1
+Version: 2.9.0
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
@@ -113,18 +113,18 @@
 You may also need to configure the theme through the use of additional settings
 (see below).
 
 
 Requirements
 ------------
 
-``Seafoam`` requires Pelican, the ``image_process`` plugin, the ``jinja
-filters`` plugin, ``beautifulsoup4``, and ``semantic_version``. If the theme is
-installed from pip, these should be automatically installed. If needed, they
-can be manually installed with pip:
+``Seafoam`` requires Pelican, the ``image_process`` plugin, the
+``jinja filters`` plugin, ``beautifulsoup4``, and ``semantic_version``. If the
+theme is installed from pip, these should be automatically installed. If
+needed, they can be manually installed with pip:
 
 .. code-block:: sh
 
    pip install pelican
    pip install pelican-image-process
    pip install pelican-jinja-filters
    pip install beautifulsoup4
@@ -133,34 +133,37 @@
 
 Supported Plugins
 -----------------
 
 Seafoam also works with several other plugins for Pelican, but none of those
 listed in this section are required.
 
+- `microblogging <https://blog.minchin.ca/label/microblogging-pelican/>`_ --
+  adds the ability to have "microposts", and tweaks the formatting of the theme
+  based on their (assumed) shorter length.
 - `readtime <https://pypi.python.org/pypi/pelican-readtime>`_ -- provides
   estimated reading time for articles. Available from PyPI as
   ``pelican-readtime``.
 - `post-stats
   <https://github.com/getpelican/pelican-plugins/tree/master/post_stats>`_ --
-  provides estimated reading time for articles if `readtime` is not available.
+  provides estimated reading time for articles if ``readtime`` is not available.
   Available in the `Pelican Plugins collection
   <https://github.com/getpelican/pelican-plugins/>`_.
 - `neighbors <https://pypi.python.org/pypi/pelican-neighbors>`_ -- provides
   post-article links to the next and previous article on your blog and the
   next and previous article in that category. Available on PyPI as
   ``pelican-neighours``.
 - `static-comments <https://blog.minchin.ca/label/static-comments/>`_ (or the
   older `pelican_comment_system
   <https://bernhard.scheirle.de/posts/2014/March/29/static-comments-via-email/>`_)
   -- add static comments to your blog. Available on PyPI as
   ``minchin.pelican.plugins.static-comments``.
 - `Related Posts
   <https://github.com/getpelican/pelican-plugins/tree/master/related_posts>`_ --
-  adds the related_posts variable to the article's context.
+  adds the ``related_posts`` variable to the article's context.
 - Tipue Search
 
 
 Additional Images
 -----------------
 
 Article with header image
@@ -207,14 +210,18 @@
 
 404 Error Page
 
 .. image:: https://github.com/MinchinWeb/seafoam/raw/master/docs/screenshots/2.6.0/404.png
     :align: center
     :alt: 404 Error
 
+.. add microblog post image
+
+.. add Strathcona theme image
+
 
 Additional Settings
 -------------------
 
 These settings can be set in your ``pelicanconf.py`` file (your Pelican settings
 file) to alter the behavior of the theme.
 
@@ -307,17 +314,19 @@
   You can show a short blurb of text about yourself and a picture. This setting
   is the path to the picture. See the ``ABOUT_ME`` setting to set the
   descriptive paragraph.
 BOOTSTRAP_NAVBAR_INVERSE = False
   Apply inverse CSS setting to Navbar. Changing this will swap the top
   navigation bar between light and dark.
 BOOTSTRAP_THEME = "seafoam"
-  Valid values are ``seafoam`` and ``strathcona``. Automatically set to
-  ``seafoam`` by the internal plugin if unspecified. Other values (including
-  leaving this unset) are not expected to work correctly.
+  Use this to set the "colour scheme" of the framework. Valid values are
+  ``seafoam`` and ``strathcona``. ``seafoam`` teal on darker green;
+  ``strathcona`` is maroon on white. This is a Automatically set to ``seafoam``
+  by the internal plugin if unspecified. Other values (including leaving this
+  unset) are not expected to work correctly.
 CATEGORIES_URL
   Same as the regular Pelican setting.
 CATEGORY_IMAGES = {}
   Provide a default featured image by category. If an image is set in the
   article metadata, that will override this.
 
   Provide a dictionary where the key is the category name and the value is the
@@ -500,14 +509,19 @@
   When set and Breadcrumbs are enabled, all items on the site are shown to be
   under both "home" (linked to at the ``SITE_ROOT_URL``) and ``MENUITEMS_2_AT``
   (linked to at ``MENUITEMS_2_AT_LINK``).
 MENUITEMS_2_AT_LINK
   When set and Breadcrumbs are enabled, all items on the site are shown to be
   under both "home" (linked to at the ``SITE_ROOT_URL``) and ``MENUITEMS_2_AT``
   (linked to at ``MENUITEMS_2_AT_LINK``).
+MICROBLOG_DEV_URL
+  The project url for the microblogging plugin. Provided by the plugin, when in
+  use.
+MICROBLOG_VERSION
+  The version of the microblogging plugin. Provided by the plugin, when in use.
 NAVBAR_ON_TOP = False
   If True, the navigation menu is on top. If False, the navigation menu is
   vertical on the left side of the page. Default is False.
 NEIGHBORS
   Activates the links to the next and previous articles, both in the "all
   posts" index and the category-specific index. Requires the
   `neighbors <https://pypi.python.org/pypi/pelican-neighbors>`_ to be both
@@ -720,9 +734,7 @@
 -------
 
 Original theme developed by `Daan Debie <http://dandydev.net/>`_.
 
 The idea that a theme could be installed as a Python package by `Jeff
 Forcier <http://bitprophet.org/>`_'s `Alabaster theme
 <https://github.com/bitprophet/alabaster>`_ for Sphinx.
-
-
```

### Comparing `seafoam-2.8.1/README.rst` & `seafoam-2.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -77,18 +77,18 @@
 You may also need to configure the theme through the use of additional settings
 (see below).
 
 
 Requirements
 ------------
 
-``Seafoam`` requires Pelican, the ``image_process`` plugin, the ``jinja
-filters`` plugin, ``beautifulsoup4``, and ``semantic_version``. If the theme is
-installed from pip, these should be automatically installed. If needed, they
-can be manually installed with pip:
+``Seafoam`` requires Pelican, the ``image_process`` plugin, the
+``jinja filters`` plugin, ``beautifulsoup4``, and ``semantic_version``. If the
+theme is installed from pip, these should be automatically installed. If
+needed, they can be manually installed with pip:
 
 .. code-block:: sh
 
    pip install pelican
    pip install pelican-image-process
    pip install pelican-jinja-filters
    pip install beautifulsoup4
@@ -97,34 +97,37 @@
 
 Supported Plugins
 -----------------
 
 Seafoam also works with several other plugins for Pelican, but none of those
 listed in this section are required.
 
+- `microblogging <https://blog.minchin.ca/label/microblogging-pelican/>`_ --
+  adds the ability to have "microposts", and tweaks the formatting of the theme
+  based on their (assumed) shorter length.
 - `readtime <https://pypi.python.org/pypi/pelican-readtime>`_ -- provides
   estimated reading time for articles. Available from PyPI as
   ``pelican-readtime``.
 - `post-stats
   <https://github.com/getpelican/pelican-plugins/tree/master/post_stats>`_ --
-  provides estimated reading time for articles if `readtime` is not available.
+  provides estimated reading time for articles if ``readtime`` is not available.
   Available in the `Pelican Plugins collection
   <https://github.com/getpelican/pelican-plugins/>`_.
 - `neighbors <https://pypi.python.org/pypi/pelican-neighbors>`_ -- provides
   post-article links to the next and previous article on your blog and the
   next and previous article in that category. Available on PyPI as
   ``pelican-neighours``.
 - `static-comments <https://blog.minchin.ca/label/static-comments/>`_ (or the
   older `pelican_comment_system
   <https://bernhard.scheirle.de/posts/2014/March/29/static-comments-via-email/>`_)
   -- add static comments to your blog. Available on PyPI as
   ``minchin.pelican.plugins.static-comments``.
 - `Related Posts
   <https://github.com/getpelican/pelican-plugins/tree/master/related_posts>`_ --
-  adds the related_posts variable to the article's context.
+  adds the ``related_posts`` variable to the article's context.
 - Tipue Search
 
 
 Additional Images
 -----------------
 
 Article with header image
@@ -171,14 +174,18 @@
 
 404 Error Page
 
 .. image:: https://github.com/MinchinWeb/seafoam/raw/master/docs/screenshots/2.6.0/404.png
     :align: center
     :alt: 404 Error
 
+.. add microblog post image
+
+.. add Strathcona theme image
+
 
 Additional Settings
 -------------------
 
 These settings can be set in your ``pelicanconf.py`` file (your Pelican settings
 file) to alter the behavior of the theme.
 
@@ -271,17 +278,19 @@
   You can show a short blurb of text about yourself and a picture. This setting
   is the path to the picture. See the ``ABOUT_ME`` setting to set the
   descriptive paragraph.
 BOOTSTRAP_NAVBAR_INVERSE = False
   Apply inverse CSS setting to Navbar. Changing this will swap the top
   navigation bar between light and dark.
 BOOTSTRAP_THEME = "seafoam"
-  Valid values are ``seafoam`` and ``strathcona``. Automatically set to
-  ``seafoam`` by the internal plugin if unspecified. Other values (including
-  leaving this unset) are not expected to work correctly.
+  Use this to set the "colour scheme" of the framework. Valid values are
+  ``seafoam`` and ``strathcona``. ``seafoam`` teal on darker green;
+  ``strathcona`` is maroon on white. This is a Automatically set to ``seafoam``
+  by the internal plugin if unspecified. Other values (including leaving this
+  unset) are not expected to work correctly.
 CATEGORIES_URL
   Same as the regular Pelican setting.
 CATEGORY_IMAGES = {}
   Provide a default featured image by category. If an image is set in the
   article metadata, that will override this.
 
   Provide a dictionary where the key is the category name and the value is the
@@ -464,14 +473,19 @@
   When set and Breadcrumbs are enabled, all items on the site are shown to be
   under both "home" (linked to at the ``SITE_ROOT_URL``) and ``MENUITEMS_2_AT``
   (linked to at ``MENUITEMS_2_AT_LINK``).
 MENUITEMS_2_AT_LINK
   When set and Breadcrumbs are enabled, all items on the site are shown to be
   under both "home" (linked to at the ``SITE_ROOT_URL``) and ``MENUITEMS_2_AT``
   (linked to at ``MENUITEMS_2_AT_LINK``).
+MICROBLOG_DEV_URL
+  The project url for the microblogging plugin. Provided by the plugin, when in
+  use.
+MICROBLOG_VERSION
+  The version of the microblogging plugin. Provided by the plugin, when in use.
 NAVBAR_ON_TOP = False
   If True, the navigation menu is on top. If False, the navigation menu is
   vertical on the left side of the page. Default is False.
 NEIGHBORS
   Activates the links to the next and previous articles, both in the "all
   posts" index and the category-specific index. Requires the
   `neighbors <https://pypi.python.org/pypi/pelican-neighbors>`_ to be both
```

### Comparing `seafoam-2.8.1/docs/CHANGELOG.rst` & `seafoam-2.9.0/docs/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Changelog
 =========
 
 .. Added, Changed, Depreciated, Removed, Fixed, Security
 
+- :release:`2.9.0 <2023-07-14>`
+- :feature:`-` add support for *microblogging*, through my `microblogging
+  plugin <https://blog.minchin.ca/label/microblogging-pelican/>`_.
+  c.f. `blog.minchin.ca Issue #105
+  <https://github.com/MinchinWeb/blog.minchin.ca/issues/105>`_.
+- :bug:`- major` no longer capitalize category names, when displayed on
+  sidebar. This is part of the changes to support microblogging.
+- :bug:`- major` review ``og`` meta tags, particularly for featured images.
+  c.f. `blog.minchin.ca Issue #104
+  <https://github.com/MinchinWeb/blog.minchin.ca/issues/104>`_.
 - :release:`2.8.1 <2023-06-11>`
 - :bug:`-` fix link to font files
 - :release:`2.8.0 <2023-06-11>`
 - :feature:`20` add support for Google Analytics v4. Use
   ``GOOGLE_ANALYTICS_V4``. The previous version of Google Analytics is being
-  deprecated, effective the end of June 2023.
+  deprecated (by Google), effective the end of June 2023.
 - :feature:`-` add ``DISPLAY_ARCHIVES_ON_MENU`` to control display of
   "Archives" link on navbar.
 - :feature:`-` add header image to pages (not just articles).
 - :feature:`-` add *strathcona* colour scheme/theme, and supporting fonts.
 - :bug:`- major` adjust supported Python versions to only include those
   currently supported upstream. Nothing has been removed that should keep older
   versions from working.
 - :bug:`16 major` upgrade version of self-hosted fonts.
 - :release:`2.7.1 <2022-04-30>`
 - :bug:`-` fix typo in comment form.
 - :support:`-` replace references to ``pelican-comment-system`` with the
   updated `Static Comments
   <https://blog.minchin.ca/2022/04/static-comments-211-released.html>`_ plugin.
-- :support:`-` bump to `minchin.releaser` 0.8.2, and thus officially support
+- :support:`-` bump to ``minchin.releaser`` 0.8.2, and thus officially support
   Python 3.10.
 - :release:`2.7.0 <2021-10-25>`
 - :bug:`- major` in ``SEAFOAM_DEV_MODE``, assume that the *Image Process*
   plugin might still be active (and so supply no-op transformations rather than
   no configuration).
 - :feature:`-` under "related posts", link to the category page, if applicable.
 - :feature:`-` add ``TAGS_TEXT`` to customize tag label.
@@ -173,10 +183,10 @@
 - :release:`1.1.0 <2016-09-12>`
 - :feature:`-` include (thumbnail of) featured image on article listing
 - :support:`-` start documentation with the changelog (this file)
 - :bug:`-` Better handling for copyright and modified dates in `footer.html`
 - :feature:`-` add breadcrumbs to main blog post listing page
 - :support:`-` add release machinery
 - :release:`1.0.0 <2016-08-15>`
-- :feature:`-` add 'setup.py', 'README.rst', 'CHANGELOG.rst'
+- :feature:`-` add ``setup.py``, ``README.rst``, ``CHANGELOG.rst``.
 - :support:`-` move package to 'minchin.pelican.themes.minchindotca'
 - :support:`-` pull code out of main Minchin.ca website repo
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/__init__.py` & `seafoam-2.9.0/pelican/plugins/seafoam/__init__.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/formatting.py` & `seafoam-2.9.0/pelican/plugins/seafoam/formatting.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/initialize.py` & `seafoam-2.9.0/pelican/plugins/seafoam/initialize.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css` & `seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -11574,14 +11574,17 @@
   background: #c8ccc2;
   color: #fdf6e3;
 }
 .grtable > tbody > tr:hover a:hover,
 .glist > tbody > tr:hover a:hover {
   color: #1a645f;
 }
+.featured-image {
+  margin-bottom: 25px;
+}
 .fake-list ul {
   padding-left: 0;
   list-style: none;
 }
 .gt-chart-name-link {
   border-bottom: none;
 }
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css` & `seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css`

 * *Files 0% similar despite different names*

```diff
@@ -11574,14 +11574,17 @@
   background: #b2b6bc;
   color: #222;
 }
 .grtable > tbody > tr:hover a:hover,
 .glist > tbody > tr:hover a:hover {
   color: #340000;
 }
+.featured-image {
+  margin-bottom: 34px;
+}
 .fake-list ul {
   padding-left: 0;
   list-style: none;
 }
 .gt-chart-name-link {
   border-bottom: none;
 }
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2` & `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/bootstrap.min.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/comments.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/comments.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/github.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/github.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/jXHR.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/jXHR.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/jquery.min.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/js/respond.min.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css` & `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js` & `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/404.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/404.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/archives.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/archives.html`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                     </div>
                     <div class="archives-spacer col-xs-12">&nbsp;</div>
                     <div class="archives-spacer col-xs-12">&nbsp;</div>
                 </div>
             {% endblock %}
 
             {# Main Archive Listing #}
+            {# "dates" is the article list, sorted by date #}
             {% for article in dates %}
                 <div class="row">
                     {% if (loop.index0 == 0) or (article.date.year != dates[loop.index0 - 1].date.year) %}
                         {% if loop.index0 != 0 -%}
                             <div class="archives-spacer col-xs-12">&nbsp;</div>
                             <div class="archives-spacer col-xs-12">&nbsp;</div>
                         {%- endif %}
@@ -87,15 +88,22 @@
                                     &mdash;
                         {% else -%}
                                     <a name="{{ article.date.year }}-{{ article.date.month }}-{{ article.date.day }}"></a>
                                     <time datetime="{{ article.date.isoformat() }}">{{ article.date | strftime('%a %-d') }}</time>
                         {%- endif -%}
                     </div>
                     <div class="archives-title col-xs-7 col-md-6">
-                        <a href="{{ SITEURL -}} / {{- article.url }}">{{ article.title }}</a>
-                        {% if article.subtitle %}<br />{{ article.subtitle }}{% endif %}
+                        {% if not article.micro %}
+                            <a href="{{ SITEURL -}} / {{- article.url }}">{{ article.title }}</a>
+                            {% if article.subtitle %}<br />{{ article.subtitle }}{% endif %}
+                        {% else %}
+                            {{ article.content }}
+                            {# &bull;&nbsp;<span class="label label-primary">
+                                <a href="{{ SITEURL -}} / {{- article.url }}"><i class="fa fa-link"></i></a>
+                            </span> #}
+                        {% endif %}
                     </div>
                 </div>
             {% endfor %}
         </div>
     </section>
 {% endblock %}
```

#### html2text {}

```diff
@@ -12,15 +12,16 @@
 dates[loop.index0 - 1].date.year) %} {% if loop.index0 != 0 %} • {% endif -%}
 %} "{{ SITEURL -}} / {{- article.date.year | datetime_from_period |
 merge_date_url (YEAR_ARCHIVE_URL) }}" {%- else -%} "#{{ article.date.year }}"
 {%- endif -%} > {{- article.date.year -}}
  {%- endif -%} {%- endfor %}
  
  
-{% endblock %} {# Main Archive Listing #} {% for article in dates %}
+{% endblock %} {# Main Archive Listing #} {# "dates" is the article list,
+sorted by date #} {% for article in dates %}
 {% if (loop.index0 == 0) or (article.date.year != dates[loop.index0 -
 1].date.year) %} {% if loop.index0 != 0 -%}
  
  
 {%- endif %}
  {{- article.date.year -}}
  
@@ -34,11 +35,12 @@
  {{- article.date | strftime('%B') -}}
  
 {% endif %}
 {%- if ((loop.index0 != 0) and (article.date.day == dates[loop.index0 -
 1].date.day) and (article.date.month == dates[loop.index0 - 1].date.month) and
 (article.date.year == dates[loop.index0 - 1].date.year)) %} — {% else -%}  {
 { article.date | strftime('%a %-d') }} {%- endif -%}
-{{_article.title_}} {% if article.subtitle %}
-{{ article.subtitle }}{% endif %}
+{% if not article.micro %} {{_article.title_}} {% if article.subtitle %}
+{{ article.subtitle }}{% endif %} {% else %} {{ article.content }} {# •    #}
+{% endif %}
 {% endfor %}
  {% endblock %}
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/article.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/article.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,24 @@
         <meta name="keywords" content="{{ article.tags|join(',')|striptags }}" />
     {% endif %}
     {% if article.summary %}
         <meta name="description" content="{{ article.summary|striptags|escape }}" />
     {% endif %}
 {% endblock %}
 
+{#
 {% block opengraph %}
     {% if OPEN_GRAPH_FB_APP_ID %}
         <meta property="fb:app_id" content="{{ OPEN_GRAPH_FB_APP_ID }}"/>
         <meta property="og:site_name" content="{{ SITENAME }}" />
         <meta property="og:type" content="article"/>
         <meta property="og:title" content="{{ article.title|striptags|escape|breaking_spaces }}"/>
         <meta property="og:url" content="{{ SITEURL -}} / {{- article.url }}"/>
         <meta property="og:description" content="{{ article.summary|striptags|escape }}"/>
-        <meta property="article:published_time" content="{{ article.date.strftime("%Y-%m-%d") }}" />
+        <meta property="article:published_time" content="{{ article.date.strftime('%Y-%m-%d') }}" />
         {% if article.category %}
             <meta property="article:section" content="{{ article.category }}" />
         {% endif %}
         {% for tag in article.tags %}
             <meta property="article:tag" content="{{ tag }}" />
         {% endfor %}
         {% if article.author %}
@@ -45,14 +46,15 @@
                   content="{{ SITEURL -}} / {{- article.og_image }}"/>
         {% elif OPEN_GRAPH_IMAGE %}
             <meta property="og:image"
                   content="{{ SITEURL -}} / {{- OPEN_GRAPH_IMAGE }}"/>
         {% endif %}
     {% endif %}
 {% endblock %}
+#}
 
 {% block canonical_rel %}
 <link rel="canonical" href="{{ SITEURL -}} / {{- article.url }}">
 {% endblock %}
 
 {% block breadcrumbs %}
     {% if DISPLAY_BREADCRUMBS %}
@@ -69,28 +71,30 @@
     {% endif %}
 {% endblock %}
 
 {% block content %}
     <section id="content">
         <article>
             {% if article.image %}
-                <img class="featured-image image-process-article-feature" src="{{ SITEURL -}} / {{- article.image|urlencode }}" alt="{{ article.title|striptags }}">
+                <img class="featured-image image-process-article-feature" src="{{ SITEURL -}} / {{- article.image|urlencode }}" alt="{{ article.title|striptags }}"/>
             {% elif CATEGORY_IMAGES and article.category in CATEGORY_IMAGES %}
-                <img class="featured-image image-process-article-feature" src="{{ SITEURL -}} / {{- CATEGORY_IMAGES[article.category]|urlencode }}"  alt="{{ article.category|striptags }}">              
+                <img class="featured-image image-process-article-feature" src="{{ SITEURL -}} / {{- CATEGORY_IMAGES[article.category]|urlencode }}" alt="{{ article.category|striptags }}"/>
             {% endif %}
 
+            {% if not article.micro %}
             <header class="entry-header">
                 <h1>
                     <a href="{{ SITEURL -}} / {{- article.url }}"
                        rel="bookmark"
                        title="Permalink to {{ article.title|striptags }}">
                         {{ article.title|replace('&nbsp;', ' ') }}
                     </a>
                 </h1>
             </header>
+            {% endif %}
             <div class="entry-content">
                 <div class="panel">
                     <div class="panel-body">
                         {% include "includes/article_info.html" %}
                     </div>
                 </div>
                 {{ article.content }}
```

#### html2text {}

```diff
@@ -1,37 +1,40 @@
 {% extends "base.html" %} {% block title -%} {
 { article.title|striptags|breaking_spaces }} — {{ super() }} {%- endblock %} {%
 block html_lang %}{{ article.lang }}{% endblock %} {% block meta %} {% if
 article.author %}
  {% else %}
  {% endif %} {% if article.tags %}
  {% endif %} {% if article.summary %}
- {% endif %} {% endblock %} {% block opengraph %} {% if OPEN_GRAPH_FB_APP_ID %}
+ {% endif %} {% endblock %} {# {% block opengraph %} {% if OPEN_GRAPH_FB_APP_ID
+%}
 
 
 
 
 
 
-Y-%m-%d") }}" /> {% if article.category %}
+ {% if article.category %}
  {% endif %} {% for tag in article.tags %}
  {% endfor %} {% if article.author %}
  {% elif AUTHOR %}
  {% endif %} {% if article.og_image %}
  {% elif OPEN_GRAPH_IMAGE %}
- {% endif %} {% endif %} {% endblock %} {% block canonical_rel %}
+ {% endif %} {% endif %} {% endblock %} #} {% block canonical_rel %}
  {% endblock %} {% block breadcrumbs %} {% if DISPLAY_BREADCRUMBS %}
    1. {% if MENUITEMS_2_AT %}
    2. {{_MENUITEMS_2_AT_}}
    3. {% endif %} {% if DISPLAY_CATEGORY_IN_BREADCRUMBS %}
    4. {{_article.category_}}
    5. {% endif %}
    6. {{ article.title | striptags }}
 {% endif %} {% endblock %} {% block content %}   {% if article.image %} [{
 { article.title|striptags }}] {% elif CATEGORY_IMAGES and article.category in
-CATEGORY_IMAGES %} [{{ article.category|striptags }}] {% endif %}
+CATEGORY_IMAGES %} [{{ article.category|striptags }}] {% endif %} {% if not
+article.micro %}
 ****** {{_article.title|replace(' ',_'_')_}} ******
+ {% endif %}
 {% include "includes/article_info.html" %}
 {{ article.content }}
  {% include 'includes/neighbors.html' %} {% include 'includes/related-
 posts.html' %} {% include 'includes/addthis.html' %} {% include 'includes/
 comments.html' %}   {% endblock %}
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/article_list.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/article_list.html`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,17 @@
           {% endif %}
             <li class="active">Articles</li>
         </ol>
     {% endif %}
 {% endblock %}
 
 {% block content %}
-    {% if articles %}
-        {% for article in (articles_page.object_list if articles_page else articles) %}
+    {# "dates" is the article list, sorted by date #}
+    {% if dates %}
+        {% for article in (dates_page.object_list if dates_page else dates) %}
             <article>
                 <h2><a href="{{ SITEURL -}} / {{- article.url }}">{{ article.title }}</a></h2>
                 {% if DISPLAY_ARTICLE_INFO_ON_INDEX %}
                     <div class="well well-sm">
                         {% include "includes/article_info.html" %}
                     </div>
                 {% endif %}
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 {% extends "base.html" %} {% block title -%} Articles — {{ super() }} {%-
 endblock %} {% block breadcrumbs %} {% if DISPLAY_BREADCRUMBS %}
    1. {% if MENUITEMS_2_AT %}
    2. {{_MENUITEMS_2_AT_}}
    3. {% endif %}
    4. Articles
-{% endif %} {% endblock %} {% block content %} {% if articles %} {% for article
-in (articles_page.object_list if articles_page else articles) %}
+{% endif %} {% endblock %} {% block content %} {# "dates" is the article list,
+sorted by date #} {% if dates %} {% for article in (dates_page.object_list if
+dates_page else dates) %}
 ***** {{_article.title_}} *****
 {% if DISPLAY_ARTICLE_INFO_ON_INDEX %}
 {% include "includes/article_info.html" %}
 {% endif %}
 {{ article.summary }} {% include 'includes/comment_count.html' %} more_...
 
 ===============================================================================
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/author.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/author.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/authors.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/authors.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/base.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/base.html`

 * *Files 11% similar despite different names*

```diff
@@ -30,33 +30,64 @@
     {# Open Graph tags #}
     {% if USE_OPEN_GRAPH is not defined %}
         {% set USE_OPEN_GRAPH = True %}
     {% endif %}
     {% if USE_OPEN_GRAPH %}
     <!-- Open Graph tags -->
         {% if OPEN_GRAPH_FB_APP_ID %}
-            <meta property="fb:app_id" content="{{ OPEN_GRAPH_FB_APP_ID }}"/>
+            <meta property="fb:app_id" content="{{ OPEN_GRAPH_FB_APP_ID }}" />
         {% endif %}
+            <meta property="og:site_name" content="{{ SITENAME }}" />
         {% if article %}
-            <meta property="og:type" content="article"/>
-            <meta property="og:title" content="{{ article.title|striptags|breaking_spaces }}"/>
-            <meta property="og:url" content="{{ SITEURL -}} / {{- article.url }}"/>
-            <meta property="og:description" content="{{ article.summary|striptags }}"/>
+            <meta property="og:type" content="article" />
+            <meta property="og:title" content="{{ article.title|striptags|breaking_spaces }}" />
+            <meta property="og:url" content="{{ SITEURL -}} / {{- article.url }}" />
+            <meta property="og:description" content="{{ article.summary|striptags|escape }}" />
+            <meta property="article:published_time" content="{{ article.date.strftime('%Y-%m-%d') }}" />
+            {% if article.category %}
+                <meta property="article:section" content="{{ article.category }}" />
+            {% endif %}
+            {% for tag in article.tags %}
+                <meta property="article:tag" content="{{ tag }}" />
+            {% endfor %}
+            {% if article.author %}
+                <meta property="article:author" content="{{ article.author }}" />
+            {% elif AUTHOR %}
+                <meta property="article:author" content="{{ AUTHOR }}" />
+            {% endif %}
+            {% if article.image %}
+                <meta property="og:image"
+                    content="{{ SITEURL -}} / {{- article.image|urlencode }}" />
+            {% elif article.og_image %}
+            <meta property="og:image"
+                    content="{{ SITEURL -}} / {{- article.og_image }}" />
+            {% elif CATEGORY_IMAGES and article.category in CATEGORY_IMAGES %}
+                <meta property="og:image"
+                    content="{{ SITEURL -}} / {{- CATEGORY_IMAGES[article.category]|urlencode }}" />
+            {% elif OPEN_GRAPH_IMAGE %}
+                <meta property="og:image" content="{{ SITEURL -}} / {{- OPEN_GRAPH_IMAGE }}" />
+            {% endif %}
         {% elif page %}
             <meta property="og:type" content="article"/>
-            <meta property="og:title" content="{{ page.title|striptags|breaking_spaces }}"/>
-            <meta property="og:url" content="{{ SITEURL -}} / {{- page.url }}"/>
+            <meta property="og:title" content="{{ page.title|striptags|breaking_spaces }}" />
+            <meta property="og:url" content="{{ SITEURL -}} / {{- page.url }}" />
+            {% if page.image %}
+                <meta property="og:image"
+                    content="{{ SITEURL -}} / {{- page.image|urlencode }}" />
+            {% elif OPEN_GRAPH_IMAGE %}
+                <meta property="og:image" content="{{ SITEURL -}} / {{- OPEN_GRAPH_IMAGE }}" />
+            {% endif %}
         {% else %}
-            <meta property="og:type" content="website"/>
-            <meta property="og:title" content="{{ SITENAME|striptags|breaking_spaces }}"/>
-            <meta property="og:url" content="{{ SITEURL }}"/>
-            <meta property="og:description" content="{{ SITENAME }}"/>
+            <meta property="og:type" content="website" />
+            <meta property="og:title" content="{{ SITENAME|striptags|breaking_spaces }}" />
+            <meta property="og:url" content="{{ SITEURL }}" />
+            <meta property="og:description" content="{{ SITENAME }}" />
             {% if OPEN_GRAPH_IMAGE %}
                 <meta property="og:image"
-                    content="{{ SITEURL }}/static/{{ OPEN_GRAPH_IMAGE }}"/>
+                    content="{{ SITEURL }}/static/{{ OPEN_GRAPH_IMAGE }}" />
             {% endif %}
         {% endif %}
     {% endif -%}
     
   {% if ASSET_CSS %}
     {# put assets in a seperate file, otherwise it breaks if the assets #}
     {# plugin is not active #}
@@ -175,15 +206,15 @@
                                             {%- if p.icon %}<span class="{{ p.icon }}"></span> {% endif %}{{- p.menulabel|default(p.title) -}}
                                         </a></li>
                                     {% endfor %}
                                 {% endif %}
                                 {% if DISPLAY_CATEGORIES_ON_MENU %}
                                     {% for cat, null in categories %}
                                         <li {% if cat == category %}class="active"{% endif %}>
-                                            <a href="{{ SITEURL -}} / {{- cat.url }}">{{ cat | capitalize }}</a>
+                                            <a href="{{ SITEURL -}} / {{- cat.url }}">{{ cat }}</a>
                                         </li>
                                     {% endfor %}
                                 {% endif %}
                             </ul>
                         {% endif %}
                         {% if DISPLAY_ARCHIVES_ON_MENU and ('tipue_search' in PLUGINS or ARCHIVES_SAVE_AS) %}
                             <ul class="nav navbar-nav {%if NAVBAR_ON_TOP %}navbar-right{% endif %}">
```

#### html2text {}

```diff
@@ -7,22 +7,34 @@
 
 
 
  {%- if FAVICON %}
  {% endif -%} {# Open Graph tags #} {% if USE_OPEN_GRAPH is not defined %} {%
 set USE_OPEN_GRAPH = True %} {% endif %} {% if USE_OPEN_GRAPH %}  {% if
 OPEN_GRAPH_FB_APP_ID %}
- {% endif %} {% if article %}
+ {% endif %}
+ {% if article %}
 
 
 
- {% elif page %}
 
+ {% if article.category %}
+ {% endif %} {% for tag in article.tags %}
+ {% endfor %} {% if article.author %}
+ {% elif AUTHOR %}
+ {% endif %} {% if article.image %}
+ {% elif article.og_image %}
+ {% elif CATEGORY_IMAGES and article.category in CATEGORY_IMAGES %}
+ {% elif OPEN_GRAPH_IMAGE %}
+ {% endif %} {% elif page %}
 
- {% else %}
+
+ {% if page.image %}
+ {% elif OPEN_GRAPH_IMAGE %}
+ {% endif %} {% else %}
 
 
 
  {% if OPEN_GRAPH_IMAGE %}
  {% endif %} {% endif %} {% endif -%} {% if ASSET_CSS %} {# put assets in a
 seperate file, otherwise it breaks if the assets #} {# plugin is not active #}
 {% include 'includes/assets-css.html' %} {% else %}  {% if BOOTSTRAP_THEME %}
@@ -64,15 +76,15 @@
     * {% endif %} {% endif %}
 {% endfor %} {% if DISPLAY_PAGES_ON_MENU %} {% for p in pages|sort
 (attribute='source_path') %}
 % if p == page %} class="active"{% endif %}>{%-_if_p.icon_%}_{%_endif_%}{{-
 p.menulabel|default(p.title)_-}}
 {% endfor %} {% endif %} {% if DISPLAY_CATEGORIES_ON_MENU %} {% for cat, null
 in categories %}
-% if cat == category %}class="active"{% endif %}> {{_cat_|_capitalize_}}
+% if cat == category %}class="active"{% endif %}> {{_cat_}}
 {% endfor %} {% endif %}
 {% endif %} {% if DISPLAY_ARCHIVES_ON_MENU and ('tipue_search' in PLUGINS or
 ARCHIVES_SAVE_AS) %}
     * {% if 'tipue_search' in PLUGINS %}
     * [q                   ] {# consider adding "go!" button #}
     * {% endif %} {% if ARCHIVES_SAVE_AS and not MENUITEMS_2_AT %}
     * Archives
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/categories.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/categories.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/category.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/category.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/addthis.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/addthis.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_info.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_info.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/article_listing.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_listing.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,74 @@
+{# 
+    This is looped to display each acticle in "summary" mode on the index pages.
+#}
+
 {% if HEADING_LEVEL is not defined %}
     {% set HEADING_LEVEL = 2 %}
 {% endif -%}
+
 {% set DISPLAY_IMAGE = false %}
 <article class="row">
-    <h{{ HEADING_LEVEL }} class="col-xs-12">
-        <a href="{{ SITEURL -}} / {{- article.url }}">{{ article.title }}</a>
-    </h{{ HEADING_LEVEL }}>
+    {% if not article.micro %}
+        <h{{ HEADING_LEVEL }} class="col-xs-12">
+            <a href="{{ SITEURL -}} / {{- article.url }}">{{ article.title }}</a>
+        </h{{ HEADING_LEVEL }}>
+    {% endif %}
     {% if article.image %}
         {% set DISPLAY_IMAGE = true %}
         <div class="col-xs-4">
-            <img class="featured-image image-process-index-feature" src="{{ SITEURL -}} / {{- article.image|urlencode }}" alt="{{ article.title|striptags }}">
+            <a href="{{ SITEURL -}} / {{- article.url }}">
+                <img class="featured-image image-process-index-feature" src="{{ SITEURL -}} / {{- article.image|urlencode }}" alt="{{ article.title|striptags }}">
+            </a>
         </div>
         <div class="summary entry-content col-xs-8">
     {% elif CATEGORY_IMAGES and article.category in CATEGORY_IMAGES %}
         {% set DISPLAY_IMAGE = true %}
         <div class="col-xs-4">
-            <img class="featured-image image-process-index-feature" src="{{ SITEURL -}} / {{- CATEGORY_IMAGES[article.category]|urlencode }}"  alt="{{ article.category|striptags }}">
+            <a href="{{ SITEURL -}} / {{- article.url }}">
+                <img class="featured-image image-process-index-feature" src="{{ SITEURL -}} / {{- CATEGORY_IMAGES[article.category]|urlencode }}"  alt="{{ article.category|striptags }}">
+            </a>
         </div>
         <div class="summary entry-content col-xs-8">
     {% else %}
         <div class="summary entry-content col-xs-12">            
     {% endif -%}
 
+    {% if not article.micro %}
         {{- article.summary -}}
+    {% else %}
+        {{- article.content -}}
+    {% endif %}
 
     </div>
     {% if DISPLAY_IMAGE == true %}
         <div class="col-xs-8 col-xs-offset-4">
     {% else %}
         <div class="col-xs-12">
     {% endif %}
         <p class="text-right"><small>
             <span class="published">
                 <i class="fa fa-calendar"></i><time datetime="{{ article.date.isoformat() }}">&nbsp;{{ article.date | article_date }}</time>
             </span>
-            {% if article.readtime_minutes -%}
+            {% if article.readtime_minutes and not article.micro -%}
                 &bull;&nbsp;<i class="fa fa-clock-o"></i>&nbsp;~{{ article.readtime_minutes }}&nbsp;min to read
-            {% elif article.stats -%}
+            {% elif article.stats and not article.micro -%}
                 &bull;&nbsp;<i class="fa fa-clock-o"></i>&nbsp;~{{ article.stats['read_mins'] }}&nbsp;min to read
             {%- endif %}
             {% if (DISQUS_SITENAME and DISQUS_DISPLAY_COUNTS) or (PELICAN_COMMENT_SYSTEM and PELICAN_COMMENT_SYSTEM_DISPLAY_COUNTS != false and article.comments_count > 0) %}
                 &bull;&nbsp;<i class="fa fa-comments"></i>
                 {% include 'includes/comment_count.html' %}
             {% endif -%}
             {# only display the 'read more' link if there is more to the article #}
-            {% if article.has_summary != false %} 
+            {% if article.has_summary != false and not article.micro %} 
                 &bull;&nbsp;<span class="label label-primary">
                     <a href="{{ SITEURL -}} / {{- article.url }}">read more&nbsp;<i class="fa fa-arrow-circle-right"></i>&nbsp;</a>
                 </span>
+            {% elif article.micro %}
+                &bull;&nbsp;<span class="label label-primary">
+                    <a href="{{ SITEURL -}} / {{- article.url }}"><i class="fa fa-link"></i>&nbsp;permalink</a>
+                </span>
             {% endif %}
         </small></p>
     </div>
 </article>
 <hr/>
```

#### html2text {}

```diff
@@ -1,25 +1,30 @@
-{% if HEADING_LEVEL is not defined %} {% set HEADING_LEVEL = 2 %} {% endif -%}
-{% set DISPLAY_IMAGE = false %}
+{# This is looped to display each acticle in "summary" mode on the index pages.
+#} {% if HEADING_LEVEL is not defined %} {% set HEADING_LEVEL = 2 %} {% endif -
+%} {% set DISPLAY_IMAGE = false %}  {% if not article.micro %}
 { HEADING_LEVEL }} class="col-xs-12"> {{_article.title_}}
-{ HEADING_LEVEL }}> {% if article.image %} {% set DISPLAY_IMAGE = true %}
-[{{ article.title|striptags }}]
+{ HEADING_LEVEL }}> {% endif %} {% if article.image %} {% set DISPLAY_IMAGE =
+true %}
+[{{_article.title|striptags_}}]
 {% elif CATEGORY_IMAGES and article.category in CATEGORY_IMAGES %} {% set
 DISPLAY_IMAGE = true %}
-[{{ article.category|striptags }}]
+[{{_article.category|striptags_}}]
 {% else %}
-{% endif -%} {{- article.summary -}}
+{% endif -%} {% if not article.micro %} {{- article.summary -}} {% else %} {{-
+article.content -}} {% endif %}
 {% if DISPLAY_IMAGE == true %}
 {% else %}
 {% endif %}
-  {{ article.date | article_date }}  {% if article.readtime_minutes -%} •  ~{
-{ article.readtime_minutes }} min to read {% elif article.stats -%} •  ~{
-{ article.stats['read_mins'] }} min to read {%- endif %} {% if (DISQUS_SITENAME
-and DISQUS_DISPLAY_COUNTS) or (PELICAN_COMMENT_SYSTEM and
-PELICAN_COMMENT_SYSTEM_DISPLAY_COUNTS != false and article.comments_count > 0)
-%} •  {% include 'includes/comment_count.html' %} {% endif -%} {# only display
-the 'read more' link if there is more to the article #} {% if
-article.has_summary != false %} • 
+  {{ article.date | article_date }}  {% if article.readtime_minutes and not
+article.micro -%} •  ~{{ article.readtime_minutes }} min to read {% elif
+article.stats and not article.micro -%} •  ~{{ article.stats['read_mins']
+}} min to read {%- endif %} {% if (DISQUS_SITENAME and DISQUS_DISPLAY_COUNTS)
+or (PELICAN_COMMENT_SYSTEM and PELICAN_COMMENT_SYSTEM_DISPLAY_COUNTS != false
+and article.comments_count > 0) %} •  {% include 'includes/comment_count.html'
+%} {% endif -%} {# only display the 'read more' link if there is more to the
+article #} {% if article.has_summary != false and not article.micro %} • 
 read_more  
+  {% elif article.micro %} • 
+ permalink
   {% endif %}
 
 ===============================================================================
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/assets-css.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/assets-css.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/cc-license.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/cc-license.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comment_count.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comment_count.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments-js.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comments-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/comments.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comments.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/disqus_script.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/disqus_script.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/footer.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/footer.html`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     {% endif %}
     {% if article.copy_date %}
         {% set copy_date = article.copy_date %}
     {% endif %}
     {% if article.modified %}
         {% set modified = article.modified.strftime('%B %d, %Y').replace(' 0',' ') %}
     {% endif %}
+    {% if article.micro %}
+        {% set micro_footer = True %}
+    {% endif %}
 {% endif -%}
 
 {% if page %}
     {% if page.date %}
         {% set copy_date = page.date.strftime('%Y') %}
     {% endif %}
     {% if page.copy_date %}
@@ -40,14 +43,20 @@
 
 {% if page_name == 'index' %}
     {% if INDEX_COPY_DATE %}
         {% set copy_date = INDEX_COPY_DATE %}
     {% endif %}
 {% endif %}
 
+{% if category %}
+    {% if category == "µ" %}
+        {% set micro_footer = True %}
+    {% endif %}
+{% endif %}
+
 <footer>
     <div class="container">
         <hr>
         <div class="row">
             <div class="col-sm-10 col-xs-8">
                 &copy; {{ copy_date }} {{ AUTHOR }}
                 {% if modified %}
@@ -62,17 +71,23 @@
                 {% endif %}
                 {% if PRJCT %}
                     &bull;
                     <a href="{{ PRJCT_FOOTER_URL or 'https://github.com/MinchinWeb/prjct'}}" target="_blank">prjct {{ PRJCT_VERSION  or "" }}</a>
                 {% endif %}
                 {# TODO: Make this optional #}
                 &bull;
-                <a href="{{ SEAFOAM_URL }}" title="Seafoam version {{ SEAFOAM_VERSION }}">
-                    Seafoam theme
-                </a>
+                <a href="{{ SEAFOAM_URL }}" title="seafoam, version {{ SEAFOAM_VERSION }}">
+                    Seafoam
+                </a> theme
+                {% if micro_footer %}
+                    &bull;
+                    <a href="{{ MICROBLOG_DEV_URL }}" title="minchin.pelican.readers.microblog, version {{ MICROBLOG_VERSION }}">
+                        Microblogging
+                    </a> plugin
+                {% endif %}
                 {% if CC_LICENSE or CC_LICENSE_DERIVATIVES or CC_LICENSE_COMMERCIAL %}
                     &bull;
                     {% from 'includes/cc-license.html' import cc_license_mark %}
                     <p><small>{{ cc_license_mark(cc_name=CC_LICENSE,derivatives=CC_LICENSE_DERIVATIVES,commercial=CC_LICENSE_COMMERCIAL,attr_markup=CC_ATTR_MARKUP,attr_props={'title':SITENAME,'name':article.author if article else AUTHOR,'url':SITEURL}) }}</small></p>
                 {% endif %}
                 {% if FEED_ALL_ATOM %}
                     &bull;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
 {% set modified = False -%} {%- if articles %} {# if we have nothing else, set
 the copyright date to what we use on the index #} {% set copy_date = articles
 [0].date.strftime('%Y') %} {% else %} {% set copy_date = INDEX_COPY_DATE %} {%
 endif -%} {% if article %} {% if article.date %} {% set copy_date =
 article.date.strftime('%Y') %} {% endif %} {% if article.copy_date %} {% set
 copy_date = article.copy_date %} {% endif %} {% if article.modified %} {% set
 modified = article.modified.strftime('%B %d, %Y').replace(' 0',' ') %} {% endif
-%} {% endif -%} {% if page %} {% if page.date %} {% set copy_date =
-page.date.strftime('%Y') %} {% endif %} {% if page.copy_date %} {% set
-copy_date = page.copy_date %} {% endif %} {% if page.modified %} {% set
-modified = page.modified.strftime('%B %d, %Y').replace(' 0',' ') %} {% endif %}
-{% endif -%} {% if ADAM %} {% if copy_date == '' %} {% set copy_date =
-ADAM_COPY_DATE %} {% endif %} {% set modified = ADAM_UPDATED %} {% endif -%} {%
-if page_name == 'index' %} {% if INDEX_COPY_DATE %} {% set copy_date =
-INDEX_COPY_DATE %} {% endif %} {% endif %}
+%} {% if article.micro %} {% set micro_footer = True %} {% endif %} {% endif -
+%} {% if page %} {% if page.date %} {% set copy_date = page.date.strftime('%Y')
+%} {% endif %} {% if page.copy_date %} {% set copy_date = page.copy_date %} {%
+endif %} {% if page.modified %} {% set modified = page.modified.strftime('%B
+%d, %Y').replace(' 0',' ') %} {% endif %} {% endif -%} {% if ADAM %} {% if
+copy_date == '' %} {% set copy_date = ADAM_COPY_DATE %} {% endif %} {% set
+modified = ADAM_UPDATED %} {% endif -%} {% if page_name == 'index' %} {% if
+INDEX_COPY_DATE %} {% set copy_date = INDEX_COPY_DATE %} {% endif %} {% endif
+%} {% if category %} {% if category == "Âµ" %} {% set micro_footer = True %} {%
+endif %} {% endif %}
 ===============================================================================
 © {{ copy_date }} {{ AUTHOR }} {% if modified %} {# 'bull' looks better than
 middot' in the Cabin font #} {# · #} • Last Updated {{ modified }} {% endif %}
 {% if ADAM_VERSION %} • {{_ADAM_VERSION_}} {% endif %} {% if PRJCT %} • prjct_{
 {_PRJCT_VERSION_or_""_}} {% endif %} {# TODO: Make this optional #} • Seafoam
-theme {% if CC_LICENSE or CC_LICENSE_DERIVATIVES or CC_LICENSE_COMMERCIAL %} •
-{% from 'includes/cc-license.html' import cc_license_mark %}
+theme {% if micro_footer %} • Microblogging plugin {% endif %} {% if CC_LICENSE
+or CC_LICENSE_DERIVATIVES or CC_LICENSE_COMMERCIAL %} • {% from 'includes/cc-
+license.html' import cc_license_mark %}
 {{ cc_license_mark
 (cc_name=CC_LICENSE,derivatives=CC_LICENSE_DERIVATIVES,commercial=CC_LICENSE_COMMERCIAL,attr_markup=CC_ATTR_MARKUP,attr_props=
 {'title':SITENAME,'name':article.author if article else AUTHOR,'url':SITEURL})
 }}
 {% endif %} {% if FEED_ALL_ATOM %} •
  Atom_Feed
  (all posts) {% endif %}
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/ga.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/ga.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/github-js.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/github-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/neighbors.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/neighbors.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/pagination.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/piwik.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/piwik.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/sidebar.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/twitter_timeline.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/index.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/tag.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-{% extends "base.html" %}
+{% extends "index.html" %}
+
+{% block title -%}
+    {{ tag|striptags|breaking_spaces }} &mdash; {{ super() }}
+{%- endblock %}
 
 {% block breadcrumbs %}
     {% if DISPLAY_BREADCRUMBS %}
-        <ol class="breadcrumb">
-            <li><a href="{{ SITE_ROOT_URL | default('/') }}" title="{{ SITENAME }}"><span class="fa fa-home fa-lg"></span></a></li>
-            {% if MENUITEMS_2_AT %}
-                <li><a href="{{ SITEURL -}} / {{- MENUITEMS_2_AT_LINK }}" title="{{ MENUITEMS_2_AT }}">{{ MENUITEMS_2_AT }}</a></li>
-            {% endif %}
-        </ol>     
+    <ol class="breadcrumb">
+        <li><a href="{{ SITE_ROOT_URL | default('/') }}" title="{{ SITENAME }}"><span class="fa fa-home fa-lg"></span></a></li>
+      {% if MENUITEMS_2_AT %}
+        <li><a href="{{ SITEURL -}} / {{- MENUITEMS_2_AT_LINK }}" title="{{ MENUITEMS_2_AT }}">{{ MENUITEMS_2_AT }}</a></li>
+      {% endif %}
+        <li><a href="{{ SITEURL -}} / {{- TAGS_URL }}" title="{{ TAGS_TEXT }}">{{ TAGS_TEXT }}</a></li>
+        <li class="active">{{ tag }}</li>
+    </ol>
     {% endif %}
 {% endblock %}
 
-{% block content %}
-    {% if articles %}
-        {% for article in (articles_page.object_list if articles_page else articles) %}
-            {% include 'includes/article_listing.html' %}
-        {% endfor %}
-    {% endif %}
-
-    {% include 'includes/pagination.html' %}
-{% endblock content %}
+{% block prjct %}
+    {% include 'includes/prjct.html' %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
-{% extends "base.html" %} {% block breadcrumbs %} {% if DISPLAY_BREADCRUMBS %}
+{% extends "index.html" %} {% block title -%} {{ tag|striptags|breaking_spaces
+}} — {{ super() }} {%- endblock %} {% block breadcrumbs %} {% if
+DISPLAY_BREADCRUMBS %}
    1. {% if MENUITEMS_2_AT %}
    2. {{_MENUITEMS_2_AT_}}
    3. {% endif %}
-{% endif %} {% endblock %} {% block content %} {% if articles %} {% for article
-in (articles_page.object_list if articles_page else articles) %} {% include
-'includes/article_listing.html' %} {% endfor %} {% endif %} {% include
-'includes/pagination.html' %} {% endblock content %}
+   4. {{_TAGS_TEXT_}}
+   5. {{ tag }}
+{% endif %} {% endblock %} {% block prjct %} {% include 'includes/prjct.html'
+%} {% endblock %}
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/page.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/page.html`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     </ol> <!-- /.breadcrumbs -->
     {% endif %}
 {% endblock %}
 
 {% block content %}
     <section id="content" class="body">
         {% if page.image %}
-            <img class="featured-image image-process-article-feature" src="{{ SITEURL -}} / {{- page.image|urlencode }}" alt="{{ page.title|striptags }}">
+            <img class="featured-image image-process-article-feature" src="{{ SITEURL -}} / {{- page.image|urlencode }}" alt="{{ page.title|striptags }}"/>
         {% endif %}
         <header class="entry-header">
             <h1 class="entry-title">{{ page.title }}</h1>
         </header>
         {% import 'includes/translations.html' as translations with context %}
         {{ translations.translations_for(page) }}
         {% if PDF_PROCESSOR %}
```

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/period_archives.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/prjct.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/prjct.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/search.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/search.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/strathcona/pricing.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/pelican/plugins/seafoam/templates/tags.html` & `seafoam-2.9.0/pelican/plugins/seafoam/templates/tags.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/seafoam.egg-info/PKG-INFO` & `seafoam-2.9.0/seafoam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.8.1
+Version: 2.9.0
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
@@ -113,18 +113,18 @@
 You may also need to configure the theme through the use of additional settings
 (see below).
 
 
 Requirements
 ------------
 
-``Seafoam`` requires Pelican, the ``image_process`` plugin, the ``jinja
-filters`` plugin, ``beautifulsoup4``, and ``semantic_version``. If the theme is
-installed from pip, these should be automatically installed. If needed, they
-can be manually installed with pip:
+``Seafoam`` requires Pelican, the ``image_process`` plugin, the
+``jinja filters`` plugin, ``beautifulsoup4``, and ``semantic_version``. If the
+theme is installed from pip, these should be automatically installed. If
+needed, they can be manually installed with pip:
 
 .. code-block:: sh
 
    pip install pelican
    pip install pelican-image-process
    pip install pelican-jinja-filters
    pip install beautifulsoup4
@@ -133,34 +133,37 @@
 
 Supported Plugins
 -----------------
 
 Seafoam also works with several other plugins for Pelican, but none of those
 listed in this section are required.
 
+- `microblogging <https://blog.minchin.ca/label/microblogging-pelican/>`_ --
+  adds the ability to have "microposts", and tweaks the formatting of the theme
+  based on their (assumed) shorter length.
 - `readtime <https://pypi.python.org/pypi/pelican-readtime>`_ -- provides
   estimated reading time for articles. Available from PyPI as
   ``pelican-readtime``.
 - `post-stats
   <https://github.com/getpelican/pelican-plugins/tree/master/post_stats>`_ --
-  provides estimated reading time for articles if `readtime` is not available.
+  provides estimated reading time for articles if ``readtime`` is not available.
   Available in the `Pelican Plugins collection
   <https://github.com/getpelican/pelican-plugins/>`_.
 - `neighbors <https://pypi.python.org/pypi/pelican-neighbors>`_ -- provides
   post-article links to the next and previous article on your blog and the
   next and previous article in that category. Available on PyPI as
   ``pelican-neighours``.
 - `static-comments <https://blog.minchin.ca/label/static-comments/>`_ (or the
   older `pelican_comment_system
   <https://bernhard.scheirle.de/posts/2014/March/29/static-comments-via-email/>`_)
   -- add static comments to your blog. Available on PyPI as
   ``minchin.pelican.plugins.static-comments``.
 - `Related Posts
   <https://github.com/getpelican/pelican-plugins/tree/master/related_posts>`_ --
-  adds the related_posts variable to the article's context.
+  adds the ``related_posts`` variable to the article's context.
 - Tipue Search
 
 
 Additional Images
 -----------------
 
 Article with header image
@@ -207,14 +210,18 @@
 
 404 Error Page
 
 .. image:: https://github.com/MinchinWeb/seafoam/raw/master/docs/screenshots/2.6.0/404.png
     :align: center
     :alt: 404 Error
 
+.. add microblog post image
+
+.. add Strathcona theme image
+
 
 Additional Settings
 -------------------
 
 These settings can be set in your ``pelicanconf.py`` file (your Pelican settings
 file) to alter the behavior of the theme.
 
@@ -307,17 +314,19 @@
   You can show a short blurb of text about yourself and a picture. This setting
   is the path to the picture. See the ``ABOUT_ME`` setting to set the
   descriptive paragraph.
 BOOTSTRAP_NAVBAR_INVERSE = False
   Apply inverse CSS setting to Navbar. Changing this will swap the top
   navigation bar between light and dark.
 BOOTSTRAP_THEME = "seafoam"
-  Valid values are ``seafoam`` and ``strathcona``. Automatically set to
-  ``seafoam`` by the internal plugin if unspecified. Other values (including
-  leaving this unset) are not expected to work correctly.
+  Use this to set the "colour scheme" of the framework. Valid values are
+  ``seafoam`` and ``strathcona``. ``seafoam`` teal on darker green;
+  ``strathcona`` is maroon on white. This is a Automatically set to ``seafoam``
+  by the internal plugin if unspecified. Other values (including leaving this
+  unset) are not expected to work correctly.
 CATEGORIES_URL
   Same as the regular Pelican setting.
 CATEGORY_IMAGES = {}
   Provide a default featured image by category. If an image is set in the
   article metadata, that will override this.
 
   Provide a dictionary where the key is the category name and the value is the
@@ -500,14 +509,19 @@
   When set and Breadcrumbs are enabled, all items on the site are shown to be
   under both "home" (linked to at the ``SITE_ROOT_URL``) and ``MENUITEMS_2_AT``
   (linked to at ``MENUITEMS_2_AT_LINK``).
 MENUITEMS_2_AT_LINK
   When set and Breadcrumbs are enabled, all items on the site are shown to be
   under both "home" (linked to at the ``SITE_ROOT_URL``) and ``MENUITEMS_2_AT``
   (linked to at ``MENUITEMS_2_AT_LINK``).
+MICROBLOG_DEV_URL
+  The project url for the microblogging plugin. Provided by the plugin, when in
+  use.
+MICROBLOG_VERSION
+  The version of the microblogging plugin. Provided by the plugin, when in use.
 NAVBAR_ON_TOP = False
   If True, the navigation menu is on top. If False, the navigation menu is
   vertical on the left side of the page. Default is False.
 NEIGHBORS
   Activates the links to the next and previous articles, both in the "all
   posts" index and the category-specific index. Requires the
   `neighbors <https://pypi.python.org/pypi/pelican-neighbors>`_ to be both
@@ -720,9 +734,7 @@
 -------
 
 Original theme developed by `Daan Debie <http://dandydev.net/>`_.
 
 The idea that a theme could be installed as a Python package by `Jeff
 Forcier <http://bitprophet.org/>`_'s `Alabaster theme
 <https://github.com/bitprophet/alabaster>`_ for Sphinx.
-
-
```

### Comparing `seafoam-2.8.1/seafoam.egg-info/SOURCES.txt` & `seafoam-2.9.0/seafoam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.8.1/setup.py` & `seafoam-2.9.0/setup.py`

 * *Files identical despite different names*

