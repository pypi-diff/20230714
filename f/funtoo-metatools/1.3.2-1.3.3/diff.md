# Comparing `tmp/funtoo-metatools-1.3.2.tar.gz` & `tmp/funtoo-metatools-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo-metatools-1.3.2.tar", last modified: Thu Jun 29 16:44:11 2023, max compression
+gzip compressed data, was "funtoo-metatools-1.3.3.tar", last modified: Thu Jul 13 22:10:46 2023, max compression
```

## Comparing `funtoo-metatools-1.3.2.tar` & `funtoo-metatools-1.3.3.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10223 2023-06-29 16:44:05.000000 funtoo-metatools-1.3.2/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-28 13:33:54.000000 funtoo-metatools-1.3.2/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-06-29 16:44:05.000000 funtoo-metatools-1.3.2/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-07-01 21:12:13.000000 funtoo-metatools-1.3.2/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-06-21 18:32:19.000000 funtoo-metatools-1.3.2/bin/blos-check
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-07-05 16:37:27.000000 funtoo-metatools-1.3.2/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5765 2023-06-21 18:57:03.000000 funtoo-metatools-1.3.2/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-07-02 21:37:50.000000 funtoo-metatools-1.3.2/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-11 18:07:53.000000 funtoo-metatools-1.3.2/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-24 17:38:15.000000 funtoo-metatools-1.3.2/bin/fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2023-03-12 20:53:30.000000 funtoo-metatools-1.3.2/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-05-27 22:00:31.000000 funtoo-metatools-1.3.2/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-05-07 21:05:04.000000 funtoo-metatools-1.3.2/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.930894 funtoo-metatools-1.3.2/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-30 18:57:30.000000 funtoo-metatools-1.3.2/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.934894 funtoo-metatools-1.3.2/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25532 2023-05-11 18:07:53.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23252 2023-06-06 20:23:35.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-04-24 17:38:15.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8494 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.938894 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-06-29 16:44:11.000000 funtoo-metatools-1.3.2/funtoo_metatools.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-06 20:18:23.000000 funtoo-metatools-1.3.2/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.942894 funtoo-metatools-1.3.2/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-07-01 21:12:17.000000 funtoo-metatools-1.3.2/metatools/blos.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.942894 funtoo-metatools-1.3.2/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5554 2023-06-21 18:28:47.000000 funtoo-metatools-1.3.2/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-24 17:38:15.000000 funtoo-metatools-1.3.2/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.942894 funtoo-metatools-1.3.2/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8955 2023-06-21 18:34:52.000000 funtoo-metatools-1.3.2/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27292 2023-06-15 16:13:13.000000 funtoo-metatools-1.3.2/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-07-01 21:12:17.000000 funtoo-metatools-1.3.2/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34989 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2023-05-31 18:48:13.000000 funtoo-metatools-1.3.2/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21776 2023-06-21 18:32:19.000000 funtoo-metatools-1.3.2/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-06-21 18:32:19.000000 funtoo-metatools-1.3.2/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18866 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-06-29 16:44:08.000000 funtoo-metatools-1.3.2/metatools/version.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-04-15 18:46:15.000000 funtoo-metatools-1.3.2/metatools/yaml_util.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/metatools/zmq/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-06 20:18:23.000000 funtoo-metatools-1.3.2/metatools/zmq/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/app_core.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/key_monkey.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_breezyops.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-06-29 16:44:11.946894 funtoo-metatools-1.3.2/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-06-29 16:44:08.000000 funtoo-metatools-1.3.2/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-31 18:17:32.000000 funtoo-metatools-1.3.2/setup.py.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-04-15 16:54:39.000000 funtoo-metatools-1.3.2/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.825162 funtoo-metatools-1.3.3/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12021 2023-07-13 22:10:34.000000 funtoo-metatools-1.3.3/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.3/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-07-13 22:09:26.000000 funtoo-metatools-1.3.3/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.3/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1523 2023-06-21 02:46:04.000000 funtoo-metatools-1.3.3/bin/blos-check
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5765 2023-07-10 01:35:42.000000 funtoo-metatools-1.3.3/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.3/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.3/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.3/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.3/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.817162 funtoo-metatools-1.3.3/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25579 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    24204 2023-07-10 01:16:20.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9207 2023-07-10 01:39:44.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8445 2023-07-10 01:39:44.000000 funtoo-metatools-1.3.3/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2065 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-07-13 22:10:46.000000 funtoo-metatools-1.3.3/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      514 2023-06-03 19:14:35.000000 funtoo-metatools-1.3.3/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/blos.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1287 2023-07-10 01:16:43.000000 funtoo-metatools-1.3.3/metatools/cmd.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5554 2023-07-10 01:35:42.000000 funtoo-metatools-1.3.3/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.3/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8962 2023-07-10 01:51:18.000000 funtoo-metatools-1.3.3/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27292 2023-07-13 22:00:11.000000 funtoo-metatools-1.3.3/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/fetch_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    35014 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.3/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21796 2023-07-10 01:01:44.000000 funtoo-metatools-1.3.3/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12435 2023-06-21 02:40:21.000000 funtoo-metatools-1.3.3/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17658 2023-07-10 01:16:43.000000 funtoo-metatools-1.3.3/metatools/tree.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-07-13 22:10:42.000000 funtoo-metatools-1.3.3/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/metatools/yaml_util.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-07-13 22:10:46.821162 funtoo-metatools-1.3.3/metatools/zmq/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2023-06-03 19:08:14.000000 funtoo-metatools-1.3.3/metatools/zmq/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/app_core.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/key_monkey.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_breezyops.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-07-13 22:10:46.825162 funtoo-metatools-1.3.3/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-07-13 22:10:42.000000 funtoo-metatools-1.3.3/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.3/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.3/subpop.yaml
```

### Comparing `funtoo-metatools-1.3.2/.pre-commit-config.yaml` & `funtoo-metatools-1.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/ChangeLog.rst` & `funtoo-metatools-1.3.3/ChangeLog.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,54 @@
+metatools 1.3.3
+===============
+
+Released on July 13, 2023.
+
+This is a maintenance/general update release.
+
+* Fix an bug for where we could receive an HTTP 304 response
+  and not call the proper handling code later, causing a
+  traceback.
+
+* IMPORTANT breaking API change for dynamic archives:
+  myarchive.initialize() is now async and needs to be awaited.
+  This now uses a higher-performance async function (see
+  below for more info.)
+
+* Hub now has a higher-performance hub.cmd.run_bg() function which
+  can be used to run a command in the background and get its
+  exit code as a return value, without pausing the metatools
+  event loop. This should be used instead of ``os.system()``
+  in your autogens.
+
+* Hub now has a hub.cmd.capture_bg() command which is similar to
+  hub.cmd.run_bg() except that it don't emit any output, but
+  instead captures stdout and err into a combined string.
+  It returns a tuple containing the process object (which can
+  be inspected for error code, etc.) and the combined string of
+  stdout and stderr.
+
+* For dynamic archives: ``Archive`` now has a ``work_path`` and
+  an async ``create_work_path`` method. This can be used as a
+  'scratch area' for temporary work. Do an::
+
+   await myarchive.create_work_path()
+
+  ``myarchive.work_path`` is now empty and ready for use.
+
+  ``Archive`` ``.store()`` and ``.store_by_name()`` now accept
+  an ``existing=`` keyword argument which can be used to point
+  to an archive/file that already exists. This will allow you
+  to basically say "THIS is the archive I wish to store -- I
+  have it already". Without using ``existing=``, the default
+  behavior is to tar up the contents of the archive's
+  ``temp_archive_dir`` to create the archive dynamically.
+
+* Convert golang and rust dynamic archive code to use async.
+
 metatools 1.3.2
 ===============
 
 Released on June 29, 2023.
 
 This is a maintenance/general update release.
 
