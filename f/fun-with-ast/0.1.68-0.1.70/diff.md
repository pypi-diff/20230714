# Comparing `tmp/fun_with_ast-0.1.68.tar.gz` & `tmp/fun_with_ast-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fun_with_ast-0.1.68.tar", max compression
+gzip compressed data, was "fun_with_ast-0.1.70.tar", max compression
```

## Comparing `fun_with_ast-0.1.68.tar` & `fun_with_ast-0.1.70.tar`

### file list

```diff
@@ -1,79 +1,89 @@
--rw-r--r--   0        0        0    11404 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/LICENSE
--rw-r--r--   0        0        0     1940 2023-06-24 19:00:12.804812 fun_with_ast-0.1.68/README.md
--rw-r--r--   0        0        0       32 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 13:45:28.535090 fun_with_ast-0.1.68/fun_with_ast/common_utils/__init__.py
--rw-r--r--   0        0        0      154 2023-05-27 13:45:39.285585 fun_with_ast-0.1.68/fun_with_ast/common_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3840 2023-06-24 14:51:23.217759 fun_with_ast-0.1.68/fun_with_ast/common_utils/__pycache__/node_tree_util.cpython-310.pyc
--rw-r--r--   0        0        0     1500 2023-06-05 02:35:19.656796 fun_with_ast-0.1.68/fun_with_ast/common_utils/__pycache__/stack.cpython-310.pyc
--rw-r--r--   0        0        0     1257 2023-06-24 14:50:52.693499 fun_with_ast-0.1.68/fun_with_ast/common_utils/__pycache__/utils_source_match.cpython-310.pyc
--rw-r--r--   0        0        0     3997 2023-06-24 14:51:22.689754 fun_with_ast-0.1.68/fun_with_ast/common_utils/node_tree_util.py
--rw-r--r--   0        0        0      659 2023-06-05 02:35:18.532789 fun_with_ast-0.1.68/fun_with_ast/common_utils/stack.py
--rw-r--r--   0        0        0     1217 2023-06-24 14:50:52.085494 fun_with_ast-0.1.68/fun_with_ast/common_utils/utils_source_match.py
--rw-r--r--   0        0        0     3707 2023-06-30 12:23:36.641693 fun_with_ast-0.1.68/fun_with_ast/get_source.py
--rw-r--r--   0        0        0      477 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/lazy_dict.py
--rw-r--r--   0        0        0        0 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__init__.py
--rw-r--r--   0        0        0      157 2023-05-21 17:24:52.778692 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3174 2023-06-30 10:11:08.896501 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/body_manipulator.cpython-310.pyc
--rw-r--r--   0        0        0    31555 2023-06-30 13:14:33.709442 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/create_node.cpython-310.pyc
--rw-r--r--   0        0        0     4418 2023-06-24 14:55:35.523802 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/if_manipulator.cpython-310.pyc
--rw-r--r--   0        0        0     2630 2023-06-30 10:11:08.420497 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/body_manipulator.py
--rw-r--r--   0        0        0    32763 2023-06-30 13:14:32.641435 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/create_node.py
--rw-r--r--   0        0        0     4773 2023-06-24 14:55:21.787693 fun_with_ast-0.1.68/fun_with_ast/manipulate_node/if_manipulator.py
--rw-r--r--   0        0        0        0 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/placeholders/__init__.py
--rw-r--r--   0        0        0      154 2023-05-21 17:24:52.782692 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4259 2023-07-01 12:18:51.393751 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/args.cpython-310.pyc
--rw-r--r--   0        0        0     1076 2023-06-05 18:47:43.727866 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/base_placeholder.cpython-310.pyc
--rw-r--r--   0        0        0     3068 2023-06-23 10:09:08.074151 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/composite.cpython-310.pyc
--rw-r--r--   0        0        0      725 2023-05-21 17:24:52.790692 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/docstring.cpython-310.pyc
--rw-r--r--   0        0        0     3979 2023-05-21 17:24:52.786692 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/list_placeholder.cpython-310.pyc
--rw-r--r--   0        0        0     1749 2023-06-05 18:40:17.762965 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/node.cpython-310.pyc
--rw-r--r--   0        0        0     2728 2023-07-01 08:33:14.465231 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/string_parser.cpython-310.pyc
--rw-r--r--   0        0        0     3001 2023-06-05 19:12:56.412060 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/string_part.cpython-310.pyc
--rw-r--r--   0        0        0     3460 2023-06-05 18:39:19.650802 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/text.cpython-310.pyc
--rw-r--r--   0        0        0      741 2023-05-21 17:24:52.786692 fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/whitespace.cpython-310.pyc
--rw-r--r--   0        0        0     5054 2023-07-01 12:18:51.005753 fun_with_ast-0.1.68/fun_with_ast/placeholders/args.py
--rw-r--r--   0        0        0      441 2023-06-05 18:47:42.631866 fun_with_ast-0.1.68/fun_with_ast/placeholders/base_placeholder.py
--rw-r--r--   0        0        0     2925 2023-06-23 09:52:44.412221 fun_with_ast-0.1.68/fun_with_ast/placeholders/composite.py
--rw-r--r--   0        0        0      313 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/placeholders/docstring.py
--rw-r--r--   0        0        0     4182 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/placeholders/list_placeholder.py
--rw-r--r--   0        0        0     1393 2023-06-05 18:40:16.714960 fun_with_ast-0.1.68/fun_with_ast/placeholders/node.py
--rw-r--r--   0        0        0     2932 2023-07-01 08:33:13.473188 fun_with_ast-0.1.68/fun_with_ast/placeholders/string_parser.py
--rw-r--r--   0        0        0     2824 2023-06-05 19:12:55.372064 fun_with_ast-0.1.68/fun_with_ast/placeholders/string_part.py
--rw-r--r--   0        0        0     3337 2023-06-05 18:39:18.550806 fun_with_ast-0.1.68/fun_with_ast/placeholders/text.py
--rw-r--r--   0        0        0      329 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/placeholders/whitespace.py
--rw-r--r--   0        0        0      367 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/setup.py
--rw-r--r--   0        0        0    17580 2023-07-01 07:18:42.391436 fun_with_ast-0.1.68/fun_with_ast/source_match.py
--rw-r--r--   0        0        0        0 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__init__.py
--rw-r--r--   0        0        0      157 2023-05-21 17:24:52.778692 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6485 2023-07-01 08:44:31.010064 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/base_matcher.cpython-310.pyc
--rw-r--r--   0        0        0     2606 2023-06-05 18:28:41.331218 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/body.cpython-310.pyc
--rw-r--r--   0        0        0     2446 2023-06-08 15:40:07.270261 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/boolop.cpython-310.pyc
--rw-r--r--   0        0        0     1970 2023-06-11 17:26:15.239433 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/constant_source_match.cpython-310.pyc
--rw-r--r--   0        0        0     3858 2023-07-01 11:49:50.215942 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/defualt_matcher.cpython-310.pyc
--rw-r--r--   0        0        0      731 2023-06-05 02:19:10.678035 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     3791 2023-06-18 03:44:31.941512 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/if_source_match.cpython-310.pyc
--rw-r--r--   0        0        0     3055 2023-06-06 13:41:19.856484 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/joined_str.cpython-310.pyc
--rw-r--r--   0        0        0     5583 2023-06-11 10:19:25.732860 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/matcher_resolver.cpython-310.pyc
--rw-r--r--   0        0        0      506 2023-06-11 17:25:45.707480 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/number.cpython-310.pyc
--rw-r--r--   0        0        0     4082 2023-06-21 19:10:20.927247 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/str.cpython-310.pyc
--rw-r--r--   0        0        0     1263 2023-05-21 17:24:52.790692 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/syntaxfreeline.cpython-310.pyc
--rw-r--r--   0        0        0      578 2023-06-11 17:15:14.139750 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/tuple.cpython-310.pyc
--rw-r--r--   0        0        0     2435 2023-06-05 19:14:38.306776 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/with_matcher.cpython-310.pyc
--rw-r--r--   0        0        0     1587 2023-06-07 05:30:29.253128 fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/withitem.cpython-310.pyc
--rw-r--r--   0        0        0     7933 2023-07-01 08:44:29.930051 fun_with_ast-0.1.68/fun_with_ast/source_matchers/base_matcher.py
--rw-r--r--   0        0        0     3070 2023-06-05 18:28:40.919216 fun_with_ast-0.1.68/fun_with_ast/source_matchers/body.py
--rw-r--r--   0        0        0     7123 2023-06-08 15:40:06.842267 fun_with_ast-0.1.68/fun_with_ast/source_matchers/boolop.py
--rw-r--r--   0        0        0     2506 2023-06-11 17:26:14.871434 fun_with_ast-0.1.68/fun_with_ast/source_matchers/constant_source_match.py
--rw-r--r--   0        0        0     8636 2023-07-01 11:49:49.231941 fun_with_ast-0.1.68/fun_with_ast/source_matchers/defualt_matcher.py
--rw-r--r--   0        0        0      187 2023-06-05 02:18:41.229809 fun_with_ast-0.1.68/fun_with_ast/source_matchers/exceptions.py
--rw-r--r--   0        0        0     4765 2023-06-18 03:44:30.861520 fun_with_ast-0.1.68/fun_with_ast/source_matchers/if_source_match.py
--rw-r--r--   0        0        0     3610 2023-06-06 13:41:19.284482 fun_with_ast-0.1.68/fun_with_ast/source_matchers/joined_str.py
--rw-r--r--   0        0        0     8333 2023-06-11 10:19:25.236980 fun_with_ast-0.1.68/fun_with_ast/source_matchers/matcher_resolver.py
--rw-r--r--   0        0        0     4032 2023-06-11 17:25:45.207480 fun_with_ast-0.1.68/fun_with_ast/source_matchers/number.py
--rw-r--r--   0        0        0     5346 2023-06-21 19:10:20.439252 fun_with_ast-0.1.68/fun_with_ast/source_matchers/str.py
--rw-r--r--   0        0        0      920 2023-05-20 15:44:20.967392 fun_with_ast-0.1.68/fun_with_ast/source_matchers/syntaxfreeline.py
--rw-r--r--   0        0        0     1464 2023-06-11 17:15:13.563748 fun_with_ast-0.1.68/fun_with_ast/source_matchers/tuple.py
--rw-r--r--   0        0        0     3438 2023-06-05 19:14:37.874754 fun_with_ast-0.1.68/fun_with_ast/source_matchers/with_matcher.py
--rw-r--r--   0        0        0     1303 2023-06-07 05:22:34.465666 fun_with_ast-0.1.68/fun_with_ast/source_matchers/withitem.py
--rw-r--r--   0        0        0      409 2023-07-01 17:50:32.916624 fun_with_ast-0.1.68/pyproject.toml
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 fun_with_ast-0.1.68/PKG-INFO
+-rw-r--r--   0        0        0    11404 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/LICENSE
+-rw-r--r--   0        0        0     2156 2023-07-14 13:43:43.562970 fun_with_ast-0.1.70/README.md
+-rw-r--r--   0        0        0       32 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:45:28.535090 fun_with_ast-0.1.70/fun_with_ast/common_utils/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-27 13:45:39.285585 fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      756 2023-07-11 15:54:25.573320 fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/constant_visitor.cpython-310.pyc
+-rw-r--r--   0        0        0     1131 2023-07-11 15:25:49.596947 fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/node_tree_util.cpython-310.pyc
+-rw-r--r--   0        0        0     1732 2023-07-09 12:44:22.373882 fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/parenthese_stack.cpython-310.pyc
+-rw-r--r--   0        0        0     1500 2023-06-05 02:35:19.656796 fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/stack.cpython-310.pyc
+-rw-r--r--   0        0        0     1140 2023-07-13 16:43:46.966659 fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/utils_source_match.cpython-310.pyc
+-rw-r--r--   0        0        0      317 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/common_utils/constant_visitor.py
+-rw-r--r--   0        0        0     4134 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/common_utils/node_tree_util.py
+-rw-r--r--   0        0        0     2266 2023-07-09 12:43:46.113659 fun_with_ast-0.1.70/fun_with_ast/common_utils/parenthese_stack.py
+-rw-r--r--   0        0        0      659 2023-06-05 02:35:18.532789 fun_with_ast-0.1.70/fun_with_ast/common_utils/stack.py
+-rw-r--r--   0        0        0     1175 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/common_utils/utils_source_match.py
+-rw-r--r--   0        0        0     3403 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/get_source.py
+-rw-r--r--   0        0        0      477 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/lazy_dict.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-21 17:24:52.778692 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3182 2023-07-09 12:58:55.453372 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/body_manipulator.cpython-310.pyc
+-rw-r--r--   0        0        0      574 2023-07-09 12:44:22.369882 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/call_args_node.cpython-310.pyc
+-rw-r--r--   0        0        0    30079 2023-07-12 15:42:08.323096 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/create_node.cpython-310.pyc
+-rw-r--r--   0        0        0     1368 2023-07-12 05:42:08.714075 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/get_node_from_input.cpython-310.pyc
+-rw-r--r--   0        0        0     4418 2023-06-24 14:55:35.523802 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/if_manipulator.cpython-310.pyc
+-rw-r--r--   0        0        0     1642 2023-07-09 12:44:22.369882 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/syntax_free_line_node.cpython-310.pyc
+-rw-r--r--   0        0        0     2638 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/body_manipulator.py
+-rw-r--r--   0        0        0      199 2023-07-09 12:43:46.113659 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/call_args_node.py
+-rw-r--r--   0        0        0    31470 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/create_node.py
+-rw-r--r--   0        0        0     1127 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/get_node_from_input.py
+-rw-r--r--   0        0        0     4773 2023-06-24 14:55:21.787693 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/if_manipulator.py
+-rw-r--r--   0        0        0     1350 2023-07-09 12:43:46.113659 fun_with_ast-0.1.70/fun_with_ast/manipulate_node/syntax_free_line_node.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/placeholders/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-21 17:24:52.782692 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5631 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/args.cpython-310.pyc
+-rw-r--r--   0        0        0     1153 2023-07-08 08:23:34.569841 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/base_match.cpython-310.pyc
+-rw-r--r--   0        0        0     1076 2023-06-05 18:47:43.727866 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/base_placeholder.cpython-310.pyc
+-rw-r--r--   0        0        0     3274 2023-07-13 16:46:27.537173 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/composite.cpython-310.pyc
+-rw-r--r--   0        0        0      725 2023-05-21 17:24:52.790692 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/docstring.cpython-310.pyc
+-rw-r--r--   0        0        0     3989 2023-07-09 12:44:22.373882 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/list_placeholder.cpython-310.pyc
+-rw-r--r--   0        0        0     1749 2023-06-05 18:40:17.762965 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/node.cpython-310.pyc
+-rw-r--r--   0        0        0     2728 2023-07-06 05:48:33.549622 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/string_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     3001 2023-06-05 19:12:56.412060 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/string_part.cpython-310.pyc
+-rw-r--r--   0        0        0     3571 2023-07-09 12:44:22.369882 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/text.cpython-310.pyc
+-rw-r--r--   0        0        0      741 2023-05-21 17:24:52.786692 fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/whitespace.cpython-310.pyc
+-rw-r--r--   0        0        0     7453 2023-07-09 12:43:46.113659 fun_with_ast-0.1.70/fun_with_ast/placeholders/args.py
+-rw-r--r--   0        0        0     1232 2023-07-08 08:00:14.819532 fun_with_ast-0.1.70/fun_with_ast/placeholders/base_match.py
+-rw-r--r--   0        0        0      441 2023-06-05 18:47:42.631866 fun_with_ast-0.1.70/fun_with_ast/placeholders/base_placeholder.py
+-rw-r--r--   0        0        0     3181 2023-07-14 13:42:36.378203 fun_with_ast-0.1.70/fun_with_ast/placeholders/composite.py
+-rw-r--r--   0        0        0      313 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/placeholders/docstring.py
+-rw-r--r--   0        0        0     4192 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/placeholders/list_placeholder.py
+-rw-r--r--   0        0        0     1393 2023-06-05 18:40:16.714960 fun_with_ast-0.1.70/fun_with_ast/placeholders/node.py
+-rw-r--r--   0        0        0     2932 2023-07-06 05:46:48.303967 fun_with_ast-0.1.70/fun_with_ast/placeholders/string_parser.py
+-rw-r--r--   0        0        0     2824 2023-06-05 19:12:55.372064 fun_with_ast-0.1.70/fun_with_ast/placeholders/string_part.py
+-rw-r--r--   0        0        0     3335 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/placeholders/text.py
+-rw-r--r--   0        0        0      329 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/placeholders/whitespace.py
+-rw-r--r--   0        0        0      367 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/setup.py
+-rw-r--r--   0        0        0    17801 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_match.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:44:20.967392 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__init__.py
+-rw-r--r--   0        0        0      157 2023-05-21 17:24:52.778692 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4955 2023-07-09 12:44:22.369882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/base_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     2611 2023-07-09 12:44:22.373882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/body.cpython-310.pyc
+-rw-r--r--   0        0        0     2222 2023-07-09 12:44:22.365882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/boolop.cpython-310.pyc
+-rw-r--r--   0        0        0     2006 2023-07-12 16:15:38.923746 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/constant_source_match.cpython-310.pyc
+-rw-r--r--   0        0        0     3775 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/defualt_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0      731 2023-06-05 02:19:10.678035 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     3851 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/if_source_match.cpython-310.pyc
+-rw-r--r--   0        0        0     3055 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/joined_str.cpython-310.pyc
+-rw-r--r--   0        0        0     5823 2023-07-09 12:44:22.365882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/matcher_resolver.cpython-310.pyc
+-rw-r--r--   0        0        0     4238 2023-07-13 16:44:11.974584 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/str.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/syntaxfreeline.cpython-310.pyc
+-rw-r--r--   0        0        0      578 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/tuple.cpython-310.pyc
+-rw-r--r--   0        0        0     2485 2023-07-09 12:44:22.377882 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/with_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     1637 2023-07-08 08:23:34.581842 fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/withitem.cpython-310.pyc
+-rw-r--r--   0        0        0     4667 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/base_matcher.py
+-rw-r--r--   0        0        0     3075 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/body.py
+-rw-r--r--   0        0        0     2388 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/boolop.py
+-rw-r--r--   0        0        0     2354 2023-07-14 13:42:36.382202 fun_with_ast-0.1.70/fun_with_ast/source_matchers/constant_source_match.py
+-rw-r--r--   0        0        0     4384 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/defualt_matcher.py
+-rw-r--r--   0        0        0      187 2023-06-05 02:18:41.229809 fun_with_ast-0.1.70/fun_with_ast/source_matchers/exceptions.py
+-rw-r--r--   0        0        0     4823 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/if_source_match.py
+-rw-r--r--   0        0        0     2955 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/joined_str.py
+-rw-r--r--   0        0        0     8085 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/matcher_resolver.py
+-rw-r--r--   0        0        0     5238 2023-07-14 13:42:36.382202 fun_with_ast-0.1.70/fun_with_ast/source_matchers/str.py
+-rw-r--r--   0        0        0      865 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/syntaxfreeline.py
+-rw-r--r--   0        0        0      281 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/tuple.py
+-rw-r--r--   0        0        0     3193 2023-07-09 12:43:46.117659 fun_with_ast-0.1.70/fun_with_ast/source_matchers/with_matcher.py
+-rw-r--r--   0        0        0     1351 2023-07-08 08:00:14.823531 fun_with_ast-0.1.70/fun_with_ast/source_matchers/withitem.py
+-rw-r--r--   0        0        0      409 2023-07-14 14:08:38.060394 fun_with_ast-0.1.70/pyproject.toml
+-rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 fun_with_ast-0.1.70/PKG-INFO
```

### Comparing `fun_with_ast-0.1.68/LICENSE` & `fun_with_ast-0.1.70/LICENSE`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/common_utils/__pycache__/stack.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/common_utils/__pycache__/stack.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/common_utils/node_tree_util.py` & `fun_with_ast-0.1.70/fun_with_ast/common_utils/node_tree_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,104 +15,104 @@
 #    _ast.TryExcept: ['body', 'orelse'],
 #    _ast.Try: ['finalbody'],
     _ast.While: ['body'],
     _ast.With: ['body'],
 }
 
 
-class IndentLevelVisitor(ast.NodeVisitor):
-  """Tracks the indent level of the current node."""
+# class IndentLevelVisitor(ast.NodeVisitor):
+#   """Tracks the indent level of the current node."""
+#
+#   def __init__(self, node_to_check):
+#     self.current_indent = 0
+#     self.node_to_check = node_to_check
+#     self.final_indent = None
+#
+#   def generic_visit(self, node):
+#     """Called if no explicit visitor function exists for a node."""
+#     if node == self.node_to_check:
+#       self.final_indent = self.current_indent
+#     for field, value in ast.iter_fields(node):
+#       if (isinstance(node, tuple(TYPE_TO_INDENT_FIELD.keys())) and
+#           field in TYPE_TO_INDENT_FIELD[node.__class__]):
+#         self.current_indent += 1
+#       if isinstance(value, list):
+#         for item in value:
+#           if isinstance(item, _ast.AST):
+#             self.visit(item)
+#       elif isinstance(value, _ast.AST):
+#         self.visit(value)
+#       if (isinstance(node, tuple(TYPE_TO_INDENT_FIELD.keys())) and
+#           field in TYPE_TO_INDENT_FIELD[node.__class__]):
+#         self.current_indent -= 1
+#     return node
+
+  # def visit_With(self, node):
+  #   if hasattr(node, 'matcher') and node.matcher.is_compound_with:
+  #     self.current_indent -= 1
+  #   self.generic_visit(node)
+  #   return node
+
+
+# def GetIndentLevel(module_node, node_to_check):
+#   visitor = IndentLevelVisitor(node_to_check)
+#   visitor.visit(module_node)
+#   if visitor.final_indent is None:
+#     raise ValueError('node is not in module.')
+#   return visitor.final_indent
+
 
-  def __init__(self, node_to_check):
-    self.current_indent = 0
-    self.node_to_check = node_to_check
-    self.final_indent = None
-
-  def generic_visit(self, node):
-    """Called if no explicit visitor function exists for a node."""
-    if node == self.node_to_check:
-      self.final_indent = self.current_indent
-    for field, value in ast.iter_fields(node):
-      if (isinstance(node, tuple(TYPE_TO_INDENT_FIELD.keys())) and
-          field in TYPE_TO_INDENT_FIELD[node.__class__]):
-        self.current_indent += 1
-      if isinstance(value, list):
-        for item in value:
-          if isinstance(item, _ast.AST):
-            self.visit(item)
-      elif isinstance(value, _ast.AST):
-        self.visit(value)
-      if (isinstance(node, tuple(TYPE_TO_INDENT_FIELD.keys())) and
-          field in TYPE_TO_INDENT_FIELD[node.__class__]):
-        self.current_indent -= 1
-    return node
-
-  def visit_With(self, node):
-    if hasattr(node, 'matcher') and node.matcher.is_compound_with:
-      self.current_indent -= 1
-    self.generic_visit(node)
-    return node
-
-
-def GetIndentLevel(module_node, node_to_check):
-  visitor = IndentLevelVisitor(node_to_check)
-  visitor.visit(module_node)
-  if visitor.final_indent is None:
-    raise ValueError('node is not in module.')
-  return visitor.final_indent
-
-
-class _WrappingStmtVisitor(ast.NodeVisitor):
-
-  def __init__(self, node_to_check):
-    self.node_to_check = node_to_check
-    self.current_stmt = None
-    self.correct_stmt = None
-
-  def generic_visit(self, node):
-    """Called if no explicit visitor function exists for a node."""
-    if isinstance(node, _ast.stmt):
-      self.current_stmt = node
-    if node == self.node_to_check:
-      self.correct_stmt = self.current_stmt
-    return super(_WrappingStmtVisitor, self).generic_visit(node)
+# class _WrappingStmtVisitor(ast.NodeVisitor):
+#
+#   def __init__(self, node_to_check):
+#     self.node_to_check = node_to_check
+#     self.current_stmt = None
+#     self.correct_stmt = None
+#
+#   def generic_visit(self, node):
+#     """Called if no explicit visitor function exists for a node."""
+#     if isinstance(node, _ast.stmt):
+#       self.current_stmt = node
+#     if node == self.node_to_check:
+#       self.correct_stmt = self.current_stmt
+#     return super(_WrappingStmtVisitor, self).generic_visit(node)
 
 #
 # def GetWrappingStmtNode(module_node, node_in_stmt):
 #   visitor = _WrappingStmtVisitor(node_in_stmt)
 #   visitor.visit(module_node)
 #   return visitor.correct_stmt
 #
 def IsEmptyModule(node):
     if not isinstance(node, _ast.Module):
         return False
     return len(node.body) == 0
 
-class _ParentVisitor(ast.NodeVisitor):
+# class _ParentVisitor(ast.NodeVisitor):
+#
+#   def __init__(self, node_to_check):
+#     self.node_to_check = node_to_check
+#     self.parent_stack = []
+#     self.correct_parent = None
+#
+#   def generic_visit(self, node):
+#     """Called if no explicit visitor function exists for a node."""
+#     if self.correct_parent:
+#       return node
+#     if node == self.node_to_check:
+#       self.correct_parent = self.parent_stack.pop()
+#     self.parent_stack.append(node)
+#     super(_ParentVisitor, self).generic_visit(node)
+#     self.parent_stack.pop()
+#
 
-  def __init__(self, node_to_check):
-    self.node_to_check = node_to_check
-    self.parent_stack = []
-    self.correct_parent = None
-
-  def generic_visit(self, node):
-    """Called if no explicit visitor function exists for a node."""
-    if self.correct_parent:
-      return node
-    if node == self.node_to_check:
-      self.correct_parent = self.parent_stack.pop()
-    self.parent_stack.append(node)
-    super(_ParentVisitor, self).generic_visit(node)
-    self.parent_stack.pop()
-
-
-def GetParentNode(module_node, node_in_stmt):
-  visitor = _ParentVisitor(node_in_stmt)
-  visitor.visit(module_node)
-  return visitor.correct_parent
+# def GetParentNode(module_node, node_in_stmt):
+#   visitor = _ParentVisitor(node_in_stmt)
+#   visitor.visit(module_node)
+#   return visitor.correct_parent
 
 
 def NodeCopy(node_to_copy):
   """Copies the node by recursively copying its fields."""
   if not isinstance(node_to_copy, _ast.AST):
     if isinstance(node_to_copy, list):
       new_list = []
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/common_utils/stack.py` & `fun_with_ast-0.1.70/fun_with_ast/common_utils/stack.py`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/common_utils/utils_source_match.py` & `fun_with_ast-0.1.70/fun_with_ast/common_utils/utils_source_match.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 
 
-def GetDefaultQuoteType():
-    return '"'
 
 def _GetListDefault(l, index, default):
     if index < len(l):
         return l[index]
     else:
         return default.Copy()
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/get_source.py` & `fun_with_ast-0.1.70/fun_with_ast/get_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,27 +53,22 @@
         if (assume_elif or (hasattr(field, 'is_alif') and field.is_alif)):
             field.matcher.is_elif = assume_elif
 
 
 def _match_text(assume_no_indent, field, text, parent_node):
     if text:
         field.matcher._match(text)
-    # TODO: Fix this to work with lambdas
-#    elif isinstance(field, ast.Module):
-#        raise NotImplementedError('Not supported: cannot match module node without input text')
     elif isinstance(field, _ast.stmt) and not assume_no_indent:
 #       if not hasattr(field, 'module_node'):
         if not isinstance(parent_node, ast.Module):
             raise ValueError(
                 'No text was provided, and we try to get source from node {} which'
                 'is a statement, so it must have a .module_node field defined. '
                 'To add this automatically, call ast_annotate.AddBasicAnnotations'
                 .format(field))
-        #raise NotImplementedError('Not clear if we ever get here')
-#        FixSourceIndentation(field.module_node, field)
 
 
 def _guess_base_from_string(string, field):
     if string.startswith('0x'):
         return 16
     if string.startswith('0b'):
         return 2
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/body_manipulator.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/body_manipulator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 10:11:08 2023 UTC, .py size: 2630 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3caa 9e64 460a 0000  o.......<..dF...
+00000000: 6f0d 0d0a 0000 0000 ffae aa64 4e0a 0000  o..........dN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 8302 5a08 6407 5300  d.d...d...Z.d.S.
 00000070: 2908 e900 0000 0029 01da 0d49 7345 6d70  )......)...IsEmp
@@ -186,14 +186,14 @@
 00000b90: 09da 2866 756e 5f77 6974 685f 6173 742e  ..(fun_with_ast.
 00000ba0: 636f 6d6d 6f6e 5f75 7469 6c73 2e6e 6f64  common_utils.nod
 00000bb0: 655f 7472 6565 5f75 7469 6c72 0200 0000  e_tree_utilr....
 00000bc0: da17 6675 6e5f 7769 7468 5f61 7374 2e67  ..fun_with_ast.g
 00000bd0: 6574 5f73 6f75 7263 6572 0300 0000 da1c  et_sourcer......
 00000be0: 6675 6e5f 7769 7468 5f61 7374 2e6d 616e  fun_with_ast.man
 00000bf0: 6970 756c 6174 655f 6e6f 6465 7204 0000  ipulate_noder...
-00000c00: 00da 2866 756e 5f77 6974 685f 6173 742e  ..(fun_with_ast.
+00000c00: 00da 3066 756e 5f77 6974 685f 6173 742e  ..0fun_with_ast.
 00000c10: 6d61 6e69 7075 6c61 7465 5f6e 6f64 652e  manipulate_node.
-00000c20: 6372 6561 7465 5f6e 6f64 6572 0500 0000  create_noder....
-00000c30: 7206 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000c40: 0a00 0000 720b 0000 00da 083c 6d6f 6475  ....r......<modu
-00000c50: 6c65 3e01 0000 0073 0a00 0000 0c00 0c01  le>....s........
-00000c60: 0c01 0c01 1203                           ......
+00000c20: 6765 745f 6e6f 6465 5f66 726f 6d5f 696e  get_node_from_in
+00000c30: 7075 7472 0500 0000 7206 0000 0072 0a00  putr....r....r..
+00000c40: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000c50: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000c60: 0a00 0000 0c00 0c01 0c01 0c01 1203       ..............
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/create_node.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/create_node.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 13:14:32 2023 UTC, .py size: 32763 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,1973 +1,1880 @@
-00000000: 6f0d 0d0a 0000 0000 38d5 9e64 fb7f 0000  o.......8..d....
+00000000: 6f0d 0d0a 0000 0000 cfc9 ae64 ee7a 0000  o..........d.z..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 d403 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 b203 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
-00000050: 6503 8303 5a04 4700 6404 6405 8400 6405  e...Z.G.d.d...d.
-00000060: 6504 8303 5a05 6406 6407 8400 5a06 6506  e...Z.d.d...Z.e.
-00000070: 6408 6409 640a 640b 640c 8d04 5a07 64cc  d.d.d.d.d...Z.d.
-00000080: 640e 640f 8401 5a08 6410 6411 8400 5a09  d.d...Z.d.d...Z.
-00000090: 6412 6413 8400 5a0a 6507 6a0b 6601 6414  d.d...Z.e.j.f.d.
-000000a0: 6415 8401 5a0c 6507 6a0b 6601 6416 6417  d...Z.e.j.f.d.d.
-000000b0: 8401 5a0d 6418 6419 8400 5a0e 641a 641b  ..Z.d.d...Z.d.d.
-000000c0: 8400 5a0f 4700 641c 641d 8400 641d 6501  ..Z.G.d.d...d.e.
-000000d0: 6a10 8303 5a11 641e 641f 8400 5a12 6700  j...Z.d.d...Z.g.
-000000e0: 6700 6401 6700 6700 6401 6700 6607 6420  g.d.g.g.d.g.f.d 
-000000f0: 6421 8401 5a13 6422 6423 8400 5a14 6424  d!..Z.d"d#..Z.d$
-00000100: 6425 8400 5a15 64cd 6426 6427 8401 5a16  d%..Z.d.d&d'..Z.
-00000110: 6428 6429 8400 5a17 642a 642b 8400 5a18  d(d)..Z.d*d+..Z.
-00000120: 642c 642d 8400 5a19 642e 642f 8400 5a1a  d,d-..Z.d.d/..Z.
-00000130: 6430 6431 8400 5a1b 6432 6433 8400 5a1c  d0d1..Z.d2d3..Z.
-00000140: 6434 6435 8400 5a1d 6436 6437 8400 5a1e  d4d5..Z.d6d7..Z.
-00000150: 6700 6700 6401 6900 6604 6438 6439 8401  g.g.d.i.f.d8d9..
-00000160: 5a1f 6700 6700 6700 6401 6401 6700 6606  Z.g.g.g.d.d.g.f.
-00000170: 643a 643b 8401 5a20 643c 643d 8400 5a21  d:d;..Z d<d=..Z!
-00000180: 643e 643f 8400 5a22 64ce 6441 6442 8401  d>d?..Z"d.dAdB..
-00000190: 5a23 6400 6443 9c01 6444 6445 8402 5a24  Z#d.dC..dDdE..Z$
-000001a0: 6446 6447 8400 5a25 6448 6449 8400 5a26  dFdG..Z%dHdI..Z&
-000001b0: 64cf 644a 644b 8401 5a27 644c 644d 8400  d.dJdK..Z'dLdM..
-000001c0: 5a28 644e 644f 8400 5a29 6401 6700 6700  Z(dNdO..Z)d.g.g.
-000001d0: 6401 6401 6605 6450 6451 8401 5a2a 6452  d.d.f.dPdQ..Z*dR
-000001e0: 6453 8400 5a2b 6454 6455 8400 5a2c 6456  dS..Z+dTdU..Z,dV
-000001f0: 6457 8400 5a2d 64cd 6458 6459 8401 5a2e  dW..Z-d.dXdY..Z.
-00000200: 645a 645b 8400 5a2f 64d0 645d 645e 8401  dZd[..Z/d.d]d^..
-00000210: 5a30 645f 6460 8400 5a31 6461 6462 8400  Z0d_d`..Z1dadb..
-00000220: 5a32 6463 6464 8400 5a33 6465 6466 8400  Z2dcdd..Z3dedf..
-00000230: 5a34 6467 6468 8400 5a35 6700 6601 6469  Z4dgdh..Z5g.f.di
-00000240: 646a 8401 5a36 646b 646c 8400 5a37 646d  dj..Z6dkdl..Z7dm
-00000250: 646e 8400 5a38 646f 6470 8400 5a39 6471  dn..Z8dodp..Z9dq
-00000260: 6472 8400 5a3a 6473 6474 8400 5a3b 6475  dr..Z:dsdt..Z;du
-00000270: 6476 8400 5a3c 6477 6478 8400 5a3d 6479  dv..Z<dwdx..Z=dy
-00000280: 647a 8400 5a3e 647b 647c 8400 5a3f 647d  dz..Z>d{d|..Z?d}
-00000290: 647e 8400 5a40 647f 6480 8400 5a41 6507  d~..Z@d.d...ZAe.
-000002a0: 6a0b 6601 6481 6482 8401 5a42 6483 6484  j.f.d.d...ZBd.d.
-000002b0: 8400 5a43 6485 6486 8400 5a44 6487 6488  ..ZCd.d...ZDd.d.
-000002c0: 8400 5a45 6489 648a 8400 5a46 648b 648c  ..ZEd.d...ZFd.d.
-000002d0: 8400 5a47 648d 648e 8400 5a48 648f 6490  ..ZGd.d...ZHd.d.
-000002e0: 8400 5a49 6491 6492 8400 5a4a 6493 6494  ..ZId.d...ZJd.d.
-000002f0: 8400 5a4b 6495 6496 8400 5a4c 6497 6498  ..ZKd.d...ZLd.d.
-00000300: 8400 5a4d 6499 649a 8400 5a4e 649b 649c  ..ZMd.d...ZNd.d.
-00000310: 8400 5a4f 64cf 649d 649e 8401 5a50 649f  ..ZOd.d.d...ZPd.
-00000320: 64a0 8400 5a51 64a1 64a2 8400 5a52 64a3  d...ZQd.d...ZRd.
-00000330: 64a4 8400 5a53 6401 6401 6401 6507 6a0b  d...ZSd.d.d.e.j.
-00000340: 6604 64a5 64a6 8401 5a54 4700 64a7 64a8  f.d.d...ZTG.d.d.
-00000350: 8400 64a8 6500 6a55 8303 5a56 4700 64a9  ..d.e.jU..ZVG.d.
-00000360: 64aa 8400 64aa 6500 6a55 8303 5a57 64ab  d...d.e.jU..ZWd.
-00000370: 64ac 8400 5a58 6700 6700 6700 6603 64ad  d...ZXg.g.g.f.d.
-00000380: 64ae 8401 5a59 6700 6601 64af 64b0 8401  d...ZYg.f.d.d...
-00000390: 5a5a 64b1 64b2 8400 5a5b 64b3 64b4 8400  ZZd.d...Z[d.d...
-000003a0: 5a5c 64b5 64b6 8400 5a5d 64cd 64b7 64b8  Z\d.d...Z]d.d.d.
-000003b0: 8401 5a5e 64b9 64ba 8400 5a5f 64d1 64bc  ..Z^d.d...Z_d.d.
-000003c0: 64bd 8401 5a60 64be 64bf 8400 5a61 64c0  d...Z`d.d...Zad.
-000003d0: 64c1 8400 5a62 64c2 64c3 8400 5a63 64c4  d...Zbd.d...Zcd.
-000003e0: 64c5 8400 5a64 64c6 64c7 8400 5a65 64c8  d...Zdd.d...Zed.
-000003f0: 64c9 8400 5a66 64ca 64cb 8400 5a67 6401  d...Zfd.d...Zgd.
-00000400: 5300 29d2 e900 0000 004e 6300 0000 0000  S.)......Nc.....
-00000410: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000420: 0000 00f3 0c00 0000 6500 5a01 6400 5a02  ........e.Z.d.Z.
-00000430: 6401 5300 2902 da05 4572 726f 724e a903  d.S.)...ErrorN..
-00000440: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000450: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000460: 6d65 5f5f a900 7208 0000 0072 0800 0000  me__..r....r....
-00000470: fa43 2f68 6f6d 652f 7368 6169 2f66 756e  .C/home/shai/fun
-00000480: 5f77 6974 685f 6173 742f 6675 6e5f 7769  _with_ast/fun_wi
-00000490: 7468 5f61 7374 2f6d 616e 6970 756c 6174  th_ast/manipulat
-000004a0: 655f 6e6f 6465 2f63 7265 6174 655f 6e6f  e_node/create_no
-000004b0: 6465 2e70 7972 0300 0000 0800 0000 f304  de.pyr..........
-000004c0: 0000 0008 0004 0172 0300 0000 6300 0000  .......r....c...
-000004d0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-000004e0: 0040 0000 0072 0200 0000 2902 da0a 496e  .@...r....)...In
-000004f0: 7661 6c69 6443 7478 4e72 0400 0000 7208  validCtxNr....r.
-00000500: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00000510: 0000 720b 0000 000c 0000 0072 0a00 0000  ..r........r....
-00000520: 720b 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000530: 0000 0100 0000 0400 0000 4b00 0000 730c  ..........K...s.
-00000540: 0000 0074 0064 0164 027c 0083 0353 0029  ...t.d.d.|...S.)
-00000550: 034e da04 456e 756d 7208 0000 0029 01da  .N..Enumr....)..
-00000560: 0474 7970 6529 01da 0565 6e75 6d73 7208  .type)...enumsr.
-00000570: 0000 0072 0800 0000 7209 0000 0072 0c00  ...r....r....r..
-00000580: 0000 1000 0000 f302 0000 000c 0172 0c00  .............r..
-00000590: 0000 da04 6c6f 6164 da05 7374 6f72 65da  ....load..store.
-000005a0: 0664 656c 6574 65da 0570 6172 616d 2904  .delete..param).
-000005b0: da04 4c4f 4144 da05 5354 4f52 45da 0344  ..LOAD..STORE..D
-000005c0: 454c da05 5041 5241 4d46 6303 0000 0000  EL..PARAMFc.....
-000005d0: 0000 0000 0000 0005 0000 0003 0000 0043  ...............C
-000005e0: 0000 0073 6600 0000 7400 a001 7c00 a101  ...sf...t...|...
-000005f0: 7d03 7c03 6a02 7212 7c02 6401 6b02 7212  }.|.j.r.|.d.k.r.
-00000600: 7c03 6a02 7c01 1900 7d04 6e0c 7c03 6a02  |.j.|...}.n.|.j.
-00000610: 721c 7c02 6402 6b02 721c 7c03 7d04 6e02  r.|.d.k.r.|.}.n.
-00000620: 7c03 5300 7403 7c04 7400 6a04 8302 7231  |.S.t.|.t.j...r1
-00000630: 6403 7c00 7600 7231 6403 7c00 7600 722e  d.|.v.r1d.|.v.r.
-00000640: 6402 6e01 6401 7c04 5f05 7c04 5300 2904  d.n.d.|._.|.S.).
-00000650: 4e46 54da 0465 6c69 6629 06da 0361 7374  NFT..elif)...ast
-00000660: da05 7061 7273 65da 0462 6f64 79da 0a69  ..parse..body..i
-00000670: 7369 6e73 7461 6e63 65da 0249 66da 0769  sinstance..If..i
-00000680: 735f 656c 6966 2905 da06 7374 7269 6e67  s_elif)...string
-00000690: da0a 626f 6479 5f69 6e64 6578 da0a 6765  ..body_index..ge
-000006a0: 745f 6d6f 6475 6c65 da0c 7061 7273 655f  t_module..parse_
-000006b0: 7265 7375 6c74 da04 6e6f 6465 7208 0000  result..noder...
-000006c0: 0072 0800 0000 7209 0000 00da 1047 6574  .r....r......Get
-000006d0: 4e6f 6465 4672 6f6d 496e 7075 741a 0000  NodeFromInput...
-000006e0: 0073 1200 0000 0a01 0e01 0c01 0e01 0601  .s..............
-000006f0: 0402 1401 1201 0401 7224 0000 0063 0200  ........r$...c..
-00000700: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-00000710: 0000 4300 0000 7378 0000 0074 007c 0074  ..C...sx...t.|.t
-00000720: 0183 0273 0974 0264 0183 0182 0174 007c  ...s.t.d.....t.|
-00000730: 0174 0183 0273 1274 0264 0283 0182 0167  .t...s.t.d.....g
-00000740: 007d 0267 007d 037c 0044 005d 077d 047c  .}.g.}.|.D.].}.|
-00000750: 02a0 037c 04a1 0101 0071 187c 0144 005d  ...|.....q.|.D.]
-00000760: 077d 057c 03a0 037c 05a1 0101 0071 2264  .}.|...|.....q"d
-00000770: 0364 0484 007c 0244 0083 017d 0264 0564  .d...|.D...}.d.d
-00000780: 0484 007c 0344 0083 017d 037c 027c 0366  ...|.D...}.|.|.f
-00000790: 0253 0029 064e fa13 6172 6773 206d 7573  .S.).N..args mus
-000007a0: 7420 6265 2061 206c 6973 747a 1764 6566  t be a listz.def
-000007b0: 6175 6c74 7320 6d75 7374 2062 6520 6120  aults must be a 
-000007c0: 6c69 7374 6301 0000 0000 0000 0000 0000  listc...........
-000007d0: 0002 0000 0004 0000 0053 0000 00f3 1400  .........S......
-000007e0: 0000 6700 7c00 5d06 7d01 7400 7c01 8301  ..g.|.].}.t.|...
-000007f0: 9102 7102 5300 7208 0000 0029 01da 0d5f  ..q.S.r....)..._
-00000800: 5772 6170 5769 7468 4172 6773 a902 da02  WrapWithArgs....
-00000810: 2e30 da03 6172 6772 0800 0000 7208 0000  .0..argr....r...
-00000820: 0072 0900 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00000830: 703e 3200 0000 f302 0000 0014 007a 275f  p>2..........z'_
-00000840: 546f 4172 6773 5769 7468 4465 6661 756c  ToArgsWithDefaul
-00000850: 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ts.<locals>.<lis
-00000860: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
-00000870: 0000 0002 0000 0004 0000 0053 0000 0072  ...........S...r
-00000880: 2600 0000 7208 0000 00a9 01da 0d5f 5772  &...r........_Wr
-00000890: 6170 5769 7468 4e61 6d65 2902 7229 0000  apWithName).r)..
-000008a0: 00da 0764 6566 6175 6c74 7208 0000 0072  ...defaultr....r
-000008b0: 0800 0000 7209 0000 0072 2b00 0000 3300  ....r....r+...3.
-000008c0: 0000 722c 0000 0029 0472 1c00 0000 da04  ..r,...).r......
-000008d0: 6c69 7374 da0a 5661 6c75 6545 7272 6f72  list..ValueError
-000008e0: da06 6170 7065 6e64 2906 da05 5f61 7267  ..append)..._arg
-000008f0: 73da 095f 6465 6661 756c 7473 da04 6172  s.._defaults..ar
-00000900: 6773 da08 6465 6661 756c 7473 722a 0000  gs..defaultsr*..
-00000910: 0072 2f00 0000 7208 0000 0072 0800 0000  .r/...r....r....
-00000920: 7209 0000 00da 135f 546f 4172 6773 5769  r......_ToArgsWi
-00000930: 7468 4465 6661 756c 7473 2700 0000 731a  thDefaults'...s.
-00000940: 0000 000a 0108 010a 0108 0104 0104 0108  ................
-00000950: 010c 0108 010c 010e 010e 0108 0172 3700  .............r7.
-00000960: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000970: 0000 0003 0000 0043 0000 0073 1800 0000  .......C...s....
-00000980: 7400 7c00 7401 6a02 8302 7208 7c00 5300  t.|.t.j...r.|.S.
-00000990: 7403 7c00 8301 5300 a901 4e29 0472 1c00  t.|...S...N).r..
-000009a0: 0000 da04 5f61 7374 da03 4153 54da 0341  ...._ast..AST..A
-000009b0: 7267 2901 da07 746f 5f77 7261 7072 0800  rg)...to_wrapr..
-000009c0: 0000 7208 0000 0072 0900 0000 7227 0000  ..r....r....r'..
-000009d0: 0037 0000 0073 0600 0000 0c01 0401 0801  .7...s..........
-000009e0: 7227 0000 0063 0200 0000 0000 0000 0000  r'...c..........
-000009f0: 0000 0200 0000 0400 0000 4300 0000 733c  ..........C...s<
-00000a00: 0000 0074 007c 0074 016a 0283 0272 087c  ...t.|.t.j...r.|
-00000a10: 0053 0074 007c 0074 0383 0272 1174 047c  .S.t.|.t...r.t.|
-00000a20: 0083 0153 0074 007c 0074 0583 0272 1c74  ...S.t.|.t...r.t
-00000a30: 067c 007c 0164 018d 0253 0074 0782 01a9  .|.|.d...S.t....
-00000a40: 024e a901 da08 6374 785f 7479 7065 2908  .N....ctx_type).
-00000a50: 721c 0000 0072 3900 0000 723a 0000 00da  r....r9...r:....
-00000a60: 0369 6e74 da08 436f 6e73 7461 6e74 da03  .int..Constant..
-00000a70: 7374 72da 044e 616d 65da 134e 6f74 496d  str..Name..NotIm
-00000a80: 706c 656d 656e 7465 6445 7272 6f72 a902  plementedError..
-00000a90: 723c 0000 0072 3f00 0000 7208 0000 0072  r<...r?...r....r
-00000aa0: 0800 0000 7209 0000 0072 2e00 0000 3d00  ....r....r....=.
-00000ab0: 0000 730e 0000 000c 0104 010a 0108 010a  ..s.............
-00000ac0: 010c 0104 0172 2e00 0000 6302 0000 0000  .....r....c.....
-00000ad0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000ae0: 0000 0073 1a00 0000 7400 7c00 7401 8302  ...s....t.|.t...
-00000af0: 7307 7402 8201 7403 7c00 7c01 6401 8d02  s.t...t.|.|.d...
-00000b00: 5300 723d 0000 0029 0472 1c00 0000 7230  S.r=...).r....r0
-00000b10: 0000 0072 4400 0000 da05 5475 706c 6572  ...rD.....Tupler
-00000b20: 4500 0000 7208 0000 0072 0800 0000 7209  E...r....r....r.
-00000b30: 0000 00da 0e5f 5772 6170 5769 7468 5475  ....._WrapWithTu
-00000b40: 706c 6547 0000 0073 0600 0000 0a01 0401  pleG...s........
-00000b50: 0c01 7247 0000 0063 0100 0000 0000 0000  ..rG...c........
-00000b60: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-00000b70: 732c 0000 0074 007c 0064 0183 0273 1474  s,...t.|.d...s.t
-00000b80: 007c 0064 0283 0273 0c7c 0053 007c 006a  .|.d...s.|.S.|.j
-00000b90: 017d 0074 007c 0064 0183 0272 057c 0053  .}.t.|.d...r.|.S
-00000ba0: 0029 034e da02 6964 da05 7661 6c75 6529  .).N..id..value)
-00000bb0: 02da 0768 6173 6174 7472 7249 0000 0029  ...hasattrrI...)
-00000bc0: 0172 2300 0000 7208 0000 0072 0800 0000  .r#...r....r....
-00000bd0: 7209 0000 00da 155f 4c65 6674 6d6f 7374  r......_Leftmost
-00000be0: 4e6f 6465 496e 446f 7456 6172 4d00 0000  NodeInDotVarM...
-00000bf0: 730c 0000 000a 010a 0104 0106 010a fd04  s...............
-00000c00: 0472 4b00 0000 6301 0000 0000 0000 0000  .rK...c.........
-00000c10: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-00000c20: 3800 0000 7c00 6400 7500 7208 7400 8300  8...|.d.u.r.t...
-00000c30: 6701 7d00 7c00 4400 5d0f 7d01 7401 7c01  g.}.|.D.].}.t.|.
-00000c40: 7402 6a03 8302 7319 7404 6401 a005 7c01  t.j...s.t.d...|.
-00000c50: a101 8301 8201 710a 7c00 5300 2902 4efa  ......q.|.S.).N.
-00000c60: 5941 6c6c 2062 6f64 7920 6e6f 6465 7320  YAll body nodes 
-00000c70: 6d75 7374 2062 6520 7374 6d74 206e 6f64  must be stmt nod
-00000c80: 6573 2c20 616e 6420 7b7d 2069 7320 6e6f  es, and {} is no
-00000c90: 742e 2054 7279 2077 7261 7070 696e 6720  t. Try wrapping 
-00000ca0: 796f 7572 206e 6f64 6520 696e 2061 6e20  your node in an 
-00000cb0: 4578 7072 206e 6f64 652e 2906 da04 5061  Expr node.)...Pa
-00000cc0: 7373 721c 0000 0072 3900 0000 da04 7374  ssr....r9.....st
-00000cd0: 6d74 7231 0000 00da 0666 6f72 6d61 7429  mtr1.....format)
-00000ce0: 0272 1b00 0000 da05 6368 696c 6472 0800  .r......childr..
-00000cf0: 0000 7208 0000 0072 0900 0000 da15 466f  ..r....r......Fo
-00000d00: 726d 6174 416e 6456 616c 6964 6174 6542  rmatAndValidateB
-00000d10: 6f64 7955 0000 0073 1400 0000 0801 0801  odyU...s........
-00000d20: 0801 0c01 0201 0201 0602 04fd 02ff 0405  ................
-00000d30: 7251 0000 0063 0000 0000 0000 0000 0000  rQ...c..........
-00000d40: 0000 0000 0000 0300 0000 0000 0000 7328  ..............s(
-00000d50: 0000 0065 005a 0164 005a 0287 0066 0164  ...e.Z.d.Z...f.d
-00000d60: 0164 0284 085a 0387 0066 0164 0364 0484  .d...Z...f.d.d..
-00000d70: 085a 0487 0004 005a 0553 0029 05da 1243  .Z.....Z.S.)...C
-00000d80: 6861 6e67 6543 7478 5472 616e 7366 6f72  hangeCtxTransfor
-00000d90: 6d63 0200 0000 0000 0000 0000 0000 0200  mc..............
-00000da0: 0000 0300 0000 0300 0000 7318 0000 0074  ..........s....t
-00000db0: 0074 017c 0083 02a0 02a1 0001 007c 017c  .t.|.........|.|
-00000dc0: 005f 0364 0053 0072 3800 0000 2904 da05  ._.d.S.r8...)...
-00000dd0: 7375 7065 7272 5200 0000 da08 5f5f 696e  superrR.....__in
-00000de0: 6974 5f5f da0d 5f6e 6577 5f63 7478 5f74  it__.._new_ctx_t
-00000df0: 7970 6529 02da 0473 656c 66da 0c6e 6577  ype)...self..new
-00000e00: 5f63 7478 5f74 7970 65a9 01da 095f 5f63  _ctx_type....__c
-00000e10: 6c61 7373 5f5f 7208 0000 0072 0900 0000  lass__r....r....
-00000e20: 7254 0000 0063 0000 0073 0400 0000 0e01  rT...c...s......
-00000e30: 0a01 7a1b 4368 616e 6765 4374 7854 7261  ..z.ChangeCtxTra
-00000e40: 6e73 666f 726d 2e5f 5f69 6e69 745f 5f63  nsform.__init__c
-00000e50: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000e60: 0300 0000 0300 0000 732a 0000 0074 0074  ........s*...t.t
-00000e70: 017c 0083 02a0 027c 01a1 017d 0174 037c  .|.....|...}.t.|
-00000e80: 0164 0183 0272 1374 047c 006a 0583 017c  .d...r.t.|.j...|
-00000e90: 015f 067c 0153 0029 024e da03 6374 7829  ._.|.S.).N..ctx)
-00000ea0: 0772 5300 0000 7252 0000 00da 0d67 656e  .rS...rR.....gen
-00000eb0: 6572 6963 5f76 6973 6974 724a 0000 00da  eric_visitrJ....
-00000ec0: 0647 6574 4374 7872 5500 0000 725a 0000  .GetCtxrU...rZ..
-00000ed0: 0029 0272 5600 0000 7223 0000 0072 5800  .).rV...r#...rX.
-00000ee0: 0000 7208 0000 0072 0900 0000 725b 0000  ..r....r....r[..
-00000ef0: 0067 0000 0073 0800 0000 1001 0a01 0c01  .g...s..........
-00000f00: 0401 7a20 4368 616e 6765 4374 7854 7261  ..z ChangeCtxTra
-00000f10: 6e73 666f 726d 2e67 656e 6572 6963 5f76  nsform.generic_v
-00000f20: 6973 6974 2906 7205 0000 0072 0600 0000  isit).r....r....
-00000f30: 7207 0000 0072 5400 0000 725b 0000 00da  r....rT...r[....
-00000f40: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7208  .__classcell__r.
-00000f50: 0000 0072 0800 0000 7258 0000 0072 0900  ...r....rX...r..
-00000f60: 0000 7252 0000 0061 0000 0073 0600 0000  ..rR...a...s....
-00000f70: 0800 0c02 1404 7252 0000 0063 0200 0000  ......rR...c....
-00000f80: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00000f90: 4300 0000 7316 0000 0074 007c 0183 017d  C...s....t.|...}
-00000fa0: 027c 02a0 017c 00a1 0101 0064 0053 0072  .|...|.....d.S.r
-00000fb0: 3800 0000 2902 7252 0000 00da 0576 6973  8...).rR.....vis
-00000fc0: 6974 2903 7223 0000 0072 5700 0000 da09  it).r#...rW.....
-00000fd0: 7472 616e 7366 6f72 6d72 0800 0000 7208  transformr....r.
-00000fe0: 0000 0072 0900 0000 da09 4368 616e 6765  ...r......Change
-00000ff0: 4374 786e 0000 0073 0400 0000 0801 0e01  Ctxn...s........
-00001000: 7260 0000 0063 0700 0000 0000 0000 0000  r`...c..........
-00001010: 0000 0700 0000 0900 0000 4300 0000 7350  ..........C...sP
-00001020: 0000 0074 007c 0174 0183 0273 0974 0264  ...t.|.t...s.t.d
-00001030: 0183 0182 017c 0572 0f74 037c 0583 017d  .....|.r.t.|...}
-00001040: 057c 0272 1574 037c 0283 017d 0274 047c  .|.r.t.|...}.t.|
-00001050: 017c 0683 025c 027d 017d 0674 056a 067c  .|...\.}.}.t.j.|
-00001060: 007c 017c 027c 037c 047c 057c 0664 028d  .|.|.|.|.|.|.d..
-00001070: 0753 0029 0361 8d01 0000 4372 6561 7465  .S.).a....Create
-00001080: 7320 616e 205f 6173 742e 4675 6e63 7469  s an _ast.Functi
-00001090: 6f6e 4465 6620 6e6f 6465 2e0a 0a20 2041  onDef node...  A
-000010a0: 7267 733a 0a20 2020 2061 7267 733a 2041  rgs:.    args: A
-000010b0: 206c 6973 7420 6f66 2061 7267 732e 0a20   list of args.. 
-000010c0: 2020 206b 6579 733a 2041 206c 6973 7420     keys: A list 
-000010d0: 6f66 206b 6579 732c 206d 7573 7420 6265  of keys, must be
-000010e0: 2074 6865 2073 616d 6520 6c65 6e67 7468   the same length
-000010f0: 2061 7320 7661 6c75 6573 2e0a 2020 2020   as values..    
-00001100: 7661 6c75 6573 3a20 4120 6c69 7374 206f  values: A list o
-00001110: 6620 7661 6c75 6573 2c20 636f 7272 6573  f values, corres
-00001120: 706f 6e64 2074 6f20 6b65 7973 2e0a 2020  pond to keys..  
-00001130: 2020 7661 7261 7267 5f6e 616d 653a 2054    vararg_name: T
-00001140: 6865 206e 616d 6520 6f66 2074 6865 2076  he name of the v
-00001150: 6172 6172 6720 7661 7269 6162 6c65 2c20  ararg variable, 
-00001160: 6f72 204e 6f6e 652e 0a20 2020 206b 7761  or None..    kwa
-00001170: 7267 5f6e 616d 653a 2054 6865 206e 616d  rg_name: The nam
-00001180: 6520 6f66 2074 6865 206b 7761 7267 7320  e of the kwargs 
-00001190: 7661 7269 6162 6c65 2c20 6f72 204e 6f6e  variable, or Non
-000011a0: 652e 0a0a 2020 5261 6973 6573 3a0a 2020  e...  Raises:.  
-000011b0: 2020 5661 6c75 6545 7272 6f72 3a20 4966    ValueError: If
-000011c0: 206c 656e 286b 6579 7329 2021 3d20 6c65   len(keys) != le
-000011d0: 6e28 7661 6c75 6573 292e 0a0a 2020 5265  n(values)...  Re
-000011e0: 7475 726e 733a 0a20 2020 2041 6e20 5f61  turns:.    An _a
-000011f0: 7374 2e46 756e 6374 696f 6e44 6566 206e  st.FunctionDef n
-00001200: 6f64 652e 0a20 2072 2500 0000 a907 da0b  ode..  r%.......
-00001210: 706f 736f 6e6c 7961 7267 7372 3500 0000  posonlyargsr5...
-00001220: da06 7661 7261 7267 da0a 6b77 6f6e 6c79  ..vararg..kwonly
-00001230: 6172 6773 da0b 6b77 5f64 6566 6175 6c74  args..kw_default
-00001240: 73da 056b 7761 7267 7236 0000 0029 0772  s..kwargr6...).r
-00001250: 1c00 0000 7230 0000 0072 3100 0000 7227  ....r0...r1...r'
-00001260: 0000 0072 3700 0000 7239 0000 00da 0961  ...r7...r9.....a
-00001270: 7267 756d 656e 7473 7261 0000 0072 0800  rgumentsra...r..
-00001280: 0000 7208 0000 0072 0900 0000 7267 0000  ..r....r....rg..
-00001290: 0078 0000 0073 2000 0000 0a10 0801 0401  .x...s .........
-000012a0: 0801 0401 0801 0e01 0401 0201 0201 0201  ................
-000012b0: 0201 0201 0201 0201 06f9 7267 0000 0063  ..........rg...c
-000012c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000012d0: 0200 0000 4300 0000 f308 0000 0074 00a0  ....C........t..
-000012e0: 01a1 0053 0072 3800 0000 2902 7239 0000  ...S.r8...).r9..
-000012f0: 00da 0341 6464 7208 0000 0072 0800 0000  ...Addr....r....
-00001300: 7208 0000 0072 0900 0000 7269 0000 0099  r....r....ri....
-00001310: 0000 00f3 0200 0000 0801 7269 0000 0063  ..........ri...c
-00001320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001330: 0200 0000 4300 0000 7268 0000 0072 3800  ....C...rh...r8.
-00001340: 0000 2902 7239 0000 00da 0341 6e64 7208  ..).r9.....Andr.
-00001350: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00001360: 0000 726b 0000 009d 0000 0072 6a00 0000  ..rk.......rj...
-00001370: 726b 0000 0063 0200 0000 0000 0000 0000  rk...c..........
-00001380: 0000 0200 0000 0400 0000 4300 0000 730e  ..........C...s.
-00001390: 0000 0074 006a 017c 007c 0164 018d 0253  ...t.j.|.|.d...S
-000013a0: 0029 024e 2902 da04 7465 7374 da03 6d73  .).N)...test..ms
-000013b0: 6729 0272 3900 0000 da06 4173 7365 7274  g).r9.....Assert
-000013c0: 2902 da05 6368 6563 6bda 076d 6573 7361  )...check..messa
-000013d0: 6765 7208 0000 0072 0800 0000 7209 0000  ger....r....r...
-000013e0: 0072 6e00 0000 a100 0000 7302 0000 000e  .rn.......s.....
-000013f0: 0172 6e00 0000 6302 0000 0000 0000 0000  .rn...c.........
-00001400: 0000 0007 0000 0007 0000 0043 0000 0073  ...........C...s
-00001410: 7200 0000 7400 7c00 7401 7402 6602 8302  r...t.|.t.t.f...
-00001420: 730b 7c00 6701 7d02 6e02 7c00 7d02 6700  s.|.g.}.n.|.}.g.
-00001430: 7d03 7c02 4400 5d17 7d04 7400 7c04 7403  }.|.D.].}.t.|.t.
-00001440: 8302 7223 7c03 a004 7405 7c04 7406 6a07  ..r#|...t.|.t.j.
-00001450: 6401 8d02 a101 0100 7111 7c03 a004 7c04  d.......q.|...|.
-00001460: a101 0100 7111 7408 7c01 8301 7d05 7409  ....q.t.|...}.t.
-00001470: 6a0a 7c03 7c01 6402 8d02 7d06 7c05 7c06  j.|.|.d...}.|.|.
-00001480: 5f0b 7c06 5300 2903 6123 0100 0043 7265  _.|.S.).a#...Cre
-00001490: 6174 6573 2061 6e20 5f61 7374 2e41 7373  ates an _ast.Ass
-000014a0: 6967 6e20 6e6f 6465 2e0a 0a20 2041 7267  ign node...  Arg
-000014b0: 733a 0a20 2020 206c 6566 743a 2054 6865  s:.    left: The
-000014c0: 206e 6f64 6520 6f6e 2074 6865 206c 6566   node on the lef
-000014d0: 7420 7369 6465 206f 6620 7468 6520 6571  t side of the eq
-000014e0: 7561 6c20 7369 676e 2e0a 2020 2020 2020  ual sign..      
-000014f0: 4d61 7920 6569 7468 6572 2062 6520 6120  May either be a 
-00001500: 6e6f 6465 2c20 6f72 2061 2073 7472 696e  node, or a strin
-00001510: 672c 2077 6869 6368 2077 696c 6c20 6175  g, which will au
-00001520: 746f 6d61 7469 6361 6c6c 7920 6765 740a  tomatically get.
-00001530: 2020 2020 2020 636f 6e76 6572 7465 6420        converted 
-00001540: 746f 2061 206e 616d 6520 6e6f 6465 2e0a  to a name node..
-00001550: 2020 2020 7269 6768 743a 2054 6865 206e      right: The n
-00001560: 6f64 6520 6f6e 2074 6865 2072 6967 6874  ode on the right
-00001570: 2073 6964 6520 6f66 2074 6865 2065 7175   side of the equ
-00001580: 616c 2073 6967 6e2e 0a0a 2020 5265 7475  al sign...  Retu
-00001590: 726e 733a 0a20 2020 2041 6e20 5f61 7374  rns:.    An _ast
-000015a0: 2e41 7373 6967 6e20 6e6f 6465 2e0a 2020  .Assign node..  
-000015b0: 723e 0000 0029 02da 0774 6172 6765 7473  r>...)...targets
-000015c0: 7249 0000 0029 0c72 1c00 0000 7230 0000  rI...).r....r0..
-000015d0: 00da 0574 7570 6c65 7242 0000 0072 3200  ...tuplerB...r2.
-000015e0: 0000 722e 0000 00da 0743 7478 456e 756d  ..r......CtxEnum
-000015f0: 7215 0000 00da 0d5f 6578 7472 6163 745f  r......_extract_
-00001600: 6261 7365 7239 0000 00da 0641 7373 6967  baser9.....Assig
-00001610: 6eda 0462 6173 6529 07da 046c 6566 74da  n..base)...left.
-00001620: 0572 6967 6874 7271 0000 00da 0b6e 6577  .rightrq.....new
-00001630: 5f74 6172 6765 7473 da06 7461 7267 6574  _targets..target
-00001640: 7276 0000 00da 0672 6573 756c 7472 0800  rv.....resultr..
-00001650: 0000 7208 0000 0072 0900 0000 7275 0000  ..r....r....ru..
-00001660: 00a5 0000 0073 1e00 0000 0e0c 0801 0402  .....s..........
-00001670: 0401 0801 0a01 1601 0c02 0801 0401 0201  ................
-00001680: 0201 06fe 0603 0401 7275 0000 0063 0300  ........ru...c..
-00001690: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-000016a0: 0000 4300 0000 7318 0000 0074 007c 0083  ..C...s....t.|..
-000016b0: 017d 0074 016a 027c 007c 017c 0264 018d  .}.t.j.|.|.|.d..
-000016c0: 0353 0029 0261 3701 0000 4372 6561 7465  .S.).a7...Create
-000016d0: 7320 616e 205f 6173 742e 4175 6741 7373  s an _ast.AugAss
-000016e0: 6967 6e20 6e6f 6465 2e0a 0a20 2041 7267  ign node...  Arg
-000016f0: 733a 0a20 2020 206c 6566 743a 2054 6865  s:.    left: The
-00001700: 206e 6f64 6520 6f6e 2074 6865 206c 6566   node on the lef
-00001710: 7420 7369 6465 206f 6620 7468 6520 6571  t side of the eq
-00001720: 7561 6c20 7369 676e 2e0a 2020 2020 2020  ual sign..      
-00001730: 4d61 7920 6569 7468 6572 2062 6520 6120  May either be a 
-00001740: 6e6f 6465 2c20 6f72 2061 2073 7472 696e  node, or a strin
-00001750: 672c 2077 6869 6368 2077 696c 6c20 6175  g, which will au
-00001760: 746f 6d61 7469 6361 6c6c 7920 6765 740a  tomatically get.
-00001770: 2020 2020 2020 636f 6e76 6572 7465 6420        converted 
-00001780: 746f 2061 206e 616d 6520 6e6f 6465 2e0a  to a name node..
-00001790: 2020 2020 6f70 3a20 4f70 6572 6174 6f72      op: Operator
-000017a0: 0a20 2020 2072 6967 6874 3a20 5468 6520  .    right: The 
-000017b0: 6e6f 6465 206f 6e20 7468 6520 7269 6768  node on the righ
-000017c0: 7420 7369 6465 206f 6620 7468 6520 6571  t side of the eq
-000017d0: 7561 6c20 7369 676e 2e0a 0a20 2052 6574  ual sign...  Ret
-000017e0: 7572 6e73 3a0a 2020 2020 416e 205f 6173  urns:.    An _as
-000017f0: 742e 4173 7369 676e 206e 6f64 652e 0a20  t.Assign node.. 
-00001800: 2029 0372 7a00 0000 da02 6f70 7249 0000   ).rz.....oprI..
-00001810: 0029 0372 2e00 0000 7239 0000 00da 0941  .).r....r9.....A
-00001820: 7567 4173 7369 676e a903 7277 0000 0072  ugAssign..rw...r
-00001830: 7c00 0000 7278 0000 0072 0800 0000 7208  |...rx...r....r.
-00001840: 0000 0072 0900 0000 727d 0000 00c2 0000  ...r....r}......
-00001850: 0073 0c00 0000 080d 0401 0201 0201 0201  .s..............
-00001860: 06fd 727d 0000 0063 0300 0000 0000 0000  ..r}...c........
-00001870: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-00001880: 7324 0000 0074 007c 0174 016a 0283 0273  s$...t.|.t.j...s
-00001890: 0a74 037c 0183 017d 0174 016a 047c 007c  .t.|...}.t.j.|.|
-000018a0: 017c 0264 018d 0353 0029 027a fa43 7265  .|.d...S.).z.Cre
-000018b0: 6174 6573 2061 6e20 5f61 7374 2e42 696e  ates an _ast.Bin
-000018c0: 4f70 206e 6f64 652e 0a0a 2020 4172 6773  Op node...  Args
-000018d0: 3a0a 2020 2020 6c65 6674 3a20 5468 6520  :.    left: The 
-000018e0: 6e6f 6465 206f 6e20 7468 6520 6c65 6674  node on the left
-000018f0: 2073 6964 6520 6f66 2074 6865 2065 7175   side of the equ
-00001900: 616c 2073 6967 6e2e 0a20 2020 206f 703a  al sign..    op:
-00001910: 2054 6865 206f 7065 7261 746f 722e 204c   The operator. L
-00001920: 6974 6572 616c 2076 616c 7565 7320 6173  iteral values as
-00001930: 2073 7472 696e 6773 2061 6c73 6f20 6163   strings also ac
-00001940: 6365 7074 6564 3a0a 2020 2020 7269 6768  cepted:.    righ
-00001950: 743a 2054 6865 206e 6f64 6520 6f6e 2074  t: The node on t
-00001960: 6865 2072 6967 6874 2073 6964 6520 6f66  he right side of
-00001970: 2074 6865 2065 7175 616c 2073 6967 6e2e   the equal sign.
-00001980: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
-00001990: 2041 6e20 5f61 7374 2e42 696e 4f70 206e   An _ast.BinOp n
-000019a0: 6f64 652e 0a20 2072 7e00 0000 2905 721c  ode..  r~...).r.
-000019b0: 0000 0072 3900 0000 723a 0000 00da 0842  ...r9...r:.....B
-000019c0: 696e 4f70 4d61 70da 0542 696e 4f70 727e  inOpMap..BinOpr~
-000019d0: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-000019e0: 0000 7280 0000 00d6 0000 0073 0e00 0000  ..r........s....
-000019f0: 0c0b 0801 0402 0201 0201 0201 06fd 7280  ..............r.
-00001a00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001a10: 0700 0000 0500 0000 4700 0000 73d0 0000  ........G...s...
-00001a20: 007c 0067 017d 0264 017d 0364 027d 0474  .|.g.}.d.}.d.}.t
-00001a30: 007c 0183 017d 017c 0172 617c 01a0 0164  .|...}.|.ra|...d
-00001a40: 03a1 017d 057c 0472 5774 027c 0574 036a  ...}.|.rWt.|.t.j
-00001a50: 0483 0273 1e74 057c 0583 017d 057c 0373  ...s.t.|...}.|.s
-00001a60: 237c 057d 036e 397c 0372 2a7c 037c 056b  #|.}.n9|.r*|.|.k
-00001a70: 0272 2a71 0b74 027c 0374 036a 0683 0272  .r*q.t.|.t.j...r
-00001a80: 3e74 0774 036a 077c 037c 0264 048d 027c  >t.t.j.|.|.d...|
-00001a90: 0567 027c 01a2 0152 008e 0053 007c 02a0  .g.|...R...S.|..
-00001aa0: 01a1 007d 067c 02a0 0874 077c 067c 0567  ...}.|...t.|.|.g
-00001ab0: 027c 01a2 0152 008e 00a1 0101 0074 036a  .|...R.......t.j
-00001ac0: 0774 03a0 09a1 007c 0264 048d 0253 007c  .t.....|.d...S.|
-00001ad0: 02a0 087c 05a1 0101 007c 040c 007d 047c  ...|.....|...}.|
-00001ae0: 0173 0d74 036a 077c 037c 0264 048d 0253  .s.t.j.|.|.d...S
-00001af0: 0029 0561 5d01 0000 4372 6561 7465 7320  .).a]...Creates 
-00001b00: 616e 205f 6173 742e 426f 6f6c 4f70 206e  an _ast.BoolOp n
-00001b10: 6f64 652e 0a0a 2020 4172 6773 3a0a 2020  ode...  Args:.  
-00001b20: 2020 6c65 6674 3a20 5468 6520 6e6f 6465    left: The node
-00001b30: 206f 6e20 7468 6520 6c65 6674 2073 6964   on the left sid
-00001b40: 6520 6f66 2074 6865 2065 7175 616c 2073  e of the equal s
-00001b50: 6967 6e2e 0a20 2020 202a 616c 7465 726e  ign..    *altern
-00001b60: 6174 696e 675f 6f70 735f 7661 6c75 6573  ating_ops_values
-00001b70: 3a20 416e 2061 6c74 6572 6e61 7469 6e67  : An alternating
-00001b80: 206c 6973 7420 6f66 206f 7073 2061 6e64   list of ops and
-00001b90: 2065 7870 7265 7373 696f 6e73 2e0a 2020   expressions..  
-00001ba0: 2020 2020 4e6f 7465 2074 6861 7420 5f61      Note that _a
-00001bb0: 7374 2e4e 6f74 2069 7320 6e6f 7420 6120  st.Not is not a 
-00001bc0: 7661 6c69 6420 626f 6f6c 6561 6e20 6f70  valid boolean op
-00001bd0: 6572 6174 6f72 2c20 6974 2069 7320 636f  erator, it is co
-00001be0: 6e73 6964 6572 6564 0a20 2020 2020 2061  nsidered.      a
-00001bf0: 2075 6e61 7279 206f 7065 7261 746f 722e   unary operator.
-00001c00: 0a20 2020 2020 2046 6f72 2065 7861 6d70  .      For examp
-00001c10: 6c65 3a20 285f 6173 742e 4f72 2c20 5f61  le: (_ast.Or, _a
-00001c20: 7374 2e4e 616d 6528 2761 2729 290a 0a20  st.Name('a')).. 
-00001c30: 2052 6574 7572 6e73 3a0a 2020 2020 416e   Returns:.    An
-00001c40: 205f 6173 742e 426f 6f6c 4f70 206e 6f64   _ast.BoolOp nod
-00001c50: 652e 0a20 204e 5472 0100 0000 2902 727c  e..  NTr....).r|
-00001c60: 0000 00da 0676 616c 7565 7329 0a72 3000  .....values).r0.
-00001c70: 0000 da03 706f 7072 1c00 0000 7239 0000  ....popr....r9..
-00001c80: 0072 3a00 0000 da09 426f 6f6c 4f70 4d61  .r:.....BoolOpMa
-00001c90: 7072 6b00 0000 da06 426f 6f6c 4f70 7232  prk.....BoolOpr2
-00001ca0: 0000 00da 024f 7229 0772 7700 0000 da16  .....Or).rw.....
-00001cb0: 616c 7465 726e 6174 696e 675f 6f70 735f  alternating_ops_
-00001cc0: 7661 6c75 6573 7281 0000 0072 7c00 0000  valuesr....r|...
-00001cd0: da07 6f70 5f6e 6578 74da 0b6f 705f 6f72  ..op_next..op_or
-00001ce0: 5f76 616c 7565 da0a 6c61 7374 5f76 616c  _value..last_val
-00001cf0: 7565 7208 0000 0072 0800 0000 7209 0000  uer....r....r...
-00001d00: 0072 8400 0000 ea00 0000 7342 0000 0006  .r........sB....
-00001d10: 0d04 0104 0108 0104 010a 0104 010c 0108  ................
-00001d20: 0104 0106 010c 0102 010c 030e 0102 0102  ................
-00001d30: ff02 0208 fe08 0408 0102 0102 ff02 020a  ................
-00001d40: fe04 0306 0102 0106 fe0a 0406 0104 e70e  ................
-00001d50: 1b72 8400 0000 6300 0000 0000 0000 0000  .r....c.........
-00001d60: 0000 0000 0000 0002 0000 0043 0000 0072  ...........C...r
-00001d70: 6800 0000 7238 0000 0029 0272 3900 0000  h...r8...).r9...
-00001d80: da06 4269 7441 6e64 7208 0000 0072 0800  ..BitAndr....r..
-00001d90: 0000 7208 0000 0072 0900 0000 728a 0000  ..r....r....r...
-00001da0: 0019 0100 0072 6a00 0000 728a 0000 0063  .....rj...r....c
-00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001dc0: 0200 0000 4300 0000 7268 0000 0072 3800  ....C...rh...r8.
-00001dd0: 0000 2902 7239 0000 00da 0542 6974 4f72  ..).r9.....BitOr
-00001de0: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00001df0: 0900 0000 728b 0000 001d 0100 0072 6a00  ....r........rj.
-00001e00: 0000 728b 0000 0063 0000 0000 0000 0000  ..r....c........
-00001e10: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
-00001e20: 7268 0000 0072 3800 0000 2902 7239 0000  rh...r8...).r9..
-00001e30: 00da 0642 6974 586f 7272 0800 0000 7208  ...BitXorr....r.
-00001e40: 0000 0072 0800 0000 7209 0000 0072 8c00  ...r....r....r..
-00001e50: 0000 2101 0000 726a 0000 0072 8c00 0000  ..!...rj...r....
-00001e60: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001e70: 0004 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-00001e80: a001 7c00 7c01 a102 5300 7238 0000 0029  ..|.|...S.r8...)
-00001e90: 0272 3900 0000 da07 6b65 7977 6f72 6429  .r9.....keyword)
-00001ea0: 0272 2a00 0000 7249 0000 0072 0800 0000  .r*...rI...r....
-00001eb0: 7208 0000 0072 0900 0000 728d 0000 0025  r....r....r....%
-00001ec0: 0100 0072 0f00 0000 728d 0000 0063 0500  ...r....r....c..
-00001ed0: 0000 0000 0000 0000 0000 0600 0000 0700  ................
-00001ee0: 0000 4300 0000 73ac 0000 0074 007c 0174  ..C...s....t.|.t
-00001ef0: 0183 0273 0974 0264 0183 0182 0174 007c  ...s.t.d.....t.|
-00001f00: 0074 0383 0272 1574 047c 00a0 0564 02a1  .t...r.t.|...d..
-00001f10: 018e 007d 0074 007c 0474 0683 0273 1e74  ...}.t.|.t...s.t
-00001f20: 0264 0383 0182 0174 007c 0074 076a 0874  .d.....t.|.t.j.t
-00001f30: 076a 0966 0283 0273 2b74 0264 0483 0182  .j.f...s+t.d....
-00001f40: 0164 0564 0684 007c 0144 0083 017d 0174  .d.d...|.D...}.t
-00001f50: 007c 0374 0383 0272 3e74 047c 03a0 0564  .|.t...r>t.|...d
-00001f60: 02a1 018e 007d 0374 007c 0474 0383 0272  .....}.t.|.t...r
-00001f70: 4a74 047c 04a0 0564 02a1 018e 007d 0474  Jt.|...d.....}.t
-00001f80: 076a 0a7c 007c 017c 027c 037c 0464 078d  .j.|.|.|.|.|.d..
-00001f90: 057d 057c 0553 0029 0861 8802 0000 4372  .}.|.S.).a....Cr
-00001fa0: 6561 7465 7320 616e 205f 6173 742e 4361  eates an _ast.Ca
-00001fb0: 6c6c 206e 6f64 652e 0a0a 2020 4172 6773  ll node...  Args
-00001fc0: 3a0a 2020 2020 6361 6c6c 6572 3a20 4569  :.    caller: Ei
-00001fd0: 7468 6572 2061 206e 6f64 6520 6f66 2074  ther a node of t
-00001fe0: 6865 2061 7070 726f 7072 6961 7465 2074  he appropriate t
-00001ff0: 7970 650a 2020 2020 2020 285f 6173 742e  ype.      (_ast.
-00002000: 5374 722c 205f 6173 742e 4e61 6d65 2c20  Str, _ast.Name, 
-00002010: 6f72 205f 6173 742e 4174 7472 6962 7574  or _ast.Attribut
-00002020: 6529 2c20 6f72 2061 2064 6f74 2d73 6570  e), or a dot-sep
-00002030: 6172 6174 6564 2073 7472 696e 672e 0a20  arated string.. 
-00002040: 2020 2061 7267 733a 2041 206c 6973 7420     args: A list 
-00002050: 6f66 2061 7267 732e 0a20 2020 206b 6579  of args..    key
-00002060: 733a 2041 206c 6973 7420 6f66 206b 6579  s: A list of key
-00002070: 732c 206d 7573 7420 6265 2074 6865 2073  s, must be the s
-00002080: 616d 6520 6c65 6e67 7468 2061 7320 7661  ame length as va
-00002090: 6c75 6573 2e0a 2020 2020 7661 6c75 6573  lues..    values
-000020a0: 3a20 4120 6c69 7374 206f 6620 7661 6c75  : A list of valu
-000020b0: 6573 2c20 636f 7272 6573 706f 6e64 2074  es, correspond t
-000020c0: 6f20 6b65 7973 2e0a 2020 2020 7374 6172  o keys..    star
-000020d0: 6172 6773 3a20 4120 6e6f 6465 2077 6974  args: A node wit
-000020e0: 6820 6120 7374 6172 2069 6e20 6672 6f6e  h a star in fron
-000020f0: 7420 6f66 2069 742e 2050 6173 7369 6e67  t of it. Passing
-00002100: 2061 2073 7472 696e 6720 7769 6c6c 2062   a string will b
-00002110: 650a 2020 2020 2020 696e 7465 7270 7265  e.      interpre
-00002120: 7465 6420 6173 2061 2056 6172 5265 6665  ted as a VarRefe
-00002130: 7265 6e63 652e 0a20 2020 206b 7761 7267  rence..    kwarg
-00002140: 733a 2041 206e 6f64 6520 7769 7468 2074  s: A node with t
-00002150: 776f 2073 7461 7273 2069 6e20 6672 6f6e  wo stars in fron
-00002160: 7420 6f66 2069 742e 2050 6173 7369 6e67  t of it. Passing
-00002170: 2061 2073 7472 696e 6720 7769 6c6c 2062   a string will b
-00002180: 650a 2020 2020 2020 696e 7465 7270 7265  e.      interpre
-00002190: 7465 6420 6173 2061 2056 6172 5265 6665  ted as a VarRefe
-000021a0: 7265 6e63 652e 0a0a 2020 5261 6973 6573  rence...  Raises
-000021b0: 3a0a 2020 2020 5661 6c75 6545 7272 6f72  :.    ValueError
-000021c0: 3a20 4966 206c 656e 286b 6579 7329 2021  : If len(keys) !
-000021d0: 3d20 6c65 6e28 7661 6c75 6573 2920 6f72  = len(values) or
-000021e0: 2063 616c 6c65 7220 6973 206e 6f74 2074   caller is not t
-000021f0: 6865 2072 6967 6874 2074 7970 652e 0a0a  he right type...
-00002200: 2020 5265 7475 726e 733a 0a20 2020 2041    Returns:.    A
-00002210: 6e20 5f61 7374 2e43 616c 6c20 6f62 6a65  n _ast.Call obje
-00002220: 6374 2e0a 2020 7225 0000 00da 012e 7a19  ct..  r%......z.
-00002230: 6b77 6172 6773 206d 7573 7420 6265 2061  kwargs must be a
-00002240: 2061 7374 2e44 6963 747a 1d63 616c 6c65   ast.Dictz.calle
-00002250: 7220 6e6f 7420 7468 6520 6578 7065 6374  r not the expect
-00002260: 6564 2076 616c 7565 6301 0000 0000 0000  ed valuec.......
-00002270: 0000 0000 0002 0000 0006 0000 0053 0000  .............S..
-00002280: 00f3 1a00 0000 6700 7c00 5d09 7d01 7400  ......g.|.].}.t.
-00002290: 7c01 7401 6a02 6400 8d02 9102 7102 5300  |.t.j.d.....q.S.
-000022a0: a901 723e 0000 00a9 0372 2e00 0000 7273  ..r>.....r....rs
-000022b0: 0000 0072 1400 0000 7228 0000 0072 0800  ...r....r(...r..
-000022c0: 0000 7208 0000 0072 0900 0000 722b 0000  ..r....r....r+..
-000022d0: 0049 0100 00f3 0200 0000 1a00 7a18 4361  .I..........z.Ca
-000022e0: 6c6c 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ll.<locals>.<lis
-000022f0: 7463 6f6d 703e 2905 da04 6675 6e63 7235  tcomp>)...funcr5
-00002300: 0000 00da 086b 6579 776f 7264 73da 0873  .....keywords..s
-00002310: 7461 7261 7267 73da 066b 7761 7267 7329  tarargs..kwargs)
-00002320: 0b72 1c00 0000 7230 0000 0072 3100 0000  .r....r0...r1...
-00002330: 7242 0000 00da 0c56 6172 5265 6665 7265  rB.....VarRefere
-00002340: 6e63 65da 0573 706c 6974 da04 6469 6374  nce..split..dict
-00002350: 7239 0000 0072 4300 0000 da09 4174 7472  r9...rC.....Attr
-00002360: 6962 7574 65da 0443 616c 6c29 06da 0663  ibute..Call)...c
-00002370: 616c 6c65 7272 3500 0000 7294 0000 0072  allerr5...r....r
-00002380: 9500 0000 7296 0000 0072 7b00 0000 7208  ....r....r{...r.
-00002390: 0000 0072 0800 0000 7209 0000 0072 9b00  ...r....r....r..
-000023a0: 0000 2901 0000 732a 0000 000a 1408 010a  ..)...s*........
-000023b0: 050e 010a 0108 0112 0108 010e 010a 010e  ................
-000023c0: 010a 010e 0104 0102 0102 0102 0102 0102  ................
-000023d0: 0106 fb04 0672 9b00 0000 6307 0000 0000  .....r....c.....
-000023e0: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
-000023f0: 0000 0073 6c00 0000 7c02 7306 7400 6401  ...sl...|.s.t.d.
-00002400: 8301 8201 7c05 6402 7501 720e 7401 6403  ....|.d.u.r.t.d.
-00002410: 8301 8201 7c04 6402 7501 7216 7401 6404  ....|.d.u.r.t.d.
-00002420: 8301 8201 7402 7c01 7403 8302 731f 7400  ....t.|.t...s.t.
-00002430: 6405 8301 8201 7404 7c02 8301 7d02 6406  d.....t.|...}.d.
-00002440: 6407 8400 7c01 4400 8301 7d01 7405 6a06  d...|.D...}.t.j.
-00002450: 7c00 7c01 7c02 7c03 7403 7c06 8301 6408  |.|.|.|.t.|...d.
-00002460: 8d05 5300 2909 615a 0100 0043 7265 6174  ..S.).aZ...Creat
-00002470: 6573 2061 6e20 5f61 7374 2e43 6c61 7373  es an _ast.Class
-00002480: 4465 6620 6e6f 6465 2e0a 0a20 2041 7267  Def node...  Arg
-00002490: 733a 0a20 2020 206e 616d 653a 2054 6865  s:.    name: The
-000024a0: 206e 616d 6520 6f66 2074 6865 2063 6c61   name of the cla
-000024b0: 7373 2e0a 2020 2020 6261 7365 733a 2054  ss..    bases: T
-000024c0: 6865 2062 6173 6520 636c 6173 7365 7320  he base classes 
-000024d0: 6f66 2074 6865 2063 6c61 7373 0a20 2020  of the class.   
-000024e0: 2062 6f64 793a 2041 206c 6973 7420 6f66   body: A list of
-000024f0: 205f 6173 742e 7374 6d74 206e 6f64 6573   _ast.stmt nodes
-00002500: 2074 6861 7420 676f 2069 6e20 7468 6520   that go in the 
-00002510: 626f 6479 206f 6620 7468 6520 636c 6173  body of the clas
-00002520: 732e 0a20 2020 2064 6563 6f72 6174 6f72  s..    decorator
-00002530: 5f6c 6973 743a 2041 206c 6973 7420 6f66  _list: A list of
-00002540: 2064 6563 6f72 6174 6f72 206e 6f64 6573   decorator nodes
-00002550: 2e0a 0a20 2052 6169 7365 733a 0a20 2020  ...  Raises:.   
-00002560: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
-00002570: 736f 6d65 2062 6f64 7920 656c 656d 656e  some body elemen
-00002580: 7420 6973 206e 6f74 2061 6e20 5f61 7374  t is not an _ast
-00002590: 2e73 746d 7420 6e6f 6465 2e0a 0a20 2052  .stmt node...  R
-000025a0: 6574 7572 6e73 3a0a 2020 2020 416e 205f  eturns:.    An _
-000025b0: 6173 742e 436c 6173 7344 6566 206e 6f64  ast.ClassDef nod
-000025c0: 652e 0a20 207a 1e63 6c61 7373 2062 6f64  e..  z.class bod
-000025d0: 7920 6d75 7374 2062 6520 6120 6e6f 6e20  y must be a non 
-000025e0: 656d 7074 794e 7a20 4e6f 6e20 4e6f 6e65  emptyNz Non None
-000025f0: 206b 7761 7267 7320 6973 206e 6f74 2073   kwargs is not s
-00002600: 7570 706f 7274 6564 7a22 4e6f 6e20 4e6f  upportedz"Non No
-00002610: 6e65 2073 7461 7261 7267 7320 6973 206e  ne starargs is n
-00002620: 6f74 2073 7570 706f 7274 6564 7a14 6261  ot supportedz.ba
-00002630: 7365 7320 6d75 7374 2062 6520 6120 6c69  ses must be a li
-00002640: 7374 6301 0000 0000 0000 0000 0000 0002  stc.............
-00002650: 0000 0006 0000 0053 0000 0072 8f00 0000  .......S...r....
-00002660: 7290 0000 0072 9100 0000 2902 7229 0000  r....r....).r)..
-00002670: 0072 7600 0000 7208 0000 0072 0800 0000  .rv...r....r....
-00002680: 7209 0000 0072 2b00 0000 6f01 0000 7292  r....r+...o...r.
-00002690: 0000 007a 1c43 6c61 7373 4465 662e 3c6c  ...z.ClassDef.<l
-000026a0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000026b0: 3e29 05da 046e 616d 65da 0562 6173 6573  >)...name..bases
-000026c0: 721b 0000 0072 9400 0000 da0e 6465 636f  r....r......deco
-000026d0: 7261 746f 725f 6c69 7374 2907 7231 0000  rator_list).r1..
-000026e0: 0072 4400 0000 721c 0000 0072 3000 0000  .rD...r....r0...
-000026f0: 7251 0000 0072 3900 0000 da08 436c 6173  rQ...r9.....Clas
-00002700: 7344 6566 2907 729d 0000 0072 9e00 0000  sDef).r....r....
-00002710: 721b 0000 0072 9400 0000 7295 0000 0072  r....r....r....r
-00002720: 9600 0000 729f 0000 0072 0800 0000 7208  ....r....r....r.
-00002730: 0000 0072 0900 0000 72a0 0000 0057 0100  ...r....r....W..
-00002740: 0073 2200 0000 040f 0801 0801 0801 0801  .s".............
-00002750: 0801 0a01 0801 0801 0e01 0401 0201 0201  ................
-00002760: 0201 0201 0601 06fb 72a0 0000 0063 0000  ........r....c..
-00002770: 0000 0000 0000 0000 0000 0500 0000 0700  ................
-00002780: 0000 4700 0000 73a8 0000 0074 007c 0083  ..G...s....t.|..
-00002790: 0164 016b 0072 0a74 0164 0283 0182 0167  .d.k.r.t.d.....g
-000027a0: 007d 0167 007d 0274 027c 0083 0144 005d  .}.g.}.t.|...D.]
-000027b0: 325c 027d 037d 047c 0364 0316 0064 046b  2\.}.}.|.d...d.k
-000027c0: 0272 3674 037c 0474 046a 0583 0273 2674  .r6t.|.t.j...s&t
-000027d0: 067c 0483 017d 0474 037c 0474 046a 0783  .|...}.t.|.t.j..
-000027e0: 0273 3074 0164 0583 0182 017c 01a0 087c  .s0t.d.....|...|
-000027f0: 04a1 0101 0071 127c 0364 066b 0372 447c  .....q.|.d.k.rD|
-00002800: 02a0 0874 097c 0474 0a6a 0b64 078d 02a1  ...t.|.t.j.d....
-00002810: 0101 0071 1274 046a 0c74 097c 0064 0619  ...q.t.j.t.|.d..
-00002820: 0074 0a6a 0b64 078d 027c 017c 0264 088d  .t.j.d...|.|.d..
-00002830: 0353 0029 0961 0201 0000 4372 6561 7465  .S.).a....Create
-00002840: 7320 616e 205f 6173 742e 436f 6d70 6172  s an _ast.Compar
-00002850: 6520 6e6f 6465 2e0a 0a20 2041 7267 733a  e node...  Args:
-00002860: 0a20 2020 202a 6172 6773 3a20 4c69 7374  .    *args: List
-00002870: 2077 6869 6368 2073 686f 756c 6420 616c   which should al
-00002880: 7465 726e 6174 6520 6265 7477 6565 6e20  ternate between 
-00002890: 7265 6775 6c61 7220 6e6f 6465 7320 616e  regular nodes an
-000028a0: 6420 5f61 7374 2e63 6d70 6f70 2e0a 0a20  d _ast.cmpop... 
-000028b0: 2052 6169 7365 733a 0a20 2020 2056 616c   Raises:.    Val
-000028c0: 7565 4572 726f 723a 2049 6620 6c65 7373  ueError: If less
-000028d0: 2074 6861 6e20 3320 6172 6773 2c20 6f72   than 3 args, or
-000028e0: 206f 6464 2061 7267 7320 6172 6520 6e6f   odd args are no
-000028f0: 7420 7661 6c69 6420 636f 6d70 6172 6973  t valid comparis
-00002900: 6f6e 0a20 2020 2020 206f 7065 7261 746f  on.      operato
-00002910: 7273 2e0a 0a20 2052 6574 7572 6e73 3a0a  rs...  Returns:.
-00002920: 2020 2020 416e 205f 6173 742e 436f 6d70      An _ast.Comp
-00002930: 6172 6520 6e6f 6465 2e0a 2020 e903 0000  are node..  ....
-00002940: 007a 194d 7573 7420 6861 7665 2061 7420  .z.Must have at 
-00002950: 6c65 6173 7420 3320 6172 6773 e902 0000  least 3 args....
-00002960: 00e9 0100 0000 7a28 4f64 6420 6172 6773  ......z(Odd args
-00002970: 206d 7573 7420 6265 2069 6e73 7461 6e63   must be instanc
-00002980: 6573 206f 6620 5f61 7374 2e63 6d70 6f70  es of _ast.cmpop
-00002990: 7201 0000 0072 3e00 0000 2903 7277 0000  r....r>...).rw..
-000029a0: 00da 036f 7073 da0b 636f 6d70 6172 6174  ...ops..comparat
-000029b0: 6f72 7329 0dda 036c 656e 7231 0000 00da  ors)...lenr1....
-000029c0: 0965 6e75 6d65 7261 7465 721c 0000 0072  .enumerater....r
-000029d0: 3900 0000 723a 0000 00da 0c43 6f6d 7061  9...r:.....Compa
-000029e0: 7265 4f70 4d61 70da 0563 6d70 6f70 7232  reOpMap..cmpopr2
-000029f0: 0000 0072 2e00 0000 7273 0000 0072 1400  ...r....rs...r..
-00002a00: 0000 da07 436f 6d70 6172 6529 0572 3500  ....Compare).r5.
-00002a10: 0000 72a4 0000 0072 a500 0000 da05 696e  ..r....r......in
-00002a20: 6465 7872 2a00 0000 7208 0000 0072 0800  dexr*...r....r..
-00002a30: 0000 7209 0000 0072 aa00 0000 7801 0000  ..r....r....x...
-00002a40: 7324 0000 000c 0d08 0104 0104 0110 010c  s$..............
-00002a50: 010c 0108 010c 0108 010c 0108 0214 0102  ................
-00002a60: 8014 0102 0102 0106 fe72 aa00 0000 6303  .........r....c.
-00002a70: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00002a80: 0000 0047 0000 0073 3200 0000 7400 7c00  ...G...s2...t.|.
-00002a90: 7401 6a02 6401 8d02 7d00 7400 7c01 7401  t.j.d...}.t.|.t.
-00002aa0: 6a03 6401 8d02 7d01 7404 6a05 7c00 7c01  j.d...}.t.j.|.|.
-00002ab0: 7406 7c03 8301 7c02 6402 8d04 5300 2903  t.|...|.d...S.).
-00002ac0: 7af6 4372 6561 7465 2061 6e20 5f61 7374  z.Create an _ast
-00002ad0: 2e63 6f6d 7072 6568 656e 7369 6f6e 206e  .comprehension n
-00002ae0: 6f64 652c 2075 7365 6420 696e 205f 6173  ode, used in _as
-00002af0: 742e 4c69 7374 436f 6d70 7265 6865 6e73  t.ListComprehens
-00002b00: 696f 6e2e 0a0a 2020 4172 6773 3a0a 2020  ion...  Args:.  
-00002b10: 2020 666f 725f 7061 7274 3a20 5468 6520    for_part: The 
-00002b20: 7061 7274 2061 6674 6572 2022 666f 7220  part after "for 
-00002b30: 220a 2020 2020 696e 5f70 6172 743a 2054  ".    in_part: T
-00002b40: 6865 2070 6172 7420 6166 7465 7220 2266  he part after "f
-00002b50: 6f72 205b 666f 725f 7061 7274 5d20 696e  or [for_part] in
-00002b60: 2022 0a20 2020 202a 6966 733a 207b 5f61   ".    *ifs: {_a
-00002b70: 7374 2e43 6f6d 7061 7265 7d0a 0a20 2052  st.Compare}..  R
-00002b80: 6574 7572 6e73 3a0a 2020 2020 7b5f 6173  eturns:.    {_as
-00002b90: 742e 636f 6d70 7265 6865 6e73 696f 6e7d  t.comprehension}
-00002ba0: 0a20 2020 203a 7061 7261 6d20 6973 5f61  .    :param is_a
-00002bb0: 7379 6e63 3a0a 2020 723e 0000 0029 0472  sync:.  r>...).r
-00002bc0: 7a00 0000 da04 6974 6572 da03 6966 73da  z.....iter..ifs.
-00002bd0: 0869 735f 6173 796e 6329 0772 2e00 0000  .is_async).r....
-00002be0: 7273 0000 0072 1500 0000 7214 0000 0072  rs...r....r....r
-00002bf0: 3900 0000 da0d 636f 6d70 7265 6865 6e73  9.....comprehens
-00002c00: 696f 6e72 3000 0000 2904 da08 666f 725f  ionr0...)...for_
-00002c10: 7061 7274 da07 696e 5f70 6172 7472 ae00  part..in_partr..
-00002c20: 0000 72ad 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00002c30: 0072 0900 0000 72af 0000 0098 0100 0073  .r....r........s
-00002c40: 0e00 0000 0e0c 0e01 0601 0201 0601 0201  ................
-00002c50: 06fd 72af 0000 0072 0800 0000 6302 0000  ..r....r....c...
-00002c60: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00002c70: 0043 0000 0073 5000 0000 7400 7c00 8301  .C...sP...t.|...
-00002c80: 7400 7c01 8301 6b03 7214 7401 6401 a002  t.|...k.r.t.d...
-00002c90: 7400 7c00 8301 7400 7c01 8301 a102 8301  t.|...t.|.......
-00002ca0: 8201 6402 6403 8400 7c00 4400 8301 7d00  ..d.d...|.D...}.
-00002cb0: 6404 6403 8400 7c01 4400 8301 7d01 7403  d.d...|.D...}.t.
-00002cc0: a004 7c00 7c01 a102 5300 2905 6131 0100  ..|.|...S.).a1..
-00002cd0: 0043 7265 6174 6573 2061 6e20 5f61 7374  .Creates an _ast
-00002ce0: 2e44 6963 7420 6e6f 6465 2e20 5468 6973  .Dict node. This
-00002cf0: 2072 6570 7265 7365 6e74 7320 6120 6469   represents a di
-00002d00: 6374 206c 6974 6572 616c 2e0a 0a20 2041  ct literal...  A
-00002d10: 7267 733a 0a20 2020 206b 6579 733a 2041  rgs:.    keys: A
-00002d20: 206c 6973 7420 6f66 206b 6579 7320 6173   list of keys as
-00002d30: 206e 6f64 6573 2e20 4d75 7374 2062 6520   nodes. Must be 
-00002d40: 7468 6520 7361 6d65 206c 656e 6774 6820  the same length 
-00002d50: 6173 2076 616c 7565 732e 0a20 2020 2076  as values..    v
-00002d60: 616c 7565 733a 2041 206c 6973 7420 6f66  alues: A list of
-00002d70: 2076 616c 7565 7320 6173 206e 6f64 6573   values as nodes
-00002d80: 2e20 4d75 7374 2062 6520 7468 6520 7361  . Must be the sa
-00002d90: 6d65 206c 656e 6774 6820 6173 2076 616c  me length as val
-00002da0: 7565 732e 0a0a 2020 5261 6973 6573 3a0a  ues...  Raises:.
-00002db0: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00002dc0: 4966 206c 656e 286b 6579 7329 2021 3d20  If len(keys) != 
-00002dd0: 6c65 6e28 7661 6c75 6573 292e 0a0a 2020  len(values)...  
-00002de0: 5265 7475 726e 733a 0a20 2020 2041 6e20  Returns:.    An 
-00002df0: 5f61 7374 2e44 6963 7420 6e6f 6465 2e0a  _ast.Dict node..
-00002e00: 2020 7a1e 6c65 6e28 6b65 7973 293d 7b7d    z.len(keys)={}
-00002e10: 2021 3d20 6c65 6e28 7661 6c75 6573 293d   != len(values)=
-00002e20: 7b7d 6301 0000 0000 0000 0000 0000 0002  {}c.............
-00002e30: 0000 0004 0000 0053 0000 0072 2600 0000  .......S...r&...
-00002e40: 7208 0000 0072 2d00 0000 2902 7229 0000  r....r-...).r)..
-00002e50: 00da 036b 6579 7208 0000 0072 0800 0000  ...keyr....r....
-00002e60: 7209 0000 0072 2b00 0000 bc01 0000 722c  r....r+.......r,
-00002e70: 0000 007a 1844 6963 742e 3c6c 6f63 616c  ...z.Dict.<local
-00002e80: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-00002e90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00002ea0: 0000 5300 0000 7226 0000 0072 0800 0000  ..S...r&...r....
-00002eb0: 722d 0000 0029 0272 2900 0000 7249 0000  r-...).r)...rI..
-00002ec0: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-00002ed0: 722b 0000 00bd 0100 0072 2c00 0000 2905  r+.......r,...).
-00002ee0: 72a6 0000 0072 3100 0000 724f 0000 0072  r....r1...rO...r
-00002ef0: 3900 0000 da04 4469 6374 2902 da04 6b65  9.....Dict)...ke
-00002f00: 7973 7281 0000 0072 0800 0000 7208 0000  ysr....r....r...
-00002f10: 0072 0900 0000 72b3 0000 00ac 0100 0073  .r....r........s
-00002f20: 0e00 0000 100d 0201 1201 04ff 0e02 0e01  ................
-00002f30: 0c01 72b3 0000 0029 0172 ae00 0000 6304  ..r....).r....c.
-00002f40: 0000 0000 0000 0001 0000 0006 0000 0007  ................
-00002f50: 0000 0047 0000 0073 5a00 0000 7400 7c00  ...G...sZ...t.|.
-00002f60: 7401 6a02 6401 8d02 7d00 7400 7c01 7401  t.j.d...}.t.|.t.
-00002f70: 6a02 6401 8d02 7d01 7400 7c02 7401 6a03  j.d...}.t.|.t.j.
-00002f80: 6401 8d02 7d02 7400 7c03 7401 6a02 6401  d...}.t.|.t.j.d.
-00002f90: 8d02 7d03 7404 6a05 7c00 7c01 7406 7c02  ..}.t.j.|.|.t.|.
-00002fa0: 7c03 7c04 6703 7c05 a201 5200 8e00 6701  |.|.g.|...R...g.
-00002fb0: 6402 8d03 5300 2903 61bd 0100 0043 7265  d...S.).a....Cre
-00002fc0: 6174 6573 205f 6173 742e 4469 6374 436f  ates _ast.DictCo
-00002fd0: 6d70 206e 6f64 6573 2e0a 0a20 2027 6c65  mp nodes...  'le
-00002fe0: 6674 5f73 6964 6527 2c20 276c 6566 745f  ft_side', 'left_
-00002ff0: 7369 6465 5f76 616c 7565 2720 666f 7220  side_value' for 
-00003000: 2766 6f72 5f70 6172 7427 2069 6e20 2769  'for_part' in 'i
-00003010: 6e5f 7061 7274 2720 6966 2027 6966 7327  n_part' if 'ifs'
-00003020: 0a0a 2020 4172 6773 3a0a 2020 2020 6c65  ..  Args:.    le
-00003030: 6674 5f73 6964 655f 6b65 793a 206b 6579  ft_side_key: key
-00003040: 2069 6e20 6c65 6674 6d6f 7374 2073 6964   in leftmost sid
-00003050: 6520 6f66 2074 6865 2065 7870 7265 7373  e of the express
-00003060: 696f 6e2e 0a20 2020 206c 6566 745f 7369  ion..    left_si
-00003070: 6465 5f76 616c 7565 3a20 7661 6c75 6520  de_value: value 
-00003080: 696e 206c 6566 746d 6f73 7420 7369 6465  in leftmost side
-00003090: 206f 6620 7468 6520 6578 7072 6573 7369   of the expressi
-000030a0: 6f6e 2e0a 2020 2020 666f 725f 7061 7274  on..    for_part
-000030b0: 3a20 5468 6520 7061 7274 2061 6674 6572  : The part after
-000030c0: 2027 5b6c 6566 745f 7369 6465 5d20 666f   '[left_side] fo
-000030d0: 7220 270a 2020 2020 696e 5f70 6172 743a  r '.    in_part:
-000030e0: 2054 6865 2070 6172 7420 6166 7465 7220   The part after 
-000030f0: 275b 6c65 6674 5f73 6964 655d 2066 6f72  '[left_side] for
-00003100: 205b 666f 725f 7061 7274 5d20 696e 2027   [for_part] in '
-00003110: 0a20 2020 202a 6966 733a 2041 6e79 2069  .    *ifs: Any i
-00003120: 6620 7374 6174 656d 656e 7473 2074 6861  f statements tha
-00003130: 7420 636f 6d65 2061 7420 7468 6520 656e  t come at the en
-00003140: 642e 0a0a 2020 5265 7475 726e 733a 0a20  d...  Returns:. 
-00003150: 2020 207b 5f61 7374 2e44 6963 7443 6f6d     {_ast.DictCom
-00003160: 707d 0a20 2020 203a 7061 7261 6d20 6973  p}.    :param is
-00003170: 5f61 7379 6e63 3a0a 2020 723e 0000 0029  _async:.  r>...)
-00003180: 0372 b200 0000 7249 0000 00da 0a67 656e  .r....rI.....gen
-00003190: 6572 6174 6f72 7329 0772 2e00 0000 7273  erators).r....rs
-000031a0: 0000 0072 1400 0000 7215 0000 0072 3900  ...r....r....r9.
-000031b0: 0000 da08 4469 6374 436f 6d70 72af 0000  ....DictCompr...
-000031c0: 0029 06da 0d6c 6566 745f 7369 6465 5f6b  .)...left_side_k
-000031d0: 6579 da0f 6c65 6674 5f73 6964 655f 7661  ey..left_side_va
-000031e0: 6c75 6572 b000 0000 72b1 0000 0072 ae00  luer....r....r..
-000031f0: 0000 72ad 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00003200: 0072 0900 0000 72b6 0000 00c1 0100 0073  .r....r........s
-00003210: 1200 0000 0e10 0e01 0e01 0e01 0401 0201  ................
-00003220: 0201 1401 06fd 72b6 0000 0063 0000 0000  ......r....c....
-00003230: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00003240: 4300 0000 7268 0000 0072 3800 0000 2902  C...rh...r8...).
-00003250: 7239 0000 00da 0344 6976 7208 0000 0072  r9.....Divr....r
-00003260: 0800 0000 7208 0000 0072 0900 0000 72b9  ....r....r....r.
-00003270: 0000 00db 0100 0072 6a00 0000 72b9 0000  .......rj...r...
-00003280: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00003290: 0000 0200 0000 4300 0000 7268 0000 0072  ......C...rh...r
-000032a0: 3800 0000 2902 7239 0000 00da 0245 7172  8...).r9.....Eqr
-000032b0: 0800 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-000032c0: 0000 0072 ba00 0000 df01 0000 726a 0000  ...r........rj..
-000032d0: 0072 ba00 0000 6303 0000 0000 0000 0000  .r....c.........
-000032e0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-000032f0: 1800 0000 7400 7c02 8301 7d02 7401 6a02  ....t.|...}.t.j.
-00003300: 7c00 7c01 7c02 6401 8d03 5300 2902 4e29  |.|.|.d...S.).N)
-00003310: 0372 0d00 0000 729d 0000 0072 1b00 0000  .r....r....r....
-00003320: 2903 7251 0000 0072 3900 0000 da0d 4578  ).rQ...r9.....Ex
-00003330: 6365 7074 4861 6e64 6c65 7229 03da 0e65  ceptHandler)...e
-00003340: 7863 6570 7469 6f6e 5f74 7970 6572 9d00  xception_typer..
-00003350: 0000 721b 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00003360: 0072 0900 0000 72bb 0000 00e3 0100 0073  .r....r........s
-00003370: 0400 0000 0801 1001 72bb 0000 0063 0100  ........r....c..
-00003380: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00003390: 0000 4300 0000 7324 0000 0074 007c 0074  ..C...s$...t.|.t
-000033a0: 016a 0283 0272 0d74 0364 01a0 047c 00a1  .j...r.t.d...|..
-000033b0: 0183 0182 0174 01a0 057c 00a1 0153 0029  .....t...|...S.)
-000033c0: 0261 1501 0000 4372 6561 7465 7320 616e  .a....Creates an
-000033d0: 205f 6173 742e 4578 7072 206e 6f64 652e   _ast.Expr node.
-000033e0: 0a0a 2020 4e6f 7465 2074 6861 7420 7468  ..  Note that th
-000033f0: 6973 206e 6f64 6520 6973 206d 6f73 746c  is node is mostl
-00003400: 7920 7573 6564 2074 6f20 7772 6170 206f  y used to wrap o
-00003410: 7468 6572 206e 6f64 6573 2073 6f20 7468  ther nodes so th
-00003420: 6579 2772 6520 7472 6561 7465 640a 2020  ey're treated.  
-00003430: 6173 2077 686f 6c65 2d6c 696e 6520 7374  as whole-line st
-00003440: 6174 656d 656e 7473 2e0a 0a20 2041 7267  atements...  Arg
-00003450: 733a 0a20 2020 2076 616c 7565 3a20 5468  s:.    value: Th
-00003460: 6520 7661 6c75 6520 7374 6f72 6564 2069  e value stored i
-00003470: 6e20 7468 6520 6e6f 6465 2e0a 0a20 2052  n the node...  R
-00003480: 6169 7365 733a 0a20 2020 2056 616c 7565  aises:.    Value
-00003490: 4572 726f 723a 2049 6620 7661 6c75 6520  Error: If value 
-000034a0: 6973 2061 6e20 5f61 7374 2e73 746d 7420  is an _ast.stmt 
-000034b0: 6e6f 6465 2e0a 0a20 2052 6574 7572 6e73  node...  Returns
-000034c0: 3a0a 2020 2020 416e 205f 6173 742e 4578  :.    An _ast.Ex
-000034d0: 7072 206e 6f64 652e 0a20 207a 7376 616c  pr node..  zsval
-000034e0: 7565 206d 7573 7420 6e6f 7420 6265 2061  ue must not be a
-000034f0: 6e20 5f61 7374 2e73 746d 7420 6e6f 6465  n _ast.stmt node
-00003500: 2c20 6265 6361 7573 6520 7468 6f73 6520  , because those 
-00003510: 6e6f 6465 7320 646f 6e27 7420 6e65 6564  nodes don't need
-00003520: 2074 6f20 6265 2077 7261 7070 6564 2069   to be wrapped i
-00003530: 6e20 616e 2045 7870 7220 6e6f 6465 2e20  n an Expr node. 
-00003540: 5661 6c75 6520 7061 7373 6564 3a20 7b7d  Value passed: {}
-00003550: 2906 721c 0000 0072 3900 0000 724e 0000  ).r....r9...rN..
-00003560: 0072 3100 0000 724f 0000 00da 0445 7870  .r1...rO.....Exp
-00003570: 72a9 0172 4900 0000 7208 0000 0072 0800  r..rI...r....r..
-00003580: 0000 7209 0000 0072 bd00 0000 e801 0000  ..r....r........
-00003590: 730c 0000 000c 0f02 0102 0106 0104 fe0a  s...............
-000035a0: 0372 bd00 0000 6300 0000 0000 0000 0000  .r....c.........
-000035b0: 0000 0000 0000 0002 0000 0043 0000 0072  ...........C...r
-000035c0: 6800 0000 7238 0000 0029 0272 3900 0000  h...r8...).r9...
-000035d0: da08 466c 6f6f 7244 6976 7208 0000 0072  ..FloorDivr....r
-000035e0: 0800 0000 7208 0000 0072 0900 0000 72bf  ....r....r....r.
-000035f0: 0000 00fe 0100 0072 6a00 0000 72bf 0000  .......rj...r...
-00003600: 0063 0600 0000 0000 0000 0000 0000 0600  .c..............
-00003610: 0000 0800 0000 4300 0000 734a 0000 007c  ......C...sJ...|
-00003620: 0172 0c74 007c 0174 016a 0283 0273 0c74  .r.t.|.t.j...s.t
-00003630: 0364 0183 0182 017c 0173 1274 0283 007d  .d.....|.s.t...}
-00003640: 016e 027c 017d 0174 047c 0283 017d 0274  .n.|.}.t.|...}.t
-00003650: 056a 067c 007c 017c 027c 047c 0574 077c  .j.|.|.|.|.|.t.|
-00003660: 0383 0164 028d 0653 0029 0361 2802 0000  ...d...S.).a(...
-00003670: 4372 6561 7465 7320 616e 205f 6173 742e  Creates an _ast.
-00003680: 4675 6e63 7469 6f6e 4465 6620 6e6f 6465  FunctionDef node
-00003690: 2e0a 0a20 2041 7267 733a 0a20 2020 206e  ...  Args:.    n
-000036a0: 616d 653a 2054 6865 206e 616d 6520 6f66  ame: The name of
-000036b0: 2074 6865 2066 756e 6374 696f 6e2e 0a20   the function.. 
-000036c0: 2020 2061 7267 733a 2041 206c 6973 7420     args: A list 
-000036d0: 6f66 2061 7267 732e 0a20 2020 206b 6579  of args..    key
-000036e0: 733a 2041 206c 6973 7420 6f66 206b 6579  s: A list of key
-000036f0: 732c 206d 7573 7420 6265 2074 6865 2073  s, must be the s
-00003700: 616d 6520 6c65 6e67 7468 2061 7320 7661  ame length as va
-00003710: 6c75 6573 2e0a 2020 2020 7661 6c75 6573  lues..    values
-00003720: 3a20 4120 6c69 7374 206f 6620 7661 6c75  : A list of valu
-00003730: 6573 2c20 636f 7272 6573 706f 6e64 2074  es, correspond t
-00003740: 6f20 6b65 7973 2e0a 2020 2020 626f 6479  o keys..    body
-00003750: 3a20 4120 6c69 7374 206f 6620 5f61 7374  : A list of _ast
-00003760: 2e73 746d 7420 6e6f 6465 7320 7468 6174  .stmt nodes that
-00003770: 2067 6f20 696e 2074 6865 2062 6f64 7920   go in the body 
-00003780: 6f66 2074 6865 2066 756e 6374 696f 6e2e  of the function.
-00003790: 0a20 2020 2076 6172 6172 675f 6e61 6d65  .    vararg_name
-000037a0: 3a20 5468 6520 6e61 6d65 206f 6620 7468  : The name of th
-000037b0: 6520 7661 7261 7267 2076 6172 6961 626c  e vararg variabl
-000037c0: 652c 206f 7220 4e6f 6e65 2e0a 2020 2020  e, or None..    
-000037d0: 6b77 6172 675f 6e61 6d65 3a20 5468 6520  kwarg_name: The 
-000037e0: 6e61 6d65 206f 6620 7468 6520 6b77 6172  name of the kwar
-000037f0: 6773 2076 6172 6961 626c 652c 206f 7220  gs variable, or 
-00003800: 4e6f 6e65 2e0a 2020 2020 6465 636f 7261  None..    decora
-00003810: 746f 725f 6c69 7374 3a20 4120 6c69 7374  tor_list: A list
-00003820: 206f 6620 6465 636f 7261 746f 7220 6e6f   of decorator no
-00003830: 6465 732e 0a20 2052 6169 7365 733a 0a20  des..  Raises:. 
-00003840: 2020 2056 616c 7565 4572 726f 723a 2049     ValueError: I
-00003850: 6620 6c65 6e28 6b65 7973 2920 213d 206c  f len(keys) != l
-00003860: 656e 2876 616c 7565 7329 2e0a 0a20 2052  en(values)...  R
-00003870: 6574 7572 6e73 3a0a 2020 2020 416e 205f  eturns:.    An _
-00003880: 6173 742e 4675 6e63 7469 6f6e 4465 6620  ast.FunctionDef 
-00003890: 6e6f 6465 2e0a 2020 7225 0000 0029 0672  node..  r%...).r
-000038a0: 9d00 0000 7235 0000 0072 1b00 0000 da07  ....r5...r......
-000038b0: 7265 7475 726e 73da 0c74 7970 655f 636f  returns..type_co
-000038c0: 6d6d 656e 7472 9f00 0000 2908 721c 0000  mmentr....).r...
-000038d0: 0072 1900 0000 7267 0000 0072 3100 0000  .r....rg...r1...
-000038e0: 7251 0000 0072 3900 0000 da0b 4675 6e63  rQ...r9.....Func
-000038f0: 7469 6f6e 4465 6672 3000 0000 2906 729d  tionDefr0...).r.
-00003900: 0000 0072 3500 0000 721b 0000 0072 9f00  ...r5...r....r..
-00003910: 0000 72c0 0000 0072 c100 0000 7208 0000  ..r....r....r...
-00003920: 0072 0800 0000 7209 0000 0072 c200 0000  .r....r....r....
-00003930: 0202 0000 731c 0000 0010 1308 0104 0108  ....s...........
-00003940: 0104 0208 0104 0102 0102 0102 0102 0102  ................
-00003950: 0106 0106 fa72 c200 0000 6303 0000 0000  .....r....c.....
-00003960: 0000 0000 0000 0005 0000 0006 0000 0047  ...............G
-00003970: 0000 0073 4e00 0000 7400 7c00 7401 6a02  ...sN...t.|.t.j.
-00003980: 6401 8d02 7d00 7400 7c01 7401 6a03 6401  d...}.t.|.t.j.d.
-00003990: 8d02 7d01 7400 7c02 7401 6a02 6401 8d02  ..}.t.|.t.j.d...
-000039a0: 7d02 7404 6a05 7c00 7406 7c01 7c02 6402  }.t.j.|.t.|.|.d.
-000039b0: 6703 7c03 a201 5200 8e00 6701 6403 8d02  g.|...R...g.d...
-000039c0: 7d04 7c04 5300 2904 6153 0100 0043 7265  }.|.S.).aS...Cre
-000039d0: 6174 6573 205f 6173 742e 4765 6e65 7261  ates _ast.Genera
-000039e0: 746f 7245 7870 206e 6f64 6573 2e0a 0a20  torExp nodes... 
-000039f0: 2027 6c65 6674 5f73 6964 6527 2066 6f72   'left_side' for
-00003a00: 2027 666f 725f 7061 7274 2720 696e 2027   'for_part' in '
-00003a10: 696e 5f70 6172 7427 2069 6620 2769 6673  in_part' if 'ifs
-00003a20: 270a 0a20 2041 7267 733a 0a20 2020 206c  '..  Args:.    l
-00003a30: 6566 745f 7369 6465 3a20 6c65 6674 6d6f  eft_side: leftmo
-00003a40: 7374 2073 6964 6520 6f66 2074 6865 2065  st side of the e
-00003a50: 7870 7265 7373 696f 6e2e 0a20 2020 2066  xpression..    f
-00003a60: 6f72 5f70 6172 743a 2054 6865 2070 6172  or_part: The par
-00003a70: 7420 6166 7465 7220 275b 6c65 6674 5f73  t after '[left_s
-00003a80: 6964 655d 2066 6f72 2027 0a20 2020 2069  ide] for '.    i
-00003a90: 6e5f 7061 7274 3a20 5468 6520 7061 7274  n_part: The part
-00003aa0: 2061 6674 6572 2027 5b6c 6566 745f 7369   after '[left_si
-00003ab0: 6465 5d20 666f 7220 5b66 6f72 5f70 6172  de] for [for_par
-00003ac0: 745d 2069 6e20 270a 2020 2020 2a69 6673  t] in '.    *ifs
-00003ad0: 3a20 416e 7920 6966 2073 7461 7465 6d65  : Any if stateme
-00003ae0: 6e74 7320 7468 6174 2063 6f6d 6520 6174  nts that come at
-00003af0: 2074 6865 2065 6e64 2e0a 0a20 2052 6574   the end...  Ret
-00003b00: 7572 6e73 3a0a 2020 2020 7b5f 6173 742e  urns:.    {_ast.
-00003b10: 4765 6e65 7261 746f 7245 7870 7d0a 2020  GeneratorExp}.  
-00003b20: 723e 0000 0072 0100 0000 a902 da03 656c  r>...r........el
-00003b30: 7472 b500 0000 2907 722e 0000 0072 7300  tr....).r....rs.
-00003b40: 0000 7214 0000 0072 1500 0000 7239 0000  ..r....r....r9..
-00003b50: 00da 0c47 656e 6572 6174 6f72 4578 7072  ...GeneratorExpr
-00003b60: af00 0000 2905 da09 6c65 6674 5f73 6964  ....)...left_sid
-00003b70: 6572 b000 0000 72b1 0000 0072 ad00 0000  er....r....r....
-00003b80: 727b 0000 0072 0800 0000 7208 0000 0072  r{...r....r....r
-00003b90: 0900 0000 72c5 0000 0025 0200 0073 1000  ....r....%...s..
-00003ba0: 0000 0e0e 0e01 0e01 0401 0201 1401 06fe  ................
-00003bb0: 0403 72c5 0000 0063 0000 0000 0000 0000  ..r....c........
-00003bc0: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
-00003bd0: 7268 0000 0072 3800 0000 2902 7239 0000  rh...r8...).r9..
-00003be0: 00da 0247 7472 0800 0000 7208 0000 0072  ...Gtr....r....r
-00003bf0: 0800 0000 7209 0000 0072 c700 0000 3c02  ....r....r....<.
-00003c00: 0000 726a 0000 0072 c700 0000 6300 0000  ..rj...r....c...
-00003c10: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00003c20: 0043 0000 0072 6800 0000 7238 0000 0029  .C...rh...r8...)
-00003c30: 0272 3900 0000 da03 4774 4572 0800 0000  .r9.....GtEr....
-00003c40: 7208 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00003c50: c800 0000 4002 0000 726a 0000 0072 c800  ....@...rj...r..
-00003c60: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
-00003c70: 0000 0005 0000 0043 0000 0073 5600 0000  .......C...sV...
-00003c80: 7400 7c01 8301 7d01 7c02 6401 7500 720a  t.|...}.|.d.u.r.
-00003c90: 6700 7d02 7401 7c02 7402 7403 6602 8302  g.}.t.|.t.t.f...
-00003ca0: 7223 7c01 4400 5d0f 7d03 7401 7c03 7404  r#|.D.].}.t.|.t.
-00003cb0: 6a05 8302 7322 7406 6402 a007 7c03 a101  j...s"t.d...|...
-00003cc0: 8301 8201 7113 7404 6a08 7c00 7c01 7c02  ....q.t.j.|.|.|.
-00003cd0: 6403 8d03 5300 2904 615b 0200 0043 7265  d...S.).a[...Cre
-00003ce0: 6174 6573 2061 6e20 5f61 7374 2e49 6620  ates an _ast.If 
-00003cf0: 6e6f 6465 2e0a 0a20 2041 7267 733a 0a20  node...  Args:. 
-00003d00: 2020 2063 6f6e 6469 7469 6f6e 616c 3a20     conditional: 
-00003d10: 5468 6520 6578 7072 6573 7369 6f6e 2077  The expression w
-00003d20: 6520 6576 616c 7561 7465 2066 6f72 2069  e evaluate for i
-00003d30: 7473 2074 7275 7468 696e 6573 732e 0a20  ts truthiness.. 
-00003d40: 2020 2062 6f64 793a 2054 6865 206c 6973     body: The lis
-00003d50: 7420 6f66 206e 6f64 6573 2074 6861 7420  t of nodes that 
-00003d60: 6d61 6b65 2075 7020 7468 6520 626f 6479  make up the body
-00003d70: 206f 6620 7468 6520 6966 2073 7461 7465   of the if state
-00003d80: 6d65 6e74 2e0a 2020 2020 2020 4578 6563  ment..      Exec
-00003d90: 7574 6564 2069 6620 5472 7565 2e0a 2020  uted if True..  
-00003da0: 2020 6f72 656c 7365 3a20 7b5b 5f61 7374    orelse: {[_ast
-00003db0: 2e49 665d 7c5b 5f61 7374 2e73 746d 745d  .If]|[_ast.stmt]
-00003dc0: 7c4e 6f6e 657d 2045 6974 6865 7220 616e  |None} Either an
-00003dd0: 6f74 6865 7220 4966 2073 7461 7465 6d65  other If stateme
-00003de0: 6e74 2061 7320 7468 650a 2020 2020 2020  nt as the.      
-00003df0: 6f6e 6c79 2065 6c65 6d65 6e74 2069 6e20  only element in 
-00003e00: 6120 6c69 7374 2c20 2869 6e20 7768 6963  a list, (in whic
-00003e10: 6820 6361 7365 2074 6869 7320 6265 636f  h case this beco
-00003e20: 6d65 7320 616e 2065 6c69 6629 2c20 6120  mes an elif), a 
-00003e30: 6c69 7374 206f 660a 2020 2020 2020 7374  list of.      st
-00003e40: 6d74 206e 6f64 6573 2028 696e 2077 6869  mt nodes (in whi
-00003e50: 6368 2063 6173 6520 7468 6973 2069 7320  ch case this is 
-00003e60: 616e 2065 6c73 6529 2c20 6f72 204e 6f6e  an else), or Non
-00003e70: 6520 2869 6e20 7768 6963 6820 6361 7365  e (in which case
-00003e80: 2c20 7468 6572 650a 2020 2020 2020 6973  , there.      is
-00003e90: 206f 6e6c 7920 7468 6520 6966 290a 0a20   only the if).. 
-00003ea0: 2052 6169 7365 733a 0a20 2020 2056 616c   Raises:.    Val
-00003eb0: 7565 4572 726f 723a 2049 6620 7468 6520  ueError: If the 
-00003ec0: 626f 6479 206f 7220 6f72 656c 7365 2061  body or orelse a
-00003ed0: 7265 206c 6973 7473 2077 6869 6368 2063  re lists which c
-00003ee0: 6f6e 7461 696e 2065 6c65 6d65 6e74 7320  ontain elements 
-00003ef0: 6e6f 740a 2020 2020 2020 696e 6865 7269  not.      inheri
-00003f00: 7469 6e67 2066 726f 6d20 5f61 7374 2e73  ting from _ast.s
-00003f10: 746d 742e 0a0a 2020 5265 7475 726e 733a  tmt...  Returns:
-00003f20: 0a20 2020 2041 6e20 5f61 7374 2e49 6620  .    An _ast.If 
-00003f30: 6e6f 6465 2e0a 2020 4e72 4c00 0000 2903  node..  NrL...).
-00003f40: 726c 0000 0072 1b00 0000 da06 6f72 656c  rl...r......orel
-00003f50: 7365 2909 7251 0000 0072 1c00 0000 7230  se).rQ...r....r0
-00003f60: 0000 0072 7200 0000 7239 0000 0072 4e00  ...rr...r9...rN.
-00003f70: 0000 7231 0000 0072 4f00 0000 721d 0000  ..r1...rO...r...
-00003f80: 0029 04da 0b63 6f6e 6469 7469 6f6e 616c  .)...conditional
-00003f90: 721b 0000 0072 c900 0000 7250 0000 0072  r....r....rP...r
-00003fa0: 0800 0000 7208 0000 0072 0900 0000 721d  ....r....r....r.
-00003fb0: 0000 0044 0200 0073 1800 0000 0813 0801  ...D...s........
-00003fc0: 0401 0e01 0801 0c01 0201 0201 0602 04fd  ................
-00003fd0: 02ff 1005 721d 0000 0063 0300 0000 0000  ....r....c......
-00003fe0: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00003ff0: 0000 7310 0000 0074 006a 017c 017c 007c  ..s....t.j.|.|.|
-00004000: 0264 018d 0353 0029 0261 4201 0000 4372  .d...S.).aB...Cr
-00004010: 6561 7465 7320 616e 205f 6173 742e 4966  eates an _ast.If
-00004020: 4578 7020 6e6f 6465 2e0a 0a20 204e 6f74  Exp node...  Not
-00004030: 6520 7468 6174 2074 6869 7320 6973 2070  e that this is p
-00004040: 7974 686f 6e27 7320 7465 726e 6172 7920  ython's ternary 
-00004050: 6f70 6572 6174 6f72 2c20 6e6f 7420 746f  operator, not to
-00004060: 2062 6520 636f 6e66 7573 6564 2077 6974   be confused wit
-00004070: 6820 5f61 7374 2e49 662e 0a0a 2020 4172  h _ast.If...  Ar
-00004080: 6773 3a0a 2020 2020 636f 6e64 6974 696f  gs:.    conditio
-00004090: 6e61 6c3a 2054 6865 2065 7870 7265 7373  nal: The express
-000040a0: 696f 6e20 7765 2065 7661 6c75 6174 6520  ion we evaluate 
-000040b0: 666f 7220 6974 7320 7472 7574 6869 6e65  for its truthine
-000040c0: 7373 2e0a 2020 2020 7472 7565 5f63 6173  ss..    true_cas
-000040d0: 653a 2057 6861 7420 746f 2064 6f20 6966  e: What to do if
-000040e0: 2063 6f6e 6469 7469 6f6e 616c 2069 7320   conditional is 
-000040f0: 5472 7565 2e0a 2020 2020 6661 6c73 655f  True..    false_
-00004100: 6361 7365 3a20 5768 6174 2074 6f20 646f  case: What to do
-00004110: 2069 6620 636f 6e64 6974 696f 6e61 6c20   if conditional 
-00004120: 6973 2046 616c 7365 2e0a 0a20 2052 6574  is False...  Ret
-00004130: 7572 6e73 3a0a 2020 2020 416e 205f 6173  urns:.    An _as
-00004140: 742e 4966 4578 7020 6e6f 6465 2e0a 2020  t.IfExp node..  
-00004150: 2903 721b 0000 0072 6c00 0000 72c9 0000  ).r....rl...r...
-00004160: 0029 0272 3900 0000 da05 4966 4578 7029  .).r9.....IfExp)
-00004170: 0372 ca00 0000 da09 7472 7565 5f63 6173  .r......true_cas
-00004180: 65da 0a66 616c 7365 5f63 6173 6572 0800  e..false_caser..
-00004190: 0000 7208 0000 0072 0900 0000 72cb 0000  ..r....r....r...
-000041a0: 0064 0200 0073 0200 0000 100d 72cb 0000  .d...s......r...
-000041b0: 00da 0063 0300 0000 0000 0000 0000 0000  ...c............
-000041c0: 0400 0000 0500 0000 4300 0000 7330 0000  ........C...s0..
-000041d0: 0074 006a 017c 007c 0264 018d 0267 017d  .t.j.|.|.d...g.}
-000041e0: 037c 0172 1274 006a 0264 027c 017c 0364  .|.r.t.j.d.|.|.d
-000041f0: 038d 0353 0074 006a 037c 0364 048d 0153  ...S.t.j.|.d...S
-00004200: 0029 0561 6301 0000 4372 6561 7465 7320  .).ac...Creates 
-00004210: 6569 7468 6572 2061 6e20 5f61 7374 2e49  either an _ast.I
-00004220: 6d70 6f72 7420 6e6f 6465 206f 7220 616e  mport node or an
-00004230: 205f 6173 742e 496d 706f 7274 4672 6f6d   _ast.ImportFrom
-00004240: 206e 6f64 652e 0a0a 2020 4172 6773 3a0a   node...  Args:.
-00004250: 2020 2020 696d 706f 7274 5f70 6172 743a      import_part:
-00004260: 2054 6865 2074 6578 7420 7468 6174 2066   The text that f
-00004270: 6f6c 6c6f 7773 2022 696d 706f 7274 222e  ollows "import".
-00004280: 0a20 2020 2066 726f 6d5f 7061 7274 3a20  .    from_part: 
-00004290: 5468 6520 7465 7874 2074 6861 7420 666f  The text that fo
-000042a0: 6c6c 6f77 7320 2266 726f 6d22 2e20 4f70  llows "from". Op
-000042b0: 7469 6f6e 616c 2e20 4465 7465 726d 696e  tional. Determin
-000042c0: 6573 2069 6620 7765 2077 696c 6c0a 2020  es if we will.  
-000042d0: 2020 2020 7265 7475 726e 2061 6e20 5f61      return an _a
-000042e0: 7374 2e49 6d70 6f72 7420 6f72 205f 6173  st.Import or _as
-000042f0: 742e 496d 706f 7274 4672 6f6d 206e 6f64  t.ImportFrom nod
-00004300: 652e 0a20 2020 2061 736e 616d 653a 2054  e..    asname: T
-00004310: 6578 7420 7468 6174 2066 6f6c 6c6f 7773  ext that follows
-00004320: 2022 6173 222e 204f 7074 696f 6e61 6c2e   "as". Optional.
-00004330: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
-00004340: 2041 6e20 5f61 7374 2e49 6d70 6f72 7420   An _ast.Import 
-00004350: 6f72 205f 6173 742e 496d 706f 7274 4672  or _ast.ImportFr
-00004360: 6f6d 206e 6f64 652e 0a20 2029 0272 9d00  om node..  ).r..
-00004370: 0000 da06 6173 6e61 6d65 7201 0000 0029  ....asnamer....)
-00004380: 03da 056c 6576 656c da06 6d6f 6475 6c65  ...level..module
-00004390: da05 6e61 6d65 7329 0172 d200 0000 2904  ..names).r....).
-000043a0: 7239 0000 00da 0561 6c69 6173 da0a 496d  r9.....alias..Im
-000043b0: 706f 7274 4672 6f6d da06 496d 706f 7274  portFrom..Import
-000043c0: 2904 da0b 696d 706f 7274 5f70 6172 74da  )...import_part.
-000043d0: 0966 726f 6d5f 7061 7274 72cf 0000 0072  .from_partr....r
-000043e0: d200 0000 7208 0000 0072 0800 0000 7209  ....r....r....r.
-000043f0: 0000 0072 d500 0000 7402 0000 7314 0000  ...r....t...s...
-00004400: 0006 0c02 0108 ff04 0204 0102 0102 0102  ................
-00004410: 0106 fd0c 0572 d500 0000 6300 0000 0000  .....r....c.....
-00004420: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
-00004430: 0000 0072 6800 0000 7238 0000 0029 0272  ...rh...r8...).r
-00004440: 3900 0000 da02 496e 7208 0000 0072 0800  9.....Inr....r..
-00004450: 0000 7208 0000 0072 0900 0000 72d8 0000  ..r....r....r...
-00004460: 008b 0200 0072 6a00 0000 72d8 0000 0063  .....rj...r....c
-00004470: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00004480: 0300 0000 4300 0000 f30a 0000 0074 00a0  ....C........t..
-00004490: 017c 00a1 0153 0072 3800 0000 2902 7239  .|...S.r8...).r9
-000044a0: 0000 00da 0549 6e64 6578 72be 0000 0072  .....Indexr....r
-000044b0: 0800 0000 7208 0000 0072 0900 0000 72da  ....r....r....r.
-000044c0: 0000 008f 0200 00f3 0200 0000 0a01 72da  ..............r.
-000044d0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000044e0: 0000 0000 0200 0000 4300 0000 7268 0000  ........C...rh..
-000044f0: 0072 3800 0000 2902 7239 0000 00da 0649  .r8...).r9.....I
-00004500: 6e76 6572 7472 0800 0000 7208 0000 0072  nvertr....r....r
-00004510: 0800 0000 7209 0000 0072 dc00 0000 9302  ....r....r......
-00004520: 0000 726a 0000 0072 dc00 0000 6300 0000  ..rj...r....c...
-00004530: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00004540: 0043 0000 0072 6800 0000 7238 0000 0029  .C...rh...r8...)
-00004550: 0272 3900 0000 da02 4973 7208 0000 0072  .r9.....Isr....r
-00004560: 0800 0000 7208 0000 0072 0900 0000 72dd  ....r....r....r.
-00004570: 0000 0097 0200 0072 6a00 0000 72dd 0000  .......rj...r...
-00004580: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00004590: 0000 0200 0000 4300 0000 7268 0000 0072  ......C...rh...r
-000045a0: 3800 0000 2902 7239 0000 00da 0549 734e  8...).r9.....IsN
-000045b0: 6f74 7208 0000 0072 0800 0000 7208 0000  otr....r....r...
-000045c0: 0072 0900 0000 72de 0000 009b 0200 0072  .r....r........r
-000045d0: 6a00 0000 72de 0000 0063 0200 0000 0000  j...r....c......
-000045e0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-000045f0: 0000 732e 0000 0074 007c 0074 0174 0266  ..s....t.|.t.t.f
-00004600: 0283 0272 0b74 0364 0183 0182 0174 047c  ...r.t.d.....t.|
-00004610: 0164 028d 017d 0274 056a 067c 027c 0064  .d...}.t.j.|.|.d
-00004620: 038d 0253 0029 047a af43 7265 6174 6573  ...S.).z.Creates
-00004630: 2061 6e20 5f61 7374 2e4c 616d 6264 6120   an _ast.Lambda 
-00004640: 6f62 6a65 6374 2e0a 0a20 2041 7267 733a  object...  Args:
-00004650: 0a20 2020 2062 6f64 793a 207b 5f61 7374  .    body: {_ast
-00004660: 2e41 5354 7d0a 2020 2020 6172 6773 3a20  .AST}.    args: 
-00004670: 7b5f 6173 742e 6172 6775 6d65 6e74 737d  {_ast.arguments}
-00004680: 0a0a 2020 5261 6973 6573 3a0a 2020 2020  ..  Raises:.    
-00004690: 5661 6c75 6545 7272 6f72 3a20 4966 2062  ValueError: If b
-000046a0: 6f64 7920 6973 2061 206c 6973 7420 6f72  ody is a list or
-000046b0: 2074 7570 6c65 2e0a 0a20 2052 6574 7572   tuple...  Retur
-000046c0: 6e73 3a0a 2020 2020 7b5f 6173 742e 4c61  ns:.    {_ast.La
-000046d0: 6d62 6461 7d0a 2020 7a34 426f 6479 2073  mbda}.  z4Body s
-000046e0: 686f 756c 6420 6265 2061 2073 696e 676c  hould be a singl
-000046f0: 6520 656c 656d 656e 742c 206e 6f74 2061  e element, not a
-00004700: 206c 6973 7420 6f72 2074 7570 6c65 2901   list or tuple).
-00004710: 7235 0000 0029 0272 3500 0000 721b 0000  r5...).r5...r...
-00004720: 0029 0772 1c00 0000 7230 0000 0072 7200  .).r....r0...rr.
-00004730: 0000 7231 0000 0072 6700 0000 7239 0000  ..r1...rg...r9..
-00004740: 00da 064c 616d 6264 6129 0372 1b00 0000  ...Lambda).r....
-00004750: 7235 0000 00da 0b6c 616d 6264 615f 6172  r5.....lambda_ar
-00004760: 6773 7208 0000 0072 0800 0000 7209 0000  gsr....r....r...
-00004770: 0072 df00 0000 9f02 0000 7308 0000 000e  .r........s.....
-00004780: 0d08 010a 030e 0172 df00 0000 6300 0000  .......r....c...
-00004790: 0000 0000 0000 0000 0006 0000 0004 0000  ................
-000047a0: 004f 0000 0073 6800 0000 7c01 a000 6401  .O...sh...|...d.
-000047b0: 7401 6a02 a102 7d02 7c00 4400 5d1d 7d03  t.j...}.|.D.].}.
-000047c0: 7403 7c03 7404 6a05 8302 7217 7406 7c02  t.|.t.j...r.t.|.
-000047d0: 8301 7c03 5f07 7109 7403 7c03 7404 6a08  ..|._.q.t.|.t.j.
-000047e0: 8302 7226 7409 7c03 8301 7d04 7406 7c02  ..r&t.|...}.t.|.
-000047f0: 8301 7c04 5f07 7109 7406 7c02 8301 7d05  ..|._.q.t.|...}.
-00004800: 7404 6a0a 740b 7c00 8301 7c05 6402 8d02  t.j.t.|...|.d...
-00004810: 5300 2903 6105 0100 0043 7265 6174 6573  S.).a....Creates
-00004820: 2061 6e20 5f61 7374 2e4c 6973 7420 6e6f   an _ast.List no
-00004830: 6465 2e0a 0a20 2041 7574 6f6d 6174 6963  de...  Automatic
-00004840: 616c 6c79 2061 646a 7573 7473 2069 6e6e  ally adjusts inn
-00004850: 6572 2063 7478 2061 7474 7273 2e0a 0a20  er ctx attrs... 
-00004860: 2041 7267 733a 0a20 2020 202a 6974 656d   Args:.    *item
-00004870: 733a 2054 6865 2069 7465 6d73 2069 6e20  s: The items in 
-00004880: 7468 6520 6c69 7374 2e0a 2020 2020 2a2a  the list..    **
-00004890: 6b77 6172 6773 3a20 4f6e 6c79 2072 6563  kwargs: Only rec
-000048a0: 6f67 6e69 7a65 6420 6b77 6172 6720 6973  ognized kwarg is
-000048b0: 2027 6374 785f 7479 7065 272c 2077 6869   'ctx_type', whi
-000048c0: 6368 2063 6f6e 7472 6f6c 7320 7468 650a  ch controls the.
-000048d0: 2020 2020 2020 6374 7820 7479 7065 206f        ctx type o
-000048e0: 6620 7468 6520 6c69 7374 2e20 5365 6520  f the list. See 
-000048f0: 4374 7845 6e75 6d2e 0a0a 2020 5265 7475  CtxEnum...  Retu
-00004900: 726e 733a 0a20 2020 2041 6e20 5f61 7374  rns:.    An _ast
-00004910: 2e4c 6973 7420 6e6f 6465 2e0a 2020 723f  .List node..  r?
-00004920: 0000 00a9 02da 0465 6c74 7372 5a00 0000  .......eltsrZ...
-00004930: 290c 7282 0000 0072 7300 0000 7214 0000  ).r....rs...r...
-00004940: 0072 1c00 0000 7239 0000 0072 4300 0000  .r....r9...rC...
-00004950: 725c 0000 0072 5a00 0000 729a 0000 0072  r\...rZ...r....r
-00004960: 4b00 0000 da04 4c69 7374 7230 0000 0029  K.....Listr0...)
-00004970: 06da 0569 7465 6d73 7296 0000 0072 3f00  ...itemsr....r?.
-00004980: 0000 da04 6974 656d da09 6e61 6d65 5f6e  ....item..name_n
-00004990: 6f64 6572 5a00 0000 7208 0000 0072 0800  oderZ...r....r..
-000049a0: 0000 7209 0000 0072 e300 0000 b402 0000  ..r....r........
-000049b0: 7318 0000 000e 0d08 020c 010c 010c 0108  s...............
-000049c0: 010a 0102 8008 010a 0102 0106 ff72 e300  .............r..
-000049d0: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
-000049e0: 0000 0006 0000 0047 0000 00f3 4a00 0000  .......G....J...
-000049f0: 7400 7c00 7401 6a02 6401 8d02 7d00 7400  t.|.t.j.d...}.t.
-00004a00: 7c01 7401 6a03 6401 8d02 7d01 7400 7c02  |.t.j.d...}.t.|.
-00004a10: 7401 6a02 6401 8d02 7d02 7404 6a05 7c00  t.j.d...}.t.j.|.
-00004a20: 7406 7c01 7c02 6402 6703 7c03 a201 5200  t.|.|.d.g.|...R.
-00004a30: 8e00 6701 6403 8d02 5300 2904 614b 0100  ..g.d...S.).aK..
-00004a40: 0043 7265 6174 6573 205f 6173 742e 4c69  .Creates _ast.Li
-00004a50: 7374 436f 6d70 206e 6f64 6573 2e0a 0a20  stComp nodes... 
-00004a60: 2027 6c65 6674 5f73 6964 6527 2066 6f72   'left_side' for
-00004a70: 2027 666f 725f 7061 7274 2720 696e 2027   'for_part' in '
-00004a80: 696e 5f70 6172 7427 2069 6620 2769 6673  in_part' if 'ifs
-00004a90: 270a 0a20 2041 7267 733a 0a20 2020 206c  '..  Args:.    l
-00004aa0: 6566 745f 7369 6465 3a20 6c65 6674 6d6f  eft_side: leftmo
-00004ab0: 7374 2073 6964 6520 6f66 2074 6865 2065  st side of the e
-00004ac0: 7870 7265 7373 696f 6e2e 0a20 2020 2066  xpression..    f
-00004ad0: 6f72 5f70 6172 743a 2054 6865 2070 6172  or_part: The par
-00004ae0: 7420 6166 7465 7220 275b 6c65 6674 5f73  t after '[left_s
-00004af0: 6964 655d 2066 6f72 2027 0a20 2020 2069  ide] for '.    i
-00004b00: 6e5f 7061 7274 3a20 5468 6520 7061 7274  n_part: The part
-00004b10: 2061 6674 6572 2027 5b6c 6566 745f 7369   after '[left_si
-00004b20: 6465 5d20 666f 7220 5b66 6f72 5f70 6172  de] for [for_par
-00004b30: 745d 2069 6e20 270a 2020 2020 2a69 6673  t] in '.    *ifs
-00004b40: 3a20 416e 7920 6966 2073 7461 7465 6d65  : Any if stateme
-00004b50: 6e74 7320 7468 6174 2063 6f6d 6520 6174  nts that come at
-00004b60: 2074 6865 2065 6e64 2e0a 0a20 2052 6574   the end...  Ret
-00004b70: 7572 6e73 3a0a 2020 2020 7b5f 6173 742e  urns:.    {_ast.
-00004b80: 4c69 7374 436f 6d70 7d0a 2020 723e 0000  ListComp}.  r>..
-00004b90: 0046 72c3 0000 0029 0772 2e00 0000 7273  .Fr....).r....rs
-00004ba0: 0000 0072 1400 0000 7215 0000 0072 3900  ...r....r....r9.
-00004bb0: 0000 da08 4c69 7374 436f 6d70 72af 0000  ....ListCompr...
-00004bc0: 00a9 0472 c600 0000 72b0 0000 0072 b100  ...r....r....r..
-00004bd0: 0000 72ad 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00004be0: 0072 0900 0000 72e8 0000 00ce 0200 00f3  .r....r.........
-00004bf0: 0e00 0000 0e0e 0e01 0e01 0401 0201 1401  ................
-00004c00: 06fe 72e8 0000 0063 0000 0000 0000 0000  ..r....c........
-00004c10: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
-00004c20: 7268 0000 0072 3800 0000 2902 7239 0000  rh...r8...).r9..
-00004c30: 00da 064c 5368 6966 7472 0800 0000 7208  ...LShiftr....r.
-00004c40: 0000 0072 0800 0000 7209 0000 0072 eb00  ...r....r....r..
-00004c50: 0000 e402 0000 726a 0000 0072 eb00 0000  ......rj...r....
-00004c60: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00004c70: 0002 0000 0043 0000 0072 6800 0000 7238  .....C...rh...r8
-00004c80: 0000 0029 0272 3900 0000 da02 4c74 7208  ...).r9.....Ltr.
-00004c90: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00004ca0: 0000 72ec 0000 00e8 0200 0072 6a00 0000  ..r........rj...
-00004cb0: 72ec 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00004cc0: 0000 0000 0000 0200 0000 4300 0000 7268  ..........C...rh
-00004cd0: 0000 0072 3800 0000 2902 7239 0000 00da  ...r8...).r9....
-00004ce0: 034c 7445 7208 0000 0072 0800 0000 7208  .LtEr....r....r.
-00004cf0: 0000 0072 0900 0000 72ed 0000 00ec 0200  ...r....r.......
-00004d00: 0072 6a00 0000 72ed 0000 0063 0000 0000  .rj...r....c....
-00004d10: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00004d20: 4300 0000 7268 0000 0072 3800 0000 2902  C...rh...r8...).
-00004d30: 7239 0000 00da 034d 6f64 7208 0000 0072  r9.....Modr....r
-00004d40: 0800 0000 7208 0000 0072 0900 0000 72ee  ....r....r....r.
-00004d50: 0000 00f0 0200 0072 6a00 0000 72ee 0000  .......rj...r...
-00004d60: 0063 0000 0000 0000 0000 0000 0000 0100  .c..............
-00004d70: 0000 0300 0000 4700 0000 731c 0000 007c  ......G...s....|
-00004d80: 0073 0674 0064 0183 0182 0174 016a 0274  .s.t.d.....t.j.t
-00004d90: 037c 0083 0164 028d 0153 0029 034e 7a2b  .|...d...S.).Nz+
-00004da0: 4d75 7374 2068 6176 6520 6174 206c 6561  Must have at lea
-00004db0: 7374 206f 6e65 2061 7267 756d 656e 7420  st one argument 
-00004dc0: 696e 2074 6865 2062 6f64 7929 0172 1b00  in the body).r..
-00004dd0: 0000 2904 7231 0000 0072 3900 0000 da06  ..).r1...r9.....
-00004de0: 4d6f 6475 6c65 7230 0000 0029 01da 0a62  Moduler0...)...b
-00004df0: 6f64 795f 6974 656d 7372 0800 0000 7208  ody_itemsr....r.
-00004e00: 0000 0072 0900 0000 72ef 0000 00f4 0200  ...r....r.......
-00004e10: 0073 0600 0000 0401 0801 1001 72ef 0000  .s..........r...
-00004e20: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00004e30: 0000 0200 0000 4300 0000 7268 0000 0072  ......C...rh...r
-00004e40: 3800 0000 2902 7239 0000 00da 044d 756c  8...).r9.....Mul
-00004e50: 7472 0800 0000 7208 0000 0072 0800 0000  tr....r....r....
-00004e60: 7209 0000 0072 f100 0000 fa02 0000 726a  r....r........rj
-00004e70: 0000 0072 f100 0000 6301 0000 0000 0000  ...r....c.......
-00004e80: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00004e90: 0072 d900 0000 7238 0000 0029 0272 3900  .r....r8...).r9.
-00004ea0: 0000 722a 0000 0029 0172 2a00 0000 7208  ..r*...).r*...r.
-00004eb0: 0000 0072 0800 0000 7209 0000 0072 3b00  ...r....r....r;.
-00004ec0: 0000 fe02 0000 72db 0000 0072 3b00 0000  ......r....r;...
-00004ed0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00004ee0: 0003 0000 0043 0000 00f3 0c00 0000 7400  .....C........t.
-00004ef0: 6a01 7c00 6401 8d01 5300 2902 4e72 be00  j.|.d...S.).Nr..
-00004f00: 0000 a902 7239 0000 0072 4100 0000 72be  ....r9...rA...r.
-00004f10: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00004f20: 0000 7241 0000 0002 0300 0072 0f00 0000  ..rA.......r....
-00004f30: 7241 0000 0063 0100 0000 0000 0000 0000  rA...c..........
-00004f40: 0000 0300 0000 0400 0000 4300 0000 735e  ..........C...s^
-00004f50: 0000 0074 007c 0074 0183 0273 0974 0264  ...t.|.t...s.t.d
-00004f60: 0183 0182 017c 0064 0075 0073 137c 0064  .....|.d.u.s.|.d
-00004f70: 0219 00a0 03a1 0072 1a74 0264 037c 009b  .......r.t.d.|..
-00004f80: 009d 0283 0182 017c 00a0 0464 0464 05a1  .......|...d.d..
-00004f90: 027d 017c 01a0 05a1 007d 027c 0273 2d74  .}.|.....}.|.s-t
-00004fa0: 0264 037c 009b 009d 0283 0182 0164 0053  .d.|.........d.S
-00004fb0: 0029 064e 7a1a 7079 7468 6f6e 2069 6420  .).Nz.python id 
-00004fc0: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
-00004fd0: 7201 0000 007a 1349 6e76 616c 6964 2070  r....z.Invalid p
-00004fe0: 7974 686f 6e20 6964 3a20 da01 5f72 ce00  ython id: .._r..
-00004ff0: 0000 2906 721c 0000 0072 4200 0000 7231  ..).r....rB...r1
-00005000: 0000 00da 0769 7364 6967 6974 da07 7265  .....isdigit..re
-00005010: 706c 6163 65da 0769 7361 6c6e 756d 2903  place..isalnum).
-00005020: da07 6e61 6d65 5f69 64da 1373 7472 6970  ..name_id..strip
-00005030: 7065 645f 756e 6465 7273 636f 7265 72f7  ped_underscorer.
-00005040: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00005050: 0000 da0b 7661 6c69 6461 7465 5f69 6406  ....validate_id.
-00005060: 0300 0073 1200 0000 0a01 0801 1401 0e01  ...s............
-00005070: 0c01 0801 0401 0e01 04ff 72fa 0000 0063  ..........r....c
-00005080: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00005090: 0400 0000 4300 0000 731e 0000 0074 007c  ....C...s....t.|
-000050a0: 0083 0101 0074 017c 0183 017d 0274 026a  .....t.|...}.t.j
-000050b0: 037c 007c 0264 018d 0253 0029 027a 8f43  .|.|.d...S.).z.C
-000050c0: 7265 6174 6573 2061 6e20 5f61 7374 2e4e  reates an _ast.N
-000050d0: 616d 6520 6e6f 6465 2e0a 0a20 2041 7267  ame node...  Arg
-000050e0: 733a 0a20 2020 206e 616d 655f 6964 3a20  s:.    name_id: 
-000050f0: 4e61 6d65 206f 6620 7468 6520 6e6f 6465  Name of the node
-00005100: 2e0a 2020 2020 6374 785f 7479 7065 3a20  ..    ctx_type: 
-00005110: 5365 6520 4374 7845 6e75 6d20 666f 7220  See CtxEnum for 
-00005120: 6f70 7469 6f6e 732e 0a0a 2020 5265 7475  options...  Retu
-00005130: 726e 733a 0a20 2020 2041 6e20 5f61 7374  rns:.    An _ast
-00005140: 2e4e 616d 6520 6e6f 6465 2e0a 2020 a902  .Name node..  ..
-00005150: 7248 0000 0072 5a00 0000 2904 72fa 0000  rH...rZ...).r...
-00005160: 0072 5c00 0000 7239 0000 0072 4300 0000  .r\...r9...rC...
-00005170: 2903 72f8 0000 0072 3f00 0000 725a 0000  ).r....r?...rZ..
-00005180: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-00005190: 7243 0000 0011 0300 0073 0a00 0000 080a  rC.......s......
-000051a0: 0801 0601 0201 06ff 7243 0000 0063 0000  ........rC...c..
-000051b0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-000051c0: 0000 4300 0000 7268 0000 0072 3800 0000  ..C...rh...r8...
-000051d0: 2902 7239 0000 00da 034e 6f74 7208 0000  ).r9.....Notr...
-000051e0: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-000051f0: 72fc 0000 0025 0300 0072 6a00 0000 72fc  r....%...rj...r.
-00005200: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00005210: 0000 0000 0200 0000 4300 0000 7268 0000  ........C...rh..
-00005220: 0072 3800 0000 2902 7239 0000 00da 054e  .r8...).r9.....N
-00005230: 6f74 4571 7208 0000 0072 0800 0000 7208  otEqr....r....r.
-00005240: 0000 0072 0900 0000 72fd 0000 0029 0300  ...r....r....)..
-00005250: 0072 6a00 0000 72fd 0000 0063 0000 0000  .rj...r....c....
-00005260: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00005270: 4300 0000 7268 0000 0072 3800 0000 2902  C...rh...r8...).
-00005280: 7239 0000 00da 054e 6f74 496e 7208 0000  r9.....NotInr...
-00005290: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-000052a0: 72fe 0000 002d 0300 0072 6a00 0000 72fe  r....-...rj...r.
-000052b0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000052c0: 0300 0000 0400 0000 4300 0000 7336 0000  ........C...s6..
-000052d0: 0074 007c 0074 0183 0273 0974 0264 0183  .t.|.t...s.t.d..
-000052e0: 0182 0174 037c 0083 017d 0174 046a 0574  ...t.|...}.t.j.t
-000052f0: 067c 007c 0183 0264 028d 017d 027c 017c  .|.|...d...}.|.|
-00005300: 025f 077c 0253 0029 03fa 1e43 7265 6174  ._.|.S.)...Creat
-00005310: 6573 2061 6e20 5f61 7374 2e43 6f6e 7374  es an _ast.Const
-00005320: 616e 7420 6e6f 6465 2e7a 256e 756d 6265  ant node.z%numbe
-00005330: 7220 6d75 7374 2062 6520 6120 7374 7220  r must be a str 
-00005340: 746f 2073 7570 706f 7274 2062 6173 6573  to support bases
-00005350: 72be 0000 0029 0872 1c00 0000 7242 0000  r....).r....rB..
-00005360: 0072 3100 0000 7274 0000 0072 3900 0000  .r1...rt...r9...
-00005370: 7241 0000 0072 4000 0000 7276 0000 0029  rA...r@...rv...)
-00005380: 03da 066e 756d 6265 7272 7600 0000 727b  ...numberrv...r{
-00005390: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-000053a0: 0000 da03 4e75 6d31 0300 0073 0c00 0000  ....Num1...s....
-000053b0: 0a02 0801 0801 1201 0601 0401 7201 0100  ............r...
-000053c0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000053d0: 0000 0300 0000 4300 0000 734a 0000 0074  ......C...sJ...t
-000053e0: 007c 0083 01a0 0164 01a1 0172 0b64 027d  .|.....d...r.d.}
-000053f0: 017c 0153 0074 007c 0083 01a0 0164 03a1  .|.S.t.|.....d..
-00005400: 0172 1664 047d 017c 0153 0074 007c 0083  .r.d.}.|.S.t.|..
-00005410: 01a0 0164 05a1 0172 2164 067d 017c 0153  ...d...r!d.}.|.S
-00005420: 0064 077d 017c 0153 0029 084e da02 3062  .d.}.|.S.).N..0b
-00005430: 72a2 0000 00da 0230 6fe9 0800 0000 da02  r......0o.......
-00005440: 3078 e910 0000 00e9 0a00 0000 2902 7242  0x..........).rB
-00005450: 0000 00da 0a73 7461 7274 7377 6974 6829  .....startswith)
-00005460: 0272 0001 0000 7276 0000 0072 0800 0000  .r....rv...r....
-00005470: 7208 0000 0072 0900 0000 7274 0000 003b  r....r....rt...;
-00005480: 0300 0073 1600 0000 0e01 0401 0407 0efa  ...s............
-00005490: 0401 0405 0efc 0401 0403 04ff 0401 7274  ..............rt
-000054a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000054b0: 0100 0000 0400 0000 4300 0000 730e 0000  ........C...s...
-000054c0: 0074 00a0 0174 027c 0083 01a1 0153 0029  .t...t.|.....S.)
-000054d0: 0172 ff00 0000 2903 7239 0000 0072 4100  .r....).r9...rA.
-000054e0: 0000 da04 626f 6f6c 2901 da07 626f 6f6c  ....bool)...bool
-000054f0: 6561 6e72 0800 0000 7208 0000 0072 0900  eanr....r....r..
-00005500: 0000 da04 426f 6f6c 4703 0000 7302 0000  ....BoolG...s...
-00005510: 000e 0272 0b01 0000 6300 0000 0000 0000  ...r....c.......
-00005520: 0000 0000 0000 0000 0002 0000 0043 0000  .............C..
-00005530: 0072 6800 0000 7238 0000 0029 0272 3900  .rh...r8...).r9.
-00005540: 0000 7285 0000 0072 0800 0000 7208 0000  ..r....r....r...
-00005550: 0072 0800 0000 7209 0000 0072 8500 0000  .r....r....r....
-00005560: 4b03 0000 726a 0000 0072 8500 0000 6300  K...rj...r....c.
-00005570: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00005580: 0000 0043 0000 0072 6800 0000 2901 7a1a  ...C...rh...).z.
-00005590: 4372 6561 7465 7320 616e 205f 6173 742e  Creates an _ast.
-000055a0: 5061 7373 206e 6f64 652e 2902 7239 0000  Pass node.).r9..
-000055b0: 0072 4d00 0000 7208 0000 0072 0800 0000  .rM...r....r....
-000055c0: 7208 0000 0072 0900 0000 724d 0000 004f  r....r....rM...O
-000055d0: 0300 0073 0200 0000 0802 724d 0000 0063  ...s......rM...c
-000055e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000055f0: 0200 0000 4300 0000 7268 0000 0072 3800  ....C...rh...r8.
-00005600: 0000 2902 7239 0000 00da 0350 6f77 7208  ..).r9.....Powr.
-00005610: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00005620: 0000 720c 0100 0054 0300 0072 6a00 0000  ..r....T...rj...
-00005630: 720c 0100 0063 0100 0000 0000 0000 0000  r....c..........
-00005640: 0000 0200 0000 0300 0000 4300 0000 7356  ..........C...sV
-00005650: 0000 0074 007c 0074 0183 0272 0c74 0274  ...t.|.t...r.t.t
-00005660: 037c 0083 0183 017d 016e 1974 007c 0074  .|.....}.n.t.|.t
-00005670: 0383 0272 1674 047c 0083 017d 016e 0f74  ...r.t.|...}.n.t
-00005680: 007c 0074 056a 0683 0272 2174 05a0 077c  .|.t.j...r!t...|
-00005690: 00a1 0153 0074 0864 0183 0182 0174 056a  ...S.t.d.....t.j
-000056a0: 077c 0164 028d 0153 0029 034e 7a14 496e  .|.d...S.).Nz.In
-000056b0: 7661 6c69 6420 7265 7475 726e 2076 616c  valid return val
-000056c0: 7565 72be 0000 0029 0972 1c00 0000 7240  uer....).r....r@
-000056d0: 0000 0072 0101 0000 7242 0000 00da 0353  ...r....rB.....S
-000056e0: 7472 7239 0000 0072 3a00 0000 da06 5265  trr9...r:.....Re
-000056f0: 7475 726e 7231 0000 0029 0272 4900 0000  turnr1...).rI...
-00005700: da0a 7661 6c75 655f 6e6f 6465 7208 0000  ..value_noder...
-00005710: 0072 0800 0000 7209 0000 0072 0e01 0000  .r....r....r....
-00005720: 5803 0000 7310 0000 000a 010e 010a 010a  X...s...........
-00005730: 010c 010a 0108 020c 0172 0e01 0000 6300  .........r....c.
-00005740: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00005750: 0000 0043 0000 0072 6800 0000 7238 0000  ...C...rh...r8..
-00005760: 0029 0272 3900 0000 da06 5253 6869 6674  .).r9.....RShift
-00005770: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00005780: 0900 0000 7210 0100 0063 0300 0072 6a00  ....r....c...rj.
-00005790: 0000 7210 0100 0063 0000 0000 0000 0000  ..r....c........
-000057a0: 0000 0000 0100 0000 0300 0000 4700 0000  ............G...
-000057b0: 7310 0000 0074 006a 0174 027c 0083 0164  s....t.j.t.|...d
-000057c0: 018d 0153 0029 027a 6943 7265 6174 6573  ...S.).ziCreates
-000057d0: 2061 6e20 5f61 7374 2e53 6574 206e 6f64   an _ast.Set nod
-000057e0: 652e 0a0a 2020 4172 6773 3a0a 2020 2020  e...  Args:.    
-000057f0: 2a69 7465 6d73 3a20 5468 6520 6974 656d  *items: The item
-00005800: 7320 696e 2074 6865 2073 6574 2e0a 0a20  s in the set... 
-00005810: 2052 6574 7572 6e73 3a0a 2020 2020 416e   Returns:.    An
-00005820: 205f 6173 742e 5365 7420 6e6f 6465 2e0a   _ast.Set node..
-00005830: 2020 2901 72e2 0000 0029 0372 3900 0000    ).r....).r9...
-00005840: da03 5365 7472 3000 0000 2901 72e4 0000  ..Setr0...).r...
-00005850: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-00005860: 7211 0100 0067 0300 0073 0200 0000 1009  r....g...s......
-00005870: 7211 0100 0063 0300 0000 0000 0000 0000  r....c..........
-00005880: 0000 0400 0000 0600 0000 4700 0000 72e7  ..........G...r.
-00005890: 0000 0029 0461 4901 0000 4372 6561 7465  ...).aI...Create
-000058a0: 7320 5f61 7374 2e53 6574 436f 6d70 206e  s _ast.SetComp n
-000058b0: 6f64 6573 2e0a 0a20 2027 6c65 6674 5f73  odes...  'left_s
-000058c0: 6964 6527 2066 6f72 2027 666f 725f 7061  ide' for 'for_pa
-000058d0: 7274 2720 696e 2027 696e 5f70 6172 7427  rt' in 'in_part'
-000058e0: 2069 6620 2769 6673 270a 0a20 2041 7267   if 'ifs'..  Arg
-000058f0: 733a 0a20 2020 206c 6566 745f 7369 6465  s:.    left_side
-00005900: 3a20 6c65 6674 6d6f 7374 2073 6964 6520  : leftmost side 
-00005910: 6f66 2074 6865 2065 7870 7265 7373 696f  of the expressio
-00005920: 6e2e 0a20 2020 2066 6f72 5f70 6172 743a  n..    for_part:
-00005930: 2054 6865 2070 6172 7420 6166 7465 7220   The part after 
-00005940: 275b 6c65 6674 5f73 6964 655d 2066 6f72  '[left_side] for
-00005950: 2027 0a20 2020 2069 6e5f 7061 7274 3a20   '.    in_part: 
-00005960: 5468 6520 7061 7274 2061 6674 6572 2027  The part after '
-00005970: 5b6c 6566 745f 7369 6465 5d20 666f 7220  [left_side] for 
-00005980: 5b66 6f72 5f70 6172 745d 2069 6e20 270a  [for_part] in '.
-00005990: 2020 2020 2a69 6673 3a20 416e 7920 6966      *ifs: Any if
-000059a0: 2073 7461 7465 6d65 6e74 7320 7468 6174   statements that
-000059b0: 2063 6f6d 6520 6174 2074 6865 2065 6e64   come at the end
-000059c0: 2e0a 0a20 2052 6574 7572 6e73 3a0a 2020  ...  Returns:.  
-000059d0: 2020 7b5f 6173 742e 5365 7443 6f6d 707d    {_ast.SetComp}
-000059e0: 0a20 2072 3e00 0000 4672 c300 0000 2907  .  r>...Fr....).
-000059f0: 722e 0000 0072 7300 0000 7214 0000 0072  r....rs...r....r
-00005a00: 1500 0000 7239 0000 00da 0753 6574 436f  ....r9.....SetCo
-00005a10: 6d70 72af 0000 0072 e900 0000 7208 0000  mpr....r....r...
-00005a20: 0072 0800 0000 7209 0000 0072 1201 0000  .r....r....r....
-00005a30: 7303 0000 72ea 0000 0072 1201 0000 6303  s...r....r....c.
-00005a40: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00005a50: 0000 0043 0000 0073 1000 0000 7400 6a01  ...C...s....t.j.
-00005a60: 7c00 7c01 7c02 6401 8d03 5300 2902 4ea9  |.|.|.d...S.).N.
-00005a70: 03da 056c 6f77 6572 da05 7570 7065 72da  ...lower..upper.
-00005a80: 0473 7465 7029 0272 3900 0000 da05 536c  .step).r9.....Sl
-00005a90: 6963 6572 1301 0000 7208 0000 0072 0800  icer....r....r..
-00005aa0: 0000 7209 0000 0072 1701 0000 8903 0000  ..r....r........
-00005ab0: 7302 0000 0010 0172 1701 0000 6301 0000  s......r....c...
-00005ac0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00005ad0: 0043 0000 0072 f200 0000 2902 7a19 4372  .C...r....).z.Cr
-00005ae0: 6561 7465 7320 616e 205f 6173 742e 5374  eates an _ast.St
-00005af0: 7220 6e6f 6465 2ea9 01da 0173 72f3 0000  r node.....sr...
-00005b00: 0072 1801 0000 7208 0000 0072 0800 0000  .r....r....r....
-00005b10: 7209 0000 0072 0d01 0000 8d03 0000 7302  r....r........s.
-00005b20: 0000 000c 0372 0d01 0000 6301 0000 0000  .....r....c.....
-00005b30: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00005b40: 0000 0073 1400 0000 7400 6a01 7c00 7402  ...s....t.j.|.t.
-00005b50: 7403 6a04 8301 6401 8d02 5300 2902 7a1d  t.j...d...S.).z.
-00005b60: 4372 6561 7465 7320 616e 205f 6173 742e  Creates an _ast.
-00005b70: 5374 6172 7265 6420 6e6f 6465 2e29 0272  Starred node.).r
-00005b80: 4900 0000 725a 0000 0029 0572 3900 0000  I...rZ...).r9...
-00005b90: da07 5374 6172 7265 6472 5c00 0000 7273  ..Starredr\...rs
-00005ba0: 0000 0072 1400 0000 7218 0100 0072 0800  ...r....r....r..
-00005bb0: 0000 7208 0000 0072 0900 0000 721a 0100  ..r....r....r...
-00005bc0: 0093 0300 0073 0200 0000 1403 721a 0100  .....s......r...
-00005bd0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00005be0: 0000 0200 0000 4300 0000 7268 0000 0072  ......C...rh...r
-00005bf0: 3800 0000 2902 7239 0000 00da 0353 7562  8...).r9.....Sub
-00005c00: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00005c10: 0900 0000 721b 0100 0099 0300 0072 6a00  ....r........rj.
-00005c20: 0000 721b 0100 0063 0500 0000 0000 0000  ..r....c........
-00005c30: 0000 0000 0800 0000 0700 0000 4300 0000  ............C...
-00005c40: 7382 0000 0074 007c 007c 0483 027d 0067  s....t.|.|...}.g
-00005c50: 0064 01a2 017d 0574 017c 017c 027c 0367  .d...}.t.|.|.|.g
-00005c60: 0383 0144 005d 1c5c 027d 067d 077c 0764  ...D.].\.}.}.|.d
-00005c70: 0075 0172 2c74 027c 0774 0383 0273 2174  .u.r,t.|.t...s!t
-00005c80: 0464 0283 0182 0174 007c 0774 056a 0664  .d.....t.|.t.j.d
-00005c90: 038d 027d 077c 077c 057c 063c 0071 1074  ...}.|.|.|.<.q.t
-00005ca0: 076a 087c 0074 097c 0564 0419 007c 0564  .j.|.t.|.d...|.d
-00005cb0: 0519 007c 0564 0619 0083 0374 0a7c 0483  ...|.d.....t.|..
-00005cc0: 0164 078d 0353 0029 084e a903 4e4e 4e7a  .d...S.).N..NNNz
-00005cd0: 1853 7562 7363 7269 7074 206d 7573 7420  .Subscript must 
-00005ce0: 6265 2061 6e20 696e 7472 3e00 0000 7201  be an intr>...r.
-00005cf0: 0000 0072 a300 0000 72a2 0000 0029 0372  ...r....r....).r
-00005d00: 4900 0000 da05 736c 6963 6572 5a00 0000  I.....slicerZ...
-00005d10: 290b 722e 0000 0072 a700 0000 721c 0000  ).r....r....r...
-00005d20: 0072 4000 0000 7231 0000 0072 7300 0000  .r@...r1...rs...
-00005d30: 7214 0000 0072 3900 0000 da09 5375 6273  r....r9.....Subs
-00005d40: 6372 6970 7472 1701 0000 725c 0000 0029  criptr....r\...)
-00005d50: 0872 4900 0000 7215 0100 0072 1401 0000  .rI...r....r....
-00005d60: 7216 0100 0072 5a00 0000 da09 6e65 775f  r....rZ.....new_
-00005d70: 626f 756e 6472 ab00 0000 72e5 0000 0072  boundr....r....r
-00005d80: 0800 0000 7208 0000 0072 0900 0000 721e  ....r....r....r.
-00005d90: 0100 009d 0300 0073 1800 0000 0a01 0801  .......s........
-00005da0: 1601 0801 0a01 0801 0e01 0801 0280 0401  ................
-00005db0: 1e01 06ff 721e 0100 0063 0000 0000 0000  ....r....c......
-00005dc0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-00005dd0: 0000 7328 0000 0065 005a 0164 005a 0287  ..s(...e.Z.d.Z..
-00005de0: 0066 0164 0164 0284 085a 0365 0464 0364  .f.d.d...Z.e.d.d
-00005df0: 0484 0083 015a 0587 0004 005a 0653 0029  .....Z.....Z.S.)
-00005e00: 05da 0743 6f6d 6d65 6e74 6302 0000 0000  ...Commentc.....
-00005e10: 0000 0000 0000 0002 0000 0003 0000 0003  ................
-00005e20: 0000 0073 3800 0000 7400 7401 7c00 8302  ...s8...t.t.|...
-00005e30: a002 a100 0100 7c01 a003 6401 a101 7310  ......|...d...s.
-00005e40: 7404 6402 8301 8201 6700 7c00 5f05 7c01  t.d.....g.|._.|.
-00005e50: 6403 6400 8502 1900 7c00 5f06 6400 5300  d.d.....|._.d.S.
-00005e60: 2904 4efa 0123 7a19 436f 6d6d 656e 7420  ).N..#z.Comment 
-00005e70: 6d75 7374 2073 7461 7274 2077 6974 6820  must start with 
-00005e80: 2372 a300 0000 2907 7253 0000 0072 2001  #r....).rS...r .
-00005e90: 0000 7254 0000 0072 0801 0000 7231 0000  ..rT...r....r1..
-00005ea0: 00da 075f 6669 656c 6473 da07 636f 6d6d  ..._fields..comm
-00005eb0: 656e 7429 0272 5600 0000 7223 0100 0072  ent).rV...r#...r
-00005ec0: 5800 0000 7208 0000 0072 0900 0000 7254  X...r....r....rT
-00005ed0: 0000 00ab 0300 0073 0a00 0000 0e01 0a01  .......s........
-00005ee0: 0801 0601 1201 7a10 436f 6d6d 656e 742e  ......z.Comment.
-00005ef0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00005f00: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00005f10: 0073 1a00 0000 7c00 6a00 6400 7501 720b  .s....|.j.d.u.r.
-00005f20: 6401 7c00 6a00 9b00 9d02 5300 6400 5300  d.|.j.....S.d.S.
-00005f30: 2902 4e72 2101 0000 2901 7223 0100 00a9  ).Nr!...).r#....
-00005f40: 0172 5600 0000 7208 0000 0072 0800 0000  .rV...r....r....
-00005f50: 7209 0000 00da 0e73 6f75 7263 655f 636f  r......source_co
-00005f60: 6d6d 656e 74b2 0300 0073 0600 0000 0a02  mment....s......
-00005f70: 0c01 04ff 7a16 436f 6d6d 656e 742e 736f  ....z.Comment.so
-00005f80: 7572 6365 5f63 6f6d 6d65 6e74 2907 7205  urce_comment).r.
-00005f90: 0000 0072 0600 0000 7207 0000 0072 5400  ...r....r....rT.
-00005fa0: 0000 da08 7072 6f70 6572 7479 7225 0100  ....propertyr%..
-00005fb0: 0072 5d00 0000 7208 0000 0072 0800 0000  .r]...r....r....
-00005fc0: 7258 0000 0072 0900 0000 7220 0100 00aa  rX...r....r ....
-00005fd0: 0300 0073 0800 0000 0800 0c01 0207 1201  ...s............
-00005fe0: 7220 0100 0063 0000 0000 0000 0000 0000  r ...c..........
-00005ff0: 0000 0000 0000 0400 0000 0000 0000 7342  ..............sB
-00006000: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00006010: 0d87 0066 0164 0564 0684 095a 0465 0564  ...f.d.d...Z.e.d
-00006020: 0764 0884 0083 015a 0665 0764 0964 0a84  .d.....Z.e.d.d..
-00006030: 0083 015a 0864 0b64 0c84 005a 0987 0004  ...Z.d.d...Z....
-00006040: 005a 0a53 0029 0eda 0e53 796e 7461 7846  .Z.S.)...SyntaxF
-00006050: 7265 654c 696e 657a 4643 6c61 7373 2064  reeLinezFClass d
-00006060: 6566 696e 696e 6720 6120 6e65 7720 6e6f  efining a new no
-00006070: 6465 2074 6861 7420 6861 7320 6e6f 2073  de that has no s
-00006080: 796e 7461 7820 286f 6e6c 7920 6f70 7469  yntax (only opti
-00006090: 6f6e 616c 2063 6f6d 6d65 6e74 7329 2e4e  onal comments).N
-000060a0: 7201 0000 0072 a300 0000 6304 0000 0000  r....r....c.....
-000060b0: 0000 0000 0000 0004 0000 0003 0000 0003  ................
-000060c0: 0000 0073 2c00 0000 7400 7401 7c00 8302  ...s,...t.t.|...
-000060d0: a002 a100 0100 7c02 7c00 5f03 6401 6701  ......|.|._.d.g.
-000060e0: 7c00 5f04 7c01 7c00 5f05 7c03 7c00 5f06  |._.|.|._.|.|._.
-000060f0: 6400 5300 2902 4eda 0966 756c 6c5f 6c69  d.S.).N..full_li
-00006100: 6e65 2907 7253 0000 0072 2701 0000 7254  ne).rS...r'...rT
-00006110: 0000 00da 0a63 6f6c 5f6f 6666 7365 7472  .....col_offsetr
-00006120: 2201 0000 7223 0100 00da 0e63 6f6d 6d65  "...r#.....comme
-00006130: 6e74 5f69 6e64 656e 7429 0472 5600 0000  nt_indent).rV...
-00006140: 7223 0100 0072 2901 0000 722a 0100 0072  r#...r)...r*...r
-00006150: 5800 0000 7208 0000 0072 0900 0000 7254  X...r....r....rT
-00006160: 0000 00ba 0300 0073 0a00 0000 0e01 0603  .......s........
-00006170: 0801 0601 0a01 7a17 5379 6e74 6178 4672  ......z.SyntaxFr
-00006180: 6565 4c69 6e65 2e5f 5f69 6e69 745f 5f63  eeLine.__init__c
-00006190: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000061a0: 0500 0000 4300 0000 732a 0000 007c 006a  ....C...s*...|.j
-000061b0: 0064 0075 0172 1364 01a0 0164 027c 006a  .d.u.r.d...d.|.j
-000061c0: 0214 0064 027c 006a 0314 007c 006a 00a1  ...d.|.j...|.j..
-000061d0: 0353 0064 0353 0029 044e 7a07 7b7d 237b  .S.d.S.).Nz.{}#{
-000061e0: 7d7b 7dfa 0120 72ce 0000 0029 0472 2301  }{}.. r....).r#.
-000061f0: 0000 724f 0000 0072 2901 0000 722a 0100  ..rO...r)...r*..
-00006200: 0072 2401 0000 7208 0000 0072 0800 0000  .r$...r....r....
-00006210: 7209 0000 0072 2801 0000 c303 0000 730c  r....r(.......s.
-00006220: 0000 000a 020c 0108 0104 0104 fe04 037a  ...............z
-00006230: 1853 796e 7461 7846 7265 654c 696e 652e  .SyntaxFreeLine.
-00006240: 6675 6c6c 5f6c 696e 6563 0200 0000 0000  full_linec......
-00006250: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00006260: 0000 7310 0000 0074 00a0 0164 017c 01a1  ..s....t...d.|..
-00006270: 027d 027c 0253 0029 024e 7a1c 5e28 5b20  .}.|.S.).Nz.^([ 
-00006280: 095d 2a29 283f 3a7c 2823 2928 5b20 095d  .]*)(?:|(#)([ .]
-00006290: 2a29 282e 2a29 290a 2902 da02 7265 da05  *)(.*)).)...re..
-000062a0: 6d61 7463 6829 03da 0363 6c73 da04 7465  match)...cls..te
-000062b0: 7874 da13 6973 5f73 796e 7461 785f 6672  xt..is_syntax_fr
-000062c0: 6565 5f6c 696e 6572 0800 0000 7208 0000  ee_liner....r...
-000062d0: 0072 0900 0000 da0c 4d61 7463 6865 7353  .r......MatchesS
-000062e0: 7461 7274 cb03 0000 7304 0000 000c 0204  tart....s.......
-000062f0: 017a 1b53 796e 7461 7846 7265 654c 696e  .z.SyntaxFreeLin
-00006300: 652e 4d61 7463 6865 7353 7461 7274 6302  e.MatchesStartc.
-00006310: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00006320: 0000 0043 0000 0073 8400 0000 7c00 a000  ...C...s....|...
-00006330: 7c01 a101 7d02 7c02 730e 7401 6401 a002  |...}.|.s.t.d...
-00006340: 7c01 a101 8301 8201 7403 7c02 a004 6402  |.......t.|...d.
-00006350: a101 8301 7c00 5f05 6403 7c00 5f06 6400  ....|._.d.|._.d.
-00006360: 7c00 5f07 7c02 a004 6404 a101 723e 6405  |._.|...d...r>d.
-00006370: 7c00 5f07 7c02 a004 6406 a101 7231 7403  |._.|...d...r1t.
-00006380: 7c02 a004 6406 a101 8301 7c00 5f06 7c02  |...d.....|._.|.
-00006390: a004 6407 a101 7240 7c02 a004 6407 a101  ..d...r@|...d...
-000063a0: 7c00 5f07 6400 5300 6400 5300 6400 5300  |._.d.S.d.S.d.S.
-000063b0: 2908 4e7a 256c 696e 6520 7b7d 2069 7320  ).Nz%line {} is 
-000063c0: 6e6f 7420 6120 7661 6c69 6420 5379 6e74  not a valid Synt
-000063d0: 6178 4672 6565 4c69 6e65 72a3 0000 0072  axFreeLiner....r
-000063e0: 0100 0000 72a2 0000 0072 ce00 0000 72a1  ....r....r....r.
-000063f0: 0000 00e9 0400 0000 2908 7231 0100 0072  ........).r1...r
-00006400: 3100 0000 724f 0000 0072 a600 0000 da05  1...rO...r......
-00006410: 6772 6f75 7072 2901 0000 722a 0100 0072  groupr)...r*...r
-00006420: 2301 0000 2903 7256 0000 00da 046c 696e  #...).rV.....lin
-00006430: 6572 2d01 0000 7208 0000 0072 0800 0000  er-...r....r....
-00006440: 7209 0000 00da 0e53 6574 4672 6f6d 5372  r......SetFromSr
-00006450: 634c 696e 65d0 0300 0073 1c00 0000 0a01  cLine....s......
-00006460: 0401 0e01 1001 0601 0601 0a01 0601 0a01  ................
-00006470: 1001 0a01 1001 04fb 0404 7a1d 5379 6e74  ..........z.Synt
-00006480: 6178 4672 6565 4c69 6e65 2e53 6574 4672  axFreeLine.SetFr
-00006490: 6f6d 5372 634c 696e 6529 034e 7201 0000  omSrcLine).Nr...
-000064a0: 0072 a300 0000 290b 7205 0000 0072 0600  .r....).r....r..
-000064b0: 0000 7207 0000 00da 075f 5f64 6f63 5f5f  ..r......__doc__
-000064c0: 7254 0000 0072 2601 0000 7228 0100 00da  rT...r&...r(....
-000064d0: 0b63 6c61 7373 6d65 7468 6f64 7231 0100  .classmethodr1..
-000064e0: 0072 3501 0000 725d 0000 0072 0800 0000  .r5...r]...r....
-000064f0: 7208 0000 0072 5800 0000 7209 0000 0072  r....rX...r....r
-00006500: 2701 0000 b703 0000 7310 0000 0008 0004  '.......s.......
-00006510: 010e 0202 090a 0102 070a 0110 0472 2701  .............r'.
-00006520: 0000 6301 0000 0000 0000 0000 0000 0007  ..c.............
-00006530: 0000 0006 0000 004b 0000 0073 ac00 0000  .......K...s....
-00006540: 7400 7c00 7401 8302 7309 7402 6401 8301  t.|.t...s.t.d...
-00006550: 8201 7c01 a003 6402 7404 6a05 a102 7d02  ..|...d.t.j...}.
-00006560: 6700 7d03 7c00 4400 5d16 7d04 7400 7c04  g.}.|.D.].}.t.|.
-00006570: 7406 7407 7408 6a09 6603 8302 7227 7c03  t.t.t.j.f...r'|.
-00006580: a00a 740b 7c04 8301 a101 0100 7114 740c  ..t.|.......q.t.
-00006590: 6403 8301 8201 7c03 4400 5d1d 7d04 7400  d.....|.D.].}.t.
-000065a0: 7c04 740d 6a0e 8302 723b 740f 7c02 8301  |.t.j...r;t.|...
-000065b0: 7c04 5f10 712d 7400 7c04 740d 6a11 8302  |._.q-t.|.t.j...
-000065c0: 724a 7412 7c04 8301 7d05 740f 7c02 8301  rJt.|...}.t.|...
-000065d0: 7c05 5f10 712d 740f 7c02 8301 7d06 740d  |._.q-t.|...}.t.
-000065e0: 6a13 7c03 7c06 6404 8d02 5300 2905 6107  j.|.|.d...S.).a.
-000065f0: 0100 0043 7265 6174 6573 2061 6e20 5f61  ...Creates an _a
-00006600: 7374 2e54 7570 6c65 206e 6f64 652e 0a0a  st.Tuple node...
-00006610: 2020 4175 746f 6d61 7469 6361 6c6c 7920    Automatically 
-00006620: 6164 6a75 7374 7320 696e 6e65 7220 6374  adjusts inner ct
-00006630: 7820 6174 7472 732e 0a0a 2020 4172 6773  x attrs...  Args
-00006640: 3a0a 2020 2020 2a69 7465 6d73 3a20 5468  :.    *items: Th
-00006650: 6520 6974 656d 7320 696e 2074 6865 206c  e items in the l
-00006660: 6973 742e 0a20 2020 202a 2a6b 7761 7267  ist..    **kwarg
-00006670: 733a 204f 6e6c 7920 7265 636f 676e 697a  s: Only recogniz
-00006680: 6564 206b 7761 7267 2069 7320 2763 7478  ed kwarg is 'ctx
-00006690: 5f74 7970 6527 2c20 7768 6963 6820 636f  _type', which co
-000066a0: 6e74 726f 6c73 2074 6865 0a20 2020 2020  ntrols the.     
-000066b0: 2063 7478 2074 7970 6520 6f66 2074 6865   ctx type of the
-000066c0: 206c 6973 742e 2053 6565 2043 7478 456e   list. See CtxEn
-000066d0: 756d 2e0a 0a20 2052 6574 7572 6e73 3a0a  um...  Returns:.
-000066e0: 2020 2020 416e 205f 6173 742e 5475 706c      An _ast.Tupl
-000066f0: 6520 6e6f 6465 2e0a 2020 7a1f 6974 656d  e node..  z.item
-00006700: 7320 696e 2074 7570 6c65 2073 686f 756c  s in tuple shoul
-00006710: 6420 6265 2061 206c 6973 7472 3f00 0000  d be a listr?...
-00006720: 7a1f 5475 706c 6520 6974 656d 2074 7970  z.Tuple item typ
-00006730: 6520 6e6f 7420 696d 706c 656d 656e 7465  e not implemente
-00006740: 6472 e100 0000 2914 721c 0000 0072 3000  dr....).r....r0.
-00006750: 0000 7231 0000 0072 8200 0000 7273 0000  ..r1...r....rs..
-00006760: 0072 1400 0000 7242 0000 0072 4000 0000  .r....rB...r@...
-00006770: 7219 0000 0072 4100 0000 7232 0000 0072  r....rA...r2...r
-00006780: 2e00 0000 7244 0000 0072 3900 0000 7243  ....rD...r9...rC
-00006790: 0000 0072 5c00 0000 725a 0000 0072 9a00  ...r\...rZ...r..
-000067a0: 0000 724b 0000 0072 4600 0000 2907 72e4  ..rK...rF...).r.
-000067b0: 0000 0072 9600 0000 723f 0000 00da 096e  ...r....r?.....n
-000067c0: 6577 5f69 7465 6d73 72e5 0000 0072 e600  ew_itemsr....r..
-000067d0: 0000 725a 0000 0072 0800 0000 7208 0000  ..rZ...r....r...
-000067e0: 0072 0900 0000 7246 0000 00df 0300 0073  .r....rF.......s
-000067f0: 2600 0000 0a0d 0801 0e01 0402 0801 1201  &...............
-00006800: 1001 0802 0802 0c01 0c01 0c01 0801 0a01  ................
-00006810: 0280 0801 0601 0201 06ff 7246 0000 0063  ..........rF...c
-00006820: 0400 0000 0000 0000 0000 0000 0500 0000  ................
-00006830: 0600 0000 4300 0000 7330 0000 0074 007c  ....C...s0...t.|
-00006840: 0283 017d 047c 0172 0b74 017c 0174 0283  ...}.|.r.t.|.t..
-00006850: 0273 0f74 0364 0183 0182 0174 046a 057c  .s.t.d.....t.j.|
-00006860: 007c 017c 047c 0364 028d 0453 0029 034e  .|.|.|.d...S.).N
-00006870: 7a2b 4578 6365 7074 696f 6e20 6861 6e64  z+Exception hand
-00006880: 6c65 7273 206d 7573 7420 6265 2061 206e  lers must be a n
-00006890: 6f6e 2d65 6d70 7479 206c 6973 7429 0472  on-empty list).r
-000068a0: 1b00 0000 da08 6861 6e64 6c65 7273 da09  ......handlers..
-000068b0: 6669 6e61 6c62 6f64 7972 c900 0000 2906  finalbodyr....).
-000068c0: 7251 0000 0072 1c00 0000 7230 0000 0072  rQ...r....r0...r
-000068d0: 3100 0000 7239 0000 00da 0354 7279 2905  1...r9.....Try).
-000068e0: 721b 0000 00da 0f65 7863 6570 745f 6861  r......except_ha
-000068f0: 6e64 6c65 7273 da0a 6669 6e61 6c79 626f  ndlers..finalybo
-00006900: 6479 72c9 0000 0072 3a01 0000 7208 0000  dyr....r:...r...
-00006910: 0072 0800 0000 7209 0000 0072 3b01 0000  .r....r....r;...
-00006920: 0204 0000 7308 0000 0008 010e 0208 0112  ....s...........
-00006930: 0172 3b01 0000 6304 0000 0000 0000 0000  .r;...c.........
-00006940: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
-00006950: 1200 0000 7400 6a01 7c00 7c01 7c02 6700  ....t.j.|.|.|.g.
-00006960: 6401 8d04 5300 2902 4e29 0172 c900 0000  d...S.).N).r....
-00006970: 2902 7219 0000 00da 0346 6f72 2904 727a  ).r......For).rz
-00006980: 0000 0072 ac00 0000 721b 0000 0072 c900  ...r....r....r..
-00006990: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
-000069a0: 0072 3e01 0000 0904 0000 7302 0000 0012  .r>.......s.....
-000069b0: 0172 3e01 0000 6300 0000 0000 0000 0000  .r>...c.........
-000069c0: 0000 0000 0000 0002 0000 0043 0000 0072  ...........C...r
-000069d0: 6800 0000 7238 0000 0029 0272 3900 0000  h...r8...).r9...
-000069e0: da04 5541 6464 7208 0000 0072 0800 0000  ..UAddr....r....
-000069f0: 7208 0000 0072 0900 0000 723f 0100 000d  r....r....r?....
-00006a00: 0400 0072 6a00 0000 723f 0100 0063 0200  ...rj...r?...c..
-00006a10: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00006a20: 0000 4300 0000 7322 0000 0074 007c 0074  ..C...s"...t.|.t
-00006a30: 016a 0283 0273 0a74 037c 0083 017d 0074  .j...s.t.|...}.t
-00006a40: 016a 047c 007c 0164 018d 0253 0029 027a  .j.|.|.d...S.).z
-00006a50: 284f 7065 7261 746f 7220 6c69 7465 7261  (Operator litera
-00006a60: 6c73 2028 276e 6f74 2729 2061 6c73 6f20  ls ('not') also 
-00006a70: 6163 6365 7074 6564 2e29 0272 7c00 0000  accepted.).r|...
-00006a80: da07 6f70 6572 616e 6429 0572 1c00 0000  ..operand).r....
-00006a90: 7239 0000 0072 3a00 0000 da0a 556e 6172  r9...r:.....Unar
-00006aa0: 794f 704d 6170 da07 556e 6172 794f 7029  yOpMap..UnaryOp)
-00006ab0: 02da 086f 7065 7261 746f 7272 4001 0000  ...operatorr@...
-00006ac0: 7208 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-00006ad0: 4201 0000 1104 0000 7306 0000 000c 0208  B.......s.......
-00006ae0: 010e 0172 4201 0000 6300 0000 0000 0000  ...rB...c.......
-00006af0: 0000 0000 0000 0000 0002 0000 0043 0000  .............C..
-00006b00: 0072 6800 0000 7238 0000 0029 0272 3900  .rh...r8...).r9.
-00006b10: 0000 da04 5553 7562 7208 0000 0072 0800  ....USubr....r..
-00006b20: 0000 7208 0000 0072 0900 0000 7244 0100  ..r....r....rD..
-00006b30: 0018 0400 0072 6a00 0000 7244 0100 0063  .....rj...rD...c
-00006b40: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00006b50: 0400 0000 4300 0000 7348 0000 0074 007c  ....C...sH...t.|
-00006b60: 0174 0183 0272 0d74 027c 0174 036a 0464  .t...r.t.|.t.j.d
-00006b70: 018d 027d 016e 0f7c 0172 1c74 007c 0174  ...}.n.|.r.t.|.t
-00006b80: 056a 0674 056a 0766 0283 0273 1c74 0864  .j.t.j.f...s.t.d
-00006b90: 0283 0182 0174 09a0 0a74 027c 0083 017c  .....t...t.|...|
-00006ba0: 01a1 0253 0029 034e 723e 0000 007a 2477  ...S.).Nr>...z$w
-00006bb0: 6974 6869 7465 6d20 6d75 7374 2062 6520  ithitem must be 
-00006bc0: 7374 722c 2074 7570 6c65 2c20 6f72 206c  str, tuple, or l
-00006bd0: 6973 7429 0b72 1c00 0000 7242 0000 0072  ist).r....rB...r
-00006be0: 4300 0000 7273 0000 0072 1500 0000 7219  C...rs...r....r.
-00006bf0: 0000 0072 4600 0000 72e3 0000 0072 3100  ...rF...r....r1.
-00006c00: 0000 7239 0000 00da 0877 6974 6869 7465  ..r9.....withite
-00006c10: 6d29 0272 9d00 0000 da0d 6f70 7469 6f6e  m).r......option
-00006c20: 616c 5f76 6172 7372 0800 0000 7208 0000  al_varsr....r...
-00006c30: 0072 0900 0000 7245 0100 001c 0400 0073  .r....rE.......s
-00006c40: 0a00 0000 0a01 1001 1601 0801 1001 7245  ..............rE
-00006c50: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
-00006c60: 0200 0000 0500 0000 4300 0000 733c 0000  ........C...s<..
-00006c70: 0074 007c 0174 0183 0273 0974 0264 0183  .t.|.t...s.t.d..
-00006c80: 0182 0174 007c 0074 0183 0273 1274 0264  ...t.|.t...s.t.d
-00006c90: 0283 0182 0174 037c 0183 017d 0174 046a  .....t.|...}.t.j
-00006ca0: 057c 007c 0164 0064 038d 0353 0029 044e  .|.|.d.d...S.).N
-00006cb0: 7a18 5769 7468 2d62 6f64 7920 6d75 7374  z.With-body must
-00006cc0: 2062 6520 6120 6c69 7374 7a18 7769 7468   be a listz.with
-00006cd0: 6974 656d 7320 6d75 7374 2062 6520 6120  items must be a 
-00006ce0: 6c69 7374 2903 72e4 0000 0072 1b00 0000  list).r....r....
-00006cf0: 72c1 0000 0029 0672 1c00 0000 7230 0000  r....).r....r0..
-00006d00: 0072 3100 0000 7251 0000 0072 3900 0000  .r1...rQ...r9...
-00006d10: da04 5769 7468 2902 da09 7769 7468 6974  ..With)...withit
-00006d20: 656d 7372 1b00 0000 7208 0000 0072 0800  emsr....r....r..
-00006d30: 0000 7209 0000 0072 4701 0000 2404 0000  ..r....rG...$...
-00006d40: 7310 0000 000a 0108 010a 0208 0108 0206  s...............
-00006d50: 0404 0106 ff72 4701 0000 e9ff ffff ff63  .....rG........c
-00006d60: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00006d70: 0500 0000 4300 0000 7338 0000 007c 0164  ....C...s8...|.d
-00006d80: 016b 0373 067c 0272 0a74 0064 0283 0182  .k.s.|.r.t.d....
-00006d90: 0174 017c 0074 026a 0383 0273 1474 0064  .t.|.t.j...s.t.d
-00006da0: 0383 0182 0174 026a 047c 007c 017c 0264  .....t.j.|.|.|.d
-00006db0: 048d 0353 0029 054e 7249 0100 007a 2c63  ...S.).NrI...z,c
-00006dc0: 6f6e 7665 7273 696f 6e20 616e 6420 666f  onversion and fo
-00006dd0: 726d 6174 5f73 7065 6320 6e6f 7420 7375  rmat_spec not su
-00006de0: 7070 6f72 7465 6420 7965 747a 2346 6f72  pported yetz#For
-00006df0: 6d61 7474 6564 5661 6c75 6520 7661 6c75  mattedValue valu
-00006e00: 6520 6d75 7374 2062 6520 6120 4e61 6d65  e must be a Name
-00006e10: a903 7249 0000 00da 0a63 6f6e 7665 7273  ..rI.....convers
-00006e20: 696f 6eda 0b66 6f72 6d61 745f 7370 6563  ion..format_spec
-00006e30: 2905 7244 0000 0072 1c00 0000 7239 0000  ).rD...r....r9..
-00006e40: 0072 4300 0000 da0e 466f 726d 6174 7465  .rC.....Formatte
-00006e50: 6456 616c 7565 724a 0100 0072 0800 0000  dValuerJ...r....
-00006e60: 7208 0000 0072 0900 0000 724d 0100 0032  r....r....rM...2
-00006e70: 0400 0073 0a00 0000 0c01 0801 0c01 0801  ...s............
-00006e80: 1001 724d 0100 0063 0100 0000 0000 0000  ..rM...c........
-00006e90: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-00006ea0: 7330 0000 007c 0044 005d 0f7d 0174 007c  s0...|.D.].}.t.|
-00006eb0: 0174 016a 0274 016a 0366 0283 0273 1174  .t.j.t.j.f...s.t
-00006ec0: 0464 0183 0182 0171 0274 056a 067c 0064  .d.....q.t.j.|.d
-00006ed0: 028d 0153 0029 034e 7a33 4a6f 696e 6564  ...S.).Nz3Joined
-00006ee0: 5374 7220 7661 6c75 6573 206d 7573 7420  Str values must 
-00006ef0: 6265 2043 6f6e 7374 616e 7420 6f72 2046  be Constant or F
-00006f00: 6f72 6d61 7474 6564 5661 6c75 6529 0172  ormattedValue).r
-00006f10: 8100 0000 2907 721c 0000 0072 1900 0000  ....).r....r....
-00006f20: 7241 0000 0072 4d01 0000 7231 0000 0072  rA...rM...r1...r
-00006f30: 3900 0000 da09 4a6f 696e 6564 5374 7229  9.....JoinedStr)
-00006f40: 0272 8100 0000 7249 0000 0072 0800 0000  .r....rI...r....
-00006f50: 7208 0000 0072 0900 0000 724e 0100 003a  r....r....rN...:
-00006f60: 0400 0073 0a00 0000 0801 1201 0801 02ff  ...s............
-00006f70: 0c02 724e 0100 0063 0100 0000 0000 0000  ..rN...c........
-00006f80: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00006f90: 7356 0000 007c 0074 006a 016b 0272 0974  sV...|.t.j.k.r.t
-00006fa0: 02a0 03a1 0053 007c 0074 006a 046b 0272  .....S.|.t.j.k.r
-00006fb0: 1274 02a0 05a1 0053 007c 0074 006a 066b  .t.....S.|.t.j.k
-00006fc0: 0272 1b74 02a0 07a1 0053 007c 0074 006a  .r.t.....S.|.t.j
-00006fd0: 086b 0272 2474 02a0 09a1 0053 0074 0a64  .k.r$t.....S.t.d
-00006fe0: 01a0 0b7c 00a1 0183 0182 0129 027a 3b43  ...|.......).z;C
-00006ff0: 7265 6174 6573 204c 6f61 642c 2053 746f  reates Load, Sto
-00007000: 7265 2c20 4465 6c2c 2061 6e64 2050 6172  re, Del, and Par
-00007010: 616d 2c20 7573 6564 2069 6e20 7468 6520  am, used in the 
-00007020: 6374 7820 6b77 6172 672e 7a1e 6374 785f  ctx kwarg.z.ctx_
-00007030: 7479 7065 207b 7d20 6973 6e27 7420 6120  type {} isn't a 
-00007040: 7661 6c69 6420 7479 7065 290c 7273 0000  valid type).rs..
-00007050: 0072 1400 0000 7239 0000 00da 044c 6f61  .r....r9.....Loa
-00007060: 6472 1500 0000 da05 5374 6f72 6572 1600  dr......Storer..
-00007070: 0000 da03 4465 6c72 1700 0000 da05 5061  ....Delr......Pa
-00007080: 7261 6d72 0b00 0000 724f 0000 0072 3e00  ramr....rO...r>.
-00007090: 0000 7208 0000 0072 0800 0000 7209 0000  ..r....r....r...
-000070a0: 0072 5c00 0000 4504 0000 7312 0000 000a  .r\...E...s.....
-000070b0: 0208 010a 0108 010a 0108 010a 0108 010e  ................
-000070c0: 0172 5c00 0000 6301 0000 0000 0000 0000  .r\...c.........
-000070d0: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-000070e0: 2000 0000 7400 6a01 7400 6a02 7400 6a03   ...t.j.t.j.t.j.
-000070f0: 7400 6a04 6401 9c04 7d01 7c01 7c00 1900  t.j.d...}.|.|...
-00007100: 8300 5300 2902 7a3e 4d61 7073 206f 7065  ..S.).z>Maps ope
-00007110: 7261 746f 7220 7374 7269 6e67 7320 666f  rator strings fo
-00007120: 7220 756e 6172 7920 6f70 6572 6174 696f  r unary operatio
-00007130: 6e73 2074 6f20 7468 6569 7220 5f61 7374  ns to their _ast
-00007140: 206e 6f64 652e 2904 fa01 2bfa 012d da03   node.)...+..-..
-00007150: 6e6f 74fa 017e 2905 7239 0000 0072 3f01  not..~).r9...r?.
-00007160: 0000 7244 0100 0072 fc00 0000 72dc 0000  ..rD...r....r...
-00007170: 00a9 0272 4301 0000 da07 6f70 5f64 6963  ...rC.....op_dic
-00007180: 7472 0800 0000 7208 0000 0072 0900 0000  tr....r....r....
-00007190: 7241 0100 0052 0400 0073 0c00 0000 0403  rA...R...s......
-000071a0: 0401 0401 0401 06fc 0a07 7241 0100 0063  ..........rA...c
-000071b0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000071c0: 0d00 0000 4300 0000 7340 0000 0074 006a  ....C...s@...t.j
-000071d0: 0174 006a 0274 006a 0374 006a 0474 006a  .t.j.t.j.t.j.t.j
-000071e0: 0574 006a 0674 006a 0774 006a 0874 006a  .t.j.t.j.t.j.t.j
-000071f0: 0974 006a 0a74 006a 0b74 006a 0c64 019c  .t.j.t.j.t.j.d..
-00007200: 0c7d 017c 017c 0019 0083 0053 0029 027a  .}.|.|.....S.).z
-00007210: 3f4d 6170 7320 6f70 6572 6174 6f72 2073  ?Maps operator s
-00007220: 7472 696e 6773 2066 6f72 2062 696e 6172  trings for binar
-00007230: 7920 6f70 6572 6174 696f 6e73 2074 6f20  y operations to 
-00007240: 7468 6569 7220 5f61 7374 206e 6f64 652e  their _ast node.
-00007250: 290c 7253 0100 0072 5401 0000 da01 2a7a  ).rS...rT.....*z
-00007260: 022a 2afa 012f 7a02 2f2f fa01 257a 023c  .**../z.//..%z.<
-00007270: 3c7a 023e 3efa 017c fa01 26fa 015e 290d  <z.>>..|..&..^).
-00007280: 7239 0000 0072 6900 0000 721b 0100 0072  r9...ri...r....r
-00007290: f100 0000 720c 0100 0072 b900 0000 72bf  ....r....r....r.
-000072a0: 0000 0072 ee00 0000 72eb 0000 0072 1001  ...r....r....r..
-000072b0: 0000 728b 0000 0072 8a00 0000 728c 0000  ..r....r....r...
-000072c0: 0072 5701 0000 7208 0000 0072 0800 0000  .rW...r....r....
-000072d0: 7209 0000 0072 7f00 0000 5e04 0000 731c  r....r....^...s.
-000072e0: 0000 0004 0304 0104 0104 0104 0104 0104  ................
-000072f0: 0104 0104 0104 0104 0104 0106 f40a 0f72  ...............r
-00007300: 7f00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00007310: 0002 0000 0003 0000 0043 0000 0073 1800  .........C...s..
-00007320: 0000 7400 6a01 7400 6a02 6401 9c02 7d01  ..t.j.t.j.d...}.
-00007330: 7c01 7c00 1900 8300 5300 2902 fa40 4d61  |.|.....S.)..@Ma
-00007340: 7073 206f 7065 7261 746f 7220 7374 7269  ps operator stri
-00007350: 6e67 7320 666f 7220 626f 6f6c 6561 6e20  ngs for boolean 
-00007360: 6f70 6572 6174 696f 6e73 2074 6f20 7468  operations to th
-00007370: 6569 7220 5f61 7374 206e 6f64 652e 2902  eir _ast node.).
-00007380: da03 616e 64da 026f 7229 0372 3900 0000  ..and..or).r9...
-00007390: 726b 0000 0072 8500 0000 7257 0100 0072  rk...r....rW...r
-000073a0: 0800 0000 7208 0000 0072 0900 0000 7283  ....r....r....r.
-000073b0: 0000 0072 0400 0073 0800 0000 0403 0401  ...r...s........
-000073c0: 06fe 0a05 7283 0000 0063 0100 0000 0000  ....r....c......
-000073d0: 0000 0000 0000 0200 0000 0b00 0000 4300  ..............C.
-000073e0: 0000 7338 0000 0074 006a 0174 006a 0274  ..s8...t.j.t.j.t
-000073f0: 006a 0374 006a 0474 006a 0574 006a 0674  .j.t.j.t.j.t.j.t
-00007400: 006a 0774 006a 0874 006a 0974 006a 0a64  .j.t.j.t.j.t.j.d
-00007410: 019c 0a7d 017c 017c 0019 0083 0053 0029  ...}.|.|.....S.)
-00007420: 0272 5f01 0000 290a 7a02 3d3d 7a02 213d  .r_...).z.==z.!=
-00007430: fa01 3c7a 023c 3dfa 013e 7a02 3e3d da02  ..<z.<=..>z.>=..
-00007440: 6973 7a06 6973 206e 6f74 da02 696e 7a06  isz.is not..inz.
-00007450: 6e6f 7420 696e 290b 7239 0000 0072 ba00  not in).r9...r..
-00007460: 0000 72fd 0000 0072 ec00 0000 72ed 0000  ..r....r....r...
-00007470: 0072 c700 0000 72c8 0000 0072 dd00 0000  .r....r....r....
-00007480: 72de 0000 0072 d800 0000 72fe 0000 0072  r....r....r....r
-00007490: 5701 0000 7208 0000 0072 0800 0000 7209  W...r....r....r.
-000074a0: 0000 0072 a800 0000 7c04 0000 7318 0000  ...r....|...s...
-000074b0: 0004 0304 0104 0104 0104 0104 0104 0104  ................
-000074c0: 0104 0104 0106 f60a 0d72 a800 0000 6300  .........r....c.
-000074d0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-000074e0: 0000 004f 0000 0073 7c00 0000 7c01 a000  ...O...s|...|...
-000074f0: 6401 7401 6a02 a102 7d02 7c00 730d 7403  d.t.j...}.|.s.t.
-00007500: 6402 8301 8201 7404 7c00 8301 6403 6b02  d.....t.|...d.k.
-00007510: 7229 7405 7c00 6404 1900 7406 8302 7225  r)t.|.d...t...r%
-00007520: 7407 6a08 7c00 6404 1900 7409 7c02 8301  t.j.|.d...t.|...
-00007530: 6405 8d02 5300 7c00 6404 1900 5300 7407  d...S.|.d...S.t.
-00007540: 6a0a 740b 7c00 6406 6407 8502 1900 6900  j.t.|.d.d.....i.
-00007550: 7c01 a401 8e01 7c00 6407 1900 7409 7c02  |.....|.d...t.|.
-00007560: 8301 6408 8d03 5300 2909 61ac 0100 0042  ..d...S.).a....B
-00007570: 7920 7468 6973 2077 6520 6d65 616e 2065  y this we mean e
-00007580: 6974 6865 7220 6120 7369 6e67 6c65 206e  ither a single n
-00007590: 616d 6520 7374 7269 6e67 206f 7220 6f6e  ame string or on
-000075a0: 6520 6f72 206d 6f72 6520 4174 7472 206e  e or more Attr n
-000075b0: 6f64 6573 2e0a 0a20 2054 6869 7320 6973  odes...  This is
-000075c0: 2075 7365 6420 7768 656e 6576 6572 2077   used whenever w
-000075d0: 6520 6861 7665 2074 6869 6e67 7320 6c69  e have things li
-000075e0: 6b65 2027 6127 206f 7220 2761 2e62 2720  ke 'a' or 'a.b' 
-000075f0: 6f72 2027 612e 622e 6327 2e0a 0a20 2041  or 'a.b.c'...  A
-00007600: 7267 733a 0a20 2020 202a 7061 7274 733a  rgs:.    *parts:
-00007610: 2054 6865 2070 6172 7473 2074 6861 7420   The parts that 
-00007620: 7368 6f75 6c64 2062 6520 646f 742d 7365  should be dot-se
-00007630: 7061 7261 7465 642e 0a20 2020 202a 2a6b  parated..    **k
-00007640: 7761 7267 733a 204f 6e6c 7920 7265 636f  wargs: Only reco
-00007650: 676e 697a 6564 206b 7761 7267 2069 7320  gnized kwarg is 
-00007660: 2763 7478 5f74 7970 6527 2c20 7768 6963  'ctx_type', whic
-00007670: 6820 636f 6e74 726f 6c73 2074 6865 0a20  h controls the. 
-00007680: 2020 2020 2063 7478 2074 7970 6520 6f66       ctx type of
-00007690: 2074 6865 206c 6973 742e 2053 6565 2043   the list. See C
-000076a0: 7478 456e 756d 2e0a 0a20 2052 6169 7365  txEnum...  Raise
-000076b0: 733a 0a20 2020 2056 616c 7565 4572 726f  s:.    ValueErro
-000076c0: 723a 2057 6865 6e20 6e6f 2070 6172 7473  r: When no parts
-000076d0: 2061 7265 2073 7065 6369 6669 6564 2e0a   are specified..
-000076e0: 0a20 2052 6574 7572 6e73 3a0a 2020 2020  .  Returns:.    
-000076f0: 416e 205f 6173 742e 4e61 6d65 206e 6f64  An _ast.Name nod
-00007700: 6520 6f72 205f 6173 742e 4174 7472 6962  e or _ast.Attrib
-00007710: 7574 6520 6e6f 6465 0a20 2072 3f00 0000  ute node.  r?...
-00007720: 7a25 4d75 7374 2068 6176 6520 6174 206c  z%Must have at l
-00007730: 6561 7374 206f 6e65 2070 6172 7420 7370  east one part sp
-00007740: 6563 6966 6965 6472 a300 0000 7201 0000  ecifiedr....r...
-00007750: 0072 fb00 0000 4e72 4901 0000 2903 7249  .r....NrI...).rI
-00007760: 0000 00da 0461 7474 7272 5a00 0000 290c  .....attrrZ...).
-00007770: 7282 0000 0072 7300 0000 7214 0000 0072  r....rs...r....r
-00007780: 3100 0000 72a6 0000 0072 1c00 0000 7242  1...r....r....rB
-00007790: 0000 0072 3900 0000 7243 0000 0072 5c00  ...r9...rC...r\.
-000077a0: 0000 729a 0000 0072 9700 0000 2903 da05  ..r....r....)...
-000077b0: 7061 7274 7372 9600 0000 723f 0000 0072  partsr....r?...r
-000077c0: 0800 0000 7208 0000 0072 0900 0000 7297  ....r....r....r.
-000077d0: 0000 008e 0400 0073 1800 0000 0e10 0402  .......s........
-000077e0: 0801 0c01 0e01 1601 0801 0401 1401 0601  ................
-000077f0: 0601 06fd 7297 0000 0029 0272 0100 0000  ....r....).r....
-00007800: 4672 3800 0000 2902 7208 0000 0072 0800  Fr8...).r....r..
-00007810: 0000 721c 0100 0029 0372 ce00 0000 72ce  ..r....).r....r.
-00007820: 0000 004e 2902 7249 0100 004e 2968 7239  ...N).rI...N)hr9
-00007830: 0000 0072 1900 0000 722c 0100 00da 0945  ...r....r,.....E
-00007840: 7863 6570 7469 6f6e 7203 0000 0072 0b00  xceptionr....r..
-00007850: 0000 720c 0000 0072 7300 0000 7224 0000  ..r....rs...r$..
-00007860: 0072 3700 0000 7227 0000 0072 1400 0000  .r7...r'...r....
-00007870: 722e 0000 0072 4700 0000 724b 0000 0072  r....rG...rK...r
-00007880: 5100 0000 da0f 4e6f 6465 5472 616e 7366  Q.....NodeTransf
-00007890: 6f72 6d65 7272 5200 0000 7260 0000 0072  ormerrR...r`...r
-000078a0: 6700 0000 7269 0000 0072 6b00 0000 726e  g...ri...rk...rn
-000078b0: 0000 0072 7500 0000 727d 0000 0072 8000  ...ru...r}...r..
-000078c0: 0000 7284 0000 0072 8a00 0000 728b 0000  ..r....r....r...
-000078d0: 0072 8c00 0000 728d 0000 0072 9b00 0000  .r....r....r....
-000078e0: 72a0 0000 0072 aa00 0000 72af 0000 0072  r....r....r....r
-000078f0: b300 0000 72b6 0000 0072 b900 0000 72ba  ....r....r....r.
-00007900: 0000 0072 bb00 0000 72bd 0000 0072 bf00  ...r....r....r..
-00007910: 0000 72c2 0000 0072 c500 0000 72c7 0000  ..r....r....r...
-00007920: 0072 c800 0000 721d 0000 0072 cb00 0000  .r....r....r....
-00007930: 72d5 0000 0072 d800 0000 72da 0000 0072  r....r....r....r
-00007940: dc00 0000 72dd 0000 0072 de00 0000 72df  ....r....r....r.
-00007950: 0000 0072 e300 0000 72e8 0000 0072 eb00  ...r....r....r..
-00007960: 0000 72ec 0000 0072 ed00 0000 72ee 0000  ..r....r....r...
-00007970: 0072 ef00 0000 72f1 0000 0072 3b00 0000  .r....r....r;...
-00007980: 7241 0000 0072 fa00 0000 7243 0000 0072  rA...r....rC...r
-00007990: fc00 0000 72fd 0000 0072 fe00 0000 7201  ....r....r....r.
-000079a0: 0100 0072 7400 0000 720b 0100 0072 8500  ...rt...r....r..
-000079b0: 0000 724d 0000 0072 0c01 0000 720e 0100  ..rM...r....r...
-000079c0: 0072 1001 0000 7211 0100 0072 1201 0000  .r....r....r....
-000079d0: 7217 0100 0072 0d01 0000 721a 0100 0072  r....r....r....r
-000079e0: 1b01 0000 721e 0100 0072 4e00 0000 7220  ....r....rN...r 
-000079f0: 0100 0072 2701 0000 7246 0000 0072 3b01  ...r'...rF...r;.
-00007a00: 0000 723e 0100 0072 3f01 0000 7242 0100  ..r>...r?...rB..
-00007a10: 0072 4401 0000 7245 0100 0072 4701 0000  .rD...rE...rG...
-00007a20: 724d 0100 0072 4e01 0000 725c 0000 0072  rM...rN...r\...r
-00007a30: 4101 0000 727f 0000 0072 8300 0000 72a8  A...r....r....r.
-00007a40: 0000 0072 9700 0000 7208 0000 0072 0800  ...r....r....r..
-00007a50: 0000 7208 0000 0072 0900 0000 da08 3c6d  ..r....r......<m
-00007a60: 6f64 756c 653e 0100 0000 73d4 0000 0008  odule>....s.....
-00007a70: 0108 0108 0110 0410 0408 0402 0402 0102  ................
-00007a80: 0102 0102 0106 fc0a 0608 0d08 100e 060e  ................
-00007a90: 0a08 0608 0812 0c08 0d18 0a08 2108 040a  ............!...
-00007aa0: 0408 0408 1d08 1408 1408 2f08 0408 0408  ........../.....
-00007ab0: 0412 0416 2e08 2108 200a 140e 1508 1a08  ......!. .......
-00007ac0: 040a 0408 0508 160a 050a ff08 2308 1708  ............#...
-00007ad0: 040a 0408 200a 1008 1708 0408 0408 0408  .... ...........
-00007ae0: 040c 0408 1508 1a08 1608 0408 0408 0408  ................
-00007af0: 0408 0608 0408 0408 040e 0b08 1408 0408  ................
-00007b00: 0408 0408 0a08 0c08 0408 0408 0508 0408  ................
-00007b10: 0b08 0408 0c0a 1608 0408 0608 0614 0412  ................
-00007b20: 0d12 0d08 2810 230c 0708 0408 0408 070a  ....(.#.........
-00007b30: 0408 080a 0e08 0808 0b08 0d08 0c08 1408  ................
-00007b40: 0a0c 12                                  ...
+00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
+00000050: 8400 6404 6504 8303 5a05 4700 6405 6406  ..d.e...Z.G.d.d.
+00000060: 8400 6406 6505 8303 5a06 6407 6408 8400  ..d.e...Z.d.d...
+00000070: 5a07 6507 6409 640a 640b 640c 640d 8d04  Z.e.d.d.d.d.d...
+00000080: 5a08 640e 640f 8400 5a09 6410 6411 8400  Z.d.d...Z.d.d...
+00000090: 5a0a 6508 6a0b 6601 6412 6413 8401 5a0c  Z.e.j.f.d.d...Z.
+000000a0: 6414 6415 8400 5a0d 6416 6417 8400 5a0e  d.d...Z.d.d...Z.
+000000b0: 4700 6418 6419 8400 6419 6501 6a0f 8303  G.d.d...d.e.j...
+000000c0: 5a10 641a 641b 8400 5a11 6700 6700 6401  Z.d.d...Z.g.g.d.
+000000d0: 6700 6700 6401 6700 6607 641c 641d 8401  g.g.d.g.f.d.d...
+000000e0: 5a12 641e 641f 8400 5a13 6420 6421 8400  Z.d.d...Z.d d!..
+000000f0: 5a14 64c6 6422 6423 8401 5a15 6424 6425  Z.d.d"d#..Z.d$d%
+00000100: 8400 5a16 6426 6427 8400 5a17 6428 6429  ..Z.d&d'..Z.d(d)
+00000110: 8400 5a18 642a 642b 8400 5a19 642c 642d  ..Z.d*d+..Z.d,d-
+00000120: 8400 5a1a 642e 642f 8400 5a1b 6430 6431  ..Z.d.d/..Z.d0d1
+00000130: 8400 5a1c 6432 6433 8400 5a1d 6700 6700  ..Z.d2d3..Z.g.g.
+00000140: 6401 6900 6604 6434 6435 8401 5a1e 6700  d.i.f.d4d5..Z.g.
+00000150: 6700 6700 6401 6401 6700 6606 6436 6437  g.g.d.d.g.f.d6d7
+00000160: 8401 5a1f 6438 6439 8400 5a20 643a 643b  ..Z.d8d9..Z d:d;
+00000170: 8400 5a21 64c7 643d 643e 8401 5a22 6400  ..Z!d.d=d>..Z"d.
+00000180: 643f 9c01 6440 6441 8402 5a23 6442 6443  d?..d@dA..Z#dBdC
+00000190: 8400 5a24 6444 6445 8400 5a25 64c8 6446  ..Z$dDdE..Z%d.dF
+000001a0: 6447 8401 5a26 6448 6449 8400 5a27 644a  dG..Z&dHdI..Z'dJ
+000001b0: 644b 8400 5a28 6401 6700 6700 6401 6401  dK..Z(d.g.g.d.d.
+000001c0: 6605 644c 644d 8401 5a29 644e 644f 8400  f.dLdM..Z)dNdO..
+000001d0: 5a2a 6450 6451 8400 5a2b 6452 6453 8400  Z*dPdQ..Z+dRdS..
+000001e0: 5a2c 64c6 6454 6455 8401 5a2d 6456 6457  Z,d.dTdU..Z-dVdW
+000001f0: 8400 5a2e 64c9 6459 645a 8401 5a2f 645b  ..Z.d.dYdZ..Z/d[
+00000200: 645c 8400 5a30 645d 645e 8400 5a31 645f  d\..Z0d]d^..Z1d_
+00000210: 6460 8400 5a32 6461 6462 8400 5a33 6463  d`..Z2dadb..Z3dc
+00000220: 6464 8400 5a34 6700 6601 6465 6466 8401  dd..Z4g.f.dedf..
+00000230: 5a35 6467 6468 8400 5a36 6469 646a 8400  Z5dgdh..Z6didj..
+00000240: 5a37 646b 646c 8400 5a38 646d 646e 8400  Z7dkdl..Z8dmdn..
+00000250: 5a39 646f 6470 8400 5a3a 6471 6472 8400  Z9dodp..Z:dqdr..
+00000260: 5a3b 6473 6474 8400 5a3c 6475 6476 8400  Z;dsdt..Z<dudv..
+00000270: 5a3d 6477 6478 8400 5a3e 64c6 6479 647a  Z=dwdx..Z>d.dydz
+00000280: 8401 5a3f 647b 647c 8400 5a40 6508 6a0b  ..Z?d{d|..Z@e.j.
+00000290: 6601 647d 647e 8401 5a41 647f 6480 8400  f.d}d~..ZAd.d...
+000002a0: 5a42 6481 6482 8400 5a43 6483 6484 8400  ZBd.d...ZCd.d...
+000002b0: 5a44 6485 6486 8400 5a45 6487 6488 8400  ZDd.d...ZEd.d...
+000002c0: 5a46 6489 648a 8400 5a47 648b 648c 8400  ZFd.d...ZGd.d...
+000002d0: 5a48 648d 648e 8400 5a49 648f 6490 8400  ZHd.d...ZId.d...
+000002e0: 5a4a 64c6 6491 6492 8401 5a4b 6493 6494  ZJd.d.d...ZKd.d.
+000002f0: 8400 5a4c 6495 6496 8400 5a4d 6497 6498  ..ZLd.d...ZMd.d.
+00000300: 8400 5a4e 64c8 6499 649a 8401 5a4f 649b  ..ZNd.d.d...ZOd.
+00000310: 649c 8400 5a50 649d 649e 8400 5a51 649f  d...ZPd.d...ZQd.
+00000320: 64a0 8400 5a52 6401 6401 6401 6508 6a0b  d...ZRd.d.d.e.j.
+00000330: 6604 64a1 64a2 8401 5a53 4700 64a3 64a4  f.d.d...ZSG.d.d.
+00000340: 8400 64a4 6500 6a54 8303 5a55 64a5 64a6  ..d.e.jT..ZUd.d.
+00000350: 8400 5a56 6700 6700 6700 6603 64a7 64a8  ..ZVg.g.g.f.d.d.
+00000360: 8401 5a57 6700 6601 64a9 64aa 8401 5a58  ..ZWg.f.d.d...ZX
+00000370: 64ab 64ac 8400 5a59 64ad 64ae 8400 5a5a  d.d...ZYd.d...ZZ
+00000380: 64af 64b0 8400 5a5b 64c6 64b1 64b2 8401  d.d...Z[d.d.d...
+00000390: 5a5c 64b3 64b4 8400 5a5d 64ca 64b6 64b7  Z\d.d...Z]d.d.d.
+000003a0: 8401 5a5e 64b8 64b9 8400 5a5f 64ba 64bb  ..Z^d.d...Z_d.d.
+000003b0: 8400 5a60 64bc 64bd 8400 5a61 64be 64bf  ..Z`d.d...Zad.d.
+000003c0: 8400 5a62 64c0 64c1 8400 5a63 64c2 64c3  ..Zbd.d...Zcd.d.
+000003d0: 8400 5a64 64c4 64c5 8400 5a65 6401 5300  ..Zdd.d...Zed.S.
+000003e0: 29cb e900 0000 004e 2901 da10 4657 414e  )......N)...FWAN
+000003f0: 6f64 6547 656e 6572 6174 6f72 6300 0000  odeGeneratorc...
+00000400: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000410: 0040 0000 00f3 0c00 0000 6500 5a01 6400  .@........e.Z.d.
+00000420: 5a02 6401 5300 2902 da05 4572 726f 724e  Z.d.S.)...ErrorN
+00000430: a903 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  ....__name__..__
+00000440: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000450: 6e61 6d65 5f5f a900 7209 0000 0072 0900  name__..r....r..
+00000460: 0000 fa43 2f68 6f6d 652f 7368 6169 2f66  ...C/home/shai/f
+00000470: 756e 5f77 6974 685f 6173 742f 6675 6e5f  un_with_ast/fun_
+00000480: 7769 7468 5f61 7374 2f6d 616e 6970 756c  with_ast/manipul
+00000490: 6174 655f 6e6f 6465 2f63 7265 6174 655f  ate_node/create_
+000004a0: 6e6f 6465 2e70 7972 0400 0000 0800 0000  node.pyr........
+000004b0: f304 0000 0008 0004 0172 0400 0000 6300  .........r....c.
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000004d0: 0000 0040 0000 0072 0300 0000 2902 da0a  ...@...r....)...
+000004e0: 496e 7661 6c69 6443 7478 4e72 0500 0000  InvalidCtxNr....
+000004f0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+00000500: 0a00 0000 720c 0000 000c 0000 0072 0b00  ....r........r..
+00000510: 0000 720c 0000 0063 0000 0000 0000 0000  ..r....c........
+00000520: 0000 0000 0100 0000 0400 0000 4b00 0000  ............K...
+00000530: 730c 0000 0074 0064 0164 027c 0083 0353  s....t.d.d.|...S
+00000540: 0029 034e da04 456e 756d 7209 0000 0029  .).N..Enumr....)
+00000550: 01da 0474 7970 6529 01da 0565 6e75 6d73  ...type)...enums
+00000560: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000570: 0d00 0000 1000 0000 f302 0000 000c 0172  ...............r
+00000580: 0d00 0000 da04 6c6f 6164 da05 7374 6f72  ......load..stor
+00000590: 65da 0664 656c 6574 65da 0570 6172 616d  e..delete..param
+000005a0: 2904 da04 4c4f 4144 da05 5354 4f52 45da  )...LOAD..STORE.
+000005b0: 0344 454c da05 5041 5241 4d63 0200 0000  .DEL..PARAMc....
+000005c0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
+000005d0: 4300 0000 7378 0000 0074 007c 0074 0183  C...sx...t.|.t..
+000005e0: 0273 0974 0264 0183 0182 0174 007c 0174  .s.t.d.....t.|.t
+000005f0: 0183 0273 1274 0264 0283 0182 0167 007d  ...s.t.d.....g.}
+00000600: 0267 007d 037c 0044 005d 077d 047c 02a0  .g.}.|.D.].}.|..
+00000610: 037c 04a1 0101 0071 187c 0144 005d 077d  .|.....q.|.D.].}
+00000620: 057c 03a0 037c 05a1 0101 0071 2264 0364  .|...|.....q"d.d
+00000630: 0484 007c 0244 0083 017d 0264 0564 0484  ...|.D...}.d.d..
+00000640: 007c 0344 0083 017d 037c 027c 0366 0253  .|.D...}.|.|.f.S
+00000650: 0029 064e fa13 6172 6773 206d 7573 7420  .).N..args must 
+00000660: 6265 2061 206c 6973 747a 1764 6566 6175  be a listz.defau
+00000670: 6c74 7320 6d75 7374 2062 6520 6120 6c69  lts must be a li
+00000680: 7374 6301 0000 0000 0000 0000 0000 0002  stc.............
+00000690: 0000 0004 0000 0053 0000 00f3 1400 0000  .......S........
+000006a0: 6700 7c00 5d06 7d01 7400 7c01 8301 9102  g.|.].}.t.|.....
+000006b0: 7102 5300 7209 0000 0029 01da 0d5f 5772  q.S.r....)..._Wr
+000006c0: 6170 5769 7468 4172 6773 a902 da02 2e30  apWithArgs.....0
+000006d0: da03 6172 6772 0900 0000 7209 0000 0072  ..argr....r....r
+000006e0: 0a00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+000006f0: 2600 0000 f302 0000 0014 007a 275f 546f  &..........z'_To
+00000700: 4172 6773 5769 7468 4465 6661 756c 7473  ArgsWithDefaults
+00000710: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000720: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00000730: 0002 0000 0004 0000 0053 0000 0072 1a00  .........S...r..
+00000740: 0000 7209 0000 00a9 01da 0d5f 5772 6170  ..r........_Wrap
+00000750: 5769 7468 4e61 6d65 2902 721d 0000 00da  WithName).r.....
+00000760: 0764 6566 6175 6c74 7209 0000 0072 0900  .defaultr....r..
+00000770: 0000 720a 0000 0072 1f00 0000 2700 0000  ..r....r....'...
+00000780: 7220 0000 0029 04da 0a69 7369 6e73 7461  r ...)...isinsta
+00000790: 6e63 65da 046c 6973 74da 0a56 616c 7565  nce..list..Value
+000007a0: 4572 726f 72da 0661 7070 656e 6429 06da  Error..append)..
+000007b0: 055f 6172 6773 da09 5f64 6566 6175 6c74  ._args.._default
+000007c0: 73da 0461 7267 73da 0864 6566 6175 6c74  s..args..default
+000007d0: 7372 1e00 0000 7223 0000 0072 0900 0000  sr....r#...r....
+000007e0: 7209 0000 0072 0a00 0000 da13 5f54 6f41  r....r......_ToA
+000007f0: 7267 7357 6974 6844 6566 6175 6c74 731b  rgsWithDefaults.
+00000800: 0000 0073 1a00 0000 0a01 0801 0a01 0801  ...s............
+00000810: 0401 0401 0801 0c01 0801 0c01 0e01 0e01  ................
+00000820: 0801 722c 0000 0063 0100 0000 0000 0000  ..r,...c........
+00000830: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00000840: 7318 0000 0074 007c 0074 016a 0283 0272  s....t.|.t.j...r
+00000850: 087c 0053 0074 037c 0083 0153 00a9 014e  .|.S.t.|...S...N
+00000860: 2904 7224 0000 00da 045f 6173 74da 0341  ).r$....._ast..A
+00000870: 5354 da03 4172 6729 01da 0774 6f5f 7772  ST..Arg)...to_wr
+00000880: 6170 7209 0000 0072 0900 0000 720a 0000  apr....r....r...
+00000890: 0072 1b00 0000 2b00 0000 7306 0000 000c  .r....+...s.....
+000008a0: 0104 0108 0172 1b00 0000 6302 0000 0000  .....r....c.....
+000008b0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+000008c0: 0000 0073 3c00 0000 7400 7c00 7401 6a02  ...s<...t.|.t.j.
+000008d0: 8302 7208 7c00 5300 7400 7c00 7403 8302  ..r.|.S.t.|.t...
+000008e0: 7211 7404 7c00 8301 5300 7400 7c00 7405  r.t.|...S.t.|.t.
+000008f0: 8302 721c 7406 7c00 7c01 6401 8d02 5300  ..r.t.|.|.d...S.
+00000900: 7407 8201 2902 4ea9 01da 0863 7478 5f74  t...).N....ctx_t
+00000910: 7970 6529 0872 2400 0000 722e 0000 0072  ype).r$...r....r
+00000920: 2f00 0000 da03 696e 74da 0843 6f6e 7374  /.....int..Const
+00000930: 616e 74da 0373 7472 da04 4e61 6d65 da13  ant..str..Name..
+00000940: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00000950: 726f 7229 0272 3100 0000 7233 0000 0072  ror).r1...r3...r
+00000960: 0900 0000 7209 0000 0072 0a00 0000 7222  ....r....r....r"
+00000970: 0000 0031 0000 0073 0e00 0000 0c01 0401  ...1...s........
+00000980: 0a01 0801 0a01 0c01 0401 7222 0000 0063  ..........r"...c
+00000990: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000009a0: 0300 0000 4300 0000 732c 0000 0074 007c  ....C...s,...t.|
+000009b0: 0064 0183 0273 1474 007c 0064 0283 0273  .d...s.t.|.d...s
+000009c0: 0c7c 0053 007c 006a 017d 0074 007c 0064  .|.S.|.j.}.t.|.d
+000009d0: 0183 0272 057c 0053 0029 034e da02 6964  ...r.|.S.).N..id
+000009e0: da05 7661 6c75 6529 02da 0768 6173 6174  ..value)...hasat
+000009f0: 7472 723a 0000 0029 01da 046e 6f64 6572  trr:...)...noder
+00000a00: 0900 0000 7209 0000 0072 0a00 0000 da15  ....r....r......
+00000a10: 5f4c 6566 746d 6f73 744e 6f64 6549 6e44  _LeftmostNodeInD
+00000a20: 6f74 5661 7241 0000 0073 0c00 0000 0a01  otVarA...s......
+00000a30: 0a01 0401 0601 0afd 0404 723d 0000 0063  ..........r=...c
+00000a40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000a50: 0500 0000 4300 0000 7338 0000 007c 0064  ....C...s8...|.d
+00000a60: 0075 0072 0874 0083 0067 017d 007c 0044  .u.r.t...g.}.|.D
+00000a70: 005d 0f7d 0174 017c 0174 026a 0383 0273  .].}.t.|.t.j...s
+00000a80: 1974 0464 01a0 057c 01a1 0183 0182 0171  .t.d...|.......q
+00000a90: 0a7c 0053 0029 024e fa59 416c 6c20 626f  .|.S.).N.YAll bo
+00000aa0: 6479 206e 6f64 6573 206d 7573 7420 6265  dy nodes must be
+00000ab0: 2073 746d 7420 6e6f 6465 732c 2061 6e64   stmt nodes, and
+00000ac0: 207b 7d20 6973 206e 6f74 2e20 5472 7920   {} is not. Try 
+00000ad0: 7772 6170 7069 6e67 2079 6f75 7220 6e6f  wrapping your no
+00000ae0: 6465 2069 6e20 616e 2045 7870 7220 6e6f  de in an Expr no
+00000af0: 6465 2e29 06da 0450 6173 7372 2400 0000  de.)...Passr$...
+00000b00: 722e 0000 00da 0473 746d 7472 2600 0000  r......stmtr&...
+00000b10: da06 666f 726d 6174 2902 da04 626f 6479  ..format)...body
+00000b20: da05 6368 696c 6472 0900 0000 7209 0000  ..childr....r...
+00000b30: 0072 0a00 0000 da15 466f 726d 6174 416e  .r......FormatAn
+00000b40: 6456 616c 6964 6174 6542 6f64 7949 0000  dValidateBodyI..
+00000b50: 0073 1400 0000 0801 0801 0801 0c01 0201  .s..............
+00000b60: 0201 0602 04fd 02ff 0405 7244 0000 0063  ..........rD...c
+00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b80: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
+00000b90: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
+00000ba0: 0387 0066 0164 0364 0484 085a 0487 0004  ...f.d.d...Z....
+00000bb0: 005a 0553 0029 05da 1243 6861 6e67 6543  .Z.S.)...ChangeC
+00000bc0: 7478 5472 616e 7366 6f72 6d63 0200 0000  txTransformc....
+00000bd0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000be0: 0300 0000 7318 0000 0074 0074 017c 0083  ....s....t.t.|..
+00000bf0: 02a0 02a1 0001 007c 017c 005f 0364 0053  .......|.|._.d.S
+00000c00: 0072 2d00 0000 2904 da05 7375 7065 7272  .r-...)...superr
+00000c10: 4500 0000 da08 5f5f 696e 6974 5f5f da0d  E.....__init__..
+00000c20: 5f6e 6577 5f63 7478 5f74 7970 6529 02da  _new_ctx_type)..
+00000c30: 0473 656c 66da 0c6e 6577 5f63 7478 5f74  .self..new_ctx_t
+00000c40: 7970 65a9 01da 095f 5f63 6c61 7373 5f5f  ype....__class__
+00000c50: 7209 0000 0072 0a00 0000 7247 0000 0057  r....r....rG...W
+00000c60: 0000 0073 0400 0000 0e01 0a01 7a1b 4368  ...s........z.Ch
+00000c70: 616e 6765 4374 7854 7261 6e73 666f 726d  angeCtxTransform
+00000c80: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
+00000c90: 0000 0000 0000 0200 0000 0300 0000 0300  ................
+00000ca0: 0000 732a 0000 0074 0074 017c 0083 02a0  ..s*...t.t.|....
+00000cb0: 027c 01a1 017d 0174 037c 0164 0183 0272  .|...}.t.|.d...r
+00000cc0: 1374 047c 006a 0583 017c 015f 067c 0153  .t.|.j...|._.|.S
+00000cd0: 0029 024e da03 6374 7829 0772 4600 0000  .).N..ctx).rF...
+00000ce0: 7245 0000 00da 0d67 656e 6572 6963 5f76  rE.....generic_v
+00000cf0: 6973 6974 723b 0000 00da 0647 6574 4374  isitr;.....GetCt
+00000d00: 7872 4800 0000 724d 0000 0029 0272 4900  xrH...rM...).rI.
+00000d10: 0000 723c 0000 0072 4b00 0000 7209 0000  ..r<...rK...r...
+00000d20: 0072 0a00 0000 724e 0000 005b 0000 0073  .r....rN...[...s
+00000d30: 0800 0000 1001 0a01 0c01 0401 7a20 4368  ............z Ch
+00000d40: 616e 6765 4374 7854 7261 6e73 666f 726d  angeCtxTransform
+00000d50: 2e67 656e 6572 6963 5f76 6973 6974 2906  .generic_visit).
+00000d60: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00000d70: 4700 0000 724e 0000 00da 0d5f 5f63 6c61  G...rN.....__cla
+00000d80: 7373 6365 6c6c 5f5f 7209 0000 0072 0900  sscell__r....r..
+00000d90: 0000 724b 0000 0072 0a00 0000 7245 0000  ..rK...r....rE..
+00000da0: 0055 0000 0073 0600 0000 0800 0c02 1404  .U...s..........
+00000db0: 7245 0000 0063 0200 0000 0000 0000 0000  rE...c..........
+00000dc0: 0000 0300 0000 0300 0000 4300 0000 7316  ..........C...s.
+00000dd0: 0000 0074 007c 0183 017d 027c 02a0 017c  ...t.|...}.|...|
+00000de0: 00a1 0101 0064 0053 0072 2d00 0000 2902  .....d.S.r-...).
+00000df0: 7245 0000 00da 0576 6973 6974 2903 723c  rE.....visit).r<
+00000e00: 0000 0072 4a00 0000 da09 7472 616e 7366  ...rJ.....transf
+00000e10: 6f72 6d72 0900 0000 7209 0000 0072 0a00  ormr....r....r..
+00000e20: 0000 da09 4368 616e 6765 4374 7862 0000  ....ChangeCtxb..
+00000e30: 0073 0400 0000 0801 0e01 7253 0000 0063  .s........rS...c
+00000e40: 0700 0000 0000 0000 0000 0000 0700 0000  ................
+00000e50: 0900 0000 4300 0000 7350 0000 0074 007c  ....C...sP...t.|
+00000e60: 0174 0183 0273 0974 0264 0183 0182 017c  .t...s.t.d.....|
+00000e70: 0572 0f74 037c 0583 017d 057c 0272 1574  .r.t.|...}.|.r.t
+00000e80: 037c 0283 017d 0274 047c 017c 0683 025c  .|...}.t.|.|...\
+00000e90: 027d 017d 0674 056a 067c 007c 017c 027c  .}.}.t.j.|.|.|.|
+00000ea0: 037c 047c 057c 0664 028d 0753 0029 0361  .|.|.|.d...S.).a
+00000eb0: 8d01 0000 4372 6561 7465 7320 616e 205f  ....Creates an _
+00000ec0: 6173 742e 4675 6e63 7469 6f6e 4465 6620  ast.FunctionDef 
+00000ed0: 6e6f 6465 2e0a 0a20 2041 7267 733a 0a20  node...  Args:. 
+00000ee0: 2020 2061 7267 733a 2041 206c 6973 7420     args: A list 
+00000ef0: 6f66 2061 7267 732e 0a20 2020 206b 6579  of args..    key
+00000f00: 733a 2041 206c 6973 7420 6f66 206b 6579  s: A list of key
+00000f10: 732c 206d 7573 7420 6265 2074 6865 2073  s, must be the s
+00000f20: 616d 6520 6c65 6e67 7468 2061 7320 7661  ame length as va
+00000f30: 6c75 6573 2e0a 2020 2020 7661 6c75 6573  lues..    values
+00000f40: 3a20 4120 6c69 7374 206f 6620 7661 6c75  : A list of valu
+00000f50: 6573 2c20 636f 7272 6573 706f 6e64 2074  es, correspond t
+00000f60: 6f20 6b65 7973 2e0a 2020 2020 7661 7261  o keys..    vara
+00000f70: 7267 5f6e 616d 653a 2054 6865 206e 616d  rg_name: The nam
+00000f80: 6520 6f66 2074 6865 2076 6172 6172 6720  e of the vararg 
+00000f90: 7661 7269 6162 6c65 2c20 6f72 204e 6f6e  variable, or Non
+00000fa0: 652e 0a20 2020 206b 7761 7267 5f6e 616d  e..    kwarg_nam
+00000fb0: 653a 2054 6865 206e 616d 6520 6f66 2074  e: The name of t
+00000fc0: 6865 206b 7761 7267 7320 7661 7269 6162  he kwargs variab
+00000fd0: 6c65 2c20 6f72 204e 6f6e 652e 0a0a 2020  le, or None...  
+00000fe0: 5261 6973 6573 3a0a 2020 2020 5661 6c75  Raises:.    Valu
+00000ff0: 6545 7272 6f72 3a20 4966 206c 656e 286b  eError: If len(k
+00001000: 6579 7329 2021 3d20 6c65 6e28 7661 6c75  eys) != len(valu
+00001010: 6573 292e 0a0a 2020 5265 7475 726e 733a  es)...  Returns:
+00001020: 0a20 2020 2041 6e20 5f61 7374 2e46 756e  .    An _ast.Fun
+00001030: 6374 696f 6e44 6566 206e 6f64 652e 0a20  ctionDef node.. 
+00001040: 2072 1900 0000 a907 da0b 706f 736f 6e6c   r........posonl
+00001050: 7961 7267 7372 2a00 0000 da06 7661 7261  yargsr*.....vara
+00001060: 7267 da0a 6b77 6f6e 6c79 6172 6773 da0b  rg..kwonlyargs..
+00001070: 6b77 5f64 6566 6175 6c74 73da 056b 7761  kw_defaults..kwa
+00001080: 7267 722b 0000 0029 0772 2400 0000 7225  rgr+...).r$...r%
+00001090: 0000 0072 2600 0000 721b 0000 0072 2c00  ...r&...r....r,.
+000010a0: 0000 722e 0000 00da 0961 7267 756d 656e  ..r......argumen
+000010b0: 7473 7254 0000 0072 0900 0000 7209 0000  tsrT...r....r...
+000010c0: 0072 0a00 0000 725a 0000 006c 0000 0073  .r....rZ...l...s
+000010d0: 2000 0000 0a10 0801 0401 0801 0401 0801   ...............
+000010e0: 0e01 0401 0201 0201 0201 0201 0201 0201  ................
+000010f0: 0201 06f9 725a 0000 0063 0000 0000 0000  ....rZ...c......
+00001100: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00001110: 0000 f308 0000 0074 00a0 01a1 0053 0072  .......t.....S.r
+00001120: 2d00 0000 2902 722e 0000 00da 0341 6464  -...).r......Add
+00001130: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+00001140: 0a00 0000 725c 0000 008d 0000 00f3 0200  ....r\..........
+00001150: 0000 0801 725c 0000 0063 0000 0000 0000  ....r\...c......
+00001160: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00001170: 0000 725b 0000 0072 2d00 0000 2902 722e  ..r[...r-...).r.
+00001180: 0000 00da 0341 6e64 7209 0000 0072 0900  .....Andr....r..
+00001190: 0000 7209 0000 0072 0a00 0000 725e 0000  ..r....r....r^..
+000011a0: 0091 0000 0072 5d00 0000 725e 0000 0063  .....r]...r^...c
+000011b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000011c0: 0400 0000 4300 0000 730e 0000 0074 006a  ....C...s....t.j
+000011d0: 017c 007c 0164 018d 0253 0029 024e 2902  .|.|.d...S.).N).
+000011e0: da04 7465 7374 da03 6d73 6729 0272 2e00  ..test..msg).r..
+000011f0: 0000 da06 4173 7365 7274 2902 da05 6368  ....Assert)...ch
+00001200: 6563 6bda 076d 6573 7361 6765 7209 0000  eck..messager...
+00001210: 0072 0900 0000 720a 0000 0072 6100 0000  .r....r....ra...
+00001220: 9500 0000 7302 0000 000e 0172 6100 0000  ....s......ra...
+00001230: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
+00001240: 0007 0000 0043 0000 0073 7200 0000 7400  .....C...sr...t.
+00001250: 7c00 7401 7402 6602 8302 730b 7c00 6701  |.t.t.f...s.|.g.
+00001260: 7d02 6e02 7c00 7d02 6700 7d03 7c02 4400  }.n.|.}.g.}.|.D.
+00001270: 5d17 7d04 7400 7c04 7403 8302 7223 7c03  ].}.t.|.t...r#|.
+00001280: a004 7405 7c04 7406 6a07 6401 8d02 a101  ..t.|.t.j.d.....
+00001290: 0100 7111 7c03 a004 7c04 a101 0100 7111  ..q.|...|.....q.
+000012a0: 7408 7c01 8301 7d05 7409 6a0a 7c03 7c01  t.|...}.t.j.|.|.
+000012b0: 6402 8d02 7d06 7c05 7c06 5f0b 7c06 5300  d...}.|.|._.|.S.
+000012c0: 2903 6123 0100 0043 7265 6174 6573 2061  ).a#...Creates a
+000012d0: 6e20 5f61 7374 2e41 7373 6967 6e20 6e6f  n _ast.Assign no
+000012e0: 6465 2e0a 0a20 2041 7267 733a 0a20 2020  de...  Args:.   
+000012f0: 206c 6566 743a 2054 6865 206e 6f64 6520   left: The node 
+00001300: 6f6e 2074 6865 206c 6566 7420 7369 6465  on the left side
+00001310: 206f 6620 7468 6520 6571 7561 6c20 7369   of the equal si
+00001320: 676e 2e0a 2020 2020 2020 4d61 7920 6569  gn..      May ei
+00001330: 7468 6572 2062 6520 6120 6e6f 6465 2c20  ther be a node, 
+00001340: 6f72 2061 2073 7472 696e 672c 2077 6869  or a string, whi
+00001350: 6368 2077 696c 6c20 6175 746f 6d61 7469  ch will automati
+00001360: 6361 6c6c 7920 6765 740a 2020 2020 2020  cally get.      
+00001370: 636f 6e76 6572 7465 6420 746f 2061 206e  converted to a n
+00001380: 616d 6520 6e6f 6465 2e0a 2020 2020 7269  ame node..    ri
+00001390: 6768 743a 2054 6865 206e 6f64 6520 6f6e  ght: The node on
+000013a0: 2074 6865 2072 6967 6874 2073 6964 6520   the right side 
+000013b0: 6f66 2074 6865 2065 7175 616c 2073 6967  of the equal sig
+000013c0: 6e2e 0a0a 2020 5265 7475 726e 733a 0a20  n...  Returns:. 
+000013d0: 2020 2041 6e20 5f61 7374 2e41 7373 6967     An _ast.Assig
+000013e0: 6e20 6e6f 6465 2e0a 2020 7232 0000 0029  n node..  r2...)
+000013f0: 02da 0774 6172 6765 7473 723a 0000 0029  ...targetsr:...)
+00001400: 0c72 2400 0000 7225 0000 00da 0574 7570  .r$...r%.....tup
+00001410: 6c65 7236 0000 0072 2700 0000 7222 0000  ler6...r'...r"..
+00001420: 00da 0743 7478 456e 756d 7216 0000 00da  ...CtxEnumr.....
+00001430: 0d5f 6578 7472 6163 745f 6261 7365 722e  ._extract_baser.
+00001440: 0000 00da 0641 7373 6967 6eda 0462 6173  .....Assign..bas
+00001450: 6529 07da 046c 6566 74da 0572 6967 6874  e)...left..right
+00001460: 7264 0000 00da 0b6e 6577 5f74 6172 6765  rd.....new_targe
+00001470: 7473 da06 7461 7267 6574 7269 0000 00da  ts..targetri....
+00001480: 0672 6573 756c 7472 0900 0000 7209 0000  .resultr....r...
+00001490: 0072 0a00 0000 7268 0000 0099 0000 0073  .r....rh.......s
+000014a0: 1e00 0000 0e0c 0801 0402 0401 0801 0a01  ................
+000014b0: 1601 0c02 0801 0401 0201 0201 06fe 0603  ................
+000014c0: 0401 7268 0000 0063 0300 0000 0000 0000  ..rh...c........
+000014d0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+000014e0: 7318 0000 0074 007c 0083 017d 0074 016a  s....t.|...}.t.j
+000014f0: 027c 007c 017c 0264 018d 0353 0029 0261  .|.|.|.d...S.).a
+00001500: 3701 0000 4372 6561 7465 7320 616e 205f  7...Creates an _
+00001510: 6173 742e 4175 6741 7373 6967 6e20 6e6f  ast.AugAssign no
+00001520: 6465 2e0a 0a20 2041 7267 733a 0a20 2020  de...  Args:.   
+00001530: 206c 6566 743a 2054 6865 206e 6f64 6520   left: The node 
+00001540: 6f6e 2074 6865 206c 6566 7420 7369 6465  on the left side
+00001550: 206f 6620 7468 6520 6571 7561 6c20 7369   of the equal si
+00001560: 676e 2e0a 2020 2020 2020 4d61 7920 6569  gn..      May ei
+00001570: 7468 6572 2062 6520 6120 6e6f 6465 2c20  ther be a node, 
+00001580: 6f72 2061 2073 7472 696e 672c 2077 6869  or a string, whi
+00001590: 6368 2077 696c 6c20 6175 746f 6d61 7469  ch will automati
+000015a0: 6361 6c6c 7920 6765 740a 2020 2020 2020  cally get.      
+000015b0: 636f 6e76 6572 7465 6420 746f 2061 206e  converted to a n
+000015c0: 616d 6520 6e6f 6465 2e0a 2020 2020 6f70  ame node..    op
+000015d0: 3a20 4f70 6572 6174 6f72 0a20 2020 2072  : Operator.    r
+000015e0: 6967 6874 3a20 5468 6520 6e6f 6465 206f  ight: The node o
+000015f0: 6e20 7468 6520 7269 6768 7420 7369 6465  n the right side
+00001600: 206f 6620 7468 6520 6571 7561 6c20 7369   of the equal si
+00001610: 676e 2e0a 0a20 2052 6574 7572 6e73 3a0a  gn...  Returns:.
+00001620: 2020 2020 416e 205f 6173 742e 4173 7369      An _ast.Assi
+00001630: 676e 206e 6f64 652e 0a20 2029 0372 6d00  gn node..  ).rm.
+00001640: 0000 da02 6f70 723a 0000 0029 0372 2200  ....opr:...).r".
+00001650: 0000 722e 0000 00da 0941 7567 4173 7369  ..r......AugAssi
+00001660: 676e a903 726a 0000 0072 6f00 0000 726b  gn..rj...ro...rk
+00001670: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00001680: 0000 7270 0000 00b6 0000 0073 0c00 0000  ..rp.......s....
+00001690: 080d 0401 0201 0201 0201 06fd 7270 0000  ............rp..
+000016a0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+000016b0: 0000 0500 0000 4300 0000 7324 0000 0074  ......C...s$...t
+000016c0: 007c 0174 016a 0283 0273 0a74 037c 0183  .|.t.j...s.t.|..
+000016d0: 017d 0174 016a 047c 007c 017c 0264 018d  .}.t.j.|.|.|.d..
+000016e0: 0353 0029 027a fa43 7265 6174 6573 2061  .S.).z.Creates a
+000016f0: 6e20 5f61 7374 2e42 696e 4f70 206e 6f64  n _ast.BinOp nod
+00001700: 652e 0a0a 2020 4172 6773 3a0a 2020 2020  e...  Args:.    
+00001710: 6c65 6674 3a20 5468 6520 6e6f 6465 206f  left: The node o
+00001720: 6e20 7468 6520 6c65 6674 2073 6964 6520  n the left side 
+00001730: 6f66 2074 6865 2065 7175 616c 2073 6967  of the equal sig
+00001740: 6e2e 0a20 2020 206f 703a 2054 6865 206f  n..    op: The o
+00001750: 7065 7261 746f 722e 204c 6974 6572 616c  perator. Literal
+00001760: 2076 616c 7565 7320 6173 2073 7472 696e   values as strin
+00001770: 6773 2061 6c73 6f20 6163 6365 7074 6564  gs also accepted
+00001780: 3a0a 2020 2020 7269 6768 743a 2054 6865  :.    right: The
+00001790: 206e 6f64 6520 6f6e 2074 6865 2072 6967   node on the rig
+000017a0: 6874 2073 6964 6520 6f66 2074 6865 2065  ht side of the e
+000017b0: 7175 616c 2073 6967 6e2e 0a0a 2020 5265  qual sign...  Re
+000017c0: 7475 726e 733a 0a20 2020 2041 6e20 5f61  turns:.    An _a
+000017d0: 7374 2e42 696e 4f70 206e 6f64 652e 0a20  st.BinOp node.. 
+000017e0: 2072 7100 0000 2905 7224 0000 0072 2e00   rq...).r$...r..
+000017f0: 0000 722f 0000 00da 0842 696e 4f70 4d61  ..r/.....BinOpMa
+00001800: 70da 0542 696e 4f70 7271 0000 0072 0900  p..BinOprq...r..
+00001810: 0000 7209 0000 0072 0a00 0000 7273 0000  ..r....r....rs..
+00001820: 00ca 0000 0073 0e00 0000 0c0b 0801 0402  .....s..........
+00001830: 0201 0201 0201 06fd 7273 0000 0063 0100  ........rs...c..
+00001840: 0000 0000 0000 0000 0000 0700 0000 0500  ................
+00001850: 0000 4700 0000 73d0 0000 007c 0067 017d  ..G...s....|.g.}
+00001860: 0264 017d 0364 027d 0474 007c 0183 017d  .d.}.d.}.t.|...}
+00001870: 017c 0172 617c 01a0 0164 03a1 017d 057c  .|.ra|...d...}.|
+00001880: 0472 5774 027c 0574 036a 0483 0273 1e74  .rWt.|.t.j...s.t
+00001890: 057c 0583 017d 057c 0373 237c 057d 036e  .|...}.|.s#|.}.n
+000018a0: 397c 0372 2a7c 037c 056b 0272 2a71 0b74  9|.r*|.|.k.r*q.t
+000018b0: 027c 0374 036a 0683 0272 3e74 0774 036a  .|.t.j...r>t.t.j
+000018c0: 077c 037c 0264 048d 027c 0567 027c 01a2  .|.|.d...|.g.|..
+000018d0: 0152 008e 0053 007c 02a0 01a1 007d 067c  .R...S.|.....}.|
+000018e0: 02a0 0874 077c 067c 0567 027c 01a2 0152  ...t.|.|.g.|...R
+000018f0: 008e 00a1 0101 0074 036a 0774 03a0 09a1  .......t.j.t....
+00001900: 007c 0264 048d 0253 007c 02a0 087c 05a1  .|.d...S.|...|..
+00001910: 0101 007c 040c 007d 047c 0173 0d74 036a  ...|...}.|.s.t.j
+00001920: 077c 037c 0264 048d 0253 0029 0561 5d01  .|.|.d...S.).a].
+00001930: 0000 4372 6561 7465 7320 616e 205f 6173  ..Creates an _as
+00001940: 742e 426f 6f6c 4f70 206e 6f64 652e 0a0a  t.BoolOp node...
+00001950: 2020 4172 6773 3a0a 2020 2020 6c65 6674    Args:.    left
+00001960: 3a20 5468 6520 6e6f 6465 206f 6e20 7468  : The node on th
+00001970: 6520 6c65 6674 2073 6964 6520 6f66 2074  e left side of t
+00001980: 6865 2065 7175 616c 2073 6967 6e2e 0a20  he equal sign.. 
+00001990: 2020 202a 616c 7465 726e 6174 696e 675f     *alternating_
+000019a0: 6f70 735f 7661 6c75 6573 3a20 416e 2061  ops_values: An a
+000019b0: 6c74 6572 6e61 7469 6e67 206c 6973 7420  lternating list 
+000019c0: 6f66 206f 7073 2061 6e64 2065 7870 7265  of ops and expre
+000019d0: 7373 696f 6e73 2e0a 2020 2020 2020 4e6f  ssions..      No
+000019e0: 7465 2074 6861 7420 5f61 7374 2e4e 6f74  te that _ast.Not
+000019f0: 2069 7320 6e6f 7420 6120 7661 6c69 6420   is not a valid 
+00001a00: 626f 6f6c 6561 6e20 6f70 6572 6174 6f72  boolean operator
+00001a10: 2c20 6974 2069 7320 636f 6e73 6964 6572  , it is consider
+00001a20: 6564 0a20 2020 2020 2061 2075 6e61 7279  ed.      a unary
+00001a30: 206f 7065 7261 746f 722e 0a20 2020 2020   operator..     
+00001a40: 2046 6f72 2065 7861 6d70 6c65 3a20 285f   For example: (_
+00001a50: 6173 742e 4f72 2c20 5f61 7374 2e4e 616d  ast.Or, _ast.Nam
+00001a60: 6528 2761 2729 290a 0a20 2052 6574 7572  e('a'))..  Retur
+00001a70: 6e73 3a0a 2020 2020 416e 205f 6173 742e  ns:.    An _ast.
+00001a80: 426f 6f6c 4f70 206e 6f64 652e 0a20 204e  BoolOp node..  N
+00001a90: 5472 0100 0000 2902 726f 0000 00da 0676  Tr....).ro.....v
+00001aa0: 616c 7565 7329 0a72 2500 0000 da03 706f  alues).r%.....po
+00001ab0: 7072 2400 0000 722e 0000 0072 2f00 0000  pr$...r....r/...
+00001ac0: da09 426f 6f6c 4f70 4d61 7072 5e00 0000  ..BoolOpMapr^...
+00001ad0: da06 426f 6f6c 4f70 7227 0000 00da 024f  ..BoolOpr'.....O
+00001ae0: 7229 0772 6a00 0000 da16 616c 7465 726e  r).rj.....altern
+00001af0: 6174 696e 675f 6f70 735f 7661 6c75 6573  ating_ops_values
+00001b00: 7274 0000 0072 6f00 0000 da07 6f70 5f6e  rt...ro.....op_n
+00001b10: 6578 74da 0b6f 705f 6f72 5f76 616c 7565  ext..op_or_value
+00001b20: da0a 6c61 7374 5f76 616c 7565 7209 0000  ..last_valuer...
+00001b30: 0072 0900 0000 720a 0000 0072 7700 0000  .r....r....rw...
+00001b40: de00 0000 7342 0000 0006 0d04 0104 0108  ....sB..........
+00001b50: 0104 010a 0104 010c 0108 0104 0106 010c  ................
+00001b60: 0102 010c 030e 0102 0102 ff02 0208 fe08  ................
+00001b70: 0408 0102 0102 ff02 020a fe04 0306 0102  ................
+00001b80: 0106 fe0a 0406 0104 e70e 1b72 7700 0000  ...........rw...
+00001b90: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001ba0: 0002 0000 0043 0000 0072 5b00 0000 722d  .....C...r[...r-
+00001bb0: 0000 0029 0272 2e00 0000 da06 4269 7441  ...).r......BitA
+00001bc0: 6e64 7209 0000 0072 0900 0000 7209 0000  ndr....r....r...
+00001bd0: 0072 0a00 0000 727d 0000 000d 0100 0072  .r....r}.......r
+00001be0: 5d00 0000 727d 0000 0063 0000 0000 0000  ]...r}...c......
+00001bf0: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00001c00: 0000 725b 0000 0072 2d00 0000 2902 722e  ..r[...r-...).r.
+00001c10: 0000 00da 0542 6974 4f72 7209 0000 0072  .....BitOrr....r
+00001c20: 0900 0000 7209 0000 0072 0a00 0000 727e  ....r....r....r~
+00001c30: 0000 0011 0100 0072 5d00 0000 727e 0000  .......r]...r~..
+00001c40: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001c50: 0000 0200 0000 4300 0000 725b 0000 0072  ......C...r[...r
+00001c60: 2d00 0000 2902 722e 0000 00da 0642 6974  -...).r......Bit
+00001c70: 586f 7272 0900 0000 7209 0000 0072 0900  Xorr....r....r..
+00001c80: 0000 720a 0000 0072 7f00 0000 1501 0000  ..r....r........
+00001c90: 725d 0000 0072 7f00 0000 6302 0000 0000  r]...r....c.....
+00001ca0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00001cb0: 0000 0073 0c00 0000 7400 a001 7c00 7c01  ...s....t...|.|.
+00001cc0: a102 5300 722d 0000 0029 0272 2e00 0000  ..S.r-...).r....
+00001cd0: da07 6b65 7977 6f72 6429 0272 1e00 0000  ..keyword).r....
+00001ce0: 723a 0000 0072 0900 0000 7209 0000 0072  r:...r....r....r
+00001cf0: 0a00 0000 7280 0000 0019 0100 0072 1000  ....r........r..
+00001d00: 0000 7280 0000 0063 0500 0000 0000 0000  ..r....c........
+00001d10: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
+00001d20: 73ac 0000 0074 007c 0174 0183 0273 0974  s....t.|.t...s.t
+00001d30: 0264 0183 0182 0174 007c 0074 0383 0272  .d.....t.|.t...r
+00001d40: 1574 047c 00a0 0564 02a1 018e 007d 0074  .t.|...d.....}.t
+00001d50: 007c 0474 0683 0273 1e74 0264 0383 0182  .|.t...s.t.d....
+00001d60: 0174 007c 0074 076a 0874 076a 0966 0283  .t.|.t.j.t.j.f..
+00001d70: 0273 2b74 0264 0483 0182 0164 0564 0684  .s+t.d.....d.d..
+00001d80: 007c 0144 0083 017d 0174 007c 0374 0383  .|.D...}.t.|.t..
+00001d90: 0272 3e74 047c 03a0 0564 02a1 018e 007d  .r>t.|...d.....}
+00001da0: 0374 007c 0474 0383 0272 4a74 047c 04a0  .t.|.t...rJt.|..
+00001db0: 0564 02a1 018e 007d 0474 076a 0a7c 007c  .d.....}.t.j.|.|
+00001dc0: 017c 027c 037c 0464 078d 057d 057c 0553  .|.|.|.d...}.|.S
+00001dd0: 0029 0861 8802 0000 4372 6561 7465 7320  .).a....Creates 
+00001de0: 616e 205f 6173 742e 4361 6c6c 206e 6f64  an _ast.Call nod
+00001df0: 652e 0a0a 2020 4172 6773 3a0a 2020 2020  e...  Args:.    
+00001e00: 6361 6c6c 6572 3a20 4569 7468 6572 2061  caller: Either a
+00001e10: 206e 6f64 6520 6f66 2074 6865 2061 7070   node of the app
+00001e20: 726f 7072 6961 7465 2074 7970 650a 2020  ropriate type.  
+00001e30: 2020 2020 285f 6173 742e 5374 722c 205f      (_ast.Str, _
+00001e40: 6173 742e 4e61 6d65 2c20 6f72 205f 6173  ast.Name, or _as
+00001e50: 742e 4174 7472 6962 7574 6529 2c20 6f72  t.Attribute), or
+00001e60: 2061 2064 6f74 2d73 6570 6172 6174 6564   a dot-separated
+00001e70: 2073 7472 696e 672e 0a20 2020 2061 7267   string..    arg
+00001e80: 733a 2041 206c 6973 7420 6f66 2061 7267  s: A list of arg
+00001e90: 732e 0a20 2020 206b 6579 733a 2041 206c  s..    keys: A l
+00001ea0: 6973 7420 6f66 206b 6579 732c 206d 7573  ist of keys, mus
+00001eb0: 7420 6265 2074 6865 2073 616d 6520 6c65  t be the same le
+00001ec0: 6e67 7468 2061 7320 7661 6c75 6573 2e0a  ngth as values..
+00001ed0: 2020 2020 7661 6c75 6573 3a20 4120 6c69      values: A li
+00001ee0: 7374 206f 6620 7661 6c75 6573 2c20 636f  st of values, co
+00001ef0: 7272 6573 706f 6e64 2074 6f20 6b65 7973  rrespond to keys
+00001f00: 2e0a 2020 2020 7374 6172 6172 6773 3a20  ..    starargs: 
+00001f10: 4120 6e6f 6465 2077 6974 6820 6120 7374  A node with a st
+00001f20: 6172 2069 6e20 6672 6f6e 7420 6f66 2069  ar in front of i
+00001f30: 742e 2050 6173 7369 6e67 2061 2073 7472  t. Passing a str
+00001f40: 696e 6720 7769 6c6c 2062 650a 2020 2020  ing will be.    
+00001f50: 2020 696e 7465 7270 7265 7465 6420 6173    interpreted as
+00001f60: 2061 2056 6172 5265 6665 7265 6e63 652e   a VarReference.
+00001f70: 0a20 2020 206b 7761 7267 733a 2041 206e  .    kwargs: A n
+00001f80: 6f64 6520 7769 7468 2074 776f 2073 7461  ode with two sta
+00001f90: 7273 2069 6e20 6672 6f6e 7420 6f66 2069  rs in front of i
+00001fa0: 742e 2050 6173 7369 6e67 2061 2073 7472  t. Passing a str
+00001fb0: 696e 6720 7769 6c6c 2062 650a 2020 2020  ing will be.    
+00001fc0: 2020 696e 7465 7270 7265 7465 6420 6173    interpreted as
+00001fd0: 2061 2056 6172 5265 6665 7265 6e63 652e   a VarReference.
+00001fe0: 0a0a 2020 5261 6973 6573 3a0a 2020 2020  ..  Raises:.    
+00001ff0: 5661 6c75 6545 7272 6f72 3a20 4966 206c  ValueError: If l
+00002000: 656e 286b 6579 7329 2021 3d20 6c65 6e28  en(keys) != len(
+00002010: 7661 6c75 6573 2920 6f72 2063 616c 6c65  values) or calle
+00002020: 7220 6973 206e 6f74 2074 6865 2072 6967  r is not the rig
+00002030: 6874 2074 7970 652e 0a0a 2020 5265 7475  ht type...  Retu
+00002040: 726e 733a 0a20 2020 2041 6e20 5f61 7374  rns:.    An _ast
+00002050: 2e43 616c 6c20 6f62 6a65 6374 2e0a 2020  .Call object..  
+00002060: 7219 0000 00da 012e 7a19 6b77 6172 6773  r.......z.kwargs
+00002070: 206d 7573 7420 6265 2061 2061 7374 2e44   must be a ast.D
+00002080: 6963 747a 1d63 616c 6c65 7220 6e6f 7420  ictz.caller not 
+00002090: 7468 6520 6578 7065 6374 6564 2076 616c  the expected val
+000020a0: 7565 6301 0000 0000 0000 0000 0000 0002  uec.............
+000020b0: 0000 0006 0000 0053 0000 00f3 1a00 0000  .......S........
+000020c0: 6700 7c00 5d09 7d01 7400 7c01 7401 6a02  g.|.].}.t.|.t.j.
+000020d0: 6400 8d02 9102 7102 5300 a901 7232 0000  d.....q.S...r2..
+000020e0: 00a9 0372 2200 0000 7266 0000 0072 1500  ...r"...rf...r..
+000020f0: 0000 721c 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00002100: 0072 0a00 0000 721f 0000 003d 0100 00f3  .r....r....=....
+00002110: 0200 0000 1a00 7a18 4361 6c6c 2e3c 6c6f  ......z.Call.<lo
+00002120: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00002130: 2905 da04 6675 6e63 722a 0000 00da 086b  )...funcr*.....k
+00002140: 6579 776f 7264 73da 0873 7461 7261 7267  eywords..stararg
+00002150: 73da 066b 7761 7267 7329 0b72 2400 0000  s..kwargs).r$...
+00002160: 7225 0000 0072 2600 0000 7236 0000 00da  r%...r&...r6....
+00002170: 0c56 6172 5265 6665 7265 6e63 65da 0573  .VarReference..s
+00002180: 706c 6974 da04 6469 6374 722e 0000 0072  plit..dictr....r
+00002190: 3700 0000 da09 4174 7472 6962 7574 65da  7.....Attribute.
+000021a0: 0443 616c 6c29 06da 0663 616c 6c65 7272  .Call)...callerr
+000021b0: 2a00 0000 7287 0000 0072 8800 0000 7289  *...r....r....r.
+000021c0: 0000 0072 6e00 0000 7209 0000 0072 0900  ...rn...r....r..
+000021d0: 0000 720a 0000 0072 8e00 0000 1d01 0000  ..r....r........
+000021e0: 732a 0000 000a 1408 010a 050e 010a 0108  s*..............
+000021f0: 0112 0108 010e 010a 010e 010a 010e 0104  ................
+00002200: 0102 0102 0102 0102 0102 0106 fb04 0672  ...............r
+00002210: 8e00 0000 6307 0000 0000 0000 0000 0000  ....c...........
+00002220: 0007 0000 0007 0000 0043 0000 0073 6c00  .........C...sl.
+00002230: 0000 7c02 7306 7400 6401 8301 8201 7c05  ..|.s.t.d.....|.
+00002240: 6402 7501 720e 7401 6403 8301 8201 7c04  d.u.r.t.d.....|.
+00002250: 6402 7501 7216 7401 6404 8301 8201 7402  d.u.r.t.d.....t.
+00002260: 7c01 7403 8302 731f 7400 6405 8301 8201  |.t...s.t.d.....
+00002270: 7404 7c02 8301 7d02 6406 6407 8400 7c01  t.|...}.d.d...|.
+00002280: 4400 8301 7d01 7405 6a06 7c00 7c01 7c02  D...}.t.j.|.|.|.
+00002290: 7c03 7403 7c06 8301 6408 8d05 5300 2909  |.t.|...d...S.).
+000022a0: 615a 0100 0043 7265 6174 6573 2061 6e20  aZ...Creates an 
+000022b0: 5f61 7374 2e43 6c61 7373 4465 6620 6e6f  _ast.ClassDef no
+000022c0: 6465 2e0a 0a20 2041 7267 733a 0a20 2020  de...  Args:.   
+000022d0: 206e 616d 653a 2054 6865 206e 616d 6520   name: The name 
+000022e0: 6f66 2074 6865 2063 6c61 7373 2e0a 2020  of the class..  
+000022f0: 2020 6261 7365 733a 2054 6865 2062 6173    bases: The bas
+00002300: 6520 636c 6173 7365 7320 6f66 2074 6865  e classes of the
+00002310: 2063 6c61 7373 0a20 2020 2062 6f64 793a   class.    body:
+00002320: 2041 206c 6973 7420 6f66 205f 6173 742e   A list of _ast.
+00002330: 7374 6d74 206e 6f64 6573 2074 6861 7420  stmt nodes that 
+00002340: 676f 2069 6e20 7468 6520 626f 6479 206f  go in the body o
+00002350: 6620 7468 6520 636c 6173 732e 0a20 2020  f the class..   
+00002360: 2064 6563 6f72 6174 6f72 5f6c 6973 743a   decorator_list:
+00002370: 2041 206c 6973 7420 6f66 2064 6563 6f72   A list of decor
+00002380: 6174 6f72 206e 6f64 6573 2e0a 0a20 2052  ator nodes...  R
+00002390: 6169 7365 733a 0a20 2020 2056 616c 7565  aises:.    Value
+000023a0: 4572 726f 723a 2049 6620 736f 6d65 2062  Error: If some b
+000023b0: 6f64 7920 656c 656d 656e 7420 6973 206e  ody element is n
+000023c0: 6f74 2061 6e20 5f61 7374 2e73 746d 7420  ot an _ast.stmt 
+000023d0: 6e6f 6465 2e0a 0a20 2052 6574 7572 6e73  node...  Returns
+000023e0: 3a0a 2020 2020 416e 205f 6173 742e 436c  :.    An _ast.Cl
+000023f0: 6173 7344 6566 206e 6f64 652e 0a20 207a  assDef node..  z
+00002400: 1e63 6c61 7373 2062 6f64 7920 6d75 7374  .class body must
+00002410: 2062 6520 6120 6e6f 6e20 656d 7074 794e   be a non emptyN
+00002420: 7a20 4e6f 6e20 4e6f 6e65 206b 7761 7267  z Non None kwarg
+00002430: 7320 6973 206e 6f74 2073 7570 706f 7274  s is not support
+00002440: 6564 7a22 4e6f 6e20 4e6f 6e65 2073 7461  edz"Non None sta
+00002450: 7261 7267 7320 6973 206e 6f74 2073 7570  rargs is not sup
+00002460: 706f 7274 6564 7a14 6261 7365 7320 6d75  portedz.bases mu
+00002470: 7374 2062 6520 6120 6c69 7374 6301 0000  st be a listc...
+00002480: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00002490: 0053 0000 0072 8200 0000 7283 0000 0072  .S...r....r....r
+000024a0: 8400 0000 2902 721d 0000 0072 6900 0000  ....).r....ri...
+000024b0: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000024c0: 1f00 0000 6301 0000 7285 0000 007a 1c43  ....c...r....z.C
+000024d0: 6c61 7373 4465 662e 3c6c 6f63 616c 733e  lassDef.<locals>
+000024e0: 2e3c 6c69 7374 636f 6d70 3e29 05da 046e  .<listcomp>)...n
+000024f0: 616d 65da 0562 6173 6573 7242 0000 0072  ame..basesrB...r
+00002500: 8700 0000 da0e 6465 636f 7261 746f 725f  ......decorator_
+00002510: 6c69 7374 2907 7226 0000 0072 3800 0000  list).r&...r8...
+00002520: 7224 0000 0072 2500 0000 7244 0000 0072  r$...r%...rD...r
+00002530: 2e00 0000 da08 436c 6173 7344 6566 2907  ......ClassDef).
+00002540: 7290 0000 0072 9100 0000 7242 0000 0072  r....r....rB...r
+00002550: 8700 0000 7288 0000 0072 8900 0000 7292  ....r....r....r.
+00002560: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00002570: 0000 7293 0000 004b 0100 0073 2200 0000  ..r....K...s"...
+00002580: 040f 0801 0801 0801 0801 0801 0a01 0801  ................
+00002590: 0801 0e01 0401 0201 0201 0201 0201 0601  ................
+000025a0: 06fb 7293 0000 0063 0000 0000 0000 0000  ..r....c........
+000025b0: 0000 0000 0500 0000 0700 0000 4700 0000  ............G...
+000025c0: 73a8 0000 0074 007c 0083 0164 016b 0072  s....t.|...d.k.r
+000025d0: 0a74 0164 0283 0182 0167 007d 0167 007d  .t.d.....g.}.g.}
+000025e0: 0274 027c 0083 0144 005d 325c 027d 037d  .t.|...D.]2\.}.}
+000025f0: 047c 0364 0316 0064 046b 0272 3674 037c  .|.d...d.k.r6t.|
+00002600: 0474 046a 0583 0273 2674 067c 0483 017d  .t.j...s&t.|...}
+00002610: 0474 037c 0474 046a 0783 0273 3074 0164  .t.|.t.j...s0t.d
+00002620: 0583 0182 017c 01a0 087c 04a1 0101 0071  .....|...|.....q
+00002630: 127c 0364 066b 0372 447c 02a0 0874 097c  .|.d.k.rD|...t.|
+00002640: 0474 0a6a 0b64 078d 02a1 0101 0071 1274  .t.j.d.......q.t
+00002650: 046a 0c74 097c 0064 0619 0074 0a6a 0b64  .j.t.|.d...t.j.d
+00002660: 078d 027c 017c 0264 088d 0353 0029 0961  ...|.|.d...S.).a
+00002670: 0201 0000 4372 6561 7465 7320 616e 205f  ....Creates an _
+00002680: 6173 742e 436f 6d70 6172 6520 6e6f 6465  ast.Compare node
+00002690: 2e0a 0a20 2041 7267 733a 0a20 2020 202a  ...  Args:.    *
+000026a0: 6172 6773 3a20 4c69 7374 2077 6869 6368  args: List which
+000026b0: 2073 686f 756c 6420 616c 7465 726e 6174   should alternat
+000026c0: 6520 6265 7477 6565 6e20 7265 6775 6c61  e between regula
+000026d0: 7220 6e6f 6465 7320 616e 6420 5f61 7374  r nodes and _ast
+000026e0: 2e63 6d70 6f70 2e0a 0a20 2052 6169 7365  .cmpop...  Raise
+000026f0: 733a 0a20 2020 2056 616c 7565 4572 726f  s:.    ValueErro
+00002700: 723a 2049 6620 6c65 7373 2074 6861 6e20  r: If less than 
+00002710: 3320 6172 6773 2c20 6f72 206f 6464 2061  3 args, or odd a
+00002720: 7267 7320 6172 6520 6e6f 7420 7661 6c69  rgs are not vali
+00002730: 6420 636f 6d70 6172 6973 6f6e 0a20 2020  d comparison.   
+00002740: 2020 206f 7065 7261 746f 7273 2e0a 0a20     operators... 
+00002750: 2052 6574 7572 6e73 3a0a 2020 2020 416e   Returns:.    An
+00002760: 205f 6173 742e 436f 6d70 6172 6520 6e6f   _ast.Compare no
+00002770: 6465 2e0a 2020 e903 0000 007a 194d 7573  de..  .....z.Mus
+00002780: 7420 6861 7665 2061 7420 6c65 6173 7420  t have at least 
+00002790: 3320 6172 6773 e902 0000 00e9 0100 0000  3 args..........
+000027a0: 7a28 4f64 6420 6172 6773 206d 7573 7420  z(Odd args must 
+000027b0: 6265 2069 6e73 7461 6e63 6573 206f 6620  be instances of 
+000027c0: 5f61 7374 2e63 6d70 6f70 7201 0000 0072  _ast.cmpopr....r
+000027d0: 3200 0000 2903 726a 0000 00da 036f 7073  2...).rj.....ops
+000027e0: da0b 636f 6d70 6172 6174 6f72 7329 0dda  ..comparators)..
+000027f0: 036c 656e 7226 0000 00da 0965 6e75 6d65  .lenr&.....enume
+00002800: 7261 7465 7224 0000 0072 2e00 0000 722f  rater$...r....r/
+00002810: 0000 00da 0c43 6f6d 7061 7265 4f70 4d61  .....CompareOpMa
+00002820: 70da 0563 6d70 6f70 7227 0000 0072 2200  p..cmpopr'...r".
+00002830: 0000 7266 0000 0072 1500 0000 da07 436f  ..rf...r......Co
+00002840: 6d70 6172 6529 0572 2a00 0000 7297 0000  mpare).r*...r...
+00002850: 0072 9800 0000 da05 696e 6465 7872 1e00  .r......indexr..
+00002860: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00002870: 0072 9d00 0000 6c01 0000 7324 0000 000c  .r....l...s$....
+00002880: 0d08 0104 0104 0110 010c 010c 0108 010c  ................
+00002890: 0108 010c 0108 0214 0102 8014 0102 0102  ................
+000028a0: 0106 fe72 9d00 0000 6303 0000 0000 0000  ...r....c.......
+000028b0: 0000 0000 0004 0000 0006 0000 0047 0000  .............G..
+000028c0: 0073 3200 0000 7400 7c00 7401 6a02 6401  .s2...t.|.t.j.d.
+000028d0: 8d02 7d00 7400 7c01 7401 6a03 6401 8d02  ..}.t.|.t.j.d...
+000028e0: 7d01 7404 6a05 7c00 7c01 7406 7c03 8301  }.t.j.|.|.t.|...
+000028f0: 7c02 6402 8d04 5300 2903 7af6 4372 6561  |.d...S.).z.Crea
+00002900: 7465 2061 6e20 5f61 7374 2e63 6f6d 7072  te an _ast.compr
+00002910: 6568 656e 7369 6f6e 206e 6f64 652c 2075  ehension node, u
+00002920: 7365 6420 696e 205f 6173 742e 4c69 7374  sed in _ast.List
+00002930: 436f 6d70 7265 6865 6e73 696f 6e2e 0a0a  Comprehension...
+00002940: 2020 4172 6773 3a0a 2020 2020 666f 725f    Args:.    for_
+00002950: 7061 7274 3a20 5468 6520 7061 7274 2061  part: The part a
+00002960: 6674 6572 2022 666f 7220 220a 2020 2020  fter "for ".    
+00002970: 696e 5f70 6172 743a 2054 6865 2070 6172  in_part: The par
+00002980: 7420 6166 7465 7220 2266 6f72 205b 666f  t after "for [fo
+00002990: 725f 7061 7274 5d20 696e 2022 0a20 2020  r_part] in ".   
+000029a0: 202a 6966 733a 207b 5f61 7374 2e43 6f6d   *ifs: {_ast.Com
+000029b0: 7061 7265 7d0a 0a20 2052 6574 7572 6e73  pare}..  Returns
+000029c0: 3a0a 2020 2020 7b5f 6173 742e 636f 6d70  :.    {_ast.comp
+000029d0: 7265 6865 6e73 696f 6e7d 0a20 2020 203a  rehension}.    :
+000029e0: 7061 7261 6d20 6973 5f61 7379 6e63 3a0a  param is_async:.
+000029f0: 2020 7232 0000 0029 0472 6d00 0000 da04    r2...).rm.....
+00002a00: 6974 6572 da03 6966 73da 0869 735f 6173  iter..ifs..is_as
+00002a10: 796e 6329 0772 2200 0000 7266 0000 0072  ync).r"...rf...r
+00002a20: 1600 0000 7215 0000 0072 2e00 0000 da0d  ....r....r......
+00002a30: 636f 6d70 7265 6865 6e73 696f 6e72 2500  comprehensionr%.
+00002a40: 0000 2904 da08 666f 725f 7061 7274 da07  ..)...for_part..
+00002a50: 696e 5f70 6172 7472 a100 0000 72a0 0000  in_partr....r...
+00002a60: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00002a70: 72a2 0000 008c 0100 0073 0e00 0000 0e0c  r........s......
+00002a80: 0e01 0601 0201 0601 0201 06fd 72a2 0000  ............r...
+00002a90: 0072 0900 0000 6302 0000 0000 0000 0000  .r....c.........
+00002aa0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+00002ab0: 5000 0000 7400 7c00 8301 7400 7c01 8301  P...t.|...t.|...
+00002ac0: 6b03 7214 7401 6401 a002 7400 7c00 8301  k.r.t.d...t.|...
+00002ad0: 7400 7c01 8301 a102 8301 8201 6402 6403  t.|.........d.d.
+00002ae0: 8400 7c00 4400 8301 7d00 6404 6403 8400  ..|.D...}.d.d...
+00002af0: 7c01 4400 8301 7d01 7403 a004 7c00 7c01  |.D...}.t...|.|.
+00002b00: a102 5300 2905 6131 0100 0043 7265 6174  ..S.).a1...Creat
+00002b10: 6573 2061 6e20 5f61 7374 2e44 6963 7420  es an _ast.Dict 
+00002b20: 6e6f 6465 2e20 5468 6973 2072 6570 7265  node. This repre
+00002b30: 7365 6e74 7320 6120 6469 6374 206c 6974  sents a dict lit
+00002b40: 6572 616c 2e0a 0a20 2041 7267 733a 0a20  eral...  Args:. 
+00002b50: 2020 206b 6579 733a 2041 206c 6973 7420     keys: A list 
+00002b60: 6f66 206b 6579 7320 6173 206e 6f64 6573  of keys as nodes
+00002b70: 2e20 4d75 7374 2062 6520 7468 6520 7361  . Must be the sa
+00002b80: 6d65 206c 656e 6774 6820 6173 2076 616c  me length as val
+00002b90: 7565 732e 0a20 2020 2076 616c 7565 733a  ues..    values:
+00002ba0: 2041 206c 6973 7420 6f66 2076 616c 7565   A list of value
+00002bb0: 7320 6173 206e 6f64 6573 2e20 4d75 7374  s as nodes. Must
+00002bc0: 2062 6520 7468 6520 7361 6d65 206c 656e   be the same len
+00002bd0: 6774 6820 6173 2076 616c 7565 732e 0a0a  gth as values...
+00002be0: 2020 5261 6973 6573 3a0a 2020 2020 5661    Raises:.    Va
+00002bf0: 6c75 6545 7272 6f72 3a20 4966 206c 656e  lueError: If len
+00002c00: 286b 6579 7329 2021 3d20 6c65 6e28 7661  (keys) != len(va
+00002c10: 6c75 6573 292e 0a0a 2020 5265 7475 726e  lues)...  Return
+00002c20: 733a 0a20 2020 2041 6e20 5f61 7374 2e44  s:.    An _ast.D
+00002c30: 6963 7420 6e6f 6465 2e0a 2020 7a1e 6c65  ict node..  z.le
+00002c40: 6e28 6b65 7973 293d 7b7d 2021 3d20 6c65  n(keys)={} != le
+00002c50: 6e28 7661 6c75 6573 293d 7b7d 6301 0000  n(values)={}c...
+00002c60: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00002c70: 0053 0000 0072 1a00 0000 7209 0000 0072  .S...r....r....r
+00002c80: 2100 0000 2902 721d 0000 00da 036b 6579  !...).r......key
+00002c90: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00002ca0: 1f00 0000 b001 0000 7220 0000 007a 1844  ........r ...z.D
+00002cb0: 6963 742e 3c6c 6f63 616c 733e 2e3c 6c69  ict.<locals>.<li
+00002cc0: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
+00002cd0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00002ce0: 721a 0000 0072 0900 0000 7221 0000 0029  r....r....r!...)
+00002cf0: 0272 1d00 0000 723a 0000 0072 0900 0000  .r....r:...r....
+00002d00: 7209 0000 0072 0a00 0000 721f 0000 00b1  r....r....r.....
+00002d10: 0100 0072 2000 0000 2905 7299 0000 0072  ...r ...).r....r
+00002d20: 2600 0000 7241 0000 0072 2e00 0000 da04  &...rA...r......
+00002d30: 4469 6374 2902 da04 6b65 7973 7274 0000  Dict)...keysrt..
+00002d40: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00002d50: 72a6 0000 00a0 0100 0073 0e00 0000 100d  r........s......
+00002d60: 0201 1201 04ff 0e02 0e01 0c01 72a6 0000  ............r...
+00002d70: 0029 0172 a100 0000 6304 0000 0000 0000  .).r....c.......
+00002d80: 0001 0000 0006 0000 0007 0000 0047 0000  .............G..
+00002d90: 0073 5a00 0000 7400 7c00 7401 6a02 6401  .sZ...t.|.t.j.d.
+00002da0: 8d02 7d00 7400 7c01 7401 6a02 6401 8d02  ..}.t.|.t.j.d...
+00002db0: 7d01 7400 7c02 7401 6a03 6401 8d02 7d02  }.t.|.t.j.d...}.
+00002dc0: 7400 7c03 7401 6a02 6401 8d02 7d03 7404  t.|.t.j.d...}.t.
+00002dd0: 6a05 7c00 7c01 7406 7c02 7c03 7c04 6703  j.|.|.t.|.|.|.g.
+00002de0: 7c05 a201 5200 8e00 6701 6402 8d03 5300  |...R...g.d...S.
+00002df0: 2903 61bd 0100 0043 7265 6174 6573 205f  ).a....Creates _
+00002e00: 6173 742e 4469 6374 436f 6d70 206e 6f64  ast.DictComp nod
+00002e10: 6573 2e0a 0a20 2027 6c65 6674 5f73 6964  es...  'left_sid
+00002e20: 6527 2c20 276c 6566 745f 7369 6465 5f76  e', 'left_side_v
+00002e30: 616c 7565 2720 666f 7220 2766 6f72 5f70  alue' for 'for_p
+00002e40: 6172 7427 2069 6e20 2769 6e5f 7061 7274  art' in 'in_part
+00002e50: 2720 6966 2027 6966 7327 0a0a 2020 4172  ' if 'ifs'..  Ar
+00002e60: 6773 3a0a 2020 2020 6c65 6674 5f73 6964  gs:.    left_sid
+00002e70: 655f 6b65 793a 206b 6579 2069 6e20 6c65  e_key: key in le
+00002e80: 6674 6d6f 7374 2073 6964 6520 6f66 2074  ftmost side of t
+00002e90: 6865 2065 7870 7265 7373 696f 6e2e 0a20  he expression.. 
+00002ea0: 2020 206c 6566 745f 7369 6465 5f76 616c     left_side_val
+00002eb0: 7565 3a20 7661 6c75 6520 696e 206c 6566  ue: value in lef
+00002ec0: 746d 6f73 7420 7369 6465 206f 6620 7468  tmost side of th
+00002ed0: 6520 6578 7072 6573 7369 6f6e 2e0a 2020  e expression..  
+00002ee0: 2020 666f 725f 7061 7274 3a20 5468 6520    for_part: The 
+00002ef0: 7061 7274 2061 6674 6572 2027 5b6c 6566  part after '[lef
+00002f00: 745f 7369 6465 5d20 666f 7220 270a 2020  t_side] for '.  
+00002f10: 2020 696e 5f70 6172 743a 2054 6865 2070    in_part: The p
+00002f20: 6172 7420 6166 7465 7220 275b 6c65 6674  art after '[left
+00002f30: 5f73 6964 655d 2066 6f72 205b 666f 725f  _side] for [for_
+00002f40: 7061 7274 5d20 696e 2027 0a20 2020 202a  part] in '.    *
+00002f50: 6966 733a 2041 6e79 2069 6620 7374 6174  ifs: Any if stat
+00002f60: 656d 656e 7473 2074 6861 7420 636f 6d65  ements that come
+00002f70: 2061 7420 7468 6520 656e 642e 0a0a 2020   at the end...  
+00002f80: 5265 7475 726e 733a 0a20 2020 207b 5f61  Returns:.    {_a
+00002f90: 7374 2e44 6963 7443 6f6d 707d 0a20 2020  st.DictComp}.   
+00002fa0: 203a 7061 7261 6d20 6973 5f61 7379 6e63   :param is_async
+00002fb0: 3a0a 2020 7232 0000 0029 0372 a500 0000  :.  r2...).r....
+00002fc0: 723a 0000 00da 0a67 656e 6572 6174 6f72  r:.....generator
+00002fd0: 7329 0772 2200 0000 7266 0000 0072 1500  s).r"...rf...r..
+00002fe0: 0000 7216 0000 0072 2e00 0000 da08 4469  ..r....r......Di
+00002ff0: 6374 436f 6d70 72a2 0000 0029 06da 0d6c  ctCompr....)...l
+00003000: 6566 745f 7369 6465 5f6b 6579 da0f 6c65  eft_side_key..le
+00003010: 6674 5f73 6964 655f 7661 6c75 6572 a300  ft_side_valuer..
+00003020: 0000 72a4 0000 0072 a100 0000 72a0 0000  ..r....r....r...
+00003030: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00003040: 72a9 0000 00b5 0100 0073 1200 0000 0e10  r........s......
+00003050: 0e01 0e01 0e01 0401 0201 0201 1401 06fd  ................
+00003060: 72a9 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00003070: 0000 0000 0000 0200 0000 4300 0000 725b  ..........C...r[
+00003080: 0000 0072 2d00 0000 2902 722e 0000 00da  ...r-...).r.....
+00003090: 0344 6976 7209 0000 0072 0900 0000 7209  .Divr....r....r.
+000030a0: 0000 0072 0a00 0000 72ac 0000 00cf 0100  ...r....r.......
+000030b0: 0072 5d00 0000 72ac 0000 0063 0000 0000  .r]...r....c....
+000030c0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+000030d0: 4300 0000 725b 0000 0072 2d00 0000 2902  C...r[...r-...).
+000030e0: 722e 0000 00da 0245 7172 0900 0000 7209  r......Eqr....r.
+000030f0: 0000 0072 0900 0000 720a 0000 0072 ad00  ...r....r....r..
+00003100: 0000 d301 0000 725d 0000 0072 ad00 0000  ......r]...r....
+00003110: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00003120: 0005 0000 0043 0000 0073 1800 0000 7400  .....C...s....t.
+00003130: 7c02 8301 7d02 7401 6a02 7c00 7c01 7c02  |...}.t.j.|.|.|.
+00003140: 6401 8d03 5300 2902 4e29 0372 0e00 0000  d...S.).N).r....
+00003150: 7290 0000 0072 4200 0000 2903 7244 0000  r....rB...).rD..
+00003160: 0072 2e00 0000 da0d 4578 6365 7074 4861  .r......ExceptHa
+00003170: 6e64 6c65 7229 03da 0e65 7863 6570 7469  ndler)...excepti
+00003180: 6f6e 5f74 7970 6572 9000 0000 7242 0000  on_typer....rB..
+00003190: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+000031a0: 72ae 0000 00d7 0100 0073 0400 0000 0801  r........s......
+000031b0: 1001 72ae 0000 0063 0100 0000 0000 0000  ..r....c........
+000031c0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
+000031d0: 7324 0000 0074 007c 0074 016a 0283 0272  s$...t.|.t.j...r
+000031e0: 0d74 0364 01a0 047c 00a1 0183 0182 0174  .t.d...|.......t
+000031f0: 01a0 057c 00a1 0153 0029 0261 1501 0000  ...|...S.).a....
+00003200: 4372 6561 7465 7320 616e 205f 6173 742e  Creates an _ast.
+00003210: 4578 7072 206e 6f64 652e 0a0a 2020 4e6f  Expr node...  No
+00003220: 7465 2074 6861 7420 7468 6973 206e 6f64  te that this nod
+00003230: 6520 6973 206d 6f73 746c 7920 7573 6564  e is mostly used
+00003240: 2074 6f20 7772 6170 206f 7468 6572 206e   to wrap other n
+00003250: 6f64 6573 2073 6f20 7468 6579 2772 6520  odes so they're 
+00003260: 7472 6561 7465 640a 2020 6173 2077 686f  treated.  as who
+00003270: 6c65 2d6c 696e 6520 7374 6174 656d 656e  le-line statemen
+00003280: 7473 2e0a 0a20 2041 7267 733a 0a20 2020  ts...  Args:.   
+00003290: 2076 616c 7565 3a20 5468 6520 7661 6c75   value: The valu
+000032a0: 6520 7374 6f72 6564 2069 6e20 7468 6520  e stored in the 
+000032b0: 6e6f 6465 2e0a 0a20 2052 6169 7365 733a  node...  Raises:
+000032c0: 0a20 2020 2056 616c 7565 4572 726f 723a  .    ValueError:
+000032d0: 2049 6620 7661 6c75 6520 6973 2061 6e20   If value is an 
+000032e0: 5f61 7374 2e73 746d 7420 6e6f 6465 2e0a  _ast.stmt node..
+000032f0: 0a20 2052 6574 7572 6e73 3a0a 2020 2020  .  Returns:.    
+00003300: 416e 205f 6173 742e 4578 7072 206e 6f64  An _ast.Expr nod
+00003310: 652e 0a20 207a 7376 616c 7565 206d 7573  e..  zsvalue mus
+00003320: 7420 6e6f 7420 6265 2061 6e20 5f61 7374  t not be an _ast
+00003330: 2e73 746d 7420 6e6f 6465 2c20 6265 6361  .stmt node, beca
+00003340: 7573 6520 7468 6f73 6520 6e6f 6465 7320  use those nodes 
+00003350: 646f 6e27 7420 6e65 6564 2074 6f20 6265  don't need to be
+00003360: 2077 7261 7070 6564 2069 6e20 616e 2045   wrapped in an E
+00003370: 7870 7220 6e6f 6465 2e20 5661 6c75 6520  xpr node. Value 
+00003380: 7061 7373 6564 3a20 7b7d 2906 7224 0000  passed: {}).r$..
+00003390: 0072 2e00 0000 7240 0000 0072 2600 0000  .r....r@...r&...
+000033a0: 7241 0000 00da 0445 7870 72a9 0172 3a00  rA.....Expr..r:.
+000033b0: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+000033c0: 0072 b000 0000 dc01 0000 730c 0000 000c  .r........s.....
+000033d0: 0f02 0102 0106 0104 fe0a 0372 b000 0000  ...........r....
+000033e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000033f0: 0002 0000 0043 0000 0072 5b00 0000 722d  .....C...r[...r-
+00003400: 0000 0029 0272 2e00 0000 da08 466c 6f6f  ...).r......Floo
+00003410: 7244 6976 7209 0000 0072 0900 0000 7209  rDivr....r....r.
+00003420: 0000 0072 0a00 0000 72b2 0000 00f2 0100  ...r....r.......
+00003430: 0072 5d00 0000 72b2 0000 0063 0600 0000  .r]...r....c....
+00003440: 0000 0000 0000 0000 0600 0000 0800 0000  ................
+00003450: 4300 0000 734a 0000 007c 0172 0c74 007c  C...sJ...|.r.t.|
+00003460: 0174 016a 0283 0273 0c74 0364 0183 0182  .t.j...s.t.d....
+00003470: 017c 0173 1274 0283 007d 016e 027c 017d  .|.s.t...}.n.|.}
+00003480: 0174 047c 0283 017d 0274 056a 067c 007c  .t.|...}.t.j.|.|
+00003490: 017c 027c 047c 0574 077c 0383 0164 028d  .|.|.|.t.|...d..
+000034a0: 0653 0029 0361 2802 0000 4372 6561 7465  .S.).a(...Create
+000034b0: 7320 616e 205f 6173 742e 4675 6e63 7469  s an _ast.Functi
+000034c0: 6f6e 4465 6620 6e6f 6465 2e0a 0a20 2041  onDef node...  A
+000034d0: 7267 733a 0a20 2020 206e 616d 653a 2054  rgs:.    name: T
+000034e0: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
+000034f0: 756e 6374 696f 6e2e 0a20 2020 2061 7267  unction..    arg
+00003500: 733a 2041 206c 6973 7420 6f66 2061 7267  s: A list of arg
+00003510: 732e 0a20 2020 206b 6579 733a 2041 206c  s..    keys: A l
+00003520: 6973 7420 6f66 206b 6579 732c 206d 7573  ist of keys, mus
+00003530: 7420 6265 2074 6865 2073 616d 6520 6c65  t be the same le
+00003540: 6e67 7468 2061 7320 7661 6c75 6573 2e0a  ngth as values..
+00003550: 2020 2020 7661 6c75 6573 3a20 4120 6c69      values: A li
+00003560: 7374 206f 6620 7661 6c75 6573 2c20 636f  st of values, co
+00003570: 7272 6573 706f 6e64 2074 6f20 6b65 7973  rrespond to keys
+00003580: 2e0a 2020 2020 626f 6479 3a20 4120 6c69  ..    body: A li
+00003590: 7374 206f 6620 5f61 7374 2e73 746d 7420  st of _ast.stmt 
+000035a0: 6e6f 6465 7320 7468 6174 2067 6f20 696e  nodes that go in
+000035b0: 2074 6865 2062 6f64 7920 6f66 2074 6865   the body of the
+000035c0: 2066 756e 6374 696f 6e2e 0a20 2020 2076   function..    v
+000035d0: 6172 6172 675f 6e61 6d65 3a20 5468 6520  ararg_name: The 
+000035e0: 6e61 6d65 206f 6620 7468 6520 7661 7261  name of the vara
+000035f0: 7267 2076 6172 6961 626c 652c 206f 7220  rg variable, or 
+00003600: 4e6f 6e65 2e0a 2020 2020 6b77 6172 675f  None..    kwarg_
+00003610: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
+00003620: 6620 7468 6520 6b77 6172 6773 2076 6172  f the kwargs var
+00003630: 6961 626c 652c 206f 7220 4e6f 6e65 2e0a  iable, or None..
+00003640: 2020 2020 6465 636f 7261 746f 725f 6c69      decorator_li
+00003650: 7374 3a20 4120 6c69 7374 206f 6620 6465  st: A list of de
+00003660: 636f 7261 746f 7220 6e6f 6465 732e 0a20  corator nodes.. 
+00003670: 2052 6169 7365 733a 0a20 2020 2056 616c   Raises:.    Val
+00003680: 7565 4572 726f 723a 2049 6620 6c65 6e28  ueError: If len(
+00003690: 6b65 7973 2920 213d 206c 656e 2876 616c  keys) != len(val
+000036a0: 7565 7329 2e0a 0a20 2052 6574 7572 6e73  ues)...  Returns
+000036b0: 3a0a 2020 2020 416e 205f 6173 742e 4675  :.    An _ast.Fu
+000036c0: 6e63 7469 6f6e 4465 6620 6e6f 6465 2e0a  nctionDef node..
+000036d0: 2020 7219 0000 0029 0672 9000 0000 722a    r....).r....r*
+000036e0: 0000 0072 4200 0000 da07 7265 7475 726e  ...rB.....return
+000036f0: 73da 0c74 7970 655f 636f 6d6d 656e 7472  s..type_commentr
+00003700: 9200 0000 2908 7224 0000 00da 0361 7374  ....).r$.....ast
+00003710: 725a 0000 0072 2600 0000 7244 0000 0072  rZ...r&...rD...r
+00003720: 2e00 0000 da0b 4675 6e63 7469 6f6e 4465  ......FunctionDe
+00003730: 6672 2500 0000 2906 7290 0000 0072 2a00  fr%...).r....r*.
+00003740: 0000 7242 0000 0072 9200 0000 72b3 0000  ..rB...r....r...
+00003750: 0072 b400 0000 7209 0000 0072 0900 0000  .r....r....r....
+00003760: 720a 0000 0072 b600 0000 f601 0000 731c  r....r........s.
+00003770: 0000 0010 1308 0104 0108 0104 0208 0104  ................
+00003780: 0102 0102 0102 0102 0102 0106 0106 fa72  ...............r
+00003790: b600 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000037a0: 0005 0000 0006 0000 0047 0000 0073 4e00  .........G...sN.
+000037b0: 0000 7400 7c00 7401 6a02 6401 8d02 7d00  ..t.|.t.j.d...}.
+000037c0: 7400 7c01 7401 6a03 6401 8d02 7d01 7400  t.|.t.j.d...}.t.
+000037d0: 7c02 7401 6a02 6401 8d02 7d02 7404 6a05  |.t.j.d...}.t.j.
+000037e0: 7c00 7406 7c01 7c02 6402 6703 7c03 a201  |.t.|.|.d.g.|...
+000037f0: 5200 8e00 6701 6403 8d02 7d04 7c04 5300  R...g.d...}.|.S.
+00003800: 2904 6153 0100 0043 7265 6174 6573 205f  ).aS...Creates _
+00003810: 6173 742e 4765 6e65 7261 746f 7245 7870  ast.GeneratorExp
+00003820: 206e 6f64 6573 2e0a 0a20 2027 6c65 6674   nodes...  'left
+00003830: 5f73 6964 6527 2066 6f72 2027 666f 725f  _side' for 'for_
+00003840: 7061 7274 2720 696e 2027 696e 5f70 6172  part' in 'in_par
+00003850: 7427 2069 6620 2769 6673 270a 0a20 2041  t' if 'ifs'..  A
+00003860: 7267 733a 0a20 2020 206c 6566 745f 7369  rgs:.    left_si
+00003870: 6465 3a20 6c65 6674 6d6f 7374 2073 6964  de: leftmost sid
+00003880: 6520 6f66 2074 6865 2065 7870 7265 7373  e of the express
+00003890: 696f 6e2e 0a20 2020 2066 6f72 5f70 6172  ion..    for_par
+000038a0: 743a 2054 6865 2070 6172 7420 6166 7465  t: The part afte
+000038b0: 7220 275b 6c65 6674 5f73 6964 655d 2066  r '[left_side] f
+000038c0: 6f72 2027 0a20 2020 2069 6e5f 7061 7274  or '.    in_part
+000038d0: 3a20 5468 6520 7061 7274 2061 6674 6572  : The part after
+000038e0: 2027 5b6c 6566 745f 7369 6465 5d20 666f   '[left_side] fo
+000038f0: 7220 5b66 6f72 5f70 6172 745d 2069 6e20  r [for_part] in 
+00003900: 270a 2020 2020 2a69 6673 3a20 416e 7920  '.    *ifs: Any 
+00003910: 6966 2073 7461 7465 6d65 6e74 7320 7468  if statements th
+00003920: 6174 2063 6f6d 6520 6174 2074 6865 2065  at come at the e
+00003930: 6e64 2e0a 0a20 2052 6574 7572 6e73 3a0a  nd...  Returns:.
+00003940: 2020 2020 7b5f 6173 742e 4765 6e65 7261      {_ast.Genera
+00003950: 746f 7245 7870 7d0a 2020 7232 0000 0072  torExp}.  r2...r
+00003960: 0100 0000 a902 da03 656c 7472 a800 0000  ........eltr....
+00003970: 2907 7222 0000 0072 6600 0000 7215 0000  ).r"...rf...r...
+00003980: 0072 1600 0000 722e 0000 00da 0c47 656e  .r....r......Gen
+00003990: 6572 6174 6f72 4578 7072 a200 0000 2905  eratorExpr....).
+000039a0: da09 6c65 6674 5f73 6964 6572 a300 0000  ..left_sider....
+000039b0: 72a4 0000 0072 a000 0000 726e 0000 0072  r....r....rn...r
+000039c0: 0900 0000 7209 0000 0072 0a00 0000 72b9  ....r....r....r.
+000039d0: 0000 0019 0200 0073 1000 0000 0e0e 0e01  .......s........
+000039e0: 0e01 0401 0201 1401 06fe 0403 72b9 0000  ............r...
+000039f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003a00: 0000 0200 0000 4300 0000 725b 0000 0072  ......C...r[...r
+00003a10: 2d00 0000 2902 722e 0000 00da 0247 7472  -...).r......Gtr
+00003a20: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00003a30: 0000 0072 bb00 0000 3002 0000 725d 0000  ...r....0...r]..
+00003a40: 0072 bb00 0000 6300 0000 0000 0000 0000  .r....c.........
+00003a50: 0000 0000 0000 0002 0000 0043 0000 0072  ...........C...r
+00003a60: 5b00 0000 722d 0000 0029 0272 2e00 0000  [...r-...).r....
+00003a70: da03 4774 4572 0900 0000 7209 0000 0072  ..GtEr....r....r
+00003a80: 0900 0000 720a 0000 0072 bc00 0000 3402  ....r....r....4.
+00003a90: 0000 725d 0000 0072 bc00 0000 6303 0000  ..r]...r....c...
+00003aa0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00003ab0: 0043 0000 0073 5600 0000 7400 7c01 8301  .C...sV...t.|...
+00003ac0: 7d01 7c02 6401 7500 720a 6700 7d02 7401  }.|.d.u.r.g.}.t.
+00003ad0: 7c02 7402 7403 6602 8302 7223 7c01 4400  |.t.t.f...r#|.D.
+00003ae0: 5d0f 7d03 7401 7c03 7404 6a05 8302 7322  ].}.t.|.t.j...s"
+00003af0: 7406 6402 a007 7c03 a101 8301 8201 7113  t.d...|.......q.
+00003b00: 7404 6a08 7c00 7c01 7c02 6403 8d03 5300  t.j.|.|.|.d...S.
+00003b10: 2904 615b 0200 0043 7265 6174 6573 2061  ).a[...Creates a
+00003b20: 6e20 5f61 7374 2e49 6620 6e6f 6465 2e0a  n _ast.If node..
+00003b30: 0a20 2041 7267 733a 0a20 2020 2063 6f6e  .  Args:.    con
+00003b40: 6469 7469 6f6e 616c 3a20 5468 6520 6578  ditional: The ex
+00003b50: 7072 6573 7369 6f6e 2077 6520 6576 616c  pression we eval
+00003b60: 7561 7465 2066 6f72 2069 7473 2074 7275  uate for its tru
+00003b70: 7468 696e 6573 732e 0a20 2020 2062 6f64  thiness..    bod
+00003b80: 793a 2054 6865 206c 6973 7420 6f66 206e  y: The list of n
+00003b90: 6f64 6573 2074 6861 7420 6d61 6b65 2075  odes that make u
+00003ba0: 7020 7468 6520 626f 6479 206f 6620 7468  p the body of th
+00003bb0: 6520 6966 2073 7461 7465 6d65 6e74 2e0a  e if statement..
+00003bc0: 2020 2020 2020 4578 6563 7574 6564 2069        Executed i
+00003bd0: 6620 5472 7565 2e0a 2020 2020 6f72 656c  f True..    orel
+00003be0: 7365 3a20 7b5b 5f61 7374 2e49 665d 7c5b  se: {[_ast.If]|[
+00003bf0: 5f61 7374 2e73 746d 745d 7c4e 6f6e 657d  _ast.stmt]|None}
+00003c00: 2045 6974 6865 7220 616e 6f74 6865 7220   Either another 
+00003c10: 4966 2073 7461 7465 6d65 6e74 2061 7320  If statement as 
+00003c20: 7468 650a 2020 2020 2020 6f6e 6c79 2065  the.      only e
+00003c30: 6c65 6d65 6e74 2069 6e20 6120 6c69 7374  lement in a list
+00003c40: 2c20 2869 6e20 7768 6963 6820 6361 7365  , (in which case
+00003c50: 2074 6869 7320 6265 636f 6d65 7320 616e   this becomes an
+00003c60: 2065 6c69 6629 2c20 6120 6c69 7374 206f   elif), a list o
+00003c70: 660a 2020 2020 2020 7374 6d74 206e 6f64  f.      stmt nod
+00003c80: 6573 2028 696e 2077 6869 6368 2063 6173  es (in which cas
+00003c90: 6520 7468 6973 2069 7320 616e 2065 6c73  e this is an els
+00003ca0: 6529 2c20 6f72 204e 6f6e 6520 2869 6e20  e), or None (in 
+00003cb0: 7768 6963 6820 6361 7365 2c20 7468 6572  which case, ther
+00003cc0: 650a 2020 2020 2020 6973 206f 6e6c 7920  e.      is only 
+00003cd0: 7468 6520 6966 290a 0a20 2052 6169 7365  the if)..  Raise
+00003ce0: 733a 0a20 2020 2056 616c 7565 4572 726f  s:.    ValueErro
+00003cf0: 723a 2049 6620 7468 6520 626f 6479 206f  r: If the body o
+00003d00: 7220 6f72 656c 7365 2061 7265 206c 6973  r orelse are lis
+00003d10: 7473 2077 6869 6368 2063 6f6e 7461 696e  ts which contain
+00003d20: 2065 6c65 6d65 6e74 7320 6e6f 740a 2020   elements not.  
+00003d30: 2020 2020 696e 6865 7269 7469 6e67 2066      inheriting f
+00003d40: 726f 6d20 5f61 7374 2e73 746d 742e 0a0a  rom _ast.stmt...
+00003d50: 2020 5265 7475 726e 733a 0a20 2020 2041    Returns:.    A
+00003d60: 6e20 5f61 7374 2e49 6620 6e6f 6465 2e0a  n _ast.If node..
+00003d70: 2020 4e72 3e00 0000 2903 725f 0000 0072    Nr>...).r_...r
+00003d80: 4200 0000 da06 6f72 656c 7365 2909 7244  B.....orelse).rD
+00003d90: 0000 0072 2400 0000 7225 0000 0072 6500  ...r$...r%...re.
+00003da0: 0000 722e 0000 0072 4000 0000 7226 0000  ..r....r@...r&..
+00003db0: 0072 4100 0000 da02 4966 2904 da0b 636f  .rA.....If)...co
+00003dc0: 6e64 6974 696f 6e61 6c72 4200 0000 72bd  nditionalrB...r.
+00003dd0: 0000 0072 4300 0000 7209 0000 0072 0900  ...rC...r....r..
+00003de0: 0000 720a 0000 0072 be00 0000 3802 0000  ..r....r....8...
+00003df0: 7318 0000 0008 1308 0104 010e 0108 010c  s...............
+00003e00: 0102 0102 0106 0204 fd02 ff10 0572 be00  .............r..
+00003e10: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00003e20: 0000 0005 0000 0043 0000 0073 1000 0000  .......C...s....
+00003e30: 7400 6a01 7c01 7c00 7c02 6401 8d03 5300  t.j.|.|.|.d...S.
+00003e40: 2902 6142 0100 0043 7265 6174 6573 2061  ).aB...Creates a
+00003e50: 6e20 5f61 7374 2e49 6645 7870 206e 6f64  n _ast.IfExp nod
+00003e60: 652e 0a0a 2020 4e6f 7465 2074 6861 7420  e...  Note that 
+00003e70: 7468 6973 2069 7320 7079 7468 6f6e 2773  this is python's
+00003e80: 2074 6572 6e61 7279 206f 7065 7261 746f   ternary operato
+00003e90: 722c 206e 6f74 2074 6f20 6265 2063 6f6e  r, not to be con
+00003ea0: 6675 7365 6420 7769 7468 205f 6173 742e  fused with _ast.
+00003eb0: 4966 2e0a 0a20 2041 7267 733a 0a20 2020  If...  Args:.   
+00003ec0: 2063 6f6e 6469 7469 6f6e 616c 3a20 5468   conditional: Th
+00003ed0: 6520 6578 7072 6573 7369 6f6e 2077 6520  e expression we 
+00003ee0: 6576 616c 7561 7465 2066 6f72 2069 7473  evaluate for its
+00003ef0: 2074 7275 7468 696e 6573 732e 0a20 2020   truthiness..   
+00003f00: 2074 7275 655f 6361 7365 3a20 5768 6174   true_case: What
+00003f10: 2074 6f20 646f 2069 6620 636f 6e64 6974   to do if condit
+00003f20: 696f 6e61 6c20 6973 2054 7275 652e 0a20  ional is True.. 
+00003f30: 2020 2066 616c 7365 5f63 6173 653a 2057     false_case: W
+00003f40: 6861 7420 746f 2064 6f20 6966 2063 6f6e  hat to do if con
+00003f50: 6469 7469 6f6e 616c 2069 7320 4661 6c73  ditional is Fals
+00003f60: 652e 0a0a 2020 5265 7475 726e 733a 0a20  e...  Returns:. 
+00003f70: 2020 2041 6e20 5f61 7374 2e49 6645 7870     An _ast.IfExp
+00003f80: 206e 6f64 652e 0a20 2029 0372 4200 0000   node..  ).rB...
+00003f90: 725f 0000 0072 bd00 0000 2902 722e 0000  r_...r....).r...
+00003fa0: 00da 0549 6645 7870 2903 72bf 0000 00da  ...IfExp).r.....
+00003fb0: 0974 7275 655f 6361 7365 da0a 6661 6c73  .true_case..fals
+00003fc0: 655f 6361 7365 7209 0000 0072 0900 0000  e_caser....r....
+00003fd0: 720a 0000 0072 c000 0000 5802 0000 7302  r....r....X...s.
+00003fe0: 0000 0010 0d72 c000 0000 da00 6303 0000  .....r......c...
+00003ff0: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00004000: 0043 0000 0073 3000 0000 7400 6a01 7c00  .C...s0...t.j.|.
+00004010: 7c02 6401 8d02 6701 7d03 7c01 7212 7400  |.d...g.}.|.r.t.
+00004020: 6a02 6402 7c01 7c03 6403 8d03 5300 7400  j.d.|.|.d...S.t.
+00004030: 6a03 7c03 6404 8d01 5300 2905 6163 0100  j.|.d...S.).ac..
+00004040: 0043 7265 6174 6573 2065 6974 6865 7220  .Creates either 
+00004050: 616e 205f 6173 742e 496d 706f 7274 206e  an _ast.Import n
+00004060: 6f64 6520 6f72 2061 6e20 5f61 7374 2e49  ode or an _ast.I
+00004070: 6d70 6f72 7446 726f 6d20 6e6f 6465 2e0a  mportFrom node..
+00004080: 0a20 2041 7267 733a 0a20 2020 2069 6d70  .  Args:.    imp
+00004090: 6f72 745f 7061 7274 3a20 5468 6520 7465  ort_part: The te
+000040a0: 7874 2074 6861 7420 666f 6c6c 6f77 7320  xt that follows 
+000040b0: 2269 6d70 6f72 7422 2e0a 2020 2020 6672  "import"..    fr
+000040c0: 6f6d 5f70 6172 743a 2054 6865 2074 6578  om_part: The tex
+000040d0: 7420 7468 6174 2066 6f6c 6c6f 7773 2022  t that follows "
+000040e0: 6672 6f6d 222e 204f 7074 696f 6e61 6c2e  from". Optional.
+000040f0: 2044 6574 6572 6d69 6e65 7320 6966 2077   Determines if w
+00004100: 6520 7769 6c6c 0a20 2020 2020 2072 6574  e will.      ret
+00004110: 7572 6e20 616e 205f 6173 742e 496d 706f  urn an _ast.Impo
+00004120: 7274 206f 7220 5f61 7374 2e49 6d70 6f72  rt or _ast.Impor
+00004130: 7446 726f 6d20 6e6f 6465 2e0a 2020 2020  tFrom node..    
+00004140: 6173 6e61 6d65 3a20 5465 7874 2074 6861  asname: Text tha
+00004150: 7420 666f 6c6c 6f77 7320 2261 7322 2e20  t follows "as". 
+00004160: 4f70 7469 6f6e 616c 2e0a 0a20 2052 6574  Optional...  Ret
+00004170: 7572 6e73 3a0a 2020 2020 416e 205f 6173  urns:.    An _as
+00004180: 742e 496d 706f 7274 206f 7220 5f61 7374  t.Import or _ast
+00004190: 2e49 6d70 6f72 7446 726f 6d20 6e6f 6465  .ImportFrom node
+000041a0: 2e0a 2020 2902 7290 0000 00da 0661 736e  ..  ).r......asn
+000041b0: 616d 6572 0100 0000 2903 da05 6c65 7665  amer....)...leve
+000041c0: 6cda 066d 6f64 756c 65da 056e 616d 6573  l..module..names
+000041d0: 2901 72c7 0000 0029 0472 2e00 0000 da05  ).r....).r......
+000041e0: 616c 6961 73da 0a49 6d70 6f72 7446 726f  alias..ImportFro
+000041f0: 6dda 0649 6d70 6f72 7429 04da 0b69 6d70  m..Import)...imp
+00004200: 6f72 745f 7061 7274 da09 6672 6f6d 5f70  ort_part..from_p
+00004210: 6172 7472 c400 0000 72c7 0000 0072 0900  artr....r....r..
+00004220: 0000 7209 0000 0072 0a00 0000 72ca 0000  ..r....r....r...
+00004230: 0068 0200 0073 1400 0000 060c 0201 08ff  .h...s..........
+00004240: 0402 0401 0201 0201 0201 06fd 0c05 72ca  ..............r.
+00004250: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00004260: 0000 0000 0200 0000 4300 0000 725b 0000  ........C...r[..
+00004270: 0072 2d00 0000 2902 722e 0000 00da 0249  .r-...).r......I
+00004280: 6e72 0900 0000 7209 0000 0072 0900 0000  nr....r....r....
+00004290: 720a 0000 0072 cd00 0000 7f02 0000 725d  r....r........r]
+000042a0: 0000 0072 cd00 0000 6301 0000 0000 0000  ...r....c.......
+000042b0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000042c0: 00f3 0a00 0000 7400 a001 7c00 a101 5300  ......t...|...S.
+000042d0: 722d 0000 0029 0272 2e00 0000 da05 496e  r-...).r......In
+000042e0: 6465 7872 b100 0000 7209 0000 0072 0900  dexr....r....r..
+000042f0: 0000 720a 0000 0072 cf00 0000 8302 0000  ..r....r........
+00004300: f302 0000 000a 0172 cf00 0000 6300 0000  .......r....c...
+00004310: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00004320: 0043 0000 0072 5b00 0000 722d 0000 0029  .C...r[...r-...)
+00004330: 0272 2e00 0000 da06 496e 7665 7274 7209  .r......Invertr.
+00004340: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00004350: 0000 72d1 0000 0087 0200 0072 5d00 0000  ..r........r]...
+00004360: 72d1 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00004370: 0000 0000 0000 0200 0000 4300 0000 725b  ..........C...r[
+00004380: 0000 0072 2d00 0000 2902 722e 0000 00da  ...r-...).r.....
+00004390: 0249 7372 0900 0000 7209 0000 0072 0900  .Isr....r....r..
+000043a0: 0000 720a 0000 0072 d200 0000 8b02 0000  ..r....r........
+000043b0: 725d 0000 0072 d200 0000 6300 0000 0000  r]...r....c.....
+000043c0: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+000043d0: 0000 0072 5b00 0000 722d 0000 0029 0272  ...r[...r-...).r
+000043e0: 2e00 0000 da05 4973 4e6f 7472 0900 0000  ......IsNotr....
+000043f0: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00004400: d300 0000 8f02 0000 725d 0000 0072 d300  ........r]...r..
+00004410: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00004420: 0000 0004 0000 0043 0000 0073 2e00 0000  .......C...s....
+00004430: 7400 7c00 7401 7402 6602 8302 720b 7403  t.|.t.t.f...r.t.
+00004440: 6401 8301 8201 7404 7c01 6402 8d01 7d02  d.....t.|.d...}.
+00004450: 7405 6a06 7c02 7c00 6403 8d02 5300 2904  t.j.|.|.d...S.).
+00004460: 7aaf 4372 6561 7465 7320 616e 205f 6173  z.Creates an _as
+00004470: 742e 4c61 6d62 6461 206f 626a 6563 742e  t.Lambda object.
+00004480: 0a0a 2020 4172 6773 3a0a 2020 2020 626f  ..  Args:.    bo
+00004490: 6479 3a20 7b5f 6173 742e 4153 547d 0a20  dy: {_ast.AST}. 
+000044a0: 2020 2061 7267 733a 207b 5f61 7374 2e61     args: {_ast.a
+000044b0: 7267 756d 656e 7473 7d0a 0a20 2052 6169  rguments}..  Rai
+000044c0: 7365 733a 0a20 2020 2056 616c 7565 4572  ses:.    ValueEr
+000044d0: 726f 723a 2049 6620 626f 6479 2069 7320  ror: If body is 
+000044e0: 6120 6c69 7374 206f 7220 7475 706c 652e  a list or tuple.
+000044f0: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
+00004500: 207b 5f61 7374 2e4c 616d 6264 617d 0a20   {_ast.Lambda}. 
+00004510: 207a 3442 6f64 7920 7368 6f75 6c64 2062   z4Body should b
+00004520: 6520 6120 7369 6e67 6c65 2065 6c65 6d65  e a single eleme
+00004530: 6e74 2c20 6e6f 7420 6120 6c69 7374 206f  nt, not a list o
+00004540: 7220 7475 706c 6529 0172 2a00 0000 2902  r tuple).r*...).
+00004550: 722a 0000 0072 4200 0000 2907 7224 0000  r*...rB...).r$..
+00004560: 0072 2500 0000 7265 0000 0072 2600 0000  .r%...re...r&...
+00004570: 725a 0000 0072 2e00 0000 da06 4c61 6d62  rZ...r......Lamb
+00004580: 6461 2903 7242 0000 0072 2a00 0000 da0b  da).rB...r*.....
+00004590: 6c61 6d62 6461 5f61 7267 7372 0900 0000  lambda_argsr....
+000045a0: 7209 0000 0072 0a00 0000 72d4 0000 0093  r....r....r.....
+000045b0: 0200 0073 0800 0000 0e0d 0801 0a03 0e01  ...s............
+000045c0: 72d4 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000045d0: 0000 0600 0000 0400 0000 4f00 0000 7368  ..........O...sh
+000045e0: 0000 007c 01a0 0064 0174 016a 02a1 027d  ...|...d.t.j...}
+000045f0: 027c 0044 005d 1d7d 0374 037c 0374 046a  .|.D.].}.t.|.t.j
+00004600: 0583 0272 1774 067c 0283 017c 035f 0771  ...r.t.|...|._.q
+00004610: 0974 037c 0374 046a 0883 0272 2674 097c  .t.|.t.j...r&t.|
+00004620: 0383 017d 0474 067c 0283 017c 045f 0771  ...}.t.|...|._.q
+00004630: 0974 067c 0283 017d 0574 046a 0a74 0b7c  .t.|...}.t.j.t.|
+00004640: 0083 017c 0564 028d 0253 0029 0361 0501  ...|.d...S.).a..
+00004650: 0000 4372 6561 7465 7320 616e 205f 6173  ..Creates an _as
+00004660: 742e 4c69 7374 206e 6f64 652e 0a0a 2020  t.List node...  
+00004670: 4175 746f 6d61 7469 6361 6c6c 7920 6164  Automatically ad
+00004680: 6a75 7374 7320 696e 6e65 7220 6374 7820  justs inner ctx 
+00004690: 6174 7472 732e 0a0a 2020 4172 6773 3a0a  attrs...  Args:.
+000046a0: 2020 2020 2a69 7465 6d73 3a20 5468 6520      *items: The 
+000046b0: 6974 656d 7320 696e 2074 6865 206c 6973  items in the lis
+000046c0: 742e 0a20 2020 202a 2a6b 7761 7267 733a  t..    **kwargs:
+000046d0: 204f 6e6c 7920 7265 636f 676e 697a 6564   Only recognized
+000046e0: 206b 7761 7267 2069 7320 2763 7478 5f74   kwarg is 'ctx_t
+000046f0: 7970 6527 2c20 7768 6963 6820 636f 6e74  ype', which cont
+00004700: 726f 6c73 2074 6865 0a20 2020 2020 2063  rols the.      c
+00004710: 7478 2074 7970 6520 6f66 2074 6865 206c  tx type of the l
+00004720: 6973 742e 2053 6565 2043 7478 456e 756d  ist. See CtxEnum
+00004730: 2e0a 0a20 2052 6574 7572 6e73 3a0a 2020  ...  Returns:.  
+00004740: 2020 416e 205f 6173 742e 4c69 7374 206e    An _ast.List n
+00004750: 6f64 652e 0a20 2072 3300 0000 a902 da04  ode..  r3.......
+00004760: 656c 7473 724d 0000 0029 0c72 7500 0000  eltsrM...).ru...
+00004770: 7266 0000 0072 1500 0000 7224 0000 0072  rf...r....r$...r
+00004780: 2e00 0000 7237 0000 0072 4f00 0000 724d  ....r7...rO...rM
+00004790: 0000 0072 8d00 0000 723d 0000 00da 044c  ...r....r=.....L
+000047a0: 6973 7472 2500 0000 2906 da05 6974 656d  istr%...)...item
+000047b0: 7372 8900 0000 7233 0000 00da 0469 7465  sr....r3.....ite
+000047c0: 6dda 096e 616d 655f 6e6f 6465 724d 0000  m..name_noderM..
+000047d0: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+000047e0: 72d8 0000 00a8 0200 0073 1800 0000 0e0d  r........s......
+000047f0: 0802 0c01 0c01 0c01 0801 0a01 0280 0801  ................
+00004800: 0a01 0201 06ff 72d8 0000 0063 0300 0000  ......r....c....
+00004810: 0000 0000 0000 0000 0400 0000 0600 0000  ................
+00004820: 4700 0000 f34a 0000 0074 007c 0074 016a  G....J...t.|.t.j
+00004830: 0264 018d 027d 0074 007c 0174 016a 0364  .d...}.t.|.t.j.d
+00004840: 018d 027d 0174 007c 0274 016a 0264 018d  ...}.t.|.t.j.d..
+00004850: 027d 0274 046a 057c 0074 067c 017c 0264  .}.t.j.|.t.|.|.d
+00004860: 0267 037c 03a2 0152 008e 0067 0164 038d  .g.|...R...g.d..
+00004870: 0253 0029 0461 4b01 0000 4372 6561 7465  .S.).aK...Create
+00004880: 7320 5f61 7374 2e4c 6973 7443 6f6d 7020  s _ast.ListComp 
+00004890: 6e6f 6465 732e 0a0a 2020 276c 6566 745f  nodes...  'left_
+000048a0: 7369 6465 2720 666f 7220 2766 6f72 5f70  side' for 'for_p
+000048b0: 6172 7427 2069 6e20 2769 6e5f 7061 7274  art' in 'in_part
+000048c0: 2720 6966 2027 6966 7327 0a0a 2020 4172  ' if 'ifs'..  Ar
+000048d0: 6773 3a0a 2020 2020 6c65 6674 5f73 6964  gs:.    left_sid
+000048e0: 653a 206c 6566 746d 6f73 7420 7369 6465  e: leftmost side
+000048f0: 206f 6620 7468 6520 6578 7072 6573 7369   of the expressi
+00004900: 6f6e 2e0a 2020 2020 666f 725f 7061 7274  on..    for_part
+00004910: 3a20 5468 6520 7061 7274 2061 6674 6572  : The part after
+00004920: 2027 5b6c 6566 745f 7369 6465 5d20 666f   '[left_side] fo
+00004930: 7220 270a 2020 2020 696e 5f70 6172 743a  r '.    in_part:
+00004940: 2054 6865 2070 6172 7420 6166 7465 7220   The part after 
+00004950: 275b 6c65 6674 5f73 6964 655d 2066 6f72  '[left_side] for
+00004960: 205b 666f 725f 7061 7274 5d20 696e 2027   [for_part] in '
+00004970: 0a20 2020 202a 6966 733a 2041 6e79 2069  .    *ifs: Any i
+00004980: 6620 7374 6174 656d 656e 7473 2074 6861  f statements tha
+00004990: 7420 636f 6d65 2061 7420 7468 6520 656e  t come at the en
+000049a0: 642e 0a0a 2020 5265 7475 726e 733a 0a20  d...  Returns:. 
+000049b0: 2020 207b 5f61 7374 2e4c 6973 7443 6f6d     {_ast.ListCom
+000049c0: 707d 0a20 2072 3200 0000 4672 b700 0000  p}.  r2...Fr....
+000049d0: 2907 7222 0000 0072 6600 0000 7215 0000  ).r"...rf...r...
+000049e0: 0072 1600 0000 722e 0000 00da 084c 6973  .r....r......Lis
+000049f0: 7443 6f6d 7072 a200 0000 a904 72ba 0000  tCompr......r...
+00004a00: 0072 a300 0000 72a4 0000 0072 a000 0000  .r....r....r....
+00004a10: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00004a20: dd00 0000 c202 0000 f30e 0000 000e 0e0e  ................
+00004a30: 010e 0104 0102 0114 0106 fe72 dd00 0000  ...........r....
+00004a40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004a50: 0002 0000 0043 0000 0072 5b00 0000 722d  .....C...r[...r-
+00004a60: 0000 0029 0272 2e00 0000 da06 4c53 6869  ...).r......LShi
+00004a70: 6674 7209 0000 0072 0900 0000 7209 0000  ftr....r....r...
+00004a80: 0072 0a00 0000 72e0 0000 00d8 0200 0072  .r....r........r
+00004a90: 5d00 0000 72e0 0000 0063 0000 0000 0000  ]...r....c......
+00004aa0: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
+00004ab0: 0000 725b 0000 0072 2d00 0000 2902 722e  ..r[...r-...).r.
+00004ac0: 0000 00da 024c 7472 0900 0000 7209 0000  .....Ltr....r...
+00004ad0: 0072 0900 0000 720a 0000 0072 e100 0000  .r....r....r....
+00004ae0: dc02 0000 725d 0000 0072 e100 0000 6300  ....r]...r....c.
+00004af0: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00004b00: 0000 0043 0000 0072 5b00 0000 722d 0000  ...C...r[...r-..
+00004b10: 0029 0272 2e00 0000 da03 4c74 4572 0900  .).r......LtEr..
+00004b20: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00004b30: 0072 e200 0000 e002 0000 725d 0000 0072  .r........r]...r
+00004b40: e200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00004b50: 0000 0000 0002 0000 0043 0000 0072 5b00  .........C...r[.
+00004b60: 0000 722d 0000 0029 0272 2e00 0000 da03  ..r-...).r......
+00004b70: 4d6f 6472 0900 0000 7209 0000 0072 0900  Modr....r....r..
+00004b80: 0000 720a 0000 0072 e300 0000 e402 0000  ..r....r........
+00004b90: 725d 0000 0072 e300 0000 6300 0000 0000  r]...r....c.....
+00004ba0: 0000 0000 0000 0001 0000 0003 0000 0047  ...............G
+00004bb0: 0000 0073 1c00 0000 7c00 7306 7400 6401  ...s....|.s.t.d.
+00004bc0: 8301 8201 7401 6a02 7403 7c00 8301 6402  ....t.j.t.|...d.
+00004bd0: 8d01 5300 2903 4e7a 2b4d 7573 7420 6861  ..S.).Nz+Must ha
+00004be0: 7665 2061 7420 6c65 6173 7420 6f6e 6520  ve at least one 
+00004bf0: 6172 6775 6d65 6e74 2069 6e20 7468 6520  argument in the 
+00004c00: 626f 6479 2901 7242 0000 0029 0472 2600  body).rB...).r&.
+00004c10: 0000 722e 0000 00da 064d 6f64 756c 6572  ..r......Moduler
+00004c20: 2500 0000 2901 da0a 626f 6479 5f69 7465  %...)...body_ite
+00004c30: 6d73 7209 0000 0072 0900 0000 720a 0000  msr....r....r...
+00004c40: 0072 e400 0000 e802 0000 7306 0000 0004  .r........s.....
+00004c50: 0108 0110 0172 e400 0000 6300 0000 0000  .....r....c.....
+00004c60: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+00004c70: 0000 0072 5b00 0000 722d 0000 0029 0272  ...r[...r-...).r
+00004c80: 2e00 0000 da04 4d75 6c74 7209 0000 0072  ......Multr....r
+00004c90: 0900 0000 7209 0000 0072 0a00 0000 72e6  ....r....r....r.
+00004ca0: 0000 00ee 0200 0072 5d00 0000 72e6 0000  .......r]...r...
+00004cb0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00004cc0: 0000 0300 0000 4300 0000 72ce 0000 0072  ......C...r....r
+00004cd0: 2d00 0000 2902 722e 0000 0072 1e00 0000  -...).r....r....
+00004ce0: 2901 721e 0000 0072 0900 0000 7209 0000  ).r....r....r...
+00004cf0: 0072 0a00 0000 7230 0000 00f2 0200 0072  .r....r0.......r
+00004d00: d000 0000 7230 0000 0063 0200 0000 0000  ....r0...c......
+00004d10: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00004d20: 0000 732c 0000 0074 006a 017c 0064 018d  ..s,...t.j.|.d..
+00004d30: 017d 0274 027c 0074 0383 0272 147c 0173  .}.t.|.t...r.|.s
+00004d40: 1174 0464 0283 0182 017c 017c 025f 057c  .t.d.....|.|._.|
+00004d50: 0253 0029 034e 72b1 0000 007a 3043 6f6e  .S.).Nr....z0Con
+00004d60: 7374 616e 7420 7374 7269 6e67 206d 7573  stant string mus
+00004d70: 7420 6265 2070 726f 7669 6465 6420 7769  t be provided wi
+00004d80: 7468 2071 756f 7465 2074 7970 6529 0672  th quote type).r
+00004d90: 2e00 0000 7235 0000 0072 2400 0000 7236  ....r5...r$...r6
+00004da0: 0000 0072 2600 0000 da0d 6465 6661 756c  ...r&.....defaul
+00004db0: 745f 7175 6f74 6529 0372 3a00 0000 da0a  t_quote).r:.....
+00004dc0: 7175 6f74 655f 7479 7065 723c 0000 0072  quote_typer<...r
+00004dd0: 0900 0000 7209 0000 0072 0a00 0000 7235  ....r....r....r5
+00004de0: 0000 00f6 0200 0073 0c00 0000 0c01 0a01  .......s........
+00004df0: 0401 0801 0601 0401 7235 0000 0063 0100  ........r5...c..
+00004e00: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00004e10: 0000 4300 0000 735e 0000 0074 007c 0074  ..C...s^...t.|.t
+00004e20: 0183 0273 0974 0264 0183 0182 017c 0064  ...s.t.d.....|.d
+00004e30: 0075 0073 137c 0064 0219 00a0 03a1 0072  .u.s.|.d.......r
+00004e40: 1a74 0264 037c 009b 009d 0283 0182 017c  .t.d.|.........|
+00004e50: 00a0 0464 0464 05a1 027d 017c 01a0 05a1  ...d.d...}.|....
+00004e60: 007d 027c 0273 2d74 0264 037c 009b 009d  .}.|.s-t.d.|....
+00004e70: 0283 0182 0164 0053 0029 064e 7a1a 7079  .....d.S.).Nz.py
+00004e80: 7468 6f6e 2069 6420 6d75 7374 2062 6520  thon id must be 
+00004e90: 6120 7374 7269 6e67 7201 0000 007a 1349  a stringr....z.I
+00004ea0: 6e76 616c 6964 2070 7974 686f 6e20 6964  nvalid python id
+00004eb0: 3a20 da01 5f72 c300 0000 2906 7224 0000  : .._r....).r$..
+00004ec0: 0072 3600 0000 7226 0000 00da 0769 7364  .r6...r&.....isd
+00004ed0: 6967 6974 da07 7265 706c 6163 65da 0769  igit..replace..i
+00004ee0: 7361 6c6e 756d 2903 da07 6e61 6d65 5f69  salnum)...name_i
+00004ef0: 64da 1373 7472 6970 7065 645f 756e 6465  d..stripped_unde
+00004f00: 7273 636f 7265 72ec 0000 0072 0900 0000  rscorer....r....
+00004f10: 7209 0000 0072 0a00 0000 da0b 7661 6c69  r....r......vali
+00004f20: 6461 7465 5f69 64ff 0200 0073 1200 0000  date_id....s....
+00004f30: 0a01 0801 1401 0e01 0c01 0801 0401 0e01  ................
+00004f40: 04ff 72ef 0000 0063 0200 0000 0000 0000  ..r....c........
+00004f50: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00004f60: 731e 0000 0074 007c 0083 0101 0074 017c  s....t.|.....t.|
+00004f70: 0183 017d 0274 026a 037c 007c 0264 018d  ...}.t.j.|.|.d..
+00004f80: 0253 0029 027a 8f43 7265 6174 6573 2061  .S.).z.Creates a
+00004f90: 6e20 5f61 7374 2e4e 616d 6520 6e6f 6465  n _ast.Name node
+00004fa0: 2e0a 0a20 2041 7267 733a 0a20 2020 206e  ...  Args:.    n
+00004fb0: 616d 655f 6964 3a20 4e61 6d65 206f 6620  ame_id: Name of 
+00004fc0: 7468 6520 6e6f 6465 2e0a 2020 2020 6374  the node..    ct
+00004fd0: 785f 7479 7065 3a20 5365 6520 4374 7845  x_type: See CtxE
+00004fe0: 6e75 6d20 666f 7220 6f70 7469 6f6e 732e  num for options.
+00004ff0: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
+00005000: 2041 6e20 5f61 7374 2e4e 616d 6520 6e6f   An _ast.Name no
+00005010: 6465 2e0a 2020 a902 7239 0000 0072 4d00  de..  ..r9...rM.
+00005020: 0000 2904 72ef 0000 0072 4f00 0000 722e  ..).r....rO...r.
+00005030: 0000 0072 3700 0000 2903 72ed 0000 0072  ...r7...).r....r
+00005040: 3300 0000 724d 0000 0072 0900 0000 7209  3...rM...r....r.
+00005050: 0000 0072 0a00 0000 7237 0000 000a 0300  ...r....r7......
+00005060: 0073 0a00 0000 080a 0801 0601 0201 06ff  .s..............
+00005070: 7237 0000 0063 0000 0000 0000 0000 0000  r7...c..........
+00005080: 0000 0000 0000 0200 0000 4300 0000 725b  ..........C...r[
+00005090: 0000 0072 2d00 0000 2902 722e 0000 00da  ...r-...).r.....
+000050a0: 034e 6f74 7209 0000 0072 0900 0000 7209  .Notr....r....r.
+000050b0: 0000 0072 0a00 0000 72f1 0000 001e 0300  ...r....r.......
+000050c0: 0072 5d00 0000 72f1 0000 0063 0000 0000  .r]...r....c....
+000050d0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+000050e0: 4300 0000 725b 0000 0072 2d00 0000 2902  C...r[...r-...).
+000050f0: 722e 0000 00da 054e 6f74 4571 7209 0000  r......NotEqr...
+00005100: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00005110: 72f2 0000 0022 0300 0072 5d00 0000 72f2  r...."...r]...r.
+00005120: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00005130: 0000 0000 0200 0000 4300 0000 725b 0000  ........C...r[..
+00005140: 0072 2d00 0000 2902 722e 0000 00da 054e  .r-...).r......N
+00005150: 6f74 496e 7209 0000 0072 0900 0000 7209  otInr....r....r.
+00005160: 0000 0072 0a00 0000 72f3 0000 0026 0300  ...r....r....&..
+00005170: 0072 5d00 0000 72f3 0000 0063 0100 0000  .r]...r....c....
+00005180: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00005190: 4300 0000 733c 0000 0074 007c 0074 0183  C...s<...t.|.t..
+000051a0: 0273 0974 0264 0183 0182 0174 037c 0083  .s.t.d.....t.|..
+000051b0: 017d 0174 046a 0574 067c 007c 0183 0264  .}.t.j.t.|.|...d
+000051c0: 028d 017d 0264 037c 025f 077c 017c 025f  ...}.d.|._.|.|._
+000051d0: 087c 0253 0029 04fa 1e43 7265 6174 6573  .|.S.)...Creates
+000051e0: 2061 6e20 5f61 7374 2e43 6f6e 7374 616e   an _ast.Constan
+000051f0: 7420 6e6f 6465 2e7a 256e 756d 6265 7220  t node.z%number 
+00005200: 6d75 7374 2062 6520 6120 7374 7220 746f  must be a str to
+00005210: 2073 7570 706f 7274 2062 6173 6573 72b1   support basesr.
+00005220: 0000 00fa 0127 2909 7224 0000 0072 3600  .....').r$...r6.
+00005230: 0000 7226 0000 0072 6700 0000 722e 0000  ..r&...rg...r...
+00005240: 0072 3500 0000 7234 0000 0072 e700 0000  .r5...r4...r....
+00005250: 7269 0000 0029 03da 066e 756d 6265 7272  ri...)...numberr
+00005260: 6900 0000 726e 0000 0072 0900 0000 7209  i...rn...r....r.
+00005270: 0000 0072 0a00 0000 da03 4e75 6d2a 0300  ...r......Num*..
+00005280: 0073 0e00 0000 0a02 0801 0801 1201 0601  .s..............
+00005290: 0601 0401 72f7 0000 0063 0100 0000 0000  ....r....c......
+000052a0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000052b0: 0000 734a 0000 0074 007c 0083 01a0 0164  ..sJ...t.|.....d
+000052c0: 01a1 0172 0b64 027d 017c 0153 0074 007c  ...r.d.}.|.S.t.|
+000052d0: 0083 01a0 0164 03a1 0172 1664 047d 017c  .....d...r.d.}.|
+000052e0: 0153 0074 007c 0083 01a0 0164 05a1 0172  .S.t.|.....d...r
+000052f0: 2164 067d 017c 0153 0064 077d 017c 0153  !d.}.|.S.d.}.|.S
+00005300: 0029 084e da02 3062 7295 0000 00da 0230  .).N..0br......0
+00005310: 6fe9 0800 0000 da02 3078 e910 0000 00e9  o.......0x......
+00005320: 0a00 0000 2902 7236 0000 00da 0a73 7461  ....).r6.....sta
+00005330: 7274 7377 6974 6829 0272 f600 0000 7269  rtswith).r....ri
+00005340: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00005350: 0000 7267 0000 0035 0300 0073 1600 0000  ..rg...5...s....
+00005360: 0e01 0401 0407 0efa 0401 0405 0efc 0401  ................
+00005370: 0403 04ff 0401 7267 0000 0063 0100 0000  ......rg...c....
+00005380: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00005390: 4300 0000 730e 0000 0074 00a0 0174 027c  C...s....t...t.|
+000053a0: 0083 01a1 0153 0029 0172 f400 0000 2903  .....S.).r....).
+000053b0: 722e 0000 0072 3500 0000 da04 626f 6f6c  r....r5.....bool
+000053c0: 2901 da07 626f 6f6c 6561 6e72 0900 0000  )...booleanr....
+000053d0: 7209 0000 0072 0a00 0000 da04 426f 6f6c  r....r......Bool
+000053e0: 4103 0000 7302 0000 000e 0272 0101 0000  A...s......r....
+000053f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00005400: 0002 0000 0043 0000 0072 5b00 0000 722d  .....C...r[...r-
+00005410: 0000 0029 0272 2e00 0000 7278 0000 0072  ...).r....rx...r
+00005420: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00005430: 0000 0072 7800 0000 4503 0000 725d 0000  ...rx...E...r]..
+00005440: 0072 7800 0000 6300 0000 0000 0000 0000  .rx...c.........
+00005450: 0000 0000 0000 0002 0000 0043 0000 0072  ...........C...r
+00005460: 5b00 0000 2901 7a1a 4372 6561 7465 7320  [...).z.Creates 
+00005470: 616e 205f 6173 742e 5061 7373 206e 6f64  an _ast.Pass nod
+00005480: 652e 2902 722e 0000 0072 3f00 0000 7209  e.).r....r?...r.
+00005490: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+000054a0: 0000 723f 0000 0049 0300 0073 0200 0000  ..r?...I...s....
+000054b0: 0802 723f 0000 0063 0000 0000 0000 0000  ..r?...c........
+000054c0: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
+000054d0: 725b 0000 0072 2d00 0000 2902 722e 0000  r[...r-...).r...
+000054e0: 00da 0350 6f77 7209 0000 0072 0900 0000  ...Powr....r....
+000054f0: 7209 0000 0072 0a00 0000 7202 0100 004e  r....r....r....N
+00005500: 0300 0072 5d00 0000 7202 0100 0063 0200  ...r]...r....c..
+00005510: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+00005520: 0000 4300 0000 7370 0000 0074 007c 0074  ..C...sp...t.|.t
+00005530: 0183 0272 0c74 0274 037c 0083 0183 017d  ...r.t.t.|.....}
+00005540: 026e 2474 007c 0074 0383 0272 217c 0164  .n$t.|.t...r!|.d
+00005550: 0075 0072 1974 0464 0183 0182 0174 057c  .u.r.t.d.....t.|
+00005560: 0083 017d 027c 017c 025f 066e 0f74 007c  ...}.|.|._.n.t.|
+00005570: 0074 076a 0883 0272 2c74 07a0 097c 00a1  .t.j...r,t...|..
+00005580: 0153 0074 0464 0283 0182 0174 076a 097c  .S.t.d.....t.j.|
+00005590: 0264 038d 017d 037c 0353 0029 044e 7a44  .d...}.|.S.).NzD
+000055a0: 4d75 7374 2070 726f 7669 7465 2071 756f  Must provite quo
+000055b0: 7465 2074 7970 6520 7768 656e 2063 7265  te type when cre
+000055c0: 6174 696e 6720 6120 5265 7475 726e 206e  ating a Return n
+000055d0: 6f64 6520 7765 6974 6820 7479 7065 2073  ode weith type s
+000055e0: 7472 2e2e 7a14 496e 7661 6c69 6420 7265  tr..z.Invalid re
+000055f0: 7475 726e 2076 616c 7565 72b1 0000 0029  turn valuer....)
+00005600: 0a72 2400 0000 7234 0000 0072 f700 0000  .r$...r4...r....
+00005610: 7236 0000 0072 2600 0000 da03 5374 7272  r6...r&.....Strr
+00005620: e700 0000 722e 0000 0072 2f00 0000 da06  ....r....r/.....
+00005630: 5265 7475 726e 2904 723a 0000 0072 e800  Return).r:...r..
+00005640: 0000 da0a 7661 6c75 655f 6e6f 6465 726e  ....value_nodern
+00005650: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00005660: 0000 7204 0100 0052 0300 0073 1800 0000  ..r....R...s....
+00005670: 0a02 0e01 0a01 0801 0801 0801 0801 0c01  ................
+00005680: 0a01 0802 0c01 0401 7204 0100 0063 0000  ........r....c..
+00005690: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000056a0: 0000 4300 0000 725b 0000 0072 2d00 0000  ..C...r[...r-...
+000056b0: 2902 722e 0000 00da 0652 5368 6966 7472  ).r......RShiftr
+000056c0: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+000056d0: 0000 0072 0601 0000 6203 0000 725d 0000  ...r....b...r]..
+000056e0: 0072 0601 0000 6300 0000 0000 0000 0000  .r....c.........
+000056f0: 0000 0001 0000 0003 0000 0047 0000 0073  ...........G...s
+00005700: 1000 0000 7400 6a01 7402 7c00 8301 6401  ....t.j.t.|...d.
+00005710: 8d01 5300 2902 7a69 4372 6561 7465 7320  ..S.).ziCreates 
+00005720: 616e 205f 6173 742e 5365 7420 6e6f 6465  an _ast.Set node
+00005730: 2e0a 0a20 2041 7267 733a 0a20 2020 202a  ...  Args:.    *
+00005740: 6974 656d 733a 2054 6865 2069 7465 6d73  items: The items
+00005750: 2069 6e20 7468 6520 7365 742e 0a0a 2020   in the set...  
+00005760: 5265 7475 726e 733a 0a20 2020 2041 6e20  Returns:.    An 
+00005770: 5f61 7374 2e53 6574 206e 6f64 652e 0a20  _ast.Set node.. 
+00005780: 2029 0172 d700 0000 2903 722e 0000 00da   ).r....).r.....
+00005790: 0353 6574 7225 0000 0029 0172 d900 0000  .Setr%...).r....
+000057a0: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000057b0: 0701 0000 6603 0000 7302 0000 0010 0972  ....f...s......r
+000057c0: 0701 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000057d0: 0004 0000 0006 0000 0047 0000 0072 dc00  .........G...r..
+000057e0: 0000 2904 6149 0100 0043 7265 6174 6573  ..).aI...Creates
+000057f0: 205f 6173 742e 5365 7443 6f6d 7020 6e6f   _ast.SetComp no
+00005800: 6465 732e 0a0a 2020 276c 6566 745f 7369  des...  'left_si
+00005810: 6465 2720 666f 7220 2766 6f72 5f70 6172  de' for 'for_par
+00005820: 7427 2069 6e20 2769 6e5f 7061 7274 2720  t' in 'in_part' 
+00005830: 6966 2027 6966 7327 0a0a 2020 4172 6773  if 'ifs'..  Args
+00005840: 3a0a 2020 2020 6c65 6674 5f73 6964 653a  :.    left_side:
+00005850: 206c 6566 746d 6f73 7420 7369 6465 206f   leftmost side o
+00005860: 6620 7468 6520 6578 7072 6573 7369 6f6e  f the expression
+00005870: 2e0a 2020 2020 666f 725f 7061 7274 3a20  ..    for_part: 
+00005880: 5468 6520 7061 7274 2061 6674 6572 2027  The part after '
+00005890: 5b6c 6566 745f 7369 6465 5d20 666f 7220  [left_side] for 
+000058a0: 270a 2020 2020 696e 5f70 6172 743a 2054  '.    in_part: T
+000058b0: 6865 2070 6172 7420 6166 7465 7220 275b  he part after '[
+000058c0: 6c65 6674 5f73 6964 655d 2066 6f72 205b  left_side] for [
+000058d0: 666f 725f 7061 7274 5d20 696e 2027 0a20  for_part] in '. 
+000058e0: 2020 202a 6966 733a 2041 6e79 2069 6620     *ifs: Any if 
+000058f0: 7374 6174 656d 656e 7473 2074 6861 7420  statements that 
+00005900: 636f 6d65 2061 7420 7468 6520 656e 642e  come at the end.
+00005910: 0a0a 2020 5265 7475 726e 733a 0a20 2020  ..  Returns:.   
+00005920: 207b 5f61 7374 2e53 6574 436f 6d70 7d0a   {_ast.SetComp}.
+00005930: 2020 7232 0000 0046 72b7 0000 0029 0772    r2...Fr....).r
+00005940: 2200 0000 7266 0000 0072 1500 0000 7216  "...rf...r....r.
+00005950: 0000 0072 2e00 0000 da07 5365 7443 6f6d  ...r......SetCom
+00005960: 7072 a200 0000 72de 0000 0072 0900 0000  pr....r....r....
+00005970: 7209 0000 0072 0a00 0000 7208 0100 0072  r....r....r....r
+00005980: 0300 0072 df00 0000 7208 0100 0063 0300  ...r....r....c..
+00005990: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+000059a0: 0000 4300 0000 7310 0000 0074 006a 017c  ..C...s....t.j.|
+000059b0: 007c 017c 0264 018d 0353 0029 024e a903  .|.|.d...S.).N..
+000059c0: da05 6c6f 7765 72da 0575 7070 6572 da04  ..lower..upper..
+000059d0: 7374 6570 2902 722e 0000 00da 0553 6c69  step).r......Sli
+000059e0: 6365 7209 0100 0072 0900 0000 7209 0000  cer....r....r...
+000059f0: 0072 0a00 0000 720d 0100 0088 0300 0073  .r....r........s
+00005a00: 0200 0000 1001 720d 0100 0063 0100 0000  ......r....c....
+00005a10: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00005a20: 4300 0000 730c 0000 0074 006a 017c 0064  C...s....t.j.|.d
+00005a30: 018d 0153 0029 027a 1943 7265 6174 6573  ...S.).z.Creates
+00005a40: 2061 6e20 5f61 7374 2e53 7472 206e 6f64   an _ast.Str nod
+00005a50: 652e a901 da01 7329 0272 2e00 0000 7235  e.....s).r....r5
+00005a60: 0000 0072 0e01 0000 7209 0000 0072 0900  ...r....r....r..
+00005a70: 0000 720a 0000 0072 0301 0000 8c03 0000  ..r....r........
+00005a80: 7302 0000 000c 0372 0301 0000 6301 0000  s......r....c...
+00005a90: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00005aa0: 0043 0000 0073 1400 0000 7400 6a01 7c00  .C...s....t.j.|.
+00005ab0: 7402 7403 6a04 8301 6401 8d02 5300 2902  t.t.j...d...S.).
+00005ac0: 7a1d 4372 6561 7465 7320 616e 205f 6173  z.Creates an _as
+00005ad0: 742e 5374 6172 7265 6420 6e6f 6465 2e29  t.Starred node.)
+00005ae0: 0272 3a00 0000 724d 0000 0029 0572 2e00  .r:...rM...).r..
+00005af0: 0000 da07 5374 6172 7265 6472 4f00 0000  ....StarredrO...
+00005b00: 7266 0000 0072 1500 0000 720e 0100 0072  rf...r....r....r
+00005b10: 0900 0000 7209 0000 0072 0a00 0000 7210  ....r....r....r.
+00005b20: 0100 0092 0300 0073 0200 0000 1403 7210  .......s......r.
+00005b30: 0100 0063 0000 0000 0000 0000 0000 0000  ...c............
+00005b40: 0000 0000 0200 0000 4300 0000 725b 0000  ........C...r[..
+00005b50: 0072 2d00 0000 2902 722e 0000 00da 0353  .r-...).r......S
+00005b60: 7562 7209 0000 0072 0900 0000 7209 0000  ubr....r....r...
+00005b70: 0072 0a00 0000 7211 0100 0098 0300 0072  .r....r........r
+00005b80: 5d00 0000 7211 0100 0063 0500 0000 0000  ]...r....c......
+00005b90: 0000 0000 0000 0800 0000 0700 0000 4300  ..............C.
+00005ba0: 0000 7382 0000 0074 007c 007c 0483 027d  ..s....t.|.|...}
+00005bb0: 0067 0064 01a2 017d 0574 017c 017c 027c  .g.d...}.t.|.|.|
+00005bc0: 0367 0383 0144 005d 1c5c 027d 067d 077c  .g...D.].\.}.}.|
+00005bd0: 0764 0075 0172 2c74 027c 0774 0383 0273  .d.u.r,t.|.t...s
+00005be0: 2174 0464 0283 0182 0174 007c 0774 056a  !t.d.....t.|.t.j
+00005bf0: 0664 038d 027d 077c 077c 057c 063c 0071  .d...}.|.|.|.<.q
+00005c00: 1074 076a 087c 0074 097c 0564 0419 007c  .t.j.|.t.|.d...|
+00005c10: 0564 0519 007c 0564 0619 0083 0374 0a7c  .d...|.d.....t.|
+00005c20: 0483 0164 078d 0353 0029 084e a903 4e4e  ...d...S.).N..NN
+00005c30: 4e7a 1853 7562 7363 7269 7074 206d 7573  Nz.Subscript mus
+00005c40: 7420 6265 2061 6e20 696e 7472 3200 0000  t be an intr2...
+00005c50: 7201 0000 0072 9600 0000 7295 0000 0029  r....r....r....)
+00005c60: 0372 3a00 0000 da05 736c 6963 6572 4d00  .r:.....slicerM.
+00005c70: 0000 290b 7222 0000 0072 9a00 0000 7224  ..).r"...r....r$
+00005c80: 0000 0072 3400 0000 7226 0000 0072 6600  ...r4...r&...rf.
+00005c90: 0000 7215 0000 0072 2e00 0000 da09 5375  ..r....r......Su
+00005ca0: 6273 6372 6970 7472 0d01 0000 724f 0000  bscriptr....rO..
+00005cb0: 0029 0872 3a00 0000 720b 0100 0072 0a01  .).r:...r....r..
+00005cc0: 0000 720c 0100 0072 4d00 0000 da09 6e65  ..r....rM.....ne
+00005cd0: 775f 626f 756e 6472 9e00 0000 72da 0000  w_boundr....r...
+00005ce0: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00005cf0: 7214 0100 009c 0300 0073 1800 0000 0a01  r........s......
+00005d00: 0801 1601 0801 0a01 0801 0e01 0801 0280  ................
+00005d10: 0401 1e01 06ff 7214 0100 0063 0000 0000  ......r....c....
+00005d20: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00005d30: 0000 0000 7328 0000 0065 005a 0164 005a  ....s(...e.Z.d.Z
+00005d40: 0287 0066 0164 0164 0284 085a 0365 0464  ...f.d.d...Z.e.d
+00005d50: 0364 0484 0083 015a 0587 0004 005a 0653  .d.....Z.....Z.S
+00005d60: 0029 05da 0743 6f6d 6d65 6e74 6302 0000  .)...Commentc...
+00005d70: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00005d80: 0003 0000 0073 3800 0000 7400 7401 7c00  .....s8...t.t.|.
+00005d90: 8302 a002 a100 0100 7c01 a003 6401 a101  ........|...d...
+00005da0: 7310 7404 6402 8301 8201 6700 7c00 5f05  s.t.d.....g.|._.
+00005db0: 7c01 6403 6400 8502 1900 7c00 5f06 6400  |.d.d.....|._.d.
+00005dc0: 5300 2904 4efa 0123 7a19 436f 6d6d 656e  S.).N..#z.Commen
+00005dd0: 7420 6d75 7374 2073 7461 7274 2077 6974  t must start wit
+00005de0: 6820 2372 9600 0000 2907 7246 0000 0072  h #r....).rF...r
+00005df0: 1601 0000 7247 0000 0072 fe00 0000 7226  ....rG...r....r&
+00005e00: 0000 00da 075f 6669 656c 6473 da07 636f  ....._fields..co
+00005e10: 6d6d 656e 7429 0272 4900 0000 7219 0100  mment).rI...r...
+00005e20: 0072 4b00 0000 7209 0000 0072 0a00 0000  .rK...r....r....
+00005e30: 7247 0000 00aa 0300 0073 0a00 0000 0e01  rG.......s......
+00005e40: 0a01 0801 0601 1201 7a10 436f 6d6d 656e  ........z.Commen
+00005e50: 742e 5f5f 696e 6974 5f5f 6301 0000 0000  t.__init__c.....
+00005e60: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00005e70: 0000 0073 1a00 0000 7c00 6a00 6400 7501  ...s....|.j.d.u.
+00005e80: 720b 6401 7c00 6a00 9b00 9d02 5300 6400  r.d.|.j.....S.d.
+00005e90: 5300 2902 4e72 1701 0000 2901 7219 0100  S.).Nr....).r...
+00005ea0: 0029 0172 4900 0000 7209 0000 0072 0900  .).rI...r....r..
+00005eb0: 0000 720a 0000 00da 0e73 6f75 7263 655f  ..r......source_
+00005ec0: 636f 6d6d 656e 74b1 0300 0073 0600 0000  comment....s....
+00005ed0: 0a02 0c01 04ff 7a16 436f 6d6d 656e 742e  ......z.Comment.
+00005ee0: 736f 7572 6365 5f63 6f6d 6d65 6e74 2907  source_comment).
+00005ef0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00005f00: 4700 0000 da08 7072 6f70 6572 7479 721a  G.....propertyr.
+00005f10: 0100 0072 5000 0000 7209 0000 0072 0900  ...rP...r....r..
+00005f20: 0000 724b 0000 0072 0a00 0000 7216 0100  ..rK...r....r...
+00005f30: 00a9 0300 0073 0800 0000 0800 0c01 0207  .....s..........
+00005f40: 1201 7216 0100 0063 0100 0000 0000 0000  ..r....c........
+00005f50: 0000 0000 0700 0000 0600 0000 4b00 0000  ............K...
+00005f60: 73ac 0000 0074 007c 0074 0183 0273 0974  s....t.|.t...s.t
+00005f70: 0264 0183 0182 017c 01a0 0364 0274 046a  .d.....|...d.t.j
+00005f80: 05a1 027d 0267 007d 037c 0044 005d 167d  ...}.g.}.|.D.].}
+00005f90: 0474 007c 0474 0674 0774 086a 0966 0383  .t.|.t.t.t.j.f..
+00005fa0: 0272 277c 03a0 0a74 0b7c 0483 01a1 0101  .r'|...t.|......
+00005fb0: 0071 1474 0c64 0383 0182 017c 0344 005d  .q.t.d.....|.D.]
+00005fc0: 1d7d 0474 007c 0474 0d6a 0e83 0272 3b74  .}.t.|.t.j...r;t
+00005fd0: 0f7c 0283 017c 045f 1071 2d74 007c 0474  .|...|._.q-t.|.t
+00005fe0: 0d6a 1183 0272 4a74 127c 0483 017d 0574  .j...rJt.|...}.t
+00005ff0: 0f7c 0283 017c 055f 1071 2d74 0f7c 0283  .|...|._.q-t.|..
+00006000: 017d 0674 0d6a 137c 037c 0664 048d 0253  .}.t.j.|.|.d...S
+00006010: 0029 0561 0701 0000 4372 6561 7465 7320  .).a....Creates 
+00006020: 616e 205f 6173 742e 5475 706c 6520 6e6f  an _ast.Tuple no
+00006030: 6465 2e0a 0a20 2041 7574 6f6d 6174 6963  de...  Automatic
+00006040: 616c 6c79 2061 646a 7573 7473 2069 6e6e  ally adjusts inn
+00006050: 6572 2063 7478 2061 7474 7273 2e0a 0a20  er ctx attrs... 
+00006060: 2041 7267 733a 0a20 2020 202a 6974 656d   Args:.    *item
+00006070: 733a 2054 6865 2069 7465 6d73 2069 6e20  s: The items in 
+00006080: 7468 6520 6c69 7374 2e0a 2020 2020 2a2a  the list..    **
+00006090: 6b77 6172 6773 3a20 4f6e 6c79 2072 6563  kwargs: Only rec
+000060a0: 6f67 6e69 7a65 6420 6b77 6172 6720 6973  ognized kwarg is
+000060b0: 2027 6374 785f 7479 7065 272c 2077 6869   'ctx_type', whi
+000060c0: 6368 2063 6f6e 7472 6f6c 7320 7468 650a  ch controls the.
+000060d0: 2020 2020 2020 6374 7820 7479 7065 206f        ctx type o
+000060e0: 6620 7468 6520 6c69 7374 2e20 5365 6520  f the list. See 
+000060f0: 4374 7845 6e75 6d2e 0a0a 2020 5265 7475  CtxEnum...  Retu
+00006100: 726e 733a 0a20 2020 2041 6e20 5f61 7374  rns:.    An _ast
+00006110: 2e54 7570 6c65 206e 6f64 652e 0a20 207a  .Tuple node..  z
+00006120: 1f69 7465 6d73 2069 6e20 7475 706c 6520  .items in tuple 
+00006130: 7368 6f75 6c64 2062 6520 6120 6c69 7374  should be a list
+00006140: 7233 0000 007a 1f54 7570 6c65 2069 7465  r3...z.Tuple ite
+00006150: 6d20 7479 7065 206e 6f74 2069 6d70 6c65  m type not imple
+00006160: 6d65 6e74 6564 72d6 0000 0029 1472 2400  mentedr....).r$.
+00006170: 0000 7225 0000 0072 2600 0000 7275 0000  ..r%...r&...ru..
+00006180: 0072 6600 0000 7215 0000 0072 3600 0000  .rf...r....r6...
+00006190: 7234 0000 0072 b500 0000 7235 0000 0072  r4...r....r5...r
+000061a0: 2700 0000 7222 0000 0072 3800 0000 722e  '...r"...r8...r.
+000061b0: 0000 0072 3700 0000 724f 0000 0072 4d00  ...r7...rO...rM.
+000061c0: 0000 728d 0000 0072 3d00 0000 da05 5475  ..r....r=.....Tu
+000061d0: 706c 6529 0772 d900 0000 7289 0000 0072  ple).r....r....r
+000061e0: 3300 0000 da09 6e65 775f 6974 656d 7372  3.....new_itemsr
+000061f0: da00 0000 72db 0000 0072 4d00 0000 7209  ....r....rM...r.
+00006200: 0000 0072 0900 0000 720a 0000 0072 1c01  ...r....r....r..
+00006210: 0000 b703 0000 7326 0000 000a 0d08 010e  ......s&........
+00006220: 0104 0208 0112 0110 0108 0208 020c 010c  ................
+00006230: 010c 0108 010a 0102 8008 0106 0102 0106  ................
+00006240: ff72 1c01 0000 6304 0000 0000 0000 0000  .r....c.........
+00006250: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00006260: 3000 0000 7400 7c02 8301 7d04 7c01 720b  0...t.|...}.|.r.
+00006270: 7401 7c01 7402 8302 730f 7403 6401 8301  t.|.t...s.t.d...
+00006280: 8201 7404 6a05 7c00 7c01 7c04 7c03 6402  ..t.j.|.|.|.|.d.
+00006290: 8d04 5300 2903 4e7a 2b45 7863 6570 7469  ..S.).Nz+Excepti
+000062a0: 6f6e 2068 616e 646c 6572 7320 6d75 7374  on handlers must
+000062b0: 2062 6520 6120 6e6f 6e2d 656d 7074 7920   be a non-empty 
+000062c0: 6c69 7374 2904 7242 0000 00da 0868 616e  list).rB.....han
+000062d0: 646c 6572 73da 0966 696e 616c 626f 6479  dlers..finalbody
+000062e0: 72bd 0000 0029 0672 4400 0000 7224 0000  r....).rD...r$..
+000062f0: 0072 2500 0000 7226 0000 0072 2e00 0000  .r%...r&...r....
+00006300: da03 5472 7929 0572 4200 0000 da0f 6578  ..Try).rB.....ex
+00006310: 6365 7074 5f68 616e 646c 6572 73da 0a66  cept_handlers..f
+00006320: 696e 616c 7962 6f64 7972 bd00 0000 721f  inalybodyr....r.
+00006330: 0100 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00006340: 0000 7220 0100 00da 0300 0073 0800 0000  ..r .......s....
+00006350: 0801 0e02 0801 1201 7220 0100 0063 0400  ........r ...c..
+00006360: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+00006370: 0000 4300 0000 7312 0000 0074 006a 017c  ..C...s....t.j.|
+00006380: 007c 017c 0267 0064 018d 0453 0029 024e  .|.|.g.d...S.).N
+00006390: 2901 72bd 0000 0029 0272 b500 0000 da03  ).r....).r......
+000063a0: 466f 7229 0472 6d00 0000 729f 0000 0072  For).rm...r....r
+000063b0: 4200 0000 72bd 0000 0072 0900 0000 7209  B...r....r....r.
+000063c0: 0000 0072 0a00 0000 7223 0100 00e1 0300  ...r....r#......
+000063d0: 0073 0200 0000 1201 7223 0100 0063 0000  .s......r#...c..
+000063e0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+000063f0: 0000 4300 0000 725b 0000 0072 2d00 0000  ..C...r[...r-...
+00006400: 2902 722e 0000 00da 0455 4164 6472 0900  ).r......UAddr..
+00006410: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00006420: 0072 2401 0000 e503 0000 725d 0000 0072  .r$.......r]...r
+00006430: 2401 0000 6302 0000 0000 0000 0000 0000  $...c...........
+00006440: 0002 0000 0004 0000 0043 0000 0073 2200  .........C...s".
+00006450: 0000 7400 7c00 7401 6a02 8302 730a 7403  ..t.|.t.j...s.t.
+00006460: 7c00 8301 7d00 7401 6a04 7c00 7c01 6401  |...}.t.j.|.|.d.
+00006470: 8d02 5300 2902 7a28 4f70 6572 6174 6f72  ..S.).z(Operator
+00006480: 206c 6974 6572 616c 7320 2827 6e6f 7427   literals ('not'
+00006490: 2920 616c 736f 2061 6363 6570 7465 642e  ) also accepted.
+000064a0: 2902 726f 0000 00da 076f 7065 7261 6e64  ).ro.....operand
+000064b0: 2905 7224 0000 0072 2e00 0000 722f 0000  ).r$...r....r/..
+000064c0: 00da 0a55 6e61 7279 4f70 4d61 70da 0755  ...UnaryOpMap..U
+000064d0: 6e61 7279 4f70 2902 da08 6f70 6572 6174  naryOp)...operat
+000064e0: 6f72 7225 0100 0072 0900 0000 7209 0000  orr%...r....r...
+000064f0: 0072 0a00 0000 7227 0100 00e9 0300 0073  .r....r'.......s
+00006500: 0600 0000 0c02 0801 0e01 7227 0100 0063  ..........r'...c
+00006510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006520: 0200 0000 4300 0000 725b 0000 0072 2d00  ....C...r[...r-.
+00006530: 0000 2902 722e 0000 00da 0455 5375 6272  ..).r......USubr
+00006540: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00006550: 0000 0072 2901 0000 f003 0000 725d 0000  ...r).......r]..
+00006560: 0072 2901 0000 6302 0000 0000 0000 0000  .r)...c.........
+00006570: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+00006580: 4800 0000 7400 7c01 7401 8302 720d 7402  H...t.|.t...r.t.
+00006590: 7c01 7403 6a04 6401 8d02 7d01 6e0f 7c01  |.t.j.d...}.n.|.
+000065a0: 721c 7400 7c01 7405 6a06 7405 6a07 6602  r.t.|.t.j.t.j.f.
+000065b0: 8302 731c 7408 6402 8301 8201 7409 a00a  ..s.t.d.....t...
+000065c0: 7402 7c00 8301 7c01 a102 5300 2903 4e72  t.|...|...S.).Nr
+000065d0: 3200 0000 7a24 7769 7468 6974 656d 206d  2...z$withitem m
+000065e0: 7573 7420 6265 2073 7472 2c20 7475 706c  ust be str, tupl
+000065f0: 652c 206f 7220 6c69 7374 290b 7224 0000  e, or list).r$..
+00006600: 0072 3600 0000 7237 0000 0072 6600 0000  .r6...r7...rf...
+00006610: 7216 0000 0072 b500 0000 721c 0100 0072  r....r....r....r
+00006620: d800 0000 7226 0000 0072 2e00 0000 da08  ....r&...r......
+00006630: 7769 7468 6974 656d 2902 7290 0000 00da  withitem).r.....
+00006640: 0d6f 7074 696f 6e61 6c5f 7661 7273 7209  .optional_varsr.
+00006650: 0000 0072 0900 0000 720a 0000 0072 2a01  ...r....r....r*.
+00006660: 0000 f403 0000 730a 0000 000a 0110 0116  ......s.........
+00006670: 0108 0110 0172 2a01 0000 6302 0000 0000  .....r*...c.....
+00006680: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00006690: 0000 0073 3c00 0000 7400 7c01 7401 8302  ...s<...t.|.t...
+000066a0: 7309 7402 6401 8301 8201 7400 7c00 7401  s.t.d.....t.|.t.
+000066b0: 8302 7312 7402 6402 8301 8201 7403 7c01  ..s.t.d.....t.|.
+000066c0: 8301 7d01 7404 6a05 7c00 7c01 6400 6403  ..}.t.j.|.|.d.d.
+000066d0: 8d03 5300 2904 4e7a 1857 6974 682d 626f  ..S.).Nz.With-bo
+000066e0: 6479 206d 7573 7420 6265 2061 206c 6973  dy must be a lis
+000066f0: 747a 1877 6974 6869 7465 6d73 206d 7573  tz.withitems mus
+00006700: 7420 6265 2061 206c 6973 7429 0372 d900  t be a list).r..
+00006710: 0000 7242 0000 0072 b400 0000 2906 7224  ..rB...r....).r$
+00006720: 0000 0072 2500 0000 7226 0000 0072 4400  ...r%...r&...rD.
+00006730: 0000 722e 0000 00da 0457 6974 6829 02da  ..r......With)..
+00006740: 0977 6974 6869 7465 6d73 7242 0000 0072  .withitemsrB...r
+00006750: 0900 0000 7209 0000 0072 0a00 0000 722c  ....r....r....r,
+00006760: 0100 00fc 0300 0073 1000 0000 0a01 0801  .......s........
+00006770: 0a02 0801 0802 0604 0401 06ff 722c 0100  ............r,..
+00006780: 00e9 ffff ffff 6303 0000 0000 0000 0000  ......c.........
+00006790: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+000067a0: 3800 0000 7c01 6401 6b03 7306 7c02 720a  8...|.d.k.s.|.r.
+000067b0: 7400 6402 8301 8201 7401 7c00 7402 6a03  t.d.....t.|.t.j.
+000067c0: 8302 7314 7400 6403 8301 8201 7402 6a04  ..s.t.d.....t.j.
+000067d0: 7c00 7c01 7c02 6404 8d03 5300 2905 4e72  |.|.|.d...S.).Nr
+000067e0: 2e01 0000 7a2c 636f 6e76 6572 7369 6f6e  ....z,conversion
+000067f0: 2061 6e64 2066 6f72 6d61 745f 7370 6563   and format_spec
+00006800: 206e 6f74 2073 7570 706f 7274 6564 2079   not supported y
+00006810: 6574 7a23 466f 726d 6174 7465 6456 616c  etz#FormattedVal
+00006820: 7565 2076 616c 7565 206d 7573 7420 6265  ue value must be
+00006830: 2061 204e 616d 65a9 0372 3a00 0000 da0a   a Name..r:.....
+00006840: 636f 6e76 6572 7369 6f6e da0b 666f 726d  conversion..form
+00006850: 6174 5f73 7065 6329 0572 3800 0000 7224  at_spec).r8...r$
+00006860: 0000 0072 2e00 0000 7237 0000 00da 0e46  ...r....r7.....F
+00006870: 6f72 6d61 7474 6564 5661 6c75 6572 2f01  ormattedValuer/.
+00006880: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00006890: 0072 3201 0000 0a04 0000 730a 0000 000c  .r2.......s.....
+000068a0: 0108 010c 0108 0110 0172 3201 0000 6301  .........r2...c.
+000068b0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+000068c0: 0000 0043 0000 0073 3000 0000 7c00 4400  ...C...s0...|.D.
+000068d0: 5d0f 7d01 7400 7c01 7401 6a02 7401 6a03  ].}.t.|.t.j.t.j.
+000068e0: 6602 8302 7311 7404 6401 8301 8201 7102  f...s.t.d.....q.
+000068f0: 7405 6a06 7c00 6402 8d01 5300 2903 4e7a  t.j.|.d...S.).Nz
+00006900: 334a 6f69 6e65 6453 7472 2076 616c 7565  3JoinedStr value
+00006910: 7320 6d75 7374 2062 6520 436f 6e73 7461  s must be Consta
+00006920: 6e74 206f 7220 466f 726d 6174 7465 6456  nt or FormattedV
+00006930: 616c 7565 2901 7274 0000 0029 0772 2400  alue).rt...).r$.
+00006940: 0000 72b5 0000 0072 3500 0000 7232 0100  ..r....r5...r2..
+00006950: 0072 2600 0000 722e 0000 00da 094a 6f69  .r&...r......Joi
+00006960: 6e65 6453 7472 2902 7274 0000 0072 3a00  nedStr).rt...r:.
+00006970: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00006980: 0072 3301 0000 1204 0000 730a 0000 0008  .r3.......s.....
+00006990: 0112 0108 0102 ff0c 0272 3301 0000 6301  .........r3...c.
+000069a0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000069b0: 0000 0043 0000 0073 5600 0000 7c00 7400  ...C...sV...|.t.
+000069c0: 6a01 6b02 7209 7402 a003 a100 5300 7c00  j.k.r.t.....S.|.
+000069d0: 7400 6a04 6b02 7212 7402 a005 a100 5300  t.j.k.r.t.....S.
+000069e0: 7c00 7400 6a06 6b02 721b 7402 a007 a100  |.t.j.k.r.t.....
+000069f0: 5300 7c00 7400 6a08 6b02 7224 7402 a009  S.|.t.j.k.r$t...
+00006a00: a100 5300 740a 6401 a00b 7c00 a101 8301  ..S.t.d...|.....
+00006a10: 8201 2902 7a3b 4372 6561 7465 7320 4c6f  ..).z;Creates Lo
+00006a20: 6164 2c20 5374 6f72 652c 2044 656c 2c20  ad, Store, Del, 
+00006a30: 616e 6420 5061 7261 6d2c 2075 7365 6420  and Param, used 
+00006a40: 696e 2074 6865 2063 7478 206b 7761 7267  in the ctx kwarg
+00006a50: 2e7a 1e63 7478 5f74 7970 6520 7b7d 2069  .z.ctx_type {} i
+00006a60: 736e 2774 2061 2076 616c 6964 2074 7970  sn't a valid typ
+00006a70: 6529 0c72 6600 0000 7215 0000 0072 2e00  e).rf...r....r..
+00006a80: 0000 da04 4c6f 6164 7216 0000 00da 0553  ....Loadr......S
+00006a90: 746f 7265 7217 0000 00da 0344 656c 7218  torer......Delr.
+00006aa0: 0000 00da 0550 6172 616d 720c 0000 0072  .....Paramr....r
+00006ab0: 4100 0000 7232 0000 0072 0900 0000 7209  A...r2...r....r.
+00006ac0: 0000 0072 0a00 0000 724f 0000 001d 0400  ...r....rO......
+00006ad0: 0073 1200 0000 0a02 0801 0a01 0801 0a01  .s..............
+00006ae0: 0801 0a01 0801 0e01 724f 0000 0063 0100  ........rO...c..
+00006af0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00006b00: 0000 4300 0000 7320 0000 0074 006a 0174  ..C...s ...t.j.t
+00006b10: 006a 0274 006a 0374 006a 0464 019c 047d  .j.t.j.t.j.d...}
+00006b20: 017c 017c 0019 0083 0053 0029 027a 3e4d  .|.|.....S.).z>M
+00006b30: 6170 7320 6f70 6572 6174 6f72 2073 7472  aps operator str
+00006b40: 696e 6773 2066 6f72 2075 6e61 7279 206f  ings for unary o
+00006b50: 7065 7261 7469 6f6e 7320 746f 2074 6865  perations to the
+00006b60: 6972 205f 6173 7420 6e6f 6465 2e29 04fa  ir _ast node.)..
+00006b70: 012b fa01 2dda 036e 6f74 fa01 7e29 0572  .+..-..not..~).r
+00006b80: 2e00 0000 7224 0100 0072 2901 0000 72f1  ....r$...r)...r.
+00006b90: 0000 0072 d100 0000 a902 7228 0100 00da  ...r......r(....
+00006ba0: 076f 705f 6469 6374 7209 0000 0072 0900  .op_dictr....r..
+00006bb0: 0000 720a 0000 0072 2601 0000 2a04 0000  ..r....r&...*...
+00006bc0: 730c 0000 0004 0304 0104 0104 0106 fc0a  s...............
+00006bd0: 0772 2601 0000 6301 0000 0000 0000 0000  .r&...c.........
+00006be0: 0000 0002 0000 000d 0000 0043 0000 0073  ...........C...s
+00006bf0: 4000 0000 7400 6a01 7400 6a02 7400 6a03  @...t.j.t.j.t.j.
+00006c00: 7400 6a04 7400 6a05 7400 6a06 7400 6a07  t.j.t.j.t.j.t.j.
+00006c10: 7400 6a08 7400 6a09 7400 6a0a 7400 6a0b  t.j.t.j.t.j.t.j.
+00006c20: 7400 6a0c 6401 9c0c 7d01 7c01 7c00 1900  t.j.d...}.|.|...
+00006c30: 8300 5300 2902 7a3f 4d61 7073 206f 7065  ..S.).z?Maps ope
+00006c40: 7261 746f 7220 7374 7269 6e67 7320 666f  rator strings fo
+00006c50: 7220 6269 6e61 7279 206f 7065 7261 7469  r binary operati
+00006c60: 6f6e 7320 746f 2074 6865 6972 205f 6173  ons to their _as
+00006c70: 7420 6e6f 6465 2e29 0c72 3801 0000 7239  t node.).r8...r9
+00006c80: 0100 00da 012a 7a02 2a2a fa01 2f7a 022f  .....*z.**../z./
+00006c90: 2ffa 0125 7a02 3c3c 7a02 3e3e fa01 7cfa  /..%z.<<z.>>..|.
+00006ca0: 0126 fa01 5e29 0d72 2e00 0000 725c 0000  .&..^).r....r\..
+00006cb0: 0072 1101 0000 72e6 0000 0072 0201 0000  .r....r....r....
+00006cc0: 72ac 0000 0072 b200 0000 72e3 0000 0072  r....r....r....r
+00006cd0: e000 0000 7206 0100 0072 7e00 0000 727d  ....r....r~...r}
+00006ce0: 0000 0072 7f00 0000 723c 0100 0072 0900  ...r....r<...r..
+00006cf0: 0000 7209 0000 0072 0a00 0000 7272 0000  ..r....r....rr..
+00006d00: 0036 0400 0073 1c00 0000 0403 0401 0401  .6...s..........
+00006d10: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00006d20: 0401 06f4 0a0f 7272 0000 0063 0100 0000  ......rr...c....
+00006d30: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00006d40: 4300 0000 7318 0000 0074 006a 0174 006a  C...s....t.j.t.j
+00006d50: 0264 019c 027d 017c 017c 0019 0083 0053  .d...}.|.|.....S
+00006d60: 0029 02fa 404d 6170 7320 6f70 6572 6174  .)..@Maps operat
+00006d70: 6f72 2073 7472 696e 6773 2066 6f72 2062  or strings for b
+00006d80: 6f6f 6c65 616e 206f 7065 7261 7469 6f6e  oolean operation
+00006d90: 7320 746f 2074 6865 6972 205f 6173 7420  s to their _ast 
+00006da0: 6e6f 6465 2e29 02da 0361 6e64 da02 6f72  node.)...and..or
+00006db0: 2903 722e 0000 0072 5e00 0000 7278 0000  ).r....r^...rx..
+00006dc0: 0072 3c01 0000 7209 0000 0072 0900 0000  .r<...r....r....
+00006dd0: 720a 0000 0072 7600 0000 4a04 0000 7308  r....rv...J...s.
+00006de0: 0000 0004 0304 0106 fe0a 0572 7600 0000  ...........rv...
+00006df0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00006e00: 000b 0000 0043 0000 0073 3800 0000 7400  .....C...s8...t.
+00006e10: 6a01 7400 6a02 7400 6a03 7400 6a04 7400  j.t.j.t.j.t.j.t.
+00006e20: 6a05 7400 6a06 7400 6a07 7400 6a08 7400  j.t.j.t.j.t.j.t.
+00006e30: 6a09 7400 6a0a 6401 9c0a 7d01 7c01 7c00  j.t.j.d...}.|.|.
+00006e40: 1900 8300 5300 2902 7244 0100 0029 0a7a  ....S.).rD...).z
+00006e50: 023d 3d7a 0221 3dfa 013c 7a02 3c3d fa01  .==z.!=..<z.<=..
+00006e60: 3e7a 023e 3dda 0269 737a 0669 7320 6e6f  >z.>=..isz.is no
+00006e70: 74da 0269 6e7a 066e 6f74 2069 6e29 0b72  t..inz.not in).r
+00006e80: 2e00 0000 72ad 0000 0072 f200 0000 72e1  ....r....r....r.
+00006e90: 0000 0072 e200 0000 72bb 0000 0072 bc00  ...r....r....r..
+00006ea0: 0000 72d2 0000 0072 d300 0000 72cd 0000  ..r....r....r...
+00006eb0: 0072 f300 0000 723c 0100 0072 0900 0000  .r....r<...r....
+00006ec0: 7209 0000 0072 0a00 0000 729b 0000 0054  r....r....r....T
+00006ed0: 0400 0073 1800 0000 0403 0401 0401 0401  ...s............
+00006ee0: 0401 0401 0401 0401 0401 0401 06f6 0a0d  ................
+00006ef0: 729b 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00006f00: 0000 0300 0000 0500 0000 4f00 0000 737c  ..........O...s|
+00006f10: 0000 007c 01a0 0064 0174 016a 02a1 027d  ...|...d.t.j...}
+00006f20: 027c 0073 0d74 0364 0283 0182 0174 047c  .|.s.t.d.....t.|
+00006f30: 0083 0164 036b 0272 2974 057c 0064 0419  ...d.k.r)t.|.d..
+00006f40: 0074 0683 0272 2574 076a 087c 0064 0419  .t...r%t.j.|.d..
+00006f50: 0074 097c 0283 0164 058d 0253 007c 0064  .t.|...d...S.|.d
+00006f60: 0419 0053 0074 076a 0a74 0b7c 0064 0664  ...S.t.j.t.|.d.d
+00006f70: 0785 0219 0069 007c 01a4 018e 017c 0064  .....i.|.....|.d
+00006f80: 0719 0074 097c 0283 0164 088d 0353 0029  ...t.|...d...S.)
+00006f90: 0961 ac01 0000 4279 2074 6869 7320 7765  .a....By this we
+00006fa0: 206d 6561 6e20 6569 7468 6572 2061 2073   mean either a s
+00006fb0: 696e 676c 6520 6e61 6d65 2073 7472 696e  ingle name strin
+00006fc0: 6720 6f72 206f 6e65 206f 7220 6d6f 7265  g or one or more
+00006fd0: 2041 7474 7220 6e6f 6465 732e 0a0a 2020   Attr nodes...  
+00006fe0: 5468 6973 2069 7320 7573 6564 2077 6865  This is used whe
+00006ff0: 6e65 7665 7220 7765 2068 6176 6520 7468  never we have th
+00007000: 696e 6773 206c 696b 6520 2761 2720 6f72  ings like 'a' or
+00007010: 2027 612e 6227 206f 7220 2761 2e62 2e63   'a.b' or 'a.b.c
+00007020: 272e 0a0a 2020 4172 6773 3a0a 2020 2020  '...  Args:.    
+00007030: 2a70 6172 7473 3a20 5468 6520 7061 7274  *parts: The part
+00007040: 7320 7468 6174 2073 686f 756c 6420 6265  s that should be
+00007050: 2064 6f74 2d73 6570 6172 6174 6564 2e0a   dot-separated..
+00007060: 2020 2020 2a2a 6b77 6172 6773 3a20 4f6e      **kwargs: On
+00007070: 6c79 2072 6563 6f67 6e69 7a65 6420 6b77  ly recognized kw
+00007080: 6172 6720 6973 2027 6374 785f 7479 7065  arg is 'ctx_type
+00007090: 272c 2077 6869 6368 2063 6f6e 7472 6f6c  ', which control
+000070a0: 7320 7468 650a 2020 2020 2020 6374 7820  s the.      ctx 
+000070b0: 7479 7065 206f 6620 7468 6520 6c69 7374  type of the list
+000070c0: 2e20 5365 6520 4374 7845 6e75 6d2e 0a0a  . See CtxEnum...
+000070d0: 2020 5261 6973 6573 3a0a 2020 2020 5661    Raises:.    Va
+000070e0: 6c75 6545 7272 6f72 3a20 5768 656e 206e  lueError: When n
+000070f0: 6f20 7061 7274 7320 6172 6520 7370 6563  o parts are spec
+00007100: 6966 6965 642e 0a0a 2020 5265 7475 726e  ified...  Return
+00007110: 733a 0a20 2020 2041 6e20 5f61 7374 2e4e  s:.    An _ast.N
+00007120: 616d 6520 6e6f 6465 206f 7220 5f61 7374  ame node or _ast
+00007130: 2e41 7474 7269 6275 7465 206e 6f64 650a  .Attribute node.
+00007140: 2020 7233 0000 007a 254d 7573 7420 6861    r3...z%Must ha
+00007150: 7665 2061 7420 6c65 6173 7420 6f6e 6520  ve at least one 
+00007160: 7061 7274 2073 7065 6369 6669 6564 7296  part specifiedr.
+00007170: 0000 0072 0100 0000 72f0 0000 004e 722e  ...r....r....Nr.
+00007180: 0100 0029 0372 3a00 0000 da04 6174 7472  ...).r:.....attr
+00007190: 724d 0000 0029 0c72 7500 0000 7266 0000  rM...).ru...rf..
+000071a0: 0072 1500 0000 7226 0000 0072 9900 0000  .r....r&...r....
+000071b0: 7224 0000 0072 3600 0000 722e 0000 0072  r$...r6...r....r
+000071c0: 3700 0000 724f 0000 0072 8d00 0000 728a  7...rO...r....r.
+000071d0: 0000 0029 03da 0570 6172 7473 7289 0000  ...)...partsr...
+000071e0: 0072 3300 0000 7209 0000 0072 0900 0000  .r3...r....r....
+000071f0: 720a 0000 0072 8a00 0000 6604 0000 7318  r....r....f...s.
+00007200: 0000 000e 1004 0208 010c 010e 0116 0108  ................
+00007210: 0104 0114 0106 0106 0106 fd72 8a00 0000  ...........r....
+00007220: 722d 0000 0029 0272 0900 0000 7209 0000  r-...).r....r...
+00007230: 0072 1201 0000 2903 72c3 0000 0072 c300  .r....).r....r..
+00007240: 0000 4e29 0272 2e01 0000 4e29 6672 2e00  ..N).r....N)fr..
+00007250: 0000 72b5 0000 00da 3066 756e 5f77 6974  ..r.....0fun_wit
+00007260: 685f 6173 742e 6d61 6e69 7075 6c61 7465  h_ast.manipulate
+00007270: 5f6e 6f64 652e 6765 745f 6e6f 6465 5f66  _node.get_node_f
+00007280: 726f 6d5f 696e 7075 7472 0200 0000 da09  rom_inputr......
+00007290: 4578 6365 7074 696f 6e72 0400 0000 720c  Exceptionr....r.
+000072a0: 0000 0072 0d00 0000 7266 0000 0072 2c00  ...r....rf...r,.
+000072b0: 0000 721b 0000 0072 1500 0000 7222 0000  ..r....r....r"..
+000072c0: 0072 3d00 0000 7244 0000 00da 0f4e 6f64  .r=...rD.....Nod
+000072d0: 6554 7261 6e73 666f 726d 6572 7245 0000  eTransformerrE..
+000072e0: 0072 5300 0000 725a 0000 0072 5c00 0000  .rS...rZ...r\...
+000072f0: 725e 0000 0072 6100 0000 7268 0000 0072  r^...ra...rh...r
+00007300: 7000 0000 7273 0000 0072 7700 0000 727d  p...rs...rw...r}
+00007310: 0000 0072 7e00 0000 727f 0000 0072 8000  ...r~...r....r..
+00007320: 0000 728e 0000 0072 9300 0000 729d 0000  ..r....r....r...
+00007330: 0072 a200 0000 72a6 0000 0072 a900 0000  .r....r....r....
+00007340: 72ac 0000 0072 ad00 0000 72ae 0000 0072  r....r....r....r
+00007350: b000 0000 72b2 0000 0072 b600 0000 72b9  ....r....r....r.
+00007360: 0000 0072 bb00 0000 72bc 0000 0072 be00  ...r....r....r..
+00007370: 0000 72c0 0000 0072 ca00 0000 72cd 0000  ..r....r....r...
+00007380: 0072 cf00 0000 72d1 0000 0072 d200 0000  .r....r....r....
+00007390: 72d3 0000 0072 d400 0000 72d8 0000 0072  r....r....r....r
+000073a0: dd00 0000 72e0 0000 0072 e100 0000 72e2  ....r....r....r.
+000073b0: 0000 0072 e300 0000 72e4 0000 0072 e600  ...r....r....r..
+000073c0: 0000 7230 0000 0072 3500 0000 72ef 0000  ..r0...r5...r...
+000073d0: 0072 3700 0000 72f1 0000 0072 f200 0000  .r7...r....r....
+000073e0: 72f3 0000 0072 f700 0000 7267 0000 0072  r....r....rg...r
+000073f0: 0101 0000 7278 0000 0072 3f00 0000 7202  ....rx...r?...r.
+00007400: 0100 0072 0401 0000 7206 0100 0072 0701  ...r....r....r..
+00007410: 0000 7208 0100 0072 0d01 0000 7203 0100  ..r....r....r...
+00007420: 0072 1001 0000 7211 0100 0072 1401 0000  .r....r....r....
+00007430: 7240 0000 0072 1601 0000 721c 0100 0072  r@...r....r....r
+00007440: 2001 0000 7223 0100 0072 2401 0000 7227   ...r#...r$...r'
+00007450: 0100 0072 2901 0000 722a 0100 0072 2c01  ...r)...r*...r,.
+00007460: 0000 7232 0100 0072 3301 0000 724f 0000  ..r2...r3...rO..
+00007470: 0072 2601 0000 7272 0000 0072 7600 0000  .r&...rr...rv...
+00007480: 729b 0000 0072 8a00 0000 7209 0000 0072  r....r....r....r
+00007490: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
+000074a0: 3c6d 6f64 756c 653e 0100 0000 73ce 0000  <module>....s...
+000074b0: 0008 0108 010c 0210 0310 0408 0402 0402  ................
+000074c0: 0102 0102 0102 0106 fc08 0708 100e 0608  ................
+000074d0: 1008 0812 0c08 0d18 0a08 2108 040a 0408  ..........!.....
+000074e0: 0408 1d08 1408 1408 2f08 0408 0408 0412  ......../.......
+000074f0: 0416 2e08 2108 200a 140e 1508 1a08 040a  ....!. .........
+00007500: 0408 0508 160a 050a ff08 2308 1708 040a  ..........#.....
+00007510: 0408 200a 1008 1708 0408 0408 0408 040c  .. .............
+00007520: 0408 1508 1a08 1608 0408 0408 0408 0408  ................
+00007530: 0608 040a 0408 090e 0b08 1408 0408 0408  ................
+00007540: 0408 0b08 0c08 0408 0408 050a 0408 1008  ................
+00007550: 0408 0c0a 1608 0408 0608 0614 0412 0d08  ................
+00007560: 0e10 230c 0708 0408 0408 070a 0408 080a  ..#.............
+00007570: 0e08 0808 0b08 0d08 0c08 1408 0a0c 12    ...............
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/manipulate_node/__pycache__/if_manipulator.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/manipulate_node/__pycache__/if_manipulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/manipulate_node/body_manipulator.py` & `fun_with_ast-0.1.70/fun_with_ast/manipulate_node/body_manipulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fun_with_ast.common_utils.node_tree_util import IsEmptyModule
 from fun_with_ast.get_source import GetSource
 from fun_with_ast.manipulate_node import create_node
-from fun_with_ast.manipulate_node.create_node import GetNodeFromInput
+from fun_with_ast.manipulate_node.get_node_from_input import GetNodeFromInput
 
 
 class BodyManipulator:
     """ Class for manipulating the body of a node. (the If body, orelse body, etc.)"""
     def __init__(self, body_block):
         self.body_block = body_block
     def inject_node(self,node_to_inject, index):
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/manipulate_node/create_node.py` & `fun_with_ast-0.1.70/fun_with_ast/manipulate_node/create_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import _ast
 import ast
-import re
 
+from fun_with_ast.manipulate_node.get_node_from_input import FWANodeGenerator
 
 
 class Error(Exception):
     pass
 
 
 class InvalidCtx(Error):
@@ -19,26 +19,14 @@
 
 CtxEnum = Enum(
     LOAD='load',
     STORE='store',
     DEL='delete',
     PARAM='param')
 
-def GetNodeFromInput(string, body_index = 0, get_module = False):
-    parse_result = ast.parse(string)
-    if parse_result.body and get_module == False:
-        node = parse_result.body[body_index]
-    elif parse_result.body and get_module == True:
-        node = parse_result
-    else:
-        return parse_result # empty Module
-    if isinstance(node, ast.If) and 'elif' in string:
-        node.is_elif = True if 'elif' in string else False
-    return node
-
 
 def _ToArgsWithDefaults(_args, _defaults):
     if not isinstance(_args, list):
         raise ValueError('args must be a list')
     if not isinstance(_defaults, list):
         raise ValueError('defaults must be a list')
     args = []
@@ -64,18 +52,18 @@
     if isinstance(to_wrap, int):
         return Constant(to_wrap)
     if isinstance(to_wrap, str):
         return Name(to_wrap, ctx_type=ctx_type)
     raise NotImplementedError
 
 
-def _WrapWithTuple(to_wrap, ctx_type=CtxEnum.LOAD):
-    if not isinstance(to_wrap, list):
-        raise NotImplementedError
-    return Tuple(to_wrap, ctx_type=ctx_type)
+# def _WrapWithTuple(to_wrap, ctx_type=CtxEnum.LOAD):
+#     if not isinstance(to_wrap, list):
+#         raise NotImplementedError
+#     return Tuple(to_wrap, ctx_type=ctx_type)
 
 
 def _LeftmostNodeInDotVar(node):
     while not hasattr(node, 'id'):
         if not hasattr(node, 'value'):
             return node
         node = node.value
@@ -763,16 +751,21 @@
     return _ast.Mult()
 
 
 def Arg(arg):
     return _ast.arg(arg)
 
 
-def Constant(value):
-    return _ast.Constant(value=value)
+def Constant(value, quote_type =None):
+    node = _ast.Constant(value=value)
+    if isinstance(value, str):
+        if not quote_type:
+            raise ValueError('Constant string must be provided with quote type')
+        node.default_quote = quote_type
+    return node
 
 
 def validate_id(name_id):
     if not isinstance(name_id, str):
         raise ValueError(f'python id must be a string')
     if name_id is None or name_id[0].isdigit():
         raise ValueError(f'Invalid python id: {name_id}')
@@ -816,14 +809,15 @@
 
 def Num(number):
     """Creates an _ast.Constant node."""
     if not isinstance(number, str):
         raise ValueError(f'number must be a str to support bases')
     base = _extract_base(number)
     result =  _ast.Constant(value=int(number, base))
+    result.default_quote = "'" # TODO this is not clean -- as this is not really necessary
     result.base = base
     return result
 
 
 def _extract_base(number):
     if str(number).startswith('0b'):
         base = 2
@@ -849,24 +843,29 @@
     return _ast.Pass()
 
 
 def Pow():
     return _ast.Pow()
 
 
-def Return(value):
+def Return(value, quote_type=None):
+
     if isinstance(value, int):
         value_node = Num(str(value))
     elif isinstance(value, str):
+        if quote_type is None:
+            raise ValueError('Must provite quote type when creating a Return node weith type str..')
         value_node = Str(value)
+        value_node.default_quote = quote_type
     elif isinstance(value, _ast.AST):
         return _ast.Return(value)
     else:
         raise ValueError('Invalid return value')
-    return _ast.Return(value=value_node)
+    result = _ast.Return(value=value_node)
+    return result
 
 def RShift():
     return _ast.RShift()
 
 
 def Set(*items):
     """Creates an _ast.Set node.
@@ -944,53 +943,14 @@
         self.comment = comment[1:]
 
     @property
     def source_comment(self):
         if self.comment is not None:
             return f'#{self.comment}'
 
-class SyntaxFreeLine(_ast.stmt):
-    """Class defining a new node that has no syntax (only optional comments)."""
-
-    def __init__(self, comment=None, col_offset=0, comment_indent=1):
-        super(SyntaxFreeLine, self).__init__()
-        #        if col_offset != 0:
-        #            raise ValueError('col offset must be zero')
-        self.col_offset = col_offset
-        self._fields = ['full_line']
-        self.comment = comment
-        self.comment_indent = comment_indent
-
-    @property
-    def full_line(self):
-        if self.comment is not None:
-            return '{}#{}{}'.format(' ' * self.col_offset,
-                                    ' ' * self.comment_indent,
-                                    self.comment)
-        return ''
-
-    @classmethod
-    def MatchesStart(cls, text):
-        is_syntax_free_line = re.match('^([ \t]*)(?:|(#)([ \t]*)(.*))\n', text)
-        return is_syntax_free_line
-
-    def SetFromSrcLine(self, line):
-        match = self.MatchesStart(line)
-        if not match:
-            raise ValueError('line {} is not a valid SyntaxFreeLine'.format(line))
-        self.col_offset = len(match.group(1))
-        self.comment_indent = 0
-        self.comment = None
-        if match.group(2):
-            self.comment = ''
-            if match.group(3):
-                self.comment_indent = len(match.group(3))
-            if match.group(4):
-                self.comment = match.group(4)
-
 
 def Tuple(items, **kwargs):
     """Creates an _ast.Tuple node.
 
   Automatically adjusts inner ctx attrs.
 
   Args:
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/manipulate_node/if_manipulator.py` & `fun_with_ast-0.1.70/fun_with_ast/manipulate_node/if_manipulator.py`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/base_placeholder.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/base_placeholder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/composite.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/composite.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 09:52:44 2023 UTC, .py size: 2925 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,205 @@
-00000000: 6f0d 0d0a 0000 0000 6c6b 9564 6d0b 0000  o.......lk.dm...
+00000000: 6f0d 0d0a 0000 0000 632a b064 6d0c 0000  o.......c*.dm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
-00000070: 6504 8303 5a09 4700 6408 6409 8400 6409  e...Z.G.d.d...d.
-00000080: 6509 8303 5a0a 6401 5300 290a e900 0000  e...Z.d.S.).....
-00000090: 004e 2901 da1b 4261 646c 7953 7065 6369  .N)...BadlySpeci
-000000a0: 6669 6564 5465 6d70 6c61 7465 4572 726f  fiedTemplateErro
-000000b0: 7229 01da 0b50 6c61 6365 686f 6c64 6572  r)...Placeholder
-000000c0: 2901 da0c 5374 7269 6e67 5061 7273 6572  )...StringParser
-000000d0: 2901 da0f 4e6f 6465 506c 6163 6568 6f6c  )...NodePlacehol
-000000e0: 6465 7263 0000 0000 0000 0000 0000 0000  derc............
-000000f0: 0000 0000 0200 0000 4000 0000 7330 0000  ........@...s0..
-00000100: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
-00000110: 0384 005a 0464 0464 0584 005a 0564 0664  ...Z.d.d...Z.d.d
-00000120: 0784 005a 0664 0864 0984 005a 0764 0a53  ...Z.d.d...Z.d.S
-00000130: 0029 0bda 1443 6f6d 706f 7369 7465 506c  .)...CompositePl
-00000140: 6163 6568 6f6c 6465 727a 294e 6f64 6520  aceholderz)Node 
-00000150: 7768 6963 6820 7772 6170 7320 6f6e 6520  which wraps one 
-00000160: 6f72 206d 6f72 6520 6f74 6865 7220 6e6f  or more other no
-00000170: 6465 732e 6303 0000 0000 0000 0000 0000  des.c...........
-00000180: 0005 0000 0005 0000 0043 0000 0073 3800  .........C...s8.
-00000190: 0000 7c00 a000 7c01 a101 0100 7c00 a001  ..|...|.....|...
-000001a0: 7c01 a101 7d03 7c00 a002 7c03 7c01 a102  |...}.|...|.|...
-000001b0: 7d03 7403 7c02 7c03 7c00 6a04 6401 8d03  }.t.|.|.|.j.d...
-000001c0: 7d04 7c04 a005 a100 5300 2902 7a2f 4d61  }.|.....S.).z/Ma
-000001d0: 6b65 7320 7375 7265 206e 6f64 652e 2873  kes sure node.(s
-000001e0: 656c 662e 6669 656c 645f 6e61 6d65 2920  elf.field_name) 
-000001f0: 6973 2069 6e20 7374 7269 6e67 2e29 01da  is in string.)..
-00000200: 0f73 7461 7274 696e 675f 7061 7265 6e73  .starting_parens
-00000210: 2906 da08 5661 6c69 6461 7465 da0b 4765  )...Validate..Ge
-00000220: 7445 6c65 6d65 6e74 73da 0c5f 7365 745f  tElements.._set_
-00000230: 7061 7265 6e74 7372 0400 0000 7207 0000  parentsr....r...
-00000240: 00da 0e47 6574 4d61 7463 6865 6454 6578  ...GetMatchedTex
-00000250: 7429 05da 0473 656c 66da 046e 6f64 65da  t)...self..node.
-00000260: 0673 7472 696e 67da 0865 6c65 6d65 6e74  .string..element
-00000270: 73da 0670 6172 7365 72a9 0072 1100 0000  s..parser..r....
-00000280: fa3e 2f68 6f6d 652f 7368 6169 2f66 756e  .>/home/shai/fun
-00000290: 5f77 6974 685f 6173 742f 6675 6e5f 7769  _with_ast/fun_wi
-000002a0: 7468 5f61 7374 2f70 6c61 6365 686f 6c64  th_ast/placehold
-000002b0: 6572 732f 636f 6d70 6f73 6974 652e 7079  ers/composite.py
-000002c0: da06 5f6d 6174 6368 0d00 0000 730e 0000  .._match....s...
-000002d0: 000a 020a 010c 0102 0108 0106 ff08 027a  ...............z
-000002e0: 1b43 6f6d 706f 7369 7465 506c 6163 6568  .CompositePlaceh
-000002f0: 6f6c 6465 722e 5f6d 6174 6368 6303 0000  older._matchc...
-00000300: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00000310: 0043 0000 0073 1400 0000 7c01 4400 5d05  .C...s....|.D.].
-00000320: 7d03 7c02 7c03 5f00 7102 7c01 5300 a901  }.|.|._.q.|.S...
-00000330: 4e29 01da 0670 6172 656e 7429 0472 0c00  N)...parent).r..
-00000340: 0000 720f 0000 0072 0d00 0000 da07 656c  ..r....r......el
-00000350: 656d 656e 7472 1100 0000 7211 0000 0072  ementr....r....r
-00000360: 1200 0000 720a 0000 0016 0000 0073 0600  ....r........s..
-00000370: 0000 0801 0801 0401 7a21 436f 6d70 6f73  ........z!Compos
-00000380: 6974 6550 6c61 6365 686f 6c64 6572 2e5f  itePlaceholder._
-00000390: 7365 745f 7061 7265 6e74 7363 0200 0000  set_parentsc....
-000003a0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-000003b0: 4300 0000 7326 0000 0064 017d 027c 00a0  C...s&...d.}.|..
-000003c0: 007c 01a1 0144 005d 097d 037c 027c 03a0  .|...D.].}.|.|..
-000003d0: 017c 01a1 0137 007d 0271 077c 0253 0029  .|...7.}.q.|.S.)
-000003e0: 024e da00 2902 7209 0000 00da 0947 6574  .N..).r......Get
-000003f0: 536f 7572 6365 2904 720c 0000 0072 0d00  Source).r....r..
-00000400: 0000 da06 736f 7572 6365 7216 0000 0072  ....sourcer....r
-00000410: 1100 0000 7211 0000 0072 1200 0000 7218  ....r....r....r.
-00000420: 0000 001b 0000 0073 0800 0000 0401 0e01  .......s........
-00000430: 1001 0401 7a1e 436f 6d70 6f73 6974 6550  ....z.CompositeP
-00000440: 6c61 6365 686f 6c64 6572 2e47 6574 536f  laceholder.GetSo
-00000450: 7572 6365 6302 0000 0000 0000 0000 0000  urcec...........
-00000460: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
-00000470: 0000 6401 5300 2902 4e54 7211 0000 0029  ..d.S.).NTr....)
-00000480: 0272 0c00 0000 da0b 756e 7573 6564 5f6e  .r......unused_n
-00000490: 6f64 6572 1100 0000 7211 0000 0072 1200  oder....r....r..
-000004a0: 0000 7208 0000 0020 0000 0073 0200 0000  ..r.... ...s....
-000004b0: 0401 7a1d 436f 6d70 6f73 6974 6550 6c61  ..z.CompositePla
-000004c0: 6365 686f 6c64 6572 2e56 616c 6964 6174  ceholder.Validat
-000004d0: 654e 2908 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
-000004e0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000004f0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000500: 5f72 1300 0000 720a 0000 0072 1800 0000  _r....r....r....
-00000510: 7208 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000520: 1100 0000 7212 0000 0072 0600 0000 0900  ....r....r......
-00000530: 0000 730c 0000 0008 0004 0208 0208 0908  ..s.............
-00000540: 050c 0572 0600 0000 6300 0000 0000 0000  ...r....c.......
-00000550: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-00000560: 0073 4800 0000 6500 5a01 6400 5a02 6401  .sH...e.Z.d.Z.d.
-00000570: 5a03 0902 640d 8700 6601 6403 6404 8409  Z...d...f.d.d...
-00000580: 5a04 6405 6406 8400 5a05 8700 6601 6407  Z.d.d...Z...f.d.
-00000590: 6408 8408 5a06 6409 640a 8400 5a07 640b  d...Z.d.d...Z.d.
-000005a0: 640c 8400 5a08 8700 0400 5a09 5300 290e  d...Z.....Z.S.).
-000005b0: da10 4669 656c 6450 6c61 6365 686f 6c64  ..FieldPlacehold
-000005c0: 6572 7a18 506c 6163 6568 6f6c 6465 7220  erz.Placeholder 
-000005d0: 666f 7220 6120 6669 656c 642e 4e63 0300  for a field.Nc..
-000005e0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-000005f0: 0000 0300 0000 731e 0000 0074 0074 017c  ......s....t.t.|
-00000600: 0083 02a0 02a1 0001 007c 017c 005f 037c  .........|.|._.|
-00000610: 027c 005f 0464 0053 0072 1400 0000 2905  .|._.d.S.r....).
-00000620: da05 7375 7065 7272 1f00 0000 da08 5f5f  ..superr......__
-00000630: 696e 6974 5f5f da0a 6669 656c 645f 6e61  init__..field_na
-00000640: 6d65 da12 6265 666f 7265 5f70 6c61 6365  me..before_place
-00000650: 686f 6c64 6572 2903 720c 0000 0072 2200  holder).r....r".
-00000660: 0000 7223 0000 00a9 01da 095f 5f63 6c61  ..r#.......__cla
-00000670: 7373 5f5f 7211 0000 0072 1200 0000 7221  ss__r....r....r!
-00000680: 0000 0027 0000 0073 0600 0000 0e02 0601  ...'...s........
-00000690: 0a01 7a19 4669 656c 6450 6c61 6365 686f  ..z.FieldPlaceho
-000006a0: 6c64 6572 2e5f 5f69 6e69 745f 5f63 0200  lder.__init__c..
-000006b0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-000006c0: 0000 4300 0000 736a 0000 0074 007c 0174  ..C...sj...t.|.t
-000006d0: 016a 0283 0272 137c 006a 0364 016b 0272  .j...r.|.j.d.k.r
-000006e0: 1374 047c 017c 006a 0364 0083 037d 026e  .t.|.|.j.d...}.n
-000006f0: 0674 047c 017c 006a 0383 027d 027c 0273  .t.|.|.j...}.|.s
-00000700: 217c 0264 026b 0372 2167 0053 0067 007d  !|.d.k.r!g.S.g.}
-00000710: 037c 006a 0572 2c7c 03a0 067c 006a 05a1  .|.j.r,|...|.j..
-00000720: 0101 007c 03a0 0674 077c 0283 01a1 0101  ...|...t.|......
-00000730: 007c 0353 0029 034e da06 6b77 6172 6773  .|.S.).N..kwargs
-00000740: 7201 0000 0029 08da 0a69 7369 6e73 7461  r....)...isinsta
-00000750: 6e63 65da 045f 6173 74da 0443 616c 6c72  nce.._ast..Callr
-00000760: 2200 0000 da07 6765 7461 7474 7272 2300  ".....getattrr#.
-00000770: 0000 da06 6170 7065 6e64 7205 0000 0029  ....appendr....)
-00000780: 0472 0c00 0000 720d 0000 00da 0b66 6965  .r....r......fie
-00000790: 6c64 5f76 616c 7565 720f 0000 0072 1100  ld_valuer....r..
-000007a0: 0000 7211 0000 0072 1200 0000 7209 0000  ..r....r....r...
-000007b0: 002d 0000 0073 1400 0000 1601 1001 0c07  .-...s..........
-000007c0: 0c02 0401 0404 0601 0c01 0e01 0401 7a1c  ..............z.
-000007d0: 4669 656c 6450 6c61 6365 686f 6c64 6572  FieldPlaceholder
-000007e0: 2e47 6574 456c 656d 656e 7473 6303 0000  .GetElementsc...
-000007f0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000800: 0003 0000 0073 1200 0000 7400 7401 7c00  .....s....t.t.|.
-00000810: 8302 a002 7c01 7c02 a102 5300 7214 0000  ....|.|...S.r...
-00000820: 0029 0372 2000 0000 721f 0000 0072 1300  .).r ...r....r..
-00000830: 0000 2903 720c 0000 0072 0d00 0000 720e  ..).r....r....r.
-00000840: 0000 0072 2400 0000 7211 0000 0072 1200  ...r$...r....r..
-00000850: 0000 7213 0000 0043 0000 0073 0200 0000  ..r....C...s....
-00000860: 1201 7a17 4669 656c 6450 6c61 6365 686f  ..z.FieldPlaceho
-00000870: 6c64 6572 2e5f 6d61 7463 6863 0200 0000  lder._matchc....
-00000880: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000890: 4300 0000 7356 0000 0074 007c 0174 016a  C...sV...t.|.t.j
-000008a0: 0283 0272 137c 006a 0364 016b 0272 1374  ...r.|.j.d.k.r.t
-000008b0: 047c 017c 006a 0364 0083 037d 026e 0674  .|.|.j.d...}.n.t
-000008c0: 047c 017c 006a 0383 027d 0274 007c 0274  .|.|.j...}.t.|.t
-000008d0: 0574 0666 0283 0272 2974 0764 02a0 087c  .t.f...r)t.d...|
-000008e0: 006a 037c 01a1 0283 0182 0164 0053 0029  .j.|.......d.S.)
-000008f0: 034e 7226 0000 007a 5d46 6965 6c64 207b  .Nr&...z]Field {
-00000900: 7d20 6f66 206e 6f64 6520 7b7d 2069 7320  } of node {} is 
-00000910: 6120 6c69 7374 2e20 706c 6561 7365 2075  a list. please u
-00000920: 7365 2061 204c 6973 7446 6965 6c64 506c  se a ListFieldPl
-00000930: 6163 6568 6f6c 6465 7269 6e73 7465 6164  aceholderinstead
-00000940: 206f 6620 6120 4669 656c 6450 6c61 6365   of a FieldPlace
-00000950: 686f 6c64 6572 2909 7227 0000 0072 2800  holder).r'...r(.
-00000960: 0000 7229 0000 0072 2200 0000 722a 0000  ..r)...r"...r*..
-00000970: 00da 046c 6973 74da 0574 7570 6c65 7202  ...list..tupler.
-00000980: 0000 00da 0666 6f72 6d61 7429 0372 0c00  .....format).r..
-00000990: 0000 720d 0000 0072 2c00 0000 7211 0000  ..r....r,...r...
-000009a0: 0072 1100 0000 7212 0000 0072 0800 0000  .r....r....r....
-000009b0: 4600 0000 7312 0000 0016 0110 010c 020e  F...s...........
-000009c0: 0102 0102 010a 0104 fe04 ff7a 1946 6965  ...........z.Fie
-000009d0: 6c64 506c 6163 6568 6f6c 6465 722e 5661  ldPlaceholder.Va
-000009e0: 6c69 6461 7465 6301 0000 0000 0000 0000  lidatec.........
-000009f0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000a00: 0c00 0000 6401 a000 7c00 6a01 a101 5300  ....d...|.j...S.
-00000a10: 2902 4e7a 1f46 6965 6c64 506c 6163 6568  ).Nz.FieldPlaceh
-00000a20: 6f6c 6465 7220 666f 7220 6669 656c 6420  older for field 
-00000a30: 227b 7d22 2902 722f 0000 0072 2200 0000  "{}").r/...r"...
-00000a40: 2901 720c 0000 0072 1100 0000 7211 0000  ).r....r....r...
-00000a50: 0072 1200 0000 da08 5f5f 7265 7072 5f5f  .r......__repr__
-00000a60: 5000 0000 7306 0000 0004 0104 0104 ff7a  P...s..........z
-00000a70: 1946 6965 6c64 506c 6163 6568 6f6c 6465  .FieldPlaceholde
-00000a80: 722e 5f5f 7265 7072 5f5f 7214 0000 0029  r.__repr__r....)
-00000a90: 0a72 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000aa0: 721e 0000 0072 2100 0000 7209 0000 0072  r....r!...r....r
-00000ab0: 1300 0000 7208 0000 0072 3000 0000 da0d  ....r....r0.....
-00000ac0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1100  __classcell__r..
-00000ad0: 0000 7211 0000 0072 2400 0000 7212 0000  ..r....r$...r...
-00000ae0: 0072 1f00 0000 2400 0000 7310 0000 0008  .r....$...s.....
-00000af0: 0004 0102 030e ff08 060c 1608 0310 0a72  ...............r
-00000b00: 1f00 0000 290b 7228 0000 00da 2766 756e  ....).r(....'fun
-00000b10: 5f77 6974 685f 6173 742e 736f 7572 6365  _with_ast.source
-00000b20: 5f6d 6174 6368 6572 732e 6578 6365 7074  _matchers.except
-00000b30: 696f 6e73 7202 0000 00da 2a66 756e 5f77  ionsr.....*fun_w
-00000b40: 6974 685f 6173 742e 706c 6163 6568 6f6c  ith_ast.placehol
-00000b50: 6465 7273 2e62 6173 655f 706c 6163 6568  ders.base_placeh
-00000b60: 6f6c 6465 7272 0300 0000 da27 6675 6e5f  olderr.....'fun_
-00000b70: 7769 7468 5f61 7374 2e70 6c61 6365 686f  with_ast.placeho
-00000b80: 6c64 6572 732e 7374 7269 6e67 5f70 6172  lders.string_par
-00000b90: 7365 7272 0400 0000 da1e 6675 6e5f 7769  serr......fun_wi
-00000ba0: 7468 5f61 7374 2e70 6c61 6365 686f 6c64  th_ast.placehold
-00000bb0: 6572 732e 6e6f 6465 7205 0000 0072 0600  ers.noder....r..
-00000bc0: 0000 721f 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00000bd0: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
-00000be0: 6475 6c65 3e01 0000 0073 0e00 0000 0800  dule>....s......
-00000bf0: 0c02 0c01 0c01 0c01 1003 141b            ............
+00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 4700  ..d.d.l.m.Z...G.
+00000070: 6406 6407 8400 6407 6505 8303 5a0a 4700  d.d...d.e...Z.G.
+00000080: 6408 6409 8400 6409 650a 8303 5a0b 6401  d.d...d.e...Z.d.
+00000090: 5300 290a e900 0000 004e 2901 da1b 4261  S.)......N)...Ba
+000000a0: 646c 7953 7065 6369 6669 6564 5465 6d70  dlySpecifiedTemp
+000000b0: 6c61 7465 4572 726f 7229 01da 0b50 6c61  lateError)...Pla
+000000c0: 6365 686f 6c64 6572 2901 da0c 5374 7269  ceholder)...Stri
+000000d0: 6e67 5061 7273 6572 2901 da0f 4e6f 6465  ngParser)...Node
+000000e0: 506c 6163 6568 6f6c 6465 7263 0000 0000  Placeholderc....
+000000f0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00000100: 4000 0000 7330 0000 0065 005a 0164 005a  @...s0...e.Z.d.Z
+00000110: 0264 015a 0364 0264 0384 005a 0464 0464  .d.Z.d.d...Z.d.d
+00000120: 0584 005a 0564 0664 0784 005a 0664 0864  ...Z.d.d...Z.d.d
+00000130: 0984 005a 0764 0a53 0029 0bda 1443 6f6d  ...Z.d.S.)...Com
+00000140: 706f 7369 7465 506c 6163 6568 6f6c 6465  positePlaceholde
+00000150: 727a 294e 6f64 6520 7768 6963 6820 7772  rz)Node which wr
+00000160: 6170 7320 6f6e 6520 6f72 206d 6f72 6520  aps one or more 
+00000170: 6f74 6865 7220 6e6f 6465 732e 6303 0000  other nodes.c...
+00000180: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+00000190: 0043 0000 0073 3800 0000 7c00 a000 7c01  .C...s8...|...|.
+000001a0: a101 0100 7c00 a001 7c01 a101 7d03 7c00  ....|...|...}.|.
+000001b0: a002 7c03 7c01 a102 7d03 7403 7c02 7c03  ..|.|...}.t.|.|.
+000001c0: 7c00 6a04 6401 8d03 7d04 7c04 a005 a100  |.j.d...}.|.....
+000001d0: 5300 2902 7a2f 4d61 6b65 7320 7375 7265  S.).z/Makes sure
+000001e0: 206e 6f64 652e 2873 656c 662e 6669 656c   node.(self.fiel
+000001f0: 645f 6e61 6d65 2920 6973 2069 6e20 7374  d_name) is in st
+00000200: 7269 6e67 2e29 01da 0f73 7461 7274 696e  ring.)...startin
+00000210: 675f 7061 7265 6e73 2906 da08 5661 6c69  g_parens)...Vali
+00000220: 6461 7465 da0b 4765 7445 6c65 6d65 6e74  date..GetElement
+00000230: 73da 0c5f 7365 745f 7061 7265 6e74 7372  s.._set_parentsr
+00000240: 0400 0000 7207 0000 00da 0e47 6574 4d61  ....r......GetMa
+00000250: 7463 6865 6454 6578 7429 05da 0473 656c  tchedText)...sel
+00000260: 66da 046e 6f64 65da 0673 7472 696e 67da  f..node..string.
+00000270: 0865 6c65 6d65 6e74 73da 0670 6172 7365  .elements..parse
+00000280: 72a9 0072 1100 0000 fa3e 2f68 6f6d 652f  r..r.....>/home/
+00000290: 7368 6169 2f66 756e 5f77 6974 685f 6173  shai/fun_with_as
+000002a0: 742f 6675 6e5f 7769 7468 5f61 7374 2f70  t/fun_with_ast/p
+000002b0: 6c61 6365 686f 6c64 6572 732f 636f 6d70  laceholders/comp
+000002c0: 6f73 6974 652e 7079 da06 5f6d 6174 6368  osite.py.._match
+000002d0: 0e00 0000 730e 0000 000a 020a 010c 0102  ....s...........
+000002e0: 0108 0106 ff08 027a 1b43 6f6d 706f 7369  .......z.Composi
+000002f0: 7465 506c 6163 6568 6f6c 6465 722e 5f6d  tePlaceholder._m
+00000300: 6174 6368 6303 0000 0000 0000 0000 0000  atchc...........
+00000310: 0004 0000 0003 0000 0043 0000 0073 3e00  .........C...s>.
+00000320: 0000 7400 7c02 7401 6a02 8302 7215 7400  ..t.|.t.j...r.t.
+00000330: 7c02 6a03 7404 8302 7315 7405 7c02 6401  |.j.t...s.t.|.d.
+00000340: 8302 7315 7406 6402 8301 8201 7c01 4400  ..s.t.d.....|.D.
+00000350: 5d05 7d03 7c02 7c03 5f07 7117 7c01 5300  ].}.|.|._.q.|.S.
+00000360: 2903 4eda 0d64 6566 6175 6c74 5f71 756f  ).N..default_quo
+00000370: 7465 7a46 436f 6e73 7461 6e74 206e 6f64  tezFConstant nod
+00000380: 6573 206d 7573 7420 6f66 2074 7970 6520  es must of type 
+00000390: 7374 7269 6e67 206d 7573 7420 6861 7665  string must have
+000003a0: 2061 2064 6566 6175 6c74 5f71 756f 7465   a default_quote
+000003b0: 2061 7474 7269 6275 7465 2908 da0a 6973   attribute)...is
+000003c0: 696e 7374 616e 6365 da03 6173 74da 0843  instance..ast..C
+000003d0: 6f6e 7374 616e 74da 0173 da03 696e 74da  onstant..s..int.
+000003e0: 0768 6173 6174 7472 da0a 5661 6c75 6545  .hasattr..ValueE
+000003f0: 7272 6f72 da06 7061 7265 6e74 2904 720c  rror..parent).r.
+00000400: 0000 0072 0f00 0000 720d 0000 00da 0765  ...r....r......e
+00000410: 6c65 6d65 6e74 7211 0000 0072 1100 0000  lementr....r....
+00000420: 7212 0000 0072 0a00 0000 1700 0000 730a  r....r........s.
+00000430: 0000 0022 0108 0108 0108 0104 017a 2143  ...".........z!C
+00000440: 6f6d 706f 7369 7465 506c 6163 6568 6f6c  ompositePlacehol
+00000450: 6465 722e 5f73 6574 5f70 6172 656e 7473  der._set_parents
+00000460: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
+00000470: 0005 0000 0043 0000 0073 2a00 0000 6401  .....C...s*...d.
+00000480: 7d02 7c00 a000 7c01 a101 7d03 7c03 4400  }.|...|...}.|.D.
+00000490: 5d09 7d04 7c02 7c04 a001 7c01 a101 3700  ].}.|.|...|...7.
+000004a0: 7d02 7109 7c02 5300 2902 4eda 0029 0272  }.q.|.S.).N..).r
+000004b0: 0900 0000 da09 4765 7453 6f75 7263 6529  ......GetSource)
+000004c0: 0572 0c00 0000 720d 0000 00da 0673 6f75  .r....r......sou
+000004d0: 7263 6572 0f00 0000 721d 0000 0072 1100  rcer....r....r..
+000004e0: 0000 7211 0000 0072 1200 0000 721f 0000  ..r....r....r...
+000004f0: 001e 0000 0073 0a00 0000 0401 0a01 0801  .....s..........
+00000500: 1001 0401 7a1e 436f 6d70 6f73 6974 6550  ....z.CompositeP
+00000510: 6c61 6365 686f 6c64 6572 2e47 6574 536f  laceholder.GetSo
+00000520: 7572 6365 6302 0000 0000 0000 0000 0000  urcec...........
+00000530: 0002 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+00000540: 0000 6401 5300 2902 4e54 7211 0000 0029  ..d.S.).NTr....)
+00000550: 0272 0c00 0000 da0b 756e 7573 6564 5f6e  .r......unused_n
+00000560: 6f64 6572 1100 0000 7211 0000 0072 1200  oder....r....r..
+00000570: 0000 7208 0000 0024 0000 0073 0200 0000  ..r....$...s....
+00000580: 0401 7a1d 436f 6d70 6f73 6974 6550 6c61  ..z.CompositePla
+00000590: 6365 686f 6c64 6572 2e56 616c 6964 6174  ceholder.Validat
+000005a0: 654e 2908 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
+000005b0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000005c0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+000005d0: 5f72 1300 0000 720a 0000 0072 1f00 0000  _r....r....r....
+000005e0: 7208 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+000005f0: 1100 0000 7212 0000 0072 0600 0000 0a00  ....r....r......
+00000600: 0000 730c 0000 0008 0004 0208 0208 0908  ..s.............
+00000610: 070c 0672 0600 0000 6300 0000 0000 0000  ...r....c.......
+00000620: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00000630: 0073 4800 0000 6500 5a01 6400 5a02 6401  .sH...e.Z.d.Z.d.
+00000640: 5a03 0902 640d 8700 6601 6403 6404 8409  Z...d...f.d.d...
+00000650: 5a04 6405 6406 8400 5a05 8700 6601 6407  Z.d.d...Z...f.d.
+00000660: 6408 8408 5a06 6409 640a 8400 5a07 640b  d...Z.d.d...Z.d.
+00000670: 640c 8400 5a08 8700 0400 5a09 5300 290e  d...Z.....Z.S.).
+00000680: da10 4669 656c 6450 6c61 6365 686f 6c64  ..FieldPlacehold
+00000690: 6572 7a18 506c 6163 6568 6f6c 6465 7220  erz.Placeholder 
+000006a0: 666f 7220 6120 6669 656c 642e 4e63 0300  for a field.Nc..
+000006b0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000006c0: 0000 0300 0000 731e 0000 0074 0074 017c  ......s....t.t.|
+000006d0: 0083 02a0 02a1 0001 007c 017c 005f 037c  .........|.|._.|
+000006e0: 027c 005f 0464 0053 00a9 014e 2905 da05  .|._.d.S...N)...
+000006f0: 7375 7065 7272 2600 0000 da08 5f5f 696e  superr&.....__in
+00000700: 6974 5f5f da0a 6669 656c 645f 6e61 6d65  it__..field_name
+00000710: da12 6265 666f 7265 5f70 6c61 6365 686f  ..before_placeho
+00000720: 6c64 6572 2903 720c 0000 0072 2a00 0000  lder).r....r*...
+00000730: 722b 0000 00a9 01da 095f 5f63 6c61 7373  r+.......__class
+00000740: 5f5f 7211 0000 0072 1200 0000 7229 0000  __r....r....r)..
+00000750: 002b 0000 0073 0600 0000 0e02 0601 0a01  .+...s..........
+00000760: 7a19 4669 656c 6450 6c61 6365 686f 6c64  z.FieldPlacehold
+00000770: 6572 2e5f 5f69 6e69 745f 5f63 0200 0000  er.__init__c....
+00000780: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000790: 4300 0000 736a 0000 0074 007c 0174 016a  C...sj...t.|.t.j
+000007a0: 0283 0272 137c 006a 0364 016b 0272 1374  ...r.|.j.d.k.r.t
+000007b0: 047c 017c 006a 0364 0083 037d 026e 0674  .|.|.j.d...}.n.t
+000007c0: 047c 017c 006a 0383 027d 027c 0273 217c  .|.|.j...}.|.s!|
+000007d0: 0264 026b 0372 2167 0053 0067 007d 037c  .d.k.r!g.S.g.}.|
+000007e0: 006a 0572 2c7c 03a0 067c 006a 05a1 0101  .j.r,|...|.j....
+000007f0: 007c 03a0 0674 077c 0283 01a1 0101 007c  .|...t.|.......|
+00000800: 0353 0029 034e da06 6b77 6172 6773 7201  .S.).N..kwargsr.
+00000810: 0000 0029 0872 1500 0000 da04 5f61 7374  ...).r......_ast
+00000820: da04 4361 6c6c 722a 0000 00da 0767 6574  ..Callr*.....get
+00000830: 6174 7472 722b 0000 00da 0661 7070 656e  attrr+.....appen
+00000840: 6472 0500 0000 2904 720c 0000 0072 0d00  dr....).r....r..
+00000850: 0000 da0b 6669 656c 645f 7661 6c75 6572  ....field_valuer
+00000860: 0f00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00000870: 0000 0072 0900 0000 3100 0000 7314 0000  ...r....1...s...
+00000880: 0016 0110 010c 070c 0204 0104 0406 010c  ................
+00000890: 010e 0104 017a 1c46 6965 6c64 506c 6163  .....z.FieldPlac
+000008a0: 6568 6f6c 6465 722e 4765 7445 6c65 6d65  eholder.GetEleme
+000008b0: 6e74 7363 0300 0000 0000 0000 0000 0000  ntsc............
+000008c0: 0300 0000 0400 0000 0300 0000 7312 0000  ............s...
+000008d0: 0074 0074 017c 0083 02a0 027c 017c 02a1  .t.t.|.....|.|..
+000008e0: 0253 0072 2700 0000 2903 7228 0000 0072  .S.r'...).r(...r
+000008f0: 2600 0000 7213 0000 0029 0372 0c00 0000  &...r....).r....
+00000900: 720d 0000 0072 0e00 0000 722c 0000 0072  r....r....r,...r
+00000910: 1100 0000 7212 0000 0072 1300 0000 4700  ....r....r....G.
+00000920: 0000 7302 0000 0012 017a 1746 6965 6c64  ..s......z.Field
+00000930: 506c 6163 6568 6f6c 6465 722e 5f6d 6174  Placeholder._mat
+00000940: 6368 6302 0000 0000 0000 0000 0000 0003  chc.............
+00000950: 0000 0005 0000 0043 0000 0073 5600 0000  .......C...sV...
+00000960: 7400 7c01 7401 6a02 8302 7213 7c00 6a03  t.|.t.j...r.|.j.
+00000970: 6401 6b02 7213 7404 7c01 7c00 6a03 6400  d.k.r.t.|.|.j.d.
+00000980: 8303 7d02 6e06 7404 7c01 7c00 6a03 8302  ..}.n.t.|.|.j...
+00000990: 7d02 7400 7c02 7405 7406 6602 8302 7229  }.t.|.t.t.f...r)
+000009a0: 7407 6402 a008 7c00 6a03 7c01 a102 8301  t.d...|.j.|.....
+000009b0: 8201 6400 5300 2903 4e72 2e00 0000 7a5d  ..d.S.).Nr....z]
+000009c0: 4669 656c 6420 7b7d 206f 6620 6e6f 6465  Field {} of node
+000009d0: 207b 7d20 6973 2061 206c 6973 742e 2070   {} is a list. p
+000009e0: 6c65 6173 6520 7573 6520 6120 4c69 7374  lease use a List
+000009f0: 4669 656c 6450 6c61 6365 686f 6c64 6572  FieldPlaceholder
+00000a00: 696e 7374 6561 6420 6f66 2061 2046 6965  instead of a Fie
+00000a10: 6c64 506c 6163 6568 6f6c 6465 7229 0972  ldPlaceholder).r
+00000a20: 1500 0000 722f 0000 0072 3000 0000 722a  ....r/...r0...r*
+00000a30: 0000 0072 3100 0000 da04 6c69 7374 da05  ...r1.....list..
+00000a40: 7475 706c 6572 0200 0000 da06 666f 726d  tupler......form
+00000a50: 6174 2903 720c 0000 0072 0d00 0000 7233  at).r....r....r3
+00000a60: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00000a70: 0000 7208 0000 004a 0000 0073 1200 0000  ..r....J...s....
+00000a80: 1601 1001 0c02 0e01 0201 0201 0a01 04fe  ................
+00000a90: 04ff 7a19 4669 656c 6450 6c61 6365 686f  ..z.FieldPlaceho
+00000aa0: 6c64 6572 2e56 616c 6964 6174 6563 0100  lder.Validatec..
+00000ab0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000ac0: 0000 4300 0000 730c 0000 0064 01a0 007c  ..C...s....d...|
+00000ad0: 006a 01a1 0153 0029 024e 7a1f 4669 656c  .j...S.).Nz.Fiel
+00000ae0: 6450 6c61 6365 686f 6c64 6572 2066 6f72  dPlaceholder for
+00000af0: 2066 6965 6c64 2022 7b7d 2229 0272 3600   field "{}").r6.
+00000b00: 0000 722a 0000 0029 0172 0c00 0000 7211  ..r*...).r....r.
+00000b10: 0000 0072 1100 0000 7212 0000 00da 085f  ...r....r......_
+00000b20: 5f72 6570 725f 5f54 0000 0073 0600 0000  _repr__T...s....
+00000b30: 0401 0401 04ff 7a19 4669 656c 6450 6c61  ......z.FieldPla
+00000b40: 6365 686f 6c64 6572 2e5f 5f72 6570 725f  ceholder.__repr_
+00000b50: 5f72 2700 0000 290a 7222 0000 0072 2300  _r'...).r"...r#.
+00000b60: 0000 7224 0000 0072 2500 0000 7229 0000  ..r$...r%...r)..
+00000b70: 0072 0900 0000 7213 0000 0072 0800 0000  .r....r....r....
+00000b80: 7237 0000 00da 0d5f 5f63 6c61 7373 6365  r7.....__classce
+00000b90: 6c6c 5f5f 7211 0000 0072 1100 0000 722c  ll__r....r....r,
+00000ba0: 0000 0072 1200 0000 7226 0000 0028 0000  ...r....r&...(..
+00000bb0: 0073 1000 0000 0800 0401 0203 0eff 0806  .s..............
+00000bc0: 0c16 0803 100a 7226 0000 0029 0c72 2f00  ......r&...).r/.
+00000bd0: 0000 7216 0000 00da 2766 756e 5f77 6974  ..r.....'fun_wit
+00000be0: 685f 6173 742e 736f 7572 6365 5f6d 6174  h_ast.source_mat
+00000bf0: 6368 6572 732e 6578 6365 7074 696f 6e73  chers.exceptions
+00000c00: 7202 0000 00da 2a66 756e 5f77 6974 685f  r.....*fun_with_
+00000c10: 6173 742e 706c 6163 6568 6f6c 6465 7273  ast.placeholders
+00000c20: 2e62 6173 655f 706c 6163 6568 6f6c 6465  .base_placeholde
+00000c30: 7272 0300 0000 da27 6675 6e5f 7769 7468  rr.....'fun_with
+00000c40: 5f61 7374 2e70 6c61 6365 686f 6c64 6572  _ast.placeholder
+00000c50: 732e 7374 7269 6e67 5f70 6172 7365 7272  s.string_parserr
+00000c60: 0400 0000 da1e 6675 6e5f 7769 7468 5f61  ......fun_with_a
+00000c70: 7374 2e70 6c61 6365 686f 6c64 6572 732e  st.placeholders.
+00000c80: 6e6f 6465 7205 0000 0072 0600 0000 7226  noder....r....r&
+00000c90: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
+00000ca0: 0000 7212 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000cb0: 3e01 0000 0073 1000 0000 0800 0801 0c02  >....s..........
+00000cc0: 0c01 0c01 0c01 1003 141e                 ..........
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/docstring.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/docstring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/list_placeholder.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/list_placeholder.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 20 15:44:20 2023 UTC, .py size: 4182 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d4ea 6864 5610 0000  o.........hdV...
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 6010 0000  o..........d`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6501 8303 5a08 4700  d.d...d.e...Z.G.
 00000070: 6407 6408 8400 6408 6508 8303 5a09 6409  d.d...d.e...Z.d.
@@ -230,20 +230,21 @@
 00000e50: 2e5f 5f69 6e69 745f 5f29 0572 3300 0000  .__init__).r3...
 00000e60: 7234 0000 0072 3500 0000 7208 0000 0072  r4...r5...r....r
 00000e70: 3700 0000 7213 0000 0072 1300 0000 7211  7...r....r....r.
 00000e80: 0000 0072 1400 0000 7238 0000 0057 0000  ...r....r8...W..
 00000e90: 0073 0400 0000 0800 1a02 7238 0000 004e  .s........r8...N
 00000ea0: 290a da23 6675 6e5f 7769 7468 5f61 7374  )..#fun_with_ast
 00000eb0: 2e70 6c61 6365 686f 6c64 6572 732e 636f  .placeholders.co
-00000ec0: 6d70 6f73 6974 6572 0200 0000 da28 6675  mpositer.....(fu
+00000ec0: 6d70 6f73 6974 6572 0200 0000 da32 6675  mpositer.....2fu
 00000ed0: 6e5f 7769 7468 5f61 7374 2e6d 616e 6970  n_with_ast.manip
-00000ee0: 756c 6174 655f 6e6f 6465 2e63 7265 6174  ulate_node.creat
-00000ef0: 655f 6e6f 6465 7203 0000 00da 2766 756e  e_noder.....'fun
-00000f00: 5f77 6974 685f 6173 742e 736f 7572 6365  _with_ast.source
-00000f10: 5f6d 6174 6368 6572 732e 6578 6365 7074  _matchers.except
-00000f20: 696f 6e73 7204 0000 00da 1e66 756e 5f77  ionsr......fun_w
-00000f30: 6974 685f 6173 742e 706c 6163 6568 6f6c  ith_ast.placehol
-00000f40: 6465 7273 2e6e 6f64 6572 0500 0000 7206  ders.noder....r.
-00000f50: 0000 0072 3800 0000 7213 0000 0072 1300  ...r8...r....r..
-00000f60: 0000 7213 0000 0072 1400 0000 da08 3c6d  ..r....r......<m
-00000f70: 6f64 756c 653e 0100 0000 730c 0000 000c  odule>....s.....
-00000f80: 000c 010c 010c 0110 0314 50              ..........P
+00000ee0: 756c 6174 655f 6e6f 6465 2e73 796e 7461  ulate_node.synta
+00000ef0: 785f 6672 6565 5f6c 696e 655f 6e6f 6465  x_free_line_node
+00000f00: 7203 0000 00da 2766 756e 5f77 6974 685f  r.....'fun_with_
+00000f10: 6173 742e 736f 7572 6365 5f6d 6174 6368  ast.source_match
+00000f20: 6572 732e 6578 6365 7074 696f 6e73 7204  ers.exceptionsr.
+00000f30: 0000 00da 1e66 756e 5f77 6974 685f 6173  .....fun_with_as
+00000f40: 742e 706c 6163 6568 6f6c 6465 7273 2e6e  t.placeholders.n
+00000f50: 6f64 6572 0500 0000 7206 0000 0072 3800  oder....r....r8.
+00000f60: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
+00000f70: 0072 1400 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000f80: 0100 0000 730c 0000 000c 000c 010c 010c  ....s...........
+00000f90: 0110 0314 50                             ....P
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/node.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/string_parser.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/string_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul  1 08:33:13 2023 UTC, .py size: 2932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c9e4 9f64 740b 0000  o..........dt...
+00000000: 6f0d 0d0a 0000 0000 4855 a664 740b 0000  o.......HU.dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 8400 5a08 4700 6407 6408 8400 6408  d...Z.G.d.d...d.
 00000070: 6509 8303 5a0a 6409 5300 290a e900 0000  e...Z.d.S.).....
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/string_part.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/string_part.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/text.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/text.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun  5 18:39:18 2023 UTC, .py size: 3337 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,217 +1,224 @@
-00000000: 6f0d 0d0a 0000 0000 d62b 7e64 090d 0000  o........+~d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 070d 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
+00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 6504 8303 5a05 4700  d.d...d.e...Z.G.
 00000060: 6406 6407 8400 6407 6505 8303 5a06 4700  d.d...d.e...Z.G.
 00000070: 6408 6409 8400 6409 6505 8303 5a07 640a  d.d...d.e...Z.d.
-00000080: 640b 8400 5a08 6401 5300 290c e900 0000  d...Z.d.S.).....
-00000090: 004e 2901 da1b 4261 646c 7953 7065 6369  .N)...BadlySpeci
-000000a0: 6669 6564 5465 6d70 6c61 7465 4572 726f  fiedTemplateErro
-000000b0: 7229 01da 0b50 6c61 6365 686f 6c64 6572  r)...Placeholder
-000000c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000000d0: 0004 0000 0000 0000 0073 4c00 0000 6500  .........sL...e.
-000000e0: 5a01 6400 5a02 6401 5a03 6410 8700 6601  Z.d.Z.d.Z.d...f.
-000000f0: 6404 6405 8409 5a04 6406 6407 8400 5a05  d.d...Z.d.d...Z.
-00000100: 6411 6408 6409 8401 5a06 640a 640b 8400  d.d.d...Z.d.d...
-00000110: 5a07 640c 640d 8400 5a08 640e 640f 8400  Z.d.d...Z.d.d...
-00000120: 5a09 8700 0400 5a0a 5300 2912 da0f 5465  Z.....Z.S.)...Te
-00000130: 7874 506c 6163 6568 6f6c 6465 727a 4650  xtPlaceholderzFP
-00000140: 6c61 6365 686f 6c64 6572 2066 6f72 2074  laceholder for t
-00000150: 6578 7420 286e 6f6e 2d66 6965 6c64 292e  ext (non-field).
-00000160: 2046 6f72 2065 7861 6d70 6c65 2c20 2764   For example, 'd
-00000170: 6566 2028 2720 696e 2046 756e 6374 696f  ef (' in Functio
-00000180: 6e44 6566 2e4e 4663 0400 0000 0000 0000  nDef.NFc........
-00000190: 0000 0000 0400 0000 0300 0000 0300 0000  ................
-000001a0: 7346 0000 0074 0074 017c 0083 02a0 02a1  sF...t.t.|......
-000001b0: 0001 007c 017c 005f 037c 00a0 047c 01a1  ...|.|._.|...|..
-000001c0: 017c 005f 057c 037c 005f 067c 0264 0075  .|._.|.|._.|.d.u
-000001d0: 0072 1b7c 017c 005f 076e 037c 027c 005f  .r.|.|._.n.|.|._
-000001e0: 0764 007c 005f 0864 0053 00a9 014e 2909  .d.|._.d.S...N).
-000001f0: da05 7375 7065 7272 0400 0000 da08 5f5f  ..superr......__
-00000200: 696e 6974 5f5f da0e 6f72 6967 696e 616c  init__..original
-00000210: 5f72 6567 6578 da0f 5f54 7261 6e73 666f  _regex.._Transfo
-00000220: 726d 5265 6765 78da 0572 6567 6578 da0d  rmRegex..regex..
-00000230: 6c6f 6e67 6573 745f 6d61 7463 68da 0764  longest_match..d
-00000240: 6566 6175 6c74 da0c 6d61 7463 6865 645f  efault..matched_
-00000250: 7465 7874 2904 da04 7365 6c66 720a 0000  text)...selfr...
-00000260: 0072 0c00 0000 720b 0000 00a9 01da 095f  .r....r........_
-00000270: 5f63 6c61 7373 5f5f a900 fa39 2f68 6f6d  _class__...9/hom
-00000280: 652f 7368 6169 2f66 756e 5f77 6974 685f  e/shai/fun_with_
-00000290: 6173 742f 6675 6e5f 7769 7468 5f61 7374  ast/fun_with_ast
-000002a0: 2f70 6c61 6365 686f 6c64 6572 732f 7465  /placeholders/te
-000002b0: 7874 2e70 7972 0700 0000 0b00 0000 7310  xt.pyr........s.
-000002c0: 0000 000e 0106 010c 0206 0108 0108 0106  ................
-000002d0: 020a 017a 1854 6578 7450 6c61 6365 686f  ...z.TextPlaceho
-000002e0: 6c64 6572 2e5f 5f69 6e69 745f 5f63 0200  lder.__init__c..
-000002f0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
-00000300: 0000 4300 0000 732c 0000 007c 01a0 0064  ..C...s,...|...d
-00000310: 01a1 017d 0264 02a0 017c 02a1 017d 017c  ...}.d...|...}.|
-00000320: 01a0 0064 03a1 017d 0364 04a0 017c 03a1  ...d...}.d...|..
-00000330: 017d 017c 0153 0029 054e 7a03 5c73 2a7a  .}.|.S.).Nz.\s*z
-00000340: 125c 732a 285c 5c5c 732a 7c23 2e2a 5c73  .\s*(\\\s*|#.*\s
-00000350: 2a29 2a7a 025c 6e7a 1228 202a 232e 2a5c  *)*z.\nz.( *#.*\
-00000360: 6e7c 202a 3b7c 202a 5c6e 2929 02da 0573  n| *;| *\n))...s
-00000370: 706c 6974 da04 6a6f 696e 2904 720e 0000  plit..join).r...
-00000380: 0072 0a00 0000 da14 6e6f 6e5f 7768 6974  .r......non_whit
-00000390: 6573 7061 6365 5f70 6172 7473 da13 6e6f  espace_parts..no
-000003a0: 6e5f 6c69 6e65 6272 6561 6b5f 7061 7274  n_linebreak_part
-000003b0: 7372 1100 0000 7211 0000 0072 1200 0000  sr....r....r....
-000003c0: 7209 0000 0017 0000 0073 0a00 0000 0a01  r........s......
-000003d0: 0a01 0a02 0a01 0402 7a1f 5465 7874 506c  ........z.TextPl
-000003e0: 6163 6568 6f6c 6465 722e 5f54 7261 6e73  aceholder._Trans
-000003f0: 666f 726d 5265 6765 7863 0400 0000 0000  formRegexc......
-00000400: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
-00000410: 0000 7384 0000 0064 017d 047c 0372 0e74  ..s....d.}.|.r.t
-00000420: 00a0 017c 006a 027c 0274 006a 03a1 037d  ...|.j.|.t.j...}
-00000430: 056e 237c 006a 0472 1d74 00a0 057c 006a  .n#|.j.r.t...|.j
-00000440: 027c 02a1 027d 0674 067c 0683 017d 046e  .|...}.t.|...}.n
-00000450: 1474 00a0 017c 006a 027c 02a1 027d 057c  .t...|.j.|...}.|
-00000460: 0573 3174 0764 02a0 087c 027c 006a 097c  .s1t.d...|.|.j.|
-00000470: 006a 02a1 0383 0182 017c 0472 397c 047c  .j.......|.r9|.|
-00000480: 005f 0a7c 006a 0a53 007c 05a0 0b64 03a1  ._.|.j.S.|...d..
-00000490: 017c 005f 0a7c 006a 0a53 0029 0461 b701  .|._.|.j.S.).a..
-000004a0: 0000 4174 7465 6d70 7473 2074 6f20 6d61  ..Attempts to ma
-000004b0: 7463 6820 7374 7269 6e67 2061 6761 696e  tch string again
-000004c0: 7374 2073 656c 662e 7265 6765 782e 0a0a  st self.regex...
-000004d0: 2020 2020 2020 2020 5361 7665 7320 7468          Saves th
-000004e0: 6520 6d61 7463 6865 6420 7365 6374 696f  e matched sectio
-000004f0: 6e20 666f 7220 7573 6520 696e 2047 6574  n for use in Get
-00000500: 536f 7572 6365 2e0a 0a20 2020 2020 2020  Source...       
-00000510: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00000520: 2075 6e75 7365 645f 6e6f 6465 3a20 756e   unused_node: un
-00000530: 7573 6564 2e0a 2020 2020 2020 2020 2020  used..          
-00000540: 7374 7269 6e67 3a20 5468 6520 7374 7269  string: The stri
-00000550: 6e67 2077 6520 6174 7465 6d70 7420 746f  ng we attempt to
-00000560: 206d 6174 6368 2061 2073 7562 7374 7269   match a substri
-00000570: 6e67 206f 662e 0a20 2020 2020 2020 2020  ng of..         
-00000580: 2064 6f74 616c 6c3a 2057 6865 7468 6572   dotall: Whether
-00000590: 2074 6f20 6170 706c 7920 7265 2e44 4f54   to apply re.DOT
-000005a0: 414c 4c20 746f 2074 6865 206d 6174 6368  ALL to the match
-000005b0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-000005c0: 733a 0a20 2020 2020 2020 2020 2042 6164  s:.          Bad
-000005d0: 6c79 5370 6563 6966 6965 6454 656d 706c  lySpecifiedTempl
-000005e0: 6174 6545 7272 6f72 3a20 4966 2074 6865  ateError: If the
-000005f0: 2072 6567 6578 2064 6f65 736e 2774 206d   regex doesn't m
-00000600: 6174 6368 2061 6e79 7768 6572 652e 0a0a  atch anywhere...
-00000610: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00000620: 0a20 2020 2020 2020 2020 2054 6865 2073  .          The s
-00000630: 7562 7374 7269 6e67 206f 6620 7374 7269  ubstring of stri
-00000640: 6e67 2074 6861 7420 6d61 7463 6865 732e  ng that matches.
-00000650: 0a20 2020 2020 2020 204e 7a39 7374 7269  .        Nz9stri
-00000660: 6e67 2022 7b7d 2220 646f 6573 206e 6f74  ng "{}" does not
-00000670: 206d 6174 6368 2072 6567 6578 2022 7b7d   match regex "{}
-00000680: 2220 2874 6563 686e 6963 616c 6c79 2c20  " (technically, 
-00000690: 227b 7d22 2972 0100 0000 290c da02 7265  "{}")r....)...re
-000006a0: da05 6d61 7463 6872 0a00 0000 da06 444f  ..matchr......DO
-000006b0: 5441 4c4c 720b 0000 00da 0766 696e 6461  TALLr......finda
-000006c0: 6c6c da03 6d61 7872 0200 0000 da06 666f  ll..maxr......fo
-000006d0: 726d 6174 7208 0000 0072 0d00 0000 da05  rmatr....r......
-000006e0: 6772 6f75 7029 0772 0e00 0000 da0b 756e  group).r......un
-000006f0: 7573 6564 5f6e 6f64 65da 0673 7472 696e  used_node..strin
-00000700: 67da 0664 6f74 616c 6cda 156c 6f6e 6765  g..dotall..longe
-00000710: 7374 5f6d 6174 6368 5f61 7474 656d 7074  st_match_attempt
-00000720: da0d 6d61 7463 685f 6174 7465 6d70 74da  ..match_attempt.
-00000730: 0b61 6c6c 5f6d 6174 6368 6573 7211 0000  .all_matchesr...
-00000740: 0072 1100 0000 7212 0000 00da 065f 6d61  .r....r......_ma
-00000750: 7463 6820 0000 0073 2200 0000 0410 0401  tch ...s".......
-00000760: 1401 0601 0e01 0a01 0e02 0401 0201 0201  ................
-00000770: 0e01 04fe 0403 0601 0603 0cff 0601 7a16  ..............z.
-00000780: 5465 7874 506c 6163 6568 6f6c 6465 722e  TextPlaceholder.
-00000790: 5f6d 6174 6368 6302 0000 0000 0000 0000  _matchc.........
-000007a0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-000007b0: 1600 0000 7c00 6a00 6401 7500 7208 7c00  ....|.j.d.u.r.|.
-000007c0: 6a01 5300 7c00 6a00 5300 2902 7a42 5265  j.S.|.j.S.).zBRe
-000007d0: 7475 726e 7320 7365 6c66 2e6d 6174 6368  turns self.match
-000007e0: 6564 5f74 6578 7420 6966 2069 7420 6578  ed_text if it ex
-000007f0: 6973 7473 2c20 6f72 2073 656c 662e 6465  ists, or self.de
-00000800: 6661 756c 7420 6f74 6865 7277 6973 652e  fault otherwise.
-00000810: 4e29 0272 0d00 0000 720c 0000 0029 0272  N).r....r....).r
-00000820: 0e00 0000 721e 0000 0072 1100 0000 7211  ....r....r....r.
-00000830: 0000 0072 1200 0000 da09 4765 7453 6f75  ...r......GetSou
-00000840: 7263 6542 0000 0073 0600 0000 0a02 0601  rceB...s........
-00000850: 0601 7a19 5465 7874 506c 6163 6568 6f6c  ..z.TextPlacehol
-00000860: 6465 722e 4765 7453 6f75 7263 6563 0100  der.GetSourcec..
-00000870: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000880: 0000 4300 0000 730e 0000 0074 007c 006a  ..C...s....t.|.j
-00000890: 017c 006a 0283 0253 0072 0500 0000 2903  .|.j...S.r....).
-000008a0: 7204 0000 0072 0a00 0000 720c 0000 00a9  r....r....r.....
-000008b0: 0172 0e00 0000 7211 0000 0072 1100 0000  .r....r....r....
-000008c0: 7212 0000 00da 0443 6f70 7948 0000 0073  r......CopyH...s
-000008d0: 0200 0000 0e01 7a14 5465 7874 506c 6163  ......z.TextPlac
-000008e0: 6568 6f6c 6465 722e 436f 7079 6301 0000  eholder.Copyc...
-000008f0: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00000900: 0043 0000 0073 1400 0000 6401 a000 7c00  .C...s....d...|.
-00000910: 6a01 7c00 6a02 7c00 6a03 a103 5300 2902  j.|.j.|.j...S.).
-00000920: 4e7a 3754 6578 7450 6c61 6365 686f 6c64  Nz7TextPlacehold
-00000930: 6572 2077 6974 6820 7265 6765 7820 227b  er with regex "{
-00000940: 7d22 2028 227b 7d22 2920 616e 6420 6465  }" ("{}") and de
-00000950: 6661 756c 7420 227b 7d22 2904 721c 0000  fault "{}").r...
-00000960: 0072 0800 0000 720a 0000 0072 0c00 0000  .r....r....r....
-00000970: 7226 0000 0072 1100 0000 7211 0000 0072  r&...r....r....r
-00000980: 1200 0000 da08 5f5f 7265 7072 5f5f 4b00  ......__repr__K.
-00000990: 0000 7306 0000 0004 010c 0104 ff7a 1854  ..s..........z.T
-000009a0: 6578 7450 6c61 6365 686f 6c64 6572 2e5f  extPlaceholder._
-000009b0: 5f72 6570 725f 5f29 024e 4629 0146 290b  _repr__).NF).F).
-000009c0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000009d0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000009e0: 6d65 5f5f da07 5f5f 646f 635f 5f72 0700  me__..__doc__r..
-000009f0: 0000 7209 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
-00000a00: 0072 2700 0000 7228 0000 00da 0d5f 5f63  .r'...r(.....__c
-00000a10: 6c61 7373 6365 6c6c 5f5f 7211 0000 0072  lasscell__r....r
-00000a20: 1100 0000 720f 0000 0072 1200 0000 7204  ....r....r....r.
-00000a30: 0000 0008 0000 0073 1000 0000 0800 0401  .......s........
-00000a40: 0e02 080c 0a09 0822 0806 1003 7204 0000  ......."....r...
-00000a50: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000a60: 0000 0300 0000 0000 0000 f31c 0000 0065  ...............e
-00000a70: 005a 0164 005a 0287 0066 0164 0164 0284  .Z.d.Z...f.d.d..
-00000a80: 085a 0387 0004 005a 0453 0029 03da 1153  .Z.....Z.S.)...S
-00000a90: 7461 7274 5061 7265 6e4d 6174 6368 6572  tartParenMatcher
-00000aa0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000ab0: 0004 0000 0003 0000 00f3 1600 0000 7400  ..............t.
-00000ac0: 7401 7c00 8302 a002 6401 6402 a102 0100  t.|.....d.d.....
-00000ad0: 6400 5300 2903 4e7a 0b5b 205c 745d 2a5c  d.S.).Nz.[ \t]*\
-00000ae0: 285c 732a da00 2903 7206 0000 0072 2f00  (\s*..).r....r/.
-00000af0: 0000 7207 0000 0072 2600 0000 720f 0000  ..r....r&...r...
-00000b00: 0072 1100 0000 7212 0000 0072 0700 0000  .r....r....r....
-00000b10: 5000 0000 f302 0000 0016 017a 1a53 7461  P..........z.Sta
-00000b20: 7274 5061 7265 6e4d 6174 6368 6572 2e5f  rtParenMatcher._
-00000b30: 5f69 6e69 745f 5fa9 0572 2900 0000 722a  _init__..r)...r*
-00000b40: 0000 0072 2b00 0000 7207 0000 0072 2d00  ...r+...r....r-.
-00000b50: 0000 7211 0000 0072 1100 0000 720f 0000  ..r....r....r...
-00000b60: 0072 1200 0000 722f 0000 004f 0000 00f3  .r....r/...O....
-00000b70: 0400 0000 0800 1401 722f 0000 0063 0000  ........r/...c..
-00000b80: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000b90: 0000 0000 0000 722e 0000 0029 03da 0f45  ......r....)...E
-00000ba0: 6e64 5061 7265 6e4d 6174 6368 6572 6301  ndParenMatcherc.
-00000bb0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000bc0: 0000 0003 0000 0072 3000 0000 2903 4e7a  .......r0...).Nz
-00000bd0: 0d5b 5c73 5d2a 5c29 5b20 5c74 5d2a 7231  .[\s]*\)[ \t]*r1
-00000be0: 0000 0029 0372 0600 0000 7235 0000 0072  ...).r....r5...r
-00000bf0: 0700 0000 7226 0000 0072 0f00 0000 7211  ....r&...r....r.
-00000c00: 0000 0072 1200 0000 7207 0000 0053 0000  ...r....r....S..
-00000c10: 0072 3200 0000 7a18 456e 6450 6172 656e  .r2...z.EndParen
-00000c20: 4d61 7463 6865 722e 5f5f 696e 6974 5f5f  Matcher.__init__
-00000c30: 7233 0000 0072 1100 0000 7211 0000 0072  r3...r....r....r
-00000c40: 0f00 0000 7212 0000 0072 3500 0000 5200  ....r....r5...R.
-00000c50: 0000 7234 0000 0072 3500 0000 6300 0000  ..r4...r5...c...
-00000c60: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000c70: 0043 0000 0073 0a00 0000 7400 6401 6402  .C...s....t.d.d.
-00000c80: 8302 5300 2903 4e7a 065b 205c 745d 2a72  ..S.).Nz.[ \t]*r
-00000c90: 3100 0000 2901 7204 0000 0072 1100 0000  1...).r....r....
-00000ca0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000cb0: 1447 6574 5768 6974 6553 7061 6365 4d61  .GetWhiteSpaceMa
-00000cc0: 7463 6865 725a 0000 0073 0200 0000 0a01  tcherZ...s......
-00000cd0: 7236 0000 0029 0972 1700 0000 da27 6675  r6...).r.....'fu
-00000ce0: 6e5f 7769 7468 5f61 7374 2e73 6f75 7263  n_with_ast.sourc
-00000cf0: 655f 6d61 7463 6865 7273 2e65 7863 6570  e_matchers.excep
-00000d00: 7469 6f6e 7372 0200 0000 da2a 6675 6e5f  tionsr.....*fun_
-00000d10: 7769 7468 5f61 7374 2e70 6c61 6365 686f  with_ast.placeho
-00000d20: 6c64 6572 732e 6261 7365 5f70 6c61 6365  lders.base_place
-00000d30: 686f 6c64 6572 7203 0000 0072 0400 0000  holderr....r....
-00000d40: 722f 0000 0072 3500 0000 7236 0000 0072  r/...r5...r6...r
-00000d50: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000d60: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000d70: 0073 0e00 0000 0800 0c03 0c01 1003 1047  .s.............G
-00000d80: 1003 0c08                                ....
+00000080: 640b 8400 5a08 640c 640d 8400 5a09 6401  d...Z.d.d...Z.d.
+00000090: 5300 290e e900 0000 004e 2901 da1b 4261  S.)......N)...Ba
+000000a0: 646c 7953 7065 6369 6669 6564 5465 6d70  dlySpecifiedTemp
+000000b0: 6c61 7465 4572 726f 7229 01da 0b50 6c61  lateError)...Pla
+000000c0: 6365 686f 6c64 6572 6300 0000 0000 0000  ceholderc.......
+000000d0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+000000e0: 0073 4c00 0000 6500 5a01 6400 5a02 6401  .sL...e.Z.d.Z.d.
+000000f0: 5a03 6410 8700 6601 6404 6405 8409 5a04  Z.d...f.d.d...Z.
+00000100: 6406 6407 8400 5a05 6411 6408 6409 8401  d.d...Z.d.d.d...
+00000110: 5a06 640a 640b 8400 5a07 640c 640d 8400  Z.d.d...Z.d.d...
+00000120: 5a08 640e 640f 8400 5a09 8700 0400 5a0a  Z.d.d...Z.....Z.
+00000130: 5300 2912 da0f 5465 7874 506c 6163 6568  S.)...TextPlaceh
+00000140: 6f6c 6465 727a 4650 6c61 6365 686f 6c64  olderzFPlacehold
+00000150: 6572 2066 6f72 2074 6578 7420 286e 6f6e  er for text (non
+00000160: 2d66 6965 6c64 292e 2046 6f72 2065 7861  -field). For exa
+00000170: 6d70 6c65 2c20 2764 6566 2028 2720 696e  mple, 'def (' in
+00000180: 2046 756e 6374 696f 6e44 6566 2e4e 4663   FunctionDef.NFc
+00000190: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+000001a0: 0300 0000 0300 0000 7346 0000 0074 0074  ........sF...t.t
+000001b0: 017c 0083 02a0 02a1 0001 007c 017c 005f  .|.........|.|._
+000001c0: 037c 00a0 047c 01a1 017c 005f 057c 037c  .|...|...|._.|.|
+000001d0: 005f 067c 0264 0075 0072 1b7c 017c 005f  ._.|.d.u.r.|.|._
+000001e0: 076e 037c 027c 005f 0764 007c 005f 0864  .n.|.|._.d.|._.d
+000001f0: 0053 00a9 014e 2909 da05 7375 7065 7272  .S...N)...superr
+00000200: 0400 0000 da08 5f5f 696e 6974 5f5f da0e  ......__init__..
+00000210: 6f72 6967 696e 616c 5f72 6567 6578 da0f  original_regex..
+00000220: 5f54 7261 6e73 666f 726d 5265 6765 78da  _TransformRegex.
+00000230: 0572 6567 6578 da0d 6c6f 6e67 6573 745f  .regex..longest_
+00000240: 6d61 7463 68da 0764 6566 6175 6c74 da0c  match..default..
+00000250: 6d61 7463 6865 645f 7465 7874 2904 da04  matched_text)...
+00000260: 7365 6c66 720a 0000 0072 0c00 0000 720b  selfr....r....r.
+00000270: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+00000280: a900 fa39 2f68 6f6d 652f 7368 6169 2f66  ...9/home/shai/f
+00000290: 756e 5f77 6974 685f 6173 742f 6675 6e5f  un_with_ast/fun_
+000002a0: 7769 7468 5f61 7374 2f70 6c61 6365 686f  with_ast/placeho
+000002b0: 6c64 6572 732f 7465 7874 2e70 7972 0700  lders/text.pyr..
+000002c0: 0000 0b00 0000 7310 0000 000e 0106 010c  ......s.........
+000002d0: 0206 0108 0108 0106 020a 017a 1854 6578  ...........z.Tex
+000002e0: 7450 6c61 6365 686f 6c64 6572 2e5f 5f69  tPlaceholder.__i
+000002f0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
+00000300: 0000 0400 0000 0300 0000 4300 0000 732c  ..........C...s,
+00000310: 0000 007c 01a0 0064 01a1 017d 0264 02a0  ...|...d...}.d..
+00000320: 017c 02a1 017d 017c 01a0 0064 03a1 017d  .|...}.|...d...}
+00000330: 0364 04a0 017c 03a1 017d 017c 0153 0029  .d...|...}.|.S.)
+00000340: 054e 7a03 5c73 2a7a 125c 732a 285c 5c5c  .Nz.\s*z.\s*(\\\
+00000350: 732a 7c23 2e2a 5c73 2a29 2a7a 025c 6e7a  s*|#.*\s*)*z.\nz
+00000360: 1228 202a 232e 2a5c 6e7c 202a 3b7c 202a  .( *#.*\n| *;| *
+00000370: 5c6e 2929 02da 0573 706c 6974 da04 6a6f  \n))...split..jo
+00000380: 696e 2904 720e 0000 0072 0a00 0000 da14  in).r....r......
+00000390: 6e6f 6e5f 7768 6974 6573 7061 6365 5f70  non_whitespace_p
+000003a0: 6172 7473 da13 6e6f 6e5f 6c69 6e65 6272  arts..non_linebr
+000003b0: 6561 6b5f 7061 7274 7372 1100 0000 7211  eak_partsr....r.
+000003c0: 0000 0072 1200 0000 7209 0000 0017 0000  ...r....r.......
+000003d0: 0073 0a00 0000 0a01 0a01 0a02 0a01 0402  .s..............
+000003e0: 7a1f 5465 7874 506c 6163 6568 6f6c 6465  z.TextPlaceholde
+000003f0: 722e 5f54 7261 6e73 666f 726d 5265 6765  r._TransformRege
+00000400: 7863 0400 0000 0000 0000 0000 0000 0700  xc..............
+00000410: 0000 0600 0000 4300 0000 7384 0000 0064  ......C...s....d
+00000420: 017d 047c 0372 0e74 00a0 017c 006a 027c  .}.|.r.t...|.j.|
+00000430: 0274 006a 03a1 037d 056e 237c 006a 0472  .t.j...}.n#|.j.r
+00000440: 1d74 00a0 057c 006a 027c 02a1 027d 0674  .t...|.j.|...}.t
+00000450: 067c 0683 017d 046e 1474 00a0 017c 006a  .|...}.n.t...|.j
+00000460: 027c 02a1 027d 057c 0573 3174 0764 02a0  .|...}.|.s1t.d..
+00000470: 087c 027c 006a 097c 006a 02a1 0383 0182  .|.|.j.|.j......
+00000480: 017c 0472 397c 047c 005f 0a7c 006a 0a53  .|.r9|.|._.|.j.S
+00000490: 007c 05a0 0b64 03a1 017c 005f 0a7c 006a  .|...d...|._.|.j
+000004a0: 0a53 0029 0461 b701 0000 4174 7465 6d70  .S.).a....Attemp
+000004b0: 7473 2074 6f20 6d61 7463 6820 7374 7269  ts to match stri
+000004c0: 6e67 2061 6761 696e 7374 2073 656c 662e  ng against self.
+000004d0: 7265 6765 782e 0a0a 2020 2020 2020 2020  regex...        
+000004e0: 5361 7665 7320 7468 6520 6d61 7463 6865  Saves the matche
+000004f0: 6420 7365 6374 696f 6e20 666f 7220 7573  d section for us
+00000500: 6520 696e 2047 6574 536f 7572 6365 2e0a  e in GetSource..
+00000510: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00000520: 2020 2020 2020 2020 2075 6e75 7365 645f           unused_
+00000530: 6e6f 6465 3a20 756e 7573 6564 2e0a 2020  node: unused..  
+00000540: 2020 2020 2020 2020 7374 7269 6e67 3a20          string: 
+00000550: 5468 6520 7374 7269 6e67 2077 6520 6174  The string we at
+00000560: 7465 6d70 7420 746f 206d 6174 6368 2061  tempt to match a
+00000570: 2073 7562 7374 7269 6e67 206f 662e 0a20   substring of.. 
+00000580: 2020 2020 2020 2020 2064 6f74 616c 6c3a           dotall:
+00000590: 2057 6865 7468 6572 2074 6f20 6170 706c   Whether to appl
+000005a0: 7920 7265 2e44 4f54 414c 4c20 746f 2074  y re.DOTALL to t
+000005b0: 6865 206d 6174 6368 2e0a 0a20 2020 2020  he match...     
+000005c0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+000005d0: 2020 2020 2042 6164 6c79 5370 6563 6966       BadlySpecif
+000005e0: 6965 6454 656d 706c 6174 6545 7272 6f72  iedTemplateError
+000005f0: 3a20 4966 2074 6865 2072 6567 6578 2064  : If the regex d
+00000600: 6f65 736e 2774 206d 6174 6368 2061 6e79  oesn't match any
+00000610: 7768 6572 652e 0a0a 2020 2020 2020 2020  where...        
+00000620: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00000630: 2020 2054 6865 2073 7562 7374 7269 6e67     The substring
+00000640: 206f 6620 7374 7269 6e67 2074 6861 7420   of string that 
+00000650: 6d61 7463 6865 732e 0a20 2020 2020 2020  matches..       
+00000660: 204e 7a39 7374 7269 6e67 2022 7b7d 2220   Nz9string "{}" 
+00000670: 646f 6573 206e 6f74 206d 6174 6368 2072  does not match r
+00000680: 6567 6578 2022 7b7d 2220 2874 6563 686e  egex "{}" (techn
+00000690: 6963 616c 6c79 2c20 227b 7d22 2972 0100  ically, "{}")r..
+000006a0: 0000 290c da02 7265 da05 6d61 7463 6872  ..)...re..matchr
+000006b0: 0a00 0000 da06 444f 5441 4c4c 720b 0000  ......DOTALLr...
+000006c0: 00da 0766 696e 6461 6c6c da03 6d61 7872  ...findall..maxr
+000006d0: 0200 0000 da06 666f 726d 6174 7208 0000  ......formatr...
+000006e0: 0072 0d00 0000 da05 6772 6f75 7029 0772  .r......group).r
+000006f0: 0e00 0000 da0b 756e 7573 6564 5f6e 6f64  ......unused_nod
+00000700: 65da 0673 7472 696e 67da 0664 6f74 616c  e..string..dotal
+00000710: 6cda 156c 6f6e 6765 7374 5f6d 6174 6368  l..longest_match
+00000720: 5f61 7474 656d 7074 da0d 6d61 7463 685f  _attempt..match_
+00000730: 6174 7465 6d70 74da 0b61 6c6c 5f6d 6174  attempt..all_mat
+00000740: 6368 6573 7211 0000 0072 1100 0000 7212  chesr....r....r.
+00000750: 0000 00da 065f 6d61 7463 6820 0000 0073  ....._match ...s
+00000760: 2200 0000 0410 0401 1401 0601 0e01 0a01  "...............
+00000770: 0e02 0401 0201 0201 0e01 04fe 0403 0601  ................
+00000780: 0603 0cff 0601 7a16 5465 7874 506c 6163  ......z.TextPlac
+00000790: 6568 6f6c 6465 722e 5f6d 6174 6368 6302  eholder._matchc.
+000007a0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+000007b0: 0000 0043 0000 0073 1600 0000 7c00 6a00  ...C...s....|.j.
+000007c0: 6401 7500 7208 7c00 6a01 5300 7c00 6a00  d.u.r.|.j.S.|.j.
+000007d0: 5300 2902 7a42 5265 7475 726e 7320 7365  S.).zBReturns se
+000007e0: 6c66 2e6d 6174 6368 6564 5f74 6578 7420  lf.matched_text 
+000007f0: 6966 2069 7420 6578 6973 7473 2c20 6f72  if it exists, or
+00000800: 2073 656c 662e 6465 6661 756c 7420 6f74   self.default ot
+00000810: 6865 7277 6973 652e 4e29 0272 0d00 0000  herwise.N).r....
+00000820: 720c 0000 0029 0272 0e00 0000 721e 0000  r....).r....r...
+00000830: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000840: da09 4765 7453 6f75 7263 6542 0000 0073  ..GetSourceB...s
+00000850: 0600 0000 0a02 0601 0601 7a19 5465 7874  ..........z.Text
+00000860: 506c 6163 6568 6f6c 6465 722e 4765 7453  Placeholder.GetS
+00000870: 6f75 7263 6563 0100 0000 0000 0000 0000  ourcec..........
+00000880: 0000 0100 0000 0300 0000 4300 0000 730e  ..........C...s.
+00000890: 0000 0074 007c 006a 017c 006a 0283 0253  ...t.|.j.|.j...S
+000008a0: 0072 0500 0000 2903 7204 0000 0072 0a00  .r....).r....r..
+000008b0: 0000 720c 0000 00a9 0172 0e00 0000 7211  ..r......r....r.
+000008c0: 0000 0072 1100 0000 7212 0000 00da 0443  ...r....r......C
+000008d0: 6f70 7948 0000 0073 0200 0000 0e01 7a14  opyH...s......z.
+000008e0: 5465 7874 506c 6163 6568 6f6c 6465 722e  TextPlaceholder.
+000008f0: 436f 7079 6301 0000 0000 0000 0000 0000  Copyc...........
+00000900: 0001 0000 0005 0000 0043 0000 0073 1400  .........C...s..
+00000910: 0000 6401 a000 7c00 6a01 7c00 6a02 7c00  ..d...|.j.|.j.|.
+00000920: 6a03 a103 5300 2902 4e7a 3754 6578 7450  j...S.).Nz7TextP
+00000930: 6c61 6365 686f 6c64 6572 2077 6974 6820  laceholder with 
+00000940: 7265 6765 7820 227b 7d22 2028 227b 7d22  regex "{}" ("{}"
+00000950: 2920 616e 6420 6465 6661 756c 7420 227b  ) and default "{
+00000960: 7d22 2904 721c 0000 0072 0800 0000 720a  }").r....r....r.
+00000970: 0000 0072 0c00 0000 7226 0000 0072 1100  ...r....r&...r..
+00000980: 0000 7211 0000 0072 1200 0000 da08 5f5f  ..r....r......__
+00000990: 7265 7072 5f5f 4b00 0000 7306 0000 0004  repr__K...s.....
+000009a0: 010c 0104 ff7a 1854 6578 7450 6c61 6365  .....z.TextPlace
+000009b0: 686f 6c64 6572 2e5f 5f72 6570 725f 5f29  holder.__repr__)
+000009c0: 024e 4629 0146 290b da08 5f5f 6e61 6d65  .NF).F)...__name
+000009d0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000009e0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+000009f0: 646f 635f 5f72 0700 0000 7209 0000 0072  doc__r....r....r
+00000a00: 2400 0000 7225 0000 0072 2700 0000 7228  $...r%...r'...r(
+00000a10: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00000a20: 5f5f 7211 0000 0072 1100 0000 720f 0000  __r....r....r...
+00000a30: 0072 1200 0000 7204 0000 0008 0000 0073  .r....r........s
+00000a40: 1000 0000 0800 0401 0e02 080c 0a09 0822  ..............."
+00000a50: 0806 1003 7204 0000 0063 0000 0000 0000  ....r....c......
+00000a60: 0000 0000 0000 0000 0000 0300 0000 0000  ................
+00000a70: 0000 f31c 0000 0065 005a 0164 005a 0287  .......e.Z.d.Z..
+00000a80: 0066 0164 0164 0284 085a 0387 0004 005a  .f.d.d...Z.....Z
+00000a90: 0453 0029 03da 1153 7461 7274 5061 7265  .S.)...StartPare
+00000aa0: 6e4d 6174 6368 6572 6301 0000 0000 0000  nMatcherc.......
+00000ab0: 0000 0000 0001 0000 0004 0000 0003 0000  ................
+00000ac0: 00f3 1600 0000 7400 7401 7c00 8302 a002  ......t.t.|.....
+00000ad0: 6401 6402 a102 0100 6400 5300 a903 4e7a  d.d.....d.S...Nz
+00000ae0: 0b5b 205c 745d 2a5c 285c 732a da00 2903  .[ \t]*\(\s*..).
+00000af0: 7206 0000 0072 2f00 0000 7207 0000 0072  r....r/...r....r
+00000b00: 2600 0000 720f 0000 0072 1100 0000 7212  &...r....r....r.
+00000b10: 0000 0072 0700 0000 5000 0000 f302 0000  ...r....P.......
+00000b20: 0016 017a 1a53 7461 7274 5061 7265 6e4d  ...z.StartParenM
+00000b30: 6174 6368 6572 2e5f 5f69 6e69 745f 5fa9  atcher.__init__.
+00000b40: 0572 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
+00000b50: 7207 0000 0072 2d00 0000 7211 0000 0072  r....r-...r....r
+00000b60: 1100 0000 720f 0000 0072 1200 0000 722f  ....r....r....r/
+00000b70: 0000 004f 0000 00f3 0400 0000 0800 1401  ...O............
+00000b80: 722f 0000 0063 0000 0000 0000 0000 0000  r/...c..........
+00000b90: 0000 0000 0000 0300 0000 0000 0000 722e  ..............r.
+00000ba0: 0000 0029 03da 0f45 6e64 5061 7265 6e4d  ...)...EndParenM
+00000bb0: 6174 6368 6572 6301 0000 0000 0000 0000  atcherc.........
+00000bc0: 0000 0001 0000 0004 0000 0003 0000 0072  ...............r
+00000bd0: 3000 0000 2903 4e7a 0d5b 5c73 5d2a 5c29  0...).Nz.[\s]*\)
+00000be0: 5b20 5c74 5d2a 7232 0000 0029 0372 0600  [ \t]*r2...).r..
+00000bf0: 0000 7236 0000 0072 0700 0000 7226 0000  ..r6...r....r&..
+00000c00: 0072 0f00 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000c10: 7207 0000 0053 0000 0072 3300 0000 7a18  r....S...r3...z.
+00000c20: 456e 6450 6172 656e 4d61 7463 6865 722e  EndParenMatcher.
+00000c30: 5f5f 696e 6974 5f5f 7234 0000 0072 1100  __init__r4...r..
+00000c40: 0000 7211 0000 0072 0f00 0000 7212 0000  ..r....r....r...
+00000c50: 0072 3600 0000 5200 0000 7235 0000 0072  .r6...R...r5...r
+00000c60: 3600 0000 6300 0000 0000 0000 0000 0000  6...c...........
+00000c70: 0000 0000 0003 0000 0043 0000 00f3 0a00  .........C......
+00000c80: 0000 7400 6401 6402 8302 5300 7231 0000  ..t.d.d...S.r1..
+00000c90: 00a9 0172 0400 0000 7211 0000 0072 1100  ...r....r....r..
+00000ca0: 0000 7211 0000 0072 1200 0000 da14 4765  ..r....r......Ge
+00000cb0: 7453 7461 7274 5061 7265 6e4d 6174 6368  tStartParenMatch
+00000cc0: 6572 5700 0000 f302 0000 000a 0172 3900  erW..........r9.
+00000cd0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000ce0: 0000 0003 0000 0043 0000 0072 3700 0000  .......C...r7...
+00000cf0: 2903 4e7a 065b 205c 745d 2a72 3200 0000  ).Nz.[ \t]*r2...
+00000d00: 7238 0000 0072 1100 0000 7211 0000 0072  r8...r....r....r
+00000d10: 1100 0000 7212 0000 00da 1447 6574 5768  ....r......GetWh
+00000d20: 6974 6553 7061 6365 4d61 7463 6865 725a  iteSpaceMatcherZ
+00000d30: 0000 0072 3a00 0000 723b 0000 0029 0a72  ...r:...r;...).r
+00000d40: 1700 0000 da27 6675 6e5f 7769 7468 5f61  .....'fun_with_a
+00000d50: 7374 2e73 6f75 7263 655f 6d61 7463 6865  st.source_matche
+00000d60: 7273 2e65 7863 6570 7469 6f6e 7372 0200  rs.exceptionsr..
+00000d70: 0000 da2a 6675 6e5f 7769 7468 5f61 7374  ...*fun_with_ast
+00000d80: 2e70 6c61 6365 686f 6c64 6572 732e 6261  .placeholders.ba
+00000d90: 7365 5f70 6c61 6365 686f 6c64 6572 7203  se_placeholderr.
+00000da0: 0000 0072 0400 0000 722f 0000 0072 3600  ...r....r/...r6.
+00000db0: 0000 7239 0000 0072 3b00 0000 7211 0000  ..r9...r;...r...
+00000dc0: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000dd0: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
+00000de0: 0000 0008 000c 030c 0110 0310 4710 0308  ............G...
+00000df0: 050c 03                                  ...
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/__pycache__/whitespace.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/__pycache__/whitespace.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/composite.py` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/composite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import _ast
+import ast
 
 from fun_with_ast.source_matchers.exceptions import BadlySpecifiedTemplateError
 from fun_with_ast.placeholders.base_placeholder import Placeholder
 from fun_with_ast.placeholders.string_parser import StringParser
 from fun_with_ast.placeholders.node import NodePlaceholder
 
 
@@ -16,21 +17,24 @@
         elements = self.GetElements(node)
         elements = self._set_parents(elements, node)
         parser = StringParser(
             string, elements, starting_parens=self.starting_parens)
         return parser.GetMatchedText()
 
     def _set_parents(self, elements, node):
+        if isinstance(node, ast.Constant) and not isinstance(node.s, int) and not hasattr(node, 'default_quote'):
+            raise ValueError('Constant nodes must of type string must have a default_quote attribute')
         for element in elements:
             element.parent = node
         return elements
 
     def GetSource(self, node):
         source = ''
-        for element in self.GetElements(node):
+        elements = self.GetElements(node)
+        for element in elements:
             source += element.GetSource(node)
         return source
     def Validate(self, unused_node):
         return True
 
 
 class FieldPlaceholder(CompositePlaceholder):
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/list_placeholder.py` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/list_placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fun_with_ast.placeholders.composite import CompositePlaceholder
-from fun_with_ast.manipulate_node.create_node import SyntaxFreeLine
+from fun_with_ast.manipulate_node.syntax_free_line_node import SyntaxFreeLine
 from fun_with_ast.source_matchers.exceptions import BadlySpecifiedTemplateError
 from fun_with_ast.placeholders.node import NodePlaceholder
 
 
 class ListFieldPlaceholder(CompositePlaceholder):
     """Placeholder for a field which is a list of child nodes."""
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/node.py` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/node.py`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/string_parser.py` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/string_parser.py`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/string_part.py` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/string_part.py`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/placeholders/text.py` & `fun_with_ast-0.1.70/fun_with_ast/placeholders/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
     def  __init__(self):
         super(StartParenMatcher, self).__init__(r'[ \t]*\(\s*', '')
 class EndParenMatcher(TextPlaceholder):
     def  __init__(self):
         super(EndParenMatcher, self).__init__(r'[\s]*\)[ \t]*', '')
 
 
-#def GetStartParenMatcher():
-#    return TextPlaceholder(r'[ \t]*\(\s*', '')
+def GetStartParenMatcher():
+    return TextPlaceholder(r'[ \t]*\(\s*', '')
 
 def GetWhiteSpaceMatcher():
     return TextPlaceholder(r'[ \t]*', '')
 
 
 #def GetEndParenMatcher():
 #    return TextPlaceholder(r'[\s]*\)[ \t]*', '')
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_match.py` & `fun_with_ast-0.1.70/fun_with_ast/source_match.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from fun_with_ast.source_matchers.body import BodyPlaceholder
 from fun_with_ast.source_matchers.defualt_matcher import DefaultSourceMatcher
 from fun_with_ast.placeholders.args import ArgsDefaultsPlaceholder, KeysValuesPlaceholder, ArgsKeywordsPlaceholder, \
     OpsComparatorsPlaceholder
 from fun_with_ast.placeholders.composite import FieldPlaceholder
 from fun_with_ast.placeholders.list_placeholder import ListFieldPlaceholder, SeparatedListFieldPlaceholder
 
-from fun_with_ast.placeholders.text import TextPlaceholder
+from fun_with_ast.placeholders.text import TextPlaceholder, GetStartParenMatcher
 
 # TODO: Consolidate with StringParser
-from fun_with_ast.source_matchers.base_matcher import MatchPlaceholder
+from fun_with_ast.placeholders.base_match import MatchPlaceholder
 from fun_with_ast.source_matchers.if_source_match import IfSourceMatcher
 from fun_with_ast.source_matchers.with_matcher import WithSourceMatcher
 from fun_with_ast.source_matchers.tuple import TupleSourceMatcher
 from fun_with_ast.source_matchers.joined_str import JoinedStrSourceMatcher
 from fun_with_ast.source_matchers.syntaxfreeline import SyntaxFreeLineMatcher
 from fun_with_ast.source_matchers.constant_source_match import ConstantSourceMatcher
 from fun_with_ast.placeholders.docstring import DocStringTextPlaceholder
@@ -164,22 +164,30 @@
 def get_Break_expected_parts():
     return [TextPlaceholder(r' *break *\n', 'break\n')]
 
 
 def get_Call_expected_parts():
     return [
         FieldPlaceholder('func'),
-        #TextPlaceholder(r'\(\s*', '('),
         ArgsKeywordsPlaceholder(
             TextPlaceholder(r'\s*,\s*', ', '),
             TextPlaceholder('')),
         FieldPlaceholder(
             'kwargs',
             before_placeholder=TextPlaceholder(r'\s*,?\s*\*\*', ', **')),
-        #TextPlaceholder(r'\s*,?\s*\)', ')'),
+    ]
+
+def get_CallArgs_expected_parts():
+    return [
+        ArgsKeywordsPlaceholder(
+            TextPlaceholder(r'\s*,\s*', ', '),
+            TextPlaceholder('')),
+        FieldPlaceholder(
+            'kwargs',
+            before_placeholder=TextPlaceholder(r'\s*,?\s*\*\*', ', **')),
     ]
 
 
 def get_ClassDef_expected_parts():
     return [
         ListFieldPlaceholder(
             'decorator_list',
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/base_matcher.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/base_matcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul  1 08:44:29 2023 UTC, .py size: 7933 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,406 +1,310 @@
-00000000: 6f0d 0d0a 0000 0000 6de7 9f64 fd1e 0000  o.......m..d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 3b12 0000  o..........d;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
-00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6406 6c0d  m.Z.m.Z...d.d.l.
-00000080: 6d0e 5a0e 0100 6400 6407 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-00000090: 0100 6400 6408 6c11 6d12 5a12 0100 6503  ..d.d.l.m.Z...e.
-000000a0: 6409 8301 5a13 640a 640b 8400 5a14 6410  d...Z.d.d...Z.d.
-000000b0: 640c 640d 8401 5a15 4700 640e 640f 8400  d.d...Z.G.d.d...
-000000c0: 640f 6516 8303 5a17 6401 5300 2911 e900  d.e...Z.d.S.)...
-000000d0: 0000 004e 2901 da0a 436f 6e74 6578 7456  ...N)...ContextV
-000000e0: 6172 2901 da05 5374 6163 6b29 03da 0f54  ar)...Stack)...T
-000000f0: 6578 7450 6c61 6365 686f 6c64 6572 da11  extPlaceholder..
-00000100: 5374 6172 7450 6172 656e 4d61 7463 6865  StartParenMatche
-00000110: 72da 0f45 6e64 5061 7265 6e4d 6174 6368  r..EndParenMatch
-00000120: 6572 2902 da1b 4261 646c 7953 7065 6369  er)...BadlySpeci
-00000130: 6669 6564 5465 6d70 6c61 7465 4572 726f  fiedTemplateErro
-00000140: 72da 1345 6d70 7479 5374 6163 6b45 7863  r..EmptyStackExc
-00000150: 6570 7469 6f6e 2901 da0d 5661 6c69 6461  eption)...Valida
-00000160: 7465 5374 6172 7429 01da 1053 7472 6970  teStart)...Strip
-00000170: 5374 6172 7450 6172 656e 7329 01da 1957  StartParens)...W
-00000180: 6869 7465 5370 6163 6554 6578 7450 6c61  hiteSpaceTextPla
-00000190: 6365 686f 6c64 6572 da0b 6675 6c6c 5f73  ceholder..full_s
-000001a0: 7472 696e 6763 0300 0000 0000 0000 0000  tringc..........
-000001b0: 0000 0600 0000 0500 0000 4300 0000 735c  ..........C...s\
-000001c0: 0000 007c 02a0 007c 017c 00a1 027d 037c  ...|...|.|...}.|
-000001d0: 0373 0a7c 0053 0074 017c 007c 0383 0201  .s.|.S.t.|.|....
-000001e0: 0074 027c 0274 0383 0273 1874 047c 0383  .t.|.t...s.t.|..
-000001f0: 017d 037c 00a0 057c 0364 01a1 025c 027d  .}.|...|.d...\.}
-00000200: 047d 0574 047c 0483 0172 2c74 0664 02a0  .}.t.|...r,t.d..
-00000210: 077c 007c 02a1 0283 0182 017c 0553 0029  .|.|.......|.S.)
-00000220: 037a 254d 6174 6368 2061 2070 6c61 6365  .z%Match a place
-00000230: 686f 6c64 6572 2061 6761 696e 7374 2061  holder against a
-00000240: 2073 7472 696e 672e e901 0000 007a 3573   string......z5s
-00000250: 7472 696e 6720 227b 7d22 2073 686f 756c  tring "{}" shoul
-00000260: 6420 6861 7665 2073 7461 7274 6564 2077  d have started w
-00000270: 6974 6820 706c 6163 6568 6f6c 6465 7220  ith placeholder 
-00000280: 227b 7d22 2908 da06 5f6d 6174 6368 7209  "{}")..._matchr.
-00000290: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
-000002a0: 0400 0000 720a 0000 00da 0573 706c 6974  ....r......split
-000002b0: 7207 0000 00da 0666 6f72 6d61 7429 06da  r......format)..
-000002c0: 0673 7472 696e 67da 046e 6f64 65da 0b70  .string..node..p
-000002d0: 6c61 6365 686f 6c64 6572 da0c 6d61 7463  laceholder..matc
-000002e0: 6865 645f 7465 7874 da06 6265 666f 7265  hed_text..before
-000002f0: da05 6166 7465 72a9 0072 1800 0000 fa44  ..after..r.....D
-00000300: 2f68 6f6d 652f 7368 6169 2f66 756e 5f77  /home/shai/fun_w
-00000310: 6974 685f 6173 742f 6675 6e5f 7769 7468  ith_ast/fun_with
-00000320: 5f61 7374 2f73 6f75 7263 655f 6d61 7463  _ast/source_matc
-00000330: 6865 7273 2f62 6173 655f 6d61 7463 6865  hers/base_matche
-00000340: 722e 7079 da10 4d61 7463 6850 6c61 6365  r.py..MatchPlace
-00000350: 686f 6c64 6572 0d00 0000 731a 0000 000c  holder....s.....
-00000360: 0204 0104 010a 010a 0108 0110 0108 0102  ................
-00000370: 0102 0108 0104 fe04 0372 1a00 0000 6304  .........r....c.
-00000380: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00000390: 0000 0043 0000 0073 3000 0000 7c00 7d04  ...C...s0...|.}.
-000003a0: 7c02 4400 5d11 7d05 7c04 7c00 6b02 720f  |.D.].}.|.|.k.r.
-000003b0: 7c05 a000 7c03 a101 0100 7401 7c04 7c01  |...|.....t.|.|.
-000003c0: 7c05 8303 7d04 7104 7c04 5300 a901 4e29  |...}.q.|.S...N)
-000003d0: 02da 1153 6574 5374 6172 7469 6e67 5061  ...SetStartingPa
-000003e0: 7265 6e73 721a 0000 0029 0672 1200 0000  rensr....).r....
-000003f0: 7213 0000 00da 0c70 6c61 6365 686f 6c64  r......placehold
-00000400: 6572 73da 0f73 7461 7274 696e 675f 7061  ers..starting_pa
-00000410: 7265 6e73 da10 7265 6d61 696e 696e 675f  rens..remaining_
-00000420: 7374 7269 6e67 7214 0000 0072 1800 0000  stringr....r....
-00000430: 7218 0000 0072 1900 0000 da14 4d61 7463  r....r......Matc
-00000440: 6850 6c61 6365 686f 6c64 6572 4c69 7374  hPlaceholderList
-00000450: 1c00 0000 7310 0000 0004 0108 0108 010a  ....s...........
-00000460: 0102 0106 0106 ff04 0272 2000 0000 6300  .........r ...c.
-00000470: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000480: 0000 0040 0000 0073 8a00 0000 6500 5a01  ...@...s....e.Z.
-00000490: 6400 5a02 6401 5a03 6504 8300 5a05 6420  d.Z.d.Z.e...Z.d 
-000004a0: 6403 6404 8401 5a06 6405 6406 8400 5a07  d.d...Z.d.d...Z.
-000004b0: 6407 6408 8400 5a08 6409 640a 8400 5a09  d.d...Z.d.d...Z.
-000004c0: 640b 640c 8400 5a0a 640d 640e 8400 5a0b  d.d...Z.d.d...Z.
-000004d0: 640f 6410 8400 5a0c 6421 6412 6413 8401  d.d...Z.d!d.d...
-000004e0: 5a0d 6414 6415 8400 5a0e 6416 6417 8400  Z.d.d...Z.d.d...
-000004f0: 5a0f 6418 6419 8400 5a10 641a 641b 8400  Z.d.d...Z.d.d...
-00000500: 5a11 641c 641d 8400 5a12 641e 641f 8400  Z.d.d...Z.d.d...
-00000510: 5a13 6402 5300 2922 da0d 536f 7572 6365  Z.d.S.)"..Source
-00000520: 4d61 7463 6865 727a 7c42 6173 6520 636c  Matcherz|Base cl
-00000530: 6173 7320 666f 7220 616c 6c20 536f 7572  ass for all Sour
-00000540: 6365 4d61 7463 6865 7220 6f62 6a65 6374  ceMatcher object
-00000550: 732e 0a0a 2020 2020 5468 6573 6520 6172  s...    These ar
-00000560: 6520 6465 7369 676e 6564 2074 6f20 6d61  e designed to ma
-00000570: 7463 6820 7468 6520 736f 7572 6365 2074  tch the source t
-00000580: 6861 7420 636f 7272 6573 706f 6e64 7320  hat corresponds 
-00000590: 746f 2061 2067 6976 656e 206e 6f64 652e  to a given node.
-000005a0: 0a20 2020 204e 6303 0000 0000 0000 0000  .    Nc.........
-000005b0: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
-000005c0: 5400 0000 7c01 7c00 5f00 6700 7c00 5f01  T...|.|._.g.|._.
-000005d0: 7402 8300 6701 7c00 5f03 7402 8300 6701  t...g.|._.t...g.
-000005e0: 7c00 5f04 6401 7c00 5f05 6402 7c00 5f06  |._.d.|._.d.|._.
-000005f0: 7c02 731a 6700 7d02 7c02 7c00 5f07 6401  |.s.g.}.|.|._.d.
-00000600: 7c00 5f08 6400 7c00 5f09 7c00 6a0a 6a0b  |._.d.|._.|.j.j.
-00000610: 7c00 5f0c 6400 5300 2903 4e46 da00 290d  |._.d.S.).NF..).
-00000620: 7213 0000 00da 1265 6e64 5f70 6172 656e  r......end_paren
-00000630: 5f6d 6174 6368 6572 7372 0b00 0000 da19  _matchersr......
-00000640: 7374 6172 745f 7768 6974 6573 7061 6365  start_whitespace
-00000650: 5f6d 6174 6368 6572 73da 1765 6e64 5f77  _matchers..end_w
-00000660: 6869 7465 7370 6163 655f 6d61 7463 6865  hitespace_matche
-00000670: 7273 da0d 7061 7265 6e5f 7772 6170 7065  rs..paren_wrappe
-00000680: 64da 1365 6e64 5f6f 665f 6c69 6e65 5f63  d..end_of_line_c
-00000690: 6f6d 6d65 6e74 da14 7374 6172 745f 7061  omment..start_pa
-000006a0: 7265 6e5f 6d61 7463 6865 7273 da07 6d61  ren_matchers..ma
-000006b0: 7463 6865 64da 0e6d 6174 6368 6564 5f73  tched..matched_s
-000006c0: 6f75 7263 65da 1170 6172 656e 7468 6573  ource..parenthes
-000006d0: 6573 5f73 7461 636b da04 7369 7a65 da17  es_stack..size..
-000006e0: 7061 7265 6e74 6865 7365 735f 7374 6163  parentheses_stac
-000006f0: 6b5f 6465 7074 6829 03da 0473 656c 6672  k_depth)...selfr
-00000700: 1300 0000 da0f 7374 7269 7070 6564 5f70  ......stripped_p
-00000710: 6172 656e 7372 1800 0000 7218 0000 0072  arensr....r....r
-00000720: 1900 0000 da08 5f5f 696e 6974 5f5f 2b00  ......__init__+.
-00000730: 0000 7318 0000 0006 0106 010a 010a 0106  ..s.............
-00000740: 0106 0104 0104 0106 0106 0106 010e 017a  ...............z
-00000750: 1653 6f75 7263 654d 6174 6368 6572 2e5f  .SourceMatcher._
-00000760: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
-00000770: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
-00000780: 7362 0000 007c 00a0 007c 01a1 0101 0074  sb...|...|.....t
-00000790: 016a 02a0 03a1 0001 007c 00a0 047c 01a1  .j.......|...|..
-000007a0: 017d 0274 057c 0283 0174 057c 0183 016b  .}.t.|...t.|...k
-000007b0: 0072 2f7a 0874 06a0 077c 01a1 0101 0057  .r/z.t...|.....W
-000007c0: 007c 0253 0004 0074 0879 2e01 0001 0001  .|.S...t.y......
-000007d0: 0074 0964 017c 019b 0064 029d 0383 0182  .t.d.|...d......
-000007e0: 0177 007c 0253 0029 034e 7a07 7374 7269  .w.|.S.).Nz.stri
-000007f0: 6e67 207a 1420 6973 206e 6f74 2076 616c  ng z. is not val
-00000800: 6964 2070 7974 686f 6e29 0ada 1a5f 6368  id python)..._ch
-00000810: 6563 6b5f 6261 6c61 6e63 655f 7061 7265  eck_balance_pare
-00000820: 6e74 6865 7365 7372 2100 0000 722b 0000  nthesesr!...r+..
-00000830: 00da 0572 6573 6574 720e 0000 00da 036c  ...resetr......l
-00000840: 656e da03 6173 74da 0570 6172 7365 da0b  en..ast..parse..
-00000850: 5379 6e74 6178 4572 726f 7272 0700 0000  SyntaxErrorr....
-00000860: 2903 722e 0000 0072 1200 0000 da06 7265  ).r....r......re
-00000870: 7375 6c74 7218 0000 0072 1800 0000 7219  sultr....r....r.
-00000880: 0000 00da 0864 6f5f 6d61 7463 683a 0000  .....do_match:..
-00000890: 0073 1600 0000 0a01 0a01 0a01 1001 0201  .s..............
-000008a0: 0c01 0403 0cfe 1001 02ff 0402 7a16 536f  ............z.So
-000008b0: 7572 6365 4d61 7463 6865 722e 646f 5f6d  urceMatcher.do_m
-000008c0: 6174 6368 6302 0000 0000 0000 0000 0000  atchc...........
-000008d0: 0002 0000 0001 0000 0043 0000 00f3 0400  .........C......
-000008e0: 0000 7400 8201 721b 0000 00a9 01da 134e  ..t...r........N
-000008f0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00000900: 6f72 2902 722e 0000 0072 1200 0000 7218  or).r....r....r.
-00000910: 0000 0072 1800 0000 7219 0000 0072 0e00  ...r....r....r..
-00000920: 0000 4600 0000 7302 0000 0004 027a 1453  ..F...s......z.S
-00000930: 6f75 7263 654d 6174 6368 6572 2e5f 6d61  ourceMatcher._ma
-00000940: 7463 6863 0100 0000 0000 0000 0000 0000  tchc............
-00000950: 0100 0000 0100 0000 4300 0000 7239 0000  ........C...r9..
-00000960: 0072 1b00 0000 723a 0000 00a9 0172 2e00  .r....r:.....r..
-00000970: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000980: 00da 0947 6574 536f 7572 6365 4a00 0000  ...GetSourceJ...
-00000990: 7302 0000 0004 017a 1753 6f75 7263 654d  s......z.SourceM
-000009a0: 6174 6368 6572 2e47 6574 536f 7572 6365  atcher.GetSource
-000009b0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-000009c0: 0003 0000 0043 0000 0073 4400 0000 7c00  .....C...sD...|.
-000009d0: 6a00 6401 1900 6a01 7d02 7c02 7218 7402  j.d...j.}.|.r.t.
-000009e0: 7c00 6a00 6401 1900 6a01 8301 7d03 7c03  |.j.d...j...}.|.
-000009f0: 7c01 6b02 7216 6402 5300 6402 5300 6403  |.k.r.d.S.d.S.d.
-00000a00: 7c01 1400 7c00 6a00 6401 1900 5f01 6402  |...|.j.d..._.d.
-00000a10: 5300 2904 7a22 4669 7820 7468 6520 696e  S.).z"Fix the in
-00000a20: 6465 6e74 6174 696f 6e20 6f66 2074 6865  dentation of the
-00000a30: 2073 6f75 7263 652e 7201 0000 004e fa01   source.r....N..
-00000a40: 2029 0372 2400 0000 7215 0000 0072 3300   ).r$...r....r3.
-00000a50: 0000 2904 722e 0000 00da 096e 6577 5f69  ..).r......new_i
-00000a60: 6465 6e74 da0a 6375 7272 656e 745f 7773  dent..current_ws
-00000a70: da0d 6375 7272 656e 745f 6964 656e 7472  ..current_identr
-00000a80: 1800 0000 7218 0000 0072 1900 0000 da0e  ....r....r......
-00000a90: 4669 7849 6e64 656e 7461 7469 6f6e 4e00  FixIndentationN.
-00000aa0: 0000 730e 0000 000c 0204 0110 0108 0104  ..s.............
-00000ab0: 0104 ff14 037a 1c53 6f75 7263 654d 6174  .....z.SourceMat
-00000ac0: 6368 6572 2e46 6978 496e 6465 6e74 6174  cher.FixIndentat
-00000ad0: 696f 6e63 0200 0000 0000 0000 0000 0000  ionc............
-00000ae0: 0400 0000 0800 0000 4300 0000 7340 0000  ........C...s@..
-00000af0: 007c 017d 027a 1309 0074 0083 007d 0374  .|.}.z...t...}.t
-00000b00: 017c 0264 027c 0383 037d 027c 006a 02a0  .|.d.|...}.|.j..
-00000b10: 037c 037c 0066 02a1 0101 0071 0404 0074  .|.|.f.....q...t
-00000b20: 0479 1f01 0001 0001 0059 007c 0253 0077  .y.......Y.|.S.w
-00000b30: 0029 037a 284d 6174 6368 6573 2074 6865  .).z(Matches the
-00000b40: 2073 7461 7274 696e 6720 7061 7265 6e73   starting parens
-00000b50: 2069 6e20 6120 7374 7269 6e67 2e54 4e29   in a string.TN)
-00000b60: 0572 0500 0000 721a 0000 0072 2b00 0000  .r....r....r+...
-00000b70: da04 7075 7368 7207 0000 0029 0472 2e00  ..pushr....).r..
-00000b80: 0000 7212 0000 0072 1f00 0000 da13 7374  ..r....r......st
-00000b90: 6172 745f 7061 7265 6e5f 6d61 7463 6865  art_paren_matche
-00000ba0: 7272 1800 0000 7218 0000 0072 1900 0000  rr....r....r....
-00000bb0: da10 4d61 7463 6853 7461 7274 5061 7265  ..MatchStartPare
-00000bc0: 6e73 5900 0000 731a 0000 0004 0402 0102  nsY...s.........
-00000bd0: 0106 0102 0106 0104 ff10 0202 fc0c 0502  ................
-00000be0: 0104 0102 fe7a 1e53 6f75 7263 654d 6174  .....z.SourceMat
-00000bf0: 6368 6572 2e4d 6174 6368 5374 6172 7450  cher.MatchStartP
-00000c00: 6172 656e 7363 0200 0000 0000 0000 0000  arensc..........
-00000c10: 0000 0800 0000 0800 0000 4300 0000 73e2  ..........C...s.
-00000c20: 0000 0074 0083 007d 027a 0874 017c 0164  ...t...}.z.t.|.d
-00000c30: 017c 0283 0301 0057 006e 0a04 0074 0279  .|.....W.n...t.y
-00000c40: 1501 0001 0001 0059 0064 0153 0077 007c  .......Y.d.S.w.|
-00000c50: 017d 037a 3509 0074 0083 007d 027c 006a  .}.z5..t...}.|.j
-00000c60: 03a0 04a1 007d 0474 057c 0464 0319 0074  .....}.t.|.d...t
-00000c70: 0683 0272 4a74 017c 0364 017c 0283 037d  ...rJt.|.d.|...}
-00000c80: 037c 006a 03a0 07a1 007d 057c 0564 0419  .|.j.....}.|.d..
-00000c90: 007d 067c 0564 0319 007d 077c 006a 08a0  .}.|.d...}.|.j..
-00000ca0: 097c 02a1 0101 007c 066a 0aa0 0b64 037c  .|.....|.j...d.|
-00000cb0: 07a1 0201 006e 016e 0171 1a57 006e 1104  .....n.n.q.W.n..
-00000cc0: 0074 0279 5601 0001 0001 0059 006e 0904  .t.yV......Y.n..
-00000cd0: 0074 0c79 5e01 0001 0001 0059 006e 0177  .t.y^......Y.n.w
-00000ce0: 007c 0373 6f74 0d7c 006a 0a83 0174 0d7c  .|.sot.|.j...t.|
-00000cf0: 006a 0883 016b 0472 6f74 0264 0583 0182  .j...k.rot.d....
-00000d00: 017c 0353 0029 067a 264d 6174 6368 6573  .|.S.).z&Matches
-00000d10: 2074 6865 2065 6e64 696e 6720 7061 7265   the ending pare
-00000d20: 6e73 2069 6e20 6120 7374 7269 6e67 2e4e  ns in a string.N
-00000d30: 5472 0100 0000 720d 0000 007a 226d 6973  Tr....r....z"mis
-00000d40: 7369 6e67 2065 6e64 2070 6172 656e 2061  sing end paren a
-00000d50: 7420 656e 6420 6f66 2073 7472 696e 6729  t end of string)
-00000d60: 0e72 0600 0000 721a 0000 0072 0700 0000  .r....r....r....
-00000d70: 722b 0000 00da 0470 6565 6b72 0f00 0000  r+.....peekr....
-00000d80: 7205 0000 00da 0370 6f70 7223 0000 00da  r......popr#....
-00000d90: 0661 7070 656e 6472 2800 0000 da06 696e  .appendr(.....in
-00000da0: 7365 7274 7208 0000 0072 3300 0000 2908  sertr....r3...).
-00000db0: 722e 0000 0072 1200 0000 da11 656e 645f  r....r......end_
-00000dc0: 7061 7265 6e5f 6d61 7463 6865 7272 1f00  paren_matcherr..
-00000dd0: 0000 da0c 6d61 7463 6865 725f 7479 7065  ....matcher_type
-00000de0: da13 7061 6972 6564 5f6d 6174 6368 6572  ..paired_matcher
-00000df0: 5f69 6e66 6fda 156f 7269 6769 6e61 6c5f  _info..original_
-00000e00: 6e6f 6465 5f6d 6174 6368 6572 7244 0000  node_matcherrD..
-00000e10: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000e20: da0d 4d61 7463 6845 6e64 5061 7265 6e69  ..MatchEndPareni
-00000e30: 0000 0073 3a00 0000 0603 0201 1001 0c01  ...s:...........
-00000e40: 0601 02ff 0405 0202 0201 0602 0a02 0e01  ................
-00000e50: 0c02 0a01 0801 0801 0c01 1001 0202 02f2  ................
-00000e60: 040e 0c01 0401 0c01 0401 02ff 1802 0801  ................
-00000e70: 0401 7a1b 536f 7572 6365 4d61 7463 6865  ..z.SourceMatche
-00000e80: 722e 4d61 7463 6845 6e64 5061 7265 6e46  r.MatchEndParenF
-00000e90: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
-00000ea0: 0004 0000 0043 0000 0073 4e00 0000 7c01  .....C...sN...|.
-00000eb0: 6400 7500 7206 6401 5300 7c01 7d03 6401  d.u.r.d.S.|.}.d.
-00000ec0: 7d04 7400 a001 6402 7c01 a102 7d05 7c05  }.t...d.|...}.|.
-00000ed0: 7217 7c05 a002 6403 a101 7d04 7c04 721c  r.|...d...}.|.r.
-00000ee0: 7c04 7c00 5f03 7c02 7225 7c05 7225 7c05  |.|._.|.r%|.r%|.
-00000ef0: a002 6404 a101 7d03 7c04 5300 2905 4e72  ..d...}.|.S.).Nr
-00000f00: 2200 0000 7a0a 285c 732a 2928 232e 2a29  "...z.(\s*)(#.*)
-00000f10: e902 0000 0072 0d00 0000 2904 da02 7265  .....r....)...re
-00000f20: da05 6d61 7463 68da 0567 726f 7570 7227  ..match..groupr'
-00000f30: 0000 0029 0672 2e00 0000 7212 0000 00da  ...).r....r.....
-00000f40: 0e72 656d 6f76 655f 636f 6d6d 656e 7472  .remove_commentr
-00000f50: 1f00 0000 da07 636f 6d6d 656e 74da 0966  ......comment..f
-00000f60: 756c 6c5f 6c69 6e65 7218 0000 0072 1800  ull_liner....r..
-00000f70: 0000 7219 0000 00da 0f4d 6174 6368 436f  ..r......MatchCo
-00000f80: 6d6d 656e 7445 4f4c 8f00 0000 7318 0000  mmentEOL....s...
-00000f90: 0008 0104 0104 0104 010c 0204 010a 0104  ................
-00000fa0: 0106 0108 010a 0104 017a 1d53 6f75 7263  .........z.Sourc
-00000fb0: 654d 6174 6368 6572 2e4d 6174 6368 436f  eMatcher.MatchCo
-00000fc0: 6d6d 656e 7445 4f4c 6301 0000 0000 0000  mmentEOLc.......
-00000fd0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00000fe0: 0073 2200 0000 6401 7d01 7c00 6a00 4400  .s"...d.}.|.j.D.
-00000ff0: 5d09 7d02 7c01 7c02 a001 6400 a101 3700  ].}.|.|...d...7.
-00001000: 7d01 7105 7c01 5300 2902 4e72 2200 0000  }.q.|.S.).Nr"...
-00001010: 2902 7228 0000 0072 3d00 0000 2903 722e  ).r(...r=...).r.
-00001020: 0000 0072 3700 0000 da07 6d61 7463 6865  ...r7.....matche
-00001030: 7272 1800 0000 7218 0000 0072 1900 0000  rr....r....r....
-00001040: da11 4765 7453 7461 7274 5061 7265 6e54  ..GetStartParenT
-00001050: 6578 74a0 0000 0073 0800 0000 0401 0a05  ext....s........
-00001060: 1001 0401 7a1f 536f 7572 6365 4d61 7463  ....z.SourceMatc
-00001070: 6865 722e 4765 7453 7461 7274 5061 7265  her.GetStartPare
-00001080: 6e54 6578 7463 0200 0000 0000 0000 0000  nTextc..........
-00001090: 0000 0300 0000 0400 0000 4300 0000 7320  ..........C...s 
-000010a0: 0000 0064 017d 027c 0172 0e64 01a0 0064  ...d.}.|.r.d...d
-000010b0: 0264 0384 007c 0144 0083 01a1 017d 027c  .d...|.D.....}.|
-000010c0: 0253 0029 044e 7222 0000 0063 0100 0000  .S.).Nr"...c....
-000010d0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000010e0: 7300 0000 f31a 0000 0081 007c 005d 087d  s..........|.].}
-000010f0: 017c 01a0 0064 00a1 0156 0001 0071 0264  .|...d...V...q.d
-00001100: 0053 0072 1b00 0000 a901 723d 0000 00a9  .S.r......r=....
-00001110: 02da 022e 3072 5700 0000 7218 0000 0072  ....0rW...r....r
-00001120: 1800 0000 7219 0000 00da 093c 6765 6e65  ....r......<gene
-00001130: 7870 723e ad00 0000 f308 0000 0002 8004  xpr>............
-00001140: 0002 0112 ff7a 3253 6f75 7263 654d 6174  .....z2SourceMat
-00001150: 6368 6572 2e47 6574 5768 6974 6553 7061  cher.GetWhiteSpa
-00001160: 6365 5465 7874 2e3c 6c6f 6361 6c73 3e2e  ceText.<locals>.
-00001170: 3c67 656e 6578 7072 3e29 01da 046a 6f69  <genexpr>)...joi
-00001180: 6e29 0372 2e00 0000 da0a 696e 5f6d 6174  n).r......in_mat
-00001190: 6368 6572 7237 0000 0072 1800 0000 7218  cherr7...r....r.
-000011a0: 0000 0072 1900 0000 da11 4765 7457 6869  ...r......GetWhi
-000011b0: 7465 5370 6163 6554 6578 74aa 0000 0073  teSpaceText....s
-000011c0: 0c00 0000 0401 0401 0a01 0201 08ff 0402  ................
-000011d0: 7a1f 536f 7572 6365 4d61 7463 6865 722e  z.SourceMatcher.
-000011e0: 4765 7457 6869 7465 5370 6163 6554 6578  GetWhiteSpaceTex
-000011f0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-00001200: 0000 0400 0000 4300 0000 7316 0000 0064  ......C...s....d
-00001210: 01a0 0064 0264 0384 007c 006a 0144 0083  ...d.d...|.j.D..
-00001220: 01a1 0153 0029 044e 7222 0000 0063 0100  ...S.).Nr"...c..
-00001230: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001240: 0000 7300 0000 7259 0000 0072 1b00 0000  ..s...rY...r....
-00001250: 725a 0000 0072 5b00 0000 7218 0000 0072  rZ...r[...r....r
-00001260: 1800 0000 7219 0000 0072 5d00 0000 b300  ....r....r].....
-00001270: 0000 725e 0000 007a 3053 6f75 7263 654d  ..r^...z0SourceM
-00001280: 6174 6368 6572 2e47 6574 456e 6450 6172  atcher.GetEndPar
-00001290: 656e 5465 7874 2e3c 6c6f 6361 6c73 3e2e  enText.<locals>.
-000012a0: 3c67 656e 6578 7072 3e29 0272 5f00 0000  <genexpr>).r_...
-000012b0: 7223 0000 0072 3c00 0000 7218 0000 0072  r#...r<...r....r
-000012c0: 1800 0000 7219 0000 00da 0f47 6574 456e  ....r......GetEn
-000012d0: 6450 6172 656e 5465 7874 b100 0000 7306  dParenText....s.
-000012e0: 0000 000a 0204 0108 ff7a 1d53 6f75 7263  .........z.Sourc
-000012f0: 654d 6174 6368 6572 2e47 6574 456e 6450  eMatcher.GetEndP
-00001300: 6172 656e 5465 7874 6301 0000 0000 0000  arenTextc.......
-00001310: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001320: 0073 4a00 0000 7c00 6a00 6401 1900 7d01  .sJ...|.j.d...}.
-00001330: 7401 7c01 7402 8302 7219 7c01 6a03 7215  t.|.t...r.|.j.r.
-00001340: 7c01 0400 6a03 6402 3700 0200 5f03 6e08  |...j.d.7..._.n.
-00001350: 6402 7c01 5f03 6e04 7404 6403 8301 8201  d.|._.n.t.d.....
-00001360: 6400 7c00 5f05 6404 7c00 5f06 6400 5300  d.|._.d.|._.d.S.
-00001370: 2905 4ee9 ffff ffff da01 0a7a 2a43 616e  ).N........z*Can
-00001380: 6e6f 7420 6164 6420 6e65 776c 696e 6520  not add newline 
-00001390: 746f 206e 6f6e 2d74 6578 7420 706c 6163  to non-text plac
-000013a0: 6568 6f6c 6465 7246 2907 da0e 6578 7065  eholderF)...expe
-000013b0: 6374 6564 5f70 6172 7473 720f 0000 0072  cted_partsr....r
-000013c0: 0400 0000 7215 0000 0072 3b00 0000 722a  ....r....r;...r*
-000013d0: 0000 0072 2900 0000 2902 722e 0000 00da  ...r)...).r.....
-000013e0: 0470 6172 7472 1800 0000 7218 0000 0072  .partr....r....r
-000013f0: 1900 0000 da15 6164 645f 6e65 776c 696e  ......add_newlin
-00001400: 655f 746f 5f73 6f75 7263 65b7 0000 0073  e_to_source....s
-00001410: 1000 0000 0a01 0a01 0601 1001 0802 0802  ................
-00001420: 0601 0a01 7a23 536f 7572 6365 4d61 7463  ....z#SourceMatc
-00001430: 6865 722e 6164 645f 6e65 776c 696e 655f  her.add_newline_
-00001440: 746f 5f73 6f75 7263 6563 0100 0000 0000  to_sourcec......
-00001450: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001460: 0000 7346 0000 007c 006a 0072 0c7c 006a  ..sF...|.j.r.|.j
-00001470: 0164 0075 0072 0c74 0264 0183 0182 017c  .d.u.r.t.d.....|
-00001480: 006a 0073 187c 006a 0164 0075 0172 1874  .j.s.|.j.d.u.r.t
-00001490: 0264 0283 0182 0174 037c 0064 0383 0272  .d.....t.|.d...r
-000014a0: 2174 0264 0483 0182 0164 0053 0029 054e  !t.d.....d.S.).N
-000014b0: 7a3e 496e 7465 726e 616c 2045 7272 6f72  z>Internal Error
-000014c0: 3a20 6d61 7463 6865 645f 7465 7874 206d  : matched_text m
-000014d0: 7573 7420 6265 2073 6574 2069 6620 6973  ust be set if is
-000014e0: 5f6d 6174 6368 6564 2069 7320 5472 7565  _matched is True
-000014f0: 7a40 496e 7465 726e 616c 2045 7272 6f72  z@Internal Error
-00001500: 3a20 6d61 7463 6865 645f 7465 7874 206d  : matched_text m
-00001510: 7573 7420 6265 204e 6f6e 6520 6966 2069  ust be None if i
-00001520: 735f 6d61 7463 6865 6420 6973 2046 616c  s_matched is Fal
-00001530: 7365 7215 0000 007a 2b49 6e74 6572 6e61  ser....z+Interna
-00001540: 6c20 4572 726f 723a 2064 6f6e 7420 6861  l Error: dont ha
-00001550: 7665 2074 6869 7320 6669 656c 6420 2d20  ve this field - 
-00001560: 6576 6572 2904 7229 0000 0072 2a00 0000  ever).r)...r*...
-00001570: da0a 5661 6c75 6545 7272 6f72 da07 6861  ..ValueError..ha
-00001580: 7361 7474 7272 3c00 0000 7218 0000 0072  sattrr<...r....r
-00001590: 1800 0000 7219 0000 00da 1776 616c 6964  ....r......valid
-000015a0: 6174 6564 5f63 616c 6c5f 746f 5f6d 6174  ated_call_to_mat
-000015b0: 6368 c200 0000 730e 0000 0010 0108 0110  ch....s.........
-000015c0: 0108 010a 0108 0104 ff7a 2553 6f75 7263  .........z%Sourc
-000015d0: 654d 6174 6368 6572 2e76 616c 6964 6174  eMatcher.validat
-000015e0: 6564 5f63 616c 6c5f 746f 5f6d 6174 6368  ed_call_to_match
-000015f0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00001600: 0003 0000 0043 0000 0073 4800 0000 6401  .....C...sH...d.
-00001610: 0400 7d02 7d03 7c01 4400 5d13 7d04 7c04  ..}.}.|.D.].}.|.
-00001620: 6402 6b02 7211 7c02 6403 3700 7d02 7106  d.k.r.|.d.7.}.q.
-00001630: 7c04 6404 6b02 7219 7c03 6403 3700 7d03  |.d.k.r.|.d.7.}.
-00001640: 7106 7c02 7c03 6b03 7222 7400 6405 8301  q.|.|.k.r"t.d...
-00001650: 8201 6400 5300 2906 4e72 0100 0000 fa01  ..d.S.).Nr......
-00001660: 2872 0d00 0000 fa01 297a 1675 6e62 616c  (r......)z.unbal
-00001670: 616e 6365 6420 7061 7265 6e74 6865 7365  anced parenthese
-00001680: 7329 0172 0700 0000 2905 722e 0000 0072  s).r....).r....r
-00001690: 1200 0000 da04 6c65 6674 da05 7269 6768  ......left..righ
-000016a0: 74da 0163 7218 0000 0072 1800 0000 7219  t..cr....r....r.
-000016b0: 0000 0072 3100 0000 ca00 0000 7314 0000  ...r1.......s...
-000016c0: 0008 0108 0108 010a 0108 0108 0102 8008  ................
-000016d0: 0208 0104 ff7a 2853 6f75 7263 654d 6174  .....z(SourceMat
-000016e0: 6368 6572 2e5f 6368 6563 6b5f 6261 6c61  cher._check_bala
-000016f0: 6e63 655f 7061 7265 6e74 6865 7365 7372  nce_parenthesesr
-00001700: 1b00 0000 2901 4629 14da 085f 5f6e 616d  ....).F)...__nam
-00001710: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00001720: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00001730: 5f64 6f63 5f5f 7203 0000 0072 2b00 0000  _doc__r....r+...
-00001740: 7230 0000 0072 3800 0000 720e 0000 0072  r0...r8...r....r
-00001750: 3d00 0000 7242 0000 0072 4500 0000 724e  =...rB...rE...rN
-00001760: 0000 0072 5600 0000 7258 0000 0072 6100  ...rV...rX...ra.
-00001770: 0000 7262 0000 0072 6700 0000 726a 0000  ..rb...rg...rj..
-00001780: 0072 3100 0000 7218 0000 0072 1800 0000  .r1...r....r....
-00001790: 7218 0000 0072 1900 0000 7221 0000 0025  r....r....r!...%
-000017a0: 0000 0073 2200 0000 0800 0401 0604 0a01  ...s"...........
-000017b0: 080f 080c 0804 0804 080b 0810 0a26 0811  .............&..
-000017c0: 080a 0807 0806 080b 0c08 7221 0000 0072  ..........r!...r
-000017d0: 1b00 0000 2918 7234 0000 0072 5000 0000  ....).r4...rP...
-000017e0: da0b 636f 6e74 6578 7476 6172 7372 0200  ..contextvarsr..
-000017f0: 0000 da1f 6675 6e5f 7769 7468 5f61 7374  ....fun_with_ast
-00001800: 2e63 6f6d 6d6f 6e5f 7574 696c 732e 7374  .common_utils.st
-00001810: 6163 6b72 0300 0000 da1e 6675 6e5f 7769  ackr......fun_wi
-00001820: 7468 5f61 7374 2e70 6c61 6365 686f 6c64  th_ast.placehold
-00001830: 6572 732e 7465 7874 7204 0000 0072 0500  ers.textr....r..
-00001840: 0000 7206 0000 00da 2766 756e 5f77 6974  ..r.....'fun_wit
-00001850: 685f 6173 742e 736f 7572 6365 5f6d 6174  h_ast.source_mat
-00001860: 6368 6572 732e 6578 6365 7074 696f 6e73  chers.exceptions
-00001870: 7207 0000 0072 0800 0000 da1e 6675 6e5f  r....r......fun_
-00001880: 7769 7468 5f61 7374 2e70 6c61 6365 686f  with_ast.placeho
-00001890: 6c64 6572 732e 6e6f 6465 7209 0000 00da  lders.noder.....
-000018a0: 2766 756e 5f77 6974 685f 6173 742e 706c  'fun_with_ast.pl
-000018b0: 6163 6568 6f6c 6465 7273 2e73 7472 696e  aceholders.strin
-000018c0: 675f 7061 7273 6572 720a 0000 00da 2466  g_parserr.....$f
-000018d0: 756e 5f77 6974 685f 6173 742e 706c 6163  un_with_ast.plac
-000018e0: 6568 6f6c 6465 7273 2e77 6869 7465 7370  eholders.whitesp
-000018f0: 6163 6572 0b00 0000 720c 0000 0072 1a00  acer....r....r..
-00001900: 0000 7220 0000 00da 066f 626a 6563 7472  ..r .....objectr
-00001910: 2100 0000 7218 0000 0072 1800 0000 7218  !...r....r....r.
-00001920: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001930: 653e 0100 0000 731a 0000 0008 0008 010c  e>....s.........
-00001940: 010c 0214 0110 010c 010c 010c 0108 0208  ................
-00001950: 010a 0f14 09                             .....
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 4700  ..d.d.l.m.Z...G.
+00000070: 6406 6407 8400 6407 650a 8303 5a0b 6401  d.d...d.e...Z.d.
+00000080: 5300 2908 e900 0000 004e 2901 da10 5061  S.)......N)...Pa
+00000090: 7261 6e74 6865 7369 7353 7461 636b 2901  ranthesisStack).
+000000a0: da0f 5465 7874 506c 6163 6568 6f6c 6465  ..TextPlaceholde
+000000b0: 7229 01da 1957 6869 7465 5370 6163 6554  r)...WhiteSpaceT
+000000c0: 6578 7450 6c61 6365 686f 6c64 6572 a901  extPlaceholder..
+000000d0: da1b 4261 646c 7953 7065 6369 6669 6564  ..BadlySpecified
+000000e0: 5465 6d70 6c61 7465 4572 726f 7263 0000  TemplateErrorc..
+000000f0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000100: 0000 4000 0000 738c 0000 0065 005a 0164  ..@...s....e.Z.d
+00000110: 005a 0264 015a 0365 0483 005a 0564 2064  .Z.d.Z.e...Z.d d
+00000120: 0364 0484 015a 0664 0564 0684 005a 0764  .d...Z.d.d...Z.d
+00000130: 0764 0884 005a 0864 0964 0a84 005a 0964  .d...Z.d.d...Z.d
+00000140: 0b64 0c84 005a 0a64 2064 0d64 0e84 015a  .d...Z.d d.d...Z
+00000150: 0b64 0f64 1084 005a 0c64 2164 1264 1384  .d.d...Z.d!d.d..
+00000160: 015a 0d64 1464 1584 005a 0e64 1664 1784  .Z.d.d...Z.d.d..
+00000170: 005a 0f64 1864 1984 005a 1064 1a64 1b84  .Z.d.d...Z.d.d..
+00000180: 005a 1164 1c64 1d84 005a 1264 1e64 1f84  .Z.d.d...Z.d.d..
+00000190: 005a 1364 0253 0029 22da 0d53 6f75 7263  .Z.d.S.)"..Sourc
+000001a0: 654d 6174 6368 6572 7a7c 4261 7365 2063  eMatcherz|Base c
+000001b0: 6c61 7373 2066 6f72 2061 6c6c 2053 6f75  lass for all Sou
+000001c0: 7263 654d 6174 6368 6572 206f 626a 6563  rceMatcher objec
+000001d0: 7473 2e0a 0a20 2020 2054 6865 7365 2061  ts...    These a
+000001e0: 7265 2064 6573 6967 6e65 6420 746f 206d  re designed to m
+000001f0: 6174 6368 2074 6865 2073 6f75 7263 6520  atch the source 
+00000200: 7468 6174 2063 6f72 7265 7370 6f6e 6473  that corresponds
+00000210: 2074 6f20 6120 6769 7665 6e20 6e6f 6465   to a given node
+00000220: 2e0a 2020 2020 4e63 0300 0000 0000 0000  ..    Nc........
+00000230: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+00000240: 7354 0000 007c 017c 005f 0067 007c 005f  sT...|.|._.g.|._
+00000250: 0174 0283 0067 017c 005f 0374 0283 0067  .t...g.|._.t...g
+00000260: 017c 005f 0464 017c 005f 0564 027c 005f  .|._.d.|._.d.|._
+00000270: 067c 0273 1a67 007d 027c 027c 005f 0764  .|.s.g.}.|.|._.d
+00000280: 017c 005f 0864 007c 005f 097c 006a 0a6a  .|._.d.|._.|.j.j
+00000290: 0b7c 005f 0c64 0053 0029 034e 46da 0029  .|._.d.S.).NF..)
+000002a0: 0dda 046e 6f64 65da 1265 6e64 5f70 6172  ...node..end_par
+000002b0: 656e 5f6d 6174 6368 6572 7372 0400 0000  en_matchersr....
+000002c0: da19 7374 6172 745f 7768 6974 6573 7061  ..start_whitespa
+000002d0: 6365 5f6d 6174 6368 6572 73da 1765 6e64  ce_matchers..end
+000002e0: 5f77 6869 7465 7370 6163 655f 6d61 7463  _whitespace_matc
+000002f0: 6865 7273 da0d 7061 7265 6e5f 7772 6170  hers..paren_wrap
+00000300: 7065 64da 1365 6e64 5f6f 665f 6c69 6e65  ped..end_of_line
+00000310: 5f63 6f6d 6d65 6e74 da14 7374 6172 745f  _comment..start_
+00000320: 7061 7265 6e5f 6d61 7463 6865 7273 da07  paren_matchers..
+00000330: 6d61 7463 6865 64da 0e6d 6174 6368 6564  matched..matched
+00000340: 5f73 6f75 7263 65da 1170 6172 656e 7468  _source..parenth
+00000350: 6573 6573 5f73 7461 636b da04 7369 7a65  eses_stack..size
+00000360: da17 7061 7265 6e74 6865 7365 735f 7374  ..parentheses_st
+00000370: 6163 6b5f 6465 7074 6829 03da 0473 656c  ack_depth)...sel
+00000380: 6672 0900 0000 da0f 7374 7269 7070 6564  fr......stripped
+00000390: 5f70 6172 656e 73a9 0072 1700 0000 fa44  _parens..r.....D
+000003a0: 2f68 6f6d 652f 7368 6169 2f66 756e 5f77  /home/shai/fun_w
+000003b0: 6974 685f 6173 742f 6675 6e5f 7769 7468  ith_ast/fun_with
+000003c0: 5f61 7374 2f73 6f75 7263 655f 6d61 7463  _ast/source_matc
+000003d0: 6865 7273 2f62 6173 655f 6d61 7463 6865  hers/base_matche
+000003e0: 722e 7079 da08 5f5f 696e 6974 5f5f 1000  r.py..__init__..
+000003f0: 0000 7318 0000 0006 0106 010a 010a 0106  ..s.............
+00000400: 0106 0104 0104 0106 0106 0106 010e 017a  ...............z
+00000410: 1653 6f75 7263 654d 6174 6368 6572 2e5f  .SourceMatcher._
+00000420: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
+00000430: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
+00000440: 7362 0000 007c 00a0 007c 01a1 0101 0074  sb...|...|.....t
+00000450: 016a 02a0 03a1 0001 007c 00a0 047c 01a1  .j.......|...|..
+00000460: 017d 0274 057c 0283 0174 057c 0183 016b  .}.t.|...t.|...k
+00000470: 0072 2f7a 0874 06a0 077c 01a1 0101 0057  .r/z.t...|.....W
+00000480: 007c 0253 0004 0074 0879 2e01 0001 0001  .|.S...t.y......
+00000490: 0074 0964 017c 019b 0064 029d 0383 0182  .t.d.|...d......
+000004a0: 0177 007c 0253 0029 034e 7a07 7374 7269  .w.|.S.).Nz.stri
+000004b0: 6e67 207a 1420 6973 206e 6f74 2076 616c  ng z. is not val
+000004c0: 6964 2070 7974 686f 6e29 0ada 1a5f 6368  id python)..._ch
+000004d0: 6563 6b5f 6261 6c61 6e63 655f 7061 7265  eck_balance_pare
+000004e0: 6e74 6865 7365 7372 0700 0000 7212 0000  nthesesr....r...
+000004f0: 00da 0572 6573 6574 da06 5f6d 6174 6368  ...reset.._match
+00000500: da03 6c65 6eda 0361 7374 da05 7061 7273  ..len..ast..pars
+00000510: 65da 0b53 796e 7461 7845 7272 6f72 7206  e..SyntaxErrorr.
+00000520: 0000 0029 0372 1500 0000 da06 7374 7269  ...).r......stri
+00000530: 6e67 da06 7265 7375 6c74 7217 0000 0072  ng..resultr....r
+00000540: 1700 0000 7218 0000 00da 0864 6f5f 6d61  ....r......do_ma
+00000550: 7463 681f 0000 0073 1600 0000 0a01 0a01  tch....s........
+00000560: 0a01 1001 0201 0c01 0403 0cfe 1001 02ff  ................
+00000570: 0402 7a16 536f 7572 6365 4d61 7463 6865  ..z.SourceMatche
+00000580: 722e 646f 5f6d 6174 6368 6302 0000 0000  r.do_matchc.....
+00000590: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
+000005a0: 0000 00f3 0400 0000 7400 8201 a901 4ea9  ........t.....N.
+000005b0: 01da 134e 6f74 496d 706c 656d 656e 7465  ...NotImplemente
+000005c0: 6445 7272 6f72 a902 7215 0000 0072 2100  dError..r....r!.
+000005d0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000005e0: 0072 1c00 0000 2b00 0000 f302 0000 0004  .r....+.........
+000005f0: 017a 1453 6f75 7263 654d 6174 6368 6572  .z.SourceMatcher
+00000600: 2e5f 6d61 7463 6863 0100 0000 0000 0000  ._matchc........
+00000610: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000620: 7224 0000 0072 2500 0000 7226 0000 00a9  r$...r%...r&....
+00000630: 0172 1500 0000 7217 0000 0072 1700 0000  .r....r....r....
+00000640: 7218 0000 00da 0947 6574 536f 7572 6365  r......GetSource
+00000650: 2e00 0000 7229 0000 007a 1753 6f75 7263  ....r)...z.Sourc
+00000660: 654d 6174 6368 6572 2e47 6574 536f 7572  eMatcher.GetSour
+00000670: 6365 6302 0000 0000 0000 0000 0000 0004  cec.............
+00000680: 0000 0003 0000 0043 0000 0073 4400 0000  .......C...sD...
+00000690: 7c00 6a00 6401 1900 6a01 7d02 7c02 7218  |.j.d...j.}.|.r.
+000006a0: 7402 7c00 6a00 6401 1900 6a01 8301 7d03  t.|.j.d...j...}.
+000006b0: 7c03 7c01 6b02 7216 6402 5300 6402 5300  |.|.k.r.d.S.d.S.
+000006c0: 6403 7c01 1400 7c00 6a00 6401 1900 5f01  d.|...|.j.d..._.
+000006d0: 6402 5300 2904 7a22 4669 7820 7468 6520  d.S.).z"Fix the 
+000006e0: 696e 6465 6e74 6174 696f 6e20 6f66 2074  indentation of t
+000006f0: 6865 2073 6f75 7263 652e 7201 0000 004e  he source.r....N
+00000700: fa01 2029 0372 0b00 0000 da0c 6d61 7463  .. ).r......matc
+00000710: 6865 645f 7465 7874 721d 0000 0029 0472  hed_textr....).r
+00000720: 1500 0000 da09 6e65 775f 6964 656e 74da  ......new_ident.
+00000730: 0a63 7572 7265 6e74 5f77 73da 0d63 7572  .current_ws..cur
+00000740: 7265 6e74 5f69 6465 6e74 7217 0000 0072  rent_identr....r
+00000750: 1700 0000 7218 0000 00da 0e46 6978 496e  ....r......FixIn
+00000760: 6465 6e74 6174 696f 6e32 0000 0073 0e00  dentation2...s..
+00000770: 0000 0c02 0401 1001 0801 0401 04ff 1403  ................
+00000780: 7a1c 536f 7572 6365 4d61 7463 6865 722e  z.SourceMatcher.
+00000790: 4669 7849 6e64 656e 7461 7469 6f6e 6303  FixIndentationc.
+000007a0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+000007b0: 0000 0043 0000 00f3 0e00 0000 7c00 6a00  ...C........|.j.
+000007c0: a001 7c00 7c01 a102 5300 2901 7a28 4d61  ..|.|...S.).z(Ma
+000007d0: 7463 6865 7320 7468 6520 7374 6172 7469  tches the starti
+000007e0: 6e67 2070 6172 656e 7320 696e 2061 2073  ng parens in a s
+000007f0: 7472 696e 672e 2902 7212 0000 00da 104d  tring.).r......M
+00000800: 6174 6368 5374 6172 7450 6172 656e 7329  atchStartParens)
+00000810: 0372 1500 0000 7221 0000 00da 0672 6574  .r....r!.....ret
+00000820: 7275 6e72 1700 0000 7217 0000 0072 1800  runr....r....r..
+00000830: 0000 7233 0000 003d 0000 0073 0200 0000  ..r3...=...s....
+00000840: 0e03 7a1e 536f 7572 6365 4d61 7463 6865  ..z.SourceMatche
+00000850: 722e 4d61 7463 6853 7461 7274 5061 7265  r.MatchStartPare
+00000860: 6e73 6302 0000 0000 0000 0000 0000 0002  nsc.............
+00000870: 0000 0004 0000 0043 0000 0072 3200 0000  .......C...r2...
+00000880: 2901 7a26 4d61 7463 6865 7320 7468 6520  ).z&Matches the 
+00000890: 656e 6469 6e67 2070 6172 656e 7320 696e  ending parens in
+000008a0: 2061 2073 7472 696e 672e 2902 7212 0000   a string.).r...
+000008b0: 00da 0e4d 6174 6368 456e 6450 6172 656e  ...MatchEndParen
+000008c0: 7372 2800 0000 7217 0000 0072 1700 0000  sr(...r....r....
+000008d0: 7218 0000 00da 0d4d 6174 6368 456e 6450  r......MatchEndP
+000008e0: 6172 656e 4200 0000 7302 0000 000e 027a  arenB...s......z
+000008f0: 1b53 6f75 7263 654d 6174 6368 6572 2e4d  .SourceMatcher.M
+00000900: 6174 6368 456e 6450 6172 656e 4663 0300  atchEndParenFc..
+00000910: 0000 0000 0000 0000 0000 0600 0000 0400  ................
+00000920: 0000 4300 0000 734e 0000 007c 0164 0075  ..C...sN...|.d.u
+00000930: 0072 0664 0153 007c 017d 0364 017d 0474  .r.d.S.|.}.d.}.t
+00000940: 00a0 0164 027c 01a1 027d 057c 0572 177c  ...d.|...}.|.r.|
+00000950: 05a0 0264 03a1 017d 047c 0472 1c7c 047c  ...d...}.|.r.|.|
+00000960: 005f 037c 0272 257c 0572 257c 05a0 0264  ._.|.r%|.r%|...d
+00000970: 04a1 017d 037c 0453 0029 054e 7208 0000  ...}.|.S.).Nr...
+00000980: 007a 0a28 5c73 2a29 2823 2e2a 29e9 0200  .z.(\s*)(#.*)...
+00000990: 0000 e901 0000 0029 04da 0272 65da 056d  .......)...re..m
+000009a0: 6174 6368 da05 6772 6f75 7072 0e00 0000  atch..groupr....
+000009b0: 2906 7215 0000 0072 2100 0000 da0e 7265  ).r....r!.....re
+000009c0: 6d6f 7665 5f63 6f6d 6d65 6e74 da10 7265  move_comment..re
+000009d0: 6d61 696e 696e 675f 7374 7269 6e67 da07  maining_string..
+000009e0: 636f 6d6d 656e 74da 0966 756c 6c5f 6c69  comment..full_li
+000009f0: 6e65 7217 0000 0072 1700 0000 7218 0000  ner....r....r...
+00000a00: 00da 0f4d 6174 6368 436f 6d6d 656e 7445  ...MatchCommentE
+00000a10: 4f4c 4800 0000 7318 0000 0008 0104 0104  OLH...s.........
+00000a20: 0104 010c 0204 010a 0104 0106 0108 010a  ................
+00000a30: 0104 017a 1d53 6f75 7263 654d 6174 6368  ...z.SourceMatch
+00000a40: 6572 2e4d 6174 6368 436f 6d6d 656e 7445  er.MatchCommentE
+00000a50: 4f4c 6301 0000 0000 0000 0000 0000 0003  OLc.............
+00000a60: 0000 0005 0000 0043 0000 0073 2200 0000  .......C...s"...
+00000a70: 6401 7d01 7c00 6a00 4400 5d09 7d02 7c01  d.}.|.j.D.].}.|.
+00000a80: 7c02 a001 6400 a101 3700 7d01 7105 7c01  |...d...7.}.q.|.
+00000a90: 5300 2902 4e72 0800 0000 2902 720f 0000  S.).Nr....).r...
+00000aa0: 0072 2b00 0000 2903 7215 0000 0072 2200  .r+...).r....r".
+00000ab0: 0000 da07 6d61 7463 6865 7272 1700 0000  ....matcherr....
+00000ac0: 7217 0000 0072 1800 0000 da11 4765 7453  r....r......GetS
+00000ad0: 7461 7274 5061 7265 6e54 6578 7459 0000  tartParenTextY..
+00000ae0: 0073 0800 0000 0401 0a01 1001 0401 7a1f  .s............z.
+00000af0: 536f 7572 6365 4d61 7463 6865 722e 4765  SourceMatcher.Ge
+00000b00: 7453 7461 7274 5061 7265 6e54 6578 7463  tStartParenTextc
+00000b10: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000b20: 0400 0000 4300 0000 7320 0000 0064 017d  ....C...s ...d.}
+00000b30: 027c 0172 0e64 01a0 0064 0264 0384 007c  .|.r.d...d.d...|
+00000b40: 0144 0083 01a1 017d 027c 0253 0029 044e  .D.....}.|.S.).N
+00000b50: 7208 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000b60: 0000 0200 0000 0400 0000 7300 0000 f31a  ..........s.....
+00000b70: 0000 0081 007c 005d 087d 017c 01a0 0064  .....|.].}.|...d
+00000b80: 00a1 0156 0001 0071 0264 0053 0072 2500  ...V...q.d.S.r%.
+00000b90: 0000 a901 722b 0000 00a9 02da 022e 3072  ....r+........0r
+00000ba0: 4100 0000 7217 0000 0072 1700 0000 7218  A...r....r....r.
+00000bb0: 0000 00da 093c 6765 6e65 7870 723e 6200  .....<genexpr>b.
+00000bc0: 0000 f308 0000 0002 8004 0002 0112 ff7a  ...............z
+00000bd0: 3253 6f75 7263 654d 6174 6368 6572 2e47  2SourceMatcher.G
+00000be0: 6574 5768 6974 6553 7061 6365 5465 7874  etWhiteSpaceText
+00000bf0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00000c00: 7072 3e29 01da 046a 6f69 6e29 0372 1500  pr>)...join).r..
+00000c10: 0000 da0a 696e 5f6d 6174 6368 6572 7222  ....in_matcherr"
+00000c20: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000c30: 0000 da11 4765 7457 6869 7465 5370 6163  ....GetWhiteSpac
+00000c40: 6554 6578 745f 0000 0073 0c00 0000 0401  eText_...s......
+00000c50: 0401 0a01 0201 08ff 0402 7a1f 536f 7572  ..........z.Sour
+00000c60: 6365 4d61 7463 6865 722e 4765 7457 6869  ceMatcher.GetWhi
+00000c70: 7465 5370 6163 6554 6578 7463 0100 0000  teSpaceTextc....
+00000c80: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000c90: 4300 0000 7316 0000 0064 01a0 0064 0264  C...s....d...d.d
+00000ca0: 0384 007c 006a 0144 0083 01a1 0153 0029  ...|.j.D.....S.)
+00000cb0: 044e 7208 0000 0063 0100 0000 0000 0000  .Nr....c........
+00000cc0: 0000 0000 0200 0000 0400 0000 7300 0000  ............s...
+00000cd0: 7243 0000 0072 2500 0000 7244 0000 0072  rC...r%...rD...r
+00000ce0: 4500 0000 7217 0000 0072 1700 0000 7218  E...r....r....r.
+00000cf0: 0000 0072 4700 0000 6800 0000 7248 0000  ...rG...h...rH..
+00000d00: 007a 3053 6f75 7263 654d 6174 6368 6572  .z0SourceMatcher
+00000d10: 2e47 6574 456e 6450 6172 656e 5465 7874  .GetEndParenText
+00000d20: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00000d30: 7072 3e29 0272 4900 0000 720a 0000 0072  pr>).rI...r....r
+00000d40: 2a00 0000 7217 0000 0072 1700 0000 7218  *...r....r....r.
+00000d50: 0000 00da 0f47 6574 456e 6450 6172 656e  .....GetEndParen
+00000d60: 5465 7874 6600 0000 7306 0000 000a 0204  Textf...s.......
+00000d70: 0108 ff7a 1d53 6f75 7263 654d 6174 6368  ...z.SourceMatch
+00000d80: 6572 2e47 6574 456e 6450 6172 656e 5465  er.GetEndParenTe
+00000d90: 7874 6301 0000 0000 0000 0000 0000 0002  xtc.............
+00000da0: 0000 0003 0000 0043 0000 0073 4a00 0000  .......C...sJ...
+00000db0: 7c00 6a00 6401 1900 7d01 7401 7c01 7402  |.j.d...}.t.|.t.
+00000dc0: 8302 7219 7c01 6a03 7215 7c01 0400 6a03  ..r.|.j.r.|...j.
+00000dd0: 6402 3700 0200 5f03 6e08 6402 7c01 5f03  d.7..._.n.d.|._.
+00000de0: 6e04 7404 6403 8301 8201 6400 7c00 5f05  n.t.d.....d.|._.
+00000df0: 6404 7c00 5f06 6400 5300 2905 4ee9 ffff  d.|._.d.S.).N...
+00000e00: ffff da01 0a7a 2a43 616e 6e6f 7420 6164  .....z*Cannot ad
+00000e10: 6420 6e65 776c 696e 6520 746f 206e 6f6e  d newline to non
+00000e20: 2d74 6578 7420 706c 6163 6568 6f6c 6465  -text placeholde
+00000e30: 7246 2907 da0e 6578 7065 6374 6564 5f70  rF)...expected_p
+00000e40: 6172 7473 da0a 6973 696e 7374 616e 6365  arts..isinstance
+00000e50: 7203 0000 0072 2d00 0000 7227 0000 0072  r....r-...r'...r
+00000e60: 1100 0000 7210 0000 0029 0272 1500 0000  ....r....).r....
+00000e70: da04 7061 7274 7217 0000 0072 1700 0000  ..partr....r....
+00000e80: 7218 0000 00da 1561 6464 5f6e 6577 6c69  r......add_newli
+00000e90: 6e65 5f74 6f5f 736f 7572 6365 6c00 0000  ne_to_sourcel...
+00000ea0: 7310 0000 000a 010a 0106 0110 0108 0208  s...............
+00000eb0: 0206 010a 017a 2353 6f75 7263 654d 6174  .....z#SourceMat
+00000ec0: 6368 6572 2e61 6464 5f6e 6577 6c69 6e65  cher.add_newline
+00000ed0: 5f74 6f5f 736f 7572 6365 6301 0000 0000  _to_sourcec.....
+00000ee0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000ef0: 0000 0073 4600 0000 7c00 6a00 720c 7c00  ...sF...|.j.r.|.
+00000f00: 6a01 6400 7500 720c 7402 6401 8301 8201  j.d.u.r.t.d.....
+00000f10: 7c00 6a00 7318 7c00 6a01 6400 7501 7218  |.j.s.|.j.d.u.r.
+00000f20: 7402 6402 8301 8201 7403 7c00 6403 8302  t.d.....t.|.d...
+00000f30: 7221 7402 6404 8301 8201 6400 5300 2905  r!t.d.....d.S.).
+00000f40: 4e7a 3e49 6e74 6572 6e61 6c20 4572 726f  Nz>Internal Erro
+00000f50: 723a 206d 6174 6368 6564 5f74 6578 7420  r: matched_text 
+00000f60: 6d75 7374 2062 6520 7365 7420 6966 2069  must be set if i
+00000f70: 735f 6d61 7463 6865 6420 6973 2054 7275  s_matched is Tru
+00000f80: 657a 4049 6e74 6572 6e61 6c20 4572 726f  ez@Internal Erro
+00000f90: 723a 206d 6174 6368 6564 5f74 6578 7420  r: matched_text 
+00000fa0: 6d75 7374 2062 6520 4e6f 6e65 2069 6620  must be None if 
+00000fb0: 6973 5f6d 6174 6368 6564 2069 7320 4661  is_matched is Fa
+00000fc0: 6c73 6572 2d00 0000 7a2b 496e 7465 726e  lser-...z+Intern
+00000fd0: 616c 2045 7272 6f72 3a20 646f 6e74 2068  al Error: dont h
+00000fe0: 6176 6520 7468 6973 2066 6965 6c64 202d  ave this field -
+00000ff0: 2065 7665 7229 0472 1000 0000 7211 0000   ever).r....r...
+00001000: 00da 0a56 616c 7565 4572 726f 72da 0768  ...ValueError..h
+00001010: 6173 6174 7472 722a 0000 0072 1700 0000  asattrr*...r....
+00001020: 7217 0000 0072 1800 0000 da17 7661 6c69  r....r......vali
+00001030: 6461 7465 645f 6361 6c6c 5f74 6f5f 6d61  dated_call_to_ma
+00001040: 7463 6877 0000 0073 0e00 0000 1001 0801  tchw...s........
+00001050: 1001 0801 0a01 0801 04ff 7a25 536f 7572  ..........z%Sour
+00001060: 6365 4d61 7463 6865 722e 7661 6c69 6461  ceMatcher.valida
+00001070: 7465 645f 6361 6c6c 5f74 6f5f 6d61 7463  ted_call_to_matc
+00001080: 6863 0200 0000 0000 0000 0000 0000 0500  hc..............
+00001090: 0000 0300 0000 4300 0000 7348 0000 0064  ......C...sH...d
+000010a0: 0104 007d 027d 037c 0144 005d 137d 047c  ...}.}.|.D.].}.|
+000010b0: 0464 026b 0272 117c 0264 0337 007d 0271  .d.k.r.|.d.7.}.q
+000010c0: 067c 0464 046b 0272 197c 0364 0337 007d  .|.d.k.r.|.d.7.}
+000010d0: 0371 067c 027c 036b 0372 2274 0064 0583  .q.|.|.k.r"t.d..
+000010e0: 0182 0164 0053 0029 064e 7201 0000 00fa  ...d.S.).Nr.....
+000010f0: 0128 7238 0000 00fa 0129 7a16 756e 6261  .(r8.....)z.unba
+00001100: 6c61 6e63 6564 2070 6172 656e 7468 6573  lanced parenthes
+00001110: 6573 7205 0000 0029 0572 1500 0000 7221  esr....).r....r!
+00001120: 0000 00da 046c 6566 74da 0572 6967 6874  .....left..right
+00001130: da01 6372 1700 0000 7217 0000 0072 1800  ..cr....r....r..
+00001140: 0000 721a 0000 007f 0000 0073 1400 0000  ..r........s....
+00001150: 0801 0801 0801 0a01 0801 0801 0280 0802  ................
+00001160: 0801 04ff 7a28 536f 7572 6365 4d61 7463  ....z(SourceMatc
+00001170: 6865 722e 5f63 6865 636b 5f62 616c 616e  her._check_balan
+00001180: 6365 5f70 6172 656e 7468 6573 6573 7225  ce_parenthesesr%
+00001190: 0000 0029 0146 2914 da08 5f5f 6e61 6d65  ...).F)...__name
+000011a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000011b0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
+000011c0: 646f 635f 5f72 0200 0000 7212 0000 0072  doc__r....r....r
+000011d0: 1900 0000 7223 0000 0072 1c00 0000 722b  ....r#...r....r+
+000011e0: 0000 0072 3100 0000 7233 0000 0072 3600  ...r1...r3...r6.
+000011f0: 0000 7240 0000 0072 4200 0000 724b 0000  ..r@...rB...rK..
+00001200: 0072 4c00 0000 7252 0000 0072 5500 0000  .rL...rR...rU...
+00001210: 721a 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00001220: 1700 0000 7218 0000 0072 0700 0000 0a00  ....r....r......
+00001230: 0000 7322 0000 0008 0004 0106 040a 0108  ..s"............
+00001240: 0f08 0c08 0308 040a 0b08 050a 0608 1108  ................
+00001250: 0608 0708 0608 0b0c 0872 0700 0000 290c  .........r....).
+00001260: 721e 0000 0072 3900 0000 da2a 6675 6e5f  r....r9....*fun_
+00001270: 7769 7468 5f61 7374 2e63 6f6d 6d6f 6e5f  with_ast.common_
+00001280: 7574 696c 732e 7061 7265 6e74 6865 7365  utils.parenthese
+00001290: 5f73 7461 636b 7202 0000 00da 1e66 756e  _stackr......fun
+000012a0: 5f77 6974 685f 6173 742e 706c 6163 6568  _with_ast.placeh
+000012b0: 6f6c 6465 7273 2e74 6578 7472 0300 0000  olders.textr....
+000012c0: da24 6675 6e5f 7769 7468 5f61 7374 2e70  .$fun_with_ast.p
+000012d0: 6c61 6365 686f 6c64 6572 732e 7768 6974  laceholders.whit
+000012e0: 6573 7061 6365 7204 0000 00da 2766 756e  espacer.....'fun
+000012f0: 5f77 6974 685f 6173 742e 736f 7572 6365  _with_ast.source
+00001300: 5f6d 6174 6368 6572 732e 6578 6365 7074  _matchers.except
+00001310: 696f 6e73 7206 0000 00da 066f 626a 6563  ionsr......objec
+00001320: 7472 0700 0000 7217 0000 0072 1700 0000  tr....r....r....
+00001330: 7217 0000 0072 1800 0000 da08 3c6d 6f64  r....r......<mod
+00001340: 756c 653e 0100 0000 730e 0000 0008 0008  ule>....s.......
+00001350: 010c 020c 010c 010c 0114 03              ...........
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/body.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/body.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun  5 18:28:40 2023 UTC, .py size: 3070 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5829 7e64 fe0b 0000  o.......X)~d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 030c 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6501 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 01da  Z.d.S.)......)..
@@ -145,19 +145,20 @@
 00000900: 5f5f 636c 6173 7363 656c 6c5f 5f72 1100  __classcell__r..
 00000910: 0000 7211 0000 0072 0f00 0000 7212 0000  ..r....r....r...
 00000920: 0072 0700 0000 0700 0000 730e 0000 0008  .r........s.....
 00000930: 0004 010c 0208 0408 0808 1f10 0772 0700  .............r..
 00000940: 0000 4e29 0ada 2a66 756e 5f77 6974 685f  ..N)..*fun_with_
 00000950: 6173 742e 706c 6163 6568 6f6c 6465 7273  ast.placeholders
 00000960: 2e6c 6973 745f 706c 6163 6568 6f6c 6465  .list_placeholde
-00000970: 7272 0200 0000 da28 6675 6e5f 7769 7468  rr.....(fun_with
+00000970: 7272 0200 0000 da32 6675 6e5f 7769 7468  rr.....2fun_with
 00000980: 5f61 7374 2e6d 616e 6970 756c 6174 655f  _ast.manipulate_
-00000990: 6e6f 6465 2e63 7265 6174 655f 6e6f 6465  node.create_node
-000009a0: 7203 0000 00da 1766 756e 5f77 6974 685f  r......fun_with_
-000009b0: 6173 742e 6765 745f 736f 7572 6365 7204  ast.get_sourcer.
-000009c0: 0000 00da 2966 756e 5f77 6974 685f 6173  ....)fun_with_as
-000009d0: 742e 736f 7572 6365 5f6d 6174 6368 6572  t.source_matcher
-000009e0: 732e 6261 7365 5f6d 6174 6368 6572 7205  s.base_matcherr.
-000009f0: 0000 0072 0600 0000 7207 0000 0072 1100  ...r....r....r..
-00000a00: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000a10: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000a20: 0a00 0000 0c00 0c01 0c01 1001 1403       ..............
+00000990: 6e6f 6465 2e73 796e 7461 785f 6672 6565  node.syntax_free
+000009a0: 5f6c 696e 655f 6e6f 6465 7203 0000 00da  _line_noder.....
+000009b0: 1766 756e 5f77 6974 685f 6173 742e 6765  .fun_with_ast.ge
+000009c0: 745f 736f 7572 6365 7204 0000 00da 2466  t_sourcer.....$f
+000009d0: 756e 5f77 6974 685f 6173 742e 706c 6163  un_with_ast.plac
+000009e0: 6568 6f6c 6465 7273 2e62 6173 655f 6d61  eholders.base_ma
+000009f0: 7463 6872 0500 0000 7206 0000 0072 0700  tchr....r....r..
+00000a00: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
+00000a10: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000a20: 0100 0000 730a 0000 000c 000c 010c 0110  ....s...........
+00000a30: 0114 03                                  ...
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/boolop.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/boolop.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 15:40:06 2023 UTC, .py size: 7123 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,153 +1,139 @@
-00000000: 6f0d 0d0a 0000 0000 56f6 8164 d31b 0000  o.......V..d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 5409 0000  o..........dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
-00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6400  m.Z.m.Z.m.Z...d.
-00000070: 6405 6c0c 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
-00000080: 6d0f 5a0f 6d10 5a10 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
-00000090: 8400 6408 6503 8303 5a11 6409 5300 290a  ..d.e...Z.d.S.).
-000000a0: e900 0000 0029 01da 0947 6574 536f 7572  .....)...GetSour
-000000b0: 6365 2903 da0d 536f 7572 6365 4d61 7463  ce)...SourceMatc
-000000c0: 6865 72da 104d 6174 6368 506c 6163 6568  her..MatchPlaceh
-000000d0: 6f6c 6465 72da 0b66 756c 6c5f 7374 7269  older..full_stri
-000000e0: 6e67 2901 da0c 5374 7269 6e67 5061 7273  ng)...StringPars
-000000f0: 6572 2903 da0f 5465 7874 506c 6163 6568  er)...TextPlaceh
-00000100: 6f6c 6465 72da 0f45 6e64 5061 7265 6e4d  older..EndParenM
-00000110: 6174 6368 6572 da11 5374 6172 7450 6172  atcher..StartPar
-00000120: 656e 4d61 7463 6865 7229 01da 0f5f 4765  enMatcher)..._Ge
-00000130: 744c 6973 7444 6566 6175 6c74 2902 da1b  tListDefault)...
-00000140: 4261 646c 7953 7065 6369 6669 6564 5465  BadlySpecifiedTe
-00000150: 6d70 6c61 7465 4572 726f 72da 1345 6d70  mplateError..Emp
-00000160: 7479 5374 6163 6b45 7863 6570 7469 6f6e  tyStackException
-00000170: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000180: 0004 0000 0000 0000 0073 3a00 0000 6500  .........s:...e.
-00000190: 5a01 6400 5a02 6401 5a03 640b 8700 6601  Z.d.Z.d.Z.d...f.
-000001a0: 6403 6404 8409 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
-000001b0: 6407 6408 8400 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
-000001c0: 8700 0400 5a08 5300 290c da13 426f 6f6c  ....Z.S.)...Bool
-000001d0: 4f70 536f 7572 6365 4d61 7463 6865 727a  OpSourceMatcherz
-000001e0: 3543 6c61 7373 2074 6f20 6765 6e65 7261  5Class to genera
-000001f0: 7465 2074 6865 2073 6f75 7263 6520 666f  te the source fo
-00000200: 7220 616e 205f 6173 742e 426f 6f6c 4f70  r an _ast.BoolOp
-00000210: 206e 6f64 652e 4e63 0400 0000 0000 0000   node.Nc........
-00000220: 0000 0000 0400 0000 0400 0000 0300 0000  ................
-00000230: 7328 0000 0074 0074 017c 0083 02a0 027c  s(...t.t.|.....|
-00000240: 017c 02a1 0201 0074 0364 0164 0283 027c  .|.....t.d.d...|
-00000250: 005f 0467 007c 005f 0564 0053 0029 034e  ._.g.|._.d.S.).N
-00000260: 7a03 5c73 2afa 0120 2906 da05 7375 7065  z.\s*.. )...supe
-00000270: 7272 0d00 0000 da08 5f5f 696e 6974 5f5f  rr......__init__
-00000280: 7207 0000 00da 1573 6570 6172 6174 6f72  r......separator
-00000290: 5f70 6c61 6365 686f 6c64 6572 da14 6d61  _placeholder..ma
-000002a0: 7463 6865 645f 706c 6163 6568 6f6c 6465  tched_placeholde
-000002b0: 7273 2904 da04 7365 6c66 da04 6e6f 6465  rs)...self..node
-000002c0: da0f 7374 6172 7469 6e67 5f70 6172 656e  ..starting_paren
-000002d0: 73da 0670 6172 656e 74a9 01da 095f 5f63  s..parent....__c
-000002e0: 6c61 7373 5f5f a900 fa3e 2f68 6f6d 652f  lass__...>/home/
-000002f0: 7368 6169 2f66 756e 5f77 6974 685f 6173  shai/fun_with_as
-00000300: 742f 6675 6e5f 7769 7468 5f61 7374 2f73  t/fun_with_ast/s
-00000310: 6f75 7263 655f 6d61 7463 6865 7273 2f62  ource_matchers/b
-00000320: 6f6f 6c6f 702e 7079 7210 0000 000c 0000  oolop.pyr.......
-00000330: 0073 0600 0000 1201 0c01 0a01 7a1c 426f  .s..........z.Bo
-00000340: 6f6c 4f70 536f 7572 6365 4d61 7463 6865  olOpSourceMatche
-00000350: 722e 5f5f 696e 6974 5f5f 6301 0000 0000  r.__init__c.....
-00000360: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000370: 0000 0073 1a00 0000 7c00 6a00 a001 a100  ...s....|.j.....
-00000380: 7d01 7c00 6a02 a003 7c01 a101 0100 7c01  }.|.j...|.....|.
-00000390: 5300 2901 4e29 0472 1100 0000 da04 436f  S.).N).r......Co
-000003a0: 7079 7212 0000 00da 0661 7070 656e 6429  pyr......append)
-000003b0: 0272 1300 0000 da04 636f 7079 7219 0000  .r......copyr...
-000003c0: 0072 1900 0000 721a 0000 00da 1047 6574  .r....r......Get
-000003d0: 5365 7061 7261 746f 7243 6f70 7911 0000  SeparatorCopy...
-000003e0: 0073 0600 0000 0a01 0c01 0401 7a24 426f  .s..........z$Bo
-000003f0: 6f6c 4f70 536f 7572 6365 4d61 7463 6865  olOpSourceMatche
-00000400: 722e 4765 7453 6570 6172 6174 6f72 436f  r.GetSeparatorCo
-00000410: 7079 6302 0000 0000 0000 0000 0000 0008  pyc.............
-00000420: 0000 0005 0000 0043 0000 0073 9600 0000  .......C...s....
-00000430: 7c00 a000 7c01 a101 7d02 7c00 6a01 6a02  |...|...}.|.j.j.
-00000440: 6401 1900 6701 7d03 7c00 6a01 6a02 6402  d...g.}.|.j.j.d.
-00000450: 6400 8502 1900 4400 5d1c 7d04 7c03 a003  d.....D.].}.|...
-00000460: 7c00 a004 a100 a101 0100 7c03 a003 7c00  |.........|...|.
-00000470: 6a01 6a05 a101 0100 7c03 a003 7c00 a004  j.j.....|...|...
-00000480: a100 a101 0100 7c03 a003 7c04 a101 0100  ......|...|.....
-00000490: 7114 7406 7c02 7c03 8302 7d05 6403 a007  q.t.|.|...}.d...
-000004a0: 7c05 6a08 a101 7d06 7c05 6a09 7d02 7c00  |.j...}.|.j.}.|.
-000004b0: a00a 7c02 a101 0100 740b a00c 7c00 a101  ..|.....t...|...
-000004c0: 7d07 7c07 5300 a904 4e72 0100 0000 e901  }.|.S...Nr......
-000004d0: 0000 00da 0029 0dda 104d 6174 6368 5374  .....)...MatchSt
-000004e0: 6172 7450 6172 656e 7372 1400 0000 da06  artParensr......
-000004f0: 7661 6c75 6573 721c 0000 0072 1e00 0000  valuesr....r....
-00000500: da02 6f70 7206 0000 00da 046a 6f69 6eda  ..opr......join.
-00000510: 126d 6174 6368 6564 5f73 7562 7374 7269  .matched_substri
-00000520: 6e67 73da 1072 656d 6169 6e69 6e67 5f73  ngs..remaining_s
-00000530: 7472 696e 67da 0d4d 6174 6368 456e 6450  tring..MatchEndP
-00000540: 6172 656e 720d 0000 0072 0200 0000 2908  arenr....r....).
-00000550: 7213 0000 00da 0673 7472 696e 6772 2700  r......stringr'.
-00000560: 0000 da08 656c 656d 656e 7473 da05 7661  ....elements..va
-00000570: 6c75 65da 0670 6172 7365 72da 0c6d 6174  lue..parser..mat
-00000580: 6368 6564 5f74 6578 74da 0672 6573 756c  ched_text..resul
-00000590: 7472 1900 0000 7219 0000 0072 1a00 0000  tr....r....r....
-000005a0: da06 5f6d 6174 6368 1600 0000 731a 0000  .._match....s...
-000005b0: 000a 010e 0214 010e 010e 010e 010c 010a  ................
-000005c0: 030c 0106 010a 020a 0304 017a 1a42 6f6f  ...........z.Boo
-000005d0: 6c4f 7053 6f75 7263 654d 6174 6368 6572  lOpSourceMatcher
-000005e0: 2e5f 6d61 7463 6863 0100 0000 0000 0000  ._matchc........
-000005f0: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
-00000600: 73c2 0000 0067 007d 017c 01a0 007c 00a0  s....g.}.|...|..
-00000610: 01a1 00a1 0101 007c 01a0 0074 027c 006a  .......|...t.|.j
-00000620: 036a 0464 0119 0083 01a1 0101 0064 017d  .j.d.........d.}
-00000630: 027c 006a 036a 0464 0264 0085 0219 0044  .|.j.j.d.d.....D
-00000640: 005d 367d 037c 01a0 0074 057c 006a 067c  .]6}.|...t.|.j.|
-00000650: 027c 006a 0783 03a0 0264 00a1 01a1 0101  .|.j.....d......
-00000660: 007c 01a0 0074 027c 006a 036a 0883 01a1  .|...t.|.j.j....
-00000670: 0101 007c 0264 0237 007d 027c 01a0 0074  ...|.d.7.}.|...t
-00000680: 057c 006a 067c 027c 006a 0783 03a0 0264  .|.j.|.|.j.....d
-00000690: 00a1 01a1 0101 007c 01a0 0074 027c 0383  .......|...t.|..
-000006a0: 01a1 0101 007c 0264 0237 007d 0271 1e7c  .....|.d.7.}.q.|
-000006b0: 01a0 007c 00a0 09a1 00a1 0101 0064 03a0  ...|.........d..
-000006c0: 0a7c 01a1 0153 0072 1f00 0000 290b 721c  .|...S.r....).r.
-000006d0: 0000 00da 1147 6574 5374 6172 7450 6172  .....GetStartPar
-000006e0: 656e 5465 7874 7202 0000 0072 1400 0000  enTextr....r....
-000006f0: 7223 0000 0072 0a00 0000 7212 0000 0072  r#...r....r....r
-00000700: 1100 0000 7224 0000 00da 0f47 6574 456e  ....r$.....GetEn
-00000710: 6450 6172 656e 5465 7874 7225 0000 0029  dParenTextr%...)
-00000720: 0472 1300 0000 da0b 736f 7572 6365 5f6c  .r......source_l
-00000730: 6973 74da 0569 6e64 6578 722b 0000 0072  ist..indexr+...r
-00000740: 1900 0000 7219 0000 0072 1a00 0000 7202  ....r....r....r.
-00000750: 0000 002a 0000 0073 3200 0000 0401 0e03  ...*...s2.......
-00000760: 1602 0401 1401 0601 0401 0201 0401 02fd  ................
-00000770: 0603 04fd 1204 0801 0601 0401 0201 0401  ................
-00000780: 02fd 0603 04fd 0e04 0a01 0e02 0a01 7a1d  ..............z.
-00000790: 426f 6f6c 4f70 536f 7572 6365 4d61 7463  BoolOpSourceMatc
-000007a0: 6865 722e 4765 7453 6f75 7263 6529 024e  her.GetSource).N
-000007b0: 4e29 09da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000007c0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000007d0: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-000007e0: 7210 0000 0072 1e00 0000 722f 0000 0072  r....r....r/...r
-000007f0: 0200 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00000800: 6c5f 5f72 1900 0000 7219 0000 0072 1700  l__r....r....r..
-00000810: 0000 721a 0000 0072 0d00 0000 0900 0000  ..r....r........
-00000820: 730c 0000 0008 0004 010e 0208 0508 0510  s...............
-00000830: 1472 0d00 0000 4e29 12da 1766 756e 5f77  .r....N)...fun_w
-00000840: 6974 685f 6173 742e 6765 745f 736f 7572  ith_ast.get_sour
-00000850: 6365 7202 0000 00da 2966 756e 5f77 6974  cer.....)fun_wit
-00000860: 685f 6173 742e 736f 7572 6365 5f6d 6174  h_ast.source_mat
-00000870: 6368 6572 732e 6261 7365 5f6d 6174 6368  chers.base_match
-00000880: 6572 7203 0000 0072 0400 0000 7205 0000  err....r....r...
-00000890: 00da 2766 756e 5f77 6974 685f 6173 742e  ..'fun_with_ast.
-000008a0: 706c 6163 6568 6f6c 6465 7273 2e73 7472  placeholders.str
-000008b0: 696e 675f 7061 7273 6572 7206 0000 00da  ing_parserr.....
-000008c0: 1e66 756e 5f77 6974 685f 6173 742e 706c  .fun_with_ast.pl
-000008d0: 6163 6568 6f6c 6465 7273 2e74 6578 7472  aceholders.textr
-000008e0: 0700 0000 7208 0000 0072 0900 0000 da2c  ....r....r.....,
-000008f0: 6675 6e5f 7769 7468 5f61 7374 2e63 6f6d  fun_with_ast.com
-00000900: 6d6f 6e5f 7574 696c 732e 7574 696c 735f  mon_utils.utils_
-00000910: 736f 7572 6365 5f6d 6174 6368 720a 0000  source_matchr...
-00000920: 00da 2766 756e 5f77 6974 685f 6173 742e  ..'fun_with_ast.
-00000930: 736f 7572 6365 5f6d 6174 6368 6572 732e  source_matchers.
-00000940: 6578 6365 7074 696f 6e73 720b 0000 0072  exceptionsr....r
-00000950: 0c00 0000 720d 0000 0072 1900 0000 7219  ....r....r....r.
-00000960: 0000 0072 1900 0000 721a 0000 00da 083c  ...r....r......<
-00000970: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-00000980: 0c00 1401 0c01 1401 0c01 1001 1403       ..............
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 0100 4700 6406 6407  d.l.m.Z...G.d.d.
+00000070: 8400 6407 6509 8303 5a0a 6408 5300 2909  ..d.e...Z.d.S.).
+00000080: e900 0000 0029 01da 0f5f 4765 744c 6973  .....)..._GetLis
+00000090: 7444 6566 6175 6c74 2901 da09 4765 7453  tDefault)...GetS
+000000a0: 6f75 7263 6529 01da 0c53 7472 696e 6750  ource)...StringP
+000000b0: 6172 7365 7229 01da 0f54 6578 7450 6c61  arser)...TextPla
+000000c0: 6365 686f 6c64 6572 2901 da0d 536f 7572  ceholder)...Sour
+000000d0: 6365 4d61 7463 6865 7263 0000 0000 0000  ceMatcherc......
+000000e0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+000000f0: 0000 733a 0000 0065 005a 0164 005a 0264  ..s:...e.Z.d.Z.d
+00000100: 015a 0364 0b87 0066 0164 0364 0484 095a  .Z.d...f.d.d...Z
+00000110: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
+00000120: 0664 0964 0a84 005a 0787 0004 005a 0853  .d.d...Z.....Z.S
+00000130: 0029 0cda 1342 6f6f 6c4f 7053 6f75 7263  .)...BoolOpSourc
+00000140: 654d 6174 6368 6572 7a35 436c 6173 7320  eMatcherz5Class 
+00000150: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
+00000160: 736f 7572 6365 2066 6f72 2061 6e20 5f61  source for an _a
+00000170: 7374 2e42 6f6f 6c4f 7020 6e6f 6465 2e4e  st.BoolOp node.N
+00000180: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00000190: 0004 0000 0003 0000 0073 2800 0000 7400  .........s(...t.
+000001a0: 7401 7c00 8302 a002 7c01 7c02 a102 0100  t.|.....|.|.....
+000001b0: 7403 6401 6402 8302 7c00 5f04 6700 7c00  t.d.d...|._.g.|.
+000001c0: 5f05 6400 5300 2903 4e7a 035c 732a fa01  _.d.S.).Nz.\s*..
+000001d0: 2029 06da 0573 7570 6572 7207 0000 00da   )...superr.....
+000001e0: 085f 5f69 6e69 745f 5f72 0500 0000 da15  .__init__r......
+000001f0: 7365 7061 7261 746f 725f 706c 6163 6568  separator_placeh
+00000200: 6f6c 6465 72da 146d 6174 6368 6564 5f70  older..matched_p
+00000210: 6c61 6365 686f 6c64 6572 7329 04da 0473  laceholders)...s
+00000220: 656c 66da 046e 6f64 65da 0f73 7461 7274  elf..node..start
+00000230: 696e 675f 7061 7265 6e73 da06 7061 7265  ing_parens..pare
+00000240: 6e74 a901 da09 5f5f 636c 6173 735f 5fa9  nt....__class__.
+00000250: 00fa 3e2f 686f 6d65 2f73 6861 692f 6675  ..>/home/shai/fu
+00000260: 6e5f 7769 7468 5f61 7374 2f66 756e 5f77  n_with_ast/fun_w
+00000270: 6974 685f 6173 742f 736f 7572 6365 5f6d  ith_ast/source_m
+00000280: 6174 6368 6572 732f 626f 6f6c 6f70 2e70  atchers/boolop.p
+00000290: 7972 0a00 0000 0b00 0000 7306 0000 0012  yr........s.....
+000002a0: 010c 010a 017a 1c42 6f6f 6c4f 7053 6f75  .....z.BoolOpSou
+000002b0: 7263 654d 6174 6368 6572 2e5f 5f69 6e69  rceMatcher.__ini
+000002c0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+000002d0: 0200 0000 0300 0000 4300 0000 731a 0000  ........C...s...
+000002e0: 007c 006a 00a0 01a1 007d 017c 006a 02a0  .|.j.....}.|.j..
+000002f0: 037c 01a1 0101 007c 0153 0029 014e 2904  .|.....|.S.).N).
+00000300: 720b 0000 00da 0443 6f70 7972 0c00 0000  r......Copyr....
+00000310: da06 6170 7065 6e64 2902 720d 0000 00da  ..append).r.....
+00000320: 0463 6f70 7972 1300 0000 7213 0000 0072  .copyr....r....r
+00000330: 1400 0000 da10 4765 7453 6570 6172 6174  ......GetSeparat
+00000340: 6f72 436f 7079 1000 0000 7306 0000 000a  orCopy....s.....
+00000350: 010c 0104 017a 2442 6f6f 6c4f 7053 6f75  .....z$BoolOpSou
+00000360: 7263 654d 6174 6368 6572 2e47 6574 5365  rceMatcher.GetSe
+00000370: 7061 7261 746f 7243 6f70 7963 0200 0000  paratorCopyc....
+00000380: 0000 0000 0000 0000 0800 0000 0500 0000  ................
+00000390: 4300 0000 7396 0000 007c 00a0 007c 01a1  C...s....|...|..
+000003a0: 017d 027c 006a 016a 0264 0119 0067 017d  .}.|.j.j.d...g.}
+000003b0: 037c 006a 016a 0264 0264 0085 0219 0044  .|.j.j.d.d.....D
+000003c0: 005d 1c7d 047c 03a0 037c 00a0 04a1 00a1  .].}.|...|......
+000003d0: 0101 007c 03a0 037c 006a 016a 05a1 0101  ...|...|.j.j....
+000003e0: 007c 03a0 037c 00a0 04a1 00a1 0101 007c  .|...|.........|
+000003f0: 03a0 037c 04a1 0101 0071 1474 067c 027c  ...|.....q.t.|.|
+00000400: 0383 027d 0564 03a0 077c 056a 08a1 017d  ...}.d...|.j...}
+00000410: 067c 056a 097d 027c 00a0 0a7c 02a1 0101  .|.j.}.|...|....
+00000420: 0074 0ba0 0c7c 00a1 017d 077c 0753 00a9  .t...|...}.|.S..
+00000430: 044e 7201 0000 00e9 0100 0000 da00 290d  .Nr...........).
+00000440: da10 4d61 7463 6853 7461 7274 5061 7265  ..MatchStartPare
+00000450: 6e73 720e 0000 00da 0676 616c 7565 7372  nsr......valuesr
+00000460: 1600 0000 7218 0000 00da 026f 7072 0400  ....r......opr..
+00000470: 0000 da04 6a6f 696e da12 6d61 7463 6865  ....join..matche
+00000480: 645f 7375 6273 7472 696e 6773 da10 7265  d_substrings..re
+00000490: 6d61 696e 696e 675f 7374 7269 6e67 da0d  maining_string..
+000004a0: 4d61 7463 6845 6e64 5061 7265 6e72 0700  MatchEndParenr..
+000004b0: 0000 7203 0000 0029 0872 0d00 0000 da06  ..r....).r......
+000004c0: 7374 7269 6e67 7221 0000 00da 0865 6c65  stringr!.....ele
+000004d0: 6d65 6e74 73da 0576 616c 7565 da06 7061  ments..value..pa
+000004e0: 7273 6572 da0c 6d61 7463 6865 645f 7465  rser..matched_te
+000004f0: 7874 da06 7265 7375 6c74 7213 0000 0072  xt..resultr....r
+00000500: 1300 0000 7214 0000 00da 065f 6d61 7463  ....r......_matc
+00000510: 6815 0000 0073 1a00 0000 0a01 0e02 1401  h....s..........
+00000520: 0e01 0e01 0e01 0c01 0a03 0c01 0601 0a02  ................
+00000530: 0a01 0401 7a1a 426f 6f6c 4f70 536f 7572  ....z.BoolOpSour
+00000540: 6365 4d61 7463 6865 722e 5f6d 6174 6368  ceMatcher._match
+00000550: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000560: 0007 0000 0043 0000 0073 c200 0000 6700  .....C...s....g.
+00000570: 7d01 7c01 a000 7c00 a001 a100 a101 0100  }.|...|.........
+00000580: 7c01 a000 7402 7c00 6a03 6a04 6401 1900  |...t.|.j.j.d...
+00000590: 8301 a101 0100 6401 7d02 7c00 6a03 6a04  ......d.}.|.j.j.
+000005a0: 6402 6400 8502 1900 4400 5d36 7d03 7c01  d.d.....D.]6}.|.
+000005b0: a000 7405 7c00 6a06 7c02 7c00 6a07 8303  ..t.|.j.|.|.j...
+000005c0: a002 6400 a101 a101 0100 7c01 a000 7402  ..d.......|...t.
+000005d0: 7c00 6a03 6a08 8301 a101 0100 7c02 6402  |.j.j.......|.d.
+000005e0: 3700 7d02 7c01 a000 7405 7c00 6a06 7c02  7.}.|...t.|.j.|.
+000005f0: 7c00 6a07 8303 a002 6400 a101 a101 0100  |.j.....d.......
+00000600: 7c01 a000 7402 7c03 8301 a101 0100 7c02  |...t.|.......|.
+00000610: 6402 3700 7d02 711e 7c01 a000 7c00 a009  d.7.}.q.|...|...
+00000620: a100 a101 0100 6403 a00a 7c01 a101 5300  ......d...|...S.
+00000630: 7219 0000 0029 0b72 1600 0000 da11 4765  r....).r......Ge
+00000640: 7453 7461 7274 5061 7265 6e54 6578 7472  tStartParenTextr
+00000650: 0300 0000 720e 0000 0072 1d00 0000 7202  ....r....r....r.
+00000660: 0000 0072 0c00 0000 720b 0000 0072 1e00  ...r....r....r..
+00000670: 0000 da0f 4765 7445 6e64 5061 7265 6e54  ....GetEndParenT
+00000680: 6578 7472 1f00 0000 2904 720d 0000 00da  extr....).r.....
+00000690: 0b73 6f75 7263 655f 6c69 7374 da05 696e  .source_list..in
+000006a0: 6465 7872 2500 0000 7213 0000 0072 1300  dexr%...r....r..
+000006b0: 0000 7214 0000 0072 0300 0000 2700 0000  ..r....r....'...
+000006c0: 7332 0000 0004 010e 0116 0204 0114 0106  s2..............
+000006d0: 0104 0102 0104 0102 fd06 0304 fd12 0408  ................
+000006e0: 0106 0104 0102 0104 0102 fd06 0304 fd0e  ................
+000006f0: 040a 010e 020a 017a 1d42 6f6f 6c4f 7053  .......z.BoolOpS
+00000700: 6f75 7263 654d 6174 6368 6572 2e47 6574  ourceMatcher.Get
+00000710: 536f 7572 6365 2902 4e4e 2909 da08 5f5f  Source).NN)...__
+00000720: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000730: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000740: da07 5f5f 646f 635f 5f72 0a00 0000 7218  ..__doc__r....r.
+00000750: 0000 0072 2900 0000 7203 0000 00da 0d5f  ...r)...r......_
+00000760: 5f63 6c61 7373 6365 6c6c 5f5f 7213 0000  _classcell__r...
+00000770: 0072 1300 0000 7211 0000 0072 1400 0000  .r....r....r....
+00000780: 7207 0000 0008 0000 0073 0c00 0000 0800  r........s......
+00000790: 0401 0e02 0805 0805 1012 7207 0000 004e  ..........r....N
+000007a0: 290b da2c 6675 6e5f 7769 7468 5f61 7374  )..,fun_with_ast
+000007b0: 2e63 6f6d 6d6f 6e5f 7574 696c 732e 7574  .common_utils.ut
+000007c0: 696c 735f 736f 7572 6365 5f6d 6174 6368  ils_source_match
+000007d0: 7202 0000 00da 1766 756e 5f77 6974 685f  r......fun_with_
+000007e0: 6173 742e 6765 745f 736f 7572 6365 7203  ast.get_sourcer.
+000007f0: 0000 00da 2766 756e 5f77 6974 685f 6173  ....'fun_with_as
+00000800: 742e 706c 6163 6568 6f6c 6465 7273 2e73  t.placeholders.s
+00000810: 7472 696e 675f 7061 7273 6572 7204 0000  tring_parserr...
+00000820: 00da 1e66 756e 5f77 6974 685f 6173 742e  ...fun_with_ast.
+00000830: 706c 6163 6568 6f6c 6465 7273 2e74 6578  placeholders.tex
+00000840: 7472 0500 0000 da29 6675 6e5f 7769 7468  tr.....)fun_with
+00000850: 5f61 7374 2e73 6f75 7263 655f 6d61 7463  _ast.source_matc
+00000860: 6865 7273 2e62 6173 655f 6d61 7463 6865  hers.base_matche
+00000870: 7272 0600 0000 7207 0000 0072 1300 0000  rr....r....r....
+00000880: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00000890: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
+000008a0: 0000 0c00 0c01 0c01 0c01 0c01 1403       ..............
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/constant_source_match.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/constant_source_match.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 11 17:26:14 2023 UTC, .py size: 2506 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b603 8664 ca09 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 a9d1 ae64 3209 0000  o..........d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6506 8303  ..G.d.d...d.e...
@@ -16,109 +16,111 @@
 000000f0: 6572 6300 0000 0000 0000 0000 0000 0000  erc.............
 00000100: 0000 0003 0000 0040 0000 0073 2600 0000  .......@...s&...
 00000110: 6500 5a01 6400 5a02 6408 6402 6403 8401  e.Z.d.Z.d.d.d...
 00000120: 5a03 6404 6405 8400 5a04 6406 6407 8400  Z.d.d...Z.d.d...
 00000130: 5a05 6401 5300 2909 da15 436f 6e73 7461  Z.d.S.)...Consta
 00000140: 6e74 536f 7572 6365 4d61 7463 6865 724e  ntSourceMatcherN
 00000150: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00000160: 0006 0000 0043 0000 0073 8600 0000 7400  .....C...s....t.
+00000160: 0006 0000 0043 0000 0073 9c00 0000 7400  .....C...s....t.
 00000170: a001 7c00 7c01 a102 0100 7402 7c01 7403  ..|.|.....t.|.t.
 00000180: 6a04 8302 730e 7405 8201 7406 7c01 7407  j...s.t...t.|.t.
 00000190: 6401 8301 7408 6402 6403 8302 6702 8302  d...t.d.d...g...
 000001a0: 7c00 5f09 7406 7c01 7407 6401 8301 7408  |._.t.|.t.d...t.
 000001b0: 6402 6403 8302 6702 8302 7c00 5f0a 7c03  d.d...g...|._.|.
 000001c0: 7c00 5f0b 7402 7c00 6a0b 7403 6a0c 8302  |._.t.|.j.t.j...
 000001d0: 7236 6404 7c00 5f0d 6e03 6405 7c00 5f0d  r6d.|._.n.d.|._.
-000001e0: 740e 7c01 7c02 7c00 6a0d 8303 7c00 5f0f  t.|.|.|.j...|._.
-000001f0: 6400 5300 2906 4eda 0576 616c 7565 7a10  d.S.).N..valuez.
-00000200: 5b20 5c74 5d2a 2823 2b2e 2a29 2a5c 6e3f  [ \t]*(#+.*)*\n?
-00000210: da00 4654 2910 7204 0000 00da 085f 5f69  ..FT).r......__i
-00000220: 6e69 745f 5fda 0a69 7369 6e73 7461 6e63  nit__..isinstanc
-00000230: 65da 0361 7374 da08 436f 6e73 7461 6e74  e..ast..Constant
-00000240: da0a 5661 6c75 6545 7272 6f72 7205 0000  ..ValueErrorr...
-00000250: 0072 0200 0000 7203 0000 00da 0b6e 756d  .r....r......num
-00000260: 5f6d 6174 6368 6572 da0c 626f 6f6c 5f6d  _matcher..bool_m
-00000270: 6174 6368 6572 da0b 7061 7265 6e74 5f6e  atcher..parent_n
-00000280: 6f64 65da 094a 6f69 6e65 6453 7472 da18  ode..JoinedStr..
-00000290: 6163 6365 7074 5f6d 756c 7469 7061 7274  accept_multipart
-000002a0: 735f 7374 7269 6e67 7206 0000 00da 0b73  s_stringr......s
-000002b0: 7472 5f6d 6174 6368 6572 2904 da04 7365  tr_matcher)...se
-000002c0: 6c66 da04 6e6f 6465 da0f 7374 6172 7469  lf..node..starti
-000002d0: 6e67 5f70 6172 656e 7372 1100 0000 a900  ng_parensr......
-000002e0: 7218 0000 00fa 4d2f 686f 6d65 2f73 6861  r.....M/home/sha
-000002f0: 692f 6675 6e5f 7769 7468 5f61 7374 2f66  i/fun_with_ast/f
-00000300: 756e 5f77 6974 685f 6173 742f 736f 7572  un_with_ast/sour
-00000310: 6365 5f6d 6174 6368 6572 732f 636f 6e73  ce_matchers/cons
-00000320: 7461 6e74 5f73 6f75 7263 655f 6d61 7463  tant_source_matc
-00000330: 682e 7079 720a 0000 000c 0000 0073 2000  h.pyr........s .
-00000340: 0000 0c01 0c01 0401 0402 0601 0801 08fe  ................
-00000350: 0405 0601 0801 08fe 0604 0e01 0801 0602  ................
-00000360: 1401 7a1e 436f 6e73 7461 6e74 536f 7572  ..z.ConstantSour
-00000370: 6365 4d61 7463 6865 722e 5f5f 696e 6974  ceMatcher.__init
-00000380: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-00000390: 0000 0003 0000 0043 0000 0073 7200 0000  .......C...sr...
-000003a0: 7400 7c00 6a01 6a02 7403 8302 720d 7c00  t.|.j.j.t...r.|.
-000003b0: 6a04 a005 7c01 a101 5300 7400 7c00 6a01  j...|...S.t.|.j.
-000003c0: 6a02 7406 8302 7221 7400 7c00 6a01 6a07  j.t...r!t.|.j.j.
-000003d0: 7406 8302 7221 7c00 6a08 a005 7c01 a101  t...r!|.j...|...
-000003e0: 5300 7400 7c00 6a01 6a02 7409 8302 7235  S.t.|.j.j.t...r5
-000003f0: 7400 7c00 6a01 6a07 7409 8302 7237 7c00  t.|.j.j.t...r7|.
-00000400: 6a0a a005 7c01 a101 5300 6400 5300 6400  j...|...S.d.S.d.
-00000410: 5300 a901 4e29 0b72 0b00 0000 7216 0000  S...N).r....r...
-00000420: 00da 016e da04 626f 6f6c 7210 0000 00da  ...n..boolr.....
-00000430: 065f 6d61 7463 68da 0369 6e74 da01 7372  ._match..int..sr
-00000440: 0f00 0000 da03 7374 7272 1400 0000 2902  ......strr....).
-00000450: 7215 0000 00da 0673 7472 696e 6772 1800  r......stringr..
-00000460: 0000 7218 0000 0072 1900 0000 721d 0000  ..r....r....r...
-00000470: 0022 0000 0073 0e00 0000 0e01 0c01 1c01  ."...s..........
-00000480: 0c01 1c01 0c01 08ff 7a1c 436f 6e73 7461  ........z.Consta
-00000490: 6e74 536f 7572 6365 4d61 7463 6865 722e  ntSourceMatcher.
-000004a0: 5f6d 6174 6368 6301 0000 0000 0000 0000  _matchc.........
-000004b0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000004c0: 8a00 0000 7c00 a000 a100 0100 7c00 6a01  ....|.......|.j.
-000004d0: 720a 7c00 6a02 5300 7403 7c00 6a04 6a05  r.|.j.S.t.|.j.j.
-000004e0: 7406 8302 721d 7403 7c00 6a04 6a07 7408  t...r.t.|.j.j.t.
-000004f0: 8302 721d 7c00 6a09 a00a a100 5300 7403  ..r.|.j.....S.t.
-00000500: 7c00 6a04 6a05 7408 8302 7230 7403 7c00  |.j.j.t...r0t.|.
-00000510: 6a04 6a07 7408 8302 7230 7c00 6a0b a00a  j.j.t...r0|.j...
-00000520: a100 5300 7403 7c00 6a04 6a05 740c 8302  ..S.t.|.j.j.t...
-00000530: 7243 7403 7c00 6a04 6a07 740c 8302 7243  rCt.|.j.j.t...rC
-00000540: 7c00 6a0d a00a a100 5300 740e 8201 721a  |.j.....S.t...r.
-00000550: 0000 0029 0fda 1776 616c 6964 6174 6564  ...)...validated
-00000560: 5f63 616c 6c5f 746f 5f6d 6174 6368 da07  _call_to_match..
-00000570: 6d61 7463 6865 64da 0c6d 6174 6368 6564  matched..matched
-00000580: 5f74 6578 7472 0b00 0000 7216 0000 0072  _textr....r....r
-00000590: 1b00 0000 721c 0000 0072 1f00 0000 721e  ....r....r....r.
-000005a0: 0000 0072 1000 0000 da09 4765 7453 6f75  ...r......GetSou
-000005b0: 7263 6572 0f00 0000 7220 0000 0072 1400  rcer....r ...r..
-000005c0: 0000 da13 4e6f 7449 6d70 6c65 6d65 6e74  ....NotImplement
-000005d0: 6564 4572 726f 7229 0172 1500 0000 7218  edError).r....r.
-000005e0: 0000 0072 1800 0000 7219 0000 0072 2500  ...r....r....r%.
-000005f0: 0000 2a00 0000 7314 0000 0008 0106 0106  ..*...s.........
-00000600: 011c 010a 011c 010a 011c 010a 0104 027a  ...............z
-00000610: 1f43 6f6e 7374 616e 7453 6f75 7263 654d  .ConstantSourceM
-00000620: 6174 6368 6572 2e47 6574 536f 7572 6365  atcher.GetSource
-00000630: 2902 4e4e 2906 da08 5f5f 6e61 6d65 5f5f  ).NN)...__name__
-00000640: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000650: 7175 616c 6e61 6d65 5f5f 720a 0000 0072  qualname__r....r
-00000660: 1d00 0000 7225 0000 0072 1800 0000 7218  ....r%...r....r.
-00000670: 0000 0072 1800 0000 7219 0000 0072 0700  ...r....r....r..
-00000680: 0000 0b00 0000 7308 0000 0008 000a 0108  ......s.........
-00000690: 160c 0872 0700 0000 290c 720c 0000 00da  ...r....).r.....
-000006a0: 2366 756e 5f77 6974 685f 6173 742e 706c  #fun_with_ast.pl
-000006b0: 6163 6568 6f6c 6465 7273 2e63 6f6d 706f  aceholders.compo
-000006c0: 7369 7465 7202 0000 00da 1e66 756e 5f77  siter......fun_w
-000006d0: 6974 685f 6173 742e 706c 6163 6568 6f6c  ith_ast.placehol
-000006e0: 6465 7273 2e74 6578 7472 0300 0000 da29  ders.textr.....)
-000006f0: 6675 6e5f 7769 7468 5f61 7374 2e73 6f75  fun_with_ast.sou
-00000700: 7263 655f 6d61 7463 6865 7273 2e62 6173  rce_matchers.bas
-00000710: 655f 6d61 7463 6865 7272 0400 0000 da2c  e_matcherr.....,
-00000720: 6675 6e5f 7769 7468 5f61 7374 2e73 6f75  fun_with_ast.sou
-00000730: 7263 655f 6d61 7463 6865 7273 2e64 6566  rce_matchers.def
-00000740: 7561 6c74 5f6d 6174 6368 6572 7205 0000  ualt_matcherr...
-00000750: 00da 2066 756e 5f77 6974 685f 6173 742e  .. fun_with_ast.
-00000760: 736f 7572 6365 5f6d 6174 6368 6572 732e  source_matchers.
-00000770: 7374 7272 0600 0000 7207 0000 0072 1800  strr....r....r..
-00000780: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000790: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000007a0: 0e00 0000 0800 0c02 0c01 0c01 0c01 0c02  ................
-000007b0: 1403                                     ..
+000001e0: 7402 7c01 6a0e 740f 8302 7249 7410 7c01  t.|.j.t...rIt.|.
+000001f0: 7c02 7c00 6a0d 8303 7c00 5f11 6400 5300  |.|.j...|._.d.S.
+00000200: 6400 7c00 5f11 6400 5300 2906 4eda 0576  d.|._.d.S.).N..v
+00000210: 616c 7565 7a10 5b20 5c74 5d2a 2823 2b2e  aluez.[ \t]*(#+.
+00000220: 2a29 2a5c 6e3f da00 4654 2912 7204 0000  *)*\n?..FT).r...
+00000230: 00da 085f 5f69 6e69 745f 5fda 0a69 7369  ...__init__..isi
+00000240: 6e73 7461 6e63 65da 0361 7374 da08 436f  nstance..ast..Co
+00000250: 6e73 7461 6e74 da0a 5661 6c75 6545 7272  nstant..ValueErr
+00000260: 6f72 7205 0000 0072 0200 0000 7203 0000  orr....r....r...
+00000270: 00da 0b6e 756d 5f6d 6174 6368 6572 da0c  ...num_matcher..
+00000280: 626f 6f6c 5f6d 6174 6368 6572 da0b 7061  bool_matcher..pa
+00000290: 7265 6e74 5f6e 6f64 65da 094a 6f69 6e65  rent_node..Joine
+000002a0: 6453 7472 da18 6163 6365 7074 5f6d 756c  dStr..accept_mul
+000002b0: 7469 7061 7274 735f 7374 7269 6e67 da01  tiparts_string..
+000002c0: 73da 0373 7472 7206 0000 00da 0b73 7472  s..strr......str
+000002d0: 5f6d 6174 6368 6572 2904 da04 7365 6c66  _matcher)...self
+000002e0: da04 6e6f 6465 da0f 7374 6172 7469 6e67  ..node..starting
+000002f0: 5f70 6172 656e 7372 1100 0000 a900 721a  _parensr......r.
+00000300: 0000 00fa 4d2f 686f 6d65 2f73 6861 692f  ....M/home/shai/
+00000310: 6675 6e5f 7769 7468 5f61 7374 2f66 756e  fun_with_ast/fun
+00000320: 5f77 6974 685f 6173 742f 736f 7572 6365  _with_ast/source
+00000330: 5f6d 6174 6368 6572 732f 636f 6e73 7461  _matchers/consta
+00000340: 6e74 5f73 6f75 7263 655f 6d61 7463 682e  nt_source_match.
+00000350: 7079 720a 0000 000b 0000 0073 2400 0000  pyr........s$...
+00000360: 0c01 0c01 0401 0401 0601 0801 08fe 0404  ................
+00000370: 0601 0801 08fe 0603 0e01 0801 0602 0c01  ................
+00000380: 1401 0a02 7a1e 436f 6e73 7461 6e74 536f  ....z.ConstantSo
+00000390: 7572 6365 4d61 7463 6865 722e 5f5f 696e  urceMatcher.__in
+000003a0: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
+000003b0: 0002 0000 0003 0000 0043 0000 0073 7200  .........C...sr.
+000003c0: 0000 7400 7c00 6a01 6a02 7403 8302 720d  ..t.|.j.j.t...r.
+000003d0: 7c00 6a04 a005 7c01 a101 5300 7400 7c00  |.j...|...S.t.|.
+000003e0: 6a01 6a02 7406 8302 7221 7400 7c00 6a01  j.j.t...r!t.|.j.
+000003f0: 6a07 7406 8302 7221 7c00 6a08 a005 7c01  j.t...r!|.j...|.
+00000400: a101 5300 7400 7c00 6a01 6a02 7409 8302  ..S.t.|.j.j.t...
+00000410: 7235 7400 7c00 6a01 6a07 7409 8302 7237  r5t.|.j.j.t...r7
+00000420: 7c00 6a0a a005 7c01 a101 5300 6400 5300  |.j...|...S.d.S.
+00000430: 6400 5300 a901 4e29 0b72 0b00 0000 7218  d.S...N).r....r.
+00000440: 0000 00da 016e da04 626f 6f6c 7210 0000  .....n..boolr...
+00000450: 00da 065f 6d61 7463 68da 0369 6e74 7214  ..._match..intr.
+00000460: 0000 0072 0f00 0000 7215 0000 0072 1600  ...r....r....r..
+00000470: 0000 2902 7217 0000 00da 0673 7472 696e  ..).r......strin
+00000480: 6772 1a00 0000 721a 0000 0072 1b00 0000  gr....r....r....
+00000490: 721f 0000 0020 0000 0073 0e00 0000 0e01  r.... ...s......
+000004a0: 0c01 1c01 0c01 1c01 0c01 08ff 7a1c 436f  ............z.Co
+000004b0: 6e73 7461 6e74 536f 7572 6365 4d61 7463  nstantSourceMatc
+000004c0: 6865 722e 5f6d 6174 6368 6301 0000 0000  her._matchc.....
+000004d0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+000004e0: 0000 0073 8a00 0000 7c00 a000 a100 0100  ...s....|.......
+000004f0: 7c00 6a01 720a 7c00 6a02 5300 7403 7c00  |.j.r.|.j.S.t.|.
+00000500: 6a04 6a05 7406 8302 721d 7403 7c00 6a04  j.j.t...r.t.|.j.
+00000510: 6a07 7408 8302 721d 7c00 6a09 a00a a100  j.t...r.|.j.....
+00000520: 5300 7403 7c00 6a04 6a05 7408 8302 7230  S.t.|.j.j.t...r0
+00000530: 7403 7c00 6a04 6a07 7408 8302 7230 7c00  t.|.j.j.t...r0|.
+00000540: 6a0b a00a a100 5300 7403 7c00 6a04 6a05  j.....S.t.|.j.j.
+00000550: 740c 8302 7243 7403 7c00 6a04 6a07 740c  t...rCt.|.j.j.t.
+00000560: 8302 7243 7c00 6a0d a00a a100 5300 740e  ..rC|.j.....S.t.
+00000570: 8201 721c 0000 0029 0fda 1776 616c 6964  ..r....)...valid
+00000580: 6174 6564 5f63 616c 6c5f 746f 5f6d 6174  ated_call_to_mat
+00000590: 6368 da07 6d61 7463 6865 64da 0c6d 6174  ch..matched..mat
+000005a0: 6368 6564 5f74 6578 7472 0b00 0000 7218  ched_textr....r.
+000005b0: 0000 0072 1d00 0000 721e 0000 0072 1400  ...r....r....r..
+000005c0: 0000 7220 0000 0072 1000 0000 da09 4765  ..r ...r......Ge
+000005d0: 7453 6f75 7263 6572 0f00 0000 7215 0000  tSourcer....r...
+000005e0: 0072 1600 0000 da13 4e6f 7449 6d70 6c65  .r......NotImple
+000005f0: 6d65 6e74 6564 4572 726f 7229 0172 1700  mentedError).r..
+00000600: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000610: 0072 2500 0000 2800 0000 7314 0000 0008  .r%...(...s.....
+00000620: 0106 0106 011c 010a 011c 010a 011c 010a  ................
+00000630: 0104 027a 1f43 6f6e 7374 616e 7453 6f75  ...z.ConstantSou
+00000640: 7263 654d 6174 6368 6572 2e47 6574 536f  rceMatcher.GetSo
+00000650: 7572 6365 2902 4e4e 2906 da08 5f5f 6e61  urce).NN)...__na
+00000660: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000670: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720a  ..__qualname__r.
+00000680: 0000 0072 1f00 0000 7225 0000 0072 1a00  ...r....r%...r..
+00000690: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+000006a0: 0072 0700 0000 0a00 0000 7308 0000 0008  .r........s.....
+000006b0: 000a 0108 150c 0872 0700 0000 290c 720c  .......r....).r.
+000006c0: 0000 00da 2366 756e 5f77 6974 685f 6173  ....#fun_with_as
+000006d0: 742e 706c 6163 6568 6f6c 6465 7273 2e63  t.placeholders.c
+000006e0: 6f6d 706f 7369 7465 7202 0000 00da 1e66  ompositer......f
+000006f0: 756e 5f77 6974 685f 6173 742e 706c 6163  un_with_ast.plac
+00000700: 6568 6f6c 6465 7273 2e74 6578 7472 0300  eholders.textr..
+00000710: 0000 da29 6675 6e5f 7769 7468 5f61 7374  ...)fun_with_ast
+00000720: 2e73 6f75 7263 655f 6d61 7463 6865 7273  .source_matchers
+00000730: 2e62 6173 655f 6d61 7463 6865 7272 0400  .base_matcherr..
+00000740: 0000 da2c 6675 6e5f 7769 7468 5f61 7374  ...,fun_with_ast
+00000750: 2e73 6f75 7263 655f 6d61 7463 6865 7273  .source_matchers
+00000760: 2e64 6566 7561 6c74 5f6d 6174 6368 6572  .defualt_matcher
+00000770: 7205 0000 00da 2066 756e 5f77 6974 685f  r..... fun_with_
+00000780: 6173 742e 736f 7572 6365 5f6d 6174 6368  ast.source_match
+00000790: 6572 732e 7374 7272 0600 0000 7207 0000  ers.strr....r...
+000007a0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+000007b0: 721b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000007c0: 0000 0073 0e00 0000 0800 0c02 0c01 0c01  ...s............
+000007d0: 0c01 0c01 1403                           ......
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/defualt_matcher.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/defualt_matcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul  1 11:49:49 2023 UTC, .py size: 8636 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,242 +1,236 @@
-00000000: 6f0d 0d0a 0000 0000 dd12 a064 bc21 0000  o..........d.!..
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 2011 0000  o..........d ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
-00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
-00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 4700  m.Z.m.Z.m.Z...G.
-00000080: 6406 6407 8400 6407 6507 8303 5a0f 6401  d.d...d.e...Z.d.
-00000090: 5300 2908 e900 0000 004e 2901 da0b 506c  S.)......N)...Pl
-000000a0: 6163 6568 6f6c 6465 7229 02da 1b42 6164  aceholder)...Bad
-000000b0: 6c79 5370 6563 6966 6965 6454 656d 706c  lySpecifiedTempl
-000000c0: 6174 6545 7272 6f72 da13 456d 7074 7953  ateError..EmptyS
-000000d0: 7461 636b 4578 6365 7074 696f 6e29 04da  tackException)..
-000000e0: 0d53 6f75 7263 654d 6174 6368 6572 da14  .SourceMatcher..
-000000f0: 4d61 7463 6850 6c61 6365 686f 6c64 6572  MatchPlaceholder
-00000100: 4c69 7374 da10 4d61 7463 6850 6c61 6365  List..MatchPlace
-00000110: 686f 6c64 6572 da0b 6675 6c6c 5f73 7472  holder..full_str
-00000120: 696e 6729 03da 0f54 6578 7450 6c61 6365  ing)...TextPlace
-00000130: 686f 6c64 6572 da0f 456e 6450 6172 656e  holder..EndParen
-00000140: 4d61 7463 6865 72da 1153 7461 7274 5061  Matcher..StartPa
-00000150: 7265 6e4d 6174 6368 6572 6300 0000 0000  renMatcherc.....
-00000160: 0000 0000 0000 0000 0000 0004 0000 0000  ................
-00000170: 0000 0073 4600 0000 6500 5a01 6400 5a02  ...sF...e.Z.d.Z.
-00000180: 6401 5a03 640d 8700 6601 6403 6404 8409  d.Z.d...f.d.d...
-00000190: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
-000001a0: 5a06 8700 6601 6409 640a 8408 5a07 640b  Z...f.d.d...Z.d.
-000001b0: 640c 8400 5a08 8700 0400 5a09 5300 290e  d...Z.....Z.S.).
-000001c0: da14 4465 6661 756c 7453 6f75 7263 654d  ..DefaultSourceM
-000001d0: 6174 6368 6572 7a28 436c 6173 7320 746f  atcherz(Class to
-000001e0: 2067 656e 6572 6174 6520 7468 6520 736f   generate the so
-000001f0: 7572 6365 2066 6f72 2061 206e 6f64 652e  urce for a node.
-00000200: 4e63 0500 0000 0000 0000 0000 0000 0700  Nc..............
-00000210: 0000 0400 0000 0300 0000 7354 0000 0074  ..........sT...t
-00000220: 0074 017c 0083 02a0 027c 017c 03a1 0201  .t.|.....|.|....
-00000230: 0064 017d 057c 0244 005d 177d 0674 037c  .d.}.|.D.].}.t.|
-00000240: 0674 0483 0273 1874 0564 0283 0182 0174  .t...s.t.d.....t
-00000250: 037c 0674 0683 0272 227c 0573 2264 037d  .|.t...r"|.s"d.}
-00000260: 0571 0d64 017d 0571 0d7c 027c 005f 0764  .q.d.}.q.|.|._.d
-00000270: 0053 0029 044e 467a 2e41 6c6c 2065 7870  .S.).NFz.All exp
-00000280: 6563 7465 6420 7061 7274 7320 6d75 7374  ected parts must
-00000290: 2062 6520 506c 6163 6568 6f6c 6465 7220   be Placeholder 
-000002a0: 6f62 6a65 6374 7354 2908 da05 7375 7065  objectsT)...supe
-000002b0: 7272 0c00 0000 da08 5f5f 696e 6974 5f5f  rr......__init__
-000002c0: da0a 6973 696e 7374 616e 6365 7202 0000  ..isinstancer...
-000002d0: 00da 0a56 616c 7565 4572 726f 7272 0900  ...ValueErrorr..
-000002e0: 0000 da0e 6578 7065 6374 6564 5f70 6172  ....expected_par
-000002f0: 7473 2907 da04 7365 6c66 da04 6e6f 6465  ts)...self..node
-00000300: 7211 0000 00da 0f73 7461 7274 696e 675f  r......starting_
-00000310: 7061 7265 6e73 da0b 7061 7265 6e74 5f6e  parens..parent_n
-00000320: 6f64 65da 1370 7265 7669 6f75 735f 7761  ode..previous_wa
-00000330: 735f 7374 7269 6e67 da04 7061 7274 a901  s_string..part..
-00000340: da09 5f5f 636c 6173 735f 5fa9 00fa 472f  ..__class__...G/
-00000350: 686f 6d65 2f73 6861 692f 6675 6e5f 7769  home/shai/fun_wi
-00000360: 7468 5f61 7374 2f66 756e 5f77 6974 685f  th_ast/fun_with_
-00000370: 6173 742f 736f 7572 6365 5f6d 6174 6368  ast/source_match
-00000380: 6572 732f 6465 6675 616c 745f 6d61 7463  ers/defualt_matc
-00000390: 6865 722e 7079 720e 0000 000c 0000 0073  her.pyr........s
-000003a0: 1200 0000 1201 0401 0803 0a01 0801 0e01  ................
-000003b0: 0601 0604 0a01 7a1d 4465 6661 756c 7453  ......z.DefaultS
-000003c0: 6f75 7263 654d 6174 6368 6572 2e5f 5f69  ourceMatcher.__i
-000003d0: 6e69 745f 5f63 0200 0000 0000 0000 0000  nit__c..........
-000003e0: 0000 0700 0000 0a00 0000 4300 0000 73a4  ..........C...s.
-000003f0: 0000 007c 00a0 007c 01a1 017d 027c 00a0  ...|...|...}.|..
-00000400: 017c 02a1 017d 027a 1174 027c 027c 006a  .|...}.z.t.|.|.j
-00000410: 037c 006a 047c 006a 0583 047d 027c 00a0  .|.j.|.j...}.|..
-00000420: 067c 02a1 017d 0257 006e 1604 0074 0779  .|...}.W.n...t.y
-00000430: 3101 007d 0301 007a 0a74 0764 01a0 087c  1..}...z.t.d...|
-00000440: 017c 007c 036a 09a1 0383 0182 0164 027d  .|.|.j.......d.}
-00000450: 037e 0377 0177 0074 0aa0 0b7c 00a1 017d  .~.w.w.t...|...}
-00000460: 047c 00a0 0c7c 02a1 017c 005f 0d7c 00a0  .|...|...|._.|..
-00000470: 0e7c 006a 0fa1 017d 057c 047c 0517 007c  .|.j...}.|.|...|
-00000480: 006a 0d17 007d 0664 037c 005f 107c 067c  .j...}.d.|._.|.|
-00000490: 005f 117c 0653 0029 0461 1603 0000 4d61  ._.|.S.).a....Ma
-000004a0: 7463 6865 7320 7468 6520 7374 7269 6e67  tches the string
-000004b0: 2061 6761 696e 7374 2073 656c 662e 6578   against self.ex
-000004c0: 7065 6374 6564 5f70 6172 7473 2e0a 0a20  pected_parts... 
-000004d0: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-000004e0: 2074 6869 7320 6973 2073 6c69 6768 746c   this is slightl
-000004f0: 7920 7065 6375 6c69 6172 2069 6e20 7468  y peculiar in th
-00000500: 6174 2069 7420 6669 7273 7420 6d61 7463  at it first matc
-00000510: 6865 7320 6669 656c 6473 2c0a 2020 2020  hes fields,.    
-00000520: 2020 2020 7468 656e 2067 6f65 7320 6261      then goes ba
-00000530: 636b 2074 6f20 6d61 7463 6820 7465 7874  ck to match text
-00000540: 2062 6566 6f72 6520 7468 656d 2e20 5468   before them. Th
-00000550: 6973 2069 7320 6265 6361 7573 6520 6375  is is because cu
-00000560: 7272 656e 746c 7920 7765 0a20 2020 2020  rrently we.     
-00000570: 2020 2064 6f6e 2774 2068 6176 6520 6d61     don't have ma
-00000580: 7463 6865 7273 2066 6f72 2065 7665 7279  tchers for every
-00000590: 206e 6f64 652c 2073 6f20 6279 2064 6566   node, so by def
-000005a0: 6175 6c74 2c20 7765 2073 6570 6172 6174  ault, we separat
-000005b0: 6520 6561 6368 0a20 2020 2020 2020 2066  e each.        f
-000005c0: 6965 6c64 2077 6974 6820 6120 272e 2a27  ield with a '.*'
-000005d0: 2054 6578 7453 6570 6172 6174 6f72 2c20   TextSeparator, 
-000005e0: 7768 6963 6820 6973 2062 6173 6963 616c  which is basical
-000005f0: 6c79 2074 6865 2063 7572 7265 6e74 2062  ly the current b
-00000600: 6568 6176 696f 720a 2020 2020 2020 2020  ehavior.        
-00000610: 6f66 2061 7374 5f61 6e6e 6f74 6174 652e  of ast_annotate.
-00000620: 2054 6869 7320 6361 6e20 6368 616e 6765   This can change
-00000630: 2061 6674 6572 2077 6520 6e6f 206c 6f6e   after we no lon
-00000640: 6765 7220 6861 7665 2061 6e79 206e 6565  ger have any nee
-00000650: 6420 666f 720a 2020 2020 2020 2020 272e  d for.        '.
-00000660: 2a27 2054 6578 7453 6570 6172 6174 6f72  *' TextSeparator
-00000670: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
-00000680: 3a0a 2020 2020 2020 2020 2020 7374 7269  :.          stri
-00000690: 6e67 3a20 7b73 7472 7d20 5468 6520 7374  ng: {str} The st
-000006a0: 7269 6e67 2074 6f20 6d61 7463 682e 0a0a  ring to match...
-000006b0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-000006c0: 0a20 2020 2020 2020 2020 2054 6865 206d  .          The m
-000006d0: 6174 6368 6564 2074 6578 742e 0a0a 2020  atched text...  
-000006e0: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-000006f0: 2020 2020 2020 2020 4261 646c 7953 7065          BadlySpe
-00000700: 6369 6669 6564 5465 6d70 6c61 7465 4572  cifiedTemplateEr
-00000710: 726f 723a 2049 6620 7468 6572 6520 6973  ror: If there is
-00000720: 2061 206d 6973 6d61 7463 6820 6265 7477   a mismatch betw
-00000730: 6565 6e20 7468 650a 2020 2020 2020 2020  een the.        
-00000740: 2020 2020 6578 7065 6374 6564 5f70 6172      expected_par
-00000750: 7473 2061 6e64 2074 6865 2073 7472 696e  ts and the strin
-00000760: 672e 0a20 2020 2020 2020 2020 2056 616c  g..          Val
-00000770: 7565 4572 726f 723a 2049 6620 7468 6572  ueError: If ther
-00000780: 6520 6973 206d 6f72 6520 7468 616e 206f  e is more than o
-00000790: 6e65 2054 6578 7450 6c61 6365 686f 6c64  ne TextPlacehold
-000007a0: 6572 2069 6e20 6120 7277 6f0a 2020 2020  er in a rwo.    
-000007b0: 2020 2020 7a46 5768 656e 2061 7474 656d      zFWhen attem
-000007c0: 7074 696e 6720 746f 206d 6174 6368 2073  pting to match s
-000007d0: 7472 696e 6720 227b 7d22 2077 6974 6820  tring "{}" with 
-000007e0: 7b7d 2c20 7468 6973 2065 7272 6f72 2072  {}, this error r
-000007f0: 6573 756c 7465 643a 0a0a 7b7d 4e54 2912  esulted:..{}NT).
-00000800: da10 4d61 7463 6857 6869 7465 5370 6163  ..MatchWhiteSpac
-00000810: 6573 da10 4d61 7463 6853 7461 7274 5061  es..MatchStartPa
-00000820: 7265 6e73 7206 0000 0072 1300 0000 7211  rensr....r....r.
-00000830: 0000 00da 1473 7461 7274 5f70 6172 656e  .....start_paren
-00000840: 5f6d 6174 6368 6572 73da 0d4d 6174 6368  _matchers..Match
-00000850: 456e 6450 6172 656e 7203 0000 00da 0666  EndParenr......f
-00000860: 6f72 6d61 74da 076d 6573 7361 6765 720c  ormat..messager.
-00000870: 0000 00da 0947 6574 536f 7572 6365 da0f  .....GetSource..
-00000880: 4d61 7463 6843 6f6d 6d65 6e74 454f 4cda  MatchCommentEOL.
-00000890: 1365 6e64 5f6f 665f 6c69 6e65 5f63 6f6d  .end_of_line_com
-000008a0: 6d65 6e74 da11 4765 7457 6869 7465 5370  ment..GetWhiteSp
-000008b0: 6163 6554 6578 74da 1765 6e64 5f77 6869  aceText..end_whi
-000008c0: 7465 7370 6163 655f 6d61 7463 6865 7273  tespace_matchers
-000008d0: da07 6d61 7463 6865 64da 0e6d 6174 6368  ..matched..match
-000008e0: 6564 5f73 6f75 7263 6529 0772 1200 0000  ed_source).r....
-000008f0: da06 7374 7269 6e67 da10 7265 6d61 696e  ..string..remain
-00000900: 696e 675f 7374 7269 6e67 da01 65da 0e6d  ing_string..e..m
-00000910: 6174 6368 6564 5f73 7472 696e 67da 0665  atched_string..e
-00000920: 6e64 5f77 73da 0672 6573 756c 7472 1a00  nd_ws..resultr..
-00000930: 0000 721a 0000 0072 1b00 0000 da06 5f6d  ..r....r......_m
-00000940: 6174 6368 1d00 0000 732c 0000 000a 150a  atch....s,......
-00000950: 0102 0302 010a 0104 0104 fe0e 030e 0202  ................
-00000960: 0102 010c 0204 fd08 8002 ff0a 060c 060c  ................
-00000970: 010e 0306 0106 0104 017a 1b44 6566 6175  .........z.Defau
-00000980: 6c74 536f 7572 6365 4d61 7463 6865 722e  ltSourceMatcher.
-00000990: 5f6d 6174 6368 6301 0000 0000 0000 0000  _matchc.........
-000009a0: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
-000009b0: a600 0000 7c00 a000 a100 0100 7c00 6a01  ....|.......|.j.
-000009c0: 720a 7c00 6a02 5300 6700 7d01 7c00 6a03  r.|.j.S.g.}.|.j.
-000009d0: 4400 5d0d 7d02 7c02 a004 7c00 6a05 a101  D.].}.|...|.j...
-000009e0: 7d03 7c01 a006 7c03 a101 0100 710f 6401  }.|...|.....q.d.
-000009f0: a007 7c01 a101 7d04 6402 a008 7c00 a009  ..|...}.d...|...
-00000a00: a100 7c04 7c00 a00a a100 a103 7d04 7c00  ..|.|.......}.|.
-00000a10: 6a0b 723a 6403 a008 7c00 a00c 7c00 6a0b  j.r:d...|...|.j.
-00000a20: a101 7c04 a102 7d04 7c00 6a0d 7247 6403  ..|...}.|.j.rGd.
-00000a30: a008 7c04 7c00 a00c 7c00 6a0d a101 a102  ..|.|...|.j.....
-00000a40: 7d04 7c00 6a0e 7251 6403 a008 7c04 7c00  }.|.j.rQd...|.|.
-00000a50: 6a0e a102 7d04 7c04 5300 2904 4eda 007a  j...}.|.S.).N..z
-00000a60: 067b 7d7b 7d7b 7d7a 047b 7d7b 7d29 0fda  .{}{}{}z.{}{})..
-00000a70: 1776 616c 6964 6174 6564 5f63 616c 6c5f  .validated_call_
-00000a80: 746f 5f6d 6174 6368 7227 0000 0072 2800  to_matchr'...r(.
-00000a90: 0000 7211 0000 0072 2200 0000 7213 0000  ..r....r"...r...
-00000aa0: 00da 0661 7070 656e 64da 046a 6f69 6e72  ...append..joinr
-00000ab0: 2000 0000 da11 4765 7453 7461 7274 5061   .....GetStartPa
-00000ac0: 7265 6e54 6578 74da 0f47 6574 456e 6450  renText..GetEndP
-00000ad0: 6172 656e 5465 7874 da19 7374 6172 745f  arenText..start_
-00000ae0: 7768 6974 6573 7061 6365 5f6d 6174 6368  whitespace_match
-00000af0: 6572 7372 2500 0000 7226 0000 0072 2400  ersr%...r&...r$.
-00000b00: 0000 2905 7212 0000 00da 0b73 6f75 7263  ..).r......sourc
-00000b10: 655f 6c69 7374 7217 0000 00da 0b70 6172  e_listr......par
-00000b20: 745f 736f 7572 6365 da06 736f 7572 6365  t_source..source
-00000b30: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000b40: 2200 0000 5200 0000 7328 0000 0008 0106  "...R...s(......
-00000b50: 0106 0104 010a 010c 010c 010a 0104 0106  ................
-00000b60: 0102 0106 0104 fd06 0514 0106 0114 0106  ................
-00000b70: 010e 0104 017a 1e44 6566 6175 6c74 536f  .....z.DefaultSo
-00000b80: 7572 6365 4d61 7463 6865 722e 4765 7453  urceMatcher.GetS
-00000b90: 6f75 7263 6563 0100 0000 0000 0000 0000  ourcec..........
-00000ba0: 0000 0100 0000 0700 0000 0300 0000 7322  ..............s"
-00000bb0: 0000 0064 01a0 0074 0174 027c 0083 02a0  ...d...t.t.|....
-00000bc0: 03a1 007c 006a 0474 05a0 067c 006a 07a1  ...|.j.t...|.j..
-00000bd0: 01a1 0353 0029 024e 7a3f 4465 6661 756c  ...S.).Nz?Defaul
-00000be0: 7453 6f75 7263 654d 6174 6368 6572 2022  tSourceMatcher "
-00000bf0: 7b7d 2220 666f 7220 6e6f 6465 2022 7b7d  {}" for node "{}
-00000c00: 2220 6578 7065 6374 696e 6720 746f 206d  " expecting to m
-00000c10: 6174 6368 2022 7b7d 2229 0872 2000 0000  atch "{}").r ...
-00000c20: 720d 0000 0072 0c00 0000 da08 5f5f 7265  r....r......__re
-00000c30: 7072 5f5f 7213 0000 00da 0670 7072 696e  pr__r......pprin
-00000c40: 74da 0770 666f 726d 6174 7211 0000 0029  t..pformatr....)
-00000c50: 0172 1200 0000 7218 0000 0072 1a00 0000  .r....r....r....
-00000c60: 721b 0000 0072 3a00 0000 8500 0000 730c  r....r:.......s.
-00000c70: 0000 0002 010e 0104 010a 0102 fe02 ff7a  ...............z
-00000c80: 1d44 6566 6175 6c74 536f 7572 6365 4d61  .DefaultSourceMa
-00000c90: 7463 6865 722e 5f5f 7265 7072 5f5f 6302  tcher.__repr__c.
-00000ca0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00000cb0: 0000 0043 0000 0073 2a00 0000 7c00 6a00  ...C...s*...|.j.
-00000cc0: 6401 1900 7d02 7c02 a001 6400 7c01 a102  d...}.|...d.|...
-00000cd0: 7d03 7c01 7402 7c03 8301 6400 8502 1900  }.|.t.|...d.....
-00000ce0: 7d01 7c01 5300 2902 4e72 0100 0000 2903  }.|.S.).Nr....).
-00000cf0: 7236 0000 0072 2f00 0000 da03 6c65 6e29  r6...r/.....len)
-00000d00: 0472 1200 0000 722a 0000 00da 0e77 735f  .r....r*.....ws_
-00000d10: 706c 6163 6568 6f6c 6465 72da 086d 6174  placeholder..mat
-00000d20: 6368 5f77 7372 1a00 0000 721a 0000 0072  ch_wsr....r....r
-00000d30: 1b00 0000 721c 0000 008b 0000 0073 0800  ....r........s..
-00000d40: 0000 0a01 0c01 1001 0402 7a25 4465 6661  ..........z%Defa
-00000d50: 756c 7453 6f75 7263 654d 6174 6368 6572  ultSourceMatcher
-00000d60: 2e4d 6174 6368 5768 6974 6553 7061 6365  .MatchWhiteSpace
-00000d70: 7329 024e 4e29 0ada 085f 5f6e 616d 655f  s).NN)...__name_
-00000d80: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000d90: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00000da0: 6f63 5f5f 720e 0000 0072 2f00 0000 7222  oc__r....r/...r"
-00000db0: 0000 0072 3a00 0000 721c 0000 00da 0d5f  ...r:...r......_
-00000dc0: 5f63 6c61 7373 6365 6c6c 5f5f 721a 0000  _classcell__r...
-00000dd0: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
-00000de0: 720c 0000 0009 0000 0073 0e00 0000 0800  r........s......
-00000df0: 0401 0e02 0811 0835 0c33 1006 720c 0000  .......5.3..r...
-00000e00: 0029 1072 3b00 0000 da2a 6675 6e5f 7769  .).r;....*fun_wi
-00000e10: 7468 5f61 7374 2e70 6c61 6365 686f 6c64  th_ast.placehold
-00000e20: 6572 732e 6261 7365 5f70 6c61 6365 686f  ers.base_placeho
-00000e30: 6c64 6572 7202 0000 00da 2766 756e 5f77  lderr.....'fun_w
-00000e40: 6974 685f 6173 742e 736f 7572 6365 5f6d  ith_ast.source_m
-00000e50: 6174 6368 6572 732e 6578 6365 7074 696f  atchers.exceptio
-00000e60: 6e73 7203 0000 0072 0400 0000 da29 6675  nsr....r.....)fu
-00000e70: 6e5f 7769 7468 5f61 7374 2e73 6f75 7263  n_with_ast.sourc
-00000e80: 655f 6d61 7463 6865 7273 2e62 6173 655f  e_matchers.base_
-00000e90: 6d61 7463 6865 7272 0500 0000 7206 0000  matcherr....r...
-00000ea0: 0072 0700 0000 7208 0000 00da 1e66 756e  .r....r......fun
-00000eb0: 5f77 6974 685f 6173 742e 706c 6163 6568  _with_ast.placeh
-00000ec0: 6f6c 6465 7273 2e74 6578 7472 0900 0000  olders.textr....
-00000ed0: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000ee0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
-00000ef0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000f00: 0073 0c00 0000 0800 0c02 1001 1801 1401  .s..............
-00000f10: 1403                                     ..
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 4700 6407 6408 8400 6408 6508 8303  ..G.d.d...d.e...
+00000080: 5a0b 6401 5300 2909 e900 0000 004e 2901  Z.d.S.)......N).
+00000090: da14 4d61 7463 6850 6c61 6365 686f 6c64  ..MatchPlacehold
+000000a0: 6572 4c69 7374 2901 da0b 506c 6163 6568  erList)...Placeh
+000000b0: 6f6c 6465 7229 01da 0f54 6578 7450 6c61  older)...TextPla
+000000c0: 6365 686f 6c64 6572 2901 da0d 536f 7572  ceholder)...Sour
+000000d0: 6365 4d61 7463 6865 7229 01da 1b42 6164  ceMatcher)...Bad
+000000e0: 6c79 5370 6563 6966 6965 6454 656d 706c  lySpecifiedTempl
+000000f0: 6174 6545 7272 6f72 6300 0000 0000 0000  ateErrorc.......
+00000100: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00000110: 0073 4600 0000 6500 5a01 6400 5a02 6401  .sF...e.Z.d.Z.d.
+00000120: 5a03 640d 8700 6601 6403 6404 8409 5a04  Z.d...f.d.d...Z.
+00000130: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
+00000140: 8700 6601 6409 640a 8408 5a07 640b 640c  ..f.d.d...Z.d.d.
+00000150: 8400 5a08 8700 0400 5a09 5300 290e da14  ..Z.....Z.S.)...
+00000160: 4465 6661 756c 7453 6f75 7263 654d 6174  DefaultSourceMat
+00000170: 6368 6572 7a28 436c 6173 7320 746f 2067  cherz(Class to g
+00000180: 656e 6572 6174 6520 7468 6520 736f 7572  enerate the sour
+00000190: 6365 2066 6f72 2061 206e 6f64 652e 4e63  ce for a node.Nc
+000001a0: 0500 0000 0000 0000 0000 0000 0700 0000  ................
+000001b0: 0400 0000 0300 0000 7354 0000 0074 0074  ........sT...t.t
+000001c0: 017c 0083 02a0 027c 017c 03a1 0201 0064  .|.....|.|.....d
+000001d0: 017d 057c 0244 005d 177d 0674 037c 0674  .}.|.D.].}.t.|.t
+000001e0: 0483 0273 1874 0564 0283 0182 0174 037c  ...s.t.d.....t.|
+000001f0: 0674 0683 0272 227c 0573 2264 037d 0571  .t...r"|.s"d.}.q
+00000200: 0d64 017d 0571 0d7c 027c 005f 0764 0053  .d.}.q.|.|._.d.S
+00000210: 0029 044e 467a 2e41 6c6c 2065 7870 6563  .).NFz.All expec
+00000220: 7465 6420 7061 7274 7320 6d75 7374 2062  ted parts must b
+00000230: 6520 506c 6163 6568 6f6c 6465 7220 6f62  e Placeholder ob
+00000240: 6a65 6374 7354 2908 da05 7375 7065 7272  jectsT)...superr
+00000250: 0700 0000 da08 5f5f 696e 6974 5f5f da0a  ......__init__..
+00000260: 6973 696e 7374 616e 6365 7203 0000 00da  isinstancer.....
+00000270: 0a56 616c 7565 4572 726f 7272 0400 0000  .ValueErrorr....
+00000280: da0e 6578 7065 6374 6564 5f70 6172 7473  ..expected_parts
+00000290: 2907 da04 7365 6c66 da04 6e6f 6465 720c  )...self..noder.
+000002a0: 0000 00da 0f73 7461 7274 696e 675f 7061  .....starting_pa
+000002b0: 7265 6e73 da0b 7061 7265 6e74 5f6e 6f64  rens..parent_nod
+000002c0: 65da 1370 7265 7669 6f75 735f 7761 735f  e..previous_was_
+000002d0: 7374 7269 6e67 da04 7061 7274 a901 da09  string..part....
+000002e0: 5f5f 636c 6173 735f 5fa9 00fa 472f 686f  __class__...G/ho
+000002f0: 6d65 2f73 6861 692f 6675 6e5f 7769 7468  me/shai/fun_with
+00000300: 5f61 7374 2f66 756e 5f77 6974 685f 6173  _ast/fun_with_as
+00000310: 742f 736f 7572 6365 5f6d 6174 6368 6572  t/source_matcher
+00000320: 732f 6465 6675 616c 745f 6d61 7463 6865  s/defualt_matche
+00000330: 722e 7079 7209 0000 000d 0000 0073 1200  r.pyr........s..
+00000340: 0000 1201 0401 0803 0a01 0801 0e01 0601  ................
+00000350: 0602 0a01 7a1d 4465 6661 756c 7453 6f75  ....z.DefaultSou
+00000360: 7263 654d 6174 6368 6572 2e5f 5f69 6e69  rceMatcher.__ini
+00000370: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00000380: 0700 0000 0a00 0000 4300 0000 73a4 0000  ........C...s...
+00000390: 007c 00a0 007c 01a1 017d 027c 00a0 017c  .|...|...}.|...|
+000003a0: 02a1 017d 027a 1174 027c 027c 006a 037c  ...}.z.t.|.|.j.|
+000003b0: 006a 047c 006a 0583 047d 027c 00a0 067c  .j.|.j...}.|...|
+000003c0: 02a1 017d 0257 006e 1604 0074 0779 3101  ...}.W.n...t.y1.
+000003d0: 007d 0301 007a 0a74 0764 01a0 087c 017c  .}...z.t.d...|.|
+000003e0: 007c 036a 09a1 0383 0182 0164 027d 037e  .|.j.......d.}.~
+000003f0: 0377 0177 0074 0aa0 0b7c 00a1 017d 047c  .w.w.t...|...}.|
+00000400: 00a0 0c7c 02a1 017c 005f 0d7c 00a0 0e7c  ...|...|._.|...|
+00000410: 006a 0fa1 017d 057c 047c 0517 007c 006a  .j...}.|.|...|.j
+00000420: 0d17 007d 0664 037c 005f 107c 067c 005f  ...}.d.|._.|.|._
+00000430: 117c 0653 0029 0461 1603 0000 4d61 7463  .|.S.).a....Matc
+00000440: 6865 7320 7468 6520 7374 7269 6e67 2061  hes the string a
+00000450: 6761 696e 7374 2073 656c 662e 6578 7065  gainst self.expe
+00000460: 6374 6564 5f70 6172 7473 2e0a 0a20 2020  cted_parts...   
+00000470: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
+00000480: 6869 7320 6973 2073 6c69 6768 746c 7920  his is slightly 
+00000490: 7065 6375 6c69 6172 2069 6e20 7468 6174  peculiar in that
+000004a0: 2069 7420 6669 7273 7420 6d61 7463 6865   it first matche
+000004b0: 7320 6669 656c 6473 2c0a 2020 2020 2020  s fields,.      
+000004c0: 2020 7468 656e 2067 6f65 7320 6261 636b    then goes back
+000004d0: 2074 6f20 6d61 7463 6820 7465 7874 2062   to match text b
+000004e0: 6566 6f72 6520 7468 656d 2e20 5468 6973  efore them. This
+000004f0: 2069 7320 6265 6361 7573 6520 6375 7272   is because curr
+00000500: 656e 746c 7920 7765 0a20 2020 2020 2020  ently we.       
+00000510: 2064 6f6e 2774 2068 6176 6520 6d61 7463   don't have matc
+00000520: 6865 7273 2066 6f72 2065 7665 7279 206e  hers for every n
+00000530: 6f64 652c 2073 6f20 6279 2064 6566 6175  ode, so by defau
+00000540: 6c74 2c20 7765 2073 6570 6172 6174 6520  lt, we separate 
+00000550: 6561 6368 0a20 2020 2020 2020 2066 6965  each.        fie
+00000560: 6c64 2077 6974 6820 6120 272e 2a27 2054  ld with a '.*' T
+00000570: 6578 7453 6570 6172 6174 6f72 2c20 7768  extSeparator, wh
+00000580: 6963 6820 6973 2062 6173 6963 616c 6c79  ich is basically
+00000590: 2074 6865 2063 7572 7265 6e74 2062 6568   the current beh
+000005a0: 6176 696f 720a 2020 2020 2020 2020 6f66  avior.        of
+000005b0: 2061 7374 5f61 6e6e 6f74 6174 652e 2054   ast_annotate. T
+000005c0: 6869 7320 6361 6e20 6368 616e 6765 2061  his can change a
+000005d0: 6674 6572 2077 6520 6e6f 206c 6f6e 6765  fter we no longe
+000005e0: 7220 6861 7665 2061 6e79 206e 6565 6420  r have any need 
+000005f0: 666f 720a 2020 2020 2020 2020 272e 2a27  for.        '.*'
+00000600: 2054 6578 7453 6570 6172 6174 6f72 732e   TextSeparators.
+00000610: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00000620: 2020 2020 2020 2020 2020 7374 7269 6e67            string
+00000630: 3a20 7b73 7472 7d20 5468 6520 7374 7269  : {str} The stri
+00000640: 6e67 2074 6f20 6d61 7463 682e 0a0a 2020  ng to match...  
+00000650: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00000660: 2020 2020 2020 2020 2054 6865 206d 6174           The mat
+00000670: 6368 6564 2074 6578 742e 0a0a 2020 2020  ched text...    
+00000680: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00000690: 2020 2020 2020 4261 646c 7953 7065 6369        BadlySpeci
+000006a0: 6669 6564 5465 6d70 6c61 7465 4572 726f  fiedTemplateErro
+000006b0: 723a 2049 6620 7468 6572 6520 6973 2061  r: If there is a
+000006c0: 206d 6973 6d61 7463 6820 6265 7477 6565   mismatch betwee
+000006d0: 6e20 7468 650a 2020 2020 2020 2020 2020  n the.          
+000006e0: 2020 6578 7065 6374 6564 5f70 6172 7473    expected_parts
+000006f0: 2061 6e64 2074 6865 2073 7472 696e 672e   and the string.
+00000700: 0a20 2020 2020 2020 2020 2056 616c 7565  .          Value
+00000710: 4572 726f 723a 2049 6620 7468 6572 6520  Error: If there 
+00000720: 6973 206d 6f72 6520 7468 616e 206f 6e65  is more than one
+00000730: 2054 6578 7450 6c61 6365 686f 6c64 6572   TextPlaceholder
+00000740: 2069 6e20 6120 7277 6f0a 2020 2020 2020   in a rwo.      
+00000750: 2020 7a46 5768 656e 2061 7474 656d 7074    zFWhen attempt
+00000760: 696e 6720 746f 206d 6174 6368 2073 7472  ing to match str
+00000770: 696e 6720 227b 7d22 2077 6974 6820 7b7d  ing "{}" with {}
+00000780: 2c20 7468 6973 2065 7272 6f72 2072 6573  , this error res
+00000790: 756c 7465 643a 0a0a 7b7d 4e54 2912 da10  ulted:..{}NT)...
+000007a0: 4d61 7463 6857 6869 7465 5370 6163 6573  MatchWhiteSpaces
+000007b0: da10 4d61 7463 6853 7461 7274 5061 7265  ..MatchStartPare
+000007c0: 6e73 7202 0000 0072 0e00 0000 720c 0000  nsr....r....r...
+000007d0: 00da 1473 7461 7274 5f70 6172 656e 5f6d  ...start_paren_m
+000007e0: 6174 6368 6572 73da 0d4d 6174 6368 456e  atchers..MatchEn
+000007f0: 6450 6172 656e 7206 0000 00da 0666 6f72  dParenr......for
+00000800: 6d61 74da 076d 6573 7361 6765 7207 0000  mat..messager...
+00000810: 00da 0947 6574 536f 7572 6365 da0f 4d61  ...GetSource..Ma
+00000820: 7463 6843 6f6d 6d65 6e74 454f 4cda 1365  tchCommentEOL..e
+00000830: 6e64 5f6f 665f 6c69 6e65 5f63 6f6d 6d65  nd_of_line_comme
+00000840: 6e74 da11 4765 7457 6869 7465 5370 6163  nt..GetWhiteSpac
+00000850: 6554 6578 74da 1765 6e64 5f77 6869 7465  eText..end_white
+00000860: 7370 6163 655f 6d61 7463 6865 7273 da07  space_matchers..
+00000870: 6d61 7463 6865 64da 0e6d 6174 6368 6564  matched..matched
+00000880: 5f73 6f75 7263 6529 0772 0d00 0000 da06  _source).r......
+00000890: 7374 7269 6e67 da10 7265 6d61 696e 696e  string..remainin
+000008a0: 675f 7374 7269 6e67 da01 65da 0e6d 6174  g_string..e..mat
+000008b0: 6368 6564 5f73 7472 696e 67da 0665 6e64  ched_string..end
+000008c0: 5f77 73da 0672 6573 756c 7472 1500 0000  _ws..resultr....
+000008d0: 7215 0000 0072 1600 0000 da06 5f6d 6174  r....r......_mat
+000008e0: 6368 1c00 0000 732c 0000 000a 150a 0102  ch....s,........
+000008f0: 0302 010a 0104 0104 fe0e 030e 0202 0102  ................
+00000900: 010c 0204 fd08 8002 ff0a 050c 010c 010e  ................
+00000910: 0106 0106 0104 017a 1b44 6566 6175 6c74  .......z.Default
+00000920: 536f 7572 6365 4d61 7463 6865 722e 5f6d  SourceMatcher._m
+00000930: 6174 6368 6301 0000 0000 0000 0000 0000  atchc...........
+00000940: 0005 0000 0006 0000 0043 0000 0073 a600  .........C...s..
+00000950: 0000 7c00 a000 a100 0100 7c00 6a01 720a  ..|.......|.j.r.
+00000960: 7c00 6a02 5300 6700 7d01 7c00 6a03 4400  |.j.S.g.}.|.j.D.
+00000970: 5d0d 7d02 7c02 a004 7c00 6a05 a101 7d03  ].}.|...|.j...}.
+00000980: 7c01 a006 7c03 a101 0100 710f 6401 a007  |...|.....q.d...
+00000990: 7c01 a101 7d04 6402 a008 7c00 a009 a100  |...}.d...|.....
+000009a0: 7c04 7c00 a00a a100 a103 7d04 7c00 6a0b  |.|.......}.|.j.
+000009b0: 723a 6403 a008 7c00 a00c 7c00 6a0b a101  r:d...|...|.j...
+000009c0: 7c04 a102 7d04 7c00 6a0d 7247 6403 a008  |...}.|.j.rGd...
+000009d0: 7c04 7c00 a00c 7c00 6a0d a101 a102 7d04  |.|...|.j.....}.
+000009e0: 7c00 6a0e 7251 6403 a008 7c04 7c00 6a0e  |.j.rQd...|.|.j.
+000009f0: a102 7d04 7c04 5300 2904 4eda 007a 067b  ..}.|.S.).N..z.{
+00000a00: 7d7b 7d7b 7d7a 047b 7d7b 7d29 0fda 1776  }{}{}z.{}{})...v
+00000a10: 616c 6964 6174 6564 5f63 616c 6c5f 746f  alidated_call_to
+00000a20: 5f6d 6174 6368 7222 0000 0072 2300 0000  _matchr"...r#...
+00000a30: 720c 0000 0072 1d00 0000 720e 0000 00da  r....r....r.....
+00000a40: 0661 7070 656e 64da 046a 6f69 6e72 1b00  .append..joinr..
+00000a50: 0000 da11 4765 7453 7461 7274 5061 7265  ....GetStartPare
+00000a60: 6e54 6578 74da 0f47 6574 456e 6450 6172  nText..GetEndPar
+00000a70: 656e 5465 7874 da19 7374 6172 745f 7768  enText..start_wh
+00000a80: 6974 6573 7061 6365 5f6d 6174 6368 6572  itespace_matcher
+00000a90: 7372 2000 0000 7221 0000 0072 1f00 0000  sr ...r!...r....
+00000aa0: 2905 720d 0000 00da 0b73 6f75 7263 655f  ).r......source_
+00000ab0: 6c69 7374 7212 0000 00da 0b70 6172 745f  listr......part_
+00000ac0: 736f 7572 6365 da06 736f 7572 6365 7215  source..sourcer.
+00000ad0: 0000 0072 1500 0000 7216 0000 0072 1d00  ...r....r....r..
+00000ae0: 0000 4900 0000 7328 0000 0008 0106 0106  ..I...s(........
+00000af0: 0104 010a 010c 010c 010a 0104 0106 0102  ................
+00000b00: 0106 0104 fd06 0514 0106 0114 0106 010e  ................
+00000b10: 0104 017a 1e44 6566 6175 6c74 536f 7572  ...z.DefaultSour
+00000b20: 6365 4d61 7463 6865 722e 4765 7453 6f75  ceMatcher.GetSou
+00000b30: 7263 6563 0100 0000 0000 0000 0000 0000  rcec............
+00000b40: 0100 0000 0700 0000 0300 0000 7322 0000  ............s"..
+00000b50: 0064 01a0 0074 0174 027c 0083 02a0 03a1  .d...t.t.|......
+00000b60: 007c 006a 0474 05a0 067c 006a 07a1 01a1  .|.j.t...|.j....
+00000b70: 0353 0029 024e 7a3f 4465 6661 756c 7453  .S.).Nz?DefaultS
+00000b80: 6f75 7263 654d 6174 6368 6572 2022 7b7d  ourceMatcher "{}
+00000b90: 2220 666f 7220 6e6f 6465 2022 7b7d 2220  " for node "{}" 
+00000ba0: 6578 7065 6374 696e 6720 746f 206d 6174  expecting to mat
+00000bb0: 6368 2022 7b7d 2229 0872 1b00 0000 7208  ch "{}").r....r.
+00000bc0: 0000 0072 0700 0000 da08 5f5f 7265 7072  ...r......__repr
+00000bd0: 5f5f 720e 0000 00da 0670 7072 696e 74da  __r......pprint.
+00000be0: 0770 666f 726d 6174 720c 0000 0029 0172  .pformatr....).r
+00000bf0: 0d00 0000 7213 0000 0072 1500 0000 7216  ....r....r....r.
+00000c00: 0000 0072 3500 0000 5f00 0000 730c 0000  ...r5..._...s...
+00000c10: 0002 010e 0104 010a 0102 fe02 ff7a 1d44  .............z.D
+00000c20: 6566 6175 6c74 536f 7572 6365 4d61 7463  efaultSourceMatc
+00000c30: 6865 722e 5f5f 7265 7072 5f5f 6302 0000  her.__repr__c...
+00000c40: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00000c50: 0043 0000 0073 2a00 0000 7c00 6a00 6401  .C...s*...|.j.d.
+00000c60: 1900 7d02 7c02 a001 6400 7c01 a102 7d03  ..}.|...d.|...}.
+00000c70: 7c01 7402 7c03 8301 6400 8502 1900 7d01  |.t.|...d.....}.
+00000c80: 7c01 5300 2902 4e72 0100 0000 2903 7231  |.S.).Nr....).r1
+00000c90: 0000 0072 2a00 0000 da03 6c65 6e29 0472  ...r*.....len).r
+00000ca0: 0d00 0000 7225 0000 00da 0e77 735f 706c  ....r%.....ws_pl
+00000cb0: 6163 6568 6f6c 6465 72da 086d 6174 6368  aceholder..match
+00000cc0: 5f77 7372 1500 0000 7215 0000 0072 1600  _wsr....r....r..
+00000cd0: 0000 7217 0000 0065 0000 0073 0800 0000  ..r....e...s....
+00000ce0: 0a01 0c01 1001 0401 7a25 4465 6661 756c  ........z%Defaul
+00000cf0: 7453 6f75 7263 654d 6174 6368 6572 2e4d  tSourceMatcher.M
+00000d00: 6174 6368 5768 6974 6553 7061 6365 7329  atchWhiteSpaces)
+00000d10: 024e 4e29 0ada 085f 5f6e 616d 655f 5fda  .NN)...__name__.
+00000d20: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000d30: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00000d40: 5f5f 7209 0000 0072 2a00 0000 721d 0000  __r....r*...r...
+00000d50: 0072 3500 0000 7217 0000 00da 0d5f 5f63  .r5...r......__c
+00000d60: 6c61 7373 6365 6c6c 5f5f 7215 0000 0072  lasscell__r....r
+00000d70: 1500 0000 7213 0000 0072 1600 0000 7207  ....r....r....r.
+00000d80: 0000 000a 0000 0073 0e00 0000 0800 0401  .......s........
+00000d90: 0e02 080f 082d 0c16 1006 7207 0000 0029  .....-....r....)
+00000da0: 0c72 3600 0000 da24 6675 6e5f 7769 7468  .r6....$fun_with
+00000db0: 5f61 7374 2e70 6c61 6365 686f 6c64 6572  _ast.placeholder
+00000dc0: 732e 6261 7365 5f6d 6174 6368 7202 0000  s.base_matchr...
+00000dd0: 00da 2a66 756e 5f77 6974 685f 6173 742e  ..*fun_with_ast.
+00000de0: 706c 6163 6568 6f6c 6465 7273 2e62 6173  placeholders.bas
+00000df0: 655f 706c 6163 6568 6f6c 6465 7272 0300  e_placeholderr..
+00000e00: 0000 da1e 6675 6e5f 7769 7468 5f61 7374  ....fun_with_ast
+00000e10: 2e70 6c61 6365 686f 6c64 6572 732e 7465  .placeholders.te
+00000e20: 7874 7204 0000 00da 2966 756e 5f77 6974  xtr.....)fun_wit
+00000e30: 685f 6173 742e 736f 7572 6365 5f6d 6174  h_ast.source_mat
+00000e40: 6368 6572 732e 6261 7365 5f6d 6174 6368  chers.base_match
+00000e50: 6572 7205 0000 00da 2766 756e 5f77 6974  err.....'fun_wit
+00000e60: 685f 6173 742e 736f 7572 6365 5f6d 6174  h_ast.source_mat
+00000e70: 6368 6572 732e 6578 6365 7074 696f 6e73  chers.exceptions
+00000e80: 7206 0000 0072 0700 0000 7215 0000 0072  r....r....r....r
+00000e90: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
+00000ea0: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
+00000eb0: 0008 000c 020c 010c 010c 010c 0114 03    ...............
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/exceptions.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/if_source_match.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/if_source_match.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 03:44:30 2023 UTC, .py size: 4765 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,237 +1,241 @@
-00000000: 6f0d 0d0a 0000 0000 9e7d 8e64 9d12 0000  o........}.d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 d712 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
+00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6407 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
-00000080: 6d0e 5a0e 0100 6400 6408 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-00000090: 0100 4700 6409 640a 8400 640a 650c 8303  ..G.d.d...d.e...
-000000a0: 5a11 6401 5300 290b e900 0000 004e 2901  Z.d.S.)......N).
-000000b0: da0f 426f 6479 506c 6163 6568 6f6c 6465  ..BodyPlaceholde
-000000c0: 7229 01da 1046 6965 6c64 506c 6163 6568  r)...FieldPlaceh
-000000d0: 6f6c 6465 7229 01da 144c 6973 7446 6965  older)...ListFie
-000000e0: 6c64 506c 6163 6568 6f6c 6465 7229 01da  ldPlaceholder)..
-000000f0: 0e53 796e 7461 7846 7265 654c 696e 6529  .SyntaxFreeLine)
-00000100: 01da 0947 6574 536f 7572 6365 2903 da0d  ...GetSource)...
-00000110: 536f 7572 6365 4d61 7463 6865 72da 144d  SourceMatcher..M
-00000120: 6174 6368 506c 6163 6568 6f6c 6465 724c  atchPlaceholderL
-00000130: 6973 74da 104d 6174 6368 506c 6163 6568  ist..MatchPlaceh
-00000140: 6f6c 6465 7229 01da 0f54 6578 7450 6c61  older)...TextPla
-00000150: 6365 686f 6c64 6572 6300 0000 0000 0000  ceholderc.......
-00000160: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-00000170: 0073 5600 0000 6500 5a01 6400 5a02 6401  .sV...e.Z.d.Z.d.
-00000180: 5a03 6411 8700 6601 6403 6404 8409 5a04  Z.d...f.d.d...Z.
-00000190: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
-000001a0: 6409 640a 8400 5a07 6508 640b 640c 8400  d.d...Z.e.d.d...
-000001b0: 8301 5a09 640d 640e 8400 5a0a 640f 6410  ..Z.d.d...Z.d.d.
-000001c0: 8400 5a0b 8700 0400 5a0c 5300 2912 da0f  ..Z.....Z.S.)...
-000001d0: 4966 536f 7572 6365 4d61 7463 6865 727a  IfSourceMatcherz
-000001e0: 3143 6c61 7373 2074 6f20 6765 6e65 7261  1Class to genera
-000001f0: 7465 2074 6865 2073 6f75 7263 6520 666f  te the source fo
-00000200: 7220 616e 205f 6173 742e 4966 206e 6f64  r an _ast.If nod
-00000210: 652e 4e63 0400 0000 0000 0000 0000 0000  e.Nc............
-00000220: 0400 0000 0400 0000 0300 0000 7364 0000  ............sd..
-00000230: 0074 0074 017c 0083 02a0 027c 017c 02a1  .t.t.|.....|.|..
-00000240: 0201 0074 0364 0164 0283 027c 005f 0474  ...t.d.d...|._.t
-00000250: 0564 0383 017c 005f 0674 0364 0464 0583  .d...|._.t.d.d..
-00000260: 027c 005f 0774 0864 0683 017c 005f 0974  .|._.t.d...|._.t
-00000270: 0364 0764 0883 027c 005f 0a74 0864 0983  .d.d...|._.t.d..
-00000280: 017c 005f 0b64 0a7c 005f 0c64 0b7c 005f  .|._.d.|._.d.|._
-00000290: 0d64 0053 0029 0c4e 7a07 202a 6966 5c73  .d.S.).Nz. *if\s
-000002a0: 2a7a 0369 6620 da04 7465 7374 7a0f 5b20  *z.if ..testz.[ 
-000002b0: 5c74 5d2a 3a5b 205c 745d 2a5c 6e7a 023a  \t]*:[ \t]*\nz.:
-000002c0: 0ada 0462 6f64 797a 0f20 2a65 6c73 653a  ...bodyz. *else:
-000002d0: 5b20 5c74 5d2a 5c6e fa06 656c 7365 3a0a  [ \t]*\n..else:.
-000002e0: da06 6f72 656c 7365 4672 0100 0000 290e  ..orelseFr....).
-000002f0: da05 7375 7065 7272 0b00 0000 da08 5f5f  ..superr......__
-00000300: 696e 6974 5f5f 720a 0000 00da 0e69 665f  init__r......if_
-00000310: 706c 6163 6568 6f6c 6465 7272 0300 0000  placeholderr....
-00000320: da10 7465 7374 5f70 6c61 6365 686f 6c64  ..test_placehold
-00000330: 6572 da14 6966 5f63 6f6c 6f6e 5f70 6c61  er..if_colon_pla
-00000340: 6365 686f 6c64 6572 7202 0000 00da 1062  ceholderr......b
-00000350: 6f64 795f 706c 6163 6568 6f6c 6465 72da  ody_placeholder.
-00000360: 1065 6c73 655f 706c 6163 6568 6f6c 6465  .else_placeholde
-00000370: 72da 126f 7265 6c73 655f 706c 6163 6568  r..orelse_placeh
-00000380: 6f6c 6465 72da 0769 735f 656c 6966 da09  older..is_elif..
-00000390: 6966 5f69 6e64 656e 7429 04da 0473 656c  if_indent)...sel
-000003a0: 66da 046e 6f64 65da 0f73 7461 7274 696e  f..node..startin
-000003b0: 675f 7061 7265 6e73 da06 7061 7265 6e74  g_parens..parent
-000003c0: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-000003d0: 472f 686f 6d65 2f73 6861 692f 6675 6e5f  G/home/shai/fun_
-000003e0: 7769 7468 5f61 7374 2f66 756e 5f77 6974  with_ast/fun_wit
-000003f0: 685f 6173 742f 736f 7572 6365 5f6d 6174  h_ast/source_mat
-00000400: 6368 6572 732f 6966 5f73 6f75 7263 655f  chers/if_source_
-00000410: 6d61 7463 682e 7079 7211 0000 000f 0000  match.pyr.......
-00000420: 0073 1200 0000 1201 0c01 0a01 0c01 0a01  .s..............
-00000430: 0c01 0a01 0601 0a01 7a18 4966 536f 7572  ........z.IfSour
-00000440: 6365 4d61 7463 6865 722e 5f5f 696e 6974  ceMatcher.__init
-00000450: 5f5f 6302 0000 0000 0000 0000 0000 0004  __c.............
-00000460: 0000 0004 0000 0043 0000 0073 6800 0000  .......C...sh...
-00000470: 7400 7c01 8301 7400 7c01 a001 a100 8301  t.|...t.|.......
-00000480: 1800 7c00 5f02 7c00 6a03 7d02 7404 7c01  ..|._.|.j.}.t.|.
-00000490: 7c00 6a05 7c02 8303 7d03 7c00 6a05 6a06  |.j.|...}.|.j.j.
-000004a0: 731d 7c00 a007 a100 5300 7c00 a008 7c03  s.|.....S.|...|.
-000004b0: a101 7d03 7c00 6a09 a00a 7c00 6a05 7c03  ..}.|.j...|.j.|.
-000004c0: a102 7d03 7c03 7330 740b 6401 8301 8201  ..}.|.s0t.d.....
-000004d0: 7c00 a007 a100 5300 2902 4e7a 1043 616e  |.....S.).Nz.Can
-000004e0: 2077 6520 6765 7420 6865 7265 3f29 0cda   we get here?)..
-000004f0: 036c 656e da06 6c73 7472 6970 7219 0000  .len..lstripr...
-00000500: 00da 0e65 7870 6563 7465 645f 7061 7274  ...expected_part
-00000510: 7372 0800 0000 721b 0000 0072 0f00 0000  sr....r....r....
-00000520: da12 5f72 6574 7572 6e5f 6672 6f6d 5f6d  .._return_from_m
-00000530: 6174 6368 da0d 5f6d 6174 6368 5f6f 7265  atch.._match_ore
-00000540: 6c73 6572 1700 0000 da06 5f6d 6174 6368  lser......_match
-00000550: da0a 5661 6c75 6545 7272 6f72 2904 721a  ..ValueError).r.
-00000560: 0000 00da 0673 7472 696e 67da 1070 6c61  .....string..pla
-00000570: 6365 686f 6c64 6572 5f6c 6973 74da 1072  ceholder_list..r
-00000580: 656d 6169 6e69 6e67 5f73 7472 696e 6772  emaining_stringr
-00000590: 2000 0000 7220 0000 0072 2100 0000 7227   ...r ...r!...r'
-000005a0: 0000 001a 0000 0073 1c00 0000 1601 0601  .......s........
-000005b0: 0201 0801 04ff 0802 0801 0a02 0601 0601  ................
-000005c0: 04ff 0402 0801 0801 7a16 4966 536f 7572  ........z.IfSour
-000005d0: 6365 4d61 7463 6865 722e 5f6d 6174 6368  ceMatcher._match
-000005e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000005f0: 0003 0000 0043 0000 0073 1a00 0000 7400  .....C...s....t.
-00000600: a001 7c00 a101 7d01 6401 7c00 5f02 7c01  ..|...}.d.|._.|.
-00000610: 7c00 5f03 7c01 5300 2902 4e54 2904 720b  |._.|.S.).NT).r.
-00000620: 0000 0072 0600 0000 da07 6d61 7463 6865  ...r......matche
-00000630: 64da 0e6d 6174 6368 6564 5f73 6f75 7263  d..matched_sourc
-00000640: 6529 0272 1a00 0000 da06 7265 7375 6c74  e).r......result
-00000650: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-00000660: 2500 0000 2900 0000 7308 0000 000a 0106  %...)...s.......
-00000670: 0106 0104 017a 2249 6653 6f75 7263 654d  .....z"IfSourceM
-00000680: 6174 6368 6572 2e5f 7265 7475 726e 5f66  atcher._return_f
-00000690: 726f 6d5f 6d61 7463 6863 0200 0000 0000  rom_matchc......
-000006a0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-000006b0: 0000 73ac 0000 007c 00a0 00a1 0001 007c  ..s....|.......|
-000006c0: 006a 0172 0a7c 006a 0253 0074 03a0 047c  .j.r.|.j.S.t...|
-000006d0: 01a1 0172 237c 006a 05a0 067c 01a1 015c  ...r#|.j...|...\
-000006e0: 027d 017d 027c 006a 076a 08a0 097c 02a1  .}.}.|.j.j...|..
-000006f0: 0101 0074 03a0 047c 01a1 0173 0f7c 01a0  ...t...|...s.|..
-00000700: 0aa1 00a0 0b64 01a1 0172 4c64 027c 005f  .....d...rLd.|._
-00000710: 0c74 0d7c 0183 0174 0d7c 01a0 0aa1 0083  .t.|...t.|......
-00000720: 0118 007d 037c 0164 007c 0385 0219 007c  ...}.|.d.|.....|
-00000730: 017c 0364 0317 0064 0085 0219 0017 007d  .|.d...d.......}
-00000740: 0174 0e64 0483 017c 005f 0f7c 0153 0074  .t.d...|._.|.S.t
-00000750: 107c 017c 006a 077c 006a 1183 037d 017c  .|.|.j.|.j...}.|
-00000760: 0153 0029 054e da04 656c 6966 54e9 0200  .S.).N..elifT...
-00000770: 0000 720f 0000 0029 12da 1776 616c 6964  ..r....)...valid
-00000780: 6174 6564 5f63 616c 6c5f 746f 5f6d 6174  ated_call_to_mat
-00000790: 6368 722c 0000 0072 2d00 0000 7205 0000  chr,...r-...r...
-000007a0: 00da 0c4d 6174 6368 6573 5374 6172 7472  ...MatchesStartr
-000007b0: 1500 0000 da13 4d61 7463 6853 796e 7461  ......MatchSynta
-000007c0: 7846 7265 654c 696e 6572 1b00 0000 720d  xFreeLiner....r.
-000007d0: 0000 00da 0661 7070 656e 6472 2300 0000  .....appendr#...
-000007e0: da0a 7374 6172 7473 7769 7468 7218 0000  ..startswithr...
-000007f0: 0072 2200 0000 7204 0000 0072 1700 0000  .r"...r....r....
-00000800: 7209 0000 0072 1600 0000 2904 721a 0000  r....r....).r...
-00000810: 0072 2b00 0000 da10 7379 6e74 6178 5f66  .r+.....syntax_f
-00000820: 7265 655f 6e6f 6465 da06 696e 6465 6e74  ree_node..indent
-00000830: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-00000840: 2600 0000 2f00 0000 7328 0000 0008 0406  &.../...s(......
-00000850: 0106 010a 020a 0206 ff0e 020a fd0e 0406  ................
-00000860: 0114 010a 010e 0104 ff0a 0604 0402 fe0a  ................
-00000870: 0104 ff04 027a 1d49 6653 6f75 7263 654d  .....z.IfSourceM
-00000880: 6174 6368 6572 2e5f 6d61 7463 685f 6f72  atcher._match_or
-00000890: 656c 7365 6301 0000 0000 0000 0000 0000  elsec...........
-000008a0: 0001 0000 0004 0000 0043 0000 0073 1400  .........C...s..
-000008b0: 0000 7c00 6a00 7c00 6a01 7c00 6a02 7c00  ..|.j.|.j.|.j.|.
-000008c0: 6a03 6704 5300 2901 4e29 0472 1200 0000  j.g.S.).N).r....
-000008d0: 7213 0000 0072 1400 0000 7215 0000 00a9  r....r....r.....
-000008e0: 0172 1a00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
-000008f0: 7221 0000 0072 2400 0000 4a00 0000 730a  r!...r$...J...s.
-00000900: 0000 0004 0204 0104 0104 0104 fd7a 1e49  .............z.I
-00000910: 6653 6f75 7263 654d 6174 6368 6572 2e65  fSourceMatcher.e
-00000920: 7870 6563 7465 645f 7061 7274 7363 0100  xpected_partsc..
-00000930: 0000 0000 0000 0000 0000 0500 0000 0600  ................
-00000940: 0000 0300 0000 73f0 0000 0088 006a 007d  ......s......j.}
-00000950: 0187 0066 0164 0164 0284 087c 0144 0083  ...f.d.d...|.D..
-00000960: 017d 0288 006a 016a 0273 1564 03a0 037c  .}...j.j.s.d...|
-00000970: 02a1 0153 0074 0488 006a 016a 0283 0164  ...S.t...j.j...d
-00000980: 046b 0272 4e74 0588 006a 016a 0264 0519  .k.rNt...j.j.d..
-00000990: 0074 066a 0783 0272 4e88 006a 0872 4e74  .t.j...rN..j.rNt
-000009a0: 0988 006a 016a 0264 0519 0083 017d 0374  ...j.j.d.....}.t
-000009b0: 047c 0383 0174 047c 03a0 0aa1 0083 0118  .|...t.|........
-000009c0: 007d 047c 02a0 0b7c 0364 007c 0485 0219  .}.|...|.d.|....
-000009d0: 0064 0617 007c 037c 0464 0085 0219 0017  .d...|.|.d......
-000009e0: 00a1 0101 006e 2588 006a 0c72 5c7c 02a0  .....n%..j.r\|..
-000009f0: 0b88 006a 0ca0 0988 006a 01a1 01a1 0101  ...j.....j......
-00000a00: 006e 0d7c 02a0 0b64 0788 006a 0d14 00a1  .n.|...d...j....
-00000a10: 0101 007c 02a0 0b64 08a1 0101 007c 02a0  ...|...d.....|..
-00000a20: 0b88 006a 0ea0 0988 006a 01a1 01a1 0101  ...j.....j......
-00000a30: 0064 03a0 037c 02a1 0153 0029 094e 6301  .d...|...S.).Nc.
-00000a40: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00000a50: 0000 0013 0000 0073 1800 0000 6700 7c00  .......s....g.|.
-00000a60: 5d08 7d01 7c01 a000 8800 6a01 a101 9102  ].}.|.....j.....
-00000a70: 7102 5300 7220 0000 0029 0272 0600 0000  q.S.r ...).r....
-00000a80: 721b 0000 0029 02da 022e 30da 0170 7238  r....)....0..pr8
-00000a90: 0000 0072 2000 0000 7221 0000 00da 0a3c  ...r ...r!.....<
-00000aa0: 6c69 7374 636f 6d70 3e53 0000 0073 0200  listcomp>S...s..
-00000ab0: 0000 1800 7a2d 4966 536f 7572 6365 4d61  ....z-IfSourceMa
-00000ac0: 7463 6865 722e 4765 7453 6f75 7263 652e  tcher.GetSource.
-00000ad0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000ae0: 6d70 3eda 00e9 0100 0000 7201 0000 00da  mp>.......r.....
-00000af0: 0265 6cfa 0120 720e 0000 0029 0f72 2400  .el.. r....).r$.
-00000b00: 0000 721b 0000 0072 0f00 0000 da04 6a6f  ..r....r......jo
-00000b10: 696e 7222 0000 00da 0a69 7369 6e73 7461  inr".....isinsta
-00000b20: 6e63 65da 045f 6173 74da 0249 6672 1800  nce.._ast..Ifr..
-00000b30: 0000 7206 0000 0072 2300 0000 7234 0000  ..r....r#...r4..
-00000b40: 0072 1600 0000 7219 0000 0072 1700 0000  .r....r....r....
-00000b50: 2905 721a 0000 0072 2a00 0000 da0b 736f  ).r....r*.....so
-00000b60: 7572 6365 5f6c 6973 74da 0b65 6c69 665f  urce_list..elif_
-00000b70: 736f 7572 6365 7237 0000 0072 2000 0000  sourcer7...r ...
-00000b80: 7238 0000 0072 2100 0000 7206 0000 0051  r8...r!...r....Q
-00000b90: 0000 0073 2400 0000 0601 1201 0801 0a01  ...s$...........
-00000ba0: 1001 1201 02ff 0402 02fe 1003 1401 2401  ..............$.
-00000bb0: 0602 1601 1002 0a01 1401 0a01 7a19 4966  ............z.If
-00000bc0: 536f 7572 6365 4d61 7463 6865 722e 4765  SourceMatcher.Ge
-00000bd0: 7453 6f75 7263 6563 0100 0000 0000 0000  tSourcec........
-00000be0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000bf0: 7334 0000 007c 006a 006a 0173 0f7c 006a  s4...|.j.j.s.|.j
-00000c00: 006a 0264 0119 006a 03a0 04a1 0001 0064  .j.d...j.......d
-00000c10: 0053 007c 006a 006a 0264 0119 006a 03a0  .S.|.j.j.d...j..
-00000c20: 04a1 0001 0064 0053 0029 024e e9ff ffff  .....d.S.).N....
-00000c30: ff29 0572 1b00 0000 720f 0000 0072 0d00  .).r....r....r..
-00000c40: 0000 da07 6d61 7463 6865 72da 1561 6464  ....matcher..add
-00000c50: 5f6e 6577 6c69 6e65 5f74 6f5f 736f 7572  _newline_to_sour
-00000c60: 6365 7238 0000 0072 2000 0000 7220 0000  cer8...r ...r ..
-00000c70: 0072 2100 0000 7248 0000 0065 0000 0073  .r!...rH...e...s
-00000c80: 0600 0000 0801 1601 1602 7a25 4966 536f  ..........z%IfSo
-00000c90: 7572 6365 4d61 7463 6865 722e 6164 645f  urceMatcher.add_
-00000ca0: 6e65 776c 696e 655f 746f 5f73 6f75 7263  newline_to_sourc
-00000cb0: 6529 024e 4e29 0dda 085f 5f6e 616d 655f  e).NN)...__name_
-00000cc0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000cd0: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
-00000ce0: 6f63 5f5f 7211 0000 0072 2700 0000 7225  oc__r....r'...r%
-00000cf0: 0000 0072 2600 0000 da08 7072 6f70 6572  ...r&.....proper
-00000d00: 7479 7224 0000 0072 0600 0000 7248 0000  tyr$...r....rH..
-00000d10: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000d20: 7220 0000 0072 2000 0000 721e 0000 0072  r ...r ...r....r
-00000d30: 2100 0000 720b 0000 000c 0000 0073 1400  !...r........s..
-00000d40: 0000 0800 0401 0e02 080b 080f 0806 021b  ................
-00000d50: 0a01 0806 1014 720b 0000 0029 1272 4200  ......r....).rB.
-00000d60: 0000 da21 6675 6e5f 7769 7468 5f61 7374  ...!fun_with_ast
-00000d70: 2e73 6f75 7263 655f 6d61 7463 6865 7273  .source_matchers
-00000d80: 2e62 6f64 7972 0200 0000 da23 6675 6e5f  .bodyr.....#fun_
-00000d90: 7769 7468 5f61 7374 2e70 6c61 6365 686f  with_ast.placeho
-00000da0: 6c64 6572 732e 636f 6d70 6f73 6974 6572  lders.compositer
-00000db0: 0300 0000 da2a 6675 6e5f 7769 7468 5f61  .....*fun_with_a
-00000dc0: 7374 2e70 6c61 6365 686f 6c64 6572 732e  st.placeholders.
-00000dd0: 6c69 7374 5f70 6c61 6365 686f 6c64 6572  list_placeholder
-00000de0: 7204 0000 00da 2866 756e 5f77 6974 685f  r.....(fun_with_
-00000df0: 6173 742e 6d61 6e69 7075 6c61 7465 5f6e  ast.manipulate_n
-00000e00: 6f64 652e 6372 6561 7465 5f6e 6f64 6572  ode.create_noder
-00000e10: 0500 0000 da17 6675 6e5f 7769 7468 5f61  ......fun_with_a
-00000e20: 7374 2e67 6574 5f73 6f75 7263 6572 0600  st.get_sourcer..
-00000e30: 0000 da29 6675 6e5f 7769 7468 5f61 7374  ...)fun_with_ast
-00000e40: 2e73 6f75 7263 655f 6d61 7463 6865 7273  .source_matchers
-00000e50: 2e62 6173 655f 6d61 7463 6865 7272 0700  .base_matcherr..
-00000e60: 0000 7208 0000 0072 0900 0000 da1e 6675  ..r....r......fu
-00000e70: 6e5f 7769 7468 5f61 7374 2e70 6c61 6365  n_with_ast.place
-00000e80: 686f 6c64 6572 732e 7465 7874 720a 0000  holders.textr...
-00000e90: 0072 0b00 0000 7220 0000 0072 2000 0000  .r....r ...r ...
-00000ea0: 7220 0000 0072 2100 0000 da08 3c6d 6f64  r ...r!.....<mod
-00000eb0: 756c 653e 0100 0000 7312 0000 0008 000c  ule>....s.......
-00000ec0: 020c 010c 010c 010c 0114 010c 0114 03    ...............
+00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
+00000080: 6408 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6400  d.l.m.Z.m.Z...d.
+00000090: 6409 6c10 6d11 5a11 0100 4700 640a 640b  d.l.m.Z...G.d.d.
+000000a0: 8400 640b 650c 8303 5a12 6401 5300 290c  ..d.e...Z.d.S.).
+000000b0: e900 0000 004e 2901 da0f 426f 6479 506c  .....N)...BodyPl
+000000c0: 6163 6568 6f6c 6465 7229 01da 1046 6965  aceholder)...Fie
+000000d0: 6c64 506c 6163 6568 6f6c 6465 7229 01da  ldPlaceholder)..
+000000e0: 144c 6973 7446 6965 6c64 506c 6163 6568  .ListFieldPlaceh
+000000f0: 6f6c 6465 7229 01da 0e53 796e 7461 7846  older)...SyntaxF
+00000100: 7265 654c 696e 6529 01da 0947 6574 536f  reeLine)...GetSo
+00000110: 7572 6365 2901 da0d 536f 7572 6365 4d61  urce)...SourceMa
+00000120: 7463 6865 7229 02da 104d 6174 6368 506c  tcher)...MatchPl
+00000130: 6163 6568 6f6c 6465 72da 144d 6174 6368  aceholder..Match
+00000140: 506c 6163 6568 6f6c 6465 724c 6973 7429  PlaceholderList)
+00000150: 01da 0f54 6578 7450 6c61 6365 686f 6c64  ...TextPlacehold
+00000160: 6572 6300 0000 0000 0000 0000 0000 0000  erc.............
+00000170: 0000 0004 0000 0000 0000 0073 5600 0000  ...........sV...
+00000180: 6500 5a01 6400 5a02 6401 5a03 6411 8700  e.Z.d.Z.d.Z.d...
+00000190: 6601 6403 6404 8409 5a04 6405 6406 8400  f.d.d...Z.d.d...
+000001a0: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
+000001b0: 5a07 6508 640b 640c 8400 8301 5a09 640d  Z.e.d.d.....Z.d.
+000001c0: 640e 8400 5a0a 640f 6410 8400 5a0b 8700  d...Z.d.d...Z...
+000001d0: 0400 5a0c 5300 2912 da0f 4966 536f 7572  ..Z.S.)...IfSour
+000001e0: 6365 4d61 7463 6865 727a 3143 6c61 7373  ceMatcherz1Class
+000001f0: 2074 6f20 6765 6e65 7261 7465 2074 6865   to generate the
+00000200: 2073 6f75 7263 6520 666f 7220 616e 205f   source for an _
+00000210: 6173 742e 4966 206e 6f64 652e 4e63 0400  ast.If node.Nc..
+00000220: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000230: 0000 0300 0000 7364 0000 0074 0074 017c  ......sd...t.t.|
+00000240: 0083 02a0 027c 017c 02a1 0201 0074 0364  .....|.|.....t.d
+00000250: 0164 0283 027c 005f 0474 0564 0383 017c  .d...|._.t.d...|
+00000260: 005f 0674 0364 0464 0583 027c 005f 0774  ._.t.d.d...|._.t
+00000270: 0864 0683 017c 005f 0974 0364 0764 0883  .d...|._.t.d.d..
+00000280: 027c 005f 0a74 0864 0983 017c 005f 0b64  .|._.t.d...|._.d
+00000290: 0a7c 005f 0c64 0b7c 005f 0d64 0053 0029  .|._.d.|._.d.S.)
+000002a0: 0c4e 7a07 202a 6966 5c73 2a7a 0369 6620  .Nz. *if\s*z.if 
+000002b0: da04 7465 7374 7a0f 5b20 5c74 5d2a 3a5b  ..testz.[ \t]*:[
+000002c0: 205c 745d 2a5c 6e7a 023a 0ada 0462 6f64   \t]*\nz.:...bod
+000002d0: 797a 0f20 2a65 6c73 653a 5b20 5c74 5d2a  yz. *else:[ \t]*
+000002e0: 5c6e fa06 656c 7365 3a0a da06 6f72 656c  \n..else:...orel
+000002f0: 7365 4672 0100 0000 290e da05 7375 7065  seFr....)...supe
+00000300: 7272 0b00 0000 da08 5f5f 696e 6974 5f5f  rr......__init__
+00000310: 720a 0000 00da 0e69 665f 706c 6163 6568  r......if_placeh
+00000320: 6f6c 6465 7272 0300 0000 da10 7465 7374  olderr......test
+00000330: 5f70 6c61 6365 686f 6c64 6572 da14 6966  _placeholder..if
+00000340: 5f63 6f6c 6f6e 5f70 6c61 6365 686f 6c64  _colon_placehold
+00000350: 6572 7202 0000 00da 1062 6f64 795f 706c  err......body_pl
+00000360: 6163 6568 6f6c 6465 72da 1065 6c73 655f  aceholder..else_
+00000370: 706c 6163 6568 6f6c 6465 72da 126f 7265  placeholder..ore
+00000380: 6c73 655f 706c 6163 6568 6f6c 6465 72da  lse_placeholder.
+00000390: 0769 735f 656c 6966 da09 6966 5f69 6e64  .is_elif..if_ind
+000003a0: 656e 7429 04da 0473 656c 66da 046e 6f64  ent)...self..nod
+000003b0: 65da 0f73 7461 7274 696e 675f 7061 7265  e..starting_pare
+000003c0: 6e73 da06 7061 7265 6e74 a901 da09 5f5f  ns..parent....__
+000003d0: 636c 6173 735f 5fa9 00fa 472f 686f 6d65  class__...G/home
+000003e0: 2f73 6861 692f 6675 6e5f 7769 7468 5f61  /shai/fun_with_a
+000003f0: 7374 2f66 756e 5f77 6974 685f 6173 742f  st/fun_with_ast/
+00000400: 736f 7572 6365 5f6d 6174 6368 6572 732f  source_matchers/
+00000410: 6966 5f73 6f75 7263 655f 6d61 7463 682e  if_source_match.
+00000420: 7079 7211 0000 0010 0000 0073 1200 0000  pyr........s....
+00000430: 1201 0c01 0a01 0c01 0a01 0c01 0a01 0601  ................
+00000440: 0a01 7a18 4966 536f 7572 6365 4d61 7463  ..z.IfSourceMatc
+00000450: 6865 722e 5f5f 696e 6974 5f5f 6302 0000  her.__init__c...
+00000460: 0000 0000 0000 0000 0004 0000 0004 0000  ................
+00000470: 0043 0000 0073 6800 0000 7400 7c01 8301  .C...sh...t.|...
+00000480: 7400 7c01 a001 a100 8301 1800 7c00 5f02  t.|.........|._.
+00000490: 7c00 6a03 7d02 7404 7c01 7c00 6a05 7c02  |.j.}.t.|.|.j.|.
+000004a0: 8303 7d03 7c00 6a05 6a06 731d 7c00 a007  ..}.|.j.j.s.|...
+000004b0: a100 5300 7c00 a008 7c03 a101 7d03 7c00  ..S.|...|...}.|.
+000004c0: 6a09 a00a 7c00 6a05 7c03 a102 7d03 7c03  j...|.j.|...}.|.
+000004d0: 7330 740b 6401 8301 8201 7c00 a007 a100  s0t.d.....|.....
+000004e0: 5300 2902 4e7a 1043 616e 2077 6520 6765  S.).Nz.Can we ge
+000004f0: 7420 6865 7265 3f29 0cda 036c 656e da06  t here?)...len..
+00000500: 6c73 7472 6970 7219 0000 00da 0e65 7870  lstripr......exp
+00000510: 6563 7465 645f 7061 7274 7372 0900 0000  ected_partsr....
+00000520: 721b 0000 0072 0f00 0000 da12 5f72 6574  r....r......_ret
+00000530: 7572 6e5f 6672 6f6d 5f6d 6174 6368 da0d  urn_from_match..
+00000540: 5f6d 6174 6368 5f6f 7265 6c73 6572 1700  _match_orelser..
+00000550: 0000 da06 5f6d 6174 6368 da0a 5661 6c75  ...._match..Valu
+00000560: 6545 7272 6f72 2904 721a 0000 00da 0673  eError).r......s
+00000570: 7472 696e 67da 1070 6c61 6365 686f 6c64  tring..placehold
+00000580: 6572 5f6c 6973 74da 1072 656d 6169 6e69  er_list..remaini
+00000590: 6e67 5f73 7472 696e 6772 2000 0000 7220  ng_stringr ...r 
+000005a0: 0000 0072 2100 0000 7227 0000 001b 0000  ...r!...r'......
+000005b0: 0073 1c00 0000 1601 0601 0201 0801 04ff  .s..............
+000005c0: 0802 0801 0a02 0601 0601 04ff 0402 0801  ................
+000005d0: 0801 7a16 4966 536f 7572 6365 4d61 7463  ..z.IfSourceMatc
+000005e0: 6865 722e 5f6d 6174 6368 6301 0000 0000  her._matchc.....
+000005f0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000600: 0000 0073 1a00 0000 7400 a001 7c00 a101  ...s....t...|...
+00000610: 7d01 6401 7c00 5f02 7c01 7c00 5f03 7c01  }.d.|._.|.|._.|.
+00000620: 5300 2902 4e54 2904 720b 0000 0072 0600  S.).NT).r....r..
+00000630: 0000 da07 6d61 7463 6865 64da 0e6d 6174  ....matched..mat
+00000640: 6368 6564 5f73 6f75 7263 6529 0272 1a00  ched_source).r..
+00000650: 0000 da06 7265 7375 6c74 7220 0000 0072  ....resultr ...r
+00000660: 2000 0000 7221 0000 0072 2500 0000 2a00   ...r!...r%...*.
+00000670: 0000 7308 0000 000a 0106 0106 0104 017a  ..s............z
+00000680: 2249 6653 6f75 7263 654d 6174 6368 6572  "IfSourceMatcher
+00000690: 2e5f 7265 7475 726e 5f66 726f 6d5f 6d61  ._return_from_ma
+000006a0: 7463 6863 0200 0000 0000 0000 0000 0000  tchc............
+000006b0: 0400 0000 0400 0000 4300 0000 73ac 0000  ........C...s...
+000006c0: 007c 00a0 00a1 0001 007c 006a 0172 0a7c  .|.......|.j.r.|
+000006d0: 006a 0253 0074 03a0 047c 01a1 0172 237c  .j.S.t...|...r#|
+000006e0: 006a 05a0 067c 01a1 015c 027d 017d 027c  .j...|...\.}.}.|
+000006f0: 006a 076a 08a0 097c 02a1 0101 0074 03a0  .j.j...|.....t..
+00000700: 047c 01a1 0173 0f7c 01a0 0aa1 00a0 0b64  .|...s.|.......d
+00000710: 01a1 0172 4c64 027c 005f 0c74 0d7c 0183  ...rLd.|._.t.|..
+00000720: 0174 0d7c 01a0 0aa1 0083 0118 007d 037c  .t.|.........}.|
+00000730: 0164 007c 0385 0219 007c 017c 0364 0317  .d.|.....|.|.d..
+00000740: 0064 0085 0219 0017 007d 0174 0e64 0483  .d.......}.t.d..
+00000750: 017c 005f 0f7c 0153 0074 107c 017c 006a  .|._.|.S.t.|.|.j
+00000760: 077c 006a 1183 037d 017c 0153 0029 054e  .|.j...}.|.S.).N
+00000770: da04 656c 6966 54e9 0200 0000 720f 0000  ..elifT.....r...
+00000780: 0029 12da 1776 616c 6964 6174 6564 5f63  .)...validated_c
+00000790: 616c 6c5f 746f 5f6d 6174 6368 722c 0000  all_to_matchr,..
+000007a0: 0072 2d00 0000 7205 0000 00da 0c4d 6174  .r-...r......Mat
+000007b0: 6368 6573 5374 6172 7472 1500 0000 da13  chesStartr......
+000007c0: 4d61 7463 6853 796e 7461 7846 7265 654c  MatchSyntaxFreeL
+000007d0: 696e 6572 1b00 0000 720d 0000 00da 0661  iner....r......a
+000007e0: 7070 656e 6472 2300 0000 da0a 7374 6172  ppendr#.....star
+000007f0: 7473 7769 7468 7218 0000 0072 2200 0000  tswithr....r"...
+00000800: 7204 0000 0072 1700 0000 7208 0000 0072  r....r....r....r
+00000810: 1600 0000 2904 721a 0000 0072 2b00 0000  ....).r....r+...
+00000820: da10 7379 6e74 6178 5f66 7265 655f 6e6f  ..syntax_free_no
+00000830: 6465 da06 696e 6465 6e74 7220 0000 0072  de..indentr ...r
+00000840: 2000 0000 7221 0000 0072 2600 0000 3000   ...r!...r&...0.
+00000850: 0000 7328 0000 0008 0406 0106 010a 020a  ..s(............
+00000860: 0206 ff0e 020a fd0e 0406 0114 010a 010e  ................
+00000870: 0104 ff0a 0604 0402 fe0a 0104 ff04 027a  ...............z
+00000880: 1d49 6653 6f75 7263 654d 6174 6368 6572  .IfSourceMatcher
+00000890: 2e5f 6d61 7463 685f 6f72 656c 7365 6301  ._match_orelsec.
+000008a0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000008b0: 0000 0043 0000 0073 1400 0000 7c00 6a00  ...C...s....|.j.
+000008c0: 7c00 6a01 7c00 6a02 7c00 6a03 6704 5300  |.j.|.j.|.j.g.S.
+000008d0: 2901 4e29 0472 1200 0000 7213 0000 0072  ).N).r....r....r
+000008e0: 1400 0000 7215 0000 00a9 0172 1a00 0000  ....r......r....
+000008f0: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
+00000900: 2400 0000 4b00 0000 730a 0000 0004 0204  $...K...s.......
+00000910: 0104 0104 0104 fd7a 1e49 6653 6f75 7263  .......z.IfSourc
+00000920: 654d 6174 6368 6572 2e65 7870 6563 7465  eMatcher.expecte
+00000930: 645f 7061 7274 7363 0100 0000 0000 0000  d_partsc........
+00000940: 0000 0000 0500 0000 0600 0000 0300 0000  ................
+00000950: 73f0 0000 0088 006a 007d 0187 0066 0164  s......j.}...f.d
+00000960: 0164 0284 087c 0144 0083 017d 0288 006a  .d...|.D...}...j
+00000970: 016a 0273 1564 03a0 037c 02a1 0153 0074  .j.s.d...|...S.t
+00000980: 0488 006a 016a 0283 0164 046b 0272 4e74  ...j.j...d.k.rNt
+00000990: 0588 006a 016a 0264 0519 0074 066a 0783  ...j.j.d...t.j..
+000009a0: 0272 4e88 006a 0872 4e74 0988 006a 016a  .rN..j.rNt...j.j
+000009b0: 0264 0519 0083 017d 0374 047c 0383 0174  .d.....}.t.|...t
+000009c0: 047c 03a0 0aa1 0083 0118 007d 047c 02a0  .|.........}.|..
+000009d0: 0b7c 0364 007c 0485 0219 0064 0617 007c  .|.d.|.....d...|
+000009e0: 037c 0464 0085 0219 0017 00a1 0101 006e  .|.d...........n
+000009f0: 2588 006a 0c72 5c7c 02a0 0b88 006a 0ca0  %..j.r\|.....j..
+00000a00: 0988 006a 01a1 01a1 0101 006e 0d7c 02a0  ...j.......n.|..
+00000a10: 0b64 0788 006a 0d14 00a1 0101 007c 02a0  .d...j.......|..
+00000a20: 0b64 08a1 0101 007c 02a0 0b88 006a 0ea0  .d.....|.....j..
+00000a30: 0988 006a 01a1 01a1 0101 0064 03a0 037c  ...j.......d...|
+00000a40: 02a1 0153 0029 094e 6301 0000 0000 0000  ...S.).Nc.......
+00000a50: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+00000a60: 0073 1800 0000 6700 7c00 5d08 7d01 7c01  .s....g.|.].}.|.
+00000a70: a000 8800 6a01 a101 9102 7102 5300 7220  ....j.....q.S.r 
+00000a80: 0000 0029 0272 0600 0000 721b 0000 0029  ...).r....r....)
+00000a90: 02da 022e 30da 0170 7238 0000 0072 2000  ....0..pr8...r .
+00000aa0: 0000 7221 0000 00da 0a3c 6c69 7374 636f  ..r!.....<listco
+00000ab0: 6d70 3e54 0000 0073 0200 0000 1800 7a2d  mp>T...s......z-
+00000ac0: 4966 536f 7572 6365 4d61 7463 6865 722e  IfSourceMatcher.
+00000ad0: 4765 7453 6f75 7263 652e 3c6c 6f63 616c  GetSource.<local
+00000ae0: 733e 2e3c 6c69 7374 636f 6d70 3eda 00e9  s>.<listcomp>...
+00000af0: 0100 0000 7201 0000 00da 0265 6cfa 0120  ....r......el.. 
+00000b00: 720e 0000 0029 0f72 2400 0000 721b 0000  r....).r$...r...
+00000b10: 0072 0f00 0000 da04 6a6f 696e 7222 0000  .r......joinr"..
+00000b20: 00da 0a69 7369 6e73 7461 6e63 65da 045f  ...isinstance.._
+00000b30: 6173 74da 0249 6672 1800 0000 7206 0000  ast..Ifr....r...
+00000b40: 0072 2300 0000 7234 0000 0072 1600 0000  .r#...r4...r....
+00000b50: 7219 0000 0072 1700 0000 2905 721a 0000  r....r....).r...
+00000b60: 0072 2a00 0000 da0b 736f 7572 6365 5f6c  .r*.....source_l
+00000b70: 6973 74da 0b65 6c69 665f 736f 7572 6365  ist..elif_source
+00000b80: 7237 0000 0072 2000 0000 7238 0000 0072  r7...r ...r8...r
+00000b90: 2100 0000 7206 0000 0052 0000 0073 2400  !...r....R...s$.
+00000ba0: 0000 0601 1201 0801 0a01 1001 1201 02ff  ................
+00000bb0: 0402 02fe 1003 1401 2401 0602 1601 1002  ........$.......
+00000bc0: 0a01 1401 0a01 7a19 4966 536f 7572 6365  ......z.IfSource
+00000bd0: 4d61 7463 6865 722e 4765 7453 6f75 7263  Matcher.GetSourc
+00000be0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+00000bf0: 0000 0200 0000 4300 0000 7334 0000 007c  ......C...s4...|
+00000c00: 006a 006a 0173 0f7c 006a 006a 0264 0119  .j.j.s.|.j.j.d..
+00000c10: 006a 03a0 04a1 0001 0064 0053 007c 006a  .j.......d.S.|.j
+00000c20: 006a 0264 0119 006a 03a0 04a1 0001 0064  .j.d...j.......d
+00000c30: 0053 0029 024e e9ff ffff ff29 0572 1b00  .S.).N.....).r..
+00000c40: 0000 720f 0000 0072 0d00 0000 da07 6d61  ..r....r......ma
+00000c50: 7463 6865 72da 1561 6464 5f6e 6577 6c69  tcher..add_newli
+00000c60: 6e65 5f74 6f5f 736f 7572 6365 7238 0000  ne_to_sourcer8..
+00000c70: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
+00000c80: 7248 0000 0066 0000 0073 0600 0000 0801  rH...f...s......
+00000c90: 1601 1602 7a25 4966 536f 7572 6365 4d61  ....z%IfSourceMa
+00000ca0: 7463 6865 722e 6164 645f 6e65 776c 696e  tcher.add_newlin
+00000cb0: 655f 746f 5f73 6f75 7263 6529 024e 4e29  e_to_source).NN)
+00000cc0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000cd0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000ce0: 616d 655f 5fda 075f 5f64 6f63 5f5f 7211  ame__..__doc__r.
+00000cf0: 0000 0072 2700 0000 7225 0000 0072 2600  ...r'...r%...r&.
+00000d00: 0000 da08 7072 6f70 6572 7479 7224 0000  ....propertyr$..
+00000d10: 0072 0600 0000 7248 0000 00da 0d5f 5f63  .r....rH.....__c
+00000d20: 6c61 7373 6365 6c6c 5f5f 7220 0000 0072  lasscell__r ...r
+00000d30: 2000 0000 721e 0000 0072 2100 0000 720b   ...r....r!...r.
+00000d40: 0000 000d 0000 0073 1400 0000 0800 0401  .......s........
+00000d50: 0e02 080b 080f 0806 021b 0a01 0806 1014  ................
+00000d60: 720b 0000 0029 1372 4200 0000 da21 6675  r....).rB....!fu
+00000d70: 6e5f 7769 7468 5f61 7374 2e73 6f75 7263  n_with_ast.sourc
+00000d80: 655f 6d61 7463 6865 7273 2e62 6f64 7972  e_matchers.bodyr
+00000d90: 0200 0000 da23 6675 6e5f 7769 7468 5f61  .....#fun_with_a
+00000da0: 7374 2e70 6c61 6365 686f 6c64 6572 732e  st.placeholders.
+00000db0: 636f 6d70 6f73 6974 6572 0300 0000 da2a  compositer.....*
+00000dc0: 6675 6e5f 7769 7468 5f61 7374 2e70 6c61  fun_with_ast.pla
+00000dd0: 6365 686f 6c64 6572 732e 6c69 7374 5f70  ceholders.list_p
+00000de0: 6c61 6365 686f 6c64 6572 7204 0000 00da  laceholderr.....
+00000df0: 3266 756e 5f77 6974 685f 6173 742e 6d61  2fun_with_ast.ma
+00000e00: 6e69 7075 6c61 7465 5f6e 6f64 652e 7379  nipulate_node.sy
+00000e10: 6e74 6178 5f66 7265 655f 6c69 6e65 5f6e  ntax_free_line_n
+00000e20: 6f64 6572 0500 0000 da17 6675 6e5f 7769  oder......fun_wi
+00000e30: 7468 5f61 7374 2e67 6574 5f73 6f75 7263  th_ast.get_sourc
+00000e40: 6572 0600 0000 da29 6675 6e5f 7769 7468  er.....)fun_with
+00000e50: 5f61 7374 2e73 6f75 7263 655f 6d61 7463  _ast.source_matc
+00000e60: 6865 7273 2e62 6173 655f 6d61 7463 6865  hers.base_matche
+00000e70: 7272 0700 0000 da24 6675 6e5f 7769 7468  rr.....$fun_with
+00000e80: 5f61 7374 2e70 6c61 6365 686f 6c64 6572  _ast.placeholder
+00000e90: 732e 6261 7365 5f6d 6174 6368 7208 0000  s.base_matchr...
+00000ea0: 0072 0900 0000 da1e 6675 6e5f 7769 7468  .r......fun_with
+00000eb0: 5f61 7374 2e70 6c61 6365 686f 6c64 6572  _ast.placeholder
+00000ec0: 732e 7465 7874 720a 0000 0072 0b00 0000  s.textr....r....
+00000ed0: 7220 0000 0072 2000 0000 7220 0000 0072  r ...r ...r ...r
+00000ee0: 2100 0000 da08 3c6d 6f64 756c 653e 0100  !.....<module>..
+00000ef0: 0000 7314 0000 0008 000c 020c 010c 010c  ..s.............
+00000f00: 010c 010c 0110 010c 0114 03              ...........
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/joined_str.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/joined_str.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 13:41:19 2023 UTC, .py size: 3610 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7f37 7f64 1a0e 0000  o........7.d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 8b0b 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000070: 8400 6407 6505 8303 5a0a 6408 5300 2909  ..d.e...Z.d.S.).
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/matcher_resolver.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/matcher_resolver.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 11 10:19:25 2023 UTC, .py size: 8333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,349 +1,364 @@
-00000000: 6f0d 0d0a 0000 0000 ad9f 8564 8d20 0000  o..........d. ..
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 951f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 001c 0000 0040 0000 0073 f403 0000 6400  .....@...s....d.
+00000020: 001e 0000 0040 0000 0073 1204 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a03 645a 6402 6403 8401 5a04  d.l.Z.dZd.d...Z.
-00000050: 6900 6500 6a05 6404 6405 6702 9301 6500  i.e.j.d.d.g...e.
-00000060: 6a06 6406 6405 6702 9301 6500 6a07 6407  j.d.d.g...e.j.d.
-00000070: 6405 6702 9301 6500 6a08 6408 6405 6702  d.g...e.j.d.d.g.
-00000080: 9301 6500 6a09 6409 6405 6702 9301 6500  ..e.j.d.d.g...e.
-00000090: 6a0a 640a 6405 6702 9301 6500 6a0b 640b  j.d.d.g...e.j.d.
-000000a0: 6405 6702 9301 6500 6a0c 640c 6405 6702  d.g...e.j.d.d.g.
-000000b0: 9301 6500 6a0d 640d 6405 6702 9301 6500  ..e.j.d.d.g...e.
-000000c0: 6a0e 640e 6405 6702 9301 6500 6a0f 640f  j.d.d.g...e.j.d.
-000000d0: 6405 6702 9301 6500 6a10 6410 6405 6702  d.g...e.j.d.d.g.
-000000e0: 9301 6500 6a11 6411 6405 6702 9301 6500  ..e.j.d.d.g...e.
-000000f0: 6a12 6412 6405 6702 9301 6500 6a13 6413  j.d.d.g...e.j.d.
-00000100: 6405 6702 9301 6500 6a14 6414 6405 6702  d.g...e.j.d.d.g.
-00000110: 9301 6500 6a15 6415 6405 6702 9301 6900  ..e.j.d.d.g...i.
-00000120: 6500 6a16 6416 6405 6702 9301 6500 6a17  e.j.d.d.g...e.j.
-00000130: 6417 6405 6702 9301 6500 6a18 6418 6405  d.d.g...e.j.d.d.
-00000140: 6702 9301 6500 6a19 6419 6405 6702 9301  g...e.j.d.d.g...
-00000150: 6500 6a1a 641a 6405 6702 9301 6500 6a1b  e.j.d.d.g...e.j.
-00000160: 641b 6405 6702 9301 6500 6a1c 641c 6405  d.d.g...e.j.d.d.
-00000170: 6702 9301 6500 6a1d 641d 6405 6702 9301  g...e.j.d.d.g...
-00000180: 6500 6a1e 641e 6405 6702 9301 6500 6a1f  e.j.d.d.g...e.j.
-00000190: 641f 6405 6702 9301 6500 6a20 6420 6405  d.d.g...e.j d d.
-000001a0: 6702 9301 6500 6a21 6421 6405 6702 9301  g...e.j!d!d.g...
-000001b0: 6500 6a22 6422 6405 6702 9301 6500 6a23  e.j"d"d.g...e.j#
-000001c0: 6423 6405 6702 9301 6500 6a24 6424 6405  d#d.g...e.j$d$d.
-000001d0: 6702 9301 6500 6a25 6425 6405 6702 9301  g...e.j%d%d.g...
-000001e0: 6500 6a26 6426 6405 6702 9301 a501 6900  e.j&d&d.g.....i.
-000001f0: 6500 6a27 6427 6428 6702 9301 6500 6a28  e.j'd'd(g...e.j(
-00000200: 6429 6405 6702 9301 6500 6a29 642a 6405  d)d.g...e.j)d*d.
-00000210: 6702 9301 6500 6a2a 642b 6405 6702 9301  g...e.j*d+d.g...
-00000220: 6500 6a2b 642c 6405 6702 9301 6500 6a2c  e.j+d,d.g...e.j,
-00000230: 642d 6405 6702 9301 6500 6a2d 642e 6405  d-d.g...e.j-d.d.
-00000240: 6702 9301 6500 6a2e 642f 6405 6702 9301  g...e.j.d/d.g...
-00000250: 6500 6a2f 6430 6405 6702 9301 6500 6a30  e.j/d0d.g...e.j0
-00000260: 6431 6405 6702 9301 6500 6a31 6432 6405  d1d.g...e.j1d2d.
-00000270: 6702 9301 6500 6a32 6433 6405 6702 9301  g...e.j2d3d.g...
-00000280: 6500 6a33 6434 6405 6702 9301 6500 6a34  e.j3d4d.g...e.j4
-00000290: 6435 6405 6702 9301 6500 6a35 6436 6405  d5d.g...e.j5d6d.
-000002a0: 6702 9301 6500 6a36 6437 6405 6702 9301  g...e.j6d7d.g...
-000002b0: 6500 6a37 6438 6405 6702 9301 a501 6900  e.j7d8d.g.....i.
-000002c0: 6500 6a38 6439 6405 6702 9301 6500 6a39  e.j8d9d.g...e.j9
-000002d0: 643a 6405 6702 9301 6500 6a3a 643b 6405  d:d.g...e.j:d;d.
-000002e0: 6702 9301 6500 6a3b 643c 6405 6702 9301  g...e.j;d<d.g...
-000002f0: 6500 6a3c 643d 6405 6702 9301 6500 6a3d  e.j<d=d.g...e.j=
-00000300: 643e 6405 6702 9301 6500 6a3e 643f 6405  d>d.g...e.j>d?d.
-00000310: 6702 9301 6500 6a3f 6440 6405 6702 9301  g...e.j?d@d.g...
-00000320: 6500 6a40 6441 6405 6702 9301 6500 6a41  e.j@dAd.g...e.jA
-00000330: 6442 6405 6702 9301 6500 6a42 6443 6405  dBd.g...e.jBdCd.
-00000340: 6702 9301 6500 6a43 6444 6405 6702 9301  g...e.jCdDd.g...
-00000350: 6500 6a44 6445 6405 6702 9301 6500 6a45  e.jDdEd.g...e.jE
-00000360: 6446 6405 6702 9301 6500 6a46 6447 6405  dFd.g...e.jFdGd.
-00000370: 6702 9301 6500 6a47 6448 6405 6702 9301  g...e.jGdHd.g...
-00000380: 6500 6a48 6449 6405 6702 9301 a501 6503  e.jHdId.g.....e.
-00000390: 6a49 6a4a 6a4b 644a 644b 6702 6503 6a49  jIjJjKdJdKg.e.jI
-000003a0: 6a4a 6a4c 644c 6405 6702 6500 6a4d 644d  jJjLdLd.g.e.jMdM
-000003b0: 6405 6702 6500 6a4e 644e 644f 6702 6500  d.g.e.jNdNdOg.e.
-000003c0: 6a4f 6450 6405 6702 6500 6a50 6451 6405  jOdPd.g.e.jPdQd.
-000003d0: 6702 6500 6a51 6452 6405 6702 6500 6a52  g.e.jQdRd.g.e.jR
-000003e0: 6453 6405 6702 6500 6a53 6454 6405 6702  dSd.g.e.jSdTd.g.
-000003f0: 6500 6a54 6455 6405 6702 6500 6a55 6456  e.jTdUd.g.e.jUdV
-00000400: 6405 6702 6500 6a56 6457 6458 6702 6500  d.g.e.jVdWdXg.e.
-00000410: 6a57 6459 6405 6702 690d a501 5a58 6401  jWdYd.g.i...ZXd.
-00000420: 5300 295b e900 0000 004e 6303 0000 0000  S.)[.....Nc.....
-00000430: 0000 0000 0000 000a 0000 0008 0000 0043  ...............C
-00000440: 0000 0073 7c00 0000 7c01 6401 7500 7206  ...s|...|.d.u.r.
-00000450: 6700 7d01 7400 7c00 6a01 1900 6402 1900  g.}.t.|.j...d...
-00000460: 7d03 7400 7c00 6a01 1900 6403 1900 7d04  }.t.|.j...d...}.
-00000470: 7402 6a03 7c04 1900 7d05 7404 7c05 7c03  t.j.|...}.t.|.|.
-00000480: 8302 7d06 7a0e 7c06 8300 7d07 7c05 6a05  ..}.z.|...}.|.j.
-00000490: 7d08 7c08 7c00 7c07 7c01 7c02 8304 5700  }.|.|.|.|.|...W.
-000004a0: 5300 0400 7406 793d 0100 0100 0100 7c06  S...t.y=......|.
-000004b0: 7c00 7c01 7c02 8303 7d09 7c09 0600 5900  |.|.|...}.|...Y.
-000004c0: 5300 7700 2904 611e 0200 0047 6574 7320  S.w.).a....Gets 
-000004d0: 616e 2069 6e69 7469 616c 697a 6564 206d  an initialized m
-000004e0: 6174 6368 6572 2066 6f72 2074 6865 2067  atcher for the g
-000004f0: 6976 656e 206e 6f64 6520 2864 6f65 736e  iven node (doesn
-00000500: 7420 6361 6c6c 202e 4d61 7463 6829 2e0a  t call .Match)..
-00000510: 0a20 2020 2049 6620 7468 6572 6520 6973  .    If there is
-00000520: 206e 6f20 636f 7272 6573 706f 6e64 696e   no correspondin
-00000530: 6720 6d61 7463 6865 7220 696e 205f 6d61  g matcher in _ma
-00000540: 7463 6865 7273 2c20 7468 6973 2077 696c  tchers, this wil
-00000550: 6c20 7265 7475 726e 2061 0a20 2020 2064  l return a.    d
-00000560: 6566 6175 6c74 206d 6174 6368 6572 2c20  efault matcher, 
-00000570: 7768 6963 6820 7374 6172 7473 2077 6974  which starts wit
-00000580: 6820 6120 706c 6163 6568 6f6c 6465 7220  h a placeholder 
-00000590: 666f 7220 7468 6520 6669 7273 7420 6669  for the first fi
-000005a0: 656c 642c 2065 6e64 730a 2020 2020 7769  eld, ends.    wi
-000005b0: 7468 2061 2070 6c61 6365 686f 6c64 6572  th a placeholder
-000005c0: 2066 6f72 2074 6865 206c 6173 7420 6669   for the last fi
-000005d0: 656c 642c 2061 6e64 2069 6e63 6c75 6465  eld, and include
-000005e0: 7320 5465 7874 506c 6163 6568 6f6c 6465  s TextPlaceholde
-000005f0: 7273 0a20 2020 2077 6974 6820 5b27 2e2a  rs.    with ['.*
-00000600: 2720 7265 6765 7865 7320 6265 7477 6565  ' regexes betwee
-00000610: 6e2e 0a0a 2020 2020 4172 6773 3a0a 2020  n...    Args:.  
-00000620: 2020 2020 6e6f 6465 3a20 5468 6520 6e6f      node: The no
-00000630: 6465 2074 6f20 6765 7420 6120 6d61 7463  de to get a matc
-00000640: 6865 7220 666f 722e 0a20 2020 2020 2073  her for..      s
-00000650: 7461 7274 696e 675f 7061 7265 6e73 3a20  tarting_parens: 
-00000660: 5468 6520 7061 7265 6e73 2074 6865 206d  The parens the m
-00000670: 6174 6368 6572 206d 6179 2073 7461 7274  atcher may start
-00000680: 2077 6974 682e 0a0a 2020 2020 5265 7475   with...    Retu
-00000690: 726e 733a 0a20 2020 2020 2041 206d 6174  rns:.      A mat
-000006a0: 6368 6572 2063 6f72 7265 7370 6f6e 6469  cher correspondi
-000006b0: 6e67 2074 6f20 7468 6174 206e 6f64 652c  ng to that node,
-000006c0: 206f 7220 7468 6520 6465 6661 756c 7420   or the default 
-000006d0: 6d61 7463 6865 7220 2873 6565 2061 626f  matcher (see abo
-000006e0: 7665 292e 0a20 2020 204e 7201 0000 00e9  ve)..    Nr.....
-000006f0: 0100 0000 2907 da11 5f64 796e 616d 6963  ....)..._dynamic
-00000700: 5f6d 6174 6368 6572 73da 095f 5f63 6c61  _matchers..__cla
-00000710: 7373 5f5f da03 7379 73da 076d 6f64 756c  ss__..sys..modul
-00000720: 6573 da07 6765 7461 7474 72da 1444 6566  es..getattr..Def
-00000730: 6175 6c74 536f 7572 6365 4d61 7463 6865  aultSourceMatche
-00000740: 72da 0954 7970 6545 7272 6f72 290a da04  r..TypeError)...
-00000750: 6e6f 6465 da0f 7374 6172 7469 6e67 5f70  node..starting_p
-00000760: 6172 656e 73da 0b70 6172 656e 745f 6e6f  arens..parent_no
-00000770: 6465 da17 7061 7274 735f 6f72 5f6d 6174  de..parts_or_mat
-00000780: 6368 6572 5f73 7472 696e 67da 1770 6172  cher_string..par
-00000790: 7473 5f6f 725f 6d61 7463 6865 725f 6d6f  ts_or_matcher_mo
-000007a0: 6475 6c65 da0e 6375 7272 656e 745f 6d6f  dule..current_mo
-000007b0: 6475 6c65 da10 7061 7274 735f 6f72 5f6d  dule..parts_or_m
-000007c0: 6174 6368 6572 da05 7061 7274 73da 1664  atcher..parts..d
-000007d0: 6566 6175 6c74 5f73 6f75 7263 655f 6d61  efault_source_ma
-000007e0: 7463 6865 72da 076d 6174 6368 6572 a900  tcher..matcher..
-000007f0: 7214 0000 00fa 482f 686f 6d65 2f73 6861  r.....H/home/sha
-00000800: 692f 6675 6e5f 7769 7468 5f61 7374 2f66  i/fun_with_ast/f
-00000810: 756e 5f77 6974 685f 6173 742f 736f 7572  un_with_ast/sour
-00000820: 6365 5f6d 6174 6368 6572 732f 6d61 7463  ce_matchers/matc
-00000830: 6865 725f 7265 736f 6c76 6572 2e70 79da  her_resolver.py.
-00000840: 1147 6574 4479 6e61 6d69 634d 6174 6368  .GetDynamicMatch
-00000850: 6572 0600 0000 731c 0000 0008 0f04 010e  er....s.........
-00000860: 010e 010a 010a 0102 0106 0106 0110 010c  ................
-00000870: 010c 0108 0102 fe72 1600 0000 da16 6765  .......r......ge
-00000880: 745f 4164 645f 6578 7065 6374 6564 5f70  t_Add_expected_p
-00000890: 6172 7473 7a19 6675 6e5f 7769 7468 5f61  artsz.fun_with_a
-000008a0: 7374 2e73 6f75 7263 655f 6d61 7463 68da  st.source_match.
-000008b0: 1867 6574 5f61 6c69 6173 5f65 7870 6563  .get_alias_expec
-000008c0: 7465 645f 7061 7274 73da 1667 6574 5f41  ted_parts..get_A
-000008d0: 6e64 5f65 7870 6563 7465 645f 7061 7274  nd_expected_part
-000008e0: 73da 1967 6574 5f41 7373 6572 745f 6578  s..get_Assert_ex
-000008f0: 7065 6374 6564 5f70 6172 7473 da19 6765  pected_parts..ge
-00000900: 745f 4173 7369 676e 5f65 7870 6563 7465  t_Assign_expecte
-00000910: 645f 7061 7274 73da 1c67 6574 5f41 7474  d_parts..get_Att
-00000920: 7269 6275 7465 5f65 7870 6563 7465 645f  ribute_expected_
-00000930: 7061 7274 73da 1c67 6574 5f41 7567 4173  parts..get_AugAs
-00000940: 7369 676e 5f65 7870 6563 7465 645f 7061  sign_expected_pa
-00000950: 7274 73da 1c67 6574 5f61 7267 756d 656e  rts..get_argumen
-00000960: 7473 5f65 7870 6563 7465 645f 7061 7274  ts_expected_part
-00000970: 73da 1667 6574 5f61 7267 5f65 7870 6563  s..get_arg_expec
-00000980: 7465 645f 7061 7274 73da 1867 6574 5f42  ted_parts..get_B
-00000990: 696e 4f70 5f65 7870 6563 7465 645f 7061  inOp_expected_pa
-000009a0: 7274 73da 1967 6574 5f42 6974 416e 645f  rts..get_BitAnd_
-000009b0: 6578 7065 6374 6564 5f70 6172 7473 da18  expected_parts..
-000009c0: 6765 745f 4269 744f 725f 6578 7065 6374  get_BitOr_expect
-000009d0: 6564 5f70 6172 7473 da19 6765 745f 4269  ed_parts..get_Bi
-000009e0: 7458 6f72 5f65 7870 6563 7465 645f 7061  tXor_expected_pa
-000009f0: 7274 73da 1342 6f6f 6c4f 7053 6f75 7263  rts..BoolOpSourc
-00000a00: 654d 6174 6368 6572 da18 6765 745f 4272  eMatcher..get_Br
-00000a10: 6561 6b5f 6578 7065 6374 6564 5f70 6172  eak_expected_par
-00000a20: 7473 da17 6765 745f 4361 6c6c 5f65 7870  ts..get_Call_exp
-00000a30: 6563 7465 645f 7061 7274 73da 1b67 6574  ected_parts..get
-00000a40: 5f43 6c61 7373 4465 665f 6578 7065 6374  _ClassDef_expect
-00000a50: 6564 5f70 6172 7473 da1a 6765 745f 436f  ed_parts..get_Co
-00000a60: 6d70 6172 655f 6578 7065 6374 6564 5f70  mpare_expected_p
-00000a70: 6172 7473 da20 6765 745f 636f 6d70 7265  arts. get_compre
-00000a80: 6865 6e73 696f 6e5f 6578 7065 6374 6564  hension_expected
-00000a90: 5f70 6172 7473 da1b 6765 745f 436f 6e74  _parts..get_Cont
-00000aa0: 696e 7565 5f65 7870 6563 7465 645f 7061  inue_expected_pa
-00000ab0: 7274 73da 1967 6574 5f44 656c 6574 655f  rts..get_Delete_
-00000ac0: 6578 7065 6374 6564 5f70 6172 7473 da17  expected_parts..
-00000ad0: 6765 745f 4469 6374 5f65 7870 6563 7465  get_Dict_expecte
-00000ae0: 645f 7061 7274 73da 1b67 6574 5f44 6963  d_parts..get_Dic
-00000af0: 7443 6f6d 705f 6578 7065 6374 6564 5f70  tComp_expected_p
-00000b00: 6172 7473 da16 6765 745f 4469 765f 6578  arts..get_Div_ex
-00000b10: 7065 6374 6564 5f70 6172 7473 da15 6765  pected_parts..ge
-00000b20: 745f 4571 5f65 7870 6563 7465 645f 7061  t_Eq_expected_pa
-00000b30: 7274 73da 1767 6574 5f45 7870 725f 6578  rts..get_Expr_ex
-00000b40: 7065 6374 6564 5f70 6172 7473 da20 6765  pected_parts. ge
-00000b50: 745f 4578 6365 7074 4861 6e64 6c65 725f  t_ExceptHandler_
-00000b60: 6578 7065 6374 6564 5f70 6172 7473 da1b  expected_parts..
-00000b70: 6765 745f 466c 6f6f 7244 6976 5f65 7870  get_FloorDiv_exp
-00000b80: 6563 7465 645f 7061 7274 73da 1667 6574  ected_parts..get
-00000b90: 5f46 6f72 5f65 7870 6563 7465 645f 7061  _For_expected_pa
-00000ba0: 7274 73da 1e67 6574 5f46 756e 6374 696f  rts..get_Functio
-00000bb0: 6e44 6566 5f65 7870 6563 7465 645f 7061  nDef_expected_pa
-00000bc0: 7274 73da 1f67 6574 5f47 656e 6572 6174  rts..get_Generat
-00000bd0: 6f72 4578 705f 6578 7065 6374 6564 5f70  orExp_expected_p
-00000be0: 6172 7473 da19 6765 745f 476c 6f62 616c  arts..get_Global
-00000bf0: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
-00000c00: 1567 6574 5f47 745f 6578 7065 6374 6564  .get_Gt_expected
-00000c10: 5f70 6172 7473 da16 6765 745f 4774 455f  _parts..get_GtE_
-00000c20: 6578 7065 6374 6564 5f70 6172 7473 da0f  expected_parts..
-00000c30: 4966 536f 7572 6365 4d61 7463 6865 727a  IfSourceMatcherz
-00000c40: 2c66 756e 5f77 6974 685f 6173 742e 736f  ,fun_with_ast.so
-00000c50: 7572 6365 5f6d 6174 6368 6572 732e 6966  urce_matchers.if
-00000c60: 5f73 6f75 7263 655f 6d61 7463 68da 1867  _source_match..g
-00000c70: 6574 5f49 6645 7870 5f65 7870 6563 7465  et_IfExp_expecte
-00000c80: 645f 7061 7274 73da 1967 6574 5f49 6d70  d_parts..get_Imp
-00000c90: 6f72 745f 6578 7065 6374 6564 5f70 6172  ort_expected_par
-00000ca0: 7473 da1d 6765 745f 496d 706f 7274 4672  ts..get_ImportFr
-00000cb0: 6f6d 5f65 7870 6563 7465 645f 7061 7274  om_expected_part
-00000cc0: 73da 1567 6574 5f49 6e5f 6578 7065 6374  s..get_In_expect
-00000cd0: 6564 5f70 6172 7473 da19 6765 745f 496e  ed_parts..get_In
-00000ce0: 7665 7274 5f65 7870 6563 7465 645f 7061  vert_expected_pa
-00000cf0: 7274 73da 1567 6574 5f49 735f 6578 7065  rts..get_Is_expe
-00000d00: 6374 6564 5f70 6172 7473 da18 6765 745f  cted_parts..get_
-00000d10: 4973 4e6f 745f 6578 7065 6374 6564 5f70  IsNot_expected_p
-00000d20: 6172 7473 da1a 6765 745f 6b65 7977 6f72  arts..get_keywor
-00000d30: 645f 6578 7065 6374 6564 5f70 6172 7473  d_expected_parts
-00000d40: da19 6765 745f 4c61 6d62 6461 5f65 7870  ..get_Lambda_exp
-00000d50: 6563 7465 645f 7061 7274 73da 1767 6574  ected_parts..get
-00000d60: 5f4c 6973 745f 6578 7065 6374 6564 5f70  _List_expected_p
-00000d70: 6172 7473 da1b 6765 745f 4c69 7374 436f  arts..get_ListCo
-00000d80: 6d70 5f65 7870 6563 7465 645f 7061 7274  mp_expected_part
-00000d90: 73da 1967 6574 5f4c 5368 6966 745f 6578  s..get_LShift_ex
-00000da0: 7065 6374 6564 5f70 6172 7473 da15 6765  pected_parts..ge
-00000db0: 745f 4c74 5f65 7870 6563 7465 645f 7061  t_Lt_expected_pa
-00000dc0: 7274 73da 1667 6574 5f4c 7445 5f65 7870  rts..get_LtE_exp
-00000dd0: 6563 7465 645f 7061 7274 73da 1667 6574  ected_parts..get
-00000de0: 5f4d 6f64 5f65 7870 6563 7465 645f 7061  _Mod_expected_pa
-00000df0: 7274 73da 1967 6574 5f4d 6f64 756c 655f  rts..get_Module_
-00000e00: 6578 7065 6374 6564 5f70 6172 7473 da17  expected_parts..
-00000e10: 6765 745f 4d75 6c74 5f65 7870 6563 7465  get_Mult_expecte
-00000e20: 645f 7061 7274 73da 1767 6574 5f4e 616d  d_parts..get_Nam
-00000e30: 655f 6578 7065 6374 6564 5f70 6172 7473  e_expected_parts
-00000e40: da16 6765 745f 4e6f 745f 6578 7065 6374  ..get_Not_expect
-00000e50: 6564 5f70 6172 7473 da18 6765 745f 4e6f  ed_parts..get_No
-00000e60: 7449 6e5f 6578 7065 6374 6564 5f70 6172  tIn_expected_par
-00000e70: 7473 da18 6765 745f 4e6f 7445 715f 6578  ts..get_NotEq_ex
-00000e80: 7065 6374 6564 5f70 6172 7473 da15 6765  pected_parts..ge
-00000e90: 745f 4f72 5f65 7870 6563 7465 645f 7061  t_Or_expected_pa
-00000ea0: 7274 73da 1767 6574 5f50 6173 735f 6578  rts..get_Pass_ex
-00000eb0: 7065 6374 6564 5f70 6172 7473 da16 6765  pected_parts..ge
-00000ec0: 745f 506f 775f 6578 7065 6374 6564 5f70  t_Pow_expected_p
-00000ed0: 6172 7473 da18 6765 745f 5261 6973 655f  arts..get_Raise_
-00000ee0: 6578 7065 6374 6564 5f70 6172 7473 da19  expected_parts..
-00000ef0: 6765 745f 5265 7475 726e 5f65 7870 6563  get_Return_expec
-00000f00: 7465 645f 7061 7274 73da 1967 6574 5f52  ted_parts..get_R
-00000f10: 5368 6966 745f 6578 7065 6374 6564 5f70  Shift_expected_p
-00000f20: 6172 7473 da18 6765 745f 536c 6963 655f  arts..get_Slice_
-00000f30: 6578 7065 6374 6564 5f70 6172 7473 da16  expected_parts..
-00000f40: 6765 745f 5375 625f 6578 7065 6374 6564  get_Sub_expected
-00000f50: 5f70 6172 7473 da16 6765 745f 5365 745f  _parts..get_Set_
-00000f60: 6578 7065 6374 6564 5f70 6172 7473 da1a  expected_parts..
-00000f70: 6765 745f 5365 7443 6f6d 705f 6578 7065  get_SetComp_expe
-00000f80: 6374 6564 5f70 6172 7473 da1c 6765 745f  cted_parts..get_
-00000f90: 5375 6273 6372 6970 745f 6578 7065 6374  Subscript_expect
-00000fa0: 6564 5f70 6172 7473 da15 436f 6e73 7461  ed_parts..Consta
-00000fb0: 6e74 536f 7572 6365 4d61 7463 6865 72da  ntSourceMatcher.
-00000fc0: 1553 796e 7461 7846 7265 654c 696e 654d  .SyntaxFreeLineM
-00000fd0: 6174 6368 6572 7a2b 6675 6e5f 7769 7468  atcherz+fun_with
-00000fe0: 5f61 7374 2e73 6f75 7263 655f 6d61 7463  _ast.source_matc
-00000ff0: 6865 7273 2e73 796e 7461 7866 7265 656c  hers.syntaxfreel
-00001000: 696e 65da 1a67 6574 5f43 6f6d 6d65 6e74  ine..get_Comment
-00001010: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
-00001020: 1867 6574 5f54 7570 6c65 5f65 7870 6563  .get_Tuple_expec
-00001030: 7465 645f 7061 7274 73da 164a 6f69 6e65  ted_parts..Joine
-00001040: 6453 7472 536f 7572 6365 4d61 7463 6865  dStrSourceMatche
-00001050: 727a 2766 756e 5f77 6974 685f 6173 742e  rz'fun_with_ast.
-00001060: 736f 7572 6365 5f6d 6174 6368 6572 732e  source_matchers.
-00001070: 6a6f 696e 6564 5f73 7472 da1c 6765 745f  joined_str..get_
-00001080: 5472 7945 7863 6570 745f 6578 7065 6374  TryExcept_expect
-00001090: 6564 5f70 6172 7473 da21 6765 745f 466f  ed_parts.!get_Fo
-000010a0: 726d 6174 7465 6456 616c 7565 5f65 7870  rmattedValue_exp
-000010b0: 6563 7465 645f 7061 7274 73da 1767 6574  ected_parts..get
-000010c0: 5f55 4164 645f 6578 7065 6374 6564 5f70  _UAdd_expected_p
-000010d0: 6172 7473 da1a 6765 745f 556e 6172 794f  arts..get_UnaryO
-000010e0: 705f 6578 7065 6374 6564 5f70 6172 7473  p_expected_parts
-000010f0: da17 6765 745f 5553 7562 5f65 7870 6563  ..get_USub_expec
-00001100: 7465 645f 7061 7274 73da 1867 6574 5f57  ted_parts..get_W
-00001110: 6869 6c65 5f65 7870 6563 7465 645f 7061  hile_expected_pa
-00001120: 7274 73da 1157 6974 6853 6f75 7263 654d  rts..WithSourceM
-00001130: 6174 6368 6572 da15 5769 7468 4974 656d  atcher..WithItem
-00001140: 536f 7572 6365 4d61 7463 6865 727a 2566  SourceMatcherz%f
-00001150: 756e 5f77 6974 685f 6173 742e 736f 7572  un_with_ast.sour
-00001160: 6365 5f6d 6174 6368 6572 732e 7769 7468  ce_matchers.with
-00001170: 6974 656d da18 6765 745f 5969 656c 645f  item..get_Yield_
-00001180: 6578 7065 6374 6564 5f70 6172 7473 2902  expected_parts).
-00001190: 4e4e 2959 da04 5f61 7374 7205 0000 00da  NN)Y.._astr.....
-000011a0: 2866 756e 5f77 6974 685f 6173 742e 6d61  (fun_with_ast.ma
-000011b0: 6e69 7075 6c61 7465 5f6e 6f64 652e 6372  nipulate_node.cr
-000011c0: 6561 7465 5f6e 6f64 65da 0c66 756e 5f77  eate_node..fun_w
-000011d0: 6974 685f 6173 7472 1600 0000 da03 4164  ith_astr......Ad
-000011e0: 64da 0561 6c69 6173 da03 416e 64da 0641  d..alias..And..A
-000011f0: 7373 6572 74da 0641 7373 6967 6eda 0941  ssert..Assign..A
-00001200: 7474 7269 6275 7465 da09 4175 6741 7373  ttribute..AugAss
-00001210: 6967 6eda 0961 7267 756d 656e 7473 da03  ign..arguments..
-00001220: 6172 67da 0542 696e 4f70 da06 4269 7441  arg..BinOp..BitA
-00001230: 6e64 da05 4269 744f 72da 0642 6974 586f  nd..BitOr..BitXo
-00001240: 72da 0642 6f6f 6c4f 70da 0542 7265 616b  r..BoolOp..Break
-00001250: da04 4361 6c6c da08 436c 6173 7344 6566  ..Call..ClassDef
-00001260: da07 436f 6d70 6172 65da 0d63 6f6d 7072  ..Compare..compr
-00001270: 6568 656e 7369 6f6e da08 436f 6e74 696e  ehension..Contin
-00001280: 7565 da06 4465 6c65 7465 da04 4469 6374  ue..Delete..Dict
-00001290: da08 4469 6374 436f 6d70 da03 4469 76da  ..DictComp..Div.
-000012a0: 0245 71da 0445 7870 72da 0d45 7863 6570  .Eq..Expr..Excep
-000012b0: 7448 616e 646c 6572 da08 466c 6f6f 7244  tHandler..FloorD
-000012c0: 6976 da03 466f 72da 0b46 756e 6374 696f  iv..For..Functio
-000012d0: 6e44 6566 da0c 4765 6e65 7261 746f 7245  nDef..GeneratorE
-000012e0: 7870 da06 476c 6f62 616c da02 4774 da03  xp..Global..Gt..
-000012f0: 4774 45da 0249 66da 0549 6645 7870 da06  GtE..If..IfExp..
-00001300: 496d 706f 7274 da0a 496d 706f 7274 4672  Import..ImportFr
-00001310: 6f6d da02 496e da06 496e 7665 7274 da02  om..In..Invert..
-00001320: 4973 da05 4973 4e6f 74da 076b 6579 776f  Is..IsNot..keywo
-00001330: 7264 da06 4c61 6d62 6461 da04 4c69 7374  rd..Lambda..List
-00001340: da08 4c69 7374 436f 6d70 da06 4c53 6869  ..ListComp..LShi
-00001350: 6674 da02 4c74 da03 4c74 45da 034d 6f64  ft..Lt..LtE..Mod
-00001360: da06 4d6f 6475 6c65 da04 4d75 6c74 da04  ..Module..Mult..
-00001370: 4e61 6d65 da03 4e6f 74da 054e 6f74 496e  Name..Not..NotIn
-00001380: da05 4e6f 7445 71da 024f 72da 0450 6173  ..NotEq..Or..Pas
-00001390: 73da 0350 6f77 da05 5261 6973 65da 0652  s..Pow..Raise..R
-000013a0: 6574 7572 6eda 0652 5368 6966 74da 0553  eturn..RShift..S
-000013b0: 6c69 6365 da03 5375 62da 0353 6574 da07  lice..Sub..Set..
-000013c0: 5365 7443 6f6d 70da 0953 7562 7363 7269  SetComp..Subscri
-000013d0: 7074 da08 436f 6e73 7461 6e74 da0f 6d61  pt..Constant..ma
-000013e0: 6e69 7075 6c61 7465 5f6e 6f64 65da 0b63  nipulate_node..c
-000013f0: 7265 6174 655f 6e6f 6465 da0e 5379 6e74  reate_node..Synt
-00001400: 6178 4672 6565 4c69 6e65 da07 436f 6d6d  axFreeLine..Comm
-00001410: 656e 74da 0554 7570 6c65 da09 4a6f 696e  ent..Tuple..Join
-00001420: 6564 5374 72da 0354 7279 da0e 466f 726d  edStr..Try..Form
-00001430: 6174 7465 6456 616c 7565 da04 5541 6464  attedValue..UAdd
-00001440: da07 556e 6172 794f 70da 0455 5375 62da  ..UnaryOp..USub.
-00001450: 0557 6869 6c65 da04 5769 7468 da08 7769  .While..With..wi
-00001460: 7468 6974 656d da05 5969 656c 6472 0300  thitem..Yieldr..
-00001470: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00001480: 0072 1500 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001490: 0100 0000 7336 0100 0008 0108 0108 020a  ....s6..........
-000014a0: 0102 1d0a 0102 ff0a 0202 fe0a 0302 fd0a  ................
-000014b0: 0402 fc0a 0502 fb0a 0602 fa0a 0702 f90a  ................
-000014c0: 0802 f80a 0902 f70a 0a02 f60a 0b02 f50a  ................
-000014d0: 0c02 f40a 0d02 f30a 0f02 f10a 1002 f00a  ................
-000014e0: 1102 ef0a 1204 ee0a 1302 ed0a 1402 ec0a  ................
-000014f0: 1502 eb0a 1602 ea0a 1702 e90a 1802 e80a  ................
-00001500: 1902 e70a 1a02 e60a 1b02 e50a 1c02 e40a  ................
-00001510: 1d02 e30a 1e02 e20a 1f02 e10a 2002 e00a  ............ ...
-00001520: 2102 df0a 2202 de0a 2306 dd0a 2402 dc0a  !..."...#...$...
-00001530: 2502 db0a 2602 da0a 2702 d90a 2802 d80a  %...&...'...(...
-00001540: 2a02 d60a 2b02 d50a 2c02 d40a 2d02 d30a  *...+...,...-...
-00001550: 2e02 d20a 2f02 d10a 3002 d00a 3102 cf0a  ..../...0...1...
-00001560: 3202 ce0a 3302 cd0a 3402 cc0a 3506 cb0a  2...3...4...5...
-00001570: 3602 ca0a 3702 c90a 3802 c80a 3902 c70a  6...7...8...9...
-00001580: 3a02 c60a 3c02 c40a 3d02 c30a 3e02 c20a  :...<...=...>...
-00001590: 4002 c00a 4102 bf0a 4202 be0a 4302 bd0a  @...A...B...C...
-000015a0: 4402 bc0a 4502 bb0a 4602 ba0a 4702 b90a  D...E...F...G...
-000015b0: 4904 b70e 4a0e 020a 010a 030a 010a 010a  I...J...........
-000015c0: 010a 010a 010a 010a 010a 010a 010a a7    ...............
+00000040: 6401 6c02 5a03 6400 6401 6c04 5a03 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6401 6c05 5a03 645b 6402 6403 8401 5a06  d.l.Z.d[d.d...Z.
+00000060: 6900 6500 6a07 6404 6405 6702 9301 6500  i.e.j.d.d.g...e.
+00000070: 6a08 6406 6405 6702 9301 6500 6a09 6407  j.d.d.g...e.j.d.
+00000080: 6405 6702 9301 6500 6a0a 6408 6405 6702  d.g...e.j.d.d.g.
+00000090: 9301 6500 6a0b 6409 6405 6702 9301 6500  ..e.j.d.d.g...e.
+000000a0: 6a0c 640a 6405 6702 9301 6500 6a0d 640b  j.d.d.g...e.j.d.
+000000b0: 6405 6702 9301 6500 6a0e 640c 6405 6702  d.g...e.j.d.d.g.
+000000c0: 9301 6500 6a0f 640d 6405 6702 9301 6500  ..e.j.d.d.g...e.
+000000d0: 6a10 640e 6405 6702 9301 6500 6a11 640f  j.d.d.g...e.j.d.
+000000e0: 6405 6702 9301 6500 6a12 6410 6405 6702  d.g...e.j.d.d.g.
+000000f0: 9301 6500 6a13 6411 6405 6702 9301 6500  ..e.j.d.d.g...e.
+00000100: 6a14 6412 6405 6702 9301 6500 6a15 6413  j.d.d.g...e.j.d.
+00000110: 6405 6702 9301 6500 6a16 6414 6405 6702  d.g...e.j.d.d.g.
+00000120: 9301 6500 6a17 6415 6405 6702 9301 6900  ..e.j.d.d.g...i.
+00000130: 6500 6a18 6416 6405 6702 9301 6500 6a19  e.j.d.d.g...e.j.
+00000140: 6417 6405 6702 9301 6500 6a1a 6418 6405  d.d.g...e.j.d.d.
+00000150: 6702 9301 6500 6a1b 6419 6405 6702 9301  g...e.j.d.d.g...
+00000160: 6500 6a1c 641a 6405 6702 9301 6500 6a1d  e.j.d.d.g...e.j.
+00000170: 641b 6405 6702 9301 6500 6a1e 641c 6405  d.d.g...e.j.d.d.
+00000180: 6702 9301 6500 6a1f 641d 6405 6702 9301  g...e.j.d.d.g...
+00000190: 6500 6a20 641e 6405 6702 9301 6500 6a21  e.j d.d.g...e.j!
+000001a0: 641f 6405 6702 9301 6500 6a22 6420 6405  d.d.g...e.j"d d.
+000001b0: 6702 9301 6500 6a23 6421 6405 6702 9301  g...e.j#d!d.g...
+000001c0: 6500 6a24 6422 6405 6702 9301 6500 6a25  e.j$d"d.g...e.j%
+000001d0: 6423 6405 6702 9301 6500 6a26 6424 6405  d#d.g...e.j&d$d.
+000001e0: 6702 9301 6500 6a27 6425 6405 6702 9301  g...e.j'd%d.g...
+000001f0: 6500 6a28 6426 6405 6702 9301 a501 6900  e.j(d&d.g.....i.
+00000200: 6500 6a29 6427 6428 6702 9301 6500 6a2a  e.j)d'd(g...e.j*
+00000210: 6429 6405 6702 9301 6500 6a2b 642a 6405  d)d.g...e.j+d*d.
+00000220: 6702 9301 6500 6a2c 642b 6405 6702 9301  g...e.j,d+d.g...
+00000230: 6500 6a2d 642c 6405 6702 9301 6500 6a2e  e.j-d,d.g...e.j.
+00000240: 642d 6405 6702 9301 6500 6a2f 642e 6405  d-d.g...e.j/d.d.
+00000250: 6702 9301 6500 6a30 642f 6405 6702 9301  g...e.j0d/d.g...
+00000260: 6500 6a31 6430 6405 6702 9301 6500 6a32  e.j1d0d.g...e.j2
+00000270: 6431 6405 6702 9301 6500 6a33 6432 6405  d1d.g...e.j3d2d.
+00000280: 6702 9301 6500 6a34 6433 6405 6702 9301  g...e.j4d3d.g...
+00000290: 6500 6a35 6434 6405 6702 9301 6500 6a36  e.j5d4d.g...e.j6
+000002a0: 6435 6405 6702 9301 6500 6a37 6436 6405  d5d.g...e.j7d6d.
+000002b0: 6702 9301 6500 6a38 6437 6405 6702 9301  g...e.j8d7d.g...
+000002c0: 6500 6a39 6438 6405 6702 9301 a501 6900  e.j9d8d.g.....i.
+000002d0: 6500 6a3a 6439 6405 6702 9301 6500 6a3b  e.j:d9d.g...e.j;
+000002e0: 643a 6405 6702 9301 6500 6a3c 643b 6405  d:d.g...e.j<d;d.
+000002f0: 6702 9301 6500 6a3d 643c 6405 6702 9301  g...e.j=d<d.g...
+00000300: 6500 6a3e 643d 6405 6702 9301 6500 6a3f  e.j>d=d.g...e.j?
+00000310: 643e 6405 6702 9301 6500 6a40 643f 6405  d>d.g...e.j@d?d.
+00000320: 6702 9301 6500 6a41 6440 6405 6702 9301  g...e.jAd@d.g...
+00000330: 6500 6a42 6441 6405 6702 9301 6500 6a43  e.jBdAd.g...e.jC
+00000340: 6442 6405 6702 9301 6500 6a44 6443 6405  dBd.g...e.jDdCd.
+00000350: 6702 9301 6500 6a45 6444 6405 6702 9301  g...e.jEdDd.g...
+00000360: 6500 6a46 6445 6405 6702 9301 6500 6a47  e.jFdEd.g...e.jG
+00000370: 6446 6405 6702 9301 6500 6a48 6447 6405  dFd.g...e.jHdGd.
+00000380: 6702 9301 6500 6a49 6448 6405 6702 9301  g...e.jIdHd.g...
+00000390: 6500 6a4a 6449 6405 6702 9301 a501 6500  e.jJdId.g.....e.
+000003a0: 6a4b 644a 6405 6702 6500 6a4c 644b 644c  jKdJd.g.e.jLdKdL
+000003b0: 6702 6500 6a4d 644d 6405 6702 6500 6a4e  g.e.jMdMd.g.e.jN
+000003c0: 644e 6405 6702 6500 6a4f 644f 6405 6702  dNd.g.e.jOdOd.g.
+000003d0: 6500 6a50 6450 6405 6702 6500 6a51 6451  e.jPdPd.g.e.jQdQ
+000003e0: 6405 6702 6500 6a52 6452 6405 6702 6500  d.g.e.jRdRd.g.e.
+000003f0: 6a53 6453 6405 6702 6500 6a54 6454 6455  jSdSd.g.e.jTdTdU
+00000400: 6702 6500 6a55 6456 6405 6702 6503 6a56  g.e.jUdVd.g.e.jV
+00000410: 6a57 6a58 6457 6458 6702 6503 6a56 6a59  jWjXdWdXg.e.jVjY
+00000420: 6a5a 6459 6405 6702 6503 6a56 6a5b 6a5c  jZdYd.g.e.jVj[j\
+00000430: 645a 6405 6702 690e a501 5a5d 6401 5300  dZd.g.i...Z]d.S.
+00000440: 295c e900 0000 004e 6304 0000 0000 0000  )\.....Nc.......
+00000450: 0000 0000 000b 0000 0008 0000 0043 0000  .............C..
+00000460: 0073 8600 0000 7c01 6401 7500 7206 6700  .s....|.d.u.r.g.
+00000470: 7d01 7400 7c00 6a01 1900 6402 1900 7d04  }.t.|.j...d...}.
+00000480: 7400 7c00 6a01 1900 6403 1900 7d05 7402  t.|.j...d...}.t.
+00000490: 6a03 7c05 1900 7d06 7404 7c06 7c04 8302  j.|...}.t.|.|...
+000004a0: 7d07 7a13 7c03 7325 7c07 8300 7d08 6e02  }.z.|.s%|...}.n.
+000004b0: 7c03 7d08 7c06 6a05 7d09 7c09 7c00 7c08  |.}.|.j.}.|.|.|.
+000004c0: 7c01 7c02 8304 5700 5300 0400 7406 7942  |.|...W.S...t.yB
+000004d0: 0100 0100 0100 7c07 7c00 7c01 7c02 8303  ......|.|.|.|...
+000004e0: 7d0a 7c0a 0600 5900 5300 7700 2904 611e  }.|...Y.S.w.).a.
+000004f0: 0200 0047 6574 7320 616e 2069 6e69 7469  ...Gets an initi
+00000500: 616c 697a 6564 206d 6174 6368 6572 2066  alized matcher f
+00000510: 6f72 2074 6865 2067 6976 656e 206e 6f64  or the given nod
+00000520: 6520 2864 6f65 736e 7420 6361 6c6c 202e  e (doesnt call .
+00000530: 4d61 7463 6829 2e0a 0a20 2020 2049 6620  Match)...    If 
+00000540: 7468 6572 6520 6973 206e 6f20 636f 7272  there is no corr
+00000550: 6573 706f 6e64 696e 6720 6d61 7463 6865  esponding matche
+00000560: 7220 696e 205f 6d61 7463 6865 7273 2c20  r in _matchers, 
+00000570: 7468 6973 2077 696c 6c20 7265 7475 726e  this will return
+00000580: 2061 0a20 2020 2064 6566 6175 6c74 206d   a.    default m
+00000590: 6174 6368 6572 2c20 7768 6963 6820 7374  atcher, which st
+000005a0: 6172 7473 2077 6974 6820 6120 706c 6163  arts with a plac
+000005b0: 6568 6f6c 6465 7220 666f 7220 7468 6520  eholder for the 
+000005c0: 6669 7273 7420 6669 656c 642c 2065 6e64  first field, end
+000005d0: 730a 2020 2020 7769 7468 2061 2070 6c61  s.    with a pla
+000005e0: 6365 686f 6c64 6572 2066 6f72 2074 6865  ceholder for the
+000005f0: 206c 6173 7420 6669 656c 642c 2061 6e64   last field, and
+00000600: 2069 6e63 6c75 6465 7320 5465 7874 506c   includes TextPl
+00000610: 6163 6568 6f6c 6465 7273 0a20 2020 2077  aceholders.    w
+00000620: 6974 6820 5b27 2e2a 2720 7265 6765 7865  ith ['.*' regexe
+00000630: 7320 6265 7477 6565 6e2e 0a0a 2020 2020  s between...    
+00000640: 4172 6773 3a0a 2020 2020 2020 6e6f 6465  Args:.      node
+00000650: 3a20 5468 6520 6e6f 6465 2074 6f20 6765  : The node to ge
+00000660: 7420 6120 6d61 7463 6865 7220 666f 722e  t a matcher for.
+00000670: 0a20 2020 2020 2073 7461 7274 696e 675f  .      starting_
+00000680: 7061 7265 6e73 3a20 5468 6520 7061 7265  parens: The pare
+00000690: 6e73 2074 6865 206d 6174 6368 6572 206d  ns the matcher m
+000006a0: 6179 2073 7461 7274 2077 6974 682e 0a0a  ay start with...
+000006b0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000006c0: 2020 2041 206d 6174 6368 6572 2063 6f72     A matcher cor
+000006d0: 7265 7370 6f6e 6469 6e67 2074 6f20 7468  responding to th
+000006e0: 6174 206e 6f64 652c 206f 7220 7468 6520  at node, or the 
+000006f0: 6465 6661 756c 7420 6d61 7463 6865 7220  default matcher 
+00000700: 2873 6565 2061 626f 7665 292e 0a20 2020  (see above)..   
+00000710: 204e 7201 0000 00e9 0100 0000 2907 da11   Nr.........)...
+00000720: 5f64 796e 616d 6963 5f6d 6174 6368 6572  _dynamic_matcher
+00000730: 73da 095f 5f63 6c61 7373 5f5f da03 7379  s..__class__..sy
+00000740: 73da 076d 6f64 756c 6573 da07 6765 7461  s..modules..geta
+00000750: 7474 72da 1444 6566 6175 6c74 536f 7572  ttr..DefaultSour
+00000760: 6365 4d61 7463 6865 72da 0954 7970 6545  ceMatcher..TypeE
+00000770: 7272 6f72 290b da04 6e6f 6465 da0f 7374  rror)...node..st
+00000780: 6172 7469 6e67 5f70 6172 656e 73da 0b70  arting_parens..p
+00000790: 6172 656e 745f 6e6f 6465 da08 7061 7274  arent_node..part
+000007a0: 735f 696e da17 7061 7274 735f 6f72 5f6d  s_in..parts_or_m
+000007b0: 6174 6368 6572 5f73 7472 696e 67da 1770  atcher_string..p
+000007c0: 6172 7473 5f6f 725f 6d61 7463 6865 725f  arts_or_matcher_
+000007d0: 6d6f 6475 6c65 da0e 6375 7272 656e 745f  module..current_
+000007e0: 6d6f 6475 6c65 da10 7061 7274 735f 6f72  module..parts_or
+000007f0: 5f6d 6174 6368 6572 da05 7061 7274 73da  _matcher..parts.
+00000800: 1664 6566 6175 6c74 5f73 6f75 7263 655f  .default_source_
+00000810: 6d61 7463 6865 72da 076d 6174 6368 6572  matcher..matcher
+00000820: a900 7215 0000 00fa 482f 686f 6d65 2f73  ..r.....H/home/s
+00000830: 6861 692f 6675 6e5f 7769 7468 5f61 7374  hai/fun_with_ast
+00000840: 2f66 756e 5f77 6974 685f 6173 742f 736f  /fun_with_ast/so
+00000850: 7572 6365 5f6d 6174 6368 6572 732f 6d61  urce_matchers/ma
+00000860: 7463 6865 725f 7265 736f 6c76 6572 2e70  tcher_resolver.p
+00000870: 79da 1147 6574 4479 6e61 6d69 634d 6174  y..GetDynamicMat
+00000880: 6368 6572 0a00 0000 7320 0000 0008 0f04  cher....s ......
+00000890: 010e 010e 010a 010a 0102 0104 0108 0104  ................
+000008a0: 0206 0110 010c 010c 0108 0102 fe72 1700  .............r..
+000008b0: 0000 da16 6765 745f 4164 645f 6578 7065  ....get_Add_expe
+000008c0: 6374 6564 5f70 6172 7473 7a19 6675 6e5f  cted_partsz.fun_
+000008d0: 7769 7468 5f61 7374 2e73 6f75 7263 655f  with_ast.source_
+000008e0: 6d61 7463 68da 1867 6574 5f61 6c69 6173  match..get_alias
+000008f0: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
+00000900: 1667 6574 5f41 6e64 5f65 7870 6563 7465  .get_And_expecte
+00000910: 645f 7061 7274 73da 1967 6574 5f41 7373  d_parts..get_Ass
+00000920: 6572 745f 6578 7065 6374 6564 5f70 6172  ert_expected_par
+00000930: 7473 da19 6765 745f 4173 7369 676e 5f65  ts..get_Assign_e
+00000940: 7870 6563 7465 645f 7061 7274 73da 1c67  xpected_parts..g
+00000950: 6574 5f41 7474 7269 6275 7465 5f65 7870  et_Attribute_exp
+00000960: 6563 7465 645f 7061 7274 73da 1c67 6574  ected_parts..get
+00000970: 5f41 7567 4173 7369 676e 5f65 7870 6563  _AugAssign_expec
+00000980: 7465 645f 7061 7274 73da 1c67 6574 5f61  ted_parts..get_a
+00000990: 7267 756d 656e 7473 5f65 7870 6563 7465  rguments_expecte
+000009a0: 645f 7061 7274 73da 1667 6574 5f61 7267  d_parts..get_arg
+000009b0: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
+000009c0: 1867 6574 5f42 696e 4f70 5f65 7870 6563  .get_BinOp_expec
+000009d0: 7465 645f 7061 7274 73da 1967 6574 5f42  ted_parts..get_B
+000009e0: 6974 416e 645f 6578 7065 6374 6564 5f70  itAnd_expected_p
+000009f0: 6172 7473 da18 6765 745f 4269 744f 725f  arts..get_BitOr_
+00000a00: 6578 7065 6374 6564 5f70 6172 7473 da19  expected_parts..
+00000a10: 6765 745f 4269 7458 6f72 5f65 7870 6563  get_BitXor_expec
+00000a20: 7465 645f 7061 7274 73da 1342 6f6f 6c4f  ted_parts..BoolO
+00000a30: 7053 6f75 7263 654d 6174 6368 6572 da18  pSourceMatcher..
+00000a40: 6765 745f 4272 6561 6b5f 6578 7065 6374  get_Break_expect
+00000a50: 6564 5f70 6172 7473 da17 6765 745f 4361  ed_parts..get_Ca
+00000a60: 6c6c 5f65 7870 6563 7465 645f 7061 7274  ll_expected_part
+00000a70: 73da 1b67 6574 5f43 6c61 7373 4465 665f  s..get_ClassDef_
+00000a80: 6578 7065 6374 6564 5f70 6172 7473 da1a  expected_parts..
+00000a90: 6765 745f 436f 6d70 6172 655f 6578 7065  get_Compare_expe
+00000aa0: 6374 6564 5f70 6172 7473 da20 6765 745f  cted_parts. get_
+00000ab0: 636f 6d70 7265 6865 6e73 696f 6e5f 6578  comprehension_ex
+00000ac0: 7065 6374 6564 5f70 6172 7473 da1b 6765  pected_parts..ge
+00000ad0: 745f 436f 6e74 696e 7565 5f65 7870 6563  t_Continue_expec
+00000ae0: 7465 645f 7061 7274 73da 1967 6574 5f44  ted_parts..get_D
+00000af0: 656c 6574 655f 6578 7065 6374 6564 5f70  elete_expected_p
+00000b00: 6172 7473 da17 6765 745f 4469 6374 5f65  arts..get_Dict_e
+00000b10: 7870 6563 7465 645f 7061 7274 73da 1b67  xpected_parts..g
+00000b20: 6574 5f44 6963 7443 6f6d 705f 6578 7065  et_DictComp_expe
+00000b30: 6374 6564 5f70 6172 7473 da16 6765 745f  cted_parts..get_
+00000b40: 4469 765f 6578 7065 6374 6564 5f70 6172  Div_expected_par
+00000b50: 7473 da15 6765 745f 4571 5f65 7870 6563  ts..get_Eq_expec
+00000b60: 7465 645f 7061 7274 73da 1767 6574 5f45  ted_parts..get_E
+00000b70: 7870 725f 6578 7065 6374 6564 5f70 6172  xpr_expected_par
+00000b80: 7473 da20 6765 745f 4578 6365 7074 4861  ts. get_ExceptHa
+00000b90: 6e64 6c65 725f 6578 7065 6374 6564 5f70  ndler_expected_p
+00000ba0: 6172 7473 da1b 6765 745f 466c 6f6f 7244  arts..get_FloorD
+00000bb0: 6976 5f65 7870 6563 7465 645f 7061 7274  iv_expected_part
+00000bc0: 73da 1667 6574 5f46 6f72 5f65 7870 6563  s..get_For_expec
+00000bd0: 7465 645f 7061 7274 73da 1e67 6574 5f46  ted_parts..get_F
+00000be0: 756e 6374 696f 6e44 6566 5f65 7870 6563  unctionDef_expec
+00000bf0: 7465 645f 7061 7274 73da 1f67 6574 5f47  ted_parts..get_G
+00000c00: 656e 6572 6174 6f72 4578 705f 6578 7065  eneratorExp_expe
+00000c10: 6374 6564 5f70 6172 7473 da19 6765 745f  cted_parts..get_
+00000c20: 476c 6f62 616c 5f65 7870 6563 7465 645f  Global_expected_
+00000c30: 7061 7274 73da 1567 6574 5f47 745f 6578  parts..get_Gt_ex
+00000c40: 7065 6374 6564 5f70 6172 7473 da16 6765  pected_parts..ge
+00000c50: 745f 4774 455f 6578 7065 6374 6564 5f70  t_GtE_expected_p
+00000c60: 6172 7473 da0f 4966 536f 7572 6365 4d61  arts..IfSourceMa
+00000c70: 7463 6865 727a 2c66 756e 5f77 6974 685f  tcherz,fun_with_
+00000c80: 6173 742e 736f 7572 6365 5f6d 6174 6368  ast.source_match
+00000c90: 6572 732e 6966 5f73 6f75 7263 655f 6d61  ers.if_source_ma
+00000ca0: 7463 68da 1867 6574 5f49 6645 7870 5f65  tch..get_IfExp_e
+00000cb0: 7870 6563 7465 645f 7061 7274 73da 1967  xpected_parts..g
+00000cc0: 6574 5f49 6d70 6f72 745f 6578 7065 6374  et_Import_expect
+00000cd0: 6564 5f70 6172 7473 da1d 6765 745f 496d  ed_parts..get_Im
+00000ce0: 706f 7274 4672 6f6d 5f65 7870 6563 7465  portFrom_expecte
+00000cf0: 645f 7061 7274 73da 1567 6574 5f49 6e5f  d_parts..get_In_
+00000d00: 6578 7065 6374 6564 5f70 6172 7473 da19  expected_parts..
+00000d10: 6765 745f 496e 7665 7274 5f65 7870 6563  get_Invert_expec
+00000d20: 7465 645f 7061 7274 73da 1567 6574 5f49  ted_parts..get_I
+00000d30: 735f 6578 7065 6374 6564 5f70 6172 7473  s_expected_parts
+00000d40: da18 6765 745f 4973 4e6f 745f 6578 7065  ..get_IsNot_expe
+00000d50: 6374 6564 5f70 6172 7473 da1a 6765 745f  cted_parts..get_
+00000d60: 6b65 7977 6f72 645f 6578 7065 6374 6564  keyword_expected
+00000d70: 5f70 6172 7473 da19 6765 745f 4c61 6d62  _parts..get_Lamb
+00000d80: 6461 5f65 7870 6563 7465 645f 7061 7274  da_expected_part
+00000d90: 73da 1767 6574 5f4c 6973 745f 6578 7065  s..get_List_expe
+00000da0: 6374 6564 5f70 6172 7473 da1b 6765 745f  cted_parts..get_
+00000db0: 4c69 7374 436f 6d70 5f65 7870 6563 7465  ListComp_expecte
+00000dc0: 645f 7061 7274 73da 1967 6574 5f4c 5368  d_parts..get_LSh
+00000dd0: 6966 745f 6578 7065 6374 6564 5f70 6172  ift_expected_par
+00000de0: 7473 da15 6765 745f 4c74 5f65 7870 6563  ts..get_Lt_expec
+00000df0: 7465 645f 7061 7274 73da 1667 6574 5f4c  ted_parts..get_L
+00000e00: 7445 5f65 7870 6563 7465 645f 7061 7274  tE_expected_part
+00000e10: 73da 1667 6574 5f4d 6f64 5f65 7870 6563  s..get_Mod_expec
+00000e20: 7465 645f 7061 7274 73da 1967 6574 5f4d  ted_parts..get_M
+00000e30: 6f64 756c 655f 6578 7065 6374 6564 5f70  odule_expected_p
+00000e40: 6172 7473 da17 6765 745f 4d75 6c74 5f65  arts..get_Mult_e
+00000e50: 7870 6563 7465 645f 7061 7274 73da 1767  xpected_parts..g
+00000e60: 6574 5f4e 616d 655f 6578 7065 6374 6564  et_Name_expected
+00000e70: 5f70 6172 7473 da16 6765 745f 4e6f 745f  _parts..get_Not_
+00000e80: 6578 7065 6374 6564 5f70 6172 7473 da18  expected_parts..
+00000e90: 6765 745f 4e6f 7449 6e5f 6578 7065 6374  get_NotIn_expect
+00000ea0: 6564 5f70 6172 7473 da18 6765 745f 4e6f  ed_parts..get_No
+00000eb0: 7445 715f 6578 7065 6374 6564 5f70 6172  tEq_expected_par
+00000ec0: 7473 da15 6765 745f 4f72 5f65 7870 6563  ts..get_Or_expec
+00000ed0: 7465 645f 7061 7274 73da 1767 6574 5f50  ted_parts..get_P
+00000ee0: 6173 735f 6578 7065 6374 6564 5f70 6172  ass_expected_par
+00000ef0: 7473 da16 6765 745f 506f 775f 6578 7065  ts..get_Pow_expe
+00000f00: 6374 6564 5f70 6172 7473 da18 6765 745f  cted_parts..get_
+00000f10: 5261 6973 655f 6578 7065 6374 6564 5f70  Raise_expected_p
+00000f20: 6172 7473 da19 6765 745f 5265 7475 726e  arts..get_Return
+00000f30: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
+00000f40: 1967 6574 5f52 5368 6966 745f 6578 7065  .get_RShift_expe
+00000f50: 6374 6564 5f70 6172 7473 da18 6765 745f  cted_parts..get_
+00000f60: 536c 6963 655f 6578 7065 6374 6564 5f70  Slice_expected_p
+00000f70: 6172 7473 da16 6765 745f 5375 625f 6578  arts..get_Sub_ex
+00000f80: 7065 6374 6564 5f70 6172 7473 da16 6765  pected_parts..ge
+00000f90: 745f 5365 745f 6578 7065 6374 6564 5f70  t_Set_expected_p
+00000fa0: 6172 7473 da1a 6765 745f 5365 7443 6f6d  arts..get_SetCom
+00000fb0: 705f 6578 7065 6374 6564 5f70 6172 7473  p_expected_parts
+00000fc0: da1c 6765 745f 5375 6273 6372 6970 745f  ..get_Subscript_
+00000fd0: 6578 7065 6374 6564 5f70 6172 7473 da15  expected_parts..
+00000fe0: 436f 6e73 7461 6e74 536f 7572 6365 4d61  ConstantSourceMa
+00000ff0: 7463 6865 72da 1867 6574 5f54 7570 6c65  tcher..get_Tuple
+00001000: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
+00001010: 164a 6f69 6e65 6453 7472 536f 7572 6365  .JoinedStrSource
+00001020: 4d61 7463 6865 727a 2766 756e 5f77 6974  Matcherz'fun_wit
+00001030: 685f 6173 742e 736f 7572 6365 5f6d 6174  h_ast.source_mat
+00001040: 6368 6572 732e 6a6f 696e 6564 5f73 7472  chers.joined_str
+00001050: da1c 6765 745f 5472 7945 7863 6570 745f  ..get_TryExcept_
+00001060: 6578 7065 6374 6564 5f70 6172 7473 da21  expected_parts.!
+00001070: 6765 745f 466f 726d 6174 7465 6456 616c  get_FormattedVal
+00001080: 7565 5f65 7870 6563 7465 645f 7061 7274  ue_expected_part
+00001090: 73da 1767 6574 5f55 4164 645f 6578 7065  s..get_UAdd_expe
+000010a0: 6374 6564 5f70 6172 7473 da1a 6765 745f  cted_parts..get_
+000010b0: 556e 6172 794f 705f 6578 7065 6374 6564  UnaryOp_expected
+000010c0: 5f70 6172 7473 da17 6765 745f 5553 7562  _parts..get_USub
+000010d0: 5f65 7870 6563 7465 645f 7061 7274 73da  _expected_parts.
+000010e0: 1867 6574 5f57 6869 6c65 5f65 7870 6563  .get_While_expec
+000010f0: 7465 645f 7061 7274 73da 1157 6974 6853  ted_parts..WithS
+00001100: 6f75 7263 654d 6174 6368 6572 da15 5769  ourceMatcher..Wi
+00001110: 7468 4974 656d 536f 7572 6365 4d61 7463  thItemSourceMatc
+00001120: 6865 727a 2566 756e 5f77 6974 685f 6173  herz%fun_with_as
+00001130: 742e 736f 7572 6365 5f6d 6174 6368 6572  t.source_matcher
+00001140: 732e 7769 7468 6974 656d da18 6765 745f  s.withitem..get_
+00001150: 5969 656c 645f 6578 7065 6374 6564 5f70  Yield_expected_p
+00001160: 6172 7473 da15 5379 6e74 6178 4672 6565  arts..SyntaxFree
+00001170: 4c69 6e65 4d61 7463 6865 727a 2b66 756e  LineMatcherz+fun
+00001180: 5f77 6974 685f 6173 742e 736f 7572 6365  _with_ast.source
+00001190: 5f6d 6174 6368 6572 732e 7379 6e74 6178  _matchers.syntax
+000011a0: 6672 6565 6c69 6e65 da1a 6765 745f 436f  freeline..get_Co
+000011b0: 6d6d 656e 745f 6578 7065 6374 6564 5f70  mment_expected_p
+000011c0: 6172 7473 da1b 6765 745f 4361 6c6c 4172  arts..get_CallAr
+000011d0: 6773 5f65 7870 6563 7465 645f 7061 7274  gs_expected_part
+000011e0: 7329 034e 4e4e 295e da04 5f61 7374 7205  s).NNN)^.._astr.
+000011f0: 0000 00da 2866 756e 5f77 6974 685f 6173  ....(fun_with_as
+00001200: 742e 6d61 6e69 7075 6c61 7465 5f6e 6f64  t.manipulate_nod
+00001210: 652e 6372 6561 7465 5f6e 6f64 65da 0c66  e.create_node..f
+00001220: 756e 5f77 6974 685f 6173 74da 3266 756e  un_with_ast.2fun
+00001230: 5f77 6974 685f 6173 742e 6d61 6e69 7075  _with_ast.manipu
+00001240: 6c61 7465 5f6e 6f64 652e 7379 6e74 6178  late_node.syntax
+00001250: 5f66 7265 655f 6c69 6e65 5f6e 6f64 65da  _free_line_node.
+00001260: 2b66 756e 5f77 6974 685f 6173 742e 6d61  +fun_with_ast.ma
+00001270: 6e69 7075 6c61 7465 5f6e 6f64 652e 6361  nipulate_node.ca
+00001280: 6c6c 5f61 7267 735f 6e6f 6465 7217 0000  ll_args_noder...
+00001290: 00da 0341 6464 da05 616c 6961 73da 0341  ...Add..alias..A
+000012a0: 6e64 da06 4173 7365 7274 da06 4173 7369  nd..Assert..Assi
+000012b0: 676e da09 4174 7472 6962 7574 65da 0941  gn..Attribute..A
+000012c0: 7567 4173 7369 676e da09 6172 6775 6d65  ugAssign..argume
+000012d0: 6e74 73da 0361 7267 da05 4269 6e4f 70da  nts..arg..BinOp.
+000012e0: 0642 6974 416e 64da 0542 6974 4f72 da06  .BitAnd..BitOr..
+000012f0: 4269 7458 6f72 da06 426f 6f6c 4f70 da05  BitXor..BoolOp..
+00001300: 4272 6561 6bda 0443 616c 6cda 0843 6c61  Break..Call..Cla
+00001310: 7373 4465 66da 0743 6f6d 7061 7265 da0d  ssDef..Compare..
+00001320: 636f 6d70 7265 6865 6e73 696f 6eda 0843  comprehension..C
+00001330: 6f6e 7469 6e75 65da 0644 656c 6574 65da  ontinue..Delete.
+00001340: 0444 6963 74da 0844 6963 7443 6f6d 70da  .Dict..DictComp.
+00001350: 0344 6976 da02 4571 da04 4578 7072 da0d  .Div..Eq..Expr..
+00001360: 4578 6365 7074 4861 6e64 6c65 72da 0846  ExceptHandler..F
+00001370: 6c6f 6f72 4469 76da 0346 6f72 da0b 4675  loorDiv..For..Fu
+00001380: 6e63 7469 6f6e 4465 66da 0c47 656e 6572  nctionDef..Gener
+00001390: 6174 6f72 4578 70da 0647 6c6f 6261 6cda  atorExp..Global.
+000013a0: 0247 74da 0347 7445 da02 4966 da05 4966  .Gt..GtE..If..If
+000013b0: 4578 70da 0649 6d70 6f72 74da 0a49 6d70  Exp..Import..Imp
+000013c0: 6f72 7446 726f 6dda 0249 6eda 0649 6e76  ortFrom..In..Inv
+000013d0: 6572 74da 0249 73da 0549 734e 6f74 da07  ert..Is..IsNot..
+000013e0: 6b65 7977 6f72 64da 064c 616d 6264 61da  keyword..Lambda.
+000013f0: 044c 6973 74da 084c 6973 7443 6f6d 70da  .List..ListComp.
+00001400: 064c 5368 6966 74da 024c 74da 034c 7445  .LShift..Lt..LtE
+00001410: da03 4d6f 64da 064d 6f64 756c 65da 044d  ..Mod..Module..M
+00001420: 756c 74da 044e 616d 65da 034e 6f74 da05  ult..Name..Not..
+00001430: 4e6f 7449 6eda 054e 6f74 4571 da02 4f72  NotIn..NotEq..Or
+00001440: da04 5061 7373 da03 506f 77da 0552 6169  ..Pass..Pow..Rai
+00001450: 7365 da06 5265 7475 726e da06 5253 6869  se..Return..RShi
+00001460: 6674 da05 536c 6963 65da 0353 7562 da03  ft..Slice..Sub..
+00001470: 5365 74da 0753 6574 436f 6d70 da09 5375  Set..SetComp..Su
+00001480: 6273 6372 6970 74da 0843 6f6e 7374 616e  bscript..Constan
+00001490: 74da 0554 7570 6c65 da09 4a6f 696e 6564  t..Tuple..Joined
+000014a0: 5374 72da 0354 7279 da0e 466f 726d 6174  Str..Try..Format
+000014b0: 7465 6456 616c 7565 da04 5541 6464 da07  tedValue..UAdd..
+000014c0: 556e 6172 794f 70da 0455 5375 62da 0557  UnaryOp..USub..W
+000014d0: 6869 6c65 da04 5769 7468 da08 7769 7468  hile..With..with
+000014e0: 6974 656d da05 5969 656c 64da 0f6d 616e  item..Yield..man
+000014f0: 6970 756c 6174 655f 6e6f 6465 da15 7379  ipulate_node..sy
+00001500: 6e74 6178 5f66 7265 655f 6c69 6e65 5f6e  ntax_free_line_n
+00001510: 6f64 65da 0e53 796e 7461 7846 7265 654c  ode..SyntaxFreeL
+00001520: 696e 65da 0b63 7265 6174 655f 6e6f 6465  ine..create_node
+00001530: da07 436f 6d6d 656e 74da 0e63 616c 6c5f  ..Comment..call_
+00001540: 6172 6773 5f6e 6f64 65da 0843 616c 6c41  args_node..CallA
+00001550: 7267 7372 0300 0000 7215 0000 0072 1500  rgsr....r....r..
+00001560: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
+00001570: 6f64 756c 653e 0100 0000 7340 0100 0008  odule>....s@....
+00001580: 0108 0108 0208 0108 010a 0302 200a 0102  ............ ...
+00001590: ff0a 0202 fe0a 0302 fd0a 0402 fc0a 0502  ................
+000015a0: fb0a 0602 fa0a 0702 f90a 0802 f80a 0902  ................
+000015b0: f70a 0a02 f60a 0b02 f50a 0c02 f40a 0d02  ................
+000015c0: f30a 0e02 f20a 0f02 f10a 1002 f00a 1104  ................
+000015d0: ef0a 1202 ee0a 1302 ed0a 1402 ec0a 1502  ................
+000015e0: eb0a 1602 ea0a 1702 e90a 1802 e80a 1902  ................
+000015f0: e70a 1a02 e60a 1b02 e50a 1c02 e40a 1d02  ................
+00001600: e30a 1e02 e20a 1f02 e10a 2002 e00a 2102  .......... ...!.
+00001610: df0a 2206 de0a 2302 dd0a 2402 dc0a 2502  .."...#...$...%.
+00001620: db0a 2602 da0a 2702 d90a 2802 d80a 2902  ..&...'...(...).
+00001630: d70a 2a02 d60a 2b02 d50a 2c02 d40a 2d02  ..*...+...,...-.
+00001640: d30a 2e02 d20a 2f02 d10a 3002 d00a 3102  ....../...0...1.
+00001650: cf0a 3202 ce0a 3306 cd0a 3402 cc0a 3502  ..2...3...4...5.
+00001660: cb0a 3602 ca0a 3702 c90a 3802 c80a 3902  ..6...7...8...9.
+00001670: c70a 3a02 c60a 3b02 c50a 3c02 c40a 3d02  ..:...;...<...=.
+00001680: c30a 3e02 c20a 3f02 c10a 4002 c00a 4102  ..>...?...@...A.
+00001690: bf0a 4202 be0a 4302 bd0a 4404 bc0a 450a  ..B...C...D...E.
+000016a0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+000016b0: 010a 010a 0102 0102 ff0e 020e 010a ad    ...............
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/str.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/str.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 21 19:10:20 2023 UTC, .py size: 5346 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,256 +1,265 @@
-00000000: 6f0d 0d0a 0000 0000 1c4b 9364 e214 0000  o........K.d....
+00000000: 6f0d 0d0a 0000 0000 db29 b064 7514 0000  o........).du...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
+00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c03 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
-00000060: 6d07 5a07 0100 6400 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000070: 6d0a 5a0a 0100 6400 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 4700 6408 6409 8400 6409 6505 8303  ..G.d.d...d.e...
-00000090: 5a0d 6401 5300 290a e900 0000 004e 2901  Z.d.S.)......N).
-000000a0: da1b 4261 646c 7953 7065 6369 6669 6564  ..BadlySpecified
-000000b0: 5465 6d70 6c61 7465 4572 726f 7229 01da  TemplateError)..
-000000c0: 104d 6174 6368 506c 6163 6568 6f6c 6465  .MatchPlaceholde
-000000d0: 7229 01da 0d53 6f75 7263 654d 6174 6368  r)...SourceMatch
-000000e0: 6572 2901 da15 5374 7269 6e67 5061 7274  er)...StringPart
-000000f0: 506c 6163 6568 6f6c 6465 7229 02da 0f5f  Placeholder)..._
-00000100: 4765 744c 6973 7444 6566 6175 6c74 da13  GetListDefault..
-00000110: 4765 7444 6566 6175 6c74 5175 6f74 6554  GetDefaultQuoteT
-00000120: 7970 6529 01da 0f54 6578 7450 6c61 6365  ype)...TextPlace
-00000130: 686f 6c64 6572 6300 0000 0000 0000 0000  holderc.........
-00000140: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-00000150: 5a00 0000 6500 5a01 6400 5a02 6401 5a03  Z...e.Z.d.Z.d.Z.
-00000160: 6414 8700 6601 6404 6405 8409 5a04 6406  d...f.d.d...Z.d.
-00000170: 6407 8400 5a05 6408 6409 8400 5a06 640a  d...Z.d.d...Z.d.
-00000180: 640b 8400 5a07 640c 640d 8400 5a08 640e  d...Z.d.d...Z.d.
-00000190: 640f 8400 5a09 6410 6411 8400 5a0a 6412  d...Z.d.d...Z.d.
-000001a0: 6413 8400 5a0b 8700 0400 5a0c 5300 2915  d...Z.....Z.S.).
-000001b0: da10 5374 7253 6f75 7263 654d 6174 6368  ..StrSourceMatch
-000001c0: 6572 7a32 436c 6173 7320 746f 2067 656e  erz2Class to gen
-000001d0: 6572 6174 6520 7468 6520 736f 7572 6365  erate the source
-000001e0: 2066 6f72 2061 6e20 5f61 7374 2e53 7472   for an _ast.Str
-000001f0: 206e 6f64 652e 4e54 6304 0000 0000 0000   node.NTc.......
-00000200: 0000 0000 0004 0000 0004 0000 0003 0000  ................
-00000210: 0073 4600 0000 7400 7401 7c00 8302 a002  .sF...t.t.|.....
-00000220: 7c01 7c02 a102 0100 7403 6401 6402 8302  |.|.....t.d.d...
-00000230: 7c00 5f04 6700 7c00 5f05 6700 7c00 5f06  |._.g.|._.g.|._.
-00000240: 6400 7c00 5f07 6400 7c00 5f08 6400 7c00  d.|._.d.|._.d.|.
-00000250: 5f09 7c03 7c00 5f0a 6400 5300 2903 4e7a  _.|.|._.d.S.).Nz
-00000260: 035c 732a da00 290b da05 7375 7065 7272  .\s*..)...superr
-00000270: 0900 0000 da08 5f5f 696e 6974 5f5f 7208  ......__init__r.
-00000280: 0000 00da 1573 6570 6172 6174 6f72 5f70  .....separator_p
-00000290: 6c61 6365 686f 6c64 6572 da0b 7175 6f74  laceholder..quot
-000002a0: 655f 7061 7274 73da 0a73 6570 6172 6174  e_parts..separat
-000002b0: 6f72 73da 0a71 756f 7465 5f74 7970 65da  ors..quote_type.
-000002c0: 136f 7269 6769 6e61 6c5f 7175 6f74 655f  .original_quote_
-000002d0: 7479 7065 da0a 6f72 6967 696e 616c 5f73  type..original_s
-000002e0: da18 6163 6365 7074 5f6d 756c 7469 7061  ..accept_multipa
-000002f0: 7274 735f 7374 7269 6e67 2904 da04 7365  rts_string)...se
-00000300: 6c66 da04 6e6f 6465 da0f 7374 6172 7469  lf..node..starti
-00000310: 6e67 5f70 6172 656e 7372 1300 0000 a901  ng_parensr......
-00000320: da09 5f5f 636c 6173 735f 5fa9 00fa 3b2f  ..__class__...;/
-00000330: 686f 6d65 2f73 6861 692f 6675 6e5f 7769  home/shai/fun_wi
-00000340: 7468 5f61 7374 2f66 756e 5f77 6974 685f  th_ast/fun_with_
-00000350: 6173 742f 736f 7572 6365 5f6d 6174 6368  ast/source_match
-00000360: 6572 732f 7374 722e 7079 720c 0000 000f  ers/str.pyr.....
-00000370: 0000 0073 1000 0000 1201 0c01 0601 0601  ...s............
-00000380: 0602 0601 0601 0a01 7a19 5374 7253 6f75  ........z.StrSou
-00000390: 7263 654d 6174 6368 6572 2e5f 5f69 6e69  rceMatcher.__ini
-000003a0: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
-000003b0: 0100 0000 0500 0000 0300 0000 731a 0000  ............s...
-000003c0: 0064 01a0 0087 0066 0164 0264 0384 0888  .d.....f.d.d....
-000003d0: 006a 0144 0083 01a1 0153 0029 044e 720a  .j.D.....S.).Nr.
-000003e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000003f0: 0200 0000 0400 0000 3300 0000 731e 0000  ........3...s...
-00000400: 0081 007c 005d 0a7d 017c 016a 00a0 0188  ...|.].}.|.j....
-00000410: 006a 02a1 0156 0001 0071 0264 0053 00a9  .j...V...q.d.S..
-00000420: 014e 2903 da16 696e 6e65 725f 7465 7874  .N)...inner_text
-00000430: 5f70 6c61 6365 686f 6c64 6572 da09 4765  _placeholder..Ge
-00000440: 7453 6f75 7263 6572 1500 0000 2902 da02  tSourcer....)...
-00000450: 2e30 da01 70a9 0172 1400 0000 7219 0000  .0..p..r....r...
-00000460: 0072 1a00 0000 da09 3c67 656e 6578 7072  .r......<genexpr
-00000470: 3e1b 0000 0073 0800 0000 0280 0400 0201  >....s..........
-00000480: 16ff 7a38 5374 7253 6f75 7263 654d 6174  ..z8StrSourceMat
-00000490: 6368 6572 2e5f 4765 744d 6174 6368 6564  cher._GetMatched
-000004a0: 496e 6e65 7254 6578 742e 3c6c 6f63 616c  InnerText.<local
-000004b0: 733e 2e3c 6765 6e65 7870 723e 2902 da04  s>.<genexpr>)...
-000004c0: 6a6f 696e 720e 0000 0072 2000 0000 7219  joinr....r ...r.
-000004d0: 0000 0072 2000 0000 721a 0000 00da 145f  ...r ...r......_
-000004e0: 4765 744d 6174 6368 6564 496e 6e65 7254  GetMatchedInnerT
-000004f0: 6578 741a 0000 0073 0600 0000 0e01 0401  ext....s........
-00000500: 08ff 7a25 5374 7253 6f75 7263 654d 6174  ..z%StrSourceMat
-00000510: 6368 6572 2e5f 4765 744d 6174 6368 6564  cher._GetMatched
-00000520: 496e 6e65 7254 6578 7463 0200 0000 0000  InnerTextc......
-00000530: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
-00000540: 0000 7378 0000 007c 00a0 007c 01a1 017d  ..sx...|...|...}
-00000550: 027c 00a0 01a1 0001 007c 00a0 02a1 007d  .|.......|.....}
-00000560: 0374 037c 0264 007c 0383 037d 027c 006a  .t.|.d.|...}.|.j
-00000570: 04a0 057c 03a1 0101 007c 00a0 067c 02a1  ...|.....|...|..
-00000580: 017d 027c 00a0 077c 02a1 0101 007c 006a  .}.|...|.....|.j
-00000590: 0464 0119 006a 086a 097c 005f 0a7c 00a0  .d...j.j.|._.|..
-000005a0: 0ba1 007d 0474 0ca0 0d7c 00a1 017d 0564  ...}.t...|...}.d
-000005b0: 027c 005f 0e7c 057c 005f 0f7c 0553 0029  .|._.|.|._.|.S.)
-000005c0: 034e 7201 0000 0054 2910 da10 4d61 7463  .Nr....T)...Matc
-000005d0: 6853 7461 7274 5061 7265 6e73 da14 5f67  hStartParens.._g
-000005e0: 6574 5f6f 7269 6769 6e61 6c5f 7374 7269  et_original_stri
-000005f0: 6e67 da12 5f70 6172 745f 706c 6163 655f  ng.._part_place_
-00000600: 686f 6c64 6572 7203 0000 0072 0e00 0000  holderr....r....
-00000610: da06 6170 7065 6e64 da11 5f68 616e 646c  ..append.._handl
-00000620: 655f 6d75 6c74 6970 6172 74da 0d4d 6174  e_multipart..Mat
-00000630: 6368 456e 6450 6172 656e da17 7175 6f74  chEndParen..quot
-00000640: 655f 6d61 7463 685f 706c 6163 6568 6f6c  e_match_placehol
-00000650: 6465 72da 0c6d 6174 6368 6564 5f74 6578  der..matched_tex
-00000660: 7472 1100 0000 da14 5f6d 6174 6368 5f70  tr......_match_p
-00000670: 6172 7365 645f 7374 7269 6e67 7209 0000  arsed_stringr...
-00000680: 0072 1d00 0000 da07 6d61 7463 6865 64da  .r......matched.
-00000690: 0e6d 6174 6368 6564 5f73 6f75 7263 6529  .matched_source)
-000006a0: 0672 1400 0000 da06 7374 7269 6e67 da10  .r......string..
-000006b0: 7265 6d61 696e 696e 675f 7374 7269 6e67  remaining_string
-000006c0: da04 7061 7274 da0d 7061 7273 6564 5f73  ..part..parsed_s
-000006d0: 7472 696e 67da 0672 6573 756c 7472 1900  tring..resultr..
-000006e0: 0000 7219 0000 0072 1a00 0000 da06 5f6d  ..r....r......_m
-000006f0: 6174 6368 1e00 0000 731c 0000 000a 0108  atch....s.......
-00000700: 0108 010c 010c 010a 020a 020c 0404 ff08  ................
-00000710: 020a 0106 0106 0104 017a 1753 7472 536f  .........z.StrSo
-00000720: 7572 6365 4d61 7463 6865 722e 5f6d 6174  urceMatcher._mat
-00000730: 6368 6301 0000 0000 0000 0000 0000 0008  chc.............
-00000740: 0000 0005 0000 0043 0000 0073 a800 0000  .......C...s....
-00000750: 7c00 a000 a100 7d01 7c00 a001 a100 7d02  |.....}.|.....}.
-00000760: 7c00 6a02 7d03 7c00 6a02 7d04 6401 7d05  |.j.}.|.j.}.d.}.
-00000770: 7c00 6a03 4400 5d08 7d06 7c05 7c06 6a04  |.j.D.].}.|.|.j.
-00000780: 6a05 3700 7d05 7113 7406 7c05 8301 7406  j.7.}.q.t.|...t.
-00000790: 7c00 6a07 8301 6b03 7230 7408 6402 7c05  |.j...k.r0t.d.|.
-000007a0: 9b00 6403 7c00 6a07 9b00 9d04 8301 8201  ..d.|.j.........
-000007b0: 7c01 7c03 1700 7c05 1700 7c04 1700 7c02  |.|...|...|...|.
-000007c0: 1700 7d07 7c07 7c01 7c03 1700 7c00 6a07  ..}.|.|.|...|.j.
-000007d0: 1700 7c04 1700 7c02 1700 6b03 7252 7408  ..|...|...k.rRt.
-000007e0: 6404 7c07 9b00 6403 7c00 6a07 9b00 9d04  d.|...d.|.j.....
-000007f0: 8301 8201 7c07 5300 2905 4e72 0a00 0000  ....|.S.).Nr....
-00000800: 7a0d 5374 7269 6e67 2062 6f64 793a 207a  z.String body: z
-00000810: 1820 646f 6573 206e 6f74 206d 6174 6368  . does not match
-00000820: 206e 6f64 652e 733a 207a 0d50 6172 7365   node.s: z.Parse
-00000830: 6420 626f 6479 3a20 2909 da11 4765 7453  d body: )...GetS
-00000840: 7461 7274 5061 7265 6e54 6578 74da 0f47  tartParenText..G
-00000850: 6574 456e 6450 6172 656e 5465 7874 7211  etEndParenTextr.
-00000860: 0000 0072 0e00 0000 721c 0000 0072 2b00  ...r....r....r+.
-00000870: 0000 da03 6c65 6e72 1200 0000 7202 0000  ....lenr....r...
-00000880: 0029 0872 1400 0000 da10 7374 6172 745f  .).r......start_
-00000890: 7061 7261 6e5f 7465 7874 da0e 656e 645f  paran_text..end_
-000008a0: 7061 7261 6e5f 7465 7874 da0b 7374 6172  paran_text..star
-000008b0: 745f 7175 6f74 65da 0965 6e64 5f71 756f  t_quote..end_quo
-000008c0: 7465 da0b 7374 7269 6e67 5f62 6f64 7972  te..string_bodyr
-000008d0: 3100 0000 7232 0000 0072 1900 0000 7219  1...r2...r....r.
-000008e0: 0000 0072 1a00 0000 722c 0000 0032 0000  ...r....r,...2..
-000008f0: 0073 1a00 0000 0801 0801 0601 0601 0402  .s..............
-00000900: 0a01 0e01 1201 1601 1401 1a01 1601 0404  ................
-00000910: 7a25 5374 7253 6f75 7263 654d 6174 6368  z%StrSourceMatch
-00000920: 6572 2e5f 6d61 7463 685f 7061 7273 6564  er._match_parsed
-00000930: 5f73 7472 696e 6763 0200 0000 0000 0000  _stringc........
-00000940: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
-00000950: 7374 0000 007c 006a 0073 057c 0153 0009  st...|.j.s.|.S..
-00000960: 007c 006a 01a0 02a1 007d 0274 037c 0164  .|.j.....}.t.|.d
-00000970: 007c 0283 037d 0374 04a0 0564 027c 03a1  .|...}.t...d.|..
-00000980: 0273 2074 04a0 0564 037c 03a1 0273 2009  .s t...d.|...s .
-00000990: 007c 0153 007c 037d 017c 006a 06a0 077c  .|.S.|.}.|.j...|
-000009a0: 02a1 0101 0074 087c 006a 0083 017d 0474  .....t.|.j...}.t
-000009b0: 037c 0164 007c 0483 037d 017c 006a 09a0  .|.d.|...}.|.j..
-000009c0: 077c 04a1 0101 0071 0629 044e 547a 1d75  .|.....q.).NTz.u
-000009d0: 7222 7c75 5222 7c55 7222 7c55 5222 7c75  r"|uR"|Ur"|UR"|u
-000009e0: 227c 5522 7c72 227c 5222 7c22 7a1d 7572  "|U"|r"|R"|"z.ur
-000009f0: 277c 7552 277c 5572 277c 5552 277c 7527  '|uR'|Ur'|UR'|u'
-00000a00: 7c55 277c 7227 7c52 277c 2729 0a72 1300  |U'|r'|R'|').r..
-00000a10: 0000 720d 0000 00da 0443 6f70 7972 0300  ..r......Copyr..
-00000a20: 0000 da02 7265 da05 6d61 7463 6872 0f00  ....re..matchr..
-00000a30: 0000 7227 0000 0072 0500 0000 720e 0000  ..r'...r....r...
-00000a40: 0029 0572 1400 0000 7230 0000 00da 0973  .).r....r0.....s
-00000a50: 6570 6172 6174 6f72 da0c 7472 6961 6c5f  eparator..trial_
-00000a60: 7374 7269 6e67 7231 0000 0072 1900 0000  stringr1...r....
-00000a70: 7219 0000 0072 1a00 0000 7228 0000 0045  r....r....r(...E
-00000a80: 0000 0073 2000 0000 0601 0401 0201 0a01  ...s ...........
-00000a90: 0c01 0c01 0a01 02ff 0202 0406 04fb 0c01  ................
-00000aa0: 0a01 0c01 0c01 02f6 7a22 5374 7253 6f75  ........z"StrSou
-00000ab0: 7263 654d 6174 6368 6572 2e5f 6861 6e64  rceMatcher._hand
-00000ac0: 6c65 5f6d 756c 7469 7061 7274 6301 0000  le_multipartc...
-00000ad0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00000ae0: 0043 0000 0073 1801 0000 7c00 6a00 6400  .C...s....|.j.d.
-00000af0: 7501 721c 7c00 6a00 7c00 6a01 6a02 6b03  u.r.|.j.|.j.j.k.
-00000b00: 721c 7c00 6a03 6401 1900 6701 7c00 5f03  r.|.j.d...g.|._.
-00000b10: 7c00 6a01 6a02 7c00 6a03 6401 1900 6a04  |.j.j.|.j.d...j.
-00000b20: 5f05 7c00 6a00 6400 7500 7235 7c00 6a06  _.|.j.d.u.r5|.j.
-00000b30: 732b 7c00 6a07 7029 7408 8300 7c00 5f06  s+|.j.p)t...|._.
-00000b40: 7c00 6a06 7c00 6a01 6a02 1700 7c00 6a06  |.j.|.j.j...|.j.
-00000b50: 1700 5300 7c00 6a06 7243 7c00 6a03 4400  ..S.|.j.rC|.j.D.
-00000b60: 5d07 7d01 7c00 6a06 7c01 6a09 5f05 713b  ].}.|.j.|.j._.q;
-00000b70: 7c00 a00a a100 6701 7d02 7c02 a00b 740c  |.....g.}.|...t.
-00000b80: 7c00 6a03 6401 6400 8303 a00d 6400 a101  |.j.d.d.....d...
-00000b90: a101 0100 740e 740f 7c00 6a03 6402 6400  ....t.t.|.j.d.d.
-00000ba0: 8502 1900 8301 8301 4400 5d1f 7d03 7c02  ........D.].}.|.
-00000bb0: a00b 740c 7c00 6a10 7c03 7c00 6a11 8303  ..t.|.j.|.|.j...
-00000bc0: a00d 6400 a101 a101 0100 7c02 a00b 740c  ..d.......|...t.
-00000bd0: 7c00 6a03 7c03 6402 1700 6400 8303 a00d  |.j.|.d...d.....
-00000be0: 6400 a101 a101 0100 7160 7c02 a00b 7c00  d.......q`|...|.
-00000bf0: a012 a100 a101 0100 6403 a013 7c02 a101  ........d...|...
-00000c00: 5300 2904 4e72 0100 0000 e901 0000 0072  S.).Nr.........r
-00000c10: 0a00 0000 2914 7212 0000 0072 1500 0000  ....).r....r....
-00000c20: da01 7372 0e00 0000 721c 0000 0072 2b00  ..sr....r....r+.
-00000c30: 0000 7210 0000 0072 1100 0000 7207 0000  ..r....r....r...
-00000c40: 0072 2a00 0000 7235 0000 0072 2700 0000  .r*...r5...r'...
-00000c50: 7206 0000 0072 1d00 0000 da05 7261 6e67  r....r......rang
-00000c60: 6572 3700 0000 720f 0000 0072 0d00 0000  er7...r....r....
-00000c70: 7236 0000 0072 2200 0000 2904 7214 0000  r6...r"...).r...
-00000c80: 0072 3100 0000 da0b 736f 7572 6365 5f6c  .r1.....source_l
-00000c90: 6973 74da 0569 6e64 6578 7219 0000 0072  ist..indexr....r
-00000ca0: 1900 0000 721a 0000 0072 1d00 0000 5500  ....r....r....U.
-00000cb0: 0000 733c 0000 0018 020e 0112 010a 0206  ..s<............
-00000cc0: 010e 0114 0106 020a 010c 010a 0206 0108  ................
-00000cd0: 0102 ff06 0104 ff1a 0206 0106 0104 0102  ................
-00000ce0: fe06 0204 fe06 030c 0102 ff06 0106 ff0e  ................
-00000cf0: 030a 017a 1a53 7472 536f 7572 6365 4d61  ...z.StrSourceMa
-00000d00: 7463 6865 722e 4765 7453 6f75 7263 6563  tcher.GetSourcec
-00000d10: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000d20: 0200 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
-00000d30: 006a 017c 005f 0264 0053 0072 1b00 0000  .j.|._.d.S.r....
-00000d40: 2903 7215 0000 0072 4300 0000 7212 0000  ).r....rC...r...
-00000d50: 0072 2000 0000 7219 0000 0072 1900 0000  .r ...r....r....
-00000d60: 721a 0000 0072 2500 0000 7100 0000 7302  r....r%...q...s.
-00000d70: 0000 000e 017a 2553 7472 536f 7572 6365  .....z%StrSource
-00000d80: 4d61 7463 6865 722e 5f67 6574 5f6f 7269  Matcher._get_ori
-00000d90: 6769 6e61 6c5f 7374 7269 6e67 6301 0000  ginal_stringc...
-00000da0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000db0: 0043 0000 0073 0a00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00000dc0: 8301 5300 721b 0000 0029 0272 0500 0000  ..S.r....).r....
-00000dd0: 7213 0000 0072 2000 0000 7219 0000 0072  r....r ...r....r
-00000de0: 1900 0000 721a 0000 0072 2600 0000 7400  ....r....r&...t.
-00000df0: 0000 7302 0000 000a 017a 2353 7472 536f  ..s......z#StrSo
-00000e00: 7572 6365 4d61 7463 6865 722e 5f70 6172  urceMatcher._par
-00000e10: 745f 706c 6163 655f 686f 6c64 6572 2902  t_place_holder).
-00000e20: 4e54 290d da08 5f5f 6e61 6d65 5f5f da0a  NT)...__name__..
-00000e30: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000e40: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000e50: 5f72 0c00 0000 7223 0000 0072 3400 0000  _r....r#...r4...
-00000e60: 722c 0000 0072 2800 0000 721d 0000 0072  r,...r(...r....r
-00000e70: 2500 0000 7226 0000 00da 0d5f 5f63 6c61  %...r&.....__cla
-00000e80: 7373 6365 6c6c 5f5f 7219 0000 0072 1900  sscell__r....r..
-00000e90: 0000 7217 0000 0072 1a00 0000 7209 0000  ..r....r....r...
-00000ea0: 000c 0000 0073 1400 0000 0800 0401 0e02  .....s..........
-00000eb0: 080b 0804 0814 0813 0810 081c 1003 7209  ..............r.
-00000ec0: 0000 0029 0e72 3e00 0000 da27 6675 6e5f  ...).r>....'fun_
-00000ed0: 7769 7468 5f61 7374 2e73 6f75 7263 655f  with_ast.source_
-00000ee0: 6d61 7463 6865 7273 2e65 7863 6570 7469  matchers.excepti
-00000ef0: 6f6e 7372 0200 0000 da29 6675 6e5f 7769  onsr.....)fun_wi
-00000f00: 7468 5f61 7374 2e73 6f75 7263 655f 6d61  th_ast.source_ma
-00000f10: 7463 6865 7273 2e62 6173 655f 6d61 7463  tchers.base_matc
-00000f20: 6865 7272 0300 0000 7204 0000 00da 2566  herr....r.....%f
-00000f30: 756e 5f77 6974 685f 6173 742e 706c 6163  un_with_ast.plac
-00000f40: 6568 6f6c 6465 7273 2e73 7472 696e 675f  eholders.string_
-00000f50: 7061 7274 7205 0000 00da 2c66 756e 5f77  partr.....,fun_w
-00000f60: 6974 685f 6173 742e 636f 6d6d 6f6e 5f75  ith_ast.common_u
-00000f70: 7469 6c73 2e75 7469 6c73 5f73 6f75 7263  tils.utils_sourc
-00000f80: 655f 6d61 7463 6872 0600 0000 7207 0000  e_matchr....r...
-00000f90: 00da 1e66 756e 5f77 6974 685f 6173 742e  ...fun_with_ast.
-00000fa0: 706c 6163 6568 6f6c 6465 7273 2e74 6578  placeholders.tex
-00000fb0: 7472 0800 0000 7209 0000 0072 1900 0000  tr....r....r....
-00000fc0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000fd0: 083c 6d6f 6475 6c65 3e01 0000 0073 1000  .<module>....s..
-00000fe0: 0000 0800 0c02 0c02 0c01 0c01 1001 0c01  ................
-00000ff0: 1403                                     ..
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 4700  ..d.d.l.m.Z...G.
+00000080: 6408 6409 8400 6409 6506 8303 5a0d 6401  d.d...d.e...Z.d.
+00000090: 5300 290a e900 0000 004e 2901 da1b 4261  S.)......N)...Ba
+000000a0: 646c 7953 7065 6369 6669 6564 5465 6d70  dlySpecifiedTemp
+000000b0: 6c61 7465 4572 726f 7229 01da 104d 6174  lateError)...Mat
+000000c0: 6368 506c 6163 6568 6f6c 6465 7229 01da  chPlaceholder)..
+000000d0: 0d53 6f75 7263 654d 6174 6368 6572 2901  .SourceMatcher).
+000000e0: da15 5374 7269 6e67 5061 7274 506c 6163  ..StringPartPlac
+000000f0: 6568 6f6c 6465 7229 01da 0f5f 4765 744c  eholder)..._GetL
+00000100: 6973 7444 6566 6175 6c74 2901 da0f 5465  istDefault)...Te
+00000110: 7874 506c 6163 6568 6f6c 6465 7263 0000  xtPlaceholderc..
+00000120: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000130: 0000 0000 0000 735a 0000 0065 005a 0164  ......sZ...e.Z.d
+00000140: 005a 0264 015a 0364 1487 0066 0164 0464  .Z.d.Z.d...f.d.d
+00000150: 0584 095a 0464 0664 0784 005a 0564 0864  ...Z.d.d...Z.d.d
+00000160: 0984 005a 0664 0a64 0b84 005a 0764 0c64  ...Z.d.d...Z.d.d
+00000170: 0d84 005a 0864 0e64 0f84 005a 0964 1064  ...Z.d.d...Z.d.d
+00000180: 1184 005a 0a64 1264 1384 005a 0b87 0004  ...Z.d.d...Z....
+00000190: 005a 0c53 0029 15da 1053 7472 536f 7572  .Z.S.)...StrSour
+000001a0: 6365 4d61 7463 6865 727a 3243 6c61 7373  ceMatcherz2Class
+000001b0: 2074 6f20 6765 6e65 7261 7465 2074 6865   to generate the
+000001c0: 2073 6f75 7263 6520 666f 7220 616e 205f   source for an _
+000001d0: 6173 742e 5374 7220 6e6f 6465 2e4e 5463  ast.Str node.NTc
+000001e0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+000001f0: 0400 0000 0300 0000 735c 0000 0074 0074  ........s\...t.t
+00000200: 017c 0083 02a0 027c 017c 02a1 0201 0074  .|.....|.|.....t
+00000210: 0364 0164 0283 027c 005f 0467 007c 005f  .d.d...|._.g.|._
+00000220: 0567 007c 005f 0674 077c 0164 0383 0272  .g.|._.t.|.d...r
+00000230: 1f7c 016a 087c 005f 096e 0474 0a64 0483  .|.j.|._.n.t.d..
+00000240: 0182 0164 007c 005f 0b64 007c 005f 0c7c  ...d.|._.d.|._.|
+00000250: 037c 005f 0d64 0053 0029 054e 7a03 5c73  .|._.d.S.).Nz.\s
+00000260: 2ada 00da 0d64 6566 6175 6c74 5f71 756f  *....default_quo
+00000270: 7465 7a28 6e6f 6465 206d 7573 7420 6861  tez(node must ha
+00000280: 7665 2061 2064 6566 6175 6c74 5f71 756f  ve a default_quo
+00000290: 7465 2061 7474 7269 6275 7465 290e da05  te attribute)...
+000002a0: 7375 7065 7272 0800 0000 da08 5f5f 696e  superr......__in
+000002b0: 6974 5f5f 7207 0000 00da 1573 6570 6172  it__r......separ
+000002c0: 6174 6f72 5f70 6c61 6365 686f 6c64 6572  ator_placeholder
+000002d0: da0b 7175 6f74 655f 7061 7274 73da 0a73  ..quote_parts..s
+000002e0: 6570 6172 6174 6f72 73da 0768 6173 6174  eparators..hasat
+000002f0: 7472 720a 0000 00da 0a71 756f 7465 5f74  trr......quote_t
+00000300: 7970 65da 0a56 616c 7565 4572 726f 72da  ype..ValueError.
+00000310: 136f 7269 6769 6e61 6c5f 7175 6f74 655f  .original_quote_
+00000320: 7479 7065 da0a 6f72 6967 696e 616c 5f73  type..original_s
+00000330: da18 6163 6365 7074 5f6d 756c 7469 7061  ..accept_multipa
+00000340: 7274 735f 7374 7269 6e67 2904 da04 7365  rts_string)...se
+00000350: 6c66 da04 6e6f 6465 da0f 7374 6172 7469  lf..node..starti
+00000360: 6e67 5f70 6172 656e 7372 1500 0000 a901  ng_parensr......
+00000370: da09 5f5f 636c 6173 735f 5fa9 00fa 3b2f  ..__class__...;/
+00000380: 686f 6d65 2f73 6861 692f 6675 6e5f 7769  home/shai/fun_wi
+00000390: 7468 5f61 7374 2f66 756e 5f77 6974 685f  th_ast/fun_with_
+000003a0: 6173 742f 736f 7572 6365 5f6d 6174 6368  ast/source_match
+000003b0: 6572 732f 7374 722e 7079 720c 0000 000f  ers/str.pyr.....
+000003c0: 0000 0073 1400 0000 1201 0c01 0601 0601  ...s............
+000003d0: 0a03 0a01 0802 0601 0601 0a01 7a19 5374  ............z.St
+000003e0: 7253 6f75 7263 654d 6174 6368 6572 2e5f  rSourceMatcher._
+000003f0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000400: 0000 0000 0100 0000 0500 0000 0300 0000  ................
+00000410: 731a 0000 0064 01a0 0087 0066 0164 0264  s....d.....f.d.d
+00000420: 0384 0888 006a 0144 0083 01a1 0153 0029  .....j.D.....S.)
+00000430: 044e 7209 0000 0063 0100 0000 0000 0000  .Nr....c........
+00000440: 0000 0000 0200 0000 0400 0000 3300 0000  ............3...
+00000450: 731e 0000 0081 007c 005d 0a7d 017c 016a  s......|.].}.|.j
+00000460: 00a0 0188 006a 02a1 0156 0001 0071 0264  .....j...V...q.d
+00000470: 0053 00a9 014e 2903 da16 696e 6e65 725f  .S...N)...inner_
+00000480: 7465 7874 5f70 6c61 6365 686f 6c64 6572  text_placeholder
+00000490: da09 4765 7453 6f75 7263 6572 1700 0000  ..GetSourcer....
+000004a0: 2902 da02 2e30 da01 70a9 0172 1600 0000  )....0..p..r....
+000004b0: 721b 0000 0072 1c00 0000 da09 3c67 656e  r....r......<gen
+000004c0: 6578 7072 3e1f 0000 0073 0800 0000 0280  expr>....s......
+000004d0: 0400 0201 16ff 7a38 5374 7253 6f75 7263  ......z8StrSourc
+000004e0: 654d 6174 6368 6572 2e5f 4765 744d 6174  eMatcher._GetMat
+000004f0: 6368 6564 496e 6e65 7254 6578 742e 3c6c  chedInnerText.<l
+00000500: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00000510: 2902 da04 6a6f 696e 720e 0000 0072 2200  )...joinr....r".
+00000520: 0000 721b 0000 0072 2200 0000 721c 0000  ..r....r"...r...
+00000530: 00da 145f 4765 744d 6174 6368 6564 496e  ..._GetMatchedIn
+00000540: 6e65 7254 6578 741e 0000 0073 0600 0000  nerText....s....
+00000550: 0e01 0401 08ff 7a25 5374 7253 6f75 7263  ......z%StrSourc
+00000560: 654d 6174 6368 6572 2e5f 4765 744d 6174  eMatcher._GetMat
+00000570: 6368 6564 496e 6e65 7254 6578 7463 0200  chedInnerTextc..
+00000580: 0000 0000 0000 0000 0000 0600 0000 0400  ................
+00000590: 0000 4300 0000 7378 0000 007c 00a0 007c  ..C...sx...|...|
+000005a0: 01a1 017d 027c 00a0 01a1 0001 007c 00a0  ...}.|.......|..
+000005b0: 02a1 007d 0374 037c 0264 007c 0383 037d  ...}.t.|.d.|...}
+000005c0: 027c 006a 04a0 057c 03a1 0101 007c 00a0  .|.j...|.....|..
+000005d0: 067c 02a1 017d 027c 00a0 077c 02a1 0101  .|...}.|...|....
+000005e0: 007c 006a 0464 0119 006a 086a 097c 005f  .|.j.d...j.j.|._
+000005f0: 0a7c 00a0 0ba1 007d 0474 0ca0 0d7c 00a1  .|.....}.t...|..
+00000600: 017d 0564 027c 005f 0e7c 057c 005f 0f7c  .}.d.|._.|.|._.|
+00000610: 0553 0029 034e 7201 0000 0054 2910 da10  .S.).Nr....T)...
+00000620: 4d61 7463 6853 7461 7274 5061 7265 6e73  MatchStartParens
+00000630: da14 5f67 6574 5f6f 7269 6769 6e61 6c5f  .._get_original_
+00000640: 7374 7269 6e67 da12 5f70 6172 745f 706c  string.._part_pl
+00000650: 6163 655f 686f 6c64 6572 7203 0000 0072  ace_holderr....r
+00000660: 0e00 0000 da06 6170 7065 6e64 da11 5f68  ......append.._h
+00000670: 616e 646c 655f 6d75 6c74 6970 6172 74da  andle_multipart.
+00000680: 0d4d 6174 6368 456e 6450 6172 656e da17  .MatchEndParen..
+00000690: 7175 6f74 655f 6d61 7463 685f 706c 6163  quote_match_plac
+000006a0: 6568 6f6c 6465 72da 0c6d 6174 6368 6564  eholder..matched
+000006b0: 5f74 6578 7472 1300 0000 da14 5f6d 6174  _textr......_mat
+000006c0: 6368 5f70 6172 7365 645f 7374 7269 6e67  ch_parsed_string
+000006d0: 7208 0000 0072 1f00 0000 da07 6d61 7463  r....r......matc
+000006e0: 6865 64da 0e6d 6174 6368 6564 5f73 6f75  hed..matched_sou
+000006f0: 7263 6529 0672 1600 0000 da06 7374 7269  rce).r......stri
+00000700: 6e67 da10 7265 6d61 696e 696e 675f 7374  ng..remaining_st
+00000710: 7269 6e67 da04 7061 7274 da0d 7061 7273  ring..part..pars
+00000720: 6564 5f73 7472 696e 67da 0672 6573 756c  ed_string..resul
+00000730: 7472 1b00 0000 721b 0000 0072 1c00 0000  tr....r....r....
+00000740: da06 5f6d 6174 6368 2200 0000 731c 0000  .._match"...s...
+00000750: 000a 0108 0108 010c 010c 010a 020a 020c  ................
+00000760: 0204 ff08 020a 0106 0106 0104 017a 1753  .............z.S
+00000770: 7472 536f 7572 6365 4d61 7463 6865 722e  trSourceMatcher.
+00000780: 5f6d 6174 6368 6301 0000 0000 0000 0000  _matchc.........
+00000790: 0000 0008 0000 0005 0000 0043 0000 0073  ...........C...s
+000007a0: a800 0000 7c00 a000 a100 7d01 7c00 a001  ....|.....}.|...
+000007b0: a100 7d02 7c00 6a02 7d03 7c00 6a02 7d04  ..}.|.j.}.|.j.}.
+000007c0: 6401 7d05 7c00 6a03 4400 5d08 7d06 7c05  d.}.|.j.D.].}.|.
+000007d0: 7c06 6a04 6a05 3700 7d05 7113 7406 7c05  |.j.j.7.}.q.t.|.
+000007e0: 8301 7406 7c00 6a07 8301 6b03 7230 7408  ..t.|.j...k.r0t.
+000007f0: 6402 7c05 9b00 6403 7c00 6a07 9b00 9d04  d.|...d.|.j.....
+00000800: 8301 8201 7c01 7c03 1700 7c05 1700 7c04  ....|.|...|...|.
+00000810: 1700 7c02 1700 7d07 7c07 7c01 7c03 1700  ..|...}.|.|.|...
+00000820: 7c00 6a07 1700 7c04 1700 7c02 1700 6b03  |.j...|...|...k.
+00000830: 7252 7408 6404 7c07 9b00 6403 7c00 6a07  rRt.d.|...d.|.j.
+00000840: 9b00 9d04 8301 8201 7c07 5300 2905 4e72  ........|.S.).Nr
+00000850: 0900 0000 7a0d 5374 7269 6e67 2062 6f64  ....z.String bod
+00000860: 793a 207a 1820 646f 6573 206e 6f74 206d  y: z. does not m
+00000870: 6174 6368 206e 6f64 652e 733a 207a 0d50  atch node.s: z.P
+00000880: 6172 7365 6420 626f 6479 3a20 2909 da11  arsed body: )...
+00000890: 4765 7453 7461 7274 5061 7265 6e54 6578  GetStartParenTex
+000008a0: 74da 0f47 6574 456e 6450 6172 656e 5465  t..GetEndParenTe
+000008b0: 7874 7213 0000 0072 0e00 0000 721e 0000  xtr....r....r...
+000008c0: 0072 2d00 0000 da03 6c65 6e72 1400 0000  .r-.....lenr....
+000008d0: 7202 0000 0029 0872 1600 0000 da10 7374  r....).r......st
+000008e0: 6172 745f 7061 7261 6e5f 7465 7874 da0e  art_paran_text..
+000008f0: 656e 645f 7061 7261 6e5f 7465 7874 da0b  end_paran_text..
+00000900: 7374 6172 745f 7175 6f74 65da 0965 6e64  start_quote..end
+00000910: 5f71 756f 7465 da0b 7374 7269 6e67 5f62  _quote..string_b
+00000920: 6f64 7972 3300 0000 7234 0000 0072 1b00  odyr3...r4...r..
+00000930: 0000 721b 0000 0072 1c00 0000 722e 0000  ..r....r....r...
+00000940: 0034 0000 0073 1a00 0000 0801 0801 0601  .4...s..........
+00000950: 0601 0402 0a01 0e01 1201 1601 1401 1a01  ................
+00000960: 1601 0403 7a25 5374 7253 6f75 7263 654d  ....z%StrSourceM
+00000970: 6174 6368 6572 2e5f 6d61 7463 685f 7061  atcher._match_pa
+00000980: 7273 6564 5f73 7472 696e 6763 0200 0000  rsed_stringc....
+00000990: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+000009a0: 4300 0000 7374 0000 007c 006a 0073 057c  C...st...|.j.s.|
+000009b0: 0153 0009 007c 006a 01a0 02a1 007d 0274  .S...|.j.....}.t
+000009c0: 037c 0164 007c 0283 037d 0374 04a0 0564  .|.d.|...}.t...d
+000009d0: 027c 03a1 0273 2074 04a0 0564 037c 03a1  .|...s t...d.|..
+000009e0: 0273 2009 007c 0153 007c 037d 017c 006a  .s ..|.S.|.}.|.j
+000009f0: 06a0 077c 02a1 0101 0074 087c 006a 0083  ...|.....t.|.j..
+00000a00: 017d 0474 037c 0164 007c 0483 037d 017c  .}.t.|.d.|...}.|
+00000a10: 006a 09a0 077c 04a1 0101 0071 0629 044e  .j...|.....q.).N
+00000a20: 547a 1d75 7222 7c75 5222 7c55 7222 7c55  Tz.ur"|uR"|Ur"|U
+00000a30: 5222 7c75 227c 5522 7c72 227c 5222 7c22  R"|u"|U"|r"|R"|"
+00000a40: 7a1d 7572 277c 7552 277c 5572 277c 5552  z.ur'|uR'|Ur'|UR
+00000a50: 277c 7527 7c55 277c 7227 7c52 277c 2729  '|u'|U'|r'|R'|')
+00000a60: 0a72 1500 0000 720d 0000 00da 0443 6f70  .r....r......Cop
+00000a70: 7972 0300 0000 da02 7265 da05 6d61 7463  yr......re..matc
+00000a80: 6872 0f00 0000 7229 0000 0072 0500 0000  hr....r)...r....
+00000a90: 720e 0000 0029 0572 1600 0000 7232 0000  r....).r....r2..
+00000aa0: 00da 0973 6570 6172 6174 6f72 da0c 7472  ...separator..tr
+00000ab0: 6961 6c5f 7374 7269 6e67 7233 0000 0072  ial_stringr3...r
+00000ac0: 1b00 0000 721b 0000 0072 1c00 0000 722a  ....r....r....r*
+00000ad0: 0000 0046 0000 0073 2000 0000 0601 0401  ...F...s .......
+00000ae0: 0201 0a01 0c01 0c01 0a01 02ff 0202 0406  ................
+00000af0: 04fb 0c01 0a01 0c01 0c01 02f6 7a22 5374  ............z"St
+00000b00: 7253 6f75 7263 654d 6174 6368 6572 2e5f  rSourceMatcher._
+00000b10: 6861 6e64 6c65 5f6d 756c 7469 7061 7274  handle_multipart
+00000b20: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000b30: 0007 0000 0043 0000 0073 1201 0000 7c00  .....C...s....|.
+00000b40: 6a00 6400 7501 721c 7c00 6a00 7c00 6a01  j.d.u.r.|.j.|.j.
+00000b50: 6a02 6b03 721c 7c00 6a03 6401 1900 6701  j.k.r.|.j.d...g.
+00000b60: 7c00 5f03 7c00 6a01 6a02 7c00 6a03 6401  |._.|.j.j.|.j.d.
+00000b70: 1900 6a04 5f05 7c00 6a00 6400 7500 7232  ..j._.|.j.d.u.r2
+00000b80: 7c00 6a06 7328 7407 6402 8301 8201 7c00  |.j.s(t.d.....|.
+00000b90: 6a06 7c00 6a01 6a02 1700 7c00 6a06 1700  j.|.j.j...|.j...
+00000ba0: 5300 7c00 6a06 7240 7c00 6a03 4400 5d07  S.|.j.r@|.j.D.].
+00000bb0: 7d01 7c00 6a06 7c01 6a0a 5f05 7138 7c00  }.|.j.|.j._.q8|.
+00000bc0: a00b a100 6701 7d02 7c02 a00c 740d 7c00  ....g.}.|...t.|.
+00000bd0: 6a03 6401 6400 8303 a00e 6400 a101 a101  j.d.d.....d.....
+00000be0: 0100 740f 7410 7c00 6a03 6403 6400 8502  ..t.t.|.j.d.d...
+00000bf0: 1900 8301 8301 4400 5d1f 7d03 7c02 a00c  ......D.].}.|...
+00000c00: 740d 7c00 6a11 7c03 7c00 6a12 8303 a00e  t.|.j.|.|.j.....
+00000c10: 6400 a101 a101 0100 7c02 a00c 740d 7c00  d.......|...t.|.
+00000c20: 6a03 7c03 6403 1700 6400 8303 a00e 6400  j.|.d...d.....d.
+00000c30: a101 a101 0100 715d 7c02 a00c 7c00 a013  ......q]|...|...
+00000c40: a100 a101 0100 6404 a014 7c02 a101 5300  ......d...|...S.
+00000c50: 2905 4e72 0100 0000 7a16 7175 6f74 655f  ).Nr....z.quote_
+00000c60: 7479 7065 206d 7573 7420 6265 2073 6574  type must be set
+00000c70: e901 0000 0072 0900 0000 2915 7214 0000  .....r....).r...
+00000c80: 0072 1700 0000 da01 7372 0e00 0000 721e  .r......sr....r.
+00000c90: 0000 0072 2d00 0000 7211 0000 0072 1200  ...r-...r....r..
+00000ca0: 0000 7213 0000 00da 1347 6574 4465 6661  ..r......GetDefa
+00000cb0: 756c 7451 756f 7465 5479 7065 722c 0000  ultQuoteTyper,..
+00000cc0: 0072 3700 0000 7229 0000 0072 0600 0000  .r7...r)...r....
+00000cd0: 721f 0000 00da 0572 616e 6765 7239 0000  r......ranger9..
+00000ce0: 0072 0f00 0000 720d 0000 0072 3800 0000  .r....r....r8...
+00000cf0: 7224 0000 0029 0472 1600 0000 7233 0000  r$...).r....r3..
+00000d00: 00da 0b73 6f75 7263 655f 6c69 7374 da05  ...source_list..
+00000d10: 696e 6465 7872 1b00 0000 721b 0000 0072  indexr....r....r
+00000d20: 1c00 0000 721f 0000 0056 0000 0073 3c00  ....r....V...s<.
+00000d30: 0000 1802 0e01 1201 0a02 0601 0801 1402  ................
+00000d40: 0602 0a01 0c01 0a02 0601 0801 02ff 0601  ................
+00000d50: 04ff 1a02 0601 0601 0401 02fe 0602 04fe  ................
+00000d60: 0603 0c01 02ff 0601 06ff 0e03 0a01 7a1a  ..............z.
+00000d70: 5374 7253 6f75 7263 654d 6174 6368 6572  StrSourceMatcher
+00000d80: 2e47 6574 536f 7572 6365 6301 0000 0000  .GetSourcec.....
+00000d90: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000da0: 0000 0073 0e00 0000 7c00 6a00 6a01 7c00  ...s....|.j.j.|.
+00000db0: 5f02 6400 5300 721d 0000 0029 0372 1700  _.d.S.r....).r..
+00000dc0: 0000 7245 0000 0072 1400 0000 7222 0000  ..rE...r....r"..
+00000dd0: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000de0: 7227 0000 0073 0000 0073 0200 0000 0e01  r'...s...s......
+00000df0: 7a25 5374 7253 6f75 7263 654d 6174 6368  z%StrSourceMatch
+00000e00: 6572 2e5f 6765 745f 6f72 6967 696e 616c  er._get_original
+00000e10: 5f73 7472 696e 6763 0100 0000 0000 0000  _stringc........
+00000e20: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00000e30: 730a 0000 0074 007c 006a 0183 0153 0072  s....t.|.j...S.r
+00000e40: 1d00 0000 2902 7205 0000 0072 1500 0000  ....).r....r....
+00000e50: 7222 0000 0072 1b00 0000 721b 0000 0072  r"...r....r....r
+00000e60: 1c00 0000 7228 0000 0076 0000 0073 0200  ....r(...v...s..
+00000e70: 0000 0a01 7a23 5374 7253 6f75 7263 654d  ....z#StrSourceM
+00000e80: 6174 6368 6572 2e5f 7061 7274 5f70 6c61  atcher._part_pla
+00000e90: 6365 5f68 6f6c 6465 7229 024e 5429 0dda  ce_holder).NT)..
+00000ea0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000eb0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000ec0: 655f 5fda 075f 5f64 6f63 5f5f 720c 0000  e__..__doc__r...
+00000ed0: 0072 2500 0000 7236 0000 0072 2e00 0000  .r%...r6...r....
+00000ee0: 722a 0000 0072 1f00 0000 7227 0000 0072  r*...r....r'...r
+00000ef0: 2800 0000 da0d 5f5f 636c 6173 7363 656c  (.....__classcel
+00000f00: 6c5f 5f72 1b00 0000 721b 0000 0072 1900  l__r....r....r..
+00000f10: 0000 721c 0000 0072 0800 0000 0c00 0000  ..r....r........
+00000f20: 7314 0000 0008 0004 010e 0208 0f08 0408  s...............
+00000f30: 1208 1208 1008 1d10 0372 0800 0000 290e  .........r....).
+00000f40: 7240 0000 00da 2766 756e 5f77 6974 685f  r@....'fun_with_
+00000f50: 6173 742e 736f 7572 6365 5f6d 6174 6368  ast.source_match
+00000f60: 6572 732e 6578 6365 7074 696f 6e73 7202  ers.exceptionsr.
+00000f70: 0000 00da 2466 756e 5f77 6974 685f 6173  ....$fun_with_as
+00000f80: 742e 706c 6163 6568 6f6c 6465 7273 2e62  t.placeholders.b
+00000f90: 6173 655f 6d61 7463 6872 0300 0000 da29  ase_matchr.....)
+00000fa0: 6675 6e5f 7769 7468 5f61 7374 2e73 6f75  fun_with_ast.sou
+00000fb0: 7263 655f 6d61 7463 6865 7273 2e62 6173  rce_matchers.bas
+00000fc0: 655f 6d61 7463 6865 7272 0400 0000 da25  e_matcherr.....%
+00000fd0: 6675 6e5f 7769 7468 5f61 7374 2e70 6c61  fun_with_ast.pla
+00000fe0: 6365 686f 6c64 6572 732e 7374 7269 6e67  ceholders.string
+00000ff0: 5f70 6172 7472 0500 0000 da2c 6675 6e5f  _partr.....,fun_
+00001000: 7769 7468 5f61 7374 2e63 6f6d 6d6f 6e5f  with_ast.common_
+00001010: 7574 696c 732e 7574 696c 735f 736f 7572  utils.utils_sour
+00001020: 6365 5f6d 6174 6368 7206 0000 00da 1e66  ce_matchr......f
+00001030: 756e 5f77 6974 685f 6173 742e 706c 6163  un_with_ast.plac
+00001040: 6568 6f6c 6465 7273 2e74 6578 7472 0700  eholders.textr..
+00001050: 0000 7208 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00001060: 0072 1b00 0000 721c 0000 00da 083c 6d6f  .r....r......<mo
+00001070: 6475 6c65 3e01 0000 0073 1000 0000 0800  dule>....s......
+00001080: 0c02 0c02 0c01 0c01 0c01 0c01 1403       ..............
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/syntaxfreeline.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/syntaxfreeline.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat May 20 15:44:20 2023 UTC, .py size: 920 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d4ea 6864 9803 0000  o.........hd....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 6103 0000  o..........da...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6405 6406 8400 6406 6503 8303 5a08 6407  d.d...d.e...Z.d.
 00000070: 5300 2908 e900 0000 0029 01da 1046 6965  S.)......)...Fie
@@ -48,15 +48,15 @@
 000002f0: 745f 7768 6974 6573 7061 6365 5f6d 6174  t_whitespace_mat
 00000300: 6368 6572 73da 0661 7070 656e 6429 0372  chers..append).r
 00000310: 0b00 0000 da10 7265 6d61 696e 696e 675f  ......remaining_
 00000320: 7374 7269 6e67 da0e 7773 5f70 6c61 6365  string..ws_place
 00000330: 686f 6c64 6572 7213 0000 0072 1300 0000  holderr....r....
 00000340: 7214 0000 00da 104d 6174 6368 5768 6974  r......MatchWhit
 00000350: 6553 7061 6365 7310 0000 0073 0600 0000  eSpaces....s....
-00000360: 0601 0c02 0401 7a26 5379 6e74 6178 4672  ......z&SyntaxFr
+00000360: 0601 0c01 0401 7a26 5379 6e74 6178 4672  ......z&SyntaxFr
 00000370: 6565 4c69 6e65 4d61 7463 6865 722e 4d61  eeLineMatcher.Ma
 00000380: 7463 6857 6869 7465 5370 6163 6573 2902  tchWhiteSpaces).
 00000390: 4e4e 2907 da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
 000003a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 000003b0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
 000003c0: 5f72 0a00 0000 7219 0000 00da 0d5f 5f63  _r....r......__c
 000003d0: 6c61 7373 6365 6c6c 5f5f 7213 0000 0072  lasscell__r....r
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/tuple.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/tuple.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 11 17:15:13 2023 UTC, .py size: 1464 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2101 8664 b805 0000  o.......!..d....
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 1901 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6501 8303  ..G.d.d...d.e...
 00000060: 5a06 6406 5300 2907 e900 0000 0029 01da  Z.d.S.)......)..
 00000070: 1444 6566 6175 6c74 536f 7572 6365 4d61  .DefaultSourceMa
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/with_matcher.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/with_matcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun  5 19:14:37 2023 UTC, .py size: 3438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,156 @@
-00000000: 6f0d 0d0a 0000 0000 1d34 7e64 6e0d 0000  o........4~dn...
+00000000: 6f0d 0d0a 0000 0000 82ab aa64 790c 0000  o..........dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
+00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
-00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
-00000080: 6506 8303 5a0c 6401 5300 2909 e900 0000  e...Z.d.S.).....
-00000090: 004e 2901 da0f 426f 6479 506c 6163 6568  .N)...BodyPlaceh
-000000a0: 6f6c 6465 7229 01da 0947 6574 536f 7572  older)...GetSour
-000000b0: 6365 2902 da0d 536f 7572 6365 4d61 7463  ce)...SourceMatc
-000000c0: 6865 72da 144d 6174 6368 506c 6163 6568  her..MatchPlaceh
-000000d0: 6f6c 6465 724c 6973 7429 01da 0f54 6578  olderList)...Tex
-000000e0: 7450 6c61 6365 686f 6c64 6572 2901 da1d  tPlaceholder)...
-000000f0: 5365 7061 7261 7465 644c 6973 7446 6965  SeparatedListFie
-00000100: 6c64 506c 6163 6568 6f6c 6465 7263 0000  ldPlaceholderc..
-00000110: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000120: 0000 0000 0000 7332 0000 0065 005a 0164  ......s2...e.Z.d
-00000130: 005a 0264 015a 0364 0987 0066 0164 0364  .Z.d.Z.d...f.d.d
-00000140: 0484 095a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00000150: 0884 005a 0687 0004 005a 0753 0029 0ada  ...Z.....Z.S.)..
-00000160: 1157 6974 6853 6f75 7263 654d 6174 6368  .WithSourceMatch
-00000170: 6572 7a33 436c 6173 7320 746f 2067 656e  erz3Class to gen
-00000180: 6572 6174 6520 7468 6520 736f 7572 6365  erate the source
-00000190: 2066 6f72 2061 6e20 5f61 7374 2e57 6974   for an _ast.Wit
-000001a0: 6820 6e6f 6465 2e4e 6304 0000 0000 0000  h node.Nc.......
-000001b0: 0000 0000 0004 0000 0005 0000 0003 0000  ................
-000001c0: 0073 5800 0000 7400 7401 7c00 8302 a002  .sX...t.t.|.....
-000001d0: 7c01 7c02 a102 0100 7403 6401 6402 8302  |.|.....t.d.d...
-000001e0: 7c00 5f04 7405 6403 7403 6404 6405 8302  |._.t.d.t.d.d...
-000001f0: 6406 8d02 7c00 5f06 7403 6407 6408 8302  d...|._.t.d.d...
-00000200: 7c00 5f07 7408 6409 8301 7c00 5f09 640a  |._.t.d...|._.d.
-00000210: 7c00 5f0a 640b 7c00 5f0b 6400 5300 290c  |._.d.|._.d.S.).
-00000220: 4e7a 0b20 2a28 7769 7468 293f 202a 7a05  Nz. *(with)? *z.
-00000230: 7769 7468 20da 0569 7465 6d73 7a03 2c20  with ..itemsz., 
-00000240: 2a7a 022c 2029 01da 1c62 6566 6f72 655f  *z., )...before_
-00000250: 7365 7061 7261 746f 725f 706c 6163 6568  separator_placeh
-00000260: 6f6c 6465 727a 043a 5c6e 3f7a 023a 0ada  olderz.:\n?z.:..
-00000270: 0462 6f64 7946 5429 0cda 0573 7570 6572  .bodyFT)...super
-00000280: 7208 0000 00da 085f 5f69 6e69 745f 5f72  r......__init__r
-00000290: 0600 0000 da10 7769 7468 5f70 6c61 6365  ......with_place
-000002a0: 686f 6c64 6572 7207 0000 00da 1577 6974  holderr......wit
-000002b0: 6869 7465 6d73 5f70 6c61 6365 686f 6c64  hitems_placehold
-000002c0: 6572 da11 636f 6c6f 6e5f 706c 6163 6568  er..colon_placeh
-000002d0: 6f6c 6465 7272 0200 0000 da10 626f 6479  olderr......body
-000002e0: 5f70 6c61 6365 686f 6c64 6572 da10 6973  _placeholder..is
-000002f0: 5f63 6f6d 706f 756e 645f 7769 7468 da0d  _compound_with..
-00000300: 7374 6172 7469 6e67 5f77 6974 6829 04da  starting_with)..
-00000310: 0473 656c 66da 046e 6f64 65da 0f73 7461  .self..node..sta
-00000320: 7274 696e 675f 7061 7265 6e73 da06 5061  rting_parens..Pa
-00000330: 7265 6e74 a901 da09 5f5f 636c 6173 735f  rent....__class_
-00000340: 5fa9 00fa 442f 686f 6d65 2f73 6861 692f  _...D/home/shai/
-00000350: 6675 6e5f 7769 7468 5f61 7374 2f66 756e  fun_with_ast/fun
-00000360: 5f77 6974 685f 6173 742f 736f 7572 6365  _with_ast/source
-00000370: 5f6d 6174 6368 6572 732f 7769 7468 5f6d  _matchers/with_m
-00000380: 6174 6368 6572 2e70 7972 0d00 0000 0d00  atcher.pyr......
-00000390: 0000 730e 0000 0012 010c 0114 010c 060a  ..s.............
-000003a0: 0106 010a 017a 1a57 6974 6853 6f75 7263  .....z.WithSourc
-000003b0: 654d 6174 6368 6572 2e5f 5f69 6e69 745f  eMatcher.__init_
-000003c0: 5f63 0200 0000 0000 0000 0000 0000 0400  _c..............
-000003d0: 0000 0400 0000 4300 0000 7390 0000 007c  ......C...s....|
-000003e0: 01a0 00a1 00a0 0164 01a1 0172 0a64 027c  .......d...r.d.|
-000003f0: 005f 027c 006a 037c 006a 0467 027d 0274  ._.|.j.|.j.g.}.t
-00000400: 057c 017c 006a 067c 0283 037d 037c 03a0  .|.|.j.|...}.|..
-00000410: 00a1 00a0 0164 03a1 0172 2f64 027c 005f  .....d...r/d.|._
-00000420: 077c 006a 087c 006a 0967 027d 0274 057c  .|.j.|.j.g.}.t.|
-00000430: 037c 006a 067c 0283 037d 036e 0d7c 006a  .|.j.|...}.n.|.j
-00000440: 0a7c 006a 0967 027d 0274 057c 037c 006a  .|.j.g.}.t.|.|.j
-00000450: 067c 0283 037d 037c 0373 407c 0153 007c  .|...}.|.s@|.S.|
-00000460: 0164 0074 0b7c 0383 0185 0219 0053 0029  .d.t.|.......S.)
-00000470: 044e da04 7769 7468 54fa 012c 290c da06  .N..withT..,)...
-00000480: 6c73 7472 6970 da0a 7374 6172 7473 7769  lstrip..startswi
-00000490: 7468 7213 0000 0072 0e00 0000 720f 0000  thr....r....r...
-000004a0: 0072 0500 0000 7215 0000 0072 1200 0000  .r....r....r....
-000004b0: da12 636f 6d70 6f75 6e64 5f73 6570 6172  ..compound_separ
-000004c0: 6174 6f72 7211 0000 0072 1000 0000 da03  atorr....r......
-000004d0: 6c65 6e29 0472 1400 0000 da06 7374 7269  len).r......stri
-000004e0: 6e67 da10 706c 6163 6568 6f6c 6465 725f  ng..placeholder_
-000004f0: 6c69 7374 da10 7265 6d61 696e 696e 675f  list..remaining_
-00000500: 7374 7269 6e67 721a 0000 0072 1a00 0000  stringr....r....
-00000510: 721b 0000 00da 065f 6d61 7463 681b 0000  r......_match...
-00000520: 0073 3200 0000 0e01 0601 0401 0401 04ff  .s2.............
-00000530: 0202 0801 04ff 0e02 0601 0401 0401 04ff  ................
-00000540: 0202 0801 06ff 0403 0401 04ff 0202 0801  ................
-00000550: 04ff 0403 0401 1001 7a18 5769 7468 536f  ........z.WithSo
-00000560: 7572 6365 4d61 7463 6865 722e 5f6d 6174  urceMatcher._mat
-00000570: 6368 6301 0000 0000 0000 0000 0000 0003  chc.............
-00000580: 0000 0004 0000 0003 0000 0073 b400 0000  ...........s....
-00000590: 6700 7d01 8800 6a00 720b 7c01 a001 8800  g.}...j.r.|.....
-000005a0: 6a02 a101 0100 7c01 a001 8800 6a03 a101  j.....|.....j...
-000005b0: 0100 8800 6a04 7240 7405 8800 6a06 6a07  ....j.r@t...j.j.
-000005c0: 6401 1900 7408 6a09 8302 7240 740a 8800  d...t.j...r@t...
-000005d0: 6a06 6a07 6401 1900 6402 8302 7331 740b  j.j.d...d...s1t.
-000005e0: 8800 6a06 6a07 6401 1900 6403 6404 8d02  ..j.j.d...d.d...
-000005f0: 0100 6405 8800 6a06 6a07 6401 1900 6a0c  ..d...j.j.d...j.
-00000600: 5f00 7c01 a001 8800 6a0d a101 0100 6e06  _.|.....j.....n.
-00000610: 7c01 a001 8800 6a0e a101 0100 7c01 a001  |.....j.....|...
-00000620: 8800 6a0f a101 0100 8700 6601 6406 6407  ..j.......f.d.d.
-00000630: 8408 7c01 4400 8301 7d02 6408 a010 7c02  ..|.D...}.d...|.
-00000640: a101 5300 2909 4e72 0100 0000 da07 6d61  ..S.).Nr......ma
-00000650: 7463 6865 7254 2901 da10 6173 7375 6d65  tcherT)...assume
-00000660: 5f6e 6f5f 696e 6465 6e74 4663 0100 0000  _no_indentFc....
-00000670: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000680: 1300 0000 7318 0000 0067 007c 005d 087d  ....s....g.|.].}
-00000690: 017c 01a0 0088 006a 01a1 0191 0271 0253  .|.....j.....q.S
-000006a0: 0072 1a00 0000 2902 7203 0000 0072 1500  .r....).r....r..
-000006b0: 0000 2902 da02 2e30 da01 70a9 0172 1400  ..)....0..p..r..
-000006c0: 0000 721a 0000 0072 1b00 0000 da0a 3c6c  ..r....r......<l
-000006d0: 6973 7463 6f6d 703e 4700 0000 7302 0000  istcomp>G...s...
-000006e0: 0018 007a 2f57 6974 6853 6f75 7263 654d  ...z/WithSourceM
-000006f0: 6174 6368 6572 2e47 6574 536f 7572 6365  atcher.GetSource
-00000700: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00000710: 6f6d 703e da00 2911 7213 0000 00da 0661  omp>..).r......a
-00000720: 7070 656e 6472 0e00 0000 720f 0000 0072  ppendr....r....r
-00000730: 1200 0000 da0a 6973 696e 7374 616e 6365  ......isinstance
-00000740: 7215 0000 0072 0b00 0000 da04 5f61 7374  r....r......_ast
-00000750: da04 5769 7468 da07 6861 7361 7474 7272  ..With..hasattrr
-00000760: 0300 0000 7226 0000 0072 2000 0000 7210  ....r&...r ...r.
-00000770: 0000 0072 1100 0000 da04 6a6f 696e 2903  ...r......join).
-00000780: 7214 0000 0072 2300 0000 da0b 736f 7572  r....r#.....sour
-00000790: 6365 5f6c 6973 7472 1a00 0000 722a 0000  ce_listr....r*..
-000007a0: 0072 1b00 0000 7203 0000 0032 0000 0073  .r....r....2...s
-000007b0: 1e00 0000 0401 0601 0c01 0c01 0602 1201  ................
-000007c0: 02ff 1202 1403 1003 0e01 0c03 0c01 1202  ................
-000007d0: 0a01 7a1b 5769 7468 536f 7572 6365 4d61  ..z.WithSourceMa
-000007e0: 7463 6865 722e 4765 7453 6f75 7263 6529  tcher.GetSource)
-000007f0: 024e 4e29 08da 085f 5f6e 616d 655f 5fda  .NN)...__name__.
-00000800: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000810: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-00000820: 5f5f 720d 0000 0072 2500 0000 7203 0000  __r....r%...r...
-00000830: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000840: 721a 0000 0072 1a00 0000 7218 0000 0072  r....r....r....r
-00000850: 1b00 0000 7208 0000 000a 0000 0073 0a00  ....r........s..
-00000860: 0000 0800 0401 0e02 080e 1017 7208 0000  ............r...
-00000870: 0029 0d72 2f00 0000 da21 6675 6e5f 7769  .).r/....!fun_wi
-00000880: 7468 5f61 7374 2e73 6f75 7263 655f 6d61  th_ast.source_ma
-00000890: 7463 6865 7273 2e62 6f64 7972 0200 0000  tchers.bodyr....
-000008a0: da17 6675 6e5f 7769 7468 5f61 7374 2e67  ..fun_with_ast.g
-000008b0: 6574 5f73 6f75 7263 6572 0300 0000 da29  et_sourcer.....)
-000008c0: 6675 6e5f 7769 7468 5f61 7374 2e73 6f75  fun_with_ast.sou
-000008d0: 7263 655f 6d61 7463 6865 7273 2e62 6173  rce_matchers.bas
-000008e0: 655f 6d61 7463 6865 7272 0400 0000 7205  e_matcherr....r.
-000008f0: 0000 00da 1e66 756e 5f77 6974 685f 6173  .....fun_with_as
-00000900: 742e 706c 6163 6568 6f6c 6465 7273 2e74  t.placeholders.t
-00000910: 6578 7472 0600 0000 da2a 6675 6e5f 7769  extr.....*fun_wi
-00000920: 7468 5f61 7374 2e70 6c61 6365 686f 6c64  th_ast.placehold
-00000930: 6572 732e 6c69 7374 5f70 6c61 6365 686f  ers.list_placeho
-00000940: 6c64 6572 7207 0000 0072 0800 0000 721a  lderr....r....r.
-00000950: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00000960: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000970: 730e 0000 0008 000c 020c 0110 010c 010c  s...............
-00000980: 0114 03                                  ...
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 4700  ..d.d.l.m.Z...G.
+00000080: 6408 6409 8400 6409 6506 8303 5a0d 6401  d.d...d.e...Z.d.
+00000090: 5300 290a e900 0000 004e 2901 da0f 426f  S.)......N)...Bo
+000000a0: 6479 506c 6163 6568 6f6c 6465 7229 01da  dyPlaceholder)..
+000000b0: 0947 6574 536f 7572 6365 2901 da0d 536f  .GetSource)...So
+000000c0: 7572 6365 4d61 7463 6865 7229 01da 144d  urceMatcher)...M
+000000d0: 6174 6368 506c 6163 6568 6f6c 6465 724c  atchPlaceholderL
+000000e0: 6973 7429 01da 0f54 6578 7450 6c61 6365  ist)...TextPlace
+000000f0: 686f 6c64 6572 2901 da1d 5365 7061 7261  holder)...Separa
+00000100: 7465 644c 6973 7446 6965 6c64 506c 6163  tedListFieldPlac
+00000110: 6568 6f6c 6465 7263 0000 0000 0000 0000  eholderc........
+00000120: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00000130: 7332 0000 0065 005a 0164 005a 0264 015a  s2...e.Z.d.Z.d.Z
+00000140: 0364 0987 0066 0164 0364 0484 095a 0464  .d...f.d.d...Z.d
+00000150: 0564 0684 005a 0564 0764 0884 005a 0687  .d...Z.d.d...Z..
+00000160: 0004 005a 0753 0029 0ada 1157 6974 6853  ...Z.S.)...WithS
+00000170: 6f75 7263 654d 6174 6368 6572 7a33 436c  ourceMatcherz3Cl
+00000180: 6173 7320 746f 2067 656e 6572 6174 6520  ass to generate 
+00000190: 7468 6520 736f 7572 6365 2066 6f72 2061  the source for a
+000001a0: 6e20 5f61 7374 2e57 6974 6820 6e6f 6465  n _ast.With node
+000001b0: 2e4e 6304 0000 0000 0000 0000 0000 0004  .Nc.............
+000001c0: 0000 0005 0000 0003 0000 0073 5800 0000  ...........sX...
+000001d0: 7400 7401 7c00 8302 a002 7c01 7c02 a102  t.t.|.....|.|...
+000001e0: 0100 7403 6401 6402 8302 7c00 5f04 7405  ..t.d.d...|._.t.
+000001f0: 6403 7403 6404 6405 8302 6406 8d02 7c00  d.t.d.d...d...|.
+00000200: 5f06 7403 6407 6408 8302 7c00 5f07 7408  _.t.d.d...|._.t.
+00000210: 6409 8301 7c00 5f09 640a 7c00 5f0a 640b  d...|._.d.|._.d.
+00000220: 7c00 5f0b 6400 5300 290c 4e7a 0b20 2a28  |._.d.S.).Nz. *(
+00000230: 7769 7468 293f 202a 7a05 7769 7468 20da  with)? *z.with .
+00000240: 0569 7465 6d73 7a03 2c20 2a7a 022c 2029  .itemsz., *z., )
+00000250: 01da 1c62 6566 6f72 655f 7365 7061 7261  ...before_separa
+00000260: 746f 725f 706c 6163 6568 6f6c 6465 727a  tor_placeholderz
+00000270: 043a 5c6e 3f7a 023a 0ada 0462 6f64 7946  .:\n?z.:...bodyF
+00000280: 5429 0cda 0573 7570 6572 7208 0000 00da  T)...superr.....
+00000290: 085f 5f69 6e69 745f 5f72 0600 0000 da10  .__init__r......
+000002a0: 7769 7468 5f70 6c61 6365 686f 6c64 6572  with_placeholder
+000002b0: 7207 0000 00da 1577 6974 6869 7465 6d73  r......withitems
+000002c0: 5f70 6c61 6365 686f 6c64 6572 da11 636f  _placeholder..co
+000002d0: 6c6f 6e5f 706c 6163 6568 6f6c 6465 7272  lon_placeholderr
+000002e0: 0200 0000 da10 626f 6479 5f70 6c61 6365  ......body_place
+000002f0: 686f 6c64 6572 da10 6973 5f63 6f6d 706f  holder..is_compo
+00000300: 756e 645f 7769 7468 da0d 7374 6172 7469  und_with..starti
+00000310: 6e67 5f77 6974 6829 04da 0473 656c 66da  ng_with)...self.
+00000320: 046e 6f64 65da 0f73 7461 7274 696e 675f  .node..starting_
+00000330: 7061 7265 6e73 da06 5061 7265 6e74 a901  parens..Parent..
+00000340: da09 5f5f 636c 6173 735f 5fa9 00fa 442f  ..__class__...D/
+00000350: 686f 6d65 2f73 6861 692f 6675 6e5f 7769  home/shai/fun_wi
+00000360: 7468 5f61 7374 2f66 756e 5f77 6974 685f  th_ast/fun_with_
+00000370: 6173 742f 736f 7572 6365 5f6d 6174 6368  ast/source_match
+00000380: 6572 732f 7769 7468 5f6d 6174 6368 6572  ers/with_matcher
+00000390: 2e70 7972 0d00 0000 0e00 0000 730e 0000  .pyr........s...
+000003a0: 0012 010c 0114 010c 010a 0106 010a 017a  ...............z
+000003b0: 1a57 6974 6853 6f75 7263 654d 6174 6368  .WithSourceMatch
+000003c0: 6572 2e5f 5f69 6e69 745f 5f63 0200 0000  er.__init__c....
+000003d0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+000003e0: 4300 0000 7390 0000 007c 01a0 00a1 00a0  C...s....|......
+000003f0: 0164 01a1 0172 0a64 027c 005f 027c 006a  .d...r.d.|._.|.j
+00000400: 037c 006a 0467 027d 0274 057c 017c 006a  .|.j.g.}.t.|.|.j
+00000410: 067c 0283 037d 037c 03a0 00a1 00a0 0164  .|...}.|.......d
+00000420: 03a1 0172 2f64 027c 005f 077c 006a 087c  ...r/d.|._.|.j.|
+00000430: 006a 0967 027d 0274 057c 037c 006a 067c  .j.g.}.t.|.|.j.|
+00000440: 0283 037d 036e 0d7c 006a 0a7c 006a 0967  ...}.n.|.j.|.j.g
+00000450: 027d 0274 057c 037c 006a 067c 0283 037d  .}.t.|.|.j.|...}
+00000460: 037c 0373 407c 0153 007c 0164 0074 0b7c  .|.s@|.S.|.d.t.|
+00000470: 0383 0185 0219 0053 0029 044e da04 7769  .......S.).N..wi
+00000480: 7468 54fa 012c 290c da06 6c73 7472 6970  thT..,)...lstrip
+00000490: da0a 7374 6172 7473 7769 7468 7213 0000  ..startswithr...
+000004a0: 0072 0e00 0000 720f 0000 0072 0500 0000  .r....r....r....
+000004b0: 7215 0000 0072 1200 0000 da12 636f 6d70  r....r......comp
+000004c0: 6f75 6e64 5f73 6570 6172 6174 6f72 7211  ound_separatorr.
+000004d0: 0000 0072 1000 0000 da03 6c65 6e29 0472  ...r......len).r
+000004e0: 1400 0000 da06 7374 7269 6e67 da10 706c  ......string..pl
+000004f0: 6163 6568 6f6c 6465 725f 6c69 7374 da10  aceholder_list..
+00000500: 7265 6d61 696e 696e 675f 7374 7269 6e67  remaining_string
+00000510: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00000520: 065f 6d61 7463 6817 0000 0073 3200 0000  ._match....s2...
+00000530: 0e01 0601 0401 0401 04ff 0202 0801 04ff  ................
+00000540: 0e02 0601 0401 0401 04ff 0202 0801 06ff  ................
+00000550: 0403 0401 04ff 0202 0801 04ff 0403 0401  ................
+00000560: 1001 7a18 5769 7468 536f 7572 6365 4d61  ..z.WithSourceMa
+00000570: 7463 6865 722e 5f6d 6174 6368 6301 0000  tcher._matchc...
+00000580: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00000590: 0003 0000 0073 b400 0000 6700 7d01 8800  .....s....g.}...
+000005a0: 6a00 720b 7c01 a001 8800 6a02 a101 0100  j.r.|.....j.....
+000005b0: 7c01 a001 8800 6a03 a101 0100 8800 6a04  |.....j.......j.
+000005c0: 7240 7405 8800 6a06 6a07 6401 1900 7408  r@t...j.j.d...t.
+000005d0: 6a09 8302 7240 740a 8800 6a06 6a07 6401  j...r@t...j.j.d.
+000005e0: 1900 6402 8302 7331 740b 8800 6a06 6a07  ..d...s1t...j.j.
+000005f0: 6401 1900 6403 6404 8d02 0100 6405 8800  d...d.d.....d...
+00000600: 6a06 6a07 6401 1900 6a0c 5f00 7c01 a001  j.j.d...j._.|...
+00000610: 8800 6a0d a101 0100 6e06 7c01 a001 8800  ..j.....n.|.....
+00000620: 6a0e a101 0100 7c01 a001 8800 6a0f a101  j.....|.....j...
+00000630: 0100 8700 6601 6406 6407 8408 7c01 4400  ....f.d.d...|.D.
+00000640: 8301 7d02 6408 a010 7c02 a101 5300 2909  ..}.d...|...S.).
+00000650: 4e72 0100 0000 da07 6d61 7463 6865 7254  Nr......matcherT
+00000660: 2901 da10 6173 7375 6d65 5f6e 6f5f 696e  )...assume_no_in
+00000670: 6465 6e74 4663 0100 0000 0000 0000 0000  dentFc..........
+00000680: 0000 0200 0000 0500 0000 1300 0000 7318  ..............s.
+00000690: 0000 0067 007c 005d 087d 017c 01a0 0088  ...g.|.].}.|....
+000006a0: 006a 01a1 0191 0271 0253 0072 1a00 0000  .j.....q.S.r....
+000006b0: 2902 7203 0000 0072 1500 0000 2902 da02  ).r....r....)...
+000006c0: 2e30 da01 70a9 0172 1400 0000 721a 0000  .0..p..r....r...
+000006d0: 0072 1b00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+000006e0: 703e 4300 0000 7302 0000 0018 007a 2f57  p>C...s......z/W
+000006f0: 6974 6853 6f75 7263 654d 6174 6368 6572  ithSourceMatcher
+00000700: 2e47 6574 536f 7572 6365 2e3c 6c6f 6361  .GetSource.<loca
+00000710: 6c73 3e2e 3c6c 6973 7463 6f6d 703e da00  ls>.<listcomp>..
+00000720: 2911 7213 0000 00da 0661 7070 656e 6472  ).r......appendr
+00000730: 0e00 0000 720f 0000 0072 1200 0000 da0a  ....r....r......
+00000740: 6973 696e 7374 616e 6365 7215 0000 0072  isinstancer....r
+00000750: 0b00 0000 da04 5f61 7374 da04 5769 7468  ......_ast..With
+00000760: da07 6861 7361 7474 7272 0300 0000 7226  ..hasattrr....r&
+00000770: 0000 0072 2000 0000 7210 0000 0072 1100  ...r ...r....r..
+00000780: 0000 da04 6a6f 696e 2903 7214 0000 0072  ....join).r....r
+00000790: 2300 0000 da0b 736f 7572 6365 5f6c 6973  #.....source_lis
+000007a0: 7472 1a00 0000 722a 0000 0072 1b00 0000  tr....r*...r....
+000007b0: 7203 0000 002e 0000 0073 1e00 0000 0401  r........s......
+000007c0: 0601 0c01 0c01 0602 1201 02ff 1202 1403  ................
+000007d0: 1003 0e01 0c03 0c01 1202 0a01 7a1b 5769  ............z.Wi
+000007e0: 7468 536f 7572 6365 4d61 7463 6865 722e  thSourceMatcher.
+000007f0: 4765 7453 6f75 7263 6529 024e 4e29 08da  GetSource).NN)..
+00000800: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000810: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000820: 655f 5fda 075f 5f64 6f63 5f5f 720d 0000  e__..__doc__r...
+00000830: 0072 2500 0000 7203 0000 00da 0d5f 5f63  .r%...r......__c
+00000840: 6c61 7373 6365 6c6c 5f5f 721a 0000 0072  lasscell__r....r
+00000850: 1a00 0000 7218 0000 0072 1b00 0000 7208  ....r....r....r.
+00000860: 0000 000b 0000 0073 0a00 0000 0800 0401  .......s........
+00000870: 0e02 0809 1017 7208 0000 0029 0e72 2f00  ......r....).r/.
+00000880: 0000 da21 6675 6e5f 7769 7468 5f61 7374  ...!fun_with_ast
+00000890: 2e73 6f75 7263 655f 6d61 7463 6865 7273  .source_matchers
+000008a0: 2e62 6f64 7972 0200 0000 da17 6675 6e5f  .bodyr......fun_
+000008b0: 7769 7468 5f61 7374 2e67 6574 5f73 6f75  with_ast.get_sou
+000008c0: 7263 6572 0300 0000 da29 6675 6e5f 7769  rcer.....)fun_wi
+000008d0: 7468 5f61 7374 2e73 6f75 7263 655f 6d61  th_ast.source_ma
+000008e0: 7463 6865 7273 2e62 6173 655f 6d61 7463  tchers.base_matc
+000008f0: 6865 7272 0400 0000 da24 6675 6e5f 7769  herr.....$fun_wi
+00000900: 7468 5f61 7374 2e70 6c61 6365 686f 6c64  th_ast.placehold
+00000910: 6572 732e 6261 7365 5f6d 6174 6368 7205  ers.base_matchr.
+00000920: 0000 00da 1e66 756e 5f77 6974 685f 6173  .....fun_with_as
+00000930: 742e 706c 6163 6568 6f6c 6465 7273 2e74  t.placeholders.t
+00000940: 6578 7472 0600 0000 da2a 6675 6e5f 7769  extr.....*fun_wi
+00000950: 7468 5f61 7374 2e70 6c61 6365 686f 6c64  th_ast.placehold
+00000960: 6572 732e 6c69 7374 5f70 6c61 6365 686f  ers.list_placeho
+00000970: 6c64 6572 7207 0000 0072 0800 0000 721a  lderr....r....r.
+00000980: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
+00000990: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000009a0: 7310 0000 0008 000c 020c 010c 010c 010c  s...............
+000009b0: 010c 0114 03                             .....
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/__pycache__/withitem.cpython-310.pyc` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/__pycache__/withitem.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 05:22:34 2023 UTC, .py size: 1303 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,103 @@
-00000000: 6f0d 0d0a 0000 0000 1a14 8064 1705 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 8e17 a964 4705 0000  o..........dG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
-00000060: 6505 8303 5a07 6406 5300 2907 e900 0000  e...Z.d.S.).....
-00000070: 0029 01da 1046 6965 6c64 506c 6163 6568  .)...FieldPlaceh
-00000080: 6f6c 6465 7229 01da 0f54 6578 7450 6c61  older)...TextPla
-00000090: 6365 686f 6c64 6572 2902 da0d 536f 7572  ceholder)...Sour
-000000a0: 6365 4d61 7463 6865 72da 144d 6174 6368  ceMatcher..Match
-000000b0: 506c 6163 6568 6f6c 6465 724c 6973 7463  PlaceholderListc
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000d0: 0400 0000 0000 0000 732e 0000 0065 005a  ........s....e.Z
-000000e0: 0164 005a 0264 0887 0066 0164 0264 0384  .d.Z.d...f.d.d..
-000000f0: 095a 0364 0464 0584 005a 0464 0664 0784  .Z.d.d...Z.d.d..
-00000100: 005a 0587 0004 005a 0653 0029 09da 1557  .Z.....Z.S.)...W
-00000110: 6974 6849 7465 6d53 6f75 7263 654d 6174  ithItemSourceMat
-00000120: 6368 6572 4e63 0400 0000 0000 0000 0000  cherNc..........
-00000130: 0000 0400 0000 0500 0000 0300 0000 7334  ..............s4
-00000140: 0000 0074 0074 017c 0083 02a0 027c 017c  ...t.t.|.....|.|
-00000150: 02a1 0201 0074 0364 0183 017c 005f 0474  .....t.d...|._.t
-00000160: 0364 0274 0564 0364 0483 0264 058d 027c  .d.t.d.d...d...|
-00000170: 005f 0664 0053 0029 064e da0c 636f 6e74  ._.d.S.).N..cont
-00000180: 6578 745f 6578 7072 da0d 6f70 7469 6f6e  ext_expr..option
-00000190: 616c 5f76 6172 737a 0620 2a61 7320 2a7a  al_varsz. *as *z
-000001a0: 0420 6173 2029 01da 1262 6566 6f72 655f  . as )...before_
-000001b0: 706c 6163 6568 6f6c 6465 7229 07da 0573  placeholder)...s
-000001c0: 7570 6572 7206 0000 00da 085f 5f69 6e69  uperr......__ini
-000001d0: 745f 5f72 0200 0000 7207 0000 0072 0300  t__r....r....r..
-000001e0: 0000 7208 0000 0029 04da 0473 656c 66da  ..r....)...self.
-000001f0: 046e 6f64 65da 0f73 7461 7274 696e 675f  .node..starting_
-00000200: 7061 7265 6e73 da06 7061 7265 6e74 a901  parens..parent..
-00000210: da09 5f5f 636c 6173 735f 5fa9 00fa 402f  ..__class__...@/
-00000220: 686f 6d65 2f73 6861 692f 6675 6e5f 7769  home/shai/fun_wi
-00000230: 7468 5f61 7374 2f66 756e 5f77 6974 685f  th_ast/fun_with_
-00000240: 6173 742f 736f 7572 6365 5f6d 6174 6368  ast/source_match
-00000250: 6572 732f 7769 7468 6974 656d 2e70 7972  ers/withitem.pyr
-00000260: 0b00 0000 0700 0000 730c 0000 0012 010a  ........s.......
-00000270: 0102 0102 0108 010c fe7a 1e57 6974 6849  .........z.WithI
-00000280: 7465 6d53 6f75 7263 654d 6174 6368 6572  temSourceMatcher
-00000290: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
-000002a0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-000002b0: 0000 7332 0000 007c 006a 007c 006a 0167  ..s2...|.j.|.j.g
-000002c0: 027d 0274 027c 017c 006a 037c 0283 037d  .}.t.|.|.j.|...}
-000002d0: 037c 0373 117c 0153 007c 0164 0074 047c  .|.s.|.S.|.d.t.|
-000002e0: 0383 0185 0219 0053 0029 014e 2905 7207  .......S.).N).r.
-000002f0: 0000 0072 0800 0000 7205 0000 0072 0d00  ...r....r....r..
-00000300: 0000 da03 6c65 6e29 0472 0c00 0000 da06  ....len).r......
-00000310: 7374 7269 6e67 da10 706c 6163 6568 6f6c  string..placehol
-00000320: 6465 725f 6c69 7374 da10 7265 6d61 696e  der_list..remain
-00000330: 696e 675f 7374 7269 6e67 7212 0000 0072  ing_stringr....r
-00000340: 1200 0000 7213 0000 00da 065f 6d61 7463  ....r......_matc
-00000350: 680f 0000 0073 1200 0000 0403 0401 04ff  h....s..........
-00000360: 0202 0801 04ff 0403 0401 1001 7a1c 5769  ............z.Wi
-00000370: 7468 4974 656d 536f 7572 6365 4d61 7463  thItemSourceMatc
-00000380: 6865 722e 5f6d 6174 6368 6301 0000 0000  her._matchc.....
-00000390: 0000 0000 0000 0003 0000 0003 0000 0003  ................
-000003a0: 0000 0073 2c00 0000 6700 7d01 8800 6a00  ...s,...g.}...j.
-000003b0: 8800 6a01 6702 7d02 8700 6601 6401 6402  ..j.g.}...f.d.d.
-000003c0: 8408 7c02 4400 8301 7d01 6403 a002 7c01  ..|.D...}.d...|.
-000003d0: a101 5300 2904 4e63 0100 0000 0000 0000  ..S.).Nc........
-000003e0: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-000003f0: 7318 0000 0067 007c 005d 087d 017c 01a0  s....g.|.].}.|..
-00000400: 0088 006a 01a1 0191 0271 0253 0072 1200  ...j.....q.S.r..
-00000410: 0000 2902 da09 4765 7453 6f75 7263 6572  ..)...GetSourcer
-00000420: 0d00 0000 2902 da02 2e30 da01 70a9 0172  ....)....0..p..r
-00000430: 0c00 0000 7212 0000 0072 1300 0000 da0a  ....r....r......
-00000440: 3c6c 6973 7463 6f6d 703e 1f00 0000 7302  <listcomp>....s.
-00000450: 0000 0018 007a 3357 6974 6849 7465 6d53  .....z3WithItemS
-00000460: 6f75 7263 654d 6174 6368 6572 2e47 6574  ourceMatcher.Get
-00000470: 536f 7572 6365 2e3c 6c6f 6361 6c73 3e2e  Source.<locals>.
-00000480: 3c6c 6973 7463 6f6d 703e da00 2903 7207  <listcomp>..).r.
-00000490: 0000 0072 0800 0000 da04 6a6f 696e 2903  ...r......join).
-000004a0: 720c 0000 00da 0b73 6f75 7263 655f 6c69  r......source_li
-000004b0: 7374 7216 0000 0072 1200 0000 721c 0000  str....r....r...
-000004c0: 0072 1300 0000 7219 0000 001b 0000 0073  .r....r........s
-000004d0: 0c00 0000 0401 0401 0401 04ff 1202 0a01  ................
-000004e0: 7a1f 5769 7468 4974 656d 536f 7572 6365  z.WithItemSource
-000004f0: 4d61 7463 6865 722e 4765 7453 6f75 7263  Matcher.GetSourc
-00000500: 6529 024e 4e29 07da 085f 5f6e 616d 655f  e).NN)...__name_
-00000510: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000520: 5f71 7561 6c6e 616d 655f 5f72 0b00 0000  _qualname__r....
-00000530: 7218 0000 0072 1900 0000 da0d 5f5f 636c  r....r......__cl
-00000540: 6173 7363 656c 6c5f 5f72 1200 0000 7212  asscell__r....r.
-00000550: 0000 0072 1000 0000 7213 0000 0072 0600  ...r....r....r..
-00000560: 0000 0600 0000 7308 0000 0008 000e 0108  ......s.........
-00000570: 0810 0c72 0600 0000 4e29 08da 2366 756e  ...r....N)..#fun
-00000580: 5f77 6974 685f 6173 742e 706c 6163 6568  _with_ast.placeh
-00000590: 6f6c 6465 7273 2e63 6f6d 706f 7369 7465  olders.composite
-000005a0: 7202 0000 00da 1e66 756e 5f77 6974 685f  r......fun_with_
-000005b0: 6173 742e 706c 6163 6568 6f6c 6465 7273  ast.placeholders
-000005c0: 2e74 6578 7472 0300 0000 da29 6675 6e5f  .textr.....)fun_
-000005d0: 7769 7468 5f61 7374 2e73 6f75 7263 655f  with_ast.source_
-000005e0: 6d61 7463 6865 7273 2e62 6173 655f 6d61  matchers.base_ma
-000005f0: 7463 6865 7272 0400 0000 7205 0000 0072  tcherr....r....r
-00000600: 0600 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
-00000610: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000620: 653e 0100 0000 7308 0000 000c 000c 0110  e>....s.........
-00000630: 0114 03                                  ...
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
+00000060: 6405 6406 8400 6406 6505 8303 5a08 6407  d.d...d.e...Z.d.
+00000070: 5300 2908 e900 0000 0029 01da 1046 6965  S.)......)...Fie
+00000080: 6c64 506c 6163 6568 6f6c 6465 7229 01da  ldPlaceholder)..
+00000090: 0f54 6578 7450 6c61 6365 686f 6c64 6572  .TextPlaceholder
+000000a0: 2901 da0d 536f 7572 6365 4d61 7463 6865  )...SourceMatche
+000000b0: 7229 01da 144d 6174 6368 506c 6163 6568  r)...MatchPlaceh
+000000c0: 6f6c 6465 724c 6973 7463 0000 0000 0000  olderListc......
+000000d0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+000000e0: 0000 732e 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000000f0: 0887 0066 0164 0264 0384 095a 0364 0464  ...f.d.d...Z.d.d
+00000100: 0584 005a 0464 0664 0784 005a 0587 0004  ...Z.d.d...Z....
+00000110: 005a 0653 0029 09da 1557 6974 6849 7465  .Z.S.)...WithIte
+00000120: 6d53 6f75 7263 654d 6174 6368 6572 4e63  mSourceMatcherNc
+00000130: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+00000140: 0500 0000 0300 0000 7334 0000 0074 0074  ........s4...t.t
+00000150: 017c 0083 02a0 027c 017c 02a1 0201 0074  .|.....|.|.....t
+00000160: 0364 0183 017c 005f 0474 0364 0274 0564  .d...|._.t.d.t.d
+00000170: 0364 0483 0264 058d 027c 005f 0664 0053  .d...d...|._.d.S
+00000180: 0029 064e da0c 636f 6e74 6578 745f 6578  .).N..context_ex
+00000190: 7072 da0d 6f70 7469 6f6e 616c 5f76 6172  pr..optional_var
+000001a0: 737a 0620 2a61 7320 2a7a 0420 6173 2029  sz. *as *z. as )
+000001b0: 01da 1262 6566 6f72 655f 706c 6163 6568  ...before_placeh
+000001c0: 6f6c 6465 7229 07da 0573 7570 6572 7206  older)...superr.
+000001d0: 0000 00da 085f 5f69 6e69 745f 5f72 0200  .....__init__r..
+000001e0: 0000 7207 0000 0072 0300 0000 7208 0000  ..r....r....r...
+000001f0: 0029 04da 0473 656c 66da 046e 6f64 65da  .)...self..node.
+00000200: 0f73 7461 7274 696e 675f 7061 7265 6e73  .starting_parens
+00000210: da06 7061 7265 6e74 a901 da09 5f5f 636c  ..parent....__cl
+00000220: 6173 735f 5fa9 00fa 402f 686f 6d65 2f73  ass__...@/home/s
+00000230: 6861 692f 6675 6e5f 7769 7468 5f61 7374  hai/fun_with_ast
+00000240: 2f66 756e 5f77 6974 685f 6173 742f 736f  /fun_with_ast/so
+00000250: 7572 6365 5f6d 6174 6368 6572 732f 7769  urce_matchers/wi
+00000260: 7468 6974 656d 2e70 7972 0b00 0000 0800  thitem.pyr......
+00000270: 0000 730c 0000 0012 010a 0102 0102 0108  ..s.............
+00000280: 010c fe7a 1e57 6974 6849 7465 6d53 6f75  ...z.WithItemSou
+00000290: 7263 654d 6174 6368 6572 2e5f 5f69 6e69  rceMatcher.__ini
+000002a0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+000002b0: 0400 0000 0400 0000 4300 0000 7332 0000  ........C...s2..
+000002c0: 007c 006a 007c 006a 0167 027d 0274 027c  .|.j.|.j.g.}.t.|
+000002d0: 017c 006a 037c 0283 037d 037c 0373 117c  .|.j.|...}.|.s.|
+000002e0: 0153 007c 0164 0074 047c 0383 0185 0219  .S.|.d.t.|......
+000002f0: 0053 0029 014e 2905 7207 0000 0072 0800  .S.).N).r....r..
+00000300: 0000 7205 0000 0072 0d00 0000 da03 6c65  ..r....r......le
+00000310: 6e29 0472 0c00 0000 da06 7374 7269 6e67  n).r......string
+00000320: da10 706c 6163 6568 6f6c 6465 725f 6c69  ..placeholder_li
+00000330: 7374 da10 7265 6d61 696e 696e 675f 7374  st..remaining_st
+00000340: 7269 6e67 7212 0000 0072 1200 0000 7213  ringr....r....r.
+00000350: 0000 00da 065f 6d61 7463 6810 0000 0073  ....._match....s
+00000360: 1200 0000 0403 0401 04ff 0202 0801 04ff  ................
+00000370: 0403 0401 1001 7a1c 5769 7468 4974 656d  ......z.WithItem
+00000380: 536f 7572 6365 4d61 7463 6865 722e 5f6d  SourceMatcher._m
+00000390: 6174 6368 6301 0000 0000 0000 0000 0000  atchc...........
+000003a0: 0003 0000 0003 0000 0003 0000 0073 2c00  .............s,.
+000003b0: 0000 6700 7d01 8800 6a00 8800 6a01 6702  ..g.}...j...j.g.
+000003c0: 7d02 8700 6601 6401 6402 8408 7c02 4400  }...f.d.d...|.D.
+000003d0: 8301 7d01 6403 a002 7c01 a101 5300 2904  ..}.d...|...S.).
+000003e0: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+000003f0: 0000 0500 0000 1300 0000 7318 0000 0067  ..........s....g
+00000400: 007c 005d 087d 017c 01a0 0088 006a 01a1  .|.].}.|.....j..
+00000410: 0191 0271 0253 0072 1200 0000 2902 da09  ...q.S.r....)...
+00000420: 4765 7453 6f75 7263 6572 0d00 0000 2902  GetSourcer....).
+00000430: da02 2e30 da01 70a9 0172 0c00 0000 7212  ...0..p..r....r.
+00000440: 0000 0072 1300 0000 da0a 3c6c 6973 7463  ...r......<listc
+00000450: 6f6d 703e 2000 0000 7302 0000 0018 007a  omp> ...s......z
+00000460: 3357 6974 6849 7465 6d53 6f75 7263 654d  3WithItemSourceM
+00000470: 6174 6368 6572 2e47 6574 536f 7572 6365  atcher.GetSource
+00000480: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000490: 6f6d 703e da00 2903 7207 0000 0072 0800  omp>..).r....r..
+000004a0: 0000 da04 6a6f 696e 2903 720c 0000 00da  ....join).r.....
+000004b0: 0b73 6f75 7263 655f 6c69 7374 7216 0000  .source_listr...
+000004c0: 0072 1200 0000 721c 0000 0072 1300 0000  .r....r....r....
+000004d0: 7219 0000 001c 0000 0073 0c00 0000 0401  r........s......
+000004e0: 0401 0401 04ff 1202 0a01 7a1f 5769 7468  ..........z.With
+000004f0: 4974 656d 536f 7572 6365 4d61 7463 6865  ItemSourceMatche
+00000500: 722e 4765 7453 6f75 7263 6529 024e 4e29  r.GetSource).NN)
+00000510: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000520: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000530: 616d 655f 5f72 0b00 0000 7218 0000 0072  ame__r....r....r
+00000540: 1900 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
+00000550: 6c5f 5f72 1200 0000 7212 0000 0072 1000  l__r....r....r..
+00000560: 0000 7213 0000 0072 0600 0000 0700 0000  ..r....r........
+00000570: 7308 0000 0008 000e 0108 0810 0c72 0600  s............r..
+00000580: 0000 4e29 09da 2366 756e 5f77 6974 685f  ..N)..#fun_with_
+00000590: 6173 742e 706c 6163 6568 6f6c 6465 7273  ast.placeholders
+000005a0: 2e63 6f6d 706f 7369 7465 7202 0000 00da  .compositer.....
+000005b0: 1e66 756e 5f77 6974 685f 6173 742e 706c  .fun_with_ast.pl
+000005c0: 6163 6568 6f6c 6465 7273 2e74 6578 7472  aceholders.textr
+000005d0: 0300 0000 da29 6675 6e5f 7769 7468 5f61  .....)fun_with_a
+000005e0: 7374 2e73 6f75 7263 655f 6d61 7463 6865  st.source_matche
+000005f0: 7273 2e62 6173 655f 6d61 7463 6865 7272  rs.base_matcherr
+00000600: 0400 0000 da24 6675 6e5f 7769 7468 5f61  .....$fun_with_a
+00000610: 7374 2e70 6c61 6365 686f 6c64 6572 732e  st.placeholders.
+00000620: 6261 7365 5f6d 6174 6368 7205 0000 0072  base_matchr....r
+00000630: 0600 0000 7212 0000 0072 1200 0000 7212  ....r....r....r.
+00000640: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000650: 653e 0100 0000 730a 0000 000c 000c 010c  e>....s.........
+00000660: 010c 0114 03                             .....
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/body.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from fun_with_ast.placeholders.list_placeholder import ListFieldPlaceholder
-from fun_with_ast.manipulate_node.create_node import SyntaxFreeLine
+from fun_with_ast.manipulate_node.syntax_free_line_node import SyntaxFreeLine
 from fun_with_ast.get_source import GetSource
-from fun_with_ast.source_matchers.base_matcher import MatchPlaceholder, MatchPlaceholderList
+from fun_with_ast.placeholders.base_match import MatchPlaceholder, MatchPlaceholderList
 
 
 class BodyPlaceholder(ListFieldPlaceholder):
     """Placeholder for a "body" field. Handles adding SyntaxFreeLine nodes."""
 
     def __init__(self, *args, **kwargs):
         self.match_after = kwargs.pop('match_after', False)
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/constant_source_match.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/constant_source_match.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import ast
 
 from fun_with_ast.placeholders.composite import FieldPlaceholder
 from fun_with_ast.placeholders.text import TextPlaceholder
 from fun_with_ast.source_matchers.base_matcher import SourceMatcher
 from fun_with_ast.source_matchers.defualt_matcher import DefaultSourceMatcher
-#from fun_with_ast.source_matchers.number import NumSourceMatcher, BoolSourceMatcher
 from fun_with_ast.source_matchers.str import StrSourceMatcher
 
 
 class ConstantSourceMatcher(SourceMatcher):
     def __init__(self, node, starting_parens=None, parent_node=None):
         SourceMatcher.__init__(self, node)
         if not isinstance(node, ast.Constant):
             raise ValueError
-#        self.node = node
         self.num_matcher = DefaultSourceMatcher(node, [
                                                        FieldPlaceholder('value'),
                                                        TextPlaceholder(r'[ \t]*(#+.*)*\n?', '')])
 
-        #        self.num_matcher = NumSourceMatcher(node, starting_parens)
         self.bool_matcher = DefaultSourceMatcher(node, [
                                                        FieldPlaceholder('value'),
                                                        TextPlaceholder(r'[ \t]*(#+.*)*\n?', '')])
-            #BoolSourceMatcher(node, starting_parens)
         self.parent_node = parent_node
         if isinstance(self.parent_node, ast.JoinedStr):
             self.accept_multiparts_string = False
         else:
             self.accept_multiparts_string = True
-        self.str_matcher = StrSourceMatcher(node, starting_parens, self.accept_multiparts_string)
-
+        if isinstance(node.s, str):
+            self.str_matcher = StrSourceMatcher(node, starting_parens, self.accept_multiparts_string)
+        else:
+            self.str_matcher = None
 
     def _match(self, string):
         if isinstance(self.node.n, bool):
             return self.bool_matcher._match(string)
         if isinstance(self.node.n, int) and isinstance(self.node.s, int):
             return self.num_matcher._match(string)
         if isinstance(self.node.n, str) and isinstance(self.node.s, str):
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/if_source_match.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/if_source_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import _ast
 
 from fun_with_ast.source_matchers.body import BodyPlaceholder
 from fun_with_ast.placeholders.composite import FieldPlaceholder
 from fun_with_ast.placeholders.list_placeholder import ListFieldPlaceholder
-from fun_with_ast.manipulate_node.create_node import SyntaxFreeLine
+from fun_with_ast.manipulate_node.syntax_free_line_node import SyntaxFreeLine
 from fun_with_ast.get_source import GetSource
-from fun_with_ast.source_matchers.base_matcher import SourceMatcher, MatchPlaceholderList, MatchPlaceholder
+from fun_with_ast.source_matchers.base_matcher import SourceMatcher
+from fun_with_ast.placeholders.base_match import MatchPlaceholder, MatchPlaceholderList
 from fun_with_ast.placeholders.text import TextPlaceholder
 
 
 class IfSourceMatcher(SourceMatcher):
     """Class to generate the source for an _ast.If node."""
 
     def __init__(self, node, starting_parens=None, parent=None):
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/joined_str.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/joined_str.py`

 * *Files 24% similar despite different names*

```diff
@@ -70,25 +70,7 @@
         elif string.startswith("f\""):
             return "\""
         raise BadlySpecifiedTemplateError('Formatted string must start with \' or \"')
 
     def _check_not_implemented(self, string):
         if '\"\"' in string:
             raise NotImplementedError('Double-quotes are not supported yet')
-# class JoinedStrSourceMatcher(StrSourceMatcher):
-#     def __init__(self, node, starting_parens=None):
-#         super(JoinedStrSourceMatcher, self).__init__(node, starting_parens)
-#         self.value_placeholder = ListFieldPlaceholder('values')
-#
-#     def _get_original_string(self):
-#         self.original_s = ''
-#
-#     def _part_place_holder(self):
-#         return JoinedStringPartPlaceholder()
-#
-#     def Match(self, string):
-#         part = self._part_place_holder()
-#         remaining_string = MatchPlaceholder(string, None, part)
-#         self.quote_parts.append(part)
-#
-#     def _handle_multipart(self, remaining_string):
-#         pass
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/matcher_resolver.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/matcher_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # A mapping of node_type: expected_parts
 import _ast
 import sys
 
 import fun_with_ast.manipulate_node.create_node
-def GetDynamicMatcher(node, starting_parens=None, parent_node=None):
+import fun_with_ast.manipulate_node.syntax_free_line_node
+import fun_with_ast.manipulate_node.call_args_node
+
+
+def GetDynamicMatcher(node, starting_parens=None, parent_node=None, parts_in=None):
     """Gets an initialized matcher for the given node (doesnt call .Match).
 
     If there is no corresponding matcher in _matchers, this will return a
     default matcher, which starts with a placeholder for the first field, ends
     with a placeholder for the last field, and includes TextPlaceholders
     with ['.*' regexes between.
 
@@ -21,15 +25,18 @@
     if starting_parens is None:
         starting_parens = []
     parts_or_matcher_string = _dynamic_matchers[node.__class__][0]
     parts_or_matcher_module = _dynamic_matchers[node.__class__][1]
     current_module = sys.modules[parts_or_matcher_module]
     parts_or_matcher = getattr(current_module, parts_or_matcher_string)
     try:
-        parts = parts_or_matcher()
+        if not parts_in :
+            parts = parts_or_matcher()
+        else:
+            parts = parts_in
         default_source_matcher = current_module.DefaultSourceMatcher
         return default_source_matcher(node, parts, starting_parens, parent_node)
     except TypeError:
         matcher = parts_or_matcher(node, starting_parens, parent_node)
         return matcher
 
 _dynamic_matchers = {
@@ -42,15 +49,14 @@
     _ast.AugAssign: ['get_AugAssign_expected_parts', 'fun_with_ast.source_match'],
     _ast.arguments: ['get_arguments_expected_parts', 'fun_with_ast.source_match'],
     _ast.arg: ['get_arg_expected_parts', 'fun_with_ast.source_match'],
     _ast.BinOp: ['get_BinOp_expected_parts', 'fun_with_ast.source_match'],
     _ast.BitAnd: ['get_BitAnd_expected_parts', 'fun_with_ast.source_match'],
     _ast.BitOr: ['get_BitOr_expected_parts', 'fun_with_ast.source_match'],
     _ast.BitXor: ['get_BitXor_expected_parts', 'fun_with_ast.source_match'],
-#    _ast.BoolOp: ['BoolOpSourceMatcher', 'fun_with_ast.boolop_source_match'],
     _ast.BoolOp: ['BoolOpSourceMatcher', 'fun_with_ast.source_match'],
     _ast.Break: ['get_Break_expected_parts', 'fun_with_ast.source_match'],
     _ast.Call: ['get_Call_expected_parts', 'fun_with_ast.source_match'],
     _ast.ClassDef: ['get_ClassDef_expected_parts', 'fun_with_ast.source_match'],
     _ast.Compare: ['get_Compare_expected_parts', 'fun_with_ast.source_match'],
     _ast.comprehension: ['get_comprehension_expected_parts', 'fun_with_ast.source_match'],
     _ast.Continue: ['get_Continue_expected_parts', 'fun_with_ast.source_match'],
@@ -69,15 +75,14 @@
     _ast.Gt: ['get_Gt_expected_parts', 'fun_with_ast.source_match'],
     _ast.GtE: ['get_GtE_expected_parts', 'fun_with_ast.source_match'],
     _ast.If: ['IfSourceMatcher', 'fun_with_ast.source_matchers.if_source_match'],
     _ast.IfExp: ['get_IfExp_expected_parts', 'fun_with_ast.source_match'],
     _ast.Import: ['get_Import_expected_parts', 'fun_with_ast.source_match'],
     _ast.ImportFrom: ['get_ImportFrom_expected_parts', 'fun_with_ast.source_match'],
     _ast.In: ['get_In_expected_parts', 'fun_with_ast.source_match'],
-    #    _ast.Index: get_Index_expected_parts', 'fun_with_ast.source_match'],
     _ast.Invert: ['get_Invert_expected_parts', 'fun_with_ast.source_match'],
     _ast.Is: ['get_Is_expected_parts', 'fun_with_ast.source_match'],
     _ast.IsNot: ['get_IsNot_expected_parts', 'fun_with_ast.source_match'],
     _ast.keyword: ['get_keyword_expected_parts', 'fun_with_ast.source_match'],
     _ast.Lambda: ['get_Lambda_expected_parts', 'fun_with_ast.source_match'],
     _ast.List: ['get_List_expected_parts', 'fun_with_ast.source_match'],
     _ast.ListComp: ['get_ListComp_expected_parts', 'fun_with_ast.source_match'],
@@ -87,39 +92,36 @@
     _ast.Mod: ['get_Mod_expected_parts', 'fun_with_ast.source_match'],
     _ast.Module: ['get_Module_expected_parts', 'fun_with_ast.source_match'],
     _ast.Mult: ['get_Mult_expected_parts', 'fun_with_ast.source_match'],
     _ast.Name: ['get_Name_expected_parts', 'fun_with_ast.source_match'],
     _ast.Not: ['get_Not_expected_parts', 'fun_with_ast.source_match'],
     _ast.NotIn: ['get_NotIn_expected_parts', 'fun_with_ast.source_match'],
     _ast.NotEq: ['get_NotEq_expected_parts', 'fun_with_ast.source_match'],
-    #    _ast.Num: NumSourceMatcher', 'fun_with_ast.source_match'],
     _ast.Or: ['get_Or_expected_parts', 'fun_with_ast.source_match'],
     _ast.Pass: ['get_Pass_expected_parts', 'fun_with_ast.source_match'],
     _ast.Pow: ['get_Pow_expected_parts', 'fun_with_ast.source_match'],
-    #    _ast.Print: get_Print_expected_parts', 'fun_with_ast.source_match'],
     _ast.Raise: ['get_Raise_expected_parts', 'fun_with_ast.source_match'],
     _ast.Return: ['get_Return_expected_parts', 'fun_with_ast.source_match'],
     _ast.RShift: ['get_RShift_expected_parts', 'fun_with_ast.source_match'],
     _ast.Slice: ['get_Slice_expected_parts', 'fun_with_ast.source_match'],
     _ast.Sub: ['get_Sub_expected_parts', 'fun_with_ast.source_match'],
     _ast.Set: ['get_Set_expected_parts', 'fun_with_ast.source_match'],
     _ast.SetComp: ['get_SetComp_expected_parts', 'fun_with_ast.source_match'],
     _ast.Subscript: ['get_Subscript_expected_parts', 'fun_with_ast.source_match'],
-    #    _ast.Str: ['StrSourceMatcher', 'fun_with_ast.source_match'],
     _ast.Constant: ['ConstantSourceMatcher', 'fun_with_ast.source_match'],
-    fun_with_ast.manipulate_node.create_node.SyntaxFreeLine: ['SyntaxFreeLineMatcher', 'fun_with_ast.source_matchers.syntaxfreeline'],
-#    manipulate_node.create_node.SyntaxFreeLine: ['get_SyntaxFreeLine_expected_parts', 'fun_with_ast.source_match'],
-    fun_with_ast.manipulate_node.create_node.Comment: ['get_Comment_expected_parts', 'fun_with_ast.source_match'],
     _ast.Tuple: ['get_Tuple_expected_parts', 'fun_with_ast.source_match'],
-    #    _ast.TryExcept: get_TryExcept_expected_parts', 'fun_with_ast.source_match'],
-    #    _ast.Try: TryFinallySourceMatcher', 'fun_with_ast.source_match'],
     _ast.JoinedStr: ['JoinedStrSourceMatcher', 'fun_with_ast.source_matchers.joined_str'],
     _ast.Try: ['get_TryExcept_expected_parts', 'fun_with_ast.source_match'],
     _ast.FormattedValue: ['get_FormattedValue_expected_parts', 'fun_with_ast.source_match'],
     _ast.UAdd: ['get_UAdd_expected_parts', 'fun_with_ast.source_match'],
     _ast.UnaryOp: ['get_UnaryOp_expected_parts', 'fun_with_ast.source_match'],
     _ast.USub: ['get_USub_expected_parts', 'fun_with_ast.source_match'],
     _ast.While: ['get_While_expected_parts', 'fun_with_ast.source_match'],
     _ast.With: ['WithSourceMatcher', 'fun_with_ast.source_match'],
     _ast.withitem: ['WithItemSourceMatcher', 'fun_with_ast.source_matchers.withitem'],
-    _ast.Yield: ['get_Yield_expected_parts', 'fun_with_ast.source_match']
+    _ast.Yield: ['get_Yield_expected_parts', 'fun_with_ast.source_match'],
+    fun_with_ast.manipulate_node.syntax_free_line_node.SyntaxFreeLine: ['SyntaxFreeLineMatcher',
+                                                                        'fun_with_ast.source_matchers.syntaxfreeline'],
+    fun_with_ast.manipulate_node.create_node.Comment: ['get_Comment_expected_parts', 'fun_with_ast.source_match'],
+    fun_with_ast.manipulate_node.call_args_node.CallArgs: ['get_CallArgs_expected_parts', 'fun_with_ast.source_match'],
+
 }
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/str.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/str.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import re
 
 from fun_with_ast.source_matchers.exceptions import BadlySpecifiedTemplateError
 
-from fun_with_ast.source_matchers.base_matcher import MatchPlaceholder
+from fun_with_ast.placeholders.base_match import MatchPlaceholder
 from fun_with_ast.source_matchers.base_matcher import SourceMatcher
 from fun_with_ast.placeholders.string_part import StringPartPlaceholder
-from fun_with_ast.common_utils.utils_source_match import _GetListDefault, GetDefaultQuoteType
+from fun_with_ast.common_utils.utils_source_match import _GetListDefault
 from fun_with_ast.placeholders.text import TextPlaceholder
 
 
 class StrSourceMatcher(SourceMatcher):
     """Class to generate the source for an _ast.Str node."""
 
     def __init__(self, node, starting_parens=None, accept_multiparts_string=True):
         super(StrSourceMatcher, self).__init__(node, starting_parens)
         self.separator_placeholder = TextPlaceholder(r'\s*', '')
         self.quote_parts = []
         self.separators = []
         # If set, will apply to all parts of the string.
-        self.quote_type = None
+
+        if  hasattr(node, 'default_quote'):
+            self.quote_type = node.default_quote
+        else:
+            raise ValueError('node must have a default_quote attribute')
         self.original_quote_type = None
         self.original_s = None
         self.accept_multiparts_string=accept_multiparts_string
 
     def _GetMatchedInnerText(self):
         return ''.join(p.inner_text_placeholder.GetSource(self.node)
                        for p in self.quote_parts)
@@ -33,16 +37,14 @@
         part = self._part_place_holder()
         remaining_string = MatchPlaceholder(remaining_string, None, part)
         self.quote_parts.append(part)
 
         remaining_string = self._handle_multipart(remaining_string)
 
         self.MatchEndParen(remaining_string)
-        #if len(self.quote_parts) != 1 :
-        #    raise NotImplementedError('Multi-part strings not yet supported')
         self.original_quote_type = (
             self.quote_parts[0].quote_match_placeholder.matched_text)
         parsed_string = self._match_parsed_string()
         result = StrSourceMatcher.GetSource(self)
         self.matched = True
         self.matched_source = result
         return result
@@ -57,16 +59,15 @@
         for part in self.quote_parts:
             string_body += part.inner_text_placeholder.matched_text
         if len(string_body) != len(self.original_s):
             raise BadlySpecifiedTemplateError(f'String body: {string_body} does not match node.s: {self.original_s}')
         parsed_string = start_paran_text + start_quote + string_body + end_quote + end_paran_text
         if parsed_string !=  start_paran_text +start_quote + self.original_s + end_quote + end_paran_text:
              raise BadlySpecifiedTemplateError(f'Parsed body: {parsed_string} does not match node.s: {self.original_s}')
-        # if not self.original_s in parsed_string:
-        #     raise BadlySpecifiedTemplateError(f'Parsed body: {parsed_string} does not match node.s: {self.original_s}')
+
 
         return parsed_string
 
     def _handle_multipart(self, remaining_string):
         if not self.accept_multiparts_string:
             return remaining_string
         while True:
@@ -86,15 +87,16 @@
         # We try to preserve the formatting on a best-effort basis
         if self.original_s is not None and self.original_s != self.node.s:
             self.quote_parts = [self.quote_parts[0]]
             self.quote_parts[0].inner_text_placeholder.matched_text = self.node.s
 
         if self.original_s is None:
             if not self.quote_type:
-                self.quote_type = self.original_quote_type or GetDefaultQuoteType()
+                raise ValueError('quote_type must be set')
+                #self.quote_type = self.original_quote_type or GetDefaultQuoteType()
             return self.quote_type + self.node.s + self.quote_type
 
         if self.quote_type:
             for part in self.quote_parts:
                 part.quote_match_placeholder.matched_text = self.quote_type
 
         source_list = [self.GetStartParenText()]
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/syntaxfreeline.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/syntaxfreeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,10 +11,9 @@
 
     def __init__(self, node, expected_parts, starting_parens=None, parent_node=None):
         parts = [FieldPlaceholder('full_line'), TextPlaceholder(r'\n', '\n')]
         super(SyntaxFreeLineMatcher, self).__init__(node, parts, starting_parens)
 
     def MatchWhiteSpaces(self, remaining_string):
         ws_placeholder = WhiteSpaceTextPlaceholder()
-#        ws_placeholder.Match(None, remaining_string)
         self.start_whitespace_matchers.append(ws_placeholder)
-        return remaining_string # NOTE: we retrun remainiing_string !
+        return remaining_string # NOTE: we return remaining_string !
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/with_matcher.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/with_matcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import _ast
 
 from fun_with_ast.source_matchers.body import BodyPlaceholder
 from fun_with_ast.get_source import GetSource
-from fun_with_ast.source_matchers.base_matcher import SourceMatcher, MatchPlaceholderList
+from fun_with_ast.source_matchers.base_matcher import SourceMatcher
+from fun_with_ast.placeholders.base_match import MatchPlaceholderList
 from fun_with_ast.placeholders.text import TextPlaceholder
 from fun_with_ast.placeholders.list_placeholder import SeparatedListFieldPlaceholder
 
 
 class WithSourceMatcher(SourceMatcher):
     """Class to generate the source for an _ast.With node."""
 
     def __init__(self, node, starting_parens=None, Parent=None):
         super(WithSourceMatcher, self).__init__(node, starting_parens)
         self.with_placeholder = TextPlaceholder(r' *(with)? *', 'with ')
         self.withitems_placeholder = SeparatedListFieldPlaceholder('items', before_separator_placeholder=TextPlaceholder(r', *', ', '))
-        #    self.context_expr = FieldPlaceholder('context_expr')
-        #    self.optional_vars = FieldPlaceholder(
-        #        'optional_vars',
-        #        before_placeholder=TextPlaceholder(r' *as *', ' as '))
-#        self.compound_separator = TextPlaceholder(r'\s*,\s*', ', ')
         self.colon_placeholder = TextPlaceholder(r':\n?', ':\n')
         self.body_placeholder = BodyPlaceholder('body')
         self.is_compound_with = False
         self.starting_with = True
 
     def _match(self, string):
         if string.lstrip().startswith('with'):
```

### Comparing `fun_with_ast-0.1.68/fun_with_ast/source_matchers/withitem.py` & `fun_with_ast-0.1.70/fun_with_ast/source_matchers/withitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from fun_with_ast.placeholders.composite import FieldPlaceholder
 from fun_with_ast.placeholders.text import TextPlaceholder
-from fun_with_ast.source_matchers.base_matcher import SourceMatcher, MatchPlaceholderList
+from fun_with_ast.source_matchers.base_matcher import SourceMatcher
+from fun_with_ast.placeholders.base_match import MatchPlaceholderList
 
 
 class WithItemSourceMatcher(SourceMatcher):
     def __init__(self, node, starting_parens=None, parent=None):
         super(WithItemSourceMatcher, self).__init__(node, starting_parens)
         self.context_expr = FieldPlaceholder('context_expr')
         self.optional_vars = FieldPlaceholder(
```

