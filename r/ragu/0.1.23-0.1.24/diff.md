# Comparing `tmp/ragu-0.1.23.tar.gz` & `tmp/ragu-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.23.tar", last modified: Sat Jul  8 16:52:01 2023, max compression
+gzip compressed data, was "ragu-0.1.24.tar", last modified: Fri Jul 14 17:23:17 2023, max compression
```

## Comparing `ragu-0.1.23.tar` & `ragu-0.1.24.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.188537 ragu-0.1.23/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.23/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    46969 2023-07-08 16:52:01.188362 ragu-0.1.23/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     5995 2023-07-08 16:50:49.000000 ragu-0.1.23/README.md
--rw-r--r--   0 btober     (501) staff       (20)     1018 2023-07-08 16:50:55.000000 ragu-0.1.23/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-08 16:52:01.188575 ragu-0.1.23/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.23/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.164172 ragu-0.1.23/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.165566 ragu-0.1.23/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.166539 ragu-0.1.23/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     1988 2023-07-08 14:00:14.000000 ragu-0.1.23/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.164353 ragu-0.1.23/src/ragu/dat/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.166683 ragu-0.1.23/src/ragu/dat/mars/
--rw-r--r--   0 btober     (501) staff       (20) 33196562 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/dat/mars/mega90n000eb.tif
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.184641 ragu-0.1.23/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.185012 ragu-0.1.23/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    20720 2023-07-08 16:49:36.000000 ragu-0.1.23/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.185551 ragu-0.1.23/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.186621 ragu-0.1.23/src/ragu/recs/
--rw-r--r--   0 btober     (501) staff       (20)  1079564 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/recs/20190928-235534_compiled.jpg
--rw-r--r--   0 btober     (501) staff       (20)    16176 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/recs/basemap_icon.png
--rw-r--r--   0 btober     (501) staff       (20)    92542 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/recs/bulb.jpg
--rw-r--r--   0 btober     (501) staff       (20)    21590 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/recs/ragu_logo.png
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.187178 ragu-0.1.23/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.188073 ragu-0.1.23/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16551 2023-07-08 16:39:19.000000 ragu-0.1.23/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68357 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.23/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-08 16:52:01.166401 ragu-0.1.23/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    46969 2023-07-08 16:52:01.000000 ragu-0.1.23/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1369 2023-07-08 16:52:01.000000 ragu-0.1.23/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-08 16:52:01.000000 ragu-0.1.23/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-08 16:52:01.000000 ragu-0.1.23/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-08 16:52:01.000000 ragu-0.1.23/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       10 2023-07-08 16:52:01.000000 ragu-0.1.23/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.166339 ragu-0.1.24/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.24/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    46991 2023-07-14 17:23:17.166175 ragu-0.1.24/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     5995 2023-07-08 16:50:49.000000 ragu-0.1.24/README.md
+-rw-r--r--   0 btober     (501) staff       (20)      910 2023-07-14 17:20:23.000000 ragu-0.1.24/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-14 17:23:17.166374 ragu-0.1.24/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.24/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.131998 ragu-0.1.24/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.133839 ragu-0.1.24/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.135030 ragu-0.1.24/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     2574 2023-07-10 16:30:52.000000 ragu-0.1.24/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.132251 ragu-0.1.24/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.135286 ragu-0.1.24/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.156364 ragu-0.1.24/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.156882 ragu-0.1.24/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    20720 2023-07-08 16:49:36.000000 ragu-0.1.24/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.159629 ragu-0.1.24/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.162907 ragu-0.1.24/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.163738 ragu-0.1.24/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.165861 ragu-0.1.24/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16551 2023-07-08 16:39:19.000000 ragu-0.1.24/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68359 2023-07-10 16:26:13.000000 ragu-0.1.24/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.134899 ragu-0.1.24/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    46991 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.23/LICENSE.txt` & `ragu-0.1.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/PKG-INFO` & `ragu-0.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.23
+Version: 0.1.24
 Summary: Radar Analysis Graphical Utility (RAGU)
-Author: Brandon S. Tober
-Author-email: tobers.brandon@gmail.com
+Author: Michael Christoffersen
+Author-email: Brandon Tober <tobers.brandon@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `ragu-0.1.23/README.md` & `ragu-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/pyproject.toml` & `ragu-0.1.24/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "ragu"
-version = "0.1.23"
+version = "0.1.24"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
-    {name = "Brandon S. Tober"},
-    {email = "tobers.brandon@gmail.com"}
+     {name = "Brandon Tober", email = "tobers.brandon@gmail.com"},
+     {name = "Michael Christoffersen"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "pandas",
     "numpy",
@@ -24,16 +24,14 @@
     "geopandas"
 ]
 
 [project.urls]
 documentation = "https://github.com/btobers/ragu/wiki"
 repository = "https://github.com/btobers/ragu"
 
-# The following would provide a command line executable called `sample`
-# which executes the function `main` from this package when invoked.
 [project.scripts]
 ragu = "ragu.bin.ragu:main"
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
```

### Comparing `ragu-0.1.23/src/ragu/bin/ragu.py` & `ragu-0.1.24/src/ragu/bin/ragu.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,27 +15,43 @@
 from ragu.ui import gui
 import os,sys,argparse
 import tkinter as tk
 from tkinter import font
 
 def main():
 