@@ -12,15 +59,15 @@
 * Add additional debugging for ``http_fetch`` if we get a 304 response
   and are not expecting it. In this case, log detailed header information
   so we can troubleshoot it. This may be an infrequently-occurring bug
   that still needs to be fixed. We should only get a 304 if we specify
   ``If-None-Match`` or ``If-Modified-Since``.
 * Small fix to allow Funtoo to only have one Python implementation as
   up until now it has had two (2.7 and 3.7 in 1.4-release, and 3.7
-  and 3.9 in next-release. We are now moving to just 3.9 in next.
+  and 3.9 in next-release. We are now moving to just 3.9 in next.)
 * Add a ``blos-check`` tool to scan the Integrity Database (this is the
   thing that maps a distfile name to a specific binary object in the
   Base Layer Object Store, or BLOS) to look for any missing binary
   objects. This is not really needed but sometimes when I am debugging
   our stores, I need to run this for due diligence. It hasn't found
   any issues yet.
 * Add ``distfile-kit-fetch`` tool which you would run on the system
```

### Comparing `funtoo-metatools-1.3.2/PKG-INFO` & `funtoo-metatools-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.2
+Version: 1.3.3
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.2/README.rst` & `funtoo-metatools-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/blos` & `funtoo-metatools-1.3.3/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/blos-check` & `funtoo-metatools-1.3.3/bin/blos-check`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/deepdive` & `funtoo-metatools-1.3.3/bin/deepdive`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/deepquery` & `funtoo-metatools-1.3.3/bin/deepquery`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/distfile-kit-fetch` & `funtoo-metatools-1.3.3/bin/distfile-kit-fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/distfile-stats` & `funtoo-metatools-1.3.3/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/doit` & `funtoo-metatools-1.3.3/bin/doit`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/fastpull-daemon` & `funtoo-metatools-1.3.3/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/fastpull-daemon-ng` & `funtoo-metatools-1.3.3/bin/fastpull-daemon-ng`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/fastpull-fixer` & `funtoo-metatools-1.3.3/bin/fastpull-fixer`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/fetch` & `funtoo-metatools-1.3.3/bin/fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/interkit-links` & `funtoo-metatools-1.3.3/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/list-kits` & `funtoo-metatools-1.3.3/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/mcafee-tool` & `funtoo-metatools-1.3.3/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/merge-gentoo-staging` & `funtoo-metatools-1.3.3/bin/merge-gentoo-staging`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/merge-kits` & `funtoo-metatools-1.3.3/bin/merge-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/missing-links` & `funtoo-metatools-1.3.3/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/release-yaml-test` & `funtoo-metatools-1.3.3/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/reposcan` & `funtoo-metatools-1.3.3/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/storage-test` & `funtoo-metatools-1.3.3/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/bin/test-metadata-extract` & `funtoo-metatools-1.3.3/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/deprecated/mongo_backends.py` & `funtoo-metatools-1.3.3/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/Makefile` & `funtoo-metatools-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/_ext/_static/consoleoutput.css` & `funtoo-metatools-1.3.3/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/_ext/consoleoutput.py` & `funtoo-metatools-1.3.3/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/autogen-dev.rst` & `funtoo-metatools-1.3.3/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/autogen.rst` & `funtoo-metatools-1.3.3/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/conf.py` & `funtoo-metatools-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/drafts/fastpull_object_store.rst` & `funtoo-metatools-1.3.3/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/drafts/repo_defs.rst` & `funtoo-metatools-1.3.3/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/features/dynamic-archives.rst` & `funtoo-metatools-1.3.3/docs/features/dynamic-archives.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/index.rst` & `funtoo-metatools-1.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/install.rst` & `funtoo-metatools-1.3.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/intro.rst` & `funtoo-metatools-1.3.3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/docs/meta-repo.rst` & `funtoo-metatools-1.3.3/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/autogen.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/autogen.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from typing import Tuple, List
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 from yaml import safe_load
 
 from subpop.util import load_plugin
 
+import metatools.cmd
+
 """
 The `PENDING_QUE` will be built up to contain a full list of all the catpkgs we want to autogen in the full run
 of 'doit'. We queue up everything first so that we have the ability to add QA checks, such as for catpkgs that
 are defined multiple times and other errors that we should catch before processing begins. The work is organized
 by the generator (pop plugin) that will be used to generate a list of catpkgs. Before we start, we have
 everything organized so that we only need to call `execute_generator` once for each generator. It will start
 work for all catpkgs in that generator, and wait for completion of this work before returning.
@@ -386,14 +388,15 @@
 				class AutoHub:
 
 					autogen_id = None
 					sub_path = generator_sub_path
 					THREAD_CTX = hub.THREAD_CTX
 					get_page = pkgtools.fetch.get_page
 					temp_path = pkgtools.model.temp_path
+					cmd = metatools.cmd
 
 					def __init__(self, autogen_id, pkgtools):
 						self.autogen_id = autogen_id
 						# self.pkgtools = FinderWrapper(pkgtools, self)
 						self.pkgtools = pkgtools
 
 					def Artifact(self, **kwargs):
```

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/ebuild.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/ebuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from collections import OrderedDict
 from datetime import datetime
 from subprocess import getstatusoutput
 from typing import Optional, Tuple
 
 import jinja2
 
