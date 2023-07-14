# Comparing `tmp/Carter-Offline-1.0.2.tar.gz` & `tmp/Carter-Offline-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-1.0.2.tar", last modified: Tue Jun 13 08:14:53 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.0.tar", last modified: Fri Jul 14 15:00:05 2023, max compression
```

## Comparing `Carter-Offline-1.0.2.tar` & `Carter-Offline-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,19 @@
-drwxr-xr-x   0 jackfranklin   (501) staff       (20)        0 2023-06-13 08:14:53.790417 Carter-Offline-1.0.2/
-drwxr-xr-x   0 jackfranklin   (501) staff       (20)        0 2023-06-13 08:14:53.790114 Carter-Offline-1.0.2/Carter_Offline.egg-info/
--rw-r--r--   0 jackfranklin   (501) staff       (20)      249 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 jackfranklin   (501) staff       (20)      197 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)        1 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)       43 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)        1 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)      249 2023-06-13 08:14:53.790296 Carter-Offline-1.0.2/PKG-INFO
--rw-r--r--   0 jackfranklin   (501) staff       (20)       38 2023-06-13 08:14:53.790455 Carter-Offline-1.0.2/setup.cfg
--rw-r--r--   0 jackfranklin   (501) staff       (20)      526 2023-06-13 08:14:29.000000 Carter-Offline-1.0.2/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:00:05.983339 Carter-Offline-2.0.0/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:00:05.977757 Carter-Offline-2.0.0/Carter-Offline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:00:05.978264 Carter-Offline-2.0.0/Carter-Offline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.0/Carter-Offline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.0/Carter-Offline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)     5868 2023-07-14 14:47:21.000000 Carter-Offline-2.0.0/Carter-Offline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.0/Carter-Offline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.0/Carter-Offline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:00:05.983048 Carter-Offline-2.0.0/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     1802 2023-07-14 15:00:05.000000 Carter-Offline-2.0.0/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      392 2023-07-14 15:00:05.000000 Carter-Offline-2.0.0/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-14 15:00:05.000000 Carter-Offline-2.0.0/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-14 15:00:05.000000 Carter-Offline-2.0.0/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       15 2023-07-14 15:00:05.000000 Carter-Offline-2.0.0/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.0/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     1802 2023-07-14 15:00:05.983230 Carter-Offline-2.0.0/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1415 2023-07-14 14:58:41.000000 Carter-Offline-2.0.0/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-14 15:00:05.983373 Carter-Offline-2.0.0/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-14 14:59:53.000000 Carter-Offline-2.0.0/setup.py
```

