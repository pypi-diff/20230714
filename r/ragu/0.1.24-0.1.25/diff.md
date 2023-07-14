# Comparing `tmp/ragu-0.1.24.tar.gz` & `tmp/ragu-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.24.tar", last modified: Fri Jul 14 17:23:17 2023, max compression
+gzip compressed data, was "ragu-0.1.25.tar", last modified: Fri Jul 14 17:30:49 2023, max compression
```

## Comparing `ragu-0.1.24.tar` & `ragu-0.1.25.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.166339 ragu-0.1.24/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.24/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    46991 2023-07-14 17:23:17.166175 ragu-0.1.24/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     5995 2023-07-08 16:50:49.000000 ragu-0.1.24/README.md
--rw-r--r--   0 btober     (501) staff       (20)      910 2023-07-14 17:20:23.000000 ragu-0.1.24/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-14 17:23:17.166374 ragu-0.1.24/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.24/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.131998 ragu-0.1.24/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.133839 ragu-0.1.24/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.135030 ragu-0.1.24/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     2574 2023-07-10 16:30:52.000000 ragu-0.1.24/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.132251 ragu-0.1.24/src/ragu/dat/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.135286 ragu-0.1.24/src/ragu/dat/mars/
--rw-r--r--   0 btober     (501) staff       (20) 33196562 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/dat/mars/mega90n000eb.tif
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.156364 ragu-0.1.24/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.156882 ragu-0.1.24/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    20720 2023-07-08 16:49:36.000000 ragu-0.1.24/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.159629 ragu-0.1.24/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.162907 ragu-0.1.24/src/ragu/recs/
--rw-r--r--   0 btober     (501) staff       (20)  1079564 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/20190928-235534_compiled.jpg
--rw-r--r--   0 btober     (501) staff       (20)    16176 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/basemap_icon.png
--rw-r--r--   0 btober     (501) staff       (20)    92542 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/bulb.jpg
--rw-r--r--   0 btober     (501) staff       (20)    21590 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/recs/ragu_logo.png
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.163738 ragu-0.1.24/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.165861 ragu-0.1.24/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16551 2023-07-08 16:39:19.000000 ragu-0.1.24/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68359 2023-07-10 16:26:13.000000 ragu-0.1.24/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.24/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:23:17.134899 ragu-0.1.24/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    46991 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1369 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       10 2023-07-14 17:23:17.000000 ragu-0.1.24/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.915653 ragu-0.1.25/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.25/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    47007 2023-07-14 17:30:49.915488 ragu-0.1.25/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     5995 2023-07-08 16:50:49.000000 ragu-0.1.25/README.md
+-rw-r--r--   0 btober     (501) staff       (20)      942 2023-07-14 17:30:43.000000 ragu-0.1.25/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2023-07-14 17:30:49.915693 ragu-0.1.25/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.25/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.878463 ragu-0.1.25/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.880412 ragu-0.1.25/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.881307 ragu-0.1.25/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     2574 2023-07-10 16:30:52.000000 ragu-0.1.25/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.878711 ragu-0.1.25/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.881623 ragu-0.1.25/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.908647 ragu-0.1.25/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2344 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2387 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     2935 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3299 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2495 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2829 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2407 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5713 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14114 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2470 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2864 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3573 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.908952 ragu-0.1.25/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    20720 2023-07-08 16:49:36.000000 ragu-0.1.25/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.909481 ragu-0.1.25/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7537 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    11495 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.913782 ragu-0.1.25/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.914404 ragu-0.1.25/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.915222 ragu-0.1.25/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16551 2023-07-08 16:39:19.000000 ragu-0.1.25/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68359 2023-07-10 16:26:13.000000 ragu-0.1.25/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.25/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2023-07-14 17:30:49.881180 ragu-0.1.25/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    47007 2023-07-14 17:30:49.000000 ragu-0.1.25/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2023-07-14 17:30:49.000000 ragu-0.1.25/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2023-07-14 17:30:49.000000 ragu-0.1.25/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2023-07-14 17:30:49.000000 ragu-0.1.25/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2023-07-14 17:30:49.000000 ragu-0.1.25/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2023-07-14 17:30:49.000000 ragu-0.1.25/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.24/LICENSE.txt` & `ragu-0.1.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/PKG-INFO` & `ragu-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.24
+Version: 0.1.25
 Summary: Radar Analysis Graphical Utility (RAGU)
-Author: Michael Christoffersen
-Author-email: Brandon Tober <tobers.brandon@gmail.com>
+Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `ragu-0.1.24/README.md` & `ragu-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/pyproject.toml` & `ragu-0.1.25/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "ragu"
-version = "0.1.24"
+version = "0.1.25"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
      {name = "Brandon Tober", email = "tobers.brandon@gmail.com"},
-     {name = "Michael Christoffersen"},
+     {name = "Michael Christoffersen", email = "mchristo28@gmail.com"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "pandas",
     "numpy",
```

### Comparing `ragu-0.1.24/src/ragu/bin/ragu.py` & `ragu-0.1.25/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/config.py` & `ragu-0.1.25/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/dat/mars/mega90n000eb.tif` & `ragu-0.1.25/src/ragu/dat/mars/mega90n000eb.tif`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/__init__.py` & `ragu-0.1.25/src/ragu/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.25/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.25/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.25/src/ragu/ingest/ingest_groundhog.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.25/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.25/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.25/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.25/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.25/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.25/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.25/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.25/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_template.py` & `ragu-0.1.25/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.25/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/nav/gps.py` & `ragu-0.1.25/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/nav/navparse.py` & `ragu-0.1.25/src/ragu/nav/navparse.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/radar/__init__.py` & `ragu-0.1.25/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/radar/pick.py` & `ragu-0.1.25/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/radar/processing.py` & `ragu-0.1.25/src/ragu/radar/processing.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/recs/20190928-235534_compiled.jpg` & `ragu-0.1.25/src/ragu/recs/20190928-235534_compiled.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/recs/basemap_icon.png` & `ragu-0.1.25/src/ragu/recs/basemap_icon.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/recs/bulb.jpg` & `ragu-0.1.25/src/ragu/recs/bulb.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/recs/ragu_logo.png` & `ragu-0.1.25/src/ragu/recs/ragu_logo.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/tools/export.py` & `ragu-0.1.25/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/tools/utils.py` & `ragu-0.1.25/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ui/basemap.py` & `ragu-0.1.25/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ui/gui.py` & `ragu-0.1.25/src/ragu/ui/gui.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ui/impick.py` & `ragu-0.1.25/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ui/notepad.py` & `ragu-0.1.25/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu/ui/wvpick.py` & `ragu-0.1.25/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.24/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.25/src/ragu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.24
+Version: 0.1.25
 Summary: Radar Analysis Graphical Utility (RAGU)
-Author: Michael Christoffersen
-Author-email: Brandon Tober <tobers.brandon@gmail.com>
+Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `ragu-0.1.24/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.25/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