-from metatools.tree import run_bg
+from metatools.cmd import capture_bg
 from metatools.store import StoreObject
 from metatools.fastpull.spider import FetchError, FetchRequest
 
 log = logging.getLogger('metatools.autogen')
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 
@@ -72,46 +72,58 @@
 		return os.path.join(pkgtools.model.temp_path, "artifact_extract", self.final_name)
 
 	@property
 	def temp_archive_path(self):
 		return os.path.join(pkgtools.model.temp_path, "archive_create", self.final_name)
 
 	@property
+	def work_path(self):
+		return os.path.join(pkgtools.model.temp_path, "archive_work", self.final_name)
+
+	async def create_work_path(self):
+		if os.path.exists(self.work_path):
+			await capture_bg(f"rm -rf {self.work_path}")
+		os.makedirs(self.work_path, exist_ok=True)
+
+	@property
 	def final_path(self):
 		return self.blos_object.blob.path
 
 	@property
 	def final_name(self):
 		return self._final_name
 
 	@property
 	def top_path(self):
 		if self._top_directory:
 			return os.path.join(self.extract_path, self._top_directory)
 		else:
 			return os.path.join(self.extract_path)
 
-	def initialize(self, top_directory=None):
+	async def initialize(self, top_directory=None):
 		"""
 		This method is supposed to create an empty extract_path so we can fill the archive with
 		things we want. top_directory is optional and specifies the directory to create which will
 		contain the files.
 		:return:
 		"""
 		self._top_directory = top_directory
 		if os.path.exists(self.extract_path):
