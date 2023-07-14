# Comparing `tmp/pyezoo-2.0.0.20230714.tar.gz` & `tmp/pyezoo-2.0.0.post20230714.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezoo-2.0.0.20230714.tar", last modified: Fri Jul 14 06:46:43 2023, max compression
+gzip compressed data, was "pyezoo-2.0.0.post20230714.tar", last modified: Fri Jul 14 06:31:08 2023, max compression
```

## Comparing `pyezoo-2.0.0.20230714.tar` & `pyezoo-2.0.0.post20230714.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.642987 pyezoo-2.0.0.20230714/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      994 2023-07-14 06:46:43.642846 pyezoo-2.0.0.20230714/PKG-INFO
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      817 2023-07-14 06:40:13.000000 pyezoo-2.0.0.20230714/README.md
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.634416 pyezoo-2.0.0.20230714/pyezoo/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     3264 2023-07-14 05:42:34.000000 pyezoo-2.0.0.20230714/pyezoo/__init__.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.635399 pyezoo-2.0.0.20230714/pyezoo/config/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      223 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/config/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     5772 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/config/config.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     3609 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/connections.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.635807 pyezoo-2.0.0.20230714/pyezoo/constants/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    12296 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/constants/ER.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      370 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/constants/FIELD_TYPE.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)        0 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/constants/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     4469 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/cursors.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     4183 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/error.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      996 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/ezoo_log.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.635911 pyezoo-2.0.0.20230714/pyezoo/gen/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/__init__.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.636766 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_algorithm/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       55 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_algorithm/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_algorithm/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)   753911 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_algorithm/ezooapi_algorithm.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_algorithm/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.637326 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_auth/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       50 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_auth/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_auth/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    82890 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_auth/ezooapi_auth.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_auth/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.637905 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_base/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       50 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_base/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_base/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)   147708 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_base/ezooapi_base.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_base/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.638745 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_client/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       52 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_client/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_client/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    66149 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_client/ezooapi_client.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_client/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.639568 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_data/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       50 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_data/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_data/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)   658695 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_data/ezooapi_data.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_data/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.639970 pyezoo-2.0.0.20230714/pyezoo/gen/ezoocommon/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       34 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezoocommon/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezoocommon/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    41022 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezoocommon/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.640377 pyezoo-2.0.0.20230714/pyezoo/gen/ezootypes/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       34 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezootypes/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezootypes/constants.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)   518083 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/gen/ezootypes/ttypes.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.641103 pyezoo-2.0.0.20230714/pyezoo/loadbalance/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)        0 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/loadbalance/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      433 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/loadbalance/strategy.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.642381 pyezoo-2.0.0.20230714/pyezoo/pool/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      136 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/pool/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     4063 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/pool/driver.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)   169483 2023-07-14 06:46:38.000000 pyezoo-2.0.0.20230714/pyezoo/pool/ezooapi.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    10810 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/pool/ezoodb_client.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    11381 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/pool/pooled_db.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    23454 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/pool/pooled_distribute.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)    20748 2023-07-14 05:43:01.000000 pyezoo-2.0.0.20230714/pyezoo/pool/steady_db.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      359 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/times.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.642650 pyezoo-2.0.0.20230714/pyezoo/utils/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       32 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/utils/__init__.py
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      233 2022-06-10 07:40:03.000000 pyezoo-2.0.0.20230714/pyezoo/utils/codec_util.py
-drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:46:43.635053 pyezoo-2.0.0.20230714/pyezoo.egg-info/
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      994 2023-07-14 06:46:43.000000 pyezoo-2.0.0.20230714/pyezoo.egg-info/PKG-INFO
--rw-r--r--   0 caoguiyuan   (501) staff       (20)     1697 2023-07-14 06:46:43.000000 pyezoo-2.0.0.20230714/pyezoo.egg-info/SOURCES.txt
--rw-r--r--   0 caoguiyuan   (501) staff       (20)        1 2023-07-14 06:46:43.000000 pyezoo-2.0.0.20230714/pyezoo.egg-info/dependency_links.txt
--rw-r--r--   0 caoguiyuan   (501) staff       (20)        7 2023-07-14 06:46:43.000000 pyezoo-2.0.0.20230714/pyezoo.egg-info/requires.txt
--rw-r--r--   0 caoguiyuan   (501) staff       (20)        7 2023-07-14 06:46:43.000000 pyezoo-2.0.0.20230714/pyezoo.egg-info/top_level.txt
--rw-r--r--   0 caoguiyuan   (501) staff       (20)       38 2023-07-14 06:46:43.643035 pyezoo-2.0.0.20230714/setup.cfg
--rw-r--r--   0 caoguiyuan   (501) staff       (20)      526 2023-07-14 06:46:37.000000 pyezoo-2.0.0.20230714/setup.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.594992 pyezoo-2.0.0.post20230714/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      993 2023-07-14 06:31:08.594843 pyezoo-2.0.0.post20230714/PKG-INFO
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.587178 pyezoo-2.0.0.post20230714/pyezoo/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     3264 2023-07-14 05:42:34.000000 pyezoo-2.0.0.post20230714/pyezoo/__init__.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.588034 pyezoo-2.0.0.post20230714/pyezoo/config/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      223 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/config/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     5772 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/config/config.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     3609 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/connections.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.588425 pyezoo-2.0.0.post20230714/pyezoo/constants/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    12296 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/constants/ER.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      370 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/constants/FIELD_TYPE.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)        0 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/constants/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     4469 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/cursors.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     4183 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/error.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      996 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/ezoo_log.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.588537 pyezoo-2.0.0.post20230714/pyezoo/gen/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/__init__.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.589470 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_algorithm/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       55 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_algorithm/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_algorithm/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)   753911 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_algorithm/ezooapi_algorithm.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_algorithm/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.590277 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_auth/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       50 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_auth/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_auth/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    82890 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_auth/ezooapi_auth.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_auth/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.590859 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_base/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       50 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_base/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_base/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)   147708 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_base/ezooapi_base.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_base/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.591405 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_client/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       52 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_client/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_client/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    66149 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_client/ezooapi_client.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_client/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.592188 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_data/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       50 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_data/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_data/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)   658695 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_data/ezooapi_data.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      489 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_data/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.592560 pyezoo-2.0.0.post20230714/pyezoo/gen/ezoocommon/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       34 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezoocommon/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezoocommon/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    41022 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezoocommon/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.592951 pyezoo-2.0.0.post20230714/pyezoo/gen/ezootypes/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       34 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezootypes/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      366 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezootypes/constants.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)   518083 2023-07-14 06:31:02.000000 pyezoo-2.0.0.post20230714/pyezoo/gen/ezootypes/ttypes.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.593444 pyezoo-2.0.0.post20230714/pyezoo/loadbalance/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)        0 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/loadbalance/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      433 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/loadbalance/strategy.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.594406 pyezoo-2.0.0.post20230714/pyezoo/pool/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      136 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     4063 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/driver.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)   169483 2023-07-14 06:31:03.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/ezooapi.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    10810 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/ezoodb_client.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    11381 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/pooled_db.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    23454 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/pooled_distribute.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)    20748 2023-07-14 05:43:01.000000 pyezoo-2.0.0.post20230714/pyezoo/pool/steady_db.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      359 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/times.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.594663 pyezoo-2.0.0.post20230714/pyezoo/utils/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       32 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/utils/__init__.py
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      233 2022-06-10 07:40:03.000000 pyezoo-2.0.0.post20230714/pyezoo/utils/codec_util.py
+drwxr-xr-x   0 caoguiyuan   (501) staff       (20)        0 2023-07-14 06:31:08.587785 pyezoo-2.0.0.post20230714/pyezoo.egg-info/
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      993 2023-07-14 06:31:08.000000 pyezoo-2.0.0.post20230714/pyezoo.egg-info/PKG-INFO
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)     1687 2023-07-14 06:31:08.000000 pyezoo-2.0.0.post20230714/pyezoo.egg-info/SOURCES.txt
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)        1 2023-07-14 06:31:08.000000 pyezoo-2.0.0.post20230714/pyezoo.egg-info/dependency_links.txt
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)        7 2023-07-14 06:31:08.000000 pyezoo-2.0.0.post20230714/pyezoo.egg-info/requires.txt
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)        7 2023-07-14 06:31:08.000000 pyezoo-2.0.0.post20230714/pyezoo.egg-info/top_level.txt
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)       38 2023-07-14 06:31:08.595033 pyezoo-2.0.0.post20230714/setup.cfg
+-rw-r--r--   0 caoguiyuan   (501) staff       (20)      481 2023-07-14 06:22:53.000000 pyezoo-2.0.0.post20230714/setup.py
```

### Comparing `pyezoo-2.0.0.20230714/PKG-INFO` & `pyezoo-2.0.0.post20230714/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pyezoo
-Version: 2.0.0.20230714
+Version: 2.0.0.post20230714
 Summary: python3 sdk for ezoodb.
 Author: eZoo
 Author-email: ezoo@ezoodb.com
 Requires: thrift
