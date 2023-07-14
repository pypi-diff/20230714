# Comparing `tmp/betabageldb-0.1.5.tar.gz` & `tmp/betabageldb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.5.tar", last modified: Mon Jul  3 13:23:20 2023, max compression
+gzip compressed data, was "betabageldb-0.1.6.tar", last modified: Fri Jul 14 10:36:14 2023, max compression
```

## Comparing `betabageldb-0.1.5.tar` & `betabageldb-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-03 13:23:20.544093 betabageldb-0.1.5/
--rw-r--r--   0 bidhan     (501) staff       (20)     6088 2023-07-03 13:19:31.000000 betabageldb-0.1.5/BagelDB.py
--rw-r--r--   0 bidhan     (501) staff       (20)       82 2023-06-27 19:31:31.000000 betabageldb-0.1.5/LICENSE.txt
--rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-03 13:23:20.543886 betabageldb-0.1.5/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     3753 2023-07-01 11:28:45.000000 betabageldb-0.1.5/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-03 13:23:20.543478 betabageldb-0.1.5/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     4384 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      215 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        9 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-03 13:23:20.000000 betabageldb-0.1.5/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-03 13:23:20.544137 betabageldb-0.1.5/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)      795 2023-07-03 13:22:47.000000 betabageldb-0.1.5/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-14 10:36:14.012907 betabageldb-0.1.6/
+-rw-r--r--   0 bidhan     (501) staff       (20)     2234 2023-07-14 10:36:14.012684 betabageldb-0.1.6/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     1679 2023-07-14 10:25:37.000000 betabageldb-0.1.6/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-14 10:36:14.012364 betabageldb-0.1.6/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     2234 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      192 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        8 2023-07-14 10:36:13.000000 betabageldb-0.1.6/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-14 10:36:14.012946 betabageldb-0.1.6/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1624 2023-07-14 10:33:33.000000 betabageldb-0.1.6/setup.py
```