-			shutil.rmtree(self.extract_path)
+			await capture_bg(f"rm -rf {self.extract_path}")
 		os.makedirs(self.top_path, exist_ok=False)
 
-
-	async def store(self, key: dict = None, metadata: dict = None):
+	async def store(self, key: dict = None, metadata: dict = None, existing=None):
 		"""
-		This method will store an archive as a dynamic archive, indexed by ``key``. If you want
-		to store a dynamic archive for later retrieval *by name*, then use the ``Archive.store_by_name``
-		method instead.
+		This method will store an archive as a dynamic archive, indexed by ``key``. By default, it
+		will use the contents of ```self.temp_archive_path``` to grab the contents; if instead you
+		already have a created archive you want to store, you can simply pass the path in the
+		``existing`` argument, and this exact file will be used instead.
+
+		If you want to store a dynamic archive for later retrieval *by name*, then use the
+		``Archive.store_by_name`` method instead.
 
 		An optional ``metadata`` dictionary can be provided, which will also be stored with the
 		dynamic archive. A datestamp will automatically be stored in ``metadata['created_on']`` for
 		you. All other metadata can be provided by you. This metadata, unlike the key, is not used
 		to *find*/*match* the object when retrieval is attempted; instead, the metadata is just made
 		available to you upon retrieval. So you can use it to store extra things that are of
 		interest to you.
@@ -119,44 +131,47 @@
 		if key is None:
 			key = {}
 
 		if metadata is None:
 			metadata = {}
 		metadata["created_on"] = datetime.utcnow()
 
-		temp_archive = self.temp_archive_path
+		if not existing:
 
-		# Ensure we have a clean location for creating a new temporary archive:
+			temp_archive = self.temp_archive_path
 
-		if not os.path.exists(os.path.dirname(temp_archive)):
-			os.makedirs(os.path.dirname(temp_archive), exist_ok=True)
+			# Ensure we have a clean location for creating a new temporary archive:
 
-		if os.path.exists(temp_archive):
-			os.unlink(temp_archive)
+			if not os.path.exists(os.path.dirname(temp_archive)):
+				os.makedirs(os.path.dirname(temp_archive), exist_ok=True)
 
-		# Create the archive:
+			if os.path.exists(temp_archive):
+				os.unlink(temp_archive)
 
-		if self.final_name.endswith(".tar.xz"):
-			cmd = f"tar -C {self.extract_path} -cJf {temp_archive} ."
-		elif self.final_name.endswith(".tar.gz"):
-			cmd = f"tar -C {self.extract_path} -czf {temp_archive} ."
-		elif self.final_name.endswith(".tar.zst"):
-			cmd = f"tar -C {self.extract_path} -c --zstd -f {temp_archive} ."
-		else:
-			raise ValueError(f"Unrecognized archive format: {self.final_name}. Supported formats: tar.gz, tar.xz, tar.zst")
-		log.debug(f"store: command: {cmd}")
+			# Create the archive:
+
+			if self.final_name.endswith(".tar.xz"):
+				cmd = f"tar -C {self.extract_path} -cJf {temp_archive} ."
+			elif self.final_name.endswith(".tar.gz"):
+				cmd = f"tar -C {self.extract_path} -czf {temp_archive} ."
+			elif self.final_name.endswith(".tar.zst"):
+				cmd = f"tar -C {self.extract_path} -c --zstd -f {temp_archive} ."
+			else:
+				raise ValueError(f"Unrecognized archive format: {self.final_name}. Supported formats: tar.gz, tar.xz, tar.zst")
+			log.debug(f"store: command: {cmd}")
 
-		proc, out = await run_bg(cmd)
-		if proc.returncode != 0:
-			raise pkgtools.ebuild.BreezyError(f"Couldn't execute {cmd}. Output: {out.decode()}")
+			proc, out = await capture_bg(cmd)
+			if proc.returncode != 0:
+				raise pkgtools.ebuild.BreezyError(f"Couldn't execute {cmd}. Output: {out.decode()}")
 
-		# Store in BLOS and create integrity database reference:
+			# Store in BLOS and create integrity database reference:
+			existing = temp_archive
 
-		self.blos_object = pkgtools.model.blos.insert_blob(temp_archive)
-		pkgtools.model.fastpull_session.store_file_dynamic(key, temp_archive, metadata=metadata)
+		self.blos_object = pkgtools.model.blos.insert_blob(existing)
+		pkgtools.model.fastpull_session.store_file_dynamic(key, existing, metadata=metadata)
 
 		# If we are running in non-production mode, then attempt to copy the generated distfile into
 		# /var/cache/portage/distfiles so it is "already fetched" as it will not exist on the CDN yet.
 		# This allows local testing of the autogenerated ebuild:
 
 		if not pkgtools.model.prod:
 			dist_path = f"/var/cache/portage/distfiles/{self.final_name}"
@@ -164,26 +179,29 @@
 			try:
 				if os.path.exists(dist_path):
 					os.unlink(dist_path)
 				shutil.copy(self.blos_object.blob.path, dist_path)
 			except PermissionError:
 				log.warning(f"Unable to copy dynamic archive to {dist_path}. Make sure you are in the portage group.")
 
-	async def store_by_name(self, key: dict = None, metadata: dict = None):
+	async def store_by_name(self, key: dict = None, metadata: dict = None, existing=None):
 		"""