-Requires-Python: >=3.7
 
-# pyezoo
+## Project description
+
+## pyezoo
+
+pyezoo is a python-sdk for [eZooDB](https://www.ezoodb.com/)
 
-**pyezoo** is a python-sdk for [eZooDB](https://www.ezoodb.com/)
 
 ```python
 >>> from pyezoo import Connection
 >>> conn = Connection(host='xxx.xxx.xxx.xxx', port=9090, user='xxx', password='xxx', auth=True)
 >>> conn.get_client().hello()
 Response(message='Welcome to ezoo!', status=0, cost_time=0.0)
 >>> conn.get_client().get_node_with_id(db_name="xxx", id=1, retry=True)
 node_s(type='xxx', props={...}, node_id=1, status=0, message='OK.', cost_time=0.000112842)
 ```
 
 ## Installing pyezoo and Supported Versions
-
 pyezoo is available op PypI:
 
-```console
+```shell
 python3 -m pip install pyezoo
 ```
-
 pyezoo officially supports Python 3.7+.
 
 ## API Reference and User Guide available on [eZoo-API DOCS](https://www.ezoodb.com/ezoo-doc?u=/doc/3.eZoo%25E6%258A%2580%25E6%259C%25AF%25E6%2589%258B%25E5%2586%258C/5.eZoo-API/)
```

### Comparing `pyezoo-2.0.0.20230714/README.md` & `pyezoo-2.0.0.post20230714/pyezoo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-# pyezoo
+Metadata-Version: 2.1
+Name: pyezoo
+Version: 2.0.0.post20230714
+Summary: python3 sdk for ezoodb.
+Author: eZoo
+Author-email: ezoo@ezoodb.com
+Requires: thrift
+
+## Project description
+
+## pyezoo
+
+pyezoo is a python-sdk for [eZooDB](https://www.ezoodb.com/)
 
-**pyezoo** is a python-sdk for [eZooDB](https://www.ezoodb.com/)
 
 ```python
 >>> from pyezoo import Connection
 >>> conn = Connection(host='xxx.xxx.xxx.xxx', port=9090, user='xxx', password='xxx', auth=True)
 >>> conn.get_client().hello()
 Response(message='Welcome to ezoo!', status=0, cost_time=0.0)
 >>> conn.get_client().get_node_with_id(db_name="xxx", id=1, retry=True)
 node_s(type='xxx', props={...}, node_id=1, status=0, message='OK.', cost_time=0.000112842)
 ```
 
 ## Installing pyezoo and Supported Versions
-
 pyezoo is available op PypI:
 
-```console
+```shell
 python3 -m pip install pyezoo
 ```
-
 pyezoo officially supports Python 3.7+.
 
-## API Reference and User Guide available on [eZoo-API DOCS](https://www.ezoodb.com/ezoo-doc?u=/doc/3.eZoo%25E6%258A%2580%25E6%259C%25AF%25E6%2589%258B%25E5%2586%258C/5.eZoo-API/)
+## API Reference and User Guide available on [eZoo-API DOCS](https://www.ezoodb.com/ezoo-doc?u=/doc/3.eZoo%25E6%258A%2580%25E6%259C%25AF%25E6%2589%258B%25E5%2586%258C/5.eZoo-API/)
```

### Comparing `pyezoo-2.0.0.20230714/pyezoo/__init__.py` & `pyezoo-2.0.0.post20230714/pyezoo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/config/config.py` & `pyezoo-2.0.0.post20230714/pyezoo/config/config.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/connections.py` & `pyezoo-2.0.0.post20230714/pyezoo/connections.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/constants/ER.py` & `pyezoo-2.0.0.post20230714/pyezoo/constants/ER.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/cursors.py` & `pyezoo-2.0.0.post20230714/pyezoo/cursors.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/error.py` & `pyezoo-2.0.0.post20230714/pyezoo/error.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/ezoo_log.py` & `pyezoo-2.0.0.post20230714/pyezoo/ezoo_log.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_algorithm/ezooapi_algorithm.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_algorithm/ezooapi_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_auth/ezooapi_auth.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_auth/ezooapi_auth.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_base/ezooapi_base.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_base/ezooapi_base.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_client/ezooapi_client.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_client/ezooapi_client.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezooapi_data/ezooapi_data.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezooapi_data/ezooapi_data.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezoocommon/ttypes.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezoocommon/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/gen/ezootypes/ttypes.py` & `pyezoo-2.0.0.post20230714/pyezoo/gen/ezootypes/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/pool/driver.py` & `pyezoo-2.0.0.post20230714/pyezoo/pool/driver.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/pool/ezooapi.py` & `pyezoo-2.0.0.post20230714/pyezoo/pool/ezooapi.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/pool/ezoodb_client.py` & `pyezoo-2.0.0.post20230714/pyezoo/pool/ezoodb_client.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/pool/pooled_db.py` & `pyezoo-2.0.0.post20230714/pyezoo/pool/pooled_db.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/pool/pooled_distribute.py` & `pyezoo-2.0.0.post20230714/pyezoo/pool/pooled_distribute.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo/pool/steady_db.py` & `pyezoo-2.0.0.post20230714/pyezoo/pool/steady_db.py`

 * *Files identical despite different names*

### Comparing `pyezoo-2.0.0.20230714/pyezoo.egg-info/SOURCES.txt` & `pyezoo-2.0.0.post20230714/pyezoo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 pyezoo/__init__.py
 pyezoo/connections.py
 pyezoo/cursors.py
 pyezoo/error.py
 pyezoo/ezoo_log.py
 pyezoo/times.py
```

