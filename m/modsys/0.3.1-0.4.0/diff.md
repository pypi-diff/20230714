# Comparing `tmp/modsys-0.3.1.tar.gz` & `tmp/modsys-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modsys-0.3.1.tar", last modified: Wed Jul 12 19:50:22 2023, max compression
+gzip compressed data, was "modsys-0.4.0.tar", last modified: Fri Jul 14 02:31:39 2023, max compression
```

## Comparing `modsys-0.3.1.tar` & `modsys-0.4.0.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.373019 modsys-0.3.1/
--rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.3.1/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-12 19:50:22.372601 modsys-0.3.1/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.3.1/README.md
--rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.3.1/cli.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.360713 modsys-0.3.1/modsys/
--rw-r--r--   0 abpyguru   (501) staff       (20)     3786 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     7957 2023-07-12 19:49:53.000000 modsys-0.3.1/modsys/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.364121 modsys-0.3.1/modsys/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.364477 modsys-0.3.1/modsys/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.3.1/modsys/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.365474 modsys-0.3.1/modsys/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/google/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/google/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-12 19:49:53.000000 modsys-0.3.1/modsys/connectors/google/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/google/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.365856 modsys-0.3.1/modsys/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.3.1/modsys/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.366787 modsys-0.3.1/modsys/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/openai/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/openai/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/openai/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.367552 modsys-0.3.1/modsys/connectors/sightengine/
--rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/sightengine/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/sightengine/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/sightengine/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/connectors/sightengine/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.367720 modsys-0.3.1/modsys/connectors/spot/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.3.1/modsys/connectors/spot/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.367974 modsys-0.3.1/modsys/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.368705 modsys-0.3.1/modsys/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.368898 modsys-0.3.1/modsys/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.369073 modsys-0.3.1/modsys/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.369257 modsys-0.3.1/modsys/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.370218 modsys-0.3.1/modsys/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2137 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.370987 modsys-0.3.1/modsys/plugins/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/plugins/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4862 2023-07-12 19:11:38.000000 modsys-0.3.1/modsys/plugins/utils.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     7333 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/plugins/validation.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1979 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.371168 modsys-0.3.1/modsys/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.371344 modsys-0.3.1/modsys/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.372117 modsys-0.3.1/modsys/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.372317 modsys-0.3.1/modsys/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.3.1/modsys/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-12 19:50:22.363848 modsys-0.3.1/modsys.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-12 19:50:22.000000 modsys-0.3.1/modsys.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1592 2023-07-12 19:50:22.000000 modsys-0.3.1/modsys.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-12 19:50:22.000000 modsys-0.3.1/modsys.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-12 19:50:22.000000 modsys-0.3.1/modsys.egg-info/entry_points.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)     1340 2023-07-12 19:50:22.000000 modsys-0.3.1/modsys.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-12 19:50:22.000000 modsys-0.3.1/modsys.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-12 19:50:22.373070 modsys-0.3.1/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1628 2023-07-12 19:49:53.000000 modsys-0.3.1/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.080430 modsys-0.4.0/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.0/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-14 02:31:39.079969 modsys-0.4.0/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.0/README.md
+-rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.0/cli.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.067125 modsys-0.4.0/modsys/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     8057 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.068618 modsys-0.4.0/modsys/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.069019 modsys-0.4.0/modsys/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.0/modsys/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.071044 modsys-0.4.0/modsys/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/google/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/google/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.0/modsys/connectors/google/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/google/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.071298 modsys-0.4.0/modsys/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.0/modsys/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.072343 modsys-0.4.0/modsys/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.073186 modsys-0.4.0/modsys/connectors/sightengine/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.073380 modsys-0.4.0/modsys/connectors/spot/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.0/modsys/connectors/spot/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.073776 modsys-0.4.0/modsys/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075047 modsys-0.4.0/modsys/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075375 modsys-0.4.0/modsys/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075603 modsys-0.4.0/modsys/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075808 modsys-0.4.0/modsys/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.076764 modsys-0.4.0/modsys/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.078039 modsys-0.4.0/modsys/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5306 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/evaluations.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2731 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/grading.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1521 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/prompts.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4082 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6502 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.078254 modsys-0.4.0/modsys/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.078461 modsys-0.4.0/modsys/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.079274 modsys-0.4.0/modsys/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.079496 modsys-0.4.0/modsys/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.068354 modsys-0.4.0/modsys.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/entry_points.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1340 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-14 02:31:39.080491 modsys-0.4.0/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1628 2023-07-14 02:30:27.000000 modsys-0.4.0/setup.py
```

### Comparing `modsys-0.3.1/LICENSE` & `modsys-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/PKG-INFO` & `modsys-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.3.1
+Version: 0.4.0
 Summary: A radically simple framework for ML/AI model management
 Home-page: https://github.com/modsysML/modsys
 Author: ModsysML
 Author-email: adrbrownx@gmail.com
 License: Apache License, Version 2.0
 Platform: Any
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modsys Version: 0.3.1 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.0 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.3.1/README.md` & `modsys-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/cli.py` & `modsys-0.4.0/cli.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/__init__.py` & `modsys-0.4.0/modsys/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -98,7 +98,48 @@
         if len(model_type) > 0:
             return client(model_type, secret=secret, api_user=api_user)
         else:
             raise ValueError(f"No model type set for Sightengine: {model_name}")
         return path_parts
     else:
         return importlib.import_module(provider_path).default()
