# Comparing `tmp/mkdocstrings_python-1.1.2.tar.gz` & `tmp/mkdocstrings_python-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.1.2.tar", last modified: Sun Jun  4 16:19:11 2023, max compression
+gzip compressed data, was "mkdocstrings_python-1.2.0.tar", last modified: Fri Jul 14 17:33:42 2023, max compression
```

## Comparing `mkdocstrings_python-1.1.2.tar` & `mkdocstrings_python-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,72 @@
--rw-r--r--   0        0        0      754 2023-06-02 14:47:59.880294 mkdocstrings_python-1.1.2/LICENSE
--rw-r--r--   0        0        0     4243 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.2/README.md
--rw-r--r--   0        0        0     2604 2023-06-04 16:19:11.833706 mkdocstrings_python-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 14:47:59.736962 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0    18098 2023-06-04 16:11:57.811980 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0     7871 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5036 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     2687 2023-06-04 13:03:08.238478 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2697 2023-06-04 13:02:56.049085 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3356 2023-06-04 13:02:13.028507 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2346 2023-06-04 13:02:01.977392 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3333 2023-06-04 13:01:52.305968 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3301 2023-06-04 13:01:34.118570 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2329 2023-06-04 13:01:20.797497 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3273 2023-06-04 13:01:08.835791 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0      999 2023-06-04 16:06:08.029138 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0      928 2023-06-04 13:03:39.709252 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
--rw-r--r--   0        0        0      934 2023-06-04 13:03:43.052249 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
--rw-r--r--   0        0        0      928 2023-06-03 22:45:13.311332 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
--rw-r--r--   0        0        0      868 2023-06-04 13:03:48.958295 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
--rw-r--r--   0        0        0     1058 2023-06-04 13:03:52.714552 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
--rw-r--r--   0        0        0     1007 2023-06-04 13:03:57.017402 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
--rw-r--r--   0        0        0      863 2023-06-04 13:04:01.126928 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
--rw-r--r--   0        0        0     1040 2023-06-04 13:04:04.606518 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
--rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      174 2023-06-02 14:47:59.730296 mkdocstrings_python-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3042 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.2/tests/conftest.py
--rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/tests/test_handler.py
--rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/tests/test_themes.py
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 mkdocstrings_python-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-07-13 17:32:07.041776 mkdocstrings_python-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4243 2023-07-13 17:32:09.575077 mkdocstrings_python-1.2.0/README.md
+-rw-r--r--   0        0        0     2559 2023-07-14 17:33:42.779897 mkdocstrings_python-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 17:32:06.915111 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    19005 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     8853 2023-07-13 18:49:48.868895 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2896 2023-07-14 15:56:20.488607 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5757 2023-07-13 17:31:51.141977 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4765 2023-07-14 15:49:17.999012 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2827 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      460 2023-07-13 18:33:11.207661 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2853 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3561 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2478 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3490 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3465 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2453 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3430 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0      674 2023-06-27 20:55:41.620344 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2941 2023-07-14 15:55:09.818844 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      250 2023-06-23 09:39:19.320748 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0      794 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
+-rw-r--r--   0        0        0      809 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
+-rw-r--r--   0        0        0      788 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
+-rw-r--r--   0        0        0     2216 2023-07-14 16:29:48.867591 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2790 2023-07-13 18:42:48.068344 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0      431 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/language.html
+-rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/languages/en.html
+-rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
+-rw-r--r--   0        0        0       39 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      999 2023-06-04 16:06:08.029138 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      988 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
+-rw-r--r--   0        0        0      994 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
+-rw-r--r--   0        0        0      988 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
+-rw-r--r--   0        0        0      928 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
+-rw-r--r--   0        0        0     1118 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
+-rw-r--r--   0        0        0     1067 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
+-rw-r--r--   0        0        0      923 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
+-rw-r--r--   0        0        0     1100 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
+-rw-r--r--   0        0        0      431 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
+-rw-r--r--   0        0        0      328 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
+-rw-r--r--   0        0        0      334 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
+-rw-r--r--   0        0        0      330 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
+-rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      174 2023-07-13 17:32:06.908444 mkdocstrings_python-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3052 2023-07-13 17:32:09.575077 mkdocstrings_python-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3295 2023-07-13 18:33:11.210995 mkdocstrings_python-1.2.0/tests/test_handler.py
+-rw-r--r--   0        0        0     3994 2023-07-13 17:31:51.141977 mkdocstrings_python-1.2.0/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.2.0/tests/test_themes.py
+-rw-r--r--   0        0        0     5697 1970-01-01 00:00:00.000000 mkdocstrings_python-1.2.0/PKG-INFO
```

### Comparing `mkdocstrings_python-1.1.2/LICENSE` & `mkdocstrings_python-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/README.md` & `mkdocstrings_python-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/pyproject.toml` & `mkdocstrings_python-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,39 +7,38 @@
 [project]
 name = "mkdocstrings-python"
 description = "A Python handler for mkdocstrings."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = []
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocstrings>=0.20",
-    "griffe>=0.24",
+    "griffe>=0.30",
 ]
-version = "1.1.2"
+version = "1.2.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,29 @@
 import glob
 import os
 import posixpath
 import re
 import sys
 from collections import ChainMap
 from contextlib import suppress
-from typing import TYPE_CHECKING, Any, BinaryIO, Iterator, Mapping
+from typing import TYPE_CHECKING, Any, BinaryIO, ClassVar, Iterator, Mapping
 
 from griffe.collections import LinesCollection, ModulesCollection
 from griffe.docstrings.parsers import Parser
 from griffe.exceptions import AliasResolutionError
+from griffe.extensions import load_extensions
 from griffe.loader import GriffeLoader
 from griffe.logger import patch_loggers
 from mkdocstrings.extension import PluginError
 from mkdocstrings.handlers.base import BaseHandler, CollectionError, CollectorItem
 from mkdocstrings.inventory import Inventory
 from mkdocstrings.loggers import get_logger
 
 from mkdocstrings_handlers.python import rendering
 
-try:
-    from griffe.extensions import load_extensions
-except ImportError:
-    # TODO: remove once support for Griffe 0.25 is dropped
-    from griffe.agents.extensions import load_extensions  # type: ignore[no-redef]
-
 if TYPE_CHECKING:
     from markdown import Markdown
 
 
 if sys.version_info >= (3, 11):
     from contextlib import chdir
 else:
@@ -67,16 +62,16 @@
         default_config: The default rendering options,
             see [`default_config`][mkdocstrings_handlers.python.handler.PythonHandler.default_config].
     """
 
     domain: str = "py"  # to match Sphinx's default domain
     enable_inventory: bool = True
     fallback_theme = "material"
-    fallback_config: dict = {"fallback": True}
-    default_config: dict = {
+    fallback_config: ClassVar[dict] = {"fallback": True}  # type: ignore[misc]
+    default_config: ClassVar[dict] = {
         "docstring_style": "google",
         "docstring_options": {},
         "show_root_heading": False,
         "show_root_toc_entry": True,
         "show_root_full_path": True,
         "show_root_members_full_path": False,
         "show_object_full_path": False,
@@ -102,14 +97,15 @@
         "show_bases": True,
         "show_submodules": False,
         "group_by_category": True,
         "heading_level": 2,
         "members_order": rendering.Order.alphabetical.value,
         "docstring_section_style": "table",
         "members": None,
+        "inherited_members": False,
         "filters": ["!^_[^_]"],
         "annotations_path": "brief",
         "preload_modules": None,
         "load_external_modules": False,
         "allow_inspection": True,
     }
     """
@@ -134,15 +130,21 @@
         show_root_toc_entry (bool): If the root heading is not shown, at least add a ToC entry for it. Default: `True`.
         show_root_full_path (bool): Show the full Python path for the root object heading. Default: `True`.
         show_root_members_full_path (bool): Show the full Python path of the root members. Default: `False`.
         show_object_full_path (bool): Show the full Python path of every object. Default: `False`.
         show_category_heading (bool): When grouped by categories, show a heading for each category. Default: `False`.
 
     Attributes: Members options:
-        members (list[str] | False | None): An explicit list of members to render. Default: `None`.
+        inherited_members (list[str] | bool | None): A boolean, or an explicit list of inherited members to render.
+            If true, select all inherited members, which can then be filtered with `members`.
+            If false or empty list, do not select any inherited member. Default: `False`.
+        members (list[str] | bool | None): A boolean, or an explicit list of members to render.
+            If true, select all members without further filtering.
+            If false or empty list, do not render members.
+            If none, select all members and apply further filtering with filters and docstrings. Default: `None`.
         members_order (str): The members ordering to use. Options: `alphabetical` - order by the members names,
             `source` - order members as they appear in the source file. Default: `"alphabetical"`.
         filters (list[str] | None): A list of filters applied to filter objects based on their name.
             A filter starting with `!` will exclude matching objects instead of including them.
             The `members` option takes precedence over `filters` (filters will still be applied recursively
             to lower members in the hierarchy). Default: `["!^_[^_]"]`.
         group_by_category (bool): Group the object's children by categories: attributes, classes, functions, and modules. Default: `True`.
@@ -176,22 +178,24 @@
     """
 
     def __init__(
         self,
         *args: Any,
         config_file_path: str | None = None,
         paths: list[str] | None = None,
+        locale: str = "en",
         **kwargs: Any,
     ) -> None:
         """Initialize the handler.
 
         Parameters:
             *args: Handler name, theme and custom templates.
             config_file_path: The MkDocs configuration file path.
             paths: A list of paths to use as Griffe search paths.