+    # get configuration file
+    basedir = os.path.join(os.path.expanduser('~'),'RAGU')
+    if not os.path.isdir(basedir):
+        os.mkdir(basedir)
+    if not os.path.isfile(basedir+'/config.ini'):
+        config.create_config(basedir+'/config.ini')
+    configPath = basedir + '/config.ini'
+
     # set up CLI
     parser = argparse.ArgumentParser(
-    description="Radar Analysis Graphical Utility (RAGU)"
+    description=f"Radar Analysis Graphical Utility (RAGU)\n\nFor documentation see: https://github.com/btobers/RAGU\nDefulat configuration file path: {configPath}",
+        formatter_class=argparse.RawTextHelpFormatter
     )
-    parser.add_argument("path", help="Data file path", nargs='?')
-    path = parser.parse_args().path
+
+    parser.add_argument("datPath", help="Data directory file path", nargs="?", default=None)
+    parser.add_argument("configPath", help="Configuration file path", nargs="?", default=configPath)
+    datPath = parser.parse_args().datPath
+    tmp = parser.parse_args().configPath
 
     # check if path exists
-    if path:
-        if not os.path.isdir(path[0]):
-            print(f"Path not found: {path[0]}")
-            print(f"Defaulting to data path specified in the RAGU configuration file.")
-            path = None
+    if datPath:
+        if not os.path.isdir(datPath[0]):
+            print(f"Data directory not found : {datPath[0]}")
+            print(f"Defaulting to data file path specified in the RAGU configuration file.")
+            datPath = None
+    if os.path.isfile(tmp) and tmp.endswith(".ini"):
+        configPath=tmp
+    else:
+        print(f"Configuration file not found at: {tmp}\nFull file path must be entered.\nDefaulting to: {configPath}")
 
     # change dir to RAGU code directory 
     os.chdir(os.path.dirname(os.path.abspath(__file__)))
 
     # initialize tkinter
     root = tk.Tk()
 
@@ -47,22 +63,14 @@
     try:
         for _i in tk.font.names():
             # tk.font.nametofont(_i).config(family="Times New Roman", size=10, weight="normal")
             tk.font.nametofont(_i).config(size=10, weight="normal")
     except:
         pass
 
-    # get configuration file
-    basedir = os.path.join(os.path.expanduser('~'),'RAGU')
-    if not os.path.isdir(basedir):
-        os.mkdir(basedir)
-    if not os.path.isfile(basedir+'/config.ini'):
-        config.create_config(basedir+'/config.ini')
-    confpath = basedir + '/config.ini'
-
     # call the RAGU mainGUI class
-    gui.mainGUI(root, confpath, datPath = path)
+    gui.mainGUI(root, configPath=configPath, datPath=datPath)
     root.lift()    
     root.mainloop()
 
 if __name__ == "__main__":
     main()
```

### Comparing `ragu-0.1.23/src/ragu/config.py` & `ragu-0.1.24/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/dat/mars/mega90n000eb.tif` & `ragu-0.1.24/src/ragu/dat/mars/mega90n000eb.tif`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/__init__.py` & `ragu-0.1.24/src/ragu/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.24/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.24/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.24/src/ragu/ingest/ingest_groundhog.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.24/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.24/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.24/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.24/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.24/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.24/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.24/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.24/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_template.py` & `ragu-0.1.24/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.24/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/nav/gps.py` & `ragu-0.1.24/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/nav/navparse.py` & `ragu-0.1.24/src/ragu/nav/navparse.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/radar/__init__.py` & `ragu-0.1.24/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/radar/pick.py` & `ragu-0.1.24/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/radar/processing.py` & `ragu-0.1.24/src/ragu/radar/processing.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/recs/20190928-235534_compiled.jpg` & `ragu-0.1.24/src/ragu/recs/20190928-235534_compiled.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/recs/basemap_icon.png` & `ragu-0.1.24/src/ragu/recs/basemap_icon.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/recs/bulb.jpg` & `ragu-0.1.24/src/ragu/recs/bulb.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/recs/ragu_logo.png` & `ragu-0.1.24/src/ragu/recs/ragu_logo.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/tools/export.py` & `ragu-0.1.24/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/tools/utils.py` & `ragu-0.1.24/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ui/basemap.py` & `ragu-0.1.24/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ui/gui.py` & `ragu-0.1.24/src/ragu/ui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import tkinter.ttk as ttk
 # try:
 #     plt.rcParams["font.family"] = "Times New Roman"
 # except:
 #     pass
 
 class mainGUI(tk.Frame):
-    def __init__(self, parent, confpath, datPath, *args, **kwargs):
+    def __init__(self, parent, configPath, datPath, *args, **kwargs):
         tk.Frame.__init__(self, parent, *args, **kwargs)
         self.parent = parent
         # read and parse config
         self.conf = configparser.ConfigParser()
         self.conf.read(confpath)
         if datPath:
             self.datPath = datPath
```

### Comparing `ragu-0.1.23/src/ragu/ui/impick.py` & `ragu-0.1.24/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ui/notepad.py` & `ragu-0.1.24/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu/ui/wvpick.py` & `ragu-0.1.24/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.23/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.24/src/ragu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.23
+Version: 0.1.24
 Summary: Radar Analysis Graphical Utility (RAGU)
-Author: Brandon S. Tober
-Author-email: tobers.brandon@gmail.com
+Author: Michael Christoffersen
+Author-email: Brandon Tober <tobers.brandon@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `ragu-0.1.23/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.24/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