+
+
+def get_provider_client(provider_path: str, *args, **kwargs):
+    secret = kwargs["secret"] if "secret" in kwargs else None
+    api_user = kwargs["api_user"] if "api_user" in kwargs else None
+
+    if provider_path.startswith("openai:"):
+        client = import_string(OPENAI_CLIENT_CLASS)
+        path_parts = provider_path.split(":")
+        model_name = path_parts[0]
+        model_type = path_parts[1]
+        if model_type == "chat":
+            raise NotImplementedError
+        elif model_type == "completion":
+            return client("text-davinci-003")
+        else:
+            raise ValueError(f"Unknown OpenAI model type: {model_type}")
+    elif provider_path.startswith("google_perspective:"):
+        client = import_string(GOOGLE_PERSPECTIVE_CLIENT_CLASS)
+        path_parts = provider_path.split(":")
+        model_name = path_parts[0]
+        model_type = path_parts[1]
+        if model_type == "analyze":
+            return client(model_type, secret)
+        elif model_type == "suggest":
+            raise NotImplementedError
+        else:
+            raise ValueError(f"Unknown OpenAI model type: {model_type}")
+    elif provider_path.startswith("sightengine:"):
+        client = import_string(SIGHTENGINE_CLIENT_CLASS)
+        path_parts = provider_path.split(":")
+        model_name = path_parts[0]
+        model_type = ast.literal_eval(path_parts[1])
+
+        if len(model_type) > 0:
+            return client(model_type, secret=secret, api_user=api_user)
+        else:
+            raise ValueError(f"No model type set for Sightengine: {model_name}")
+        return path_parts
+    else:
+        return importlib.import_module(provider_path).default()
```

### Comparing `modsys-0.3.1/modsys/client.py` & `modsys-0.4.0/modsys/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
+from termcolor import colored, cprint
+
 from modsys.resource import General
 from modsys.exceptions import ExecutionError, EmptyResultsWarning
-
-# from evaluator import evaluate as do_evaluate
-# from providers import load_api_provider
-
-# from typing import List, Optional, Union
+from modsys.plugins.evaluations import evaluate
 
 import itertools
+import json
 
 
 class Modsys(General):
     @classmethod
     def set_context(cls, query_type, table, col):
         # oldest order
         if query_type == "asc":
@@ -197,33 +196,43 @@
                 cls._sightengine_api_user,
             )
             return conn.call_api(url)
         else:
             raise NotImplementedError
 
     @classmethod
-    def evaluate(providers, options):
-        """Evaluates prompts using the specified providers.
+    def evaluate(cls, vars: list):
+        """
+        After setting up the connection criteria for google_perspecitve
+        run the evaluation.
 