+            locale: The locale to use when rendering content.
             **kwargs: Same thing, but with keyword arguments.
         """
         super().__init__(*args, **kwargs)
         self._config_file_path = config_file_path
         paths = paths or []
         glob_base_dir = os.path.dirname(os.path.abspath(config_file_path)) if config_file_path else "."
         with chdir(glob_base_dir):
@@ -204,14 +208,15 @@
             if not os.path.isabs(path) and config_file_path:
                 path = os.path.abspath(os.path.join(os.path.dirname(config_file_path), path))  # noqa: PLW2901
             if path not in search_paths:
                 search_paths.insert(0, path)
         self._paths = search_paths
         self._modules_collection: ModulesCollection = ModulesCollection()
         self._lines_collection: LinesCollection = LinesCollection()
+        self._locale = locale
 
     @classmethod
     def load_inventory(
         cls,
         in_file: BinaryIO,
         url: str,
         base_url: str | None = None,
@@ -317,15 +322,21 @@
                 (re.compile(filtr.lstrip("!")), filtr.startswith("!")) for filtr in final_config["filters"]
             ]
 
         # TODO: goal reached: remove once `signature_crossrefs` feature becomes public
         final_config["signature_crossrefs"] = False
 
         return template.render(
-            **{"config": final_config, data.kind.value: data, "heading_level": heading_level, "root": True},
+            **{
+                "config": final_config,
+                data.kind.value: data,
+                "heading_level": heading_level,
+                "root": True,
+                "locale": self._locale,
+            },
         )
 
     def update_env(self, md: Markdown, config: dict) -> None:  # noqa: D102 (ignore missing docstring)
         super().update_env(md, config)
         self.env.trim_blocks = True
         self.env.lstrip_blocks = True
         self.env.keep_trailing_newline = False
@@ -333,41 +344,45 @@
         self.env.filters["multi_crossref"] = rendering.do_multi_crossref
         self.env.filters["order_members"] = rendering.do_order_members
         self.env.filters["format_code"] = rendering.do_format_code
         self.env.filters["format_signature"] = rendering.do_format_signature
         self.env.filters["filter_objects"] = rendering.do_filter_objects
         self.env.filters["stash_crossref"] = lambda ref, length: ref
         self.env.filters["get_template"] = rendering.do_get_template
+        self.env.tests["existing_template"] = lambda template_name: template_name in self.env.list_templates()
 
     def get_anchors(self, data: CollectorItem) -> set[str]:  # noqa: D102 (ignore missing docstring)
         try:
             return {data.path, data.canonical_path, *data.aliases}
         except AliasResolutionError:
             return {data.path}
 
 
 def get_handler(
     theme: str,
     custom_templates: str | None = None,
     config_file_path: str | None = None,
     paths: list[str] | None = None,
+    locale: str = "en",
     **config: Any,  # noqa: ARG001
 ) -> PythonHandler:
     """Simply return an instance of `PythonHandler`.
 
     Arguments:
         theme: The theme to use when rendering contents.
         custom_templates: Directory containing custom templates.
         config_file_path: The MkDocs configuration file path.
         paths: A list of paths to use as Griffe search paths.
+        locale: The locale to use when rendering content.
         **config: Configuration passed to the handler.
 
     Returns:
         An instance of `PythonHandler`.
     """
     return PythonHandler(
         handler="python",
         theme=theme,
         custom_templates=custom_templates,
         config_file_path=config_file_path,
         paths=paths,
+        locale=locale,
     )
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/rendering.py`

 * *Files 21% similar despite different names*

```diff
@@ -99,16 +99,15 @@
     Returns:
         The same code, formatted.
     """
     env = context.environment
     template = env.get_template("signature.html")
     signature = template.render(context.parent, function=function)
     signature = _format_signature(callable_path, signature, line_length)
-    signature = str(env.filters["highlight"](signature, language="python", inline=False))
-    return signature
+    return str(env.filters["highlight"](signature, language="python", inline=False))
 
 
 def do_order_members(
     members: Sequence[Object | Alias],
     order: Order,
     members_list: list[str] | None,
 ) -> Sequence[Object | Alias]:
@@ -191,52 +190,71 @@
     return keep
 
 
 def do_filter_objects(
     objects_dictionary: dict[str, Object | Alias],
     *,
     filters: Sequence[tuple[Pattern, bool]] | None = None,
-    members_list: list[str] | None = None,
+    members_list: bool | list[str] | None = None,
+    inherited_members: bool | list[str] = False,
     keep_no_docstrings: bool = True,
 ) -> list[Object | Alias]:
     """Filter a dictionary of objects based on their docstrings.
 
     Parameters:
         objects_dictionary: The dictionary of objects.
         filters: Filters to apply, based on members' names.
             Each element is a tuple: a pattern, and a boolean indicating whether
             to reject the object if the pattern matches.
         members_list: An optional, explicit list of members to keep.
             When given and empty, return an empty list.
             When given and not empty, ignore filters and docstrings presence/absence.
+        inherited_members: Whether to keep inherited members or exclude them.
         keep_no_docstrings: Whether to keep objects with no/empty docstrings (recursive check).
 
     Returns:
         A list of objects.
     """
-    # no members
-    if members_list is False or members_list == []:
-        return []
-
-    objects = list(objects_dictionary.values())
+    inherited_members_specified = False
+    if inherited_members is True:
+        # Include all inherited members.
+        objects = list(objects_dictionary.values())
+    elif inherited_members is False:
+        # Include no inherited members.
+        objects = [obj for obj in objects_dictionary.values() if not obj.inherited]
+    else:
+        # Include specific inherited members.
+        inherited_members_specified = True
+        objects = [
+            obj for obj in objects_dictionary.values() if not obj.inherited or obj.name in set(inherited_members)
+        ]
 
-    # all members
     if members_list is True:
+        # Return all pre-selected members.
         return objects
 
-    # list of members
+    if members_list is False or members_list == []:
+        # Return selected inherited members, if any.
+        return [obj for obj in objects if obj.inherited]
+
     if members_list is not None:
-        return [obj for obj in objects if obj.name in set(members_list)]
+        # Return selected members (keeping any pre-selected inherited members).
+        return [
+            obj for obj in objects if obj.name in set(members_list) or (inherited_members_specified and obj.inherited)
+        ]
 
-    # none, use filters and docstrings
+    # Use filters and docstrings.
     if filters:
-        objects = [obj for obj in objects if _keep_object(obj.name, filters)]
+        objects = [
+            obj for obj in objects if _keep_object(obj.name, filters) or (inherited_members_specified and obj.inherited)
+        ]
     if keep_no_docstrings:
         return objects
-    return [obj for obj in objects if obj.has_docstrings]
+
+    return [obj for obj in objects if obj.has_docstrings or (inherited_members_specified and obj.inherited)]
 
 
 @lru_cache(maxsize=1)
 def _get_black_formatter() -> Callable[[str, int], str]:
     try:
         from black import Mode, format_str
     except ModuleNotFoundError:
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files 10% similar despite different names*

```diff
@@ -17,53 +17,63 @@
 
     {% filter heading(heading_level,
         role="data" if attribute.parent.kind.value == "module" else "attr",
         id=html_id,
         class="doc doc-heading",
         toc_label=attribute.name) %}
 
-      {% if config.separate_signature %}
-        <span class="doc doc-object-name doc-attribute-name">{% if show_full_path %}{{ attribute.path }}{% else %}{{ attribute.name }}{% endif %}</span>
-      {% else %}
-        {% filter highlight(language="python", inline=True) %}
-          {% if show_full_path %}{{ attribute.path }}{% else %}{{ attribute.name }}{% endif %}
-          {% if attribute.annotation %}: {{ attribute.annotation }}{% endif %}
-          {% if attribute.value %} = {{ attribute.value }}{% endif %}
-        {% endfilter %}
-      {% endif %}
-
-      {% with labels = attribute.labels %}
-        {% include "labels.html" with context %}
-      {% endwith %}
+      {% block heading scoped %}
+        {% if config.separate_signature %}
+          <span class="doc doc-object-name doc-attribute-name">{% if show_full_path %}{{ attribute.path }}{% else %}{{ attribute.name }}{% endif %}</span>
+        {% else %}
+          {% filter highlight(language="python", inline=True) %}
+            {% if show_full_path %}{{ attribute.path }}{% else %}{{ attribute.name }}{% endif %}
+            {% if attribute.annotation %}: {{ attribute.annotation }}{% endif %}
+            {% if attribute.value %} = {{ attribute.value }}{% endif %}
+          {% endfilter %}
+        {% endif %}
+      {% endblock heading %}
+
+      {% block labels scoped %}
+        {% with labels = attribute.labels %}
+          {% include "labels.html" with context %}
+        {% endwith %}
+      {% endblock labels %}
 
     {% endfilter %}
 
-    {% if config.separate_signature %}
-      {% filter highlight(language="python", inline=False) %}
-        {% filter format_code(config.line_length) %}
-          {% if show_full_path %}{{ attribute.path }}{% else %}{{ attribute.name }}{% endif %}
-          {% if attribute.annotation %}: {{ attribute.annotation|safe }}{% endif %}
-          {% if attribute.value %} = {{ attribute.value|safe }}{% endif %}
+    {% block signature scoped %}
+      {% if config.separate_signature %}
+        {% filter highlight(language="python", inline=False) %}
+          {% filter format_code(config.line_length) %}
+            {% if show_full_path %}{{ attribute.path }}{% else %}{{ attribute.name }}{% endif %}
+            {% if attribute.annotation %}: {{ attribute.annotation|safe }}{% endif %}
+            {% if attribute.value %} = {{ attribute.value|safe }}{% endif %}
+          {% endfilter %}
         {% endfilter %}
-      {% endfilter %}
-    {% endif %}
+      {% endif %}
+    {% endblock signature %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
       {% filter heading(heading_level,
           role="data" if attribute.parent.kind.value == "module" else "attr",
           id=html_id,
           toc_label=attribute.path if config.show_root_full_path else attribute.name,
           hidden=True) %}
       {% endfilter %}
     {% endif %}
     {% set heading_level = heading_level - 1 %}
   {% endif %}
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
-    {% with docstring_sections = attribute.docstring.parsed %}
-      {% include "docstring.html" with context %}
-    {% endwith %}
+    {% block contents scoped %}
+      {% block docstring scoped %}
+        {% with docstring_sections = attribute.docstring.parsed %}
+          {% include "docstring.html" with context %}
+        {% endwith %}
+      {% endblock docstring %}
+    {% endblock contents %}
   </div>
 
 {% endwith %}
 </div>
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files 11% similar despite different names*

```diff
@@ -17,94 +17,109 @@
 
     {% filter heading(heading_level,
         role="class",
         id=html_id,
         class="doc doc-heading",
         toc_label=class.name) %}
 
