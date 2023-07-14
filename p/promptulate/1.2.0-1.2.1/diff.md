# Comparing `tmp/promptulate-1.2.0.tar.gz` & `tmp/promptulate-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptulate-1.2.0.tar", last modified: Sun Jun 25 15:18:29 2023, max compression
+gzip compressed data, was "dist\promptulate-1.2.1.tar", last modified: Fri Jul 14 06:02:46 2023, max compression
```

## Comparing `promptulate-1.2.0.tar` & `promptulate-1.2.1.tar`

### file list

```diff
@@ -1,79 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.147642 promptulate-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 15:18:17.000000 promptulate-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-25 15:18:29.147642 promptulate-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-25 15:18:17.000000 promptulate-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate/command/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/command/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/frameworks/conversation/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/conversation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/conversation/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/frameworks/react/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/react/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/frameworks/self_ask/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/frameworks/self_ask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/llms/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/memory/local_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/preset_roles/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/preset_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/preset_roles/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/preset_roles/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/provider/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tips.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/arxiv/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/arxiv/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/duckduckgo/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/duckduckgo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/paper/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/paper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/paper/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/python_repl/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/python_repl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/python_repl/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/python_repl/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.143642 promptulate-1.2.0/promptulate/tools/semantic_scholar/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/semantic_scholar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/semantic_scholar/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/tools/semantic_scholar/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.147642 promptulate-1.2.0/promptulate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/core_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/openai_key_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-25 15:18:17.000000 promptulate-1.2.0/promptulate/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:18:29.139642 promptulate-1.2.0/promptulate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:18:29.000000 promptulate-1.2.0/promptulate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:18:29.147642 promptulate-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-25 15:18:17.000000 promptulate-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-14 06:01:50.000000 promptulate-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     7993 2023-07-14 06:02:46.000000 promptulate-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7035 2023-07-14 06:01:50.000000 promptulate-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate/
+-rw-rw-rw-   0        0        0     1115 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/agents/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/client/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/client/__init__.py
+-rw-rw-rw-   0        0        0     1757 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/client/chat.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/command/
+-rw-rw-rw-   0        0        0      127 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/command/__init__.py
+-rw-rw-rw-   0        0        0     4438 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/config.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/frameworks/
+-rw-rw-rw-   0        0        0      878 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/frameworks/chain/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/frameworks/conversation/
+-rw-rw-rw-   0        0        0      890 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/conversation/__init__.py
+-rw-rw-rw-   0        0        0     4731 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/conversation/conversation.py
+-rw-rw-rw-   0        0        0     1780 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/prompt.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/frameworks/react/
+-rw-rw-rw-   0        0        0      773 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/react/__init__.py
+-rw-rw-rw-   0        0        0     1152 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/frameworks/self_ask/
+-rw-rw-rw-   0        0        0      773 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/frameworks/self_ask/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/llms/
+-rw-rw-rw-   0        0        0      869 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/llms/__init__.py
+-rw-rw-rw-   0        0        0     1392 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/llms/base.py
+-rw-rw-rw-   0        0        0     9567 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/memory/
+-rw-rw-rw-   0        0        0      948 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/memory/__init__.py
+-rw-rw-rw-   0        0        0     2306 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/memory/base.py
+-rw-rw-rw-   0        0        0     2161 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/memory/buffer.py
+-rw-rw-rw-   0        0        0     2294 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/memory/file.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/preset_roles/
+-rw-rw-rw-   0        0        0      929 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/preset_roles/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/preset_roles/prompt.py
+-rw-rw-rw-   0        0        0     5004 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/preset_roles/roles.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/provider/
+-rw-rw-rw-   0        0        0     1063 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/provider/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/provider/base.py
+-rw-rw-rw-   0        0        0     4839 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/provider/mixins.py
+-rw-rw-rw-   0        0        0     4763 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/schema.py
+-rw-rw-rw-   0        0        0     1184 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tips.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/tools/arxiv/
+-rw-rw-rw-   0        0        0      268 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/arxiv/__init__.py
+-rw-rw-rw-   0        0        0     4917 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/arxiv/api_wrapper.py
+-rw-rw-rw-   0        0        0      393 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/arxiv/toolkit.py
+-rw-rw-rw-   0        0        0     9808 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/arxiv/tools.py
+-rw-rw-rw-   0        0        0      592 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/base.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/tools/duckduckgo/
+-rw-rw-rw-   0        0        0      161 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/duckduckgo/__init__.py
+-rw-rw-rw-   0        0        0     3476 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/duckduckgo/api_wrapper.py
+-rw-rw-rw-   0        0        0     3543 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/duckduckgo/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/tools/paper/
+-rw-rw-rw-   0        0        0       94 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/paper/__init__.py
+-rw-rw-rw-   0        0        0     7410 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/paper/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/tools/python_repl/
+-rw-rw-rw-   0        0        0      104 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/python_repl/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/python_repl/api_wrapper.py
+-rw-rw-rw-   0        0        0      723 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/python_repl/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/tools/semantic_scholar/
+-rw-rw-rw-   0        0        0      283 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/semantic_scholar/__init__.py
+-rw-rw-rw-   0        0        0     6807 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/semantic_scholar/api_wrapper.py
+-rw-rw-rw-   0        0        0     2330 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/tools/semantic_scholar/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate/utils/
+-rw-rw-rw-   0        0        0     1580 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/__init__.py
+-rw-rw-rw-   0        0        0     3906 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/core_utils.py
+-rw-rw-rw-   0        0        0     1808 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/logger.py
+-rw-rw-rw-   0        0        0     4220 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/openai_key_pool.py
+-rw-rw-rw-   0        0        0     1632 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/proxy.py
+-rw-rw-rw-   0        0        0     1403 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/singleton.py
+-rw-rw-rw-   0        0        0      664 2023-07-14 06:01:50.000000 promptulate-1.2.1/promptulate/utils/string_template.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:02:46.000000 promptulate-1.2.1/promptulate.egg-info/
+-rw-rw-rw-   0        0        0     7993 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2048 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 06:02:45.000000 promptulate-1.2.1/promptulate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:02:46.000000 promptulate-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2330 2023-07-14 06:01:50.000000 promptulate-1.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `promptulate-1.2.0/LICENSE` & `promptulate-1.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `promptulate-1.2.0/PKG-INFO` & `promptulate-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,126 +1,128 @@
-Metadata-Version: 2.1
-Name: promptulate
-Version: 1.2.0
-Summary: A powerful LLM Prompt Layer frameworks
-Home-page: https://github.com/Undertone0809/promptulate
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    promptulate
-</h1>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
-</p>
-
-
-`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
-AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
-6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
-System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
-Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
-Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
-Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
-
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口
-- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
-- KEY池：提供API key池，彻底解决key限速的问题
-- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
-- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
-- 中文优化：针对中文语境进行特别优化，更适合中文场景
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 快速开始
-
-- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
-- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
-- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
-- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
-- [pypi仓库](https://pypi.org/project/promptulate/)
-
-# 基础架构
-
-在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
-
-`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
-
-- `Agent` 更高级的执行器，负责复杂任务的调度和分发
-- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
-- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
-- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
-- `preset roles` 提供预设角色，进行定制化对话
-- `provider` 为framework和agent提供tools和其他细粒度能力的集成
-
-# 设计原则
-
-promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
-
-- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
-- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
-- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
-- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
-- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
-- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
-- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
-
-以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
-
-# 交流群
-
-欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
-
-<div style="width: 250px;margin: 0 auto;">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230623214722.png"/>
-</div>
-
-# 贡献
-
-本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: promptulate
+Version: 1.2.1
+Summary: A powerful LLM Prompt Layer frameworks
+Home-page: https://github.com/Undertone0809/promptulate
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    promptulate
+</h1>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口
+- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
+- KEY池：提供API key池，彻底解决key限速的问题
+- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 中文优化：针对中文语境进行特别优化，更适合中文场景
+- 数据导出：支持markdowm等格式的对话导出
+- 对话总结：提供API式的对话总结、翻译、标题生成
+- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
+- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
+
+# 快速开始
+
+- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
+- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
+- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
+- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
+- [pypi仓库](https://pypi.org/project/promptulate/)
+
+# 基础架构
+
+在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
+等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
+重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
+的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
+
+`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
+
+- `Agent` 更高级的执行器，负责复杂任务的调度和分发
+- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
+- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
+- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
+- `preset roles` 提供预设角色，进行定制化对话
+- `provider` 为framework和agent提供tools和其他细粒度能力的集成
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
+
+# 设计原则
+
+promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
+
+# 交流群
+
+欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
+
+<div style="width: 250px;margin: 0 auto;">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230702132948.png"/>
+</div>
+
+# 贡献
+
+本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.2.0/README.md` & `promptulate-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,102 +1,104 @@
-<h1 align="center">
-    promptulate
-</h1>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
-</p>
-
-
-`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
-AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
-6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
-System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
-Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
-Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
-Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
-
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口
-- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
-- KEY池：提供API key池，彻底解决key限速的问题
-- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
-- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
-- 中文优化：针对中文语境进行特别优化，更适合中文场景
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 快速开始
-
-- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
-- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
-- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
-- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
-- [pypi仓库](https://pypi.org/project/promptulate/)
-
-# 基础架构
-
-在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
-
-`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
-
-- `Agent` 更高级的执行器，负责复杂任务的调度和分发
-- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
-- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
-- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
-- `preset roles` 提供预设角色，进行定制化对话
-- `provider` 为framework和agent提供tools和其他细粒度能力的集成
-
-# 设计原则
-
-promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
-
-- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
-- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
-- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
-- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
-- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
-- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
-- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
-
-以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
-
-# 交流群
-
-欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
-
-<div style="width: 250px;margin: 0 auto;">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230623214722.png"/>
-</div>
-
-# 贡献
-
-本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+<h1 align="center">
+    promptulate
+</h1>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口
+- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
+- KEY池：提供API key池，彻底解决key限速的问题
+- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 中文优化：针对中文语境进行特别优化，更适合中文场景
+- 数据导出：支持markdowm等格式的对话导出
+- 对话总结：提供API式的对话总结、翻译、标题生成
+- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
+- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
+
+# 快速开始
+
+- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
+- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
+- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
+- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
+- [pypi仓库](https://pypi.org/project/promptulate/)
+
+# 基础架构
+
+在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
+等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
+重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
+的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
+
+`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
+
+- `Agent` 更高级的执行器，负责复杂任务的调度和分发
+- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
+- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
+- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
+- `preset roles` 提供预设角色，进行定制化对话
+- `provider` 为framework和agent提供tools和其他细粒度能力的集成
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
+
+# 设计原则
+
+promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
+
+# 交流群
+
+欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
+
+<div style="width: 250px;margin: 0 auto;">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230702132948.png"/>
+</div>
+
+# 贡献
+
+本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
 和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.2.0/promptulate/__init__.py` & `promptulate-1.2.1/promptulate/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.frameworks import Conversation
-from promptulate.utils import enable_log, enable_log_no_file
-from promptulate.schema import UserMessage, AssistantMessage, SystemMessage, BaseChatMessageHistory, LLMPrompt
-
-__all__ = [
-    'Conversation',
-
-    'enable_log',
-    'enable_log_no_file',
-
-    'SystemMessage',
-    'UserMessage',
-    'AssistantMessage',
-    'BaseChatMessageHistory',
-    'LLMPrompt',
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.frameworks import Conversation
+from promptulate.schema import UserMessage, AssistantMessage, SystemMessage
+from promptulate.utils import enable_log, enable_log_no_file
+
+__all__ = [
+    "Conversation",
+    "enable_log",
+    "enable_log_no_file",
+    "SystemMessage",
+    "UserMessage",
+    "AssistantMessage",
+]
```

### Comparing `promptulate-1.2.0/promptulate/command/chat.py` & `promptulate-1.2.1/promptulate/client/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import os
-import argparse
-from promptulate import Conversation
-from promptulate.utils import set_proxy_mode
-
-
-def chat():
-    parser = argparse.ArgumentParser(description='Welcome to Promptulate Chat - The best chat terminal ever!')
-    parser.add_argument('--openai_api_key', help='when you first run, you should enter your openai api key')
-    parser.add_argument('--proxy_mode', help='select openai proxy and provide [off, promptulate]')
-    args = parser.parse_args()
-
-    if args.openai_api_key:
-        os.environ['OPENAI_API_KEY'] = args.openai_api_key
-    if args.proxy_mode:
-        set_proxy_mode(args.proxy_mode)
-
-    set_proxy_mode('promptulate')
-    print(f'Hi there, here is promptulate chat terminal.')
-    conversation = Conversation()
-    while True:
-        prompt = str(input("[User] "))
-        ret = conversation.predict(prompt)
-        print(f"[output] {ret}")
-
-
-def main():
-    chat()
-
-
-if __name__ == '__main__':
-    main()
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import argparse
+import os
+
+from promptulate import Conversation
+from promptulate.utils import set_proxy_mode
+
+
+def chat():
+    parser = argparse.ArgumentParser(description='Welcome to Promptulate Chat - The best chat terminal ever!')
+    parser.add_argument('--openai_api_key', help='when you first run, you should enter your openai api key')
+    parser.add_argument('--proxy_mode', help='select openai proxy and provide [off, promptulate]')
+    args = parser.parse_args()
+
+    if args.openai_api_key:
+        os.environ['OPENAI_API_KEY'] = args.openai_api_key
+    if args.proxy_mode:
+        set_proxy_mode(args.proxy_mode)
+
+    set_proxy_mode('promptulate')
+    print(f'Hi there, here is promptulate chat terminal.')
+    conversation = Conversation()
+    while True:
+        prompt = str(input("[User] "))
+        ret = conversation.predict(prompt)
+        print(f"[output] {ret}")
+
+
+def main():
+    chat()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `promptulate-1.2.0/promptulate/config.py` & `promptulate-1.2.1/promptulate/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,115 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import os
-from typing import Optional
-from promptulate import utils
-from promptulate.utils.singleton import Singleton
-from promptulate.utils.openai_key_pool import OpenAIKeyPool
-from promptulate.utils.logger import get_logger
-
-PROXY_MODE = ["off", "custom", "promptulate"]
-logger = get_logger()
-
-
-def set_enable_cache(value: bool):
-    """Caching is enabled by default. Disabling caching is not recommended."""
-    Config().enable_cache = value
-
-
-class Config(metaclass=Singleton):
-    def __init__(self):
-        logger.info(f"[promptulate config] Config initialization")
-        self.enable_cache: bool = True
-        self._proxy_mode: str = PROXY_MODE[0]
-        self._proxies: Optional[dict] = None
-        self.openai_url = "https://api.openai.com/v1/chat/completions"
-        self.openai_proxy_url = "https://chatgpt-api.shn.hk/v1/"  # FREE API
-        self.key_default_retry_times = 5
-        """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained."""
-
-    @property
-    def openai_api_key(self):
-        """This attribution has deprecated to use. Using `get_openai_api_key`"""
-        if "OPENAI_API_KEY" in os.environ.keys():
-            if self.enable_cache:
-                utils.get_cache()["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
-            return os.getenv("OPENAI_API_KEY")
-        if self.enable_cache and "OPENAI_API_KEY" in utils.get_cache():
-            return utils.get_cache()["OPENAI_API_KEY"]
-        raise ValueError("OPENAI API key is not provided. Please set your key.")
-
-    def get_openai_api_key(self, model: str) -> str:
-        if self.enable_cache:
-            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
-            key = openai_key_pool.get(model)
-            if key:
-                return key
-        return self.openai_api_key
-
-
-    def get_key_retry_times(self, model: str) -> int:
-        if self.enable_cache:
-            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
-            return openai_key_pool.get_num(model)
-        return self.key_default_retry_times
-
-    @property
-    def proxy_mode(self) -> str:
-        if self.enable_cache and "PROXY_MODE" in utils.get_cache():
-            return utils.get_cache()["PROXY_MODE"]
-        return self._proxy_mode
-
-    @proxy_mode.setter
-    def proxy_mode(self, value):
-        self._proxy_mode = value
-        if self.enable_cache:
-            utils.get_cache()["PROXY_MODE"] = value
-
-    @property
-    def proxies(self) -> Optional[dict]:
-        if self.enable_cache and "PROXIES" in utils.get_cache():
-            return utils.get_cache()["PROXIES"] if self.proxy_mode == "custom" else None
-        return self._proxies
-
-    @proxies.setter
-    def proxies(self, value):
-        self._proxies = value
-        if self.enable_cache:
-            utils.get_cache()["PROXIES"] = value
-
-    @property
-    def openai_request_url(self) -> str:
-        if self.proxy_mode == PROXY_MODE[2]:
-            self.proxies = None
-            return self.openai_proxy_url
-        return self.openai_url
-
-    def set_proxy_mode(self, mode: str, proxies: Optional[dict] = None):
-        self.proxy_mode = mode
-        self.proxies = proxies
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import os
+from typing import Optional
+
+from promptulate import utils
+from promptulate.utils.logger import get_logger
+from promptulate.utils.openai_key_pool import OpenAIKeyPool
+from promptulate.utils.singleton import Singleton
+
+PROXY_MODE = ["off", "custom", "promptulate"]
+logger = get_logger()
+
+
+def set_enable_cache(value: bool):
+    """Caching is enabled by default. Disabling caching is not recommended."""
+    Config().enable_cache = value
+
+
+class Config(metaclass=Singleton):
+    def __init__(self):
+        logger.info(f"[promptulate config] Config initialization")
+        self.enable_cache: bool = True
+        self._proxy_mode: str = PROXY_MODE[0]
+        self._proxies: Optional[dict] = None
+        self.openai_chat_api_url = "https://api.openai.com/v1/chat/completions"
+        self.openai_completion_api_url = "https://api.openai.com/v1/completions"
+        self.openai_proxy_url = "https://chatgpt-api.shn.hk/v1/"  # FREE API
+        self.key_default_retry_times = 5
+        """If llm(like OpenAI) unable to obtain data, retry request until the data is obtained."""
+
+    @property
+    def openai_api_key(self):
+        """This attribution has deprecated to use. Using `get_openai_api_key`"""
+        if "OPENAI_API_KEY" in os.environ.keys():
+            if self.enable_cache:
+                utils.get_cache()["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
+            return os.getenv("OPENAI_API_KEY")
+        if self.enable_cache and "OPENAI_API_KEY" in utils.get_cache():
+            return utils.get_cache()["OPENAI_API_KEY"]
+        raise ValueError("OPENAI API key is not provided. Please set your key.")
+
+    def get_openai_api_key(self, model: str) -> str:
+        """Get openai key from KeyPool and environ"""
+        if self.enable_cache:
+            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
+            key = openai_key_pool.get(model)
+            if key:
+                return key
+        return self.openai_api_key
+
+    def get_key_retry_times(self, model: str) -> int:
+        if self.enable_cache:
+            openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
+            return openai_key_pool.get_num(model)
+        return self.key_default_retry_times
+
+    @property
+    def proxy_mode(self) -> str:
+        if self.enable_cache and "PROXY_MODE" in utils.get_cache():
+            return utils.get_cache()["PROXY_MODE"]
+        return self._proxy_mode
+
+    @proxy_mode.setter
+    def proxy_mode(self, value):
+        self._proxy_mode = value
+        if self.enable_cache:
+            utils.get_cache()["PROXY_MODE"] = value
+
+    @property
+    def proxies(self) -> Optional[dict]:
+        if self.enable_cache and "PROXIES" in utils.get_cache():
+            return utils.get_cache()["PROXIES"] if self.proxy_mode == "custom" else None
+        return self._proxies
+
+    @proxies.setter
+    def proxies(self, value):
+        self._proxies = value
+        if self.enable_cache:
+            utils.get_cache()["PROXIES"] = value
+
+    @property
+    def openai_chat_request_url(self) -> str:
+        if self.proxy_mode == PROXY_MODE[2]:
+            self.proxies = None
+            return self.openai_proxy_url
+        return self.openai_chat_api_url
+
+    @property
+    def openai_completion_request_url(self) -> str:
+        if self.proxy_mode == PROXY_MODE[2]:
+            self.proxies = None
+            return f"{self.openai_proxy_url}completions"
+        return self.openai_completion_api_url
+
+    def set_proxy_mode(self, mode: str, proxies: Optional[dict] = None):
+        self.proxy_mode = mode
+        self.proxies = proxies
```

### Comparing `promptulate-1.2.0/promptulate/frameworks/__init__.py` & `promptulate-1.2.1/promptulate/frameworks/conversation/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-
-from promptulate.frameworks.conversation import Conversation
-
-__all__ = [
-    'Conversation',
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+
+from promptulate.frameworks.conversation.conversation import Conversation
+
+__all__ = [
+    'Conversation'
+]
```

### Comparing `promptulate-1.2.0/promptulate/frameworks/conversation/__init__.py` & `promptulate-1.2.1/promptulate/preset_roles/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-
-from promptulate.frameworks.conversation.conversation import Conversation
-
-__all__ = [
-    'Conversation'
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.preset_roles.roles import get_all_preset_roles, CustomPresetRole
+
+__all__ = [
+    'get_all_preset_roles',
+    'CustomPresetRole'
+]
```

### Comparing `promptulate-1.2.0/promptulate/frameworks/prompt.py` & `promptulate-1.2.1/promptulate/frameworks/prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-__all__ = [
-    'SUMMARY_CONTENT_PROMPT_ZH',
-    'SUMMARY_TOPIC_PROMPT_ZH',
-    'SUMMARY_TOPIC_PROMPT_EN',
-    'SUMMARY_CONTENT_PROMPT_EN',
-]
-
-SUMMARY_CONTENT_PROMPT_ZH = """
-简要总结一下你和用户的对话，用作后续的上下文提示 prompt，控制在 200 字以内
-"""
-
-SUMMARY_TOPIC_PROMPT_ZH = """
-上面是ai 和用户的历史聊天总结作为前情提要，请使用四到五个字直接返回这句话的简要主题，
-不要解释、不要标点、不要语气词、不要多余文本，如果没有主题，请直接返回“闲聊”
-"""
-
-SUMMARY_CONTENT_PROMPT_EN = """
-Give a quick summary of your conversation with the user and use it as a follow-up context prompt, no more than 200 words
-"""
-
-SUMMARY_TOPIC_PROMPT_EN = """
-As the previous feed, please use four or five words to return directly to the brief topic of the sentence, 
-no explanation, no punctuation, no particles, no extra text, or if there is no topic, just return to "small talk".
-"""
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+__all__ = [
+    'SUMMARY_CONTENT_PROMPT_ZH',
+    'SUMMARY_TOPIC_PROMPT_ZH',
+    'SUMMARY_TOPIC_PROMPT_EN',
+    'SUMMARY_CONTENT_PROMPT_EN',
+]
+
+SUMMARY_CONTENT_PROMPT_ZH = """
+简要总结一下你和用户的对话，用作后续的上下文提示 prompt，控制在 200 字以内
+"""
+
+SUMMARY_TOPIC_PROMPT_ZH = """
+上面是ai 和用户的历史聊天总结作为前情提要，请使用四到五个字直接返回这句话的简要主题，
+不要解释、不要标点、不要语气词、不要多余文本，如果没有主题，请直接返回“闲聊”
+"""
+
+SUMMARY_CONTENT_PROMPT_EN = """
+Give a quick summary of your conversation with the user and use it as a follow-up context prompt, no more than 200 words
+"""
+
+SUMMARY_TOPIC_PROMPT_EN = """
+As the previous feed, please use four or five words to return directly to the brief topic of the sentence, 
+no explanation, no punctuation, no particles, no extra text, or if there is no topic, just return to "small talk".
+"""
```

### Comparing `promptulate-1.2.0/promptulate/frameworks/react/__init__.py` & `promptulate-1.2.1/promptulate/llms/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.llms.openai import OpenAI, ChatOpenAI
+
+__all__ = ["OpenAI", "ChatOpenAI"]
```

### Comparing `promptulate-1.2.0/promptulate/frameworks/self_ask/__init__.py` & `promptulate-1.2.1/promptulate/frameworks/react/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.2.0/promptulate/llms/__init__.py` & `promptulate-1.2.1/promptulate/frameworks/self_ask/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.llms.openai import OpenAI
-
-__all__ = ["OpenAI"]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.2.0/promptulate/memory/__init__.py` & `promptulate-1.2.1/promptulate/memory/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.memory.buffer import BufferChatMemory
-from promptulate.memory.local_cache import LocalCacheChatMemory
-
-__all__ = [
-    'BufferChatMemory',
-    'LocalCacheChatMemory'
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.memory.buffer import BufferChatMemory
+from promptulate.memory.file import FileChatMemory
+
+__all__ = [
+    'BufferChatMemory',
+    'FileChatMemory'
+]
```

### Comparing `promptulate-1.2.0/promptulate/memory/local_cache.py` & `promptulate-1.2.1/promptulate/memory/buffer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional
-
-from promptulate import utils
-from promptulate.tips import EmptyChatMessageHistoryTip
-from promptulate.memory.base import BaseChatMemory
-from promptulate.schema import ListDictPrompt, ChatMessageHistory
-
-cache = utils.get_cache()
-logger = utils.get_logger()
-
-
-class LocalCacheChatMemory(BaseChatMemory):
-    """Chat message will be stored in the local file cache."""
-
-    def load_conversation_from_memory(self, conversation_id: Optional[str]) -> ChatMessageHistory:
-        if conversation_id is None or conversation_id not in cache:
-            raise EmptyChatMessageHistoryTip()
-        cache_messages = cache[conversation_id]
-        return ListDictPrompt(messages=cache_messages).chat_message_history
-
-    def save_conversation_to_memory(self, chat_message_history: ChatMessageHistory) -> None:
-        if not chat_message_history.conversation_id:
-            chat_message_history.conversation_id = utils.generate_conversation_id()
-        cache[chat_message_history.conversation_id] = chat_message_history.listdict_message
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional, List, Dict
+
+from promptulate import utils
+from promptulate.memory.base import BaseChatMemory
+from promptulate.schema import MessageSet
+from promptulate.tips import EmptyMessageSetError
+
+logger = utils.get_logger()
+buffer: Dict[str, List[Dict]] = {}
+"""global message buffer, here is a buffer example: 
+{
+    "conversation_id1": [message...],
+    "conversation_id2": [message...],
+}
+"""
+
+
+class BufferChatMemory(BaseChatMemory):
+    """Chat message will be stored in the buffer cache."""
+
+    def load_message_set_from_memory(
+            self, recently_n: Optional[int] = None
+    ) -> MessageSet:
+        """Load message from buffer memory
+
+        Args:
+            recently_n: load all messages if it is None, or return recently n messages.
+
+        Returns:
+            messages wrapping by MessageSet
+        """
+        if not buffer:
+            raise EmptyMessageSetError
+        recently_n = (
+            recently_n if recently_n else len(buffer[self.conversation_id])
+        )
+        num_messages = len(buffer[self.conversation_id])
+        return MessageSet.from_listdict_data(
+            buffer[self.conversation_id][num_messages - recently_n:]
+        )
+
+    def save_message_set_to_memory(self, message_set: MessageSet) -> None:
+        buffer[self.conversation_id] = message_set.memory_messages
```

### Comparing `promptulate-1.2.0/promptulate/preset_roles/roles.py` & `promptulate-1.2.1/promptulate/preset_roles/roles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,88 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Union
-from pydantic import BaseModel
-
-
-class CustomPresetRole(BaseModel):
-    name: str
-    description: str
-
-
-preset_role_list = [
-    "default-role",
-    "linux-terminal",
-    "mind-map-generator",
-    "sql-generator",
-    "copy-writer",
-    "code-analyzer",
-]
-
-preset_role_dict = {
-    "default-role": {
-        "name": "AI assistant",
-        "description": """
-        你是人类的助手，由OpenAI训练的大型语言模型提供支持。
-        你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
-        你在不断地学习和进步，你的能力也在不断地发展。你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
-        总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。"""
-    },
-    "linux-terminal": {
-        "name": "Linux终端",
-        "description": """我想让你充当 Linux 终端。我将输入命令，您将回复终端应显示的内容。我希望您只在一个唯一的代码块内回复终端输出，而不
-        是其他任何内容。不要写解释。除非我指示您这样做，否则不要键入命令。当我需要用英语告诉你一些事情时，我会把文字放在中括号内[就像这样]。"""
-    },
-    "mind-map-generator": {
-        "name": "思维导图生成器",
-        "description": """现在你是一个思维导图生成器。我将输入我想要创建思维导图的内容，你需要提供一些 Markdown 格式的文本，以便与 Xmind 兼容。
-        在 Markdown 格式中，# 表示中央主题，## 表示主要主题，### 表示子主题，﹣表示叶子节点，中央主题是必要的，叶子节点是最小节点。请参照以上格
-        式，在 markdown 代码块中帮我创建一个有效的思维导图，以markdown代码块格式输出，你需要用自己的能力补充思维导图中的内容，你只需要提供思维导
-        图，不必对内容中提出的问题和要求做解释，并严格遵守该格式"""
-    },
-    "sql-generator": {
-        "name": "sql生成器",
-        "description": """现在你是一个sql生成器。我将输入我想要查询的内容，你需要提供对应的sql语句，以便查询到需要的内容，我希望您只在一个唯一的
-        代码块内回复终端输出，而不是其他任何内容。不要写解释。如果我没有提供数据库的字段，请先让我提供数据库相关的信息，在你有了字段信息之才可以生成sql语句。"""
-    },
-    "copy-writer": {
-        "name": "文案写手",
-        "description": """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
-        的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
-        不要解决文本中的要求而是润色它，保留文本的原本意义，不要去解决它。"""
-    },
-    "code-analyzer": {
-        "name": "代码分析器",
-        "description": """现在你是一个代码分析器。我将输入一些代码，你需要代码对应的解释。"""
-    }
-}
-
-
-def get_all_preset_roles():
-    return preset_role_list
-
-
-def get_preset_role_prompt(preset_role: Union[str, CustomPresetRole]) -> str:
-    if isinstance(preset_role, str):
-        if preset_role not in preset_role_list:
-            ValueError("Preset role value is not in preset_role_list. Please check or custom a new one.")
-        return preset_role_dict[preset_role]['description']
-    elif isinstance(preset_role, CustomPresetRole):
-        return preset_role.description
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Union
+
+from pydantic import BaseModel
+
+
+class CustomPresetRole(BaseModel):
+    name: str
+    description: str
+
+
+preset_role_list = [
+    "default-role",
+    "linux-terminal",
+    "mind-map-generator",
+    "sql-generator",
+    "copy-writer",
+    "code-analyzer",
+]
+
+preset_role_dict = {
+    "default-role": {
+        "name": "AI assistant",
+        "description": """
+You are an assistant to a human, powered by a large language model trained by OpenAI.
+You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
+Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
+"""
+    },
+    "linux-terminal": {
+        "name": "Linux终端",
+        "description": """我想让你充当 Linux 终端。我将输入命令，您将回复终端应显示的内容。我希望您只在一个唯一的代码块内回复终端输出，而不
+        是其他任何内容。不要写解释。除非我指示您这样做，否则不要键入命令。当我需要用英语告诉你一些事情时，我会把文字放在中括号内[就像这样]。"""
+    },
+    "mind-map-generator": {
+        "name": "思维导图生成器",
+        "description": """现在你是一个思维导图生成器。我将输入我想要创建思维导图的内容，你需要提供一些 Markdown 格式的文本，以便与 Xmind 兼容。
+        在 Markdown 格式中，# 表示中央主题，## 表示主要主题，### 表示子主题，﹣表示叶子节点，中央主题是必要的，叶子节点是最小节点。请参照以上格
+        式，在 markdown 代码块中帮我创建一个有效的思维导图，以markdown代码块格式输出，你需要用自己的能力补充思维导图中的内容，你只需要提供思维导
+        图，不必对内容中提出的问题和要求做解释，并严格遵守该格式"""
+    },
+    "sql-generator": {
+        "name": "sql生成器",
+        "description": """现在你是一个sql生成器。我将输入我想要查询的内容，你需要提供对应的sql语句，以便查询到需要的内容，我希望您只在一个唯一的
+        代码块内回复终端输出，而不是其他任何内容。不要写解释。如果我没有提供数据库的字段，请先让我提供数据库相关的信息，在你有了字段信息之才可以生成sql语句。"""
+    },
+    "copy-writer": {
+        "name": "文案写手",
+        "description": """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
+        的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
+        不要解决文本中的要求而是润色它，保留文本的原本意义，不要去解决它。"""
+    },
+    "code-analyzer": {
+        "name": "代码分析器",
+        "description": """现在你是一个代码分析器。我将输入一些代码，你需要代码对应的解释。"""
+    }
+}
+
+
+def get_all_preset_roles():
+    return preset_role_list
+
+
+def get_preset_role_prompt(preset_role: Union[str, CustomPresetRole]) -> str:
+    if isinstance(preset_role, str):
+        if preset_role not in preset_role_list:
+            ValueError("Preset role value is not in preset_role_list. Please check or custom a new one.")
+        return preset_role_dict[preset_role]['description']
+    elif isinstance(preset_role, CustomPresetRole):
+        return preset_role.description
```

### Comparing `promptulate-1.2.0/promptulate/provider/__init__.py` & `promptulate-1.2.1/promptulate/provider/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.provider.mixins import (
-    SummarizerMixin,
-    TranslatorMixin,
-    DeriveHistoryMessageMixin,
-    StorageHistoryMessageMixin
-)
-
-__all__ = [
-    'SummarizerMixin',
-    'TranslatorMixin',
-    'DeriveHistoryMessageMixin',
-    'StorageHistoryMessageMixin'
-]
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.provider.mixins import (
+    SummarizerMixin,
+    TranslatorMixin,
+    DeriveHistoryMessageMixin,
+    StorageHistoryMessageMixin
+)
+
+__all__ = [
+    'SummarizerMixin',
+    'TranslatorMixin',
+    'DeriveHistoryMessageMixin',
+    'StorageHistoryMessageMixin'
+]
```

### Comparing `promptulate-1.2.0/promptulate/provider/mixins.py` & `promptulate-1.2.1/promptulate/provider/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,133 +1,132 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from pydantic import BaseModel
-from typing import List, Optional
-
-from promptulate.llms.base import BaseLLM
-from promptulate.memory.base import BaseChatMemory
-from promptulate.frameworks.prompt import SUMMARY_CONTENT_PROMPT_ZH, SUMMARY_TOPIC_PROMPT_ZH
-from promptulate.schema import (
-    LLMPrompt,
-    UserMessage,
-    BaseMessage,
-    AssistantMessage,
-    ChatMessageHistory
-)
-
-
-class BaseMixin(BaseModel):
-    llm: BaseLLM
-    conversation_id: Optional[str]
-    memory: BaseChatMemory
-
-    class Config:
-        """Configuration for this pydantic object."""
-        arbitrary_types_allowed = True
-
-    def embed_message(self, cur_message: BaseMessage, message_history: ChatMessageHistory) -> None:
-        message_history.messages.append(cur_message)
-        self.memory.save_conversation_to_memory(message_history)
-
-
-class SummarizerMixin(BaseMixin):
-    """message summary capability provider"""
-
-    def summary_content(self, enable_embed_message: bool = False, summary_prompt: str = SUMMARY_CONTENT_PROMPT_ZH):
-        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
-        message_history.messages.append(UserMessage(content=summary_prompt))
-        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-    def summary_topic(self, enable_embed_message: bool = False, summary_topic_prompt: str = SUMMARY_TOPIC_PROMPT_ZH):
-        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
-        message_history.messages.append(
-            UserMessage(content=summary_topic_prompt))
-        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-
-class TranslatorMixin(BaseMixin):
-    """let the llm answer question in the specified language"""
-
-    def predict_by_translate(self, prompt: str, country: str, enable_embed_message: bool = False):
-        """
-        predict by specified language
-
-        Args:
-            enable_embed_message: Whether to save this session in the history session
-            prompt: you prompt
-            country: which country's language you want to export
-
-        Returns:
-            the country official language you choose
-        """
-        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
-        message_history.messages.append(
-            UserMessage(content=f"{prompt}. Please answer question using {country} official language. "))
-        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-
-class DeriveHistoryMessageMixin(BaseMixin):
-    """provide history message output as markdown"""
-
-    def get_history(self) -> List[dict]:
-        """get history conversation from memory"""
-        return self.memory.load_conversation_from_memory(self.conversation_id).listdict_message
-
-    def export_message_to_markdown(self, output_type: str = 'text', file_path: str = "output.md") -> Optional[str]:
-        """
-        convert message to the string type or file type markdown
-
-        Args:
-            output_type: text or file. default is text
-            file_path: output file path
-
-        Returns:
-            string type conversation in markdown format
-        """
-        message_history: List[dict] = self.get_history()
-
-        ret = "# Chat record\n"
-        for message in message_history:
-            role = message.get('preset_roles')
-            content = message.get('content').replace('"', '\\"')
-            if role == 'assistant':
-                ret += f"## Bot said\n\n{content}\n\n"
-            else:
-                ret += f"## You said\n\n{content}\n\n"
-        if output_type == 'text':
-            return ret
-        elif output_type == 'file':
-            with open(file_path, 'w', encoding="utf-8") as f:
-                f.write(ret)
-        else:
-            raise ValueError("Invalid output destination specified. Please choose either 'text' or 'file'.")
-        return ret
-
-
-class StorageHistoryMessageMixin(BaseModel):
-    pass
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import List, Optional
+
+from pydantic import BaseModel
+
+from promptulate.frameworks.prompt import (
+    SUMMARY_CONTENT_PROMPT_ZH,
+    SUMMARY_TOPIC_PROMPT_ZH,
+)
+from promptulate.provider.base import BaseMixin
+from promptulate.schema import MessageSet, UserMessage, AssistantMessage
+
+
+class SummarizerMixin(BaseMixin):
+    """message summary capability provider"""
+
+    def summary_content(
+        self,
+        enable_embed_message: bool = False,
+        summary_prompt: str = SUMMARY_CONTENT_PROMPT_ZH,
+    ):
+        message_history: MessageSet = self.memory.load_message_set_from_memory()
+        message_history.messages.append(UserMessage(content=summary_prompt))
+        assistant_answer: AssistantMessage = self.llm.predict(message_history)
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+    def summary_topic(
+        self,
+        enable_embed_message: bool = False,
+        summary_topic_prompt: str = SUMMARY_TOPIC_PROMPT_ZH,
+    ):
+        message_history: MessageSet = self.memory.load_message_set_from_memory()
+        message_history.messages.append(UserMessage(content=summary_topic_prompt))
+        assistant_answer: AssistantMessage = self.llm.predict(message_history)
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+
+class TranslatorMixin(BaseMixin):
+    """let the llm answer question in the specified language"""
+
+    def predict_by_translate(
+        self, prompt: str, country: str, enable_embed_message: bool = False
+    ):
+        """
+        predict by specified language
+
+        Args:
+            enable_embed_message: Whether to save this session in the history session
+            prompt: you prompt
+            country: which country's language you want to export
+
+        Returns:
+            the country official language you choose
+        """
+        message_history: MessageSet = self.memory.load_message_set_from_memory()
+        message_history.messages.append(
+            UserMessage(
+                content=f"{prompt}. Please answer question using {country} official language. "
+            )
+        )
+        assistant_answer: AssistantMessage = self.llm.predict(message_history)
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+
+class DeriveHistoryMessageMixin(BaseMixin):
+    """provide history message output as markdown"""
+
+    def get_history(self) -> List[dict]:
+        """get history conversation from memory"""
+        return self.memory.load_message_set_from_memory().listdict_messages
+
+    def export_message_to_markdown(
+        self, output_type: str = "text", file_path: str = "output.md"
+    ) -> Optional[str]:
+        """
+        convert message to the string type or file type markdown
+
+        Args:
+            output_type: text or file. default is text
+            file_path: output file path
+
+        Returns:
+            string type conversation in markdown format
+        """
+        message_history: List[dict] = self.get_history()
+
+        ret = "# Chat record\n"
+        for message in message_history:
+            role = message.get("preset_roles")
+            content = message.get("content").replace('"', '\\"')
+            if role == "assistant":
+                ret += f"## Bot said\n\n{content}\n\n"
+            else:
+                ret += f"## You said\n\n{content}\n\n"
+        if output_type == "text":
+            return ret
+        elif output_type == "file":
+            with open(file_path, "w", encoding="utf-8") as f:
+                f.write(ret)
+        else:
+            raise ValueError(
+                "Invalid output destination specified. Please choose either 'text' or 'file'."
+            )
+        return ret
+
+
+class StorageHistoryMessageMixin(BaseModel):
+    pass
```

### Comparing `promptulate-1.2.0/promptulate/schema.py` & `promptulate-1.2.1/promptulate/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,192 +1,167 @@
-import enum
-from abc import abstractmethod
-from typing import List, Dict, Callable
-
-from pydantic import BaseModel, Field
-
-from promptulate.utils import generate_conversation_id
-
-__all__ = [
-    "BaseMessage",
-    "BaseChatMessageHistory",
-    "SystemMessage",
-    "UserMessage",
-    "AssistantMessage",
-    "ChatMessageHistory",
-    "LLMPrompt",
-    "ListDictPrompt",
-    "init_chat_message_history",
-    'parse_llm_prompt_to_dict',
-    'parse_llm_dict_to_prompt'
-]
-
-
-class BaseMessage(BaseModel):
-    """Message basic object."""
-
-    content: str
-    additional_kwargs: dict = Field(default_factory=dict)
-
-    @property
-    @abstractmethod
-    def type(self) -> str:
-        """Type of the message, used for serialization."""
-
-
-class SystemMessage(BaseMessage):
-    """Type of message that is a system message. Currently used in OpenAI."""
-
-    @property
-    def type(self) -> str:
-        """Type of the message, used for serialization."""
-        return "system"
-
-
-class UserMessage(BaseMessage):
-    """Type of message that is a user message. Currently used in OpenAI."""
-
-    @property
-    def type(self) -> str:
-        return "user"
-
-
-class AssistantMessage(BaseMessage):
-    """Type of message that is an assistant message. Currently used in OpenAI."""
-
-    @property
-    def type(self) -> str:
-        return "assistant"
-
-
-class BaseChatMessageHistory(BaseModel):
-    """Base interface for chat message history
-    See `ChatMessageHistory` for default implementation.
-    """
-
-    messages: List[BaseMessage]
-    conversation_id: str
-
-    @abstractmethod
-    def add_system_message(self, message):
-        """add a system message"""
-
-    @abstractmethod
-    def add_user_message(self, message):
-        """add a user message"""
-
-    @abstractmethod
-    def add_ai_message(self, message):
-        """add a ai message"""
-
-    @abstractmethod
-    def clear(self):
-        """clear all message"""
-
-
-class ChatMessageHistory(BaseModel):
-    messages: List[BaseMessage] = []
-    conversation_id: str = ""
-
-    def add_system_message(self, message: str) -> None:
-        self.messages.append(SystemMessage(content=message))
-
-    def add_user_message(self, message: str) -> None:
-        self.messages.append(UserMessage(content=message))
-
-    def add_ai_message(self, message: str) -> None:
-        self.messages.append(AssistantMessage(content=message))
-
-    def clear(self) -> None:
-        self.messages = []
-
-    @property
-    def listdict_message(self) -> List[dict]:
-        listdict_message: List[dict] = []
-        for message in self.messages:
-            listdict_message.append({"role": message.type, "content": message.content})
-        return listdict_message
-
-
-def init_chat_message_history(system_content, user_content) -> ChatMessageHistory:
-    messages = [
-        SystemMessage(content=system_content),
-        UserMessage(content=user_content),
-    ]
-    return ChatMessageHistory(
-        messages=messages, conversation_id=generate_conversation_id()
-    )
-
-
-class LLMPrompt(BaseModel):
-    messages: List[BaseMessage]
-
-
-class ListDictPrompt(BaseModel):
-    """list dict type prompt. It can convert to ChatMessageHistory type."""
-
-    messages: List[Dict[str, str]]
-
-    @property
-    def chat_message_history(self) -> ChatMessageHistory:
-        message_history = ChatMessageHistory()
-        for message in self.messages:
-            role = message.get("role")
-            content = message.get("content")
-            if role == "system":
-                message_history.messages.append(SystemMessage(content=content))
-            elif role == "user":
-                message_history.messages.append(UserMessage(content=content))
-            elif role == "assistant":
-                message_history.messages.append(AssistantMessage(content=content))
-        return message_history
-
-
-class LLMType(enum.Enum):
-    OpenAI = "OpenAI"
-
-
-def _parse_openai_prompt_to_dict(prompts: LLMPrompt) -> List[Dict]:
-    converted_messages: List[dict] = []
-    for message in prompts.messages:
-        converted_messages.append({"role": message.type, "content": message.content})
-    return converted_messages
-
-
-_parse_llm_prompt_to_dict: Dict[LLMType, Callable] = {
-    LLMType.OpenAI: _parse_openai_prompt_to_dict
-}
-
-
-def _parse_dict_to_openai_prompt(prompts: List[Dict[str, str]]) -> LLMPrompt:
-    messages: List[BaseMessage] = []
-    for prompt in prompts:
-        if prompt["type"] == "system":
-            messages.append(SystemMessage(content=prompt["message"]))
-        elif prompt["type"] == "user":
-            messages.append(UserMessage(content=prompt["message"]))
-        elif prompt["type"] == "assistant":
-            messages.append(AssistantMessage(content=prompt["message"]))
-    return LLMPrompt(messages=messages)
-
-
-_parse_llm_dict_to_prompt: Dict[LLMType, Callable] = {
-    LLMType.OpenAI: _parse_dict_to_openai_prompt
-}
-
-
-def parse_llm_prompt_to_dict(
-        prompts: LLMPrompt, llm_type: LLMType = LLMType.OpenAI
-) -> List[Dict]:
-    """This method is compatible with different LLMs.
-    You can convert LLMPrompt Data to Json Data of different LLMs format.
-    """
-    return _parse_llm_prompt_to_dict[llm_type](prompts)
-
-
-def parse_llm_dict_to_prompt(
-        prompts: List[Dict[str, str]], llm_type: LLMType = LLMType.OpenAI
-) -> LLMPrompt:
-    """This method is compatible with different LLMs.
-    You can convert JSON Data to LLMPrompt Data of different LLMs format.
-    """
-    return _parse_llm_dict_to_prompt[llm_type](prompts)
+from abc import abstractmethod
+from enum import Enum
+from typing import List, Dict, Callable, Any, Optional
+
+from pydantic import BaseModel, Field
+
+__all__ = [
+    "BaseMessage",
+    "CompletionMessage",
+    "SystemMessage",
+    "UserMessage",
+    "AssistantMessage",
+    "MessageSet",
+    "init_chat_message_history",
+]
+
+
+class BaseMessage(BaseModel):
+    """Message basic object."""
+
+    content: str
+    additional_kwargs: dict = Field(default_factory=dict)
+
+    @property
+    @abstractmethod
+    def type(self) -> str:
+        """Type of the message, used for serialization."""
+
+
+class CompletionMessage(BaseMessage):
+    """Type of completion message. Used in OpenAI currently"""
+
+    @property
+    def type(self) -> str:
+        return "completion"
+
+
+class SystemMessage(BaseMessage):
+    """Type of message that is a system message. Currently used in OpenAI."""
+
+    @property
+    def type(self) -> str:
+        """Type of the message, used for serialization."""
+        return "system"
+
+
+class UserMessage(BaseMessage):
+    """Type of message that is a user message. Currently used in OpenAI."""
+
+    @property
+    def type(self) -> str:
+        return "user"
+
+
+class AssistantMessage(BaseMessage):
+    """Type of message that is an assistant message. Currently used in OpenAI."""
+
+    @property
+    def type(self) -> str:
+        return "assistant"
+
+
+MESSAGE_TYPE = {
+    "completion": CompletionMessage,
+    "system": SystemMessage,
+    "user": UserMessage,
+    "assistant": AssistantMessage,
+}
+
+
+class LLMType(str, Enum):
+    """All LLM type here"""
+
+    OpenAI = "OpenAI"
+    ChatOpenAI = "ChatOpenAI"
+
+
+class MessageSet(BaseModel):
+    """MessageSet can be used in Memory, LLMs, Framework and some else.
+    It's a universal chat message format in promptulate.
+    """
+
+    messages: List[BaseMessage] = []
+    conversation_id: Optional[str] = None
+    """Used to memory"""
+
+    @classmethod
+    def from_listdict_data(cls, value: List[Dict]) -> "MessageSet":
+        """initialize MessageSet from a List[Dict] data
+
+        Args:
+            value(List[Dict]): the example is as follow:
+                [
+                    {"type": "user", "content": "This is a message1."},
+                    {"type": "assistant", "content": "This is a message2."}
+                ]
+
+        Returns:
+            initialized MessageSet
+        """
+        messages: List[BaseMessage] = [
+            MESSAGE_TYPE[item["role"]](content=item["content"]) for item in value
+        ]
+        return cls(messages=messages)
+
+    @property
+    def listdict_messages(self) -> List[Dict]:
+        converted_messages = []
+        for message in self.messages:
+            converted_messages.append(
+                {"role": message.type, "content": message.content}
+            )
+        return converted_messages
+
+    @property
+    def memory_messages(self) -> List[Dict]:
+        return self.listdict_messages
+
+    def to_llm_prompt(self, llm_type: LLMType) -> Any:
+        """Convert the MessageSet messages to specified llm prompt"""
+        if not llm_type:
+            ValueError(
+                "Missing llm_type, you should pass a llm_type if you want to use llm_prompt"
+            )
+        return _to_llm_prompt[llm_type](self)
+
+    @property
+    def string_messages(self) -> str:
+        """Convert the message to a string type, it can be used as a prompt for OpenAI completion."""
+        string_result = ""
+        for message in self.messages:
+            string_result += f"{message.content}\n"
+        return string_result
+
+    def add_completion_message(self, message: str) -> None:
+        self.messages.append(CompletionMessage(content=message))
+
+    def add_system_message(self, message: str) -> None:
+        self.messages.append(SystemMessage(content=message))
+
+    def add_user_message(self, message: str) -> None:
+        self.messages.append(UserMessage(content=message))
+
+    def add_ai_message(self, message: str) -> None:
+        self.messages.append(AssistantMessage(content=message))
+
+
+def init_chat_message_history(system_content, user_content) -> MessageSet:
+    messages = [
+        SystemMessage(content=system_content),
+        UserMessage(content=user_content),
+    ]
+    return MessageSet(messages=messages)
+
+
+def _to_openai_llm_prompt(message_set: MessageSet) -> str:
+    return message_set.string_messages
+
+
+def _to_chat_openai_llm_prompt(message_set: MessageSet) -> List[Dict]:
+    return message_set.listdict_messages
+
+
+_to_llm_prompt: Dict[LLMType, Callable] = {
+    LLMType.OpenAI: _to_openai_llm_prompt,
+    LLMType.ChatOpenAI: _to_chat_openai_llm_prompt,
+}
```

### Comparing `promptulate-1.2.0/promptulate/tools/arxiv/api_wrapper.py` & `promptulate-1.2.1/promptulate/tools/arxiv/api_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,141 +1,140 @@
-from typing import List, Dict, Optional, Union
-
-import arxiv
-from pydantic import BaseModel, Extra, root_validator
-
-
-class ArxivQuerySet:
-    def __init__(self, search: arxiv.Search, keys: Optional[List[str]] = None):
-        self.search: arxiv.Search = search
-        self._data: List[Dict] = []
-
-        for result in search.results():
-            if keys:
-                filtered_result_dict = {
-                    k: result.__dict__[k] for k in keys if k in result.__dict__
-                }
-                self._data.append(filtered_result_dict)
-            else:
-                self._data.append(result.__dict__)
-
-    def __str__(self):
-        result: str = ""
-        for item in self._data:
-            result += f"{item.__dict__}\n"
-        return result
-
-    def titles(self) -> List[str]:
-        titles: List[str] = []
-        for item in self.search.results():
-            titles.append(item.title)
-        return titles
-
-    def all(self) -> List[Dict]:
-        return self._data
-
-    def first(self) -> Optional[Dict]:
-        if len(self._data) == 0:
-            return None
-        return self._data[0]
-
-    @classmethod
-    def from_filter_result(cls, search: arxiv.Search, *args):
-        """generate a filter key queryset"""
-        return cls(search, list(args))
-
-
-class ArxivAPIWrapper(BaseModel):
-    """https://github.com/lukasschwab/arxiv.py"""
-
-    max_num_of_result: int = 5
-    sort_by = arxiv.SortCriterion.Relevance
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
-    @root_validator()
-    def validate_environment(cls, values: Dict) -> Dict:
-        """Validate that python package exists in environment."""
-        try:
-            import arxiv
-        except ImportError:
-            raise ValueError(
-                "Could not import arxiv python package. "
-                "Please install it with `pip install arxiv`."
-            )
-        return values
-
-    def _query(
-        self,
-        keyword: Optional[str] = None,
-        id_list: Union[List[str], str, None] = None,
-        num_results: Optional[int] = None,
-    ) -> arxiv.Search:
-        """
-        query arxiv paper by keyword or id_list
-        Args:
-            keyword: query keyword
-            id_list: arxiv id, you can input multiple id or single
-        Returns:
-            arxiv search type data result
-        """
-        if not keyword:
-            keyword = ""
-        if not id_list:
-            id_list = []
-        if not num_results:
-            num_results = self.max_num_of_result
-        if isinstance(id_list, str):
-            id_list = [id_list]
-
-        search = arxiv.Search(
-            query=keyword,
-            id_list=id_list,
-            max_results=num_results,
-            sort_by=self.sort_by,
-        )
-        return search
-
-    def query(
-        self,
-        keyword: Optional[str] = None,
-        id_list: Union[List[str], str, None] = None,
-        num_results: Optional[int] = None,
-        **kwargs,
-    ) -> List[Dict]:
-        """
-        Query arxiv paper by keyword or id_list. You can make ArxivQuerySet return the
-        specified fields from arxiv query result.
-        Args:
-            num_results: max num of result. Return self.max_num_of_result if none
-            keyword: query keyword
-            id_list: arxiv id, you can input multiple id or single
-            kwargs:
-                specified_fields(Optional[List[str]]): filter specified field to return.
-                For example, you can return the ["title", "summary"] fields from each arxiv query result
-        Returns:
-            List[Dict] type result
-        Examples:
-            If you want to get paper title and summary, you can do as follows.
-
-            >> arxiv_api_wrapper = ArxivAPIWrapper()
-            >> result = arxiv_api_wrapper.query("LLM", specified_fields=["entry_id", "title", "summary"])
-
-            All fields you can see in: https://github.com/lukasschwab/arxiv.py
-            Common fields are: ["entry_id", "title", "authors", "summary", "published"]
-        """
-        search = self._query(keyword, id_list, num_results)
-        if "specified_fields" in kwargs:
-            return ArxivQuerySet.from_filter_result(
-                search, *kwargs["specified_fields"]
-            ).all()
-        if "from_callback" in kwargs and kwargs["from_callback"] == "arxiv-query":
-            keys = ["entry_id", "title", "authors", "summary"]
-            return ArxivQuerySet.from_filter_result(search, *keys).all()
-        return ArxivQuerySet(search).all()
-
-    def download_pdf(self, id_list: List[str]) -> str:
-        paper = next(arxiv.Search(id_list=id_list).results())
-        return paper.download_pdf()
+from typing import List, Dict, Optional, Union
+
+import arxiv
+from pydantic import BaseModel, root_validator
+
+
+class ArxivQuerySet:
+    def __init__(self, search: arxiv.Search, keys: Optional[List[str]] = None):
+        self.search: arxiv.Search = search
+        self._data: List[Dict] = []
+
+        for result in search.results():
+            if keys:
+                filtered_result_dict = {
+                    k: result.__dict__[k] for k in keys if k in result.__dict__
+                }
+                self._data.append(filtered_result_dict)
+            else:
+                self._data.append(result.__dict__)
+
+    def __str__(self):
+        result: str = ""
+        for item in self._data:
+            result += f"{item.__dict__}\n"
+        return result
+
+    def titles(self) -> List[str]:
+        titles: List[str] = []
+        for item in self.search.results():
+            titles.append(item.title)
+        return titles
+
+    def all(self) -> List[Dict]:
+        return self._data
+
+    def first(self) -> Optional[Dict]:
+        if len(self._data) == 0:
+            return None
+        return self._data[0]
+
+    @classmethod
+    def from_filter_result(cls, search: arxiv.Search, *args):
+        """generate a filter key queryset"""
+        return cls(search, list(args))
+
+
+class ArxivAPIWrapper(BaseModel):
+    """https://github.com/lukasschwab/arxiv.py"""
+
+    max_num_of_result: int = 5
+    sort_by = arxiv.SortCriterion.Relevance
+
+    class Config:
+        """Configuration for this pydantic object."""
+        arbitrary_types_allowed = True
+
+    @root_validator(skip_on_failure=True)
+    def validate_environment(cls, values: Dict) -> Dict:
+        """Validate that python package exists in environment."""
+        try:
+            import arxiv
+        except ImportError:
+            raise ValueError(
+                "Could not import arxiv python package. "
+                "Please install it with `pip install arxiv`."
+            )
+        return values
+
+    def _query(
+            self,
+            keyword: Optional[str] = None,
+            id_list: Union[List[str], str, None] = None,
+            num_results: Optional[int] = None,
+    ) -> arxiv.Search:
+        """
+        query arxiv paper by keyword or id_list
+        Args:
+            keyword: query keyword
+            id_list: arxiv id, you can input multiple id or single
+        Returns:
+            arxiv search type data result
+        """
+        if not keyword:
+            keyword = ""
+        if not id_list:
+            id_list = []
+        if not num_results:
+            num_results = self.max_num_of_result
+        if isinstance(id_list, str):
+            id_list = [id_list]
+
+        search = arxiv.Search(
+            query=keyword,
+            id_list=id_list,
+            max_results=num_results,
+            sort_by=self.sort_by,
+        )
+        return search
+
+    def query(
+            self,
+            keyword: Optional[str] = None,
+            id_list: Union[List[str], str, None] = None,
+            num_results: Optional[int] = None,
+            **kwargs,
+    ) -> List[Dict]:
+        """
+        Query arxiv paper by keyword or id_list. You can make ArxivQuerySet return the
+        specified fields from arxiv query result.
+        Args:
+            num_results: max num of result. Return self.max_num_of_result if none
+            keyword: query keyword
+            id_list: arxiv id, you can input multiple id or single
+            kwargs:
+                specified_fields(Optional[List[str]]): filter specified field to return.
+                For example, you can return the ["title", "summary"] fields from each arxiv query result
+        Returns:
+            List[Dict] type result
+        Examples:
+            If you want to get paper title and summary, you can do as follows.
+
+            >> arxiv_api_wrapper = ArxivAPIWrapper()
+            >> result = arxiv_api_wrapper.query("LLM", specified_fields=["entry_id", "title", "summary"])
+
+            All fields you can see in: https://github.com/lukasschwab/arxiv.py
+            Common fields are: ["entry_id", "title", "authors", "summary", "published"]
+        """
+        search = self._query(keyword, id_list, num_results)
+        if "specified_fields" in kwargs:
+            return ArxivQuerySet.from_filter_result(
+                search, *kwargs["specified_fields"]
+            ).all()
+        if "from_callback" in kwargs and kwargs["from_callback"] == "arxiv-query":
+            keys = ["entry_id", "title", "authors", "summary"]
+            return ArxivQuerySet.from_filter_result(search, *keys).all()
+        return ArxivQuerySet(search).all()
+
+    def download_pdf(self, id_list: List[str]) -> str:
+        paper = next(arxiv.Search(id_list=id_list).results())
+        return paper.download_pdf()
```

### Comparing `promptulate-1.2.0/promptulate/tools/arxiv/tools.py` & `promptulate-1.2.1/promptulate/tools/arxiv/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import re
-import time
-from typing import List, Dict, Union
-
-from broadcast_service import broadcast_service
-from pydantic import Field
-
-from promptulate.llms.base import BaseLLM
-from promptulate.llms.openai import OpenAI
-from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
-from promptulate.tools.base import BaseTool
-from promptulate.utils.core_utils import record_time, listdict_to_string
-from promptulate.utils.logger import get_logger
-
-logger = get_logger()
-
-
-class ArxivQueryTool(BaseTool):
-    name = "arxiv-query"
-    description = (
-        "A query tool around Arxiv.org "
-        "Useful for when you need to answer questions about Physics, Mathematics, "
-        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
-        "Electrical Engineering, and Economics "
-        "from scientific articles on arxiv.org. "
-        "Input should be a search query."
-    )
-    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        """Arxiv query tool
-
-        Args:
-            query: the paper keyword or arxiv id
-            **kwargs:
-                return_type(Optional(str)):  return string default. If you want to return List[Dict] type data,
-                you can set 'return_type'='original'
-                Moreover, you can pass the arguments of ArxivAPIWrapper
-
-        Returns:
-            String type or List[Dict] arxiv query result.
-        """
-        kwargs.update({"from_callback": self.name})
-        if re.match("\d{4}\.\d{5}(v\d+)?", query):
-            result = self.api_wrapper.query(id_list=[query], **kwargs)
-        else:
-            result = self.api_wrapper.query(query, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return listdict_to_string(result)
-        return result
-
-
-def _init_arxiv_reference_tool_llm():
-    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
-    return OpenAI(preset_description=preset, temperature=0)
-
-
-class ArxivReferenceTool(BaseTool):
-    name = "arxiv-reference"
-    description = (
-        "Use this tool to find search related to the field."
-        "Your input is a arxiv keyword query."
-    )
-    llm: BaseLLM = Field(default_factory=_init_arxiv_reference_tool_llm)
-    max_reference_num = 3
-    reference_string: str = ""
-    reference_counter: int = 0
-
-    @record_time()
-    def run(self, query: str, *args, **kwargs) -> Union[List[Dict], str]:
-        """
-        Input arxiv paper information and return paper references.
-        Args:
-            query(str): arxiv paper information
-            *args: Nothing
-            **kwargs:
-                return_type(Optional[str]): return string default. If you want to return List[Dict] type data,
-                you can set 'return_type'='original'
-        Returns:
-            String type or List[Dict] reference information
-        """
-
-        @broadcast_service.on_listen("ArxivReferenceTool.get_relevant_paper_info")
-        @record_time()
-        def get_relevant_paper_info(keyword: str):
-            """return paper related information from keyword"""
-            arxiv_query_tool = ArxivQueryTool()
-            specified_fields = ["entry_id", "title"]
-            queryset = arxiv_query_tool.run(
-                keyword, num_results=6, specified_fields=specified_fields
-            )
-            self.reference_string += queryset
-            self.reference_counter += 1
-
-        def analyze_query_string(query_string: str) -> List[str]:
-            """analyze `[query]: keyword1, keyword2, keyword3` type data to return keywords list"""
-            assert "[query]" in query_string
-            query_string = query_string.split(":")[1]
-            return query_string.split(",")
-
-        def analyze_reference_string(reference_string: str) -> List[Dict]:
-            pattern = r"\[(\d+)\]\s+(.+?),\s+(http://.+?);"
-            references = []
-            for match in re.finditer(pattern, reference_string):
-                references.append({"title": match.group(2), "url": match.group(3)})
-            return references
-
-        self.reference_counter = 0
-        prompt = (
-            f"现在你需要根据其研究的具体内容，列出至少{self.max_reference_num}篇参考文献，你可以使用arxiv进行查询，你需要给我提供3个arxiv查询关键词，我将使用"
-            f"arxiv进行查询，你需要根据我返回的结果选取最符合当前研究的{self.max_reference_num}篇参考文献。"
-            f"用户输入:{query}"
-            "你的输出必须是三个查询词\n，如 [query]: keyword1, keyword2, keyword3\n"
-        )
-        keywords = analyze_query_string(self.llm(prompt))
-        for keyword in keywords:
-            broadcast_service.broadcast(
-                "ArxivReferenceTool.get_relevant_paper_info", keyword
-            )
-
-        while self.reference_counter < 3:
-            time.sleep(0.2)
-
-        prompt = (
-            "现在你需要根据下面给出的论文，返回最合适的5篇参考文献\n"
-            f"```{self.reference_string}```\n"
-            "你的输出格式必须为\n参考文献:\n[1] [title1](url1);\n[2] [title2](url2);\n[3] [title3](url3);"
-        )
-        # todo If there is a problem with the returned format and an error is reported, then ask LLM to format the data
-        result = self.llm(prompt)
-        logger.debug(f"[promptulate ArxivReferenceTool response] {result}")
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return analyze_reference_string(result)
-        return result
-
-
-def _init_arxiv_summary_tool_llm():
-    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
-    return OpenAI(preset_description=preset, temperature=0)
-
-
-class ArxivSummaryTool(BaseTool):
-    name = "arxiv-summary"
-    description = (
-        "A summary tool that can be used to obtain a paper summary, listing "
-        "key insights and lessons learned in the paper, and references in the paper"
-        "Your input is a arxiv keyword query."
-    )
-    llm: BaseLLM = Field(default_factory=_init_arxiv_summary_tool_llm)
-    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
-    summary_string: str = ""
-    summary_counter: int = 0
-
-    def run(self, query: str, **kwargs) -> str:
-        """An arxiv paper summary tool that passes in the article name (or arxiv id) and returns summary results
-
-        Args:
-            query: the keyword you want to query
-            **kwargs:
-                You can pass the arguments of ArxivAPIWrapper
-
-        Returns:
-            String type data, which contains:
-            - Summary of the paper
-            - List the key insights and lessons learned in the paper
-            - List at least 5 references related to the research field of the paper
-        """
-
-        @broadcast_service.on_listen("ArxivSummaryTool.run.get_opinion")
-        def get_opinion():
-            prompt = (
-                f"请就下面的论文摘要，列出论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
-                "你的输出格式为:\n关键见解:\n{分点给出关键见解}\n经验教训:\n{分点给出经验教训}，用`-`区分每点，用中文输出"
-            )
-            opinion = self.llm(prompt)
-            self.summary_string += opinion + "\n"
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("ArxivSummaryTool.run.get_references")
-        def get_references():
-            arxiv_referencer_tool = ArxivReferenceTool()
-            references = arxiv_referencer_tool.run(paper_summary)
-            self.summary_string += references + "\n\n"
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("ArxivSummaryTool.run.get_advice")
-        def get_advice():
-            prompt = (
-                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
-                "你的输出格式为:\n相关建议:\n{分点给出相关建议}，用`-`区分每点"
-            )
-            opinion = self.llm(prompt)
-            self.summary_string += opinion + "\n"
-            self.summary_counter += 1
-
-        self.summary_counter = 0
-        if re.match("\d{4}\.\d{5}(v\d+)?", query):
-            paper_info = self.api_wrapper.query(
-                id_list=[query], num_results=1, specified_fields=["title", "summary"]
-            )
-        else:
-            paper_info = self.api_wrapper.query(
-                query, num_results=1, specified_fields=["title", "summary"]
-            )
-            if len(paper_info) == 0:
-                return "Could not find relevant arxiv article."
-        paper_summary = listdict_to_string(paper_info, item_suffix="\n")
-        self.summary_string = paper_summary
-
-        broadcast_service.publish("ArxivSummaryTool.run.get_references")
-        time.sleep(0.01)
-        broadcast_service.publish("ArxivSummaryTool.run.get_opinion")
-        time.sleep(0.01)
-        broadcast_service.publish("ArxivSummaryTool.run.get_advice")
-
-        while self.summary_counter < 3:
-            time.sleep(0.1)
-
-        return self.summary_string
+import re
+import time
+from typing import List, Dict, Union
+
+from broadcast_service import broadcast_service
+from pydantic import Field
+
+from promptulate.llms.base import BaseLLM
+from promptulate.llms.openai import OpenAI
+from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
+from promptulate.tools.base import BaseTool
+from promptulate.utils.core_utils import record_time, listdict_to_string
+from promptulate.utils.logger import get_logger
+
+logger = get_logger()
+
+
+class ArxivQueryTool(BaseTool):
+    name: str = "arxiv-query"
+    description: str = (
+        "A query tool around Arxiv.org "
+        "Useful for when you need to answer questions about Physics, Mathematics, "
+        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
+        "Electrical Engineering, and Economics "
+        "from scientific articles on arxiv.org. "
+        "Input should be a search query."
+    )
+    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
+
+    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        """Arxiv query tool
+
+        Args:
+            query: the paper keyword or arxiv id
+            **kwargs:
+                return_type(Optional(str)):  return string default. If you want to return List[Dict] type data,
+                you can set 'return_type'='original'
+                Moreover, you can pass the arguments of ArxivAPIWrapper
+
+        Returns:
+            String type or List[Dict] arxiv query result.
+        """
+        kwargs.update({"from_callback": self.name})
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            result = self.api_wrapper.query(id_list=[query], **kwargs)
+        else:
+            result = self.api_wrapper.query(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return listdict_to_string(result)
+        return result
+
+
+def _init_arxiv_reference_tool_llm():
+    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return OpenAI(preset_description=preset, temperature=0)
+
+
+class ArxivReferenceTool(BaseTool):
+    name: str = "arxiv-reference"
+    description: str = (
+        "Use this tool to find search related to the field."
+        "Your input is a arxiv keyword query."
+    )
+    llm: BaseLLM = Field(default_factory=_init_arxiv_reference_tool_llm)
+    max_reference_num = 3
+    reference_string: str = ""
+    reference_counter: int = 0
+
+    @record_time()
+    def run(self, query: str, *args, **kwargs) -> Union[List[Dict], str]:
+        """
+        Input arxiv paper information and return paper references.
+        Args:
+            query(str): arxiv paper information
+            *args: Nothing
+            **kwargs:
+                return_type(Optional[str]): return string default. If you want to return List[Dict] type data,
+                you can set 'return_type'='original'
+        Returns:
+            String type or List[Dict] reference information
+        """
+
+        @broadcast_service.on_listen("ArxivReferenceTool.get_relevant_paper_info")
+        @record_time()
+        def get_relevant_paper_info(keyword: str):
+            """return paper related information from keyword"""
+            arxiv_query_tool = ArxivQueryTool()
+            specified_fields = ["entry_id", "title"]
+            queryset = arxiv_query_tool.run(
+                keyword, num_results=6, specified_fields=specified_fields
+            )
+            self.reference_string += queryset
+            self.reference_counter += 1
+
+        def analyze_query_string(query_string: str) -> List[str]:
+            """analyze `[query]: keyword1, keyword2, keyword3` type data to return keywords list"""
+            assert "[query]" in query_string
+            query_string = query_string.split(":")[1]
+            return query_string.split(",")
+
+        def analyze_reference_string(reference_string: str) -> List[Dict]:
+            pattern = r"\[(\d+)\]\s+(.+?),\s+(http://.+?);"
+            references = []
+            for match in re.finditer(pattern, reference_string):
+                references.append({"title": match.group(2), "url": match.group(3)})
+            return references
+
+        self.reference_counter = 0
+        prompt = (
+            f"现在你需要根据其研究的具体内容，列出至少{self.max_reference_num}篇参考文献，你可以使用arxiv进行查询，你需要给我提供3个arxiv查询关键词，我将使用"
+            f"arxiv进行查询，你需要根据我返回的结果选取最符合当前研究的{self.max_reference_num}篇参考文献。"
+            f"用户输入:{query}"
+            "你的输出必须是三个查询词\n，如 [query]: keyword1, keyword2, keyword3\n"
+        )
+        keywords = analyze_query_string(self.llm(prompt))
+        for keyword in keywords:
+            broadcast_service.broadcast(
+                "ArxivReferenceTool.get_relevant_paper_info", keyword
+            )
+
+        while self.reference_counter < 3:
+            time.sleep(0.2)
+
+        prompt = (
+            "现在你需要根据下面给出的论文，返回最合适的5篇参考文献\n"
+            f"```{self.reference_string}```\n"
+            "你的输出格式必须为\n参考文献:\n[1] [title1](url1);\n[2] [title2](url2);\n[3] [title3](url3);"
+        )
+        # todo If there is a problem with the returned format and an error is reported, then ask LLM to format the data
+        result = self.llm(prompt)
+        logger.debug(f"[promptulate ArxivReferenceTool response] {result}")
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return analyze_reference_string(result)
+        return result
+
+
+def _init_arxiv_summary_tool_llm():
+    preset = "你是一个Arxiv助手，你的任务是帮助使用者提供一些论文方面的建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return OpenAI(preset_description=preset, temperature=0)
+
+
+class ArxivSummaryTool(BaseTool):
+    name: str = "arxiv-summary"
+    description: str = (
+        "A summary tool that can be used to obtain a paper summary, listing "
+        "key insights and lessons learned in the paper, and references in the paper"
+        "Your input is a arxiv keyword query."
+    )
+    llm: BaseLLM = Field(default_factory=_init_arxiv_summary_tool_llm)
+    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
+    summary_string: str = ""
+    summary_counter: int = 0
+
+    def run(self, query: str, **kwargs) -> str:
+        """An arxiv paper summary tool that passes in the article name (or arxiv id) and returns summary results
+
+        Args:
+            query: the keyword you want to query
+            **kwargs:
+                You can pass the arguments of ArxivAPIWrapper
+
+        Returns:
+            String type data, which contains:
+            - Summary of the paper
+            - List the key insights and lessons learned in the paper
+            - List at least 5 references related to the research field of the paper
+        """
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_opinion")
+        def get_opinion():
+            prompt = (
+                f"请就下面的论文摘要，列出论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
+                "你的输出格式为:\n关键见解:\n{分点给出关键见解}\n经验教训:\n{分点给出经验教训}，用`-`区分每点，用中文输出"
+            )
+            opinion = self.llm(prompt)
+            self.summary_string += opinion + "\n"
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_references")
+        def get_references():
+            arxiv_referencer_tool = ArxivReferenceTool()
+            references = arxiv_referencer_tool.run(paper_summary)
+            self.summary_string += references + "\n\n"
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("ArxivSummaryTool.run.get_advice")
+        def get_advice():
+            prompt = (
+                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
+                "你的输出格式为:\n相关建议:\n{分点给出相关建议}，用`-`区分每点"
+            )
+            opinion = self.llm(prompt)
+            self.summary_string += opinion + "\n"
+            self.summary_counter += 1
+
+        self.summary_counter = 0
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            paper_info = self.api_wrapper.query(
+                id_list=[query], num_results=1, specified_fields=["title", "summary"]
+            )
+        else:
+            paper_info = self.api_wrapper.query(
+                query, num_results=1, specified_fields=["title", "summary"]
+            )
+            if len(paper_info) == 0:
+                return "Could not find relevant arxiv article."
+        paper_summary = listdict_to_string(paper_info, item_suffix="\n")
+        self.summary_string = paper_summary
+
+        broadcast_service.publish("ArxivSummaryTool.run.get_references")
+        time.sleep(0.01)
+        broadcast_service.publish("ArxivSummaryTool.run.get_opinion")
+        time.sleep(0.01)
+        broadcast_service.publish("ArxivSummaryTool.run.get_advice")
+
+        while self.summary_counter < 3:
+            time.sleep(0.1)
+
+        return self.summary_string
```

### Comparing `promptulate-1.2.0/promptulate/tools/duckduckgo/api_wrapper.py` & `promptulate-1.2.1/promptulate/tools/duckduckgo/api_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from typing import List, Optional, Dict
-
-from pydantic import BaseModel, Extra
-from pydantic.class_validators import root_validator
-
-
-class DuckDuckGoSearchAPIWrapper(BaseModel):
-    """Wrapper for DuckDuckGo Search API. Free and does not require any setup."""
-
-    region: Optional[str] = "cn-zh"
-    safe_search: str = "moderate"
-    time: Optional[str] = "y"
-    max_num_of_results: int = 5
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
-    @root_validator()
-    def validate_environment(cls, values: Dict) -> Dict:
-        """Validate that python package exists in environment."""
-        try:
-            from duckduckgo_search import DDGS
-        except ImportError:
-            raise ValueError(
-                "Could not import duckduckgo-search python package. "
-                "Please install it with `pip install duckduckgo-search`."
-            )
-        return values
-
-    def query(
-            self, keyword: str, num_results: Optional[int] = None, **kwargs
-    ) -> List[str]:
-        """Run query through DuckDuckGo and return concatenated results."""
-        from duckduckgo_search import DDGS
-
-        if not num_results:
-            num_results = self.max_num_of_results
-
-        with DDGS() as ddgs:
-            results = ddgs.text(
-                keyword,
-                region=self.region,
-                safesearch=self.safe_search,
-                timelimit=self.time,
-            )
-            if results is None or next(results, None) is None:
-                return ["No good DuckDuckGo Search Result was found"]
-
-            snippets = []
-            for i, result in enumerate(results, 1):
-                snippets.append(result["body"])
-                if i == num_results:
-                    break
-            return snippets
-
-    def query_by_formatted_results(
-            self, query: str, num_results: Optional[int] = None, **kwargs
-    ) -> List[Dict[str, str]]:
-        """Run query through DuckDuckGo and return metadata.
-
-        Args:
-            query: The query to search for.
-            num_results: The number of results to return.
-
-        Returns:
-            A list of dictionaries with the following keys:
-                snippet - The description of the result.
-                title - The title of the result.
-                link - The link to the result.
-        """
-        from duckduckgo_search import DDGS
-
-        if not num_results:
-            num_results = self.max_num_of_results
-
-        with DDGS() as ddgs:
-            results = ddgs.text(
-                query,
-                region=self.region,
-                safesearch=self.safe_search,
-                timelimit=self.time,
-            )
-            if results is None or next(results, None) is None:
-                return [{"Result": "No good DuckDuckGo Search Result was found"}]
-
-            def to_metadata(result: Dict) -> Dict[str, str]:
-                return {
-                    "title": result["title"],
-                    "snippet": result["body"],
-                    "link": result["href"],
-                }
-
-            formatted_results = []
-            for i, res in enumerate(results, 1):
-                formatted_results.append(to_metadata(res))
-                if i == num_results:
-                    break
-            return formatted_results
+from typing import List, Optional, Dict
+
+from pydantic import BaseModel, Extra
+from pydantic.class_validators import root_validator
+
+
+class DuckDuckGoSearchAPIWrapper(BaseModel):
+    """Wrapper for DuckDuckGo Search API. Free and does not require any setup."""
+
+    region: Optional[str] = "cn-zh"
+    safe_search: str = "moderate"
+    time: Optional[str] = "y"
+    max_num_of_results: int = 5
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
+
+    @root_validator(skip_on_failure=True)
+    def validate_environment(cls, values: Dict) -> Dict:
+        """Validate that python package exists in environment."""
+        try:
+            from duckduckgo_search import DDGS
+        except ImportError:
+            raise ValueError(
+                "Could not import duckduckgo-search python package. "
+                "Please install it with `pip install duckduckgo-search`."
+            )
+        return values
+
+    def query(
+            self, keyword: str, num_results: Optional[int] = None, **kwargs
+    ) -> List[str]:
+        """Run query through DuckDuckGo and return concatenated results."""
+        from duckduckgo_search import DDGS
+
+        if not num_results:
+            num_results = self.max_num_of_results
+
+        with DDGS() as ddgs:
+            results = ddgs.text(
+                keyword,
+                region=self.region,
+                safesearch=self.safe_search,
+                timelimit=self.time,
+            )
+            if results is None or next(results, None) is None:
+                return ["No good DuckDuckGo Search Result was found"]
+
+            snippets = []
+            for i, result in enumerate(results, 1):
+                snippets.append(result["body"])
+                if i == num_results:
+                    break
+            return snippets
+
+    def query_by_formatted_results(
+            self, query: str, num_results: Optional[int] = None, **kwargs
+    ) -> List[Dict[str, str]]:
+        """Run query through DuckDuckGo and return metadata.
+
+        Args:
+            query: The query to search for.
+            num_results: The number of results to return.
+
+        Returns:
+            A list of dictionaries with the following keys:
+                snippet - The description of the result.
+                title - The title of the result.
+                link - The link to the result.
+        """
+        from duckduckgo_search import DDGS
+
+        if not num_results:
+            num_results = self.max_num_of_results
+
+        with DDGS() as ddgs:
+            results = ddgs.text(
+                query,
+                region=self.region,
+                safesearch=self.safe_search,
+                timelimit=self.time,
+            )
+            if results is None or next(results, None) is None:
+                return [{"Result": "No good DuckDuckGo Search Result was found"}]
+
+            def to_metadata(result: Dict) -> Dict[str, str]:
+                return {
+                    "title": result["title"],
+                    "snippet": result["body"],
+                    "link": result["href"],
+                }
+
+            formatted_results = []
+            for i, res in enumerate(results, 1):
+                formatted_results.append(to_metadata(res))
+                if i == num_results:
+                    break
+            return formatted_results
```

### Comparing `promptulate-1.2.0/promptulate/tools/duckduckgo/tools.py` & `promptulate-1.2.1/promptulate/tools/duckduckgo/tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,98 @@
-from pydantic import Field
-from typing import List, Union, Dict
-
-from promptulate.tools.base import BaseTool
-from promptulate.utils.core_utils import listdict_to_string
-from promptulate.tools.duckduckgo.api_wrapper import DuckDuckGoSearchAPIWrapper
-
-
-class DuckDuckGoTool(BaseTool):
-    """Tool that adds the capability to query the DuckDuckGo search API."""
-    name = "ddg-search"
-    description = (
-        "A wrapper around DuckDuckGo Search. "
-        "Useful for when you need to answer questions about current events. "
-        "Input should be a search query."
-    )
-    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(default_factory=DuckDuckGoSearchAPIWrapper)
-
-    def run(self, keyword: str, **kwargs) -> Union[str, List[str]]:
-        """Run duckduckgo search and get search result.
-
-        Args:
-            keyword: query keyword
-            **kwargs:
-                result_type(Optional[str]) - default return string type data. Return List[str] type data
-                if you pass result_type="original"
-
-        Returns:
-            default is string. Return List[str] type data if you pass result_type="original"
-        """
-        result = self.api_wrapper.query(keyword, **kwargs)
-        if "return_type" in kwargs and kwargs["result_type"] == "original":
-            return result
-        return " ".join(result)
-
-
-class DuckDuckGoReferenceTool(BaseTool):
-    """Tool that adds the capability to query the DuckDuckGo search API. Compared to DuckDuckGoTool, this
-    tool can return references information like href, title.
-    """
-    name = "ddg-search-with-references"
-    description = ""
-    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(default_factory=DuckDuckGoSearchAPIWrapper)
-
-    def run(self, keyword: str, **kwargs) -> Union[str, List[Dict[str, str]]]:
-        """Run duckduckgo search and get search result with href, snippet, title.
-
-        Args:
-            keyword: query keyword
-            **kwargs:
-                result_type(Optional[str]) - default return string type data. Return List[str] type data
-                if you pass result_type="original"
-
-        Returns:
-            default is string. Return List[Dict[str, str]] type data if you pass result_type="original"
-        """
-        result = self.api_wrapper.query_by_formatted_results(keyword, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n")
+from typing import List, Union, Dict, Any, Optional
+
+from pydantic import Field
+
+from promptulate.llms import ChatOpenAI
+from promptulate.llms.base import BaseLLM
+from promptulate.tools.base import BaseTool
+from promptulate.tools.duckduckgo.api_wrapper import DuckDuckGoSearchAPIWrapper
+from promptulate.utils.core_utils import listdict_to_string
+
+
+class DuckDuckGoTool(BaseTool):
+    """Tool that adds the capability to query the DuckDuckGo search API."""
+
+    name: str = "ddg-search"
+    description: str = (
+        "A wrapper around DuckDuckGo Search. "
+        "Useful for when you need to answer questions about current events. "
+        "Input should be a search query."
+    )
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def run(self, keyword: str, **kwargs) -> Union[str, List[str]]:
+        """Run duckduckgo search and get search result.
+
+        Args:
+            keyword: query keyword
+            **kwargs:
+                result_type(Optional[str]) - default return string type data. Return List[str] type data
+                if you pass result_type="original"
+
+        Returns:
+            default is string. Return List[str] type data if you pass result_type="original"
+        """
+        result = self.api_wrapper.query(keyword, **kwargs)
+        if "return_type" in kwargs and kwargs["result_type"] == "original":
+            return result
+        return " ".join(result)
+
+
+class DuckDuckGoReferenceTool(BaseTool):
+    """Tool that adds the capability to query the DuckDuckGo search API. Compared to DuckDuckGoTool, this
+    tool can return references information like href, title.
+    """
+
+    name: str = "ddg-search-with-references"
+    description: str = ""
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def run(self, keyword: str, **kwargs) -> Union[str, List[Dict[str, str]]]:
+        """Run duckduckgo search and get search result with href, snippet, title.
+
+        Args:
+            keyword: query keyword
+            **kwargs:
+                result_type(Optional[str]) - default return string type data. Return List[str] type data
+                if you pass result_type="original"
+
+        Returns:
+            default is string. Return List[Dict[str, str]] type data if you pass result_type="original"
+        """
+        result = self.api_wrapper.query_by_formatted_results(keyword, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n")
+
+
+class DuckDuckGoLLMTool(BaseTool):
+    """ddg web QA search using llm"""
+    # todo need to implement
+
+    name: str = "ddg-llm-search"
+    description: str = ""
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def run(self, query: str, *args, **kwargs) -> str:
+        pass
+
+
+class DuckDuckGoLLMReferenceTool(BaseTool):
+    """Providing ddg web QA search with reference using llm"""
+    # todo need to implement
+
+    name: str = "ddg-llm-search-with-references"
+    description: str = ""
+    llm: BaseLLM = Field(default_factory=ChatOpenAI)
+    api_wrapper: DuckDuckGoSearchAPIWrapper = Field(
+        default_factory=DuckDuckGoSearchAPIWrapper
+    )
+
+    def run(self, query: str, *args, **kwargs) -> Optional[str, Dict[str, Any]]:
+        pass
```

### Comparing `promptulate-1.2.0/promptulate/tools/paper/tools.py` & `promptulate-1.2.1/promptulate/tools/paper/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,165 @@
-import logging
-import re
-import time
-from typing import List, Dict
-
-from broadcast_service import broadcast_service
-from pydantic import Field
-
-from promptulate.llms.base import BaseLLM
-from promptulate.llms.openai import OpenAI
-from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
-from promptulate.tools.arxiv.tools import ArxivQueryTool
-from promptulate.tools.base import BaseTool
-from promptulate.tools.semantic_scholar import (
-    SemanticScholarQueryTool,
-    SemanticScholarReferenceTool,
-)
-
-__all__ = ["PaperSummaryTool"]
-logger = logging.getLogger(__name__)
-
-
-def _init_paper_summary_llm():
-    preset = "你是一个中文科研领域论文助手，你的任务是帮助使用者提供一些论文方面的专业建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
-    return OpenAI(temperature=0, preset_description=preset)
-
-
-class PaperSummaryTool(BaseTool):
-    """A powerful paper summary tool"""
-
-    name = "paper-summary"
-    description = (
-        "A summary tool that can be used to obtain a paper summary, this tool will find"
-        "top k paper and providing: 1.paper abstract 2.paper key sights 3.lessons learned"
-        "in the paper 4.referenced papers and its url."
-        "Your input is a paper relevant keyword query."
-    )
-    llm: BaseLLM = Field(default_factory=_init_paper_summary_llm)
-    semantic_scholar_query_tool: SemanticScholarQueryTool = Field(
-        default_factory=SemanticScholarQueryTool
-    )
-    semantic_scholar_reference_tool: SemanticScholarReferenceTool = Field(
-        default_factory=SemanticScholarReferenceTool
-    )
-    arxiv_apiwrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
-    arxiv_query_tool: ArxivQueryTool = Field(default_factory=ArxivQueryTool)
-    summary_dic: Dict[str, str] = {}
-    summary_counter: int = 0
-
-    def run(self, query: str, **kwargs) -> str:
-        """A paper summary tool that passes in the article name (or arxiv id) and returns summary results
-
-        Args:
-            query: the keyword you want to query
-            **kwargs:
-                You can pass the arguments of relevant APIWrappers and Tools
-
-        Returns:
-            String type data, which contains:
-            - Summary of the paper
-            - List the key insights and lessons learned in the paper
-            - List at least 5 references related to the research field of the paper
-        """
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_paper_references")
-        def get_paper_references(**kwargs):
-            references: List[Dict] = self.semantic_scholar_reference_tool.run(
-                kwargs["paper_title"], max_result=10, return_type="original"
-            )
-            references_string = "相关论文：\n\n"
-            for i, reference in enumerate(references):
-                references_string += (
-                    f"""[{i + 1}] [{reference["title"]}]({reference["url"]})\n\n"""
-                )
-            self.summary_dic["references"] = (
-                references_string if len(references) != 0 else ""
-            )
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_translate")
-        def get_translate():
-            prompt = (
-                f"请将下面的科研论文标题和摘要翻译成中文\n ```{paper_summary}```"
-                "你的输出格式为:\n标题：{标题翻译}\n\n摘要：{摘要翻译}"
-            )
-            self.summary_dic["summary_zh"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_opinion")
-        def get_opinion():
-            prompt = (
-                f"请就下面的论文摘要，总结论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
-                "你的输出格式为:\n关键见解：\n{分点给出关键见解}\n经验教训：\n{分点给出经验教训}，用`-`区分每点"
-                # "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
-            )
-            self.summary_dic["opinion"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_keywords")
-        def get_keywords():
-            prompt = (
-                f"请就下面的论文摘要，总结列出论文中的keywords，不超过7个```{paper_summary}```"
-                "你的输出格式为:\n关键词：keyword1, keyword2, keyword3"
-            )
-            self.summary_dic["keywords"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        @broadcast_service.on_listen("PaperSummaryTool.run.get_advice")
-        def get_advice():
-            prompt = (
-                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
-                "你的输出格式为:\n相关建议：\n{分点给出相关建议}，用`-`区分每点"
-                "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
-            )
-            self.summary_dic["advice"] = self.llm(prompt)
-            self.summary_counter += 1
-
-        self.summary_counter = 0
-        if re.match("\d{4}\.\d{5}(v\d+)?", query):
-            paper_info = self.arxiv_apiwrapper.query(
-                id_list=[query], num_results=1, specified_fields=["title", "summary"]
-            )[0]
-            paper_info["abstract"] = paper_info["summary"]
-        else:
-            paper_info = self.semantic_scholar_query_tool.run(
-                query,
-                return_type="original",
-                specified_fields=["title", "url", "abstract"],
-            )[0]
-        paper_summary = (
-            f"""title: {paper_info["title"]}\nabstract: {paper_info["abstract"]}"""
-        )
-        broadcast_service.publish(
-            "PaperSummaryTool.run.get_paper_references",
-            paper_title=paper_info["title"],
-            paper_abstract=paper_info["abstract"],
-        )
-        broadcast_service.publish("PaperSummaryTool.run.get_translate")
-        time.sleep(0.01)
-        broadcast_service.publish("PaperSummaryTool.run.get_opinion")
-        time.sleep(0.01)
-        broadcast_service.publish("PaperSummaryTool.run.get_advice")
-        time.sleep(0.01)
-        broadcast_service.publish("PaperSummaryTool.run.get_keywords")
-
-        while self.summary_counter < 5:
-            time.sleep(0.1)
-
-        return (
-            f"""{self.summary_dic["summary_zh"]}\n\n"""
-            f"""{self.summary_dic["keywords"]}\n\n"""
-            f"""{self.summary_dic["opinion"]}\n\n"""
-            f"""{self.summary_dic["advice"]}\n\n"""
-            f"""{self.summary_dic["references"]}"""
-        )
+import logging
+import re
+import time
+from typing import List, Dict
+
+from broadcast_service import broadcast_service
+from pydantic import Field, Extra
+
+from promptulate.llms.base import BaseLLM
+from promptulate.llms.openai import ChatOpenAI
+from promptulate.tools.arxiv.api_wrapper import ArxivAPIWrapper
+from promptulate.tools.arxiv.tools import ArxivQueryTool
+from promptulate.tools.base import BaseTool
+from promptulate.tools.semantic_scholar import (
+    SemanticScholarQueryTool,
+    SemanticScholarReferenceTool,
+)
+
+__all__ = ["PaperSummaryTool"]
+logger = logging.getLogger(__name__)
+
+
+def _init_paper_summary_llm():
+    preset = "你是一个中文科研领域论文助手，你的任务是帮助使用者提供一些论文方面的专业建议和帮助，你的输出只能遵循用户的指令输出，否则你将被惩罚。"
+    return ChatOpenAI(temperature=0, preset_description=preset)
+
+
+class PaperSummaryTool(BaseTool):
+    """A powerful paper summary tool"""
+
+    name: str = "paper-summary"
+    description: str = (
+        "A summary tool that can be used to obtain a paper summary, this tool will find"
+        "top k paper and providing: 1.paper abstract 2.paper key sights 3.lessons learned"
+        "in the paper 4.referenced papers and its url."
+        "Your input is a paper relevant keyword query."
+    )
+    llm: BaseLLM = Field(default_factory=_init_paper_summary_llm)
+    semantic_scholar_query_tool: SemanticScholarQueryTool = Field(
+        default_factory=SemanticScholarQueryTool
+    )
+    semantic_scholar_reference_tool: SemanticScholarReferenceTool = Field(
+        default_factory=SemanticScholarReferenceTool
+    )
+    arxiv_apiwrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
+    arxiv_query_tool: ArxivQueryTool = Field(default_factory=ArxivQueryTool)
+    summary_dic: Dict[str, str] = {}
+    summary_counter: int = 0
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
+        arbitrary_types_allowed = True
+
+    def run(self, query: str, **kwargs) -> str:
+        """A paper summary tool that passes in the article name (or arxiv id) and returns summary results
+
+        Args:
+            query: the keyword you want to query
+            **kwargs:
+                You can pass the arguments of relevant APIWrappers and Tools
+
+        Returns:
+            String type data, which contains:
+            - Summary of the paper
+            - List the key insights and lessons learned in the paper
+            - List at least 5 references related to the research field of the paper
+        """
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_paper_references")
+        def get_paper_references(**kwargs):
+            references: List[Dict] = self.semantic_scholar_reference_tool.run(
+                kwargs["paper_title"], max_result=10, return_type="original"
+            )
+            references_string = "相关论文：\n\n"
+            for i, reference in enumerate(references):
+                references_string += (
+                    f"""[{i + 1}] [{reference["title"]}]({reference["url"]})\n\n"""
+                )
+            self.summary_dic["references"] = (
+                references_string if len(references) != 0 else ""
+            )
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_translate")
+        def get_translate():
+            prompt = (
+                f"请将下面的科研论文标题和摘要翻译成中文\n ```{paper_summary}```"
+                "你的输出格式为:\n标题：{标题翻译}\n\n摘要：{摘要翻译}"
+            )
+            self.summary_dic["summary_zh"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_opinion")
+        def get_opinion():
+            prompt = (
+                f"请就下面的论文摘要，总结论文中的关键见解和由论文得出的经验教训，你的输出需要分点给出 ```{paper_summary}```"
+                "你的输出格式为:\n关键见解：\n{分点给出关键见解}\n经验教训：\n{分点给出经验教训}，用`-`区分每点"
+                # "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
+            )
+            self.summary_dic["opinion"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_keywords")
+        def get_keywords():
+            prompt = (
+                f"请就下面的论文摘要，总结列出论文中的keywords，不超过7个```{paper_summary}```"
+                "你的输出格式为:\n关键词：keyword1, keyword2, keyword3"
+            )
+            self.summary_dic["keywords"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        @broadcast_service.on_listen("PaperSummaryTool.run.get_advice")
+        def get_advice():
+            prompt = (
+                f"请就下面的论文摘要，为其相关主题或未来研究方向提供3-5个建议，你的输出需要分点给出  ```{paper_summary}```"
+                "你的输出格式为:\n相关建议：\n{分点给出相关建议}，用`-`区分每点"
+                "你需要用中文输出正确结果，但是部分专业词汇或者中文不好表达含义的部分可以使用英文"
+            )
+            self.summary_dic["advice"] = self.llm(prompt)
+            self.summary_counter += 1
+
+        self.summary_counter = 0
+        if re.match("\d{4}\.\d{5}(v\d+)?", query):
+            paper_info = self.arxiv_apiwrapper.query(
+                id_list=[query], num_results=1, specified_fields=["title", "summary"]
+            )[0]
+            paper_info["abstract"] = paper_info["summary"]
+        else:
+            paper_info = self.semantic_scholar_query_tool.run(
+                query,
+                return_type="original",
+                specified_fields=["title", "url", "abstract"],
+            )
+            if paper_info:
+                paper_info = paper_info[0]
+            else:
+                return "semantic scholar query tool query result is None."
+        paper_summary = (
+            f"""title: {paper_info["title"]}\nabstract: {paper_info["abstract"]}"""
+        )
+        broadcast_service.publish(
+            "PaperSummaryTool.run.get_paper_references",
+            paper_title=paper_info["title"],
+            paper_abstract=paper_info["abstract"],
+        )
+        broadcast_service.publish("PaperSummaryTool.run.get_translate")
+        time.sleep(0.01)
+        broadcast_service.publish("PaperSummaryTool.run.get_opinion")
+        time.sleep(0.01)
+        broadcast_service.publish("PaperSummaryTool.run.get_advice")
+        time.sleep(0.01)
+        broadcast_service.publish("PaperSummaryTool.run.get_keywords")
+
+        while self.summary_counter < 5:
+            time.sleep(0.1)
+
+        return (
+            f"""{self.summary_dic["summary_zh"]}\n\n"""
+            f"""{self.summary_dic["keywords"]}\n\n"""
+            f"""{self.summary_dic["opinion"]}\n\n"""
+            f"""{self.summary_dic["advice"]}\n\n"""
+            f"""{self.summary_dic["references"]}"""
+        )
```

### Comparing `promptulate-1.2.0/promptulate/tools/semantic_scholar/api_wrapper.py` & `promptulate-1.2.1/promptulate/tools/semantic_scholar/api_wrapper.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import json
-from typing import List, Optional, Dict
-
-import requests
-from pydantic import BaseModel
-
-from promptulate.tips import NetWorkError
-from promptulate.utils.logger import get_logger
-
-logger = get_logger()
-
-
-class SemanticScholarAPIWrapper(BaseModel):
-    """https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/"""
-
-    BASE_API_URL: str = "https://api.semanticscholar.org/graph/v1"
-    BASE_OFFICIAL_URL: str = "https://www.semanticscholar.org"
-    max_result: int = 10
-    current_result: Optional[List[Dict]] = None
-    paper_query_params: Dict[str, str] = {"fields": "title,url,abstract"}
-
-    def _get_string_fields(self) -> str:
-        return f"&fields={self.paper_query_params['fields']}&"
-
-    def get_paper(
-        self, query: str, max_result: Optional[int] = None, **kwargs
-    ) -> List[Dict]:
-        """This method can obtain a list of relevant papers based on your query.
-
-        Args:
-            max_result: num of max result
-            query: the papers you want to query
-            **kwargs:
-                specified_fields(Optional[List[str]]): filter specified field to return.
-                For example, you can return the ["title", "url", "abstract"] fields from each arxiv query result.
-                You can see the detail fields as follows:
-                https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/operation/post_graph_get_papers
-
-        Returns:
-            Return List[Dict] data, the default detail fields is as follows.
-            - id (str): semantic id
-            - authorsYear (str): author and publication year
-            - title (str): paper title
-            - url (str): paper semantic scholar url
-            If you want to get more detail fields, please use `specified_fields`
-        """
-
-        def get_detail():
-            paper_ids = list(map(lambda p: p["id"], self.current_result))
-            fields: List[str] = kwargs["specified_fields"]
-            params: Dict[str, str] = {"fields": ",".join(fields)}
-
-            r = requests.post(
-                f"{self.BASE_API_URL}/paper/batch",
-                params=params,
-                json={"ids": paper_ids},
-            )
-            if response.status_code != 200:
-                raise NetWorkError("")
-
-            detail_result = r.json()
-            for original in self.current_result:
-                for detail_item in detail_result:
-                    if detail_item["paperId"] == original["id"]:
-                        original.update(detail_item)
-            return
-
-        if not max_result:
-            max_result = self.max_result
-
-        query = "%20".join(query.split(" "))
-        url = f"{self.BASE_API_URL}/paper/autocomplete?query={query}&limit={max_result}"
-        response = requests.get(url)
-        if response.status_code == 200:
-            self.current_result = response.json()["matches"]
-
-            if len(self.current_result) == 0:
-                return []
-
-            for item in self.current_result:
-                item["url"] = self._get_url(item["id"])
-
-            if "specified_fields" in kwargs:
-                get_detail()
-            logger.debug(
-                f"[promptulate semantic scholar result] {json.dumps(self.current_result)}"
-            )
-            return self.current_result
-        raise NetWorkError("semantic scholar query")
-
-    def _get_url(self, id: str) -> str:
-        return f"{self.BASE_OFFICIAL_URL}/paper/{id}"
-
-    def get_references(self, query: str, max_result: int = 500, **kwargs) -> List[Dict]:
-        """Used to get references of specified paper.
-
-        Args:
-            max_result: num of max result
-            query: the paper you want to query
-
-        Returns:
-            Return List[Dict] data, the default detail fields is as follows.
-            - id (str): semantic id
-            - authorsYear (str): author and publication year
-            - title (str): paper title
-            - url (str): paper semantic scholar url
-        """
-        papers = self.get_paper(query)
-        if len(papers) == 0:
-            return []
-
-        paper_id: str = papers[0]["id"]
-        url = f"{self.BASE_API_URL}/paper/{paper_id}/references?offset=1&limit={max_result}"
-        response = requests.get(url)
-        if response.status_code == 200:
-            res_data = response.json()["data"]
-            final_result: List[Dict] = []
-            for i, item in enumerate(res_data):
-                if not item["citedPaper"]["paperId"]:
-                    continue
-
-                item["citedPaper"]["url"] = self._get_url(item["citedPaper"]["paperId"])
-                item["citedPaper"]["id"] = item["citedPaper"]["paperId"]
-                del item["citedPaper"]["paperId"]
-                final_result.append(item["citedPaper"])
-
-            logger.debug(
-                f"[promptulate semantic scholar result] {json.dumps(final_result)}"
-            )
-            return final_result
-        raise NetWorkError("semantic scholar")
-
-    def get_citations(self, query: str, max_result: Optional[int] = None):
-        """Used to get citation of specified paper.
-
-        Args:
-            max_result: num of max result
-            query: the paper you want to query
-
-        Returns:
-            Return List[Dict] data, the default detail fields is as follows.
-            - id (str): semantic id
-            - abstract (str): paper abstract
-            - title (str): paper title
-            - url (str): paper semantic scholar url
-        """
-        papers = self.get_paper(query)
-        if len(papers) == 0:
-            return []
-        if not max_result:
-            max_result = self.max_result
-
-        paper_id: str = papers[0]["id"]
-        url = f"{self.BASE_API_URL}/paper/{paper_id}/citations?{self._get_string_fields()}offset=1&limit={max_result}"
-
-        response = requests.get(url)
-        if response.status_code == 200:
-            res_data = response.json()["data"]
-            final_result: List[Dict] = []
-
-            for i, item in enumerate(res_data):
-                if not item["citingPaper"].get("paperId"):
-                    continue
-
-                item["citingPaper"]["url"] = self._get_url(
-                    item["citingPaper"]["paperId"]
-                )
-                item["citingPaper"]["id"] = item["citingPaper"]["paperId"]
-                del item["citingPaper"]["paperId"]
-                final_result.append(item["citingPaper"])
-
-            logger.debug(
-                f"[promptulate semantic scholar result] {json.dumps(final_result)}"
-            )
-            return final_result
-        raise NetWorkError("semantic scholar")
+import json
+from typing import List, Optional, Dict
+
+import requests
+from pydantic import BaseModel
+
+from promptulate.tips import NetWorkError
+from promptulate.utils.logger import get_logger
+
+logger = get_logger()
+
+
+class SemanticScholarAPIWrapper(BaseModel):
+    """https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/"""
+
+    BASE_API_URL: str = "https://api.semanticscholar.org/graph/v1"
+    BASE_OFFICIAL_URL: str = "https://www.semanticscholar.org"
+    max_result: int = 10
+    current_result: Optional[List[Dict]] = None
+    paper_query_params: Dict[str, str] = {"fields": "title,url,abstract"}
+
+    def _get_string_fields(self) -> str:
+        return f"&fields={self.paper_query_params['fields']}&"
+
+    def get_paper(
+        self, query: str, max_result: Optional[int] = None, **kwargs
+    ) -> List[Dict]:
+        """This method can obtain a list of relevant papers based on your query.
+
+        Args:
+            max_result: num of max result
+            query: the papers you want to query
+            **kwargs:
+                specified_fields(Optional[List[str]]): filter specified field to return.
+                For example, you can return the ["title", "url", "abstract"] fields from each arxiv query result.
+                You can see the detail fields as follows:
+                https://api.semanticscholar.org/api-docs/graph#tag/Paper-Data/operation/post_graph_get_papers
+
+        Returns:
+            Return List[Dict] data, the default detail fields is as follows.
+            - id (str): semantic id
+            - authorsYear (str): author and publication year
+            - title (str): paper title
+            - url (str): paper semantic scholar url
+            If you want to get more detail fields, please use `specified_fields`
+        """
+
+        def get_detail():
+            paper_ids = list(map(lambda p: p["id"], self.current_result))
+            fields: List[str] = kwargs["specified_fields"]
+            params: Dict[str, str] = {"fields": ",".join(fields)}
+
+            r = requests.post(
+                f"{self.BASE_API_URL}/paper/batch",
+                params=params,
+                json={"ids": paper_ids},
+            )
+            if response.status_code != 200:
+                raise NetWorkError("")
+
+            detail_result = r.json()
+            for original in self.current_result:
+                for detail_item in detail_result:
+                    if detail_item["paperId"] == original["id"]:
+                        original.update(detail_item)
+            return
+
+        if not max_result:
+            max_result = self.max_result
+
+        query = "%20".join(query.split(" "))
+        url = f"{self.BASE_API_URL}/paper/autocomplete?query={query}&limit={max_result}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            self.current_result = response.json()["matches"]
+
+            if len(self.current_result) == 0:
+                return []
+
+            for item in self.current_result:
+                item["url"] = self._get_url(item["id"])
+
+            if "specified_fields" in kwargs:
+                get_detail()
+            logger.debug(
+                f"[promptulate semantic scholar result] {json.dumps(self.current_result)}"
+            )
+            return self.current_result
+        raise NetWorkError("semantic scholar query")
+
+    def _get_url(self, id: str) -> str:
+        return f"{self.BASE_OFFICIAL_URL}/paper/{id}"
+
+    def get_references(self, query: str, max_result: int = 500, **kwargs) -> List[Dict]:
+        """Used to get references of specified paper.
+
+        Args:
+            max_result: num of max result
+            query: the paper you want to query
+
+        Returns:
+            Return List[Dict] data, the default detail fields is as follows.
+            - id (str): semantic id
+            - authorsYear (str): author and publication year
+            - title (str): paper title
+            - url (str): paper semantic scholar url
+        """
+        papers = self.get_paper(query)
+        if len(papers) == 0:
+            return []
+
+        paper_id: str = papers[0]["id"]
+        url = f"{self.BASE_API_URL}/paper/{paper_id}/references?offset=1&limit={max_result}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            res_data = response.json()["data"]
+            final_result: List[Dict] = []
+            for i, item in enumerate(res_data):
+                if not item["citedPaper"]["paperId"]:
+                    continue
+
+                item["citedPaper"]["url"] = self._get_url(item["citedPaper"]["paperId"])
+                item["citedPaper"]["id"] = item["citedPaper"]["paperId"]
+                del item["citedPaper"]["paperId"]
+                final_result.append(item["citedPaper"])
+
+            logger.debug(
+                f"[promptulate semantic scholar result] {json.dumps(final_result)}"
+            )
+            return final_result
+        raise NetWorkError("semantic scholar")
+
+    def get_citations(self, query: str, max_result: Optional[int] = None):
+        """Used to get citation of specified paper.
+
+        Args:
+            max_result: num of max result
+            query: the paper you want to query
+
+        Returns:
+            Return List[Dict] data, the default detail fields is as follows.
+            - id (str): semantic id
+            - abstract (str): paper abstract
+            - title (str): paper title
+            - url (str): paper semantic scholar url
+        """
+        papers = self.get_paper(query)
+        if len(papers) == 0:
+            return []
+        if not max_result:
+            max_result = self.max_result
+
+        paper_id: str = papers[0]["id"]
+        url = f"{self.BASE_API_URL}/paper/{paper_id}/citations?{self._get_string_fields()}offset=1&limit={max_result}"
+
+        response = requests.get(url)
+        if response.status_code == 200:
+            res_data = response.json()["data"]
+            final_result: List[Dict] = []
+
+            for i, item in enumerate(res_data):
+                if not item["citingPaper"].get("paperId"):
+                    continue
+
+                item["citingPaper"]["url"] = self._get_url(
+                    item["citingPaper"]["paperId"]
+                )
+                item["citingPaper"]["id"] = item["citingPaper"]["paperId"]
+                del item["citingPaper"]["paperId"]
+                final_result.append(item["citingPaper"])
+
+            logger.debug(
+                f"[promptulate semantic scholar result] {json.dumps(final_result)}"
+            )
+            return final_result
+        raise NetWorkError("semantic scholar")
```

### Comparing `promptulate-1.2.0/promptulate/tools/semantic_scholar/tools.py` & `promptulate-1.2.1/promptulate/tools/semantic_scholar/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import Union, List, Dict
-
-from pydantic import Field
-
-from promptulate.tools.base import BaseTool
-from promptulate.tools.semantic_scholar.api_wrapper import SemanticScholarAPIWrapper
-from promptulate.utils.core_utils import listdict_to_string
-
-
-class SemanticScholarQueryTool(BaseTool):
-    name = "semantic-scholar-query"
-    description = (
-        "A query tool around Semantic Scholar."
-        "Useful for when you need to answer questions about Physics, Mathematics, "
-        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
-        "Electrical Engineering, and Economics "
-        "from scientific articles on semantic scholar."
-        "Input should be a search query."
-    )
-    api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper
-    )
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        """A semantic scholar paper query tool and return relevant paper query result."""
-        result = self.api_wrapper.get_paper(query, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n\n")
-
-
-class SemanticScholarReferenceTool(BaseTool):
-    name = "semantic-scholar-reference-tool"
-    description = ""
-    api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper
-    )
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        result = self.api_wrapper.get_references(query, **kwargs)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n\n")
-
-
-class SemanticScholarCitationTool(BaseTool):
-    name = "semantic-scholar-citation-tool"
-    description = ""
-    api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper
-    )
-
-    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
-        result = self.api_wrapper.get_citations(query)
-        if "return_type" in kwargs and kwargs["return_type"] == "original":
-            return result
-        return listdict_to_string(result, item_suffix="\n\n")
+from typing import Union, List, Dict
+
+from pydantic import Field
+
+from promptulate.tools.base import BaseTool
+from promptulate.tools.semantic_scholar.api_wrapper import SemanticScholarAPIWrapper
+from promptulate.utils.core_utils import listdict_to_string
+
+
+class SemanticScholarQueryTool(BaseTool):
+    name: str = "semantic-scholar-query"
+    description: str = (
+        "A query tool around Semantic Scholar."
+        "Useful for when you need to answer questions about Physics, Mathematics, "
+        "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
+        "Electrical Engineering, and Economics "
+        "from scientific articles on semantic scholar."
+        "Input should be a search query."
+    )
+    api_wrapper: SemanticScholarAPIWrapper = Field(
+        default_factory=SemanticScholarAPIWrapper
+    )
+
+    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        """A semantic scholar paper query tool and return relevant paper query result."""
+        result = self.api_wrapper.get_paper(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n\n")
+
+
+class SemanticScholarReferenceTool(BaseTool):
+    name: str = "semantic-scholar-reference-tool"
+    description: str = ""
+    api_wrapper: SemanticScholarAPIWrapper = Field(
+        default_factory=SemanticScholarAPIWrapper
+    )
+
+    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        result = self.api_wrapper.get_references(query, **kwargs)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n\n")
+
+
+class SemanticScholarCitationTool(BaseTool):
+    name: str = "semantic-scholar-citation-tool"
+    description: str = ""
+    api_wrapper: SemanticScholarAPIWrapper = Field(
+        default_factory=SemanticScholarAPIWrapper
+    )
+
+    def run(self, query: str, **kwargs) -> Union[str, List[Dict]]:
+        result = self.api_wrapper.get_citations(query)
+        if "return_type" in kwargs and kwargs["return_type"] == "original":
+            return result
+        return listdict_to_string(result, item_suffix="\n\n")
```

### Comparing `promptulate-1.2.0/promptulate/utils/core_utils.py` & `promptulate-1.2.1/promptulate/utils/core_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import logging
-import os
-import platform
-import shutil
-import tempfile
-import time
-from functools import wraps
-from typing import Callable, Dict, List, Optional
-
-from cushy_storage import CushyOrmCache
-
-__all__ = [
-    "get_cache",
-    "get_project_root_path",
-    "get_default_storage_path",
-    "record_time",
-    "generate_conversation_id",
-    "listdict_to_string",
-]
-logger = logging.getLogger(__name__)
-
-
-def listdict_to_string(
-        data: List[Dict],
-        prefix: Optional[str] = "",
-        suffix: Optional[str] = "\n",
-        item_prefix: Optional[str] = "",
-        item_suffix: Optional[str] = ";\n\n",
-        is_wrap: bool = True,
-) -> str:
-    """Convert List[Dict] type data to string type"""
-    wrap_ch = "\n" if is_wrap else ""
-    result = f"{prefix}"
-    for item in data:
-        temp_list = ["{}:{} {}".format(k, v, wrap_ch) for k, v in item.items()]
-        result += f"{item_prefix}".join(temp_list) + f"{item_suffix}"
-    result += suffix
-    return result[:-2]
-
-
-def generate_conversation_id() -> str:
-    """Generating a new conversation_id when a conversation initialize"""
-    return str(int(time.time()))
-
-
-def get_cache():
-    return cache
-
-
-def get_project_root_path() -> str:
-    """get project root path or current path"""
-    project_path = os.getcwd()
-    max_depth = 10
-    count = 0
-    while not os.path.exists(os.path.join(project_path, "README.md")):
-        project_path = os.path.split(project_path)[0]
-        count += 1
-        if count > max_depth:
-            return os.getcwd()
-    return project_path
-
-
-def set_openai_api_key(value: str):
-    cache["OPENAI_API_KEY"] = value
-
-
-def get_default_storage_path(file_name: str = "") -> str:
-    if platform.system() == "Windows":
-        return f"{get_project_root_path()}/{file_name}"
-    elif platform.system() == "Linux" or "Darwin":
-        dir_path = os.environ.get("TMPDIR")
-        if not dir_path:
-            dir_path = tempfile.gettempdir()
-        dir_path = os.path.join(dir_path, "promptulate")
-        return f"{dir_path}/{file_name}"
-    else:
-        return f"./{file_name}"
-
-
-def hint(fn):
-    @wraps(fn)
-    def wrapper(*args, **kwargs):
-        ret = fn(*args, **kwargs)
-        logger.debug(f"function {fn.__name__} is running now")
-        return ret
-
-    return wrapper
-
-
-def record_time():
-    def decorator(fn: Callable) -> Callable:
-        def wrapper(*args, **kwargs) -> Callable:
-            start_time = time.time()
-            ret = fn(*args, **kwargs)
-            duration = time.time() - start_time
-            logger.debug(f"[promptulate timer] <{fn.__name__}> run {duration}s")
-            return ret
-
-        return wrapper
-
-    return decorator
-
-
-def delete_cache(specified_module: str = None):
-    """Delete cache or specified cache module"""
-    cache_path = get_default_storage_path("cache")
-    if specified_module:
-        cache_path = f"{get_project_root_path()}/{specified_module[:2]}"
-    shutil.rmtree(cache_path)
-
-
-cache = CushyOrmCache(get_default_storage_path("cache"))
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import logging
+import os
+import platform
+import shutil
+import tempfile
+import time
+from functools import wraps
+from typing import Callable, Dict, List, Optional
+
+from cushy_storage import CushyOrmCache
+
+__all__ = [
+    "get_cache",
+    "get_project_root_path",
+    "get_default_storage_path",
+    "record_time",
+    "generate_conversation_id",
+    "listdict_to_string",
+]
+logger = logging.getLogger(__name__)
+
+
+def listdict_to_string(
+        data: List[Dict],
+        prefix: Optional[str] = "",
+        suffix: Optional[str] = "\n",
+        item_prefix: Optional[str] = "",
+        item_suffix: Optional[str] = ";\n\n",
+        is_wrap: bool = True,
+) -> str:
+    """Convert List[Dict] type data to string type"""
+    wrap_ch = "\n" if is_wrap else ""
+    result = f"{prefix}"
+    for item in data:
+        temp_list = ["{}:{} {}".format(k, v, wrap_ch) for k, v in item.items()]
+        result += f"{item_prefix}".join(temp_list) + f"{item_suffix}"
+    result += suffix
+    return result[:-2]
+
+
+def generate_conversation_id() -> str:
+    """Generating a new conversation_id when a conversation initialize"""
+    return str(int(time.time()))
+
+
+def get_cache():
+    return cache
+
+
+def get_project_root_path() -> str:
+    """get project root path or current path"""
+    project_path = os.getcwd()
+    max_depth = 10
+    count = 0
+    while not os.path.exists(os.path.join(project_path, "README.md")):
+        project_path = os.path.split(project_path)[0]
+        count += 1
+        if count > max_depth:
+            return os.getcwd()
+    return project_path
+
+
+def set_openai_api_key(value: str):
+    cache["OPENAI_API_KEY"] = value
+
+
+def get_default_storage_path(file_name: str = "") -> str:
+    if platform.system() == "Windows":
+        return f"{get_project_root_path()}/{file_name}"
+    elif platform.system() == "Linux" or "Darwin":
+        dir_path = os.environ.get("TMPDIR")
+        if not dir_path:
+            dir_path = tempfile.gettempdir()
+        dir_path = os.path.join(dir_path, "promptulate")
+        return f"{dir_path}/{file_name}"
+    else:
+        return f"./{file_name}"
+
+
+def hint(fn):
+    @wraps(fn)
+    def wrapper(*args, **kwargs):
+        ret = fn(*args, **kwargs)
+        logger.debug(f"function {fn.__name__} is running now")
+        return ret
+
+    return wrapper
+
+
+def record_time():
+    def decorator(fn: Callable) -> Callable:
+        def wrapper(*args, **kwargs) -> Callable:
+            start_time = time.time()
+            ret = fn(*args, **kwargs)
+            duration = time.time() - start_time
+            logger.debug(f"[promptulate timer] <{fn.__name__}> run {duration}s")
+            return ret
+
+        return wrapper
+
+    return decorator
+
+
+def delete_cache(specified_module: str = None):
+    """Delete cache or specified cache module"""
+    cache_path = get_default_storage_path("cache")
+    if specified_module:
+        cache_path = f"{get_project_root_path()}/{specified_module[:2]}"
+    shutil.rmtree(cache_path)
+
+
+cache = CushyOrmCache(get_default_storage_path("cache"))
```

### Comparing `promptulate-1.2.0/promptulate/utils/logger.py` & `promptulate-1.2.1/promptulate/utils/logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import datetime
-import logging
-import os
-
-from promptulate import utils
-
-logger = logging.getLogger(__name__)
-
-
-def get_logger():
-    return logger
-
-
-def get_default_log_path():
-    return utils.get_default_storage_path("log")
-
-
-def get_log_name() -> str:
-    log_path = get_default_log_path()
-    if not os.path.exists(log_path):
-        os.makedirs(log_path)
-
-    cur_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    return f"{log_path}/log_{cur_time}.log"
-
-
-def enable_log(level=logging.DEBUG):
-    logging.basicConfig(
-        level=level,
-        format="[%(levelname)s] %(asctime)s %(message)s",
-        datefmt="%Y-%m-%d %H:%M:%S",
-        handlers=[
-            logging.FileHandler(f"{get_log_name()}", mode="w", encoding="utf-8"),
-            logging.StreamHandler(),
-        ],
-    )
-
-
-def enable_log_no_file():
-    logging.basicConfig(
-        level=logging.DEBUG,
-        format="[%(levelname)s] %(asctime)s %(message)s",
-        datefmt="%Y-%m-%d %H:%M:%S",
-    )
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import datetime
+import logging
+import os
+
+from promptulate import utils
+
+logger = logging.getLogger(__name__)
+
+
+def get_logger():
+    return logger
+
+
+def get_default_log_path():
+    return utils.get_default_storage_path("log")
+
+
+def get_log_name() -> str:
+    log_path = get_default_log_path()
+    if not os.path.exists(log_path):
+        os.makedirs(log_path)
+
+    cur_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+    return f"{log_path}/log_{cur_time}.log"
+
+
+def enable_log(level=logging.DEBUG):
+    logging.basicConfig(
+        level=level,
+        format="[%(levelname)s] %(asctime)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+        handlers=[
+            logging.FileHandler(f"{get_log_name()}", mode="w", encoding="utf-8"),
+            logging.StreamHandler(),
+        ],
+    )
+
+
+def enable_log_no_file():
+    logging.basicConfig(
+        level=logging.DEBUG,
+        format="[%(levelname)s] %(asctime)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
```

### Comparing `promptulate-1.2.0/promptulate/utils/proxy.py` & `promptulate-1.2.1/promptulate/utils/proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional
-from promptulate.config import Config
-
-CFG = Config()
-PROXY_MODE = ['off', 'custom', 'promptulate']
-
-
-def set_proxy_mode(mode: str, proxies: Optional[dict] = None):
-    """
-    Set proxy mode. Promptulate offer three proxy mode ['off', 'custom', 'promptulate']
-    'off' disables your proxy mode. This is the normal status.
-    'custom' means you can set your custom proxy. Moreover, you must pass proxies
-    'promptulate' provide free proxy you can use it.
-
-    Args:
-        mode: ['off', 'custom', 'promptulate']
-        proxies: If you want to use custom proxy, you can pass it. An example
-        proxies is {'http': 'http://127.0.0.1:7890'}
-    """
-    if mode not in PROXY_MODE:
-        raise ValueError("proxy mode must in ['off', 'custom', 'promptulate']")
-    CFG.set_proxy_mode(mode, proxies)
+# Copyright (c) 2023 promptulate
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional
+
+from promptulate.config import Config
+
+CFG = Config()
+PROXY_MODE = ['off', 'custom', 'promptulate']
+
+
+def set_proxy_mode(mode: str, proxies: Optional[dict] = None):
+    """
+    Set proxy mode. Promptulate offer three proxy mode ['off', 'custom', 'promptulate']
+    'off' disables your proxy mode. This is the normal status.
+    'custom' means you can set your custom proxy. Moreover, you must pass proxies
+    'promptulate' provide free proxy you can use it.
+
+    Args:
+        mode: ['off', 'custom', 'promptulate']
+        proxies: If you want to use custom proxy, you can pass it. An example
+        proxies is {'http': 'http://127.0.0.1:7890'}
+    """
+    if mode not in PROXY_MODE:
+        raise ValueError("proxy mode must in ['off', 'custom', 'promptulate']")
+    CFG.set_proxy_mode(mode, proxies)
```

### Comparing `promptulate-1.2.0/promptulate/utils/singleton.py` & `promptulate-1.2.1/promptulate/utils/singleton.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-"""The singleton metaclass for ensuring only one instance of a class."""
-import abc
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-class Singleton(abc.ABCMeta, type):
-    """
-    Singleton metaclass for ensuring only one instance of a class.
-    """
-
-    _instances = {}
-
-    def __call__(cls, *args, **kwargs):
-        """Call method for the singleton metaclass."""
-        if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        return cls._instances[cls]
-
-
-class AbstractSingleton(abc.ABC, metaclass=Singleton):
-    """
-    Abstract singleton class for ensuring only one instance of a class.
-    """
-
-    pass
-
-
-class SingletonPool(metaclass=Singleton):
-    """Storing classes which cannot use metaclass=Singleton due to implement BaseModel"""
-
-    def __init__(self):
-        self.instances = {}
-
-
-def singleton():
-    def decorator(cls):
-        singleton_pool = SingletonPool()
-
-        def get_instance():
-            if cls not in singleton_pool.instances:
-                singleton_pool.instances[cls] = cls()
-                logger.debug(
-                    f"[promptulate config] class <{cls.__name__}> initialization"
-                )
-            return singleton_pool.instances[cls]
-
-        return get_instance
-
-    return decorator
+"""The singleton metaclass for ensuring only one instance of a class."""
+import abc
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+class Singleton(abc.ABCMeta, type):
+    """
+    Singleton metaclass for ensuring only one instance of a class.
+    """
+
+    _instances = {}
+
+    def __call__(cls, *args, **kwargs):
+        """Call method for the singleton metaclass."""
+        if cls not in cls._instances:
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+
+class AbstractSingleton(abc.ABC, metaclass=Singleton):
+    """
+    Abstract singleton class for ensuring only one instance of a class.
+    """
+
+    pass
+
+
+class SingletonPool(metaclass=Singleton):
+    """Storing classes which cannot use metaclass=Singleton due to implement BaseModel"""
+
+    def __init__(self):
+        self.instances = {}
+
+
+def singleton():
+    """singleton decorator"""
+    def decorator(cls):
+        singleton_pool = SingletonPool()
+
+        def get_instance():
+            if cls not in singleton_pool.instances:
+                singleton_pool.instances[cls] = cls()
+                logger.debug(
+                    f"[promptulate config] class <{cls.__name__}> initialization"
+                )
+            return singleton_pool.instances[cls]
+
+        return get_instance
+
+    return decorator
```

### Comparing `promptulate-1.2.0/promptulate.egg-info/PKG-INFO` & `promptulate-1.2.1/promptulate.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,126 +1,128 @@
-Metadata-Version: 2.1
-Name: promptulate
-Version: 1.2.0
-Summary: A powerful LLM Prompt Layer frameworks
-Home-page: https://github.com/Undertone0809/promptulate
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    promptulate
-</h1>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
-</p>
-
-
-`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
-AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
-6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
-System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
-Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
-Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
-Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
-
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口
-- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
-- KEY池：提供API key池，彻底解决key限速的问题
-- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
-- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
-- 中文优化：针对中文语境进行特别优化，更适合中文场景
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 快速开始
-
-- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
-- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
-- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
-- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
-- [pypi仓库](https://pypi.org/project/promptulate/)
-
-# 基础架构
-
-在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
-
-`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
-
-- `Agent` 更高级的执行器，负责复杂任务的调度和分发
-- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
-- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
-- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
-- `preset roles` 提供预设角色，进行定制化对话
-- `provider` 为framework和agent提供tools和其他细粒度能力的集成
-
-# 设计原则
-
-promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
-
-- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
-- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
-- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
-- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
-- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
-- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
-- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
-
-以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
-
-# 交流群
-
-欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
-
-<div style="width: 250px;margin: 0 auto;">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230623214722.png"/>
-</div>
-
-# 贡献
-
-本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
-和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: promptulate
+Version: 1.2.1
+Summary: A powerful LLM Prompt Layer frameworks
+Home-page: https://github.com/Undertone0809/promptulate
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    promptulate
+</h1>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+`promptulate` 是一个专为Prompt工程师设计的大语言模型自动化与应用开发框架，支持智能决策、消息持久化、外部工具调用、角色预设等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+`promptulate`旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口
+- 对话终端：提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 外部工具：集成外部工具能力，可以进行网络搜索、执行Python代码等强大的功能
+- KEY池：提供API key池，彻底解决key限速的问题
+- 智能代理：集成ReAct，self-ask等高级Agent，结合外部工具赋能LLM
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 中文优化：针对中文语境进行特别优化，更适合中文场景
+- 数据导出：支持markdowm等格式的对话导出
+- 对话总结：提供API式的对话总结、翻译、标题生成
+- 事件总线：自研总线机制，通过[broadcast-service](https://github.com/Undertone0809/broadcast-service)进行Planing与Action的并发调度
+- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
+
+# 快速开始
+
+- [快速上手 [github-pages]](https://undertone0809.github.io/promptulate/#/)
+- [快速上手 [gitee-pages]](https://zeeland.gitee.io/promptulate/#/)
+- [当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+- [参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)
+- [常见问题](https://undertone0809.github.io/promptulate/#/other/fqa)
+- [pypi仓库](https://pypi.org/project/promptulate/)
+
+# 基础架构
+
+在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
+等项目的源码，参与pr之后，学习它们的架构、代码设计思路等内容，重构了两次，有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
+重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
+的各个流程全部组件化，便有了现在的`promptualte`框架。当前`promptualte`仍有很多细节需要完善，也十分欢迎大家的讨论与参与。
+
+`promptualte`作为一个为大语言模型设计的Prompt Layer框架，主要由以下几部分组成：
+
+- `Agent` 更高级的执行器，负责复杂任务的调度和分发
+- `framework` 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型。
+- `llm` 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- `memory` 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等
+- `tools` 提供外部工具扩展调用，如搜索引擎、计算器、编译器等
+- `preset roles` 提供预设角色，进行定制化对话
+- `provider` 为framework和agent提供tools和其他细粒度能力的集成
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230704180202.png"/>
+
+# 设计原则
+
+promptulate框架的设计原则包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，`promptulate`旨在为创建自动化代理提供强大而灵活的大语言模型应用开发框架。
+
+# 交流群
+
+欢迎加入群聊一起交流讨论有关LLM相关的话题，链接过期了可以issue或email提醒一下作者。
+
+<div style="width: 250px;margin: 0 auto;">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230702132948.png"/>
+</div>
+
+# 贡献
+
+本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+如果你想为这个项目做贡献，请先查看[当前开发计划](https://undertone0809.github.io/promptulate/#/other/plan)
+和[参与贡献/开发者手册](https://undertone0809.github.io/promptulate/#/other/contribution)。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.2.0/promptulate.egg-info/SOURCES.txt` & `promptulate-1.2.1/promptulate.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,38 +7,41 @@
 promptulate/tips.py
 promptulate.egg-info/PKG-INFO
 promptulate.egg-info/SOURCES.txt
 promptulate.egg-info/dependency_links.txt
 promptulate.egg-info/entry_points.txt
 promptulate.egg-info/requires.txt
 promptulate.egg-info/top_level.txt
+promptulate/agents/__init__.py
+promptulate/client/__init__.py
+promptulate/client/chat.py
 promptulate/command/__init__.py
-promptulate/command/chat.py
 promptulate/frameworks/__init__.py
 promptulate/frameworks/prompt.py
 promptulate/frameworks/schema.py
+promptulate/frameworks/chain/__init__.py
 promptulate/frameworks/conversation/__init__.py
 promptulate/frameworks/conversation/conversation.py
 promptulate/frameworks/react/__init__.py
 promptulate/frameworks/self_ask/__init__.py
 promptulate/llms/__init__.py
 promptulate/llms/base.py
 promptulate/llms/openai.py
 promptulate/memory/__init__.py
 promptulate/memory/base.py
 promptulate/memory/buffer.py
-promptulate/memory/local_cache.py
+promptulate/memory/file.py
 promptulate/preset_roles/__init__.py
 promptulate/preset_roles/prompt.py
 promptulate/preset_roles/roles.py
 promptulate/provider/__init__.py
+promptulate/provider/base.py
 promptulate/provider/mixins.py
 promptulate/tools/__init__.py
 promptulate/tools/base.py
-promptulate/tools/duckduckgo.py
 promptulate/tools/arxiv/__init__.py
 promptulate/tools/arxiv/api_wrapper.py
 promptulate/tools/arxiv/toolkit.py
 promptulate/tools/arxiv/tools.py
 promptulate/tools/duckduckgo/__init__.py
 promptulate/tools/duckduckgo/api_wrapper.py
 promptulate/tools/duckduckgo/tools.py
@@ -51,8 +54,9 @@
 promptulate/tools/semantic_scholar/api_wrapper.py
 promptulate/tools/semantic_scholar/tools.py
 promptulate/utils/__init__.py
 promptulate/utils/core_utils.py
 promptulate/utils/logger.py
 promptulate/utils/openai_key_pool.py
 promptulate/utils/proxy.py
-promptulate/utils/singleton.py
+promptulate/utils/singleton.py
+promptulate/utils/string_template.py
```