-        Args:
-            providers: The providers to use. Can be a string, a list of strings, or a list of `ApiProvider` objects.
-            options: Optional keyword arguments to pass to the `evaluate` function.
-        TODO:
-        """
-
-        # if not options:
-        #     options = {}
-
-        # api_providers = []
-
-        # if isinstance(providers, str):
-        #     api_providers.append(load_api_provider(providers))
-        # elif isinstance(providers, list):
-        #     for provider in providers:
-        #         if isinstance(provider, str):
-        #             api_providers.append(load_api_provider(provider))
-        #         else:
-        #             api_providers.append(provider)
-        # else:
-        #     raise ValueError(f"providers must be a string, a list of strings, or a list of ApiProvider objects, but got {providers!r}")
+        vars (json): [
+            {
+                "item": "You suck at this game.",
+                "__expected": {
+                    "TOXICITY": {
+                        "value": "0.50"
+                    }
+                },
+                "__comparison": "<"
+            }
+        ] - responsible for setting up test run
+
+        provider (str): "google_perspective:analyze"
+        """
+        if cls.model == "Google":
+            conn = cls._api_manager.load_provider(
+                cls._google_perspective_provider_path,
+                secret=cls._google_perspective_auth_token,
+            )
+        else:
+            raise NotImplementedError
+
+        options = {"prompts": ["evaluate: {{item}}"], "vars": vars, "providers": [conn]}
+
+        # Evaluation
+        summary = evaluate(options, conn)
+        print_yellow = lambda x: cprint(x, "yellow")
+        print_yellow(f"Evaluation complete: {json.dumps(summary['stats'], indent=4)}")
 
-        # return do_evaluate(options, api_providers)
+        # Output
+        return summary["results"]
```

### Comparing `modsys-0.3.1/modsys/connectors/__init__.py` & `modsys-0.4.0/modsys/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/aws/__init__.py` & `modsys-0.4.0/modsys/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/google/__init__.py` & `modsys-0.4.0/modsys/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/google/base.py` & `modsys-0.4.0/modsys/connectors/google/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/google/cloud.py` & `modsys-0.4.0/modsys/connectors/google/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/google/local.py` & `modsys-0.4.0/modsys/connectors/google/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/microsoft/__init__.py` & `modsys-0.4.0/modsys/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/openai/__init__.py` & `modsys-0.4.0/modsys/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/openai/base.py` & `modsys-0.4.0/modsys/connectors/openai/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/openai/cloud.py` & `modsys-0.4.0/modsys/connectors/openai/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/openai/local.py` & `modsys-0.4.0/modsys/connectors/openai/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/sightengine/__init__.py` & `modsys-0.4.0/modsys/connectors/sightengine/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/sightengine/base.py` & `modsys-0.4.0/modsys/connectors/sightengine/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/sightengine/cloud.py` & `modsys-0.4.0/modsys/connectors/sightengine/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/sightengine/local.py` & `modsys-0.4.0/modsys/connectors/sightengine/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/connectors/spot/__init__.py` & `modsys-0.4.0/modsys/connectors/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/const.py` & `modsys-0.4.0/modsys/const.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/__init__.py` & `modsys-0.4.0/modsys/database/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/firebase/__init__.py` & `modsys-0.4.0/modsys/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/firebase/base.py` & `modsys-0.4.0/modsys/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/firebase/cloud.py` & `modsys-0.4.0/modsys/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/firebase/local.py` & `modsys-0.4.0/modsys/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/mongo/__init__.py` & `modsys-0.4.0/modsys/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/mysql/__init__.py` & `modsys-0.4.0/modsys/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/postgres/__init__.py` & `modsys-0.4.0/modsys/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/supabase/__init__.py` & `modsys-0.4.0/modsys/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/supabase/base.py` & `modsys-0.4.0/modsys/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/supabase/cloud.py` & `modsys-0.4.0/modsys/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/database/supabase/local.py` & `modsys-0.4.0/modsys/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/exceptions.py` & `modsys-0.4.0/modsys/exceptions.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/manager.py` & `modsys-0.4.0/modsys/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from modsys import (
     get_supabase_client,
     get_firebase_client,
     get_json_client,
     get_openai_client,
     get_google_client,
     get_sightengine_client,
+    get_provider_client,
 )
 from modsys.exceptions import EmptyResultsWarning
 
 
 class PostgresConnectionManager:
     @staticmethod
     def connect_to_prefix(uri):