-		This method will store the current archive as a dynamic archive, and will be indexed by name, and with
-		an optional provided key, so that it can be retrieved by name using the ``Archive.find_by_name``
+		This method will store the contents of ``self.temp_archive_path`` as a dynamic archive, and will be indexed by
+		name, and with an optional provided key, so that it can be retrieved by name using the ``Archive.find_by_name``
 		classmethod.
+
+		This method now has an optional ``existing=`` keyword argument if you already have an archive that exists.
+		If you provide a path to this archive, its exact contents will be used instead of tarring up whatever is in
+		``self.temp_archive_path``.
 		"""
 		if key is None:
 			key = {}
 		# We must make final_name part of the key used to find the archive:
 		key["final_name"] = self.final_name
-		return await self.store(key, metadata)
-
+		return await self.store(key, metadata, existing=existing)
 
 	@classmethod
 	def find(cls, key: dict = None, final_name: str = None) -> Tuple[Archive, dict] | Tuple[None, None]:
 		"""
 		This classmethod is the big brother of ``Archive.find_by_name()`` and is more flexible. It allows
 		dynamic archives to be found by an arbitrary key. This allows archives to be found where you may not
 		exactly know the final_name (aka filename) of the archive.
```

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/fetch.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/fetch.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/github.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/github.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/golang.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/golang.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 	:param hub: your hub (local variable)
 	:param pkginfo: your pkginfo
 	:return: an ``Archive``, suitable to be added to ``SRC_URI``.
 	"""
 	gosum_bundle = pkginfo["gosum_bundle"]
 	my_archive = hub.Archive(gosum_bundle.final_name)
-	my_archive.initialize(f"funtoo-go-bundle-{pkginfo['name']}")
+	await my_archive.initialize(f"funtoo-go-bundle-{pkginfo['name']}")
 	module_artifacts = []
 	for mod_attrs in gosum_bundle.mod_attrs_list:
 		module_artifacts.append(hub.pkgtools.ebuild.Artifact(**mod_attrs))
 
 	# Fetch dependencies in parallel
 	await asyncio.gather(*[artifact.fetch() for artifact in module_artifacts])
```

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/http.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/http.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/meson.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/pages.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/pyhelper.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/pyhelper.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/funtoo/pkgtools/rust.py` & `funtoo-metatools-1.3.3/funtoo/pkgtools/rust.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import os
 import subprocess
 import toml
 import asyncio
 import hashlib
 import shutil
 
