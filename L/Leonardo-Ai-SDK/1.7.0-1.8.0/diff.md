# Comparing `tmp/Leonardo-Ai-SDK-1.7.0.tar.gz` & `tmp/Leonardo-Ai-SDK-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-1.7.0.tar", last modified: Thu Jul 13 00:25:21 2023, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-1.8.0.tar", last modified: Fri Jul 14 00:24:18 2023, max compression
```

## Comparing `Leonardo-Ai-SDK-1.7.0.tar` & `Leonardo-Ai-SDK-1.8.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.528750 Leonardo-Ai-SDK-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-13 00:25:21.528750 Leonardo-Ai-SDK-1.7.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3505 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:25:21.528750 Leonardo-Ai-SDK-1.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.516750 Leonardo-Ai-SDK-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.520750 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 00:25:21.000000 Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.520750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8343 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6385 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/generation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/initimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4716 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.520750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.524750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createdataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7310 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/creategeneration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3867 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createvariationupscale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7835 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getmodelbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getuserself.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getvariationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2397 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploadinitimage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.524750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/controlnet_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/custom_model_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/job_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/sd_generation_style.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/sd_versions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/strength.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/variation_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:25:21.524750 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-13 00:25:10.000000 Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8343 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6385 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/generation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/initimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4716 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createdataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7310 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/creategeneration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3867 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7835 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getuserself.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2397 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploadinitimage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/controlnet_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/custom_model_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/job_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/sd_versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/strength.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/variation_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-1.7.0/LICENSE.md` & `Leonardo-Ai-SDK-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/PKG-INFO` & `Leonardo-Ai-SDK-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 1.7.0
+Version: 1.8.0
 Summary: Leonardo Ai Python Client SDK
 Home-page: UNKNOWN
 Author: Leonardo-Ai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -19,17 +19,19 @@
 ```bash
 pip install Leonardo-Ai-SDK
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
+
+
 ```python
 import leonardoaisdk
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import operations, shared
 
 s = leonardoaisdk.LeonardoAiSDK(
     security=shared.Security(
         bearer_auth="",
     ),
 )
```

### Comparing `Leonardo-Ai-SDK-1.7.0/README.md` & `Leonardo-Ai-SDK-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 ```bash
 pip install Leonardo-Ai-SDK
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
+
+
 ```python
 import leonardoaisdk
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import operations, shared
 
 s = leonardoaisdk.LeonardoAiSDK(
     security=shared.Security(
         bearer_auth="",
     ),
 )
```

### Comparing `Leonardo-Ai-SDK-1.7.0/setup.py` & `Leonardo-Ai-SDK-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="Leonardo-Ai-SDK",
-    version="1.7.0",
+    version="1.8.0",
     author="Leonardo-Ai",
     description="Leonardo Ai Python Client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 1.7.0
+Version: 1.8.0
 Summary: Leonardo Ai Python Client SDK
 Home-page: UNKNOWN
 Author: Leonardo-Ai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -19,17 +19,19 @@
 ```bash
 pip install Leonardo-Ai-SDK
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
+
+
 ```python
 import leonardoaisdk
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import operations, shared
 
 s = leonardoaisdk.LeonardoAiSDK(
     security=shared.Security(
         bearer_auth="",
     ),
 )
```

### Comparing `Leonardo-Ai-SDK-1.7.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '1.7.0'
-    gen_version: str = '2.62.1'
+    sdk_version: str = '1.8.0'
+    gen_version: str = '2.65.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.7.0/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