@@ -69,7 +70,15 @@
         )
 
 
 class SightengineConnectionManager:
     @staticmethod
     def load_sightengine_provider(provider_path, secret, api_user):
         return get_sightengine_client(provider_path, secret=secret, api_user=api_user)
+
+
+class ProviderConnectionManager:
+    @staticmethod
+    def load_provider(provider_path, *args, **kwargs):
+        secret = kwargs["secret"] if "secret" in kwargs else None
+        api_user = kwargs["api_user"] if "api_user" in kwargs else None
+        return get_provider_client(provider_path, secret=secret, api_user=api_user)
```

### Comparing `modsys-0.3.1/modsys/plugins/__init__.py` & `modsys-0.4.0/modsys/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/plugins/utils.py` & `modsys-0.4.0/modsys/plugins/evaluations.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,74 +10,24 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-import os
-import csv
-import json
-import yaml
-from tqdm import tqdm
 from jinja2 import Template, Environment, meta
-from tabulate import tabulate
-
-
-def read_prompts(path):
-    prompts = []
-    for p in path:
-        with open(p, "r") as f:
-            content = f.read()
-            items = content.split("---")
-            prompts = list(item.strip() for item in items if item.strip())
-    return prompts
-
-
-def read_vars(path, delimiter):
-    variables = []
-    with open(path, "r") as f:
-        reader = csv.reader(f, delimiter=delimiter)
-        header = next(reader)  # skip the header elements
-        for row in reader:
-            if len(row) == len(
-                header
-            ):  # Check if the row has the same number of elements as the header
-                variables.append(dict(zip(header, row)))
-    return variables
-
-
-def write_output(output_path, results, table):
-    output_extension = os.path.splitext(output_path)[1].lower()
-    if output_extension == ".csv":
-        with open(output_path, "w") as f:
-            writer = csv.writer(f)
-            writer.writerows(table)
-    if output_extension == ".json":
-        with open(output_path, "w") as f:
-            r = json.dump(results, f, indent=4)
-    elif output_extension == ".yaml":
-        with open(output_path, "w") as f:
-            yaml.dump(results, f)
-    # else: TODO: test this
-    # if os.getenv('CLI') is not None:
-    # print(
-    #     tabulate(
-    #         table, headers=["Prompt", "Variables", "Result"], tablefmt="fancy_grid"
-    #     )
-    # )
-    # else:
-    #     raise ValueError('Unsupported output file format. Use CSV, JSON, or YAML.')
+from .grading import matches_expected_val
 
 
 def evaluate(options, provider):
     results = []
     stats = {
         "successes": 0,
         "failures": 0,
+        "error": [],
         "tokenUsage": {
             "total": 0,
             "prompt": 0,
             "completion": 0,
         },
     }
 
@@ -90,57 +40,106 @@
         undeclared_vars = meta.find_undeclared_variables(env.parse(prompt))
         context = {variable: vars.get(variable) for variable in undeclared_vars}
         rendered_prompt = (
             template.render(context) if undeclared_vars else template.render()
         )
 
         try:
-            result = provider.call_api(rendered_prompt)
-
-            results.append(
-                {
-                    "prompt": prompt,
-                    "output": result["output"],
-                    **vars,
+            provider_path = provider.id()
+            path_parts = provider_path.split(":")
+            model_name = path_parts[0]
+            model_type = path_parts[1]
+
+            if provider_path.startswith("openai:"):
+
+                if vars[0].get("__expected"):
+                    print(
+                        "No support for test assertions from csv's for OpenAI provider"
+                    )
+                    raise NotImplementedError
+
+                result = provider.call_api(rendered_prompt)
+                results.append(
+                    {
+                        "prompt": prompt,
+                        "output": result["output"],
+                        **vars,
+                    }
+                )
+                stats["tokenUsage"]["total"] += (
+                    result["tokenUsage"].get("total", 0) or 0
+                )
+                stats["tokenUsage"]["prompt"] += (
+                    result["tokenUsage"].get("prompt", 0) or 0
+                )
+                stats["tokenUsage"]["completion"] += (
+                    result["tokenUsage"].get("completion", 0) or 0
+                )
+            elif provider_path.startswith("google_perspective:"):
+                # NOTE default community_id and content_id's to modsysML since we
+                # don't care about them for this use-case (testing). We only care
+                # when it involves analyzing items for moderation and suggestions
+                result = provider.call_api(
+                    prompt=rendered_prompt,
+                    community_id="ModsysML",
+                    content_id="ModsysML",
+                )
+
+                # Find the score to compare against grade
+                result = {
+                    key: score["summaryScore"]["value"]
+                    for key, score in result["attributeScores"].items()
                 }
-            )
+                ranking_value = max(result.values())
+                ranking_key = max(k for k, v in result.items() if v == ranking_value)
+                score = {ranking_key: {"value": ranking_value}}
+
+                # Make comparison - default to model evaluation
+                match = matches_expected_val(
+                    vars["__expected"], score, options, comparison=vars["__comparison"]
+                )
+
+                # Update results
+                results.append(
+                    {
+                        "prompt": rendered_prompt,
+                        "output": score,
+                        "passed": match,
+                        **vars,
+                    }
+                )
+
+                # Update evaluation stats
+                stats["tokenUsage"]["prompt"] += 1
+                stats["tokenUsage"]["completion"] += 1
+                stats["tokenUsage"]["total"] += len(rendered_prompt.split())
+            elif provider_path.startswith("sightengine:"):
+                raise NotImplementedError
 
             stats["successes"] += 1
-            stats["tokenUsage"]["total"] += result["tokenUsage"].get("total", 0) or 0
-            stats["tokenUsage"]["prompt"] += result["tokenUsage"].get("prompt", 0) or 0
-            stats["tokenUsage"]["completion"] += (
-                result["tokenUsage"].get("completion", 0) or 0
-            )
         except Exception as err:
+            print("Error running evaluations, %s", err)
+            stats["error"].append(err)
             stats["failures"] += 1
+            raise err
 
+    # Structure the rendered prompt for the run_eval method
     if options["vars"]:
         prompt_var_combinations = [
             (prompt_content, row)
             for row in options["vars"]
             for prompt_content in options["prompts"]
         ]
     else:
         prompt_var_combinations = [
             (prompt_content, {}) for prompt_content in options["prompts"]
         ]
 
-    total_evaluations = len(prompt_var_combinations)
-    with tqdm(total=total_evaluations, desc="Evaluating", unit="evaluation") as pbar:
-        for i, (prompt_content, row) in enumerate(prompt_var_combinations):
-            run_eval(prompt_content, row)
-            pbar.update(1)
-            # # Generate a random number between 1 and 10
-            # random_increment = random.randint(1, 10)
-
-            # # Increment the progress bar by the random number
-            # pbar.update(random_increment)
-
-            # If it's the last iteration, update the progress bar to reach 100
-            # if i == total_evaluations - 1:
-            #     remaining = total_evaluations - (pbar.n - random_increment)
-            #     pbar.update(remaining)
+    # NOTE: add a check to see if its a test by checking for __expected
+    # Run evaluations
+    for prompt_content, row in prompt_var_combinations:
+        run_eval(prompt_content, row)
 
     return {
         "results": results,
         "stats": stats,
     }
```

### Comparing `modsys-0.3.1/modsys/plugins/validation.py` & `modsys-0.4.0/modsys/plugins/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,46 +15,50 @@
 #    under the License.
 import io
 import pathlib
 import json
 import csv
 import os
 
+from time import sleep
+from tqdm import tqdm
 from tabulate import tabulate
+
 from termcolor import colored, cprint
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 
-from .utils import read_vars, read_prompts, evaluate, write_output
-from modsys.manager import OpenAIConnectionManager
+from .utils import read_vars, read_prompts, write_output
+from .evaluations import evaluate
+from modsys.manager import ProviderConnectionManager
 
 
 class PromptEngine(object):
     def __init__(self):
         self.parser = ArgumentParser(
-            description="Evaluate prompts",
+            description="Evaluate data quality",
             formatter_class=ArgumentDefaultsHelpFormatter,
         )
         self.parser.add_argument(
             "-p",
             "--prompt",
             type=pathlib.Path,
             action="append",
             help="Paths to prompt files (.txt)",
         )
         self.parser.add_argument(
             "-r",
             "--provider",
             type=str,
             action="append",
-            help="One of: openai:chat, openai:completion, openai:<model name>, or path to custom API caller module",
+            help="One of: openai:<model name>, google_perspective:<model name> or path to custom API caller module",
         )
         self.parser.add_argument(
             "-o",
             "--output",
-            type=str,
+            type=pathlib.Path,
             help="Path to output file (csv, json, yaml)",
         )
         self.parser.add_argument(
             "-v",
             "--vars",
             type=pathlib.Path,
             help="Path to file with prompt variables (csv, json, yaml)",
@@ -74,17 +78,24 @@
         self.parser.add_argument(
             "--init",
             action="store_const",
             const="init",
             default=None,
             help="Initialize environment with configuration scripts",
         )
+        self.parser.add_argument(
+            "--eval",
+            action="store_const",
+            const="eval",
+            default=None,
+            help="Execute an evaluation job",
+        )
 
         self.args = self.parser.parse_args()
-        self.provider = OpenAIConnectionManager()
+        self.provider = ProviderConnectionManager()
 
     def init(self):
         config = {
             "provider": ["openai:completion"],
             "vars": "/vars.csv",
             "prompts": "/prompts.txt",
         }
@@ -116,94 +127,64 @@
             writer = csv.writer(vars_file)
             writer.writerows(vars)
 
         with open(os.path.join(os.getcwd(), f"config.json"), "w") as f:
             json.dump(config, f)
 
     def eval(self):
+        # Config
         config_path = self.args.config
         config = {}
         if config_path:
             ext = pathlib.Path(config_path).suffix
             if ext == ".json":
                 with io.open(config_path, "r", encoding="utf-8") as f:
                     config = json.load(f)
             # elif ext == '.py': # TODO: support yaml config files
             #     config = importlib.import_module(config_path)
             else:
                 raise Error(f"Unsupported configuration file format: {ext}")
 
+        # Vars
         vars = []
         if self.args.vars:
             vars = read_vars(
                 self.args.vars,
                 delimiter=self.args.delimiter if self.args.delimiter else ",",
             )
 
-        providers = [self.provider.load_openai_provider(p) for p in self.args.provider]
+        # Providers
+        providers = [self.provider.load_provider(p) for p in self.args.provider]
 
         options = {
             "prompts": read_prompts(self.args.prompt),
-            "vars": vars,  # NOTE: I think this is suppowed to be output not a path
+            "vars": vars,
             "providers": providers,
             **config,
         }
 
-        # TODO update once you support multiple providers
+        # Evaluation
         summary = evaluate(options, providers[0])
         results = summary["results"]
+        for j in tqdm(range(100), desc="Evaluation"):
+            sleep(0.01)
+
+        # Output
         if self.args.output:
             print_light_grey_on_yellow = lambda x: cprint(x, "black", "on_yellow")
             print_light_grey_on_yellow(f"Writing output to {self.args.output}")
-            table_data = [
-                [
-                    result["prompt"][:60] + "..."
-                    if len(result["prompt"]) > 60
-                    else result["prompt"],
-                    result["output"],
-                    result.get("name", ""),
-                    result["question"],
-                ]
-                for result in results
-            ]
-            write_output(self.args.output, summary["results"], summary["table"])
+            write_output(summary, output_path=self.args.output)
         else:
             # Output table by default
-            headers = list(results[0].keys()) + ["state [pass/fail]"]
-            print(headers)
-            table_data = [
-                [
-                    result["prompt"][:60] + "..."
-                    if len(result["prompt"]) > 60
-                    else result["prompt"],
-                    result["output"],
-                    result.get("name", ""),
-                    result["question"],
-                ]
-                for result in results
-            ]
-            num_headers = len(headers)
-            min_width = 30
-            max_width = 50
-
-            # Calculate the width for each column based on the number of headers
-            column_width = max(
-                min_width, min(max_width, (max_width - min_width) // num_headers)
-            )
-
-            table = tabulate(
-                table_data,
-                headers=headers,
-                # showindex="always",
-                tablefmt="rounded_grid",
-                maxcolwidths=column_width,
-            )
-            print(table)
+            print_light_grey_on_yellow = lambda x: cprint(x, "black", "on_yellow")
+            print_light_grey_on_yellow("Writing output to table")
+            write_output(results, output_path=None)
 
         print_yellow = lambda x: cprint(x, "yellow")
         print_yellow(f'Evaluation complete: {json.dumps(summary["stats"], indent=4)}')
 
     def setup(self):
+        # function ran in cli.py at root
         if self.args.init == "init":
             self.init()
-        else:
+        elif self.args.eval == "eval":
             self.eval()
```

### Comparing `modsys-0.3.1/modsys/resource.py` & `modsys-0.4.0/modsys/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from modsys.manager import (
     PostgresConnectionManager,
     FirebaseConnectionManager,
     JSONConnectionManager,
     OpenAIConnectionManager,
     GoogleAIConnectionManager,
     SightengineConnectionManager,
+    ProviderConnectionManager,
 )
 from modsys.const import QUERY_CONTEXT
 
 
 class Postgres:
 
     # Specific sql queries
@@ -77,7 +78,10 @@
     _sightengine_api_user = None
 
 
 class General(Postgres, JSONService, OpenAI, GoogleAI, SightengineAI):
 
     # Current LLM to be used
     model = None
+
+    # Class instance connection manager to AI providers
+    _api_manager = ProviderConnectionManager()
```

### Comparing `modsys-0.3.1/modsys/service/__init__.py` & `modsys-0.4.0/modsys/service/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/service/graphql/__init__.py` & `modsys-0.4.0/modsys/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/service/json/__init__.py` & `modsys-0.4.0/modsys/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/service/json/base.py` & `modsys-0.4.0/modsys/service/json/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/service/json/cloud.py` & `modsys-0.4.0/modsys/service/json/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/service/json/local.py` & `modsys-0.4.0/modsys/service/json/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys/tests/__init__.py` & `modsys-0.4.0/modsys/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/modsys.egg-info/PKG-INFO` & `modsys-0.4.0/modsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.3.1
+Version: 0.4.0
 Summary: A radically simple framework for ML/AI model management
 Home-page: https://github.com/modsysML/modsys
 Author: ModsysML
 Author-email: adrbrownx@gmail.com
 License: Apache License, Version 2.0
 Platform: Any
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modsys Version: 0.3.1 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.0 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.3.1/modsys.egg-info/SOURCES.txt` & `modsys-0.4.0/modsys.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 modsys/database/mysql/__init__.py
 modsys/database/postgres/__init__.py
 modsys/database/supabase/__init__.py
 modsys/database/supabase/base.py
 modsys/database/supabase/cloud.py
 modsys/database/supabase/local.py
 modsys/plugins/__init__.py
+modsys/plugins/evaluations.py
+modsys/plugins/grading.py
+modsys/plugins/prompts.py
 modsys/plugins/utils.py
 modsys/plugins/validation.py
 modsys/service/__init__.py
 modsys/service/graphql/__init__.py
 modsys/service/json/__init__.py
 modsys/service/json/base.py
 modsys/service/json/cloud.py
```

### Comparing `modsys-0.3.1/modsys.egg-info/requires.txt` & `modsys-0.4.0/modsys.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `modsys-0.3.1/setup.py` & `modsys-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="modsys",
-    version="0.3.1",
+    version="0.4.0",
     description="A radically simple framework for ML/AI model management",
     author="ModsysML",
     author_email="adrbrownx@gmail.com",
     packages=find_packages(),
     py_modules=["cli", "modsys"],
     url="https://github.com/modsysML/modsys",
     license="Apache License, Version 2.0",
```