-import dyne.org.funtoo.metatools.pkgtools as pkgtools
 from subpop.util import AttrDict
 
-from metatools.tree import run_shell
+from metatools.cmd import run_shell
 
 
 async def add_crates_bundle(
 	hub,
 	pkginfo,
 	cargo_lock_data=None,
 	cargo_lock_path=None,
@@ -134,15 +133,15 @@
 		key=crates_bundle.key, final_name=crates_bundle.final_name
 	)
 
 	if crates_archive:
 		return crates_archive
 
 	crates_archive = hub.Archive(crates_bundle.final_name)
-	crates_archive.initialize(f"funtoo-crates-bundle-{pkginfo['name']}")
+	await crates_archive.initialize(f"funtoo-crates-bundle-{pkginfo['name']}")
 
 	crates_artifacts = [
 		hub.pkgtools.ebuild.Artifact(**crate_attrs)
 		for crate_attrs in crates_bundle.crates_attrs
 	]
 
 	# Fetch crates in parallel
```

### Comparing `funtoo-metatools-1.3.2/funtoo_metatools.egg-info/PKG-INFO` & `funtoo-metatools-1.3.3/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.3.2
+Version: 1.3.3
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.3.2/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo-metatools-1.3.3/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 funtoo_metatools.egg-info/PKG-INFO
 funtoo_metatools.egg-info/SOURCES.txt
 funtoo_metatools.egg-info/dependency_links.txt
 funtoo_metatools.egg-info/requires.txt
 funtoo_metatools.egg-info/top_level.txt
 metatools/__init__.py
 metatools/blos.py
+metatools/cmd.py
 metatools/context.py
 metatools/fetch_cache.py
 metatools/hashutils.py
 metatools/kit.py
 metatools/kit_cache.py
 metatools/metadata.py
 metatools/model.py
```

### Comparing `funtoo-metatools-1.3.2/make.sh` & `funtoo-metatools-1.3.3/make.sh`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/blos.py` & `funtoo-metatools-1.3.3/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/config/autogen.py` & `funtoo-metatools-1.3.3/metatools/config/autogen.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/config/base.py` & `funtoo-metatools-1.3.3/metatools/config/base.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/config/merge.py` & `funtoo-metatools-1.3.3/metatools/config/merge.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/context.py` & `funtoo-metatools-1.3.3/metatools/context.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/fastpull/core.py` & `funtoo-metatools-1.3.3/metatools/fastpull/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import logging
 from datetime import datetime
 from typing import Tuple
 
 from metatools.blos import BaseLayerObjectStore
 from metatools.fastpull.spider import FetchRequest, Download
-from metatools.tree import run_bg
+from metatools.cmd import capture_bg
 from metatools.store import Store, FileStorageBackend, DerivedKey, StoreObject
 
 log = logging.getLogger('metatools.autogen')
 
 
 class FileIntegrityError(Exception):
 	pass
@@ -141,15 +141,15 @@
 	elif fn.endswith(".bz2"):
 		run_cmd = "bzip2 -dc {archive} > /dev/null"
 		arc_desc = "bzip2"
 	elif fn.endswith(".xz"):
 		run_cmd = "xz -dc {archive} > /dev/null"
 		arc_desc = "xz"
 	if run_cmd:
-		proc, out = await run_bg(run_cmd.format(archive=download.temp_path))
+		proc, out = await capture_bg(run_cmd.format(archive=download.temp_path))
 		if proc.returncode != 0:
 			raise FileIntegrityError(f"File {download.temp_path} downloaded from {download.request.url} does not appear to be a valid {arc_desc} archive!")
 		log.info(f"Download from {download.request.url} verified as valid {arc_desc} archive.")
 	else:
 		log.debug(f"NO RUN CMD for verifying {download.temp_path}")
 	return download
```

### Comparing `funtoo-metatools-1.3.2/metatools/fastpull/spider.py` & `funtoo-metatools-1.3.3/metatools/fastpull/spider.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/fetch_cache.py` & `funtoo-metatools-1.3.3/metatools/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/hashutils.py` & `funtoo-metatools-1.3.3/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/kit.py` & `funtoo-metatools-1.3.3/metatools/kit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from subpop.util import AttrDict
 
 import metatools.steps
 from metatools.config.merge import AutoGeneratedKit, SourcedKit
 from metatools.hashutils import get_md5
 from metatools.metadata import AUXDB_LINES, get_catpkg_relations_from_depstring, get_filedata, extract_ebuild_metadata, strip_rev
 from metatools.model import get_model