-      {% if config.separate_signature %}
-        <span class="doc doc-object-name doc-class-name">{% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}</span>
-      {% elif config.merge_init_into_class and "__init__" in class.members -%}
-        {%- with function = class.members["__init__"] -%}
-          {%- filter highlight(language="python", inline=True) -%}
-            {% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}
-            {%- include "signature.html" with context -%}
-          {%- endfilter -%}
-        {%- endwith -%}
-      {% else %}
-        <code>{% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}</code>
-      {% endif %}
+      {% block heading scoped %}
+        {% if config.separate_signature %}
+          <span class="doc doc-object-name doc-class-name">{% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}</span>
+        {% elif config.merge_init_into_class and "__init__" in class.members -%}
+          {%- with function = class.members["__init__"] -%}
+            {%- filter highlight(language="python", inline=True) -%}
+              {% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}
+              {%- include "signature.html" with context -%}
+            {%- endfilter -%}
+          {%- endwith -%}
+        {% else %}
+          <code>{% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}</code>
+        {% endif %}
+      {% endblock heading %}
 
-      {% with labels = class.labels %}
-        {% include "labels.html" with context %}
-      {% endwith %}
+      {% block labels scoped %}
+        {% with labels = class.labels %}
+          {% include "labels.html" with context %}
+        {% endwith %}
+      {% endblock labels %}
 
     {% endfilter %}
 