-from metatools.tree import GitTreeError, run_shell, Tree
+from metatools.tree import GitTreeError, Tree
+from metatools.cmd import run_shell
 from metatools.zmq.app_core import RouterListener
 
 model = get_model("metatools.merge")
 
 
 class EclassHashCollection:
 	"""
```

### Comparing `funtoo-metatools-1.3.2/metatools/kit_cache.py` & `funtoo-metatools-1.3.3/metatools/kit_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/metadata.py` & `funtoo-metatools-1.3.3/metatools/metadata.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/model.py` & `funtoo-metatools-1.3.3/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/pretty_logging.py` & `funtoo-metatools-1.3.3/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/steps.py` & `funtoo-metatools-1.3.3/metatools/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 import itertools
 import os
 import re
 import shutil
 import jinja2
 
+import metatools.cmd
 from metatools import metadata
 import metatools.tree
 
 from metatools.model import get_model
 model = get_model("metatools.merge")
 
 
 def run_shell(cmd_list, abort_on_failure=True, chdir=None):
-	return metatools.tree.run_shell(cmd_list, abort_on_failure=abort_on_failure, chdir=chdir, logger=model.log)
+	return metatools.cmd.run_shell(cmd_list, abort_on_failure=abort_on_failure, chdir=chdir, logger=model.log)
 
 
 class MergeStep:
 
 	# This is only used for Repository Steps:
 	collector = None
```

### Comparing `funtoo-metatools-1.3.2/metatools/store.py` & `funtoo-metatools-1.3.3/metatools/store.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/tree.py` & `funtoo-metatools-1.3.3/metatools/tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import asyncio
 import glob
 import logging
 import os
 import subprocess
 
+from metatools.cmd import capture_bg, run_bg, ShellError, run_shell
+
 
 def head_sha1(tree):
 	retval, out = subprocess.getstatusoutput("(cd %s && git rev-parse HEAD)" % tree)
 	if retval == 0:
 		return out.strip()
 	return None
 
@@ -75,15 +76,15 @@
 		cmd_str = f"cd {autogen_path} && doit --fast --fastpull_scope={scope} --moonbeam"
 		if self.model.debug:
 			cmd_str += " --debug"
 			self.log.debug(cmd_str)
 		if self.model.prod:
 			cmd_str += " --prod"
 		# We must fork and run this async, so we can receive moonbeam messages while this is running:
-		retcode = await run_cmd_bg(cmd_str)
+		retcode = await run_bg(cmd_str)
 		# use subprocess.call so we can see the output of autogen:
 		# TODO: we don't need to see this GitTreeError traceback
 		if retcode != 0:
 			self.log.error(f"Command failure from merge-kits: {cmd_str}")
 			raise GitTreeError(f"failed autogen in {self.root} -- offset {src_offset}.")
 		self.autogenned = src_offset
 
@@ -159,15 +160,15 @@
 		cmd += ")\n"
 		print("running: %s" % cmd)
 		myenv = os.environ.copy()
 		if os.geteuid() == 0:
 			# make sure HOME is set if we are root (maybe we entered to a minimal environment -- this will mess git up.)
 			# In particular, a new tmux window will have HOME set to /root but NOT exported. Which will mess git up. (It won't know where to find ~/.gitconfig.)
 			myenv["HOME"] = "/root"
-		retval = await run_cmd_bg(cmd, env=myenv)
+		retval = await run_bg(cmd, env=myenv)
 		if retval not in [0, 1]:  # can return 1
 			print("Commit failed.")
 			raise ShellError("Aborting due to failed command.")
 		if push is True:
 			await self.mirror_local_branches()
 
 	async def mirror_local_branches(self):
@@ -278,15 +279,15 @@
 	async def _create_branches(self):
 		await self.run_shell(f"git checkout master; git checkout -b {self.branch}", chdir=self.root)
 		await self.run_shell(f"git push --set-upstream origin {self.branch}", chdir=self.root)
 
 	# if we don't specify root destination tree, assume we are source only:
 
 	async def has_local_changes(self):
-		proc, out = await run_bg(f"(cd {self.root} && git status --porcelain)")
+		proc, out = await capture_bg(f"(cd {self.root} && git status --porcelain)")
 		out = out.strip()
 		return len(out) > 0
 
 	async def _initialize_tree(self):
 		if self.root is None:
 			base = self.model.source_trees
 			self.root = "%s/%s" % (base, self.name)
@@ -317,15 +318,15 @@
 
 		cur_branch = self.current_local_branch
 
 		# We allow this to be turned off for GitTrees like kit-fixups, where you really don't need any branches
 		# for mirroring purposes and there may be many bugfix branches:
 		if self.checkout_all_branches:
 			# We should also, for the sake of mirroring working, create all local branches for remote branches.
-			proc, stdout = await run_bg(f"(cd {self.root} && git branch -r | grep -v /HEAD)")
+			proc, stdout = await capture_bg(f"(cd {self.root} && git branch -r | grep -v /HEAD)")
 			if proc.returncode != 0:
 				# This will happen if, for example, meta-repo is an AutoGeneratedGitTree, and then it is referenced
 				# as a regular GitTree by deepdive. It will have no remotes.
 				init_branches.append(self.branch)
 			else:
 				for branch in stdout.split():
 					init_branches.append("/".join(branch.split("/")[1:]))
@@ -345,15 +346,15 @@
 
 		for branch in init_branches:
 			if not self.local_branch_exists(branch):
 				await self.git_checkout(branch, from_init=True)
 
 		# if we've gotten here, we can assume that the repo exists at self.root.
 		if self.url is not None and self.origin_check:
-			proc, out = await run_bg("(cd %s && git remote get-url origin)" % self.root)
+			proc, out = await capture_bg("(cd %s && git remote get-url origin)" % self.root)
 			out = out.strip()
 			my_url = self.url
 			if my_url.endswith(".git"):
 				my_url = my_url[:-4]
 			if out.endswith(".git"):
 				out = out[:-4]
 			if out != my_url:
@@ -484,53 +485,7 @@
 			raise GitTreeError(
 				"%s: On branch %s. not able to check out branch %s." % (self.root, self.current_local_branch, branch)
 			)
 		self.branch = branch
 		self.commit_sha1 = sha1
 
 
-async def run_bg(cmd):
-	"""
-	Run command in a forked background process, await its completion -- don't emit any output, but instead capture
-	stdout and err into a combined string.
-
-	Return the process object and the combined string of stdout and stderr.
-	"""
-	proc = await asyncio.create_subprocess_shell(cmd,
-	stdout=asyncio.subprocess.PIPE,
-	stderr=asyncio.subprocess.STDOUT)
-
-	stdout, stderr = await proc.communicate()
-	return proc, stdout.decode("utf-8")
-
-
-async def run_cmd_bg(cmd, env=None):
-	"""
-	Run command in a forked background process, await its completion -- output all its output to existing stdout/err.
-	Return its returncode.
-	"""
-	proc = await asyncio.create_subprocess_shell(cmd, env=env)
-	return await proc.wait()
-
-
-class ShellError(Exception):
-	pass
-
-
-async def run_shell(cmd_list, abort_on_failure=True, chdir=None, logger=None):
-	if isinstance(cmd_list, list):
-		cmd_str = " ".join(cmd_list)
-	else:
-		cmd_str = cmd_list
-	if logger:
-		logger.info(f"executing: {cmd_str}")
-	if chdir:
-		cmd_str = f"( cd {chdir}; {cmd_str})"
-
-	proc, output = await run_bg(cmd_str)
-
-	if proc.returncode != 0:
-		if abort_on_failure:
-			raise ShellError(f"Aborted due to failed command. Error executing '{cmd_str}':\n{output}\n")
-		else:
-			return False
-	return True
```

### Comparing `funtoo-metatools-1.3.2/metatools/yaml_util.py` & `funtoo-metatools-1.3.3/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/zmq/app_core.py` & `funtoo-metatools-1.3.3/metatools/zmq/app_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/zmq/key_monkey.py` & `funtoo-metatools-1.3.3/metatools/zmq/key_monkey.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_breezyops.py` & `funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_breezyops.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/metatools/zmq/zmq_msg_core.py` & `funtoo-metatools-1.3.3/metatools/zmq/zmq_msg_core.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.3.2/setup.py` & `funtoo-metatools-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.3.2",
+	version="1.3.3",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
```

### Comparing `funtoo-metatools-1.3.2/setup.py.in` & `funtoo-metatools-1.3.3/setup.py.in`

 * *Files identical despite different names*