-    {% if config.separate_signature and config.merge_init_into_class %}
-      {% if "__init__" in class.members %}
-        {% with function = class.members["__init__"] %}
-          {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
-            {% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}
-          {% endfilter %}
-        {% endwith %}
+    {% block signature scoped %}
+      {% if config.separate_signature and config.merge_init_into_class %}
+        {% if "__init__" in class.members %}
+          {% with function = class.members["__init__"] %}
+            {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
+              {% if show_full_path %}{{ class.path }}{% else %}{{ class.name }}{% endif %}
+            {% endfilter %}
+          {% endwith %}
+        {% endif %}
       {% endif %}
-    {% endif %}
+    {% endblock signature %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
       {% filter heading(heading_level,
           role="class",
           id=html_id,
           toc_label=class.path if config.show_root_full_path else class.name,
           hidden=True) %}
       {% endfilter %}
     {% endif %}
     {% set heading_level = heading_level - 1 %}
   {% endif %}
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
-    {% if config.show_bases and class.bases %}
-      <p class="doc doc-class-bases">
-        Bases: {% for expression in class.bases -%}
-          <code>{% include "expression.html" with context %}</code>{% if not loop.last %}, {% endif %}
-        {% endfor -%}
-      </p>
-    {% endif %}
+    {% block contents scoped %}
+      {% block bases scoped %}
+        {% if config.show_bases and class.bases %}
+          <p class="doc doc-class-bases">
+            Bases: {% for expression in class.bases -%}
+              <code>{% include "expression.html" with context %}</code>{% if not loop.last %}, {% endif %}
+            {% endfor -%}
+          </p>
+        {% endif %}
+      {% endblock bases %}
 
-    {% with docstring_sections = class.docstring.parsed %}
-      {% include "docstring.html" with context %}
-    {% endwith %}
-
-    {% if config.merge_init_into_class %}
-      {% if "__init__" in class.members and class.members["__init__"].has_docstring %}
-        {% with docstring_sections = class.members["__init__"].docstring.parsed %}
+      {% block docstring scoped %}
+        {% with docstring_sections = class.docstring.parsed %}
           {% include "docstring.html" with context %}
         {% endwith %}
-      {% endif %}
-    {% endif %}
+        {% if config.merge_init_into_class %}
+          {% if "__init__" in class.members and class.members["__init__"].has_docstring %}
+            {% with docstring_sections = class.members["__init__"].docstring.parsed %}
+              {% include "docstring.html" with context %}
+            {% endwith %}
+          {% endif %}
+        {% endif %}
+      {% endblock docstring %}
 
-    {% if config.show_source %}
-      {% if config.merge_init_into_class %}
-        {% if "__init__" in class.members and class.members["__init__"].source %}
-          <details class="quote">
-            <summary>Source code in <code>{{ class.relative_filepath }}</code></summary>
-            {{ class.members["__init__"].source|highlight(language="python", linestart=class.members["__init__"].lineno, linenums=True) }}
-          </details>
+      {% block source scoped %}
+        {% if config.show_source %}
+          {% if config.merge_init_into_class %}
+            {% if "__init__" in class.members and class.members["__init__"].source %}
+              <details class="quote">
+                <summary>Source code in <code>{{ class.relative_filepath }}</code></summary>
+                {{ class.members["__init__"].source|highlight(language="python", linestart=class.members["__init__"].lineno, linenums=True) }}
+              </details>
+            {% endif %}
+          {% elif class.source %}
+            <details class="quote">
+              <summary>Source code in <code>{{ class.relative_filepath }}</code></summary>
+              {{ class.source|highlight(language="python", linestart=class.lineno, linenums=True) }}
+            </details>
+          {% endif %}
         {% endif %}
-      {% elif class.source %}
-        <details class="quote">
-          <summary>Source code in <code>{{ class.relative_filepath }}</code></summary>
-          {{ class.source|highlight(language="python", linestart=class.lineno, linenums=True) }}
-        </details>
-      {% endif %}
-    {% endif %}
+      {% endblock source %}
 
-    {% with obj = class %}
-      {% set root = False %}
-      {% set heading_level = heading_level + 1 %}
-      {% include "children.html" with context %}
-    {% endwith %}
+      {% block children scoped %}
+        {% with obj = class %}
+          {% set root = False %}
+          {% set heading_level = heading_level + 1 %}
+          {% include "children.html" with context %}
+        {% endwith %}
+      {% endblock children %}
+    {% endblock contents %}
   </div>
 
 {% endwith %}
 </div>
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 {{ log.debug("Rendering attributes section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  <p><strong>{{ section.title or "Attributes:" }}</strong></p>
+  <p><strong>{{ section.title or lang.t("Attributes:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        <th>Name</th>
-        <th>Type</th>
-        <th>Description</th>
+        <th>{{ lang.t("Name") }}</th>
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
       {% for attribute in section.value %}
         <tr>
           <td><code>{{ attribute.name }}</code></td>
           <td>
@@ -29,15 +32,15 @@
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Attributes:" }}</p>
+  <p>{{ section.title or lang.t("Attributes:") }}</p>
   <ul>
     {% for attribute in section.value %}
       <li class="field-body">
         <b>{{ attribute.name }}</b>
         {% if attribute.annotation %}
           {% with expression = attribute.annotation %}
             (<code>{% include "expression.html" with context %}</code>)
@@ -52,16 +55,16 @@
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "ATTRIBUTE").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("ATTRIBUTE")).rstrip(":").upper() }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
     <tbody>
       {% for attribute in section.value %}
         <tr>
           <td><code>{{ attribute.name }}</code></td>
           <td class="doc-attribute-details">
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-{{ log.debug("Rendering attributes section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %}
-{{ section.title or "Attributes:" }}
-Name              Type                 Description
+{{ log.debug("Rendering attributes section") }} {% import "language.html" as
+lang with context %} {% if config.docstring_section_style == "table" %} {%
+block table_style %}
+{{ section.title or lang.t("Attributes:") }}
+{{ lang.t("Name") {{ lang.t("Type") }} {{ lang.t("Description") }}
+}}
                   {% if
                   attribute.annotation
                   %} {% with
                   expression =         {
 {{ attribute.name attribute.annotation {
 }}                %} {% include        attribute.description|convert_markdown
                   "expression.html"    (heading_level, html_id) }}
                   with context %} {%
                   endwith %} {% endif
                   %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Attributes:" }}
+{{ section.title or lang.t("Attributes:") }}
     * {% for attribute in section.value %}
     * {{ attribute.name }} {% if attribute.annotation %} {% with expression =
       attribute.annotation %} ({% include "expression.html" with context %}) {%
       endwith %} {% endif %} â
       {{ attribute.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or                DESCRIPTION
-"ATTRIBUTE").rstrip(":").upper() }}
-                                    {
-                                    { attribute.description|convert_markdown
-                                    (heading_level, html_id) }}
-{{ attribute.name }}                {% if attribute.annotation %}  TYPE: {%
-                                    with expression = attribute.annotation
-                                    %} {% include "expression.html" with
-                                    context %} {% endwith %}  {% endif %}
+{{ (section.title or lang.t           {{ lang.t("DESCRIPTION") }}
+("ATTRIBUTE")).rstrip(":").upper() }}
+                                      {{ attribute.description|convert_markdown
+                                      (heading_level, html_id) }}
+{{ attribute.name }}                  {% if attribute.annotation %}  TYPE: {%
+                                      with expression = attribute.annotation %}
+                                      {% include "expression.html" with context
+                                      %} {% endwith %}  {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 {{ log.debug("Rendering other parameters section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  <p><strong>{{ section.title or "Other Parameters:" }}</strong></p>
+  <p><strong>{{ section.title or lang.t("Other Parameters:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        <th>Name</th>
-        <th>Type</th>
-        <th>Description</th>
+        <th>{{ lang.t("Name") }}</th>
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
       {% for parameter in section.value %}
         <tr>
           <td><code>{{ parameter.name }}</code></td>
           <td>
@@ -29,15 +32,15 @@
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Other Parameters:" }}</p>
+  <p>{{ section.title or lang.t("Other Parameters:") }}</p>
   <ul>
     {% for parameter in section.value %}
       <li class="field-body">
         <b>{{ parameter.name }}</b>
         {% if parameter.annotation %}
           {% with expression = parameter.annotation %}
             (<code>{% include "expression.html" with context %}</code>)
@@ -52,30 +55,30 @@
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "PARAMETER").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("PARAMETER")).rstrip(":").upper() }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
     <tbody>
       {% for parameter in section.value %}
         <tr>
           <td><code>{{ parameter.name }}</code></td>
           <td class="doc-param-details">
             <div class="doc-md-description">
               {{ parameter.description|convert_markdown(heading_level, html_id) }}
             </div>
             <p>
               {% if parameter.annotation %}
                 <span class="doc-param-annotation">
-                  <b>TYPE:</b>
+                  <b>{{ lang.t("TYPE:") }}</b>
                   {% with expression = parameter.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
                 </span>
               {% endif %}
             </p>
           </td>
```

#### html2text {}

```diff
@@ -1,35 +1,37 @@
-{{ log.debug("Rendering other parameters section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %}
-{{ section.title or "Other Parameters:" }}
-Name              Type                 Description
+{{ log.debug("Rendering other parameters section") }} {% import "language.html"
+as lang with context %} {% if config.docstring_section_style == "table" %} {%
+block table_style %}
+{{ section.title or lang.t("Other Parameters:") }}
+{{ lang.t("Name") {{ lang.t("Type") }} {{ lang.t("Description") }}
+}}
                   {% if
                   parameter.annotation
                   %} {% with
                   expression =         {
 {{ parameter.name parameter.annotation {
 }}                %} {% include        parameter.description|convert_markdown
                   "expression.html"    (heading_level, html_id) }}
                   with context %} {%
                   endwith %} {% endif
                   %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Other Parameters:" }}
+{{ section.title or lang.t("Other Parameters:") }}
     * {% for parameter in section.value %}
     * {{ parameter.name }} {% if parameter.annotation %} {% with expression =
       parameter.annotation %} ({% include "expression.html" with context %}) {%
       endwith %} {% endif %} â
       {{ parameter.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or                DESCRIPTION
-"PARAMETER").rstrip(":").upper() }}
-                                    {
-                                    { parameter.description|convert_markdown
-                                    (heading_level, html_id) }}
-{{ parameter.name }}                {% if parameter.annotation %}  TYPE: {%
-                                    with expression = parameter.annotation
-                                    %} {% include "expression.html" with
-                                    context %} {% endwith %}  {% endif %}
+{{ (section.title or lang.t           {{ lang.t("DESCRIPTION") }}
+("PARAMETER")).rstrip(":").upper() }}
+                                      {{ parameter.description|convert_markdown
+                                      (heading_level, html_id) }}
+                                      {% if parameter.annotation %}  {{ lang.t
+{{ parameter.name }}                  ("TYPE:") }} {% with expression =
+                                      parameter.annotation %} {% include
+                                      "expression.html" with context %} {%
+                                      endwith %}  {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,103 @@
-{{ log.debug("Rendering parameters section") }}
+{{ log.debug("Rendering receives section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  <p><strong>{{ section.title or "Parameters:" }}</strong></p>
+  {% set name_column = section.value|selectattr("name")|any %}
+  <p><strong>{{ section.title or lang.t("Receives:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        <th>Name</th>
-        <th>Type</th>
-        <th>Description</th>
-        <th>Default</th>
+        {% if name_column %}<th>{{ lang.t("Name") }}</th>{% endif %}
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
-      {% for parameter in section.value %}
+      {% for receives in section.value %}
         <tr>
-          <td><code>{{ parameter.name }}</code></td>
+          {% if name_column %}<td>{% if receives.name %}<code>{{ receives.name }}</code>{% endif %}</td>{% endif %}
           <td>
-            {% if parameter.annotation %}
-              {% with expression = parameter.annotation %}
+            {% if receives.annotation %}
+              {% with expression = receives.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
           <td>
             <div class="doc-md-description">
-              {{ parameter.description|convert_markdown(heading_level, html_id) }}
+              {{ receives.description|convert_markdown(heading_level, html_id) }}
             </div>
           </td>
-          <td>
-            {% if parameter.default %}
-              {% with expression = parameter.default %}
-                <code>{% include "expression.html" with context %}</code>
-              {% endwith %}
-            {% else %}
-              <em>required</em>
-            {% endif %}
-          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Parameters:" }}</p>
+  <p>{{ section.title or lang.t("Receives:") }}</p>
   <ul>
-    {% for parameter in section.value %}
+    {% for receives in section.value %}
       <li class="field-body">
-        <b>{{ parameter.name }}</b>
-        {% if parameter.annotation %}
-          {% with expression = parameter.annotation %}
-            (<code>{% include "expression.html" with context %}</code>)
+        {% if receives.name %}<b>{{ receives.name }}</b>{% endif %}
+        {% if receives.annotation %}
+          {% with expression = receives.annotation %}
+            {% if receives.name %}({% endif %}
+            <code>{% include "expression.html" with context %}</code>
+            {% if receives.name %}){% endif %}
           {% endwith %}
         {% endif %}
         –
         <div class="doc-md-description">
-          {{ parameter.description|convert_markdown(heading_level, html_id) }}
+          {{ receives.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "PARAMETER").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("RECEIVES")).rstrip(":").upper()) }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
     <tbody>
-      {% for parameter in section.value %}
+      {% for receives in section.value %}
         <tr>
-          <td><code>{{ parameter.name }}</code></td>
-          <td class="doc-param-details">
+          <td>
+            {% if receives.name %}
+              <code>{{ receives.name }}</code>
+            {% elif receives.annotation %}
+              <span class="doc-receives-annotation">
+                {% with expression = receives.annotation %}
+                  <code>{% include "expression.html" with context %}</code>
+                {% endwith %}
+              </span>
+            {% endif %}
+          </td>
+          <td class="doc-receives-details">
             <div class="doc-md-description">
-              {{ parameter.description|convert_markdown(heading_level, html_id) }}
+              {{ receives.description|convert_markdown(heading_level, html_id) }}
             </div>
-            <p>
-              {% if parameter.annotation %}
-                <span class="doc-param-annotation">
-                  <b>TYPE:</b>
-                  {% with expression = parameter.annotation %}
-                    <code>{% include "expression.html" with context %}</code>
-                  {% endwith %}
-                </span>
-              {% endif %}
-              {% if parameter.default %}
-                <span class="doc-param-default">
-                  <b>DEFAULT:</b> 
-                  {% with expression = parameter.default %}
+            {% if receives.name and receives.annotation %}
+              <p>
+                <span class="doc-receives-annotation">
+                  <b>{{ lang.t("TYPE:") }}</b>
+                  {% with expression = receives.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
                 </span>
-              {% endif %}
-            </p>
+              </p>
+            {% endif %}
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-{{ log.debug("Rendering parameters section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %}
-{{ section.title or "Parameters:" }}
-Name           Type                 Description                            Default
-               {% if                                                       {% if
-               parameter.annotation                                        parameter.default
-               %} {% with                                                  %} {% with
-{              expression =         {                                      expression =
-{              parameter.annotation {                                      parameter.default
-parameter.name %} {% include        parameter.description|convert_markdown %} {% include
-}}             "expression.html"    (heading_level, html_id) }}            "expression.html"
-               with context %} {%                                          with context %}
-               endwith %} {% endif                                         {% endwith %} {%
-               %}                                                          else %} required
-                                                                           {% endif %}
+{{ log.debug("Rendering receives section") }} {% import "language.html" as lang
+with context %} {% if config.docstring_section_style == "table" %} {% block
+table_style %} {% set name_column = section.value|selectattr("name")|any %}
+{{ section.title or lang.t("Receives:") }}
+{{ lang.t("Name") }} {{ lang.t("Type") }} {{ lang.t("Description") }}
+                     {% if
+                     receives.annotation
+                     %} {% with
+{% if receives.name  expression =         {
+%}{{ receives.name   receives.annotation  {
+}}{% endif %}        %} {% include        receives.description|convert_markdown
+                     "expression.html"    (heading_level, html_id) }}
+                     with context %} {%
+                     endwith %} {% endif
+                     %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Parameters:" }}
-    * {% for parameter in section.value %}
-    * {{ parameter.name }} {% if parameter.annotation %} {% with expression =
-      parameter.annotation %} ({% include "expression.html" with context %}) {%
-      endwith %} {% endif %} â
-      {{ parameter.description|convert_markdown(heading_level, html_id) }}
+{{ section.title or lang.t("Receives:") }}
+    * {% for receives in section.value %}
+    * {% if receives.name %}{{ receives.name }}{% endif %} {% if
+      receives.annotation %} {% with expression = receives.annotation %} {% if
+      receives.name %}({% endif %} {% include "expression.html" with context %}
+      {% if receives.name %}){% endif %} {% endwith %} {% endif %} â
+      {{ receives.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or                DESCRIPTION
-"PARAMETER").rstrip(":").upper() }}
-                                    {
-                                    { parameter.description|convert_markdown
-                                    (heading_level, html_id) }}
-                                    {% if parameter.annotation %}  TYPE: {%
-                                    with expression = parameter.annotation
-{{ parameter.name }}                %} {% include "expression.html" with
-                                    context %} {% endwith %}  {% endif %} {%
-                                    if parameter.default %}  DEFAULT: {%
-                                    with expression = parameter.default %}
-                                    {% include "expression.html" with
-                                    context %} {% endwith %}  {% endif %}
+{{ (section.title or lang.t             {{ lang.t("DESCRIPTION") }}
+("RECEIVES")).rstrip(":").upper()) }}
+                                        {
+                                        { receives.description|convert_markdown
+{% if receives.name %} {{ receives.name (heading_level, html_id) }}
+}} {% elif receives.annotation %}  {%   {% if receives.name and
+with expression = receives.annotation   receives.annotation %}
+%} {% include "expression.html" with     {{ lang.t("TYPE:") }} {% with
+context %} {% endwith %}  {% endif %}   expression = receives.annotation %} {%
+                                        include "expression.html" with context
+                                        %} {% endwith %}
+                                        {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug("Rendering raises section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  <p><strong>{{ section.title or "Raises:" }}</strong></p>
+  <p><strong>{{ section.title or lang.t("Raises:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        <th>Type</th>
-        <th>Description</th>
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
       {% for raises in section.value %}
         <tr>
           <td>
             {% if raises.annotation %}
@@ -27,15 +30,15 @@
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Raises:" }}</p>
+  <p>{{ lang.t(section.title) or lang.t("Raises:") }}</p>
   <ul>
     {% for raises in section.value %}
       <li class="field-body">
         {% if raises.annotation %}
           {% with expression = raises.annotation %}
             <code>{% include "expression.html" with context %}</code>
           {% endwith %}
@@ -49,16 +52,16 @@
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "RAISES").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("RAISES")).rstrip(":").upper() }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
     <tbody>
       {% for raises in section.value %}
         <tr>
           <td>
             <span class="doc-raises-annotation">
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-{{ log.debug("Rendering raises section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %}
-{{ section.title or "Raises:" }}
-Type                                   Description
+{{ log.debug("Rendering raises section") }} {% import "language.html" as lang
+with context %} {% if config.docstring_section_style == "table" %} {% block
+table_style %}
+{{ section.title or lang.t("Raises:") }}
+{{ lang.t("Type") }}                   {{ lang.t("Description") }}
 {% if raises.annotation %} {% with
 expression = raises.annotation %} {%   {{ raises.description|convert_markdown
 include "expression.html" with context (heading_level, html_id) }}
 %} {% endwith %} {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Raises:" }}
+{{ lang.t(section.title) or lang.t("Raises:") }}
     * {% for raises in section.value %}
     * {% if raises.annotation %} {% with expression = raises.annotation %} {%
       include "expression.html" with context %} {% endwith %} â {% endif %}
       {{ raises.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "RAISES").rstrip(": DESCRIPTION
-").upper() }}
- {% with expression = raises.annotation  {{ raises.description|convert_markdown
-%} {% include "expression.html" with     (heading_level, html_id) }}
+{{ (section.title or lang.t             {{ lang.t("DESCRIPTION") }}
+("RAISES")).rstrip(":").upper() }}
+ {% with expression = raises.annotation {{ raises.description|convert_markdown
+%} {% include "expression.html" with    (heading_level, html_id) }}
 context %} {% endwith %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,83 @@
-{{ log.debug("Rendering receives section") }}
+{{ log.debug("Rendering warns section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  {% set name_column = section.value|selectattr("name")|any %}
-  <p><strong>{{ section.title or "Receives:" }}</strong></p>
+  <p><strong>{{ section.title or lang.t("Warns:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        {% if name_column %}<th>Name</th>{% endif %}
-        <th>Type</th>
-        <th>Description</th>
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
-      {% for receives in section.value %}
+      {% for warns in section.value %}
         <tr>
-          {% if name_column %}<td>{% if receives.name %}<code>{{ receives.name }}</code>{% endif %}</td>{% endif %}
           <td>
-            {% if receives.annotation %}
-              {% with expression = receives.annotation %}
+            {% if warns.annotation %}
+              {% with expression = warns.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
           <td>
             <div class="doc-md-description">
-              {{ receives.description|convert_markdown(heading_level, html_id) }}
+              {{ warns.description|convert_markdown(heading_level, html_id) }}
             </div>
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Receives:" }}</p>
+  <p>{{ section.title or lang.t("Warns:") }}</p>
   <ul>
-    {% for receives in section.value %}
+    {% for warns in section.value %}
       <li class="field-body">
-        {% if receives.name %}<b>{{ receives.name }}</b>{% endif %}
-        {% if receives.annotation %}
-          {% with expression = receives.annotation %}
-            {% if receives.name %}({% endif %}
+        {% if warns.annotation %}
+          {% with expression = warns.annotation %}
             <code>{% include "expression.html" with context %}</code>
-            {% if receives.name %}){% endif %}
           {% endwith %}
+          –
         {% endif %}
-        –
         <div class="doc-md-description">
-          {{ receives.description|convert_markdown(heading_level, html_id) }}
+          {{ warns.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "RECEIVES").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("WARNS")).rstrip(":").upper() }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
     <tbody>
-      {% for receives in section.value %}
+      {% for warns in section.value %}
         <tr>
           <td>
-            {% if receives.name %}
-              <code>{{ receives.name }}</code>
-            {% elif receives.annotation %}
-              <span class="doc-receives-annotation">
-                {% with expression = receives.annotation %}
-                  <code>{% include "expression.html" with context %}</code>
-                {% endwith %}
-              </span>
-            {% endif %}
+            <span class="doc-warns-annotation">
+              {% with expression = warns.annotation %}
+                <code>{% include "expression.html" with context %}</code>
+              {% endwith %}
+            </span>
           </td>
-          <td class="doc-receives-details">
+          <td class="doc-warns-details">
             <div class="doc-md-description">
-              {{ receives.description|convert_markdown(heading_level, html_id) }}
+              {{ warns.description|convert_markdown(heading_level, html_id) }}
             </div>
-            {% if receives.name and receives.annotation %}
-              <p>
-                <span class="doc-receives-annotation">
-                  <b>TYPE:</b>
-                  {% with expression = receives.annotation %}
-                    <code>{% include "expression.html" with context %}</code>
-                  {% endwith %}
-                </span>
-              </p>
-            {% endif %}
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,39 +1,25 @@
-{{ log.debug("Rendering receives section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %} {% set
-name_column = section.value|selectattr("name")|any %}
-{{ section.title or "Receives:" }}
-Name                Type                  Description
-                    {% if
-                    receives.annotation
-                    %} {% with expression {
-{% if receives.name = receives.annotation {
-%}{{ receives.name  %} {% include         receives.description|convert_markdown
-}}{% endif %}       "expression.html"     (heading_level, html_id) }}
-                    with context %} {%
-                    endwith %} {% endif
-                    %}
+{{ log.debug("Rendering warns section") }} {% import "language.html" as lang
+with context %} {% if config.docstring_section_style == "table" %} {% block
+table_style %}
+{{ section.title or lang.t("Warns:") }}
+{{ lang.t("Type") }}                      {{ lang.t("Description") }}
+{% if warns.annotation %} {% with
+expression = warns.annotation %} {%       {{ warns.description|convert_markdown
+include "expression.html" with context %} (heading_level, html_id) }}
+{% endwith %} {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Receives:" }}
-    * {% for receives in section.value %}
-    * {% if receives.name %}{{ receives.name }}{% endif %} {% if
-      receives.annotation %} {% with expression = receives.annotation %} {% if
-      receives.name %}({% endif %} {% include "expression.html" with context %}
-      {% if receives.name %}){% endif %} {% endwith %} {% endif %} â
-      {{ receives.description|convert_markdown(heading_level, html_id) }}
+{{ section.title or lang.t("Warns:") }}
+    * {% for warns in section.value %}
+    * {% if warns.annotation %} {% with expression = warns.annotation %} {%
+      include "expression.html" with context %} {% endwith %} â {% endif %}
+      {{ warns.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "RECEIVES").rstrip DESCRIPTION
-(":").upper() }}
-                                        {
-                                        { receives.description|convert_markdown
-{% if receives.name %} {{ receives.name (heading_level, html_id) }}
-}} {% elif receives.annotation %}  {%   {% if receives.name and
-with expression = receives.annotation   receives.annotation %}
-%} {% include "expression.html" with     TYPE: {% with expression =
-context %} {% endwith %}  {% endif %}   receives.annotation %} {% include
-                                        "expression.html" with context %} {%
-                                        endwith %}
-                                        {% endif %}
+{{ (section.title or lang.t               {{ lang.t("DESCRIPTION") }}
+("WARNS")).rstrip(":").upper() }}
+ {% with expression = warns.annotation %} {{ warns.description|convert_markdown
+{% include "expression.html" with context (heading_level, html_id) }}
+%} {% endwith %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 {{ log.debug("Rendering returns section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
   {% set name_column = section.value|selectattr("name")|any %}
-  <p><strong>{{ section.title or "Returns:" }}</strong></p>
+  <p><strong>{{ section.title or lang.t("Returns:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        {% if name_column %}<th>Name</th>{% endif %}
-        <th>Type</th>
-        <th>Description</th>
+        {% if name_column %}<th>{{ lang.t("Name") }}</th>{% endif %}
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
       {% for returns in section.value %}
         <tr>
           {% if name_column %}<td>{% if returns.name %}<code>{{ returns.name }}</code>{% endif %}</td>{% endif %}
           <td>
@@ -30,15 +33,15 @@
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Returns:" }}</p>
+  <p>{{ section.title or lang.t("Returns:") }}</p>
   <ul>
     {% for returns in section.value %}
       <li class="field-body">
         {% if returns.name %}<b>{{ returns.name }}</b>{% endif %}
         {% if returns.annotation %}
           {% with expression = returns.annotation %}
             {% if returns.name %}({% endif %}
@@ -55,16 +58,16 @@
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "RETURNS").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("RETURNS")).rstrip(":").upper() }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION").upper() }}</b></th>
       </tr>
     </thead>
     <tbody>
       {% for returns in section.value %}
         <tr>
           <td>
             {% if returns.name %}
@@ -80,15 +83,15 @@
           <td class="doc-returns-details">
             <div class="doc-md-description">
               {{ returns.description|convert_markdown(heading_level, html_id) }}
             </div>
             {% if returns.name and returns.annotation %}
               <p>
                 <span class="doc-returns-annotation">
-                  <b>TYPE:</b>
+                  <b>{{ lang.t("TYPE:") }}</b>
                   {% with expression = returns.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
                 </span>
               </p>
             {% endif %}
           </td>
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-{{ log.debug("Rendering returns section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %} {% set
-name_column = section.value|selectattr("name")|any %}
-{{ section.title or "Returns:" }}
-Name                 Type                  Description
+{{ log.debug("Rendering returns section") }} {% import "language.html" as lang
+with context %} {% if config.docstring_section_style == "table" %} {% block
+table_style %} {% set name_column = section.value|selectattr("name")|any %}
+{{ section.title or lang.t("Returns:") }}
+{{ lang.t("Name") }} {{ lang.t("Type") }}  {{ lang.t("Description") }}
                      {% if
                      returns.annotation %}
                      {% with expression =  {
 {% if returns.name   returns.annotation %} {
 %}{{ returns.name }} {% include            returns.description|convert_markdown
 {% endif %}          "expression.html"     (heading_level, html_id) }}
                      with context %} {%
                      endwith %} {% endif
                      %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Returns:" }}
+{{ section.title or lang.t("Returns:") }}
     * {% for returns in section.value %}
     * {% if returns.name %}{{ returns.name }}{% endif %} {% if
       returns.annotation %} {% with expression = returns.annotation %} {% if
       returns.name %}({% endif %} {% include "expression.html" with context %}
       {% if returns.name %}){% endif %} {% endwith %} {% endif %} â
       {{ returns.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "RETURNS").rstrip  DESCRIPTION
-(":").upper() }}
+{{ (section.title or lang.t             {{ lang.t("DESCRIPTION").upper() }}
+("RETURNS")).rstrip(":").upper() }}
                                         {{ returns.description|convert_markdown
                                         (heading_level, html_id) }}
 {% if returns.name %} {{ returns.name   {% if returns.name and
 }} {% elif returns.annotation %}  {%    returns.annotation %}
-with expression = returns.annotation %}  TYPE: {% with expression =
-{% include "expression.html" with       returns.annotation %} {% include
-context %} {% endwith %}  {% endif %}   "expression.html" with context %} {%
-                                        endwith %}
+with expression = returns.annotation %}  {{ lang.t("TYPE:") }} {% with
+{% include "expression.html" with       expression = returns.annotation %} {%
+context %} {% endwith %}  {% endif %}   include "expression.html" with context
+                                        %} {% endwith %}
                                         {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,103 @@
-{{ log.debug("Rendering warns section") }}
+{{ log.debug("Rendering yields section") }}
+
+{% import "language.html" as lang with context %}
+
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  <p><strong>{{ section.title or "Warns:" }}</strong></p>
+  {% set name_column = section.value|selectattr("name")|any %}
+  <p><strong>{{ section.title or lang.t("Yields:") }}</strong></p>
   <table>
     <thead>
       <tr>
-        <th>Type</th>
-        <th>Description</th>
+        {% if name_column %}<th>{{ lang.t("Name") }}</th>{% endif %}
+        <th>{{ lang.t("Type") }}</th>
+        <th>{{ lang.t("Description") }}</th>
       </tr>
     </thead>
     <tbody>
-      {% for warns in section.value %}
+      {% for yields in section.value %}
         <tr>
+          {% if name_column %}<td>{% if yields.name %}<code>{{ yields.name }}</code>{% endif %}</td>{% endif %}
           <td>
-            {% if warns.annotation %}
-              {% with expression = warns.annotation %}
+            {% if yields.annotation %}
+              {% with expression = yields.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
           <td>
             <div class="doc-md-description">
-              {{ warns.description|convert_markdown(heading_level, html_id) }}
+              {{ yields.description|convert_markdown(heading_level, html_id) }}
             </div>
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Warns:" }}</p>
+  <p>{{ section.title or lang.t("Yields:") }}</p>
   <ul>
-    {% for warns in section.value %}
+    {% for yields in section.value %}
       <li class="field-body">
-        {% if warns.annotation %}
-          {% with expression = warns.annotation %}
+        {% if yields.name %}<b>{{ yields.name }}</b>{% endif %}
+        {% if yields.annotation %}
+          {% with expression = yields.annotation %}
+            {% if yields.name %}({% endif %}
             <code>{% include "expression.html" with context %}</code>
+            {% if yields.name %}){% endif %}
           {% endwith %}
-          –
         {% endif %}
+        –
         <div class="doc-md-description">
-          {{ warns.description|convert_markdown(heading_level, html_id) }}
+          {{ yields.description|convert_markdown(heading_level, html_id) }}
         </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "WARNS").rstrip(":").upper() }}</b></th>
-        <th><b>DESCRIPTION</b></th>
+        <th><b>{{ (section.title or lang.t("YIELDS")).rstrip(":").upper() }}</b></th>
+        <th><b>{{ lang.t("DESCRIPTION") }}</b></th>
       </tr>
     </thead>
     <tbody>
-      {% for warns in section.value %}
+      {% for yields in section.value %}
         <tr>
           <td>
-            <span class="doc-warns-annotation">
-              {% with expression = warns.annotation %}
-                <code>{% include "expression.html" with context %}</code>
-              {% endwith %}
-            </span>
+            {% if yields.name %}
+              <code>{{ yields.name }}</code>
+            {% elif yields.annotation %}
+              <span class="doc-yields-annotation">
+                {% with expression = yields.annotation %}
+                  <code>{% include "expression.html" with context %}</code>
+                {% endwith %}
+              </span>
+            {% endif %}
           </td>
-          <td class="doc-warns-details">
+          <td class="doc-yields-details">
             <div class="doc-md-description">
-              {{ warns.description|convert_markdown(heading_level, html_id) }}
+              {{ yields.description|convert_markdown(heading_level, html_id) }}
             </div>
+            {% if yields.name and yields.annotation %}
+              <p>
+                <span class="doc-yields-annotation">
+                  <b>{{ lang.t("TYPE:") }}:</b>
+                  {% with expression = yields.annotation %}
+                    <code>{% include "expression.html" with context %}</code>
+                  {% endwith %}
+                </span>
+              </p>
+            {% endif %}
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,24 +1,38 @@
-{{ log.debug("Rendering warns section") }} {% if config.docstring_section_style
-== "table" %} {% block table_style %}
-{{ section.title or "Warns:" }}
-Type                                      Description
-{% if warns.annotation %} {% with
-expression = warns.annotation %} {%       {{ warns.description|convert_markdown
-include "expression.html" with context %} (heading_level, html_id) }}
-{% endwith %} {% endif %}
+{{ log.debug("Rendering yields section") }} {% import "language.html" as lang
+with context %} {% if config.docstring_section_style == "table" %} {% block
+table_style %} {% set name_column = section.value|selectattr("name")|any %}
+{{ section.title or lang.t("Yields:") }}
+{{ lang.t("Name") }}  {{ lang.t("Type") }}  {{ lang.t("Description") }}
+                      {% if
+                      yields.annotation %}
+                      {% with expression =  {
+{% if yields.name %}{ yields.annotation %}  {
+{ yields.name }}{%    {% include            yields.description|convert_markdown
+endif %}              "expression.html"     (heading_level, html_id) }}
+                      with context %} {%
+                      endwith %} {% endif
+                      %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Warns:" }}
-    * {% for warns in section.value %}
-    * {% if warns.annotation %} {% with expression = warns.annotation %} {%
-      include "expression.html" with context %} {% endwith %} â {% endif %}
-      {{ warns.description|convert_markdown(heading_level, html_id) }}
+{{ section.title or lang.t("Yields:") }}
+    * {% for yields in section.value %}
+    * {% if yields.name %}{{ yields.name }}{% endif %} {% if yields.annotation
+      %} {% with expression = yields.annotation %} {% if yields.name %}({%
+      endif %} {% include "expression.html" with context %} {% if yields.name
+      %}){% endif %} {% endwith %} {% endif %} â
+      {{ yields.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "WARNS").rstrip(":   DESCRIPTION
-").upper() }}
- {% with expression = warns.annotation %} {{ warns.description|convert_markdown
-{% include "expression.html" with context (heading_level, html_id) }}
-%} {% endwith %}
+{{ (section.title or lang.t             {{ lang.t("DESCRIPTION") }}
+("YIELDS")).rstrip(":").upper() }}
+                                        {{ yields.description|convert_markdown
+                                        (heading_level, html_id) }}
+{% if yields.name %} {{ yields.name }}  {% if yields.name and yields.annotation
+{% elif yields.annotation %}  {% with   %}
+expression = yields.annotation %} {%     {{ lang.t("TYPE:") }}: {% with
+include "expression.html" with context  expression = yields.annotation %} {%
+%} {% endwith %}  {% endif %}           include "expression.html" with context
+                                        %} {% endwith %}
+                                        {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 {{ log.debug("Rendering " + function.path) }}
 
+{% import "language.html" as lang with context %}
+
 <div class="doc doc-object doc-function">
 {% with html_id = function.path %}
 
   {% if root %}
     {% set show_full_path = config.show_root_full_path %}
     {% set root_members = True %}
   {% elif root_members %}
@@ -17,55 +19,67 @@
 
     {% filter heading(heading_level,
         role="function",
         id=html_id,
         class="doc doc-heading",
         toc_label=function.name ~ "()") %}
 
+      {% block heading scoped %}
+        {% if config.separate_signature %}
+          <span class="doc doc-object-name doc-function-name">{% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}</span>
+        {% else %}
+          {% filter highlight(language="python", inline=True) %}
+            {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
+            {% include "signature.html" with context %}
+          {% endfilter %}
+        {% endif %}
+      {% endblock heading %}
+
+      {% block labels scoped %}
+        {% with labels = function.labels %}
+          {% include "labels.html" with context %}
+        {% endwith %}
+      {% endblock labels %}
+
+    {% endfilter %}
+
+    {% block signature scoped %}
       {% if config.separate_signature %}
-        <span class="doc doc-object-name doc-function-name">{% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}</span>
-      {% else %}
-        {% filter highlight(language="python", inline=True) %}
+        {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
           {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
-          {% include "signature.html" with context %}
         {% endfilter %}
       {% endif %}
-
-      {% with labels = function.labels %}
-        {% include "labels.html" with context %}
-      {% endwith %}
-
-    {% endfilter %}
-
-    {% if config.separate_signature %}
-      {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
-        {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
-      {% endfilter %}
-    {% endif %}
+    {% endblock signature %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
       {% filter heading(heading_level,
           role="function",
           id=html_id,
           toc_label=function.path if config.show_root_full_path else function.name,
           hidden=True) %}
       {% endfilter %}
     {% endif %}
     {% set heading_level = heading_level - 1 %}
   {% endif %}
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
-    {% with docstring_sections = function.docstring.parsed %}
-      {% include "docstring.html" with context %}
-    {% endwith %}
-
-    {% if config.show_source and function.source %}
-      <details class="quote">
-        <summary>Source code in <code>{{ function.relative_filepath }}</code></summary>
-        {{ function.source|highlight(language="python", linestart=function.lineno, linenums=True) }}
-      </details>
-    {% endif %}
+    {% block contents scoped %}
+      {% block docstring scoped %}
+        {% with docstring_sections = function.docstring.parsed %}
+          {% include "docstring.html" with context %}
+        {% endwith %}
+      {% endblock docstring %}
+
+      {% block source scoped %}
+        {% if config.show_source and function.source %}
+          <details class="quote">
+            <summary>{{ lang.t("Source code in") }} <code>{{ function.relative_filepath }}</code></summary>
+            {{ function.source|highlight(language="python", linestart=function.lineno, linenums=True) }}
+          </details>
+        {% endif %}
+      {% endblock source %}
+    {% endblock contents %}
   </div>
 
 {% endwith %}
 </div>
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 
     {% filter heading(heading_level,
         role="module",
         id=html_id,
         class="doc doc-heading",
         toc_label=module.name) %}
 
-      {% with module_name = module.path if show_full_path else module.name %}
-        {% if config.separate_signature %}
-          <span class="doc doc-object-name doc-module-name">{{ module_name }}</span>
-        {% else %}
-          <code>{{ module_name }}</code>
-        {% endif %}
-      {% endwith %}
-
-      {% with labels = module.labels %}
-        {% include "labels.html" with context %}
-      {% endwith %}
+      {% block heading scoped %}
+        {% with module_name = module.path if show_full_path else module.name %}
+          {% if config.separate_signature %}
+            <span class="doc doc-object-name doc-module-name">{{ module_name }}</span>
+          {% else %}
+            <code>{{ module_name }}</code>
+          {% endif %}
+        {% endwith %}
+      {% endblock heading %}
+
+      {% block labels scoped %}
+        {% with labels = module.labels %}
+          {% include "labels.html" with context %}
+        {% endwith %}
+      {% endblock labels %}
 
     {% endfilter %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
       {% filter heading(heading_level,
           role="module",
@@ -44,20 +48,26 @@
           hidden=True) %}
       {% endfilter %}
     {% endif %}
     {% set heading_level = heading_level - 1 %}
   {% endif %}
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
-    {% with docstring_sections = module.docstring.parsed %}
-      {% include "docstring.html" with context %}
-    {% endwith %}
-
-    {% with obj = module %}
-      {% set root = False %}
-      {% set heading_level = heading_level + 1 %}
-      {% include "children.html" with context %}
-    {% endwith %}
+    {% block contents scoped %}
+      {% block docstring scoped %}
+        {% with docstring_sections = module.docstring.parsed %}
+          {% include "docstring.html" with context %}
+        {% endwith %}
+      {% endblock docstring %}
+
+      {% block children scoped %}
+        {% with obj = module %}
+          {% set root = False %}
+          {% set heading_level = heading_level + 1 %}
+          {% include "children.html" with context %}
+        {% endwith %}
+      {% endblock children %}
+    {% endblock contents %}
   </div>
 
 {% endwith %}
 </div>
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files 15% similar despite different names*

```diff
@@ -51,15 +51,18 @@
           {% if parameter.kind.value == "variadic positional" %}*{% elif parameter.kind.value == "variadic keyword" %}**{% endif -%}
           {{ parameter.name }}{{ ns.annotation }}{{ default }}
           {%- if not loop.last %}, {% endif -%}
 
         {%- endif -%}
       {%- endfor -%}
     )
-    {%- if config.show_signature_annotations and function.annotation %} -> {% if config.separate_signature and config.signature_crossrefs -%}
+    {%- if config.show_signature_annotations
+        and function.annotation
+        and not (config.merge_init_into_class and function.name == "__init__" )
+    %} -> {% if config.separate_signature and config.signature_crossrefs -%}
         {%- with expression = function.annotation %}{% include "expression.html" with context %}{%- endwith -%}
       {%- else -%}
         {{ function.annotation|safe }}
       {%- endif -%}
     {%- endif -%}
 
   {%- endwith -%}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Attributes:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Attributes:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for attribute in section.value %}
             <li>
               <b>{{ attribute.name }}</b>
               {% if attribute.annotation %}
                 {% with expression = attribute.annotation %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
 {                 * {% for attribute in section.value %}
 {                 * {{ attribute.name }} {% if attribute.annotation %} {% with
 section.title       expression = attribute.annotation %} ({% include "expression.html"
-or                  with context %}) {% endwith %} {% endif %} â
-"Attributes:        {{ attribute.description|convert_markdown(heading_level, html_id)
-" }}                }}
+or lang.t           with context %}) {% endwith %} {% endif %} â
+("Attributes:       {{ attribute.description|convert_markdown(heading_level, html_id)
+") }}               }}
                   * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Other parameters:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Parameters:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for parameter in section.value %}
             <li>
               <b>{{ parameter.name }}</b>
               {% if parameter.annotation %}
                 {% with expression = parameter.annotation %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
 {                 * {% for parameter in section.value %}
 {                 * {{ parameter.name }} {% if parameter.annotation %} {% with
 section.title       expression = parameter.annotation %} ({% include "expression.html"
-or "Other           with context %}) {% endwith %} {% endif %} â
-parameters:         {{ parameter.description|convert_markdown(heading_level, html_id)
-" }}                }}
+or lang.t           with context %}) {% endwith %} {% endif %} â
+("Parameters:       {{ parameter.description|convert_markdown(heading_level, html_id)
+") }}               }}
                   * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Parameters:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Other parameters:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for parameter in section.value %}
             <li>
               <b>{{ parameter.name }}</b>
               {% if parameter.annotation %}
                 {% with expression = parameter.annotation %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
 {                 * {% for parameter in section.value %}
 {                 * {{ parameter.name }} {% if parameter.annotation %} {% with
 section.title       expression = parameter.annotation %} ({% include "expression.html"
-or                  with context %}) {% endwith %} {% endif %} â
-"Parameters:        {{ parameter.description|convert_markdown(heading_level, html_id)
-" }}                }}
-                  * {% endfor %}
+or lang.t           with context %}) {% endwith %} {% endif %} â
+("Other             {{ parameter.description|convert_markdown(heading_level, html_id)
+parameters:")       }}
+}}                * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Raises:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Raises:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for raises in section.value %}
             <li>
               {% if raises.annotation %}
                 {% with expression = raises.annotation %}
                   <code>{% include "expression.html" with context %}</code>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
 {                 * {% for raises in section.value %}
 {                 * {% if raises.annotation %} {% with expression = raises.annotation %} {%
 section.title       include "expression.html" with context %} {% endwith %} {% endif %} â
-or "Raises:         {{ raises.description|convert_markdown(heading_level, html_id) }}
-" }}              * {% endfor %}
+or lang.t           {{ raises.description|convert_markdown(heading_level, html_id) }}
+("Raises:")       * {% endfor %}
+}}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Receives:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Receives:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for receives in section.value %}
             <li>
               {% if receives.name %}<b>{{ receives.name }}</b>{% endif %}
               {% if receives.annotation %}
                 {% with expression = receives.annotation %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
                   * {% for receives in section.value %}
-                  * {% if receives.name %}{{ receives.name }}{% endif %} {% if
+{                 * {% if receives.name %}{{ receives.name }}{% endif %} {% if
 {                   receives.annotation %} {% with expression =
-{                   receives.annotation %} {% if receives.name %}({% endif %} {%
-section.title       include "expression.html" with context %} {% if receives.name
-or "Receives:       %}){% endif %} {% endwith %} {% endif %} â
-" }}                {{ receives.description|convert_markdown(heading_level,
+section.title       receives.annotation %} {% if receives.name %}({% endif %} {%
+or lang.t           include "expression.html" with context %} {% if receives.name
+("Receives:")       %}){% endif %} {% endwith %} {% endif %} â
+}}                  {{ receives.description|convert_markdown(heading_level,
                     html_id) }}
                   * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-    <th class="field-name">{{ section.title or "Returns:" }}</th>
+    <th class="field-name">{{ section.title or lang.t("Returns:") }}</th>
     <td class="field-body">
       <ul class="first simple">
         {% for returns in section.value %}
           <li>
             {% if returns.name %}<b>{{ returns.name }}</b>{% endif %}
             {% if returns.annotation %}
               {% with expression = returns.annotation %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
                   * {% for returns in section.value %}
-                  * {% if returns.name %}{{ returns.name }}{% endif %} {% if
+{                 * {% if returns.name %}{{ returns.name }}{% endif %} {% if
 {                   returns.annotation %} {% with expression =
-{                   returns.annotation %} {% if returns.name %}({% endif %} {%
-section.title       include "expression.html" with context %} {% if returns.name
-or "Returns:        %}){% endif %} {% endwith %} {% endif %} â
-" }}                {{ returns.description|convert_markdown(heading_level,
+section.title       returns.annotation %} {% if returns.name %}({% endif %} {%
+or lang.t           include "expression.html" with context %} {% if returns.name
+("Returns:")        %}){% endif %} {% endwith %} {% endif %} â
+}}                  {{ returns.description|convert_markdown(heading_level,
                     html_id) }}
                   * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Warns:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Warns:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for warns in section.value %}
             <li>
               {% if warns.annotation %}
                 {% with expression = warns.annotation %}
                   <code>{% include "expression.html" with context %}</code>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
 {                 * {% for warns in section.value %}
 {                 * {% if warns.annotation %} {% with expression = warns.annotation %} {%
 section.title       include "expression.html" with context %} {% endwith %} {% endif %} â
-or "Warns:          {{ warns.description|convert_markdown(heading_level, html_id) }}
-" }}              * {% endfor %}
+or lang.t           {{ warns.description|convert_markdown(heading_level, html_id) }}
+("Warns:") }}     * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {{ log.debug() }}
+
+{% import "language.html" as lang with context %}
+
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">{{ section.title or "Yields:" }}</th>
+      <th class="field-name">{{ section.title or lang.t("Yields:") }}</th>
       <td class="field-body">
         <ul class="first simple">
           {% for yields in section.value %}
             <li>
               {% if yields.name %}<b>{{ yields.name }}</b>{% endif %}
               {% if yields.annotation %}
                 {% with expression = yields.annotation %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{{ log.debug() }}
+{{ log.debug() }} {% import "language.html" as lang with context %}
                   * {% for yields in section.value %}
-                  * {% if yields.name %}{{ yields.name }}{% endif %} {% if
+{                 * {% if yields.name %}{{ yields.name }}{% endif %} {% if
 {                   yields.annotation %} {% with expression = yields.annotation
-{                   %} {% if yields.name %}({% endif %} {% include
-section.title       "expression.html" with context %} {% if yields.name %}){%
-or "Yields:         endif %} {% endwith %} {% endif %} â
-" }}                {{ yields.description|convert_markdown(heading_level,
+section.title       %} {% if yields.name %}({% endif %} {% include
+or lang.t           "expression.html" with context %} {% if yields.name %}){%
+("Yields:")         endif %} {% endwith %} {% endif %} â
+}}                  {{ yields.description|convert_markdown(heading_level,
                     html_id) }}
                   * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.2.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/tests/conftest.py` & `mkdocstrings_python-1.2.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     from pathlib import Path
 
     from mkdocstrings.plugin import MkdocstringsPlugin
 
     from mkdocstrings_handlers.python.handler import PythonHandler
 
 
+pytest_plugins = ["griffe.tests"]
+
+
 @pytest.fixture(name="mkdocs_conf")
 def fixture_mkdocs_conf(request: pytest.FixtureRequest, tmp_path: Path) -> Iterator[config.Config]:
     """Yield a MkDocs configuration object.
 
     Parameters:
         request: Pytest fixture.
         tmp_path: Pytest fixture.
@@ -37,15 +40,15 @@
         "site_name": "foo",
         "site_url": "https://example.org/",
         "site_dir": str(tmp_path),
         "plugins": [{"mkdocstrings": {"default_handler": "python"}}],
         **getattr(request, "param", {}),
     }
     # Re-create it manually as a workaround for https://github.com/mkdocs/mkdocs/issues/2289
-    mdx_configs: dict[str, Any] = dict(ChainMap(*conf_dict.get("markdown_extensions", [])))  # type: ignore[arg-type]
+    mdx_configs: dict[str, Any] = dict(ChainMap(*conf_dict.get("markdown_extensions", [])))
 
     conf.load_dict(conf_dict)
     assert conf.validate() == ([], [])
 
     conf["mdx_configs"] = mdx_configs
     conf["markdown_extensions"].insert(0, "toc")  # Guaranteed to be added by MkDocs.
```

### Comparing `mkdocstrings_python-1.1.2/tests/test_handler.py` & `mkdocstrings_python-1.2.0/tests/test_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     section = DocstringSectionExamples(
         value=[
             (DocstringSectionKind.text, "This is an example."),
             (DocstringSectionKind.examples, ">>> print('Hello')\nHello"),
         ],
     )
     template = handler.env.get_template("docstring/examples.html")
-    rendered = template.render(section=section)
+    rendered = template.render(section=section, locale="en")
+    template.render(section=section, locale="not_existing")
     assert "<p>This is an example.</p>" in rendered
     assert "print" in rendered
     assert "Hello" in rendered
 
 
 def test_expand_globs(tmp_path: Path) -> None:
     """Assert globs are correctly expanded.
```

### Comparing `mkdocstrings_python-1.1.2/tests/test_rendering.py` & `mkdocstrings_python-1.2.0/tests/test_rendering.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any
 
 import pytest
+from griffe.collections import ModulesCollection
+from griffe.tests import temporary_visited_module
 
 from mkdocstrings_handlers.python import rendering
 
 if TYPE_CHECKING:
     from markupsafe import Markup
 
 
@@ -44,14 +46,15 @@
     for length in (5, 100):
         assert rendering._format_signature(name, signature, length)
 
 
 @dataclass
 class _FakeObject:
     name: str
+    inherited: bool = False
 
 
 @pytest.mark.parametrize(
     ("names", "filter_params", "expected_names"),
     [
         (["aa", "ab", "ac", "da"], {"filters": [(re.compile("^a[^b]"), True)]}, {"ab", "da"}),
         (["aa", "ab", "ac", "da"], {"members_list": ["aa", "ab"]}, {"aa", "ab"}),
@@ -65,7 +68,66 @@
         filter_params: Parameters passed to the filter function.
         expected_names: Names expected to be kept.
     """
     objects = {name: _FakeObject(name) for name in names}
     filtered = rendering.do_filter_objects(objects, **filter_params)  # type: ignore[arg-type]
     filtered_names = {obj.name for obj in filtered}
     assert set(filtered_names) == set(expected_names)
+
+
+@pytest.mark.parametrize(
+    ("members", "inherited_members", "expected_names"),
+    [
+        (True, True, {"base", "main"}),
+        (True, False, {"main"}),
+        (True, ["base"], {"base", "main"}),
+        (True, [], {"main"}),
+        (False, True, {"base"}),
+        (False, False, set()),
+        (False, ["base"], {"base"}),
+        (False, [], set()),
+        ([], True, {"base"}),
+        ([], False, set()),
+        ([], ["base"], {"base"}),
+        ([], [], set()),
+        (None, True, {"base", "main"}),
+        (None, False, {"main"}),
+        (None, ["base"], {"base", "main"}),
+        (None, [], {"main"}),
+        (["base"], True, {"base"}),
+        (["base"], False, set()),
+        (["base"], ["base"], {"base"}),
+        (["base"], [], set()),
+        (["main"], True, {"main"}),
+        (["main"], False, {"main"}),
+        (["main"], ["base"], {"base", "main"}),
+        (["main"], [], {"main"}),
+    ],
+)
+def test_filter_inherited_members(
+    members: bool | list[str] | None,
+    inherited_members: bool | list[str],
+    expected_names: list[str],
+) -> None:
+    """Test inherited members filtering.
+
+    Parameters:
+        members: Members option (parametrized).
+        inherited_members: Inherited members option (parametrized).
+        expected_names: The expected result as a list of member names.
+    """
+    collection = ModulesCollection()
+    with temporary_visited_module(
+        """
+        class Base:
+            def base(self): ...
+
+        class Main(Base):
+            def main(self): ...
+        """,
+        modules_collection=collection,
+    ) as module:
+        collection["module"] = module
+        objects = module["Main"].all_members
+        filtered = rendering.do_filter_objects(objects, members_list=members, inherited_members=inherited_members)
+        names = {obj.name for obj in filtered}
+        assert names == expected_names
```

### Comparing `mkdocstrings_python-1.1.2/tests/test_themes.py` & `mkdocstrings_python-1.2.0/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.2/PKG-INFO` & `mkdocstrings_python-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.1.2
+Version: 1.2.0
 Summary: A Python handler for mkdocstrings.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
@@ -23,17 +22,17 @@
 Project-URL: Documentation, https://mkdocstrings.github.io/python
 Project-URL: Changelog, https://mkdocstrings.github.io/python/changelog
 Project-URL: Repository, https://github.com/mkdocstrings/python
 Project-URL: Issues, https://github.com/mkdocstrings/python/issues
 Project-URL: Discussions, https://github.com/mkdocstrings/python/discussions
 Project-URL: Gitter, https://gitter.im/mkdocstrings/python
 Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: mkdocstrings>=0.20
-Requires-Dist: griffe>=0.24
+Requires-Dist: griffe>=0.30
 Description-Content-Type: text/markdown
 
 <h1 align="center">mkdocstrings-python</h1>
 
 <p align="center">A Python handler for <a href="https://github.com/mkdocstrings/mkdocstrings"><i>mkdocstrings</i></a>.</p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.1.2 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.2.0 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
 pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Documentation Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Documentation Classifier: Topic :: Utilities
-Classifier: Typing :: Typed Project-URL: Homepage, https://
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Documentation Classifier: Topic ::
+Utilities Classifier: Typing :: Typed Project-URL: Homepage, https://
 mkdocstrings.github.io/python Project-URL: Documentation, https://
 mkdocstrings.github.io/python Project-URL: Changelog, https://
 mkdocstrings.github.io/python/changelog Project-URL: Repository, https://
 github.com/mkdocstrings/python Project-URL: Issues, https://github.com/
 mkdocstrings/python/issues Project-URL: Discussions, https://github.com/
 mkdocstrings/python/discussions Project-URL: Gitter, https://gitter.im/
 mkdocstrings/python Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.7 Requires-Dist: mkdocstrings>=0.20 Requires-Dist:
-griffe>=0.24 Description-Content-Type: text/markdown
+Requires-Python: >=3.8 Requires-Dist: mkdocstrings>=0.20 Requires-Dist:
+griffe>=0.30 Description-Content-Type: text/markdown
                        ****** mkdocstrings-python ******
                       A Python handler for mkdocstrings.
              [ci] [documentation] [pypi_version] [gitpod] [gitter]
 ---
                                   [logo.png]
 The Python handler uses [Griffe](https://mkdocstrings.github.io/griffe) to
 collect documentation from Python source code. The word "griffe" can sometimes
```

