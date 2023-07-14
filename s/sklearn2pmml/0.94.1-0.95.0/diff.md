# Comparing `tmp/sklearn2pmml-0.94.1.tar.gz` & `tmp/sklearn2pmml-0.95.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.94.1.tar", last modified: Sat Jul  8 06:47:06 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.95.0.tar", last modified: Fri Jul 14 16:52:51 2023, max compression
```

## Comparing `sklearn2pmml-0.94.1.tar` & `sklearn2pmml-0.95.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.1/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.1/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    11627 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6333 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.31.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   202327 2023-06-11 10:10:38.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-python-1.1.15.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.31.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-08 05:55:57.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6242 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.31.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   442644 2023-07-08 05:55:57.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   472037 2023-07-08 06:03:23.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-1.7.31.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-07-08 06:28:35.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    46831 2023-06-15 18:20:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-h2o-1.2.7.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5711 2023-07-08 06:24:13.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7311 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.31.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    83825 2023-07-08 06:03:24.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.31.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/pickle-1.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.94.1/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-07-08 06:24:05.000000 sklearn2pmml-0.94.1/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-08 06:47:06.000000 sklearn2pmml-0.94.1/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.94.1/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.0/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.0/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    12289 2023-07-14 16:34:45.000000 sklearn2pmml-0.95.0/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   472037 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    48655 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-h2o-1.2.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7311 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6244 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    83824 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   203268 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-python-1.1.16.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-08 05:55:57.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    14761 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   442644 2023-07-08 05:55:57.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5709 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pickle-1.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.94.1/LICENSE.txt` & `sklearn2pmml-0.95.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/setup.py` & `sklearn2pmml-0.95.0/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/PKG-INFO` & `sklearn2pmml-0.95.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.94.1
+Version: 0.95.0
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.94.1.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.95.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/h2o.py` & `sklearn2pmml-0.95.0/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/tpot.py` & `sklearn2pmml-0.95.0/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 from sklearn.feature_selection import SelectFromModel
 from sklearn.pipeline import FeatureUnion, Pipeline
 from sklearn_pandas import DataFrameMapper
 from sklearn2pmml.resources import _package_classpath
 from subprocess import PIPE, Popen
 from zipfile import ZipFile
 
+import dill
 import joblib
 import numpy
 import os
 import pandas
 import platform
 import re
 import sklearn
 import sklearn_pandas
 import tempfile
+import warnings
 
 from .metadata import __copyright__, __license__, __version__
 from .pipeline import PMMLPipeline
 
 def _is_categorical(dtype):
 	if dtype == object or dtype == str or dtype == bool:
 		return True
@@ -191,23 +193,32 @@
 			try:
 				zipentry = zipfile.getinfo(name)
 			except KeyError:
 				pass
 			else:
 				fun(zipfile.open(zipentry))
 
-def _dump(obj, prefix):
+def _dill_dump(obj, prefix):
+	fd, path = tempfile.mkstemp(prefix = (prefix + "-"), suffix = ".pkl")
+	try:
+		with open(path, "wb") as dill_file:
+			dill.dump(obj, dill_file)
+	finally:
+		os.close(fd)
+	return path
+
+def _joblib_dump(obj, prefix):
 	fd, path = tempfile.mkstemp(prefix = (prefix + "-"), suffix = ".pkl.z")
 	try:
 		joblib.dump(obj, path, compress = 3)
 	finally:
 		os.close(fd)
 	return path
 
-def sklearn2pmml(pipeline, pmml, with_repr = False, java_home = None, java_opts = None, user_classpath = [], debug = False):
+def sklearn2pmml(pipeline, pmml, with_repr = False, java_home = None, java_opts = None, user_classpath = [], dump_flavour = "joblib", debug = False):
 	"""Converts a fitted PMML pipeline object to PMML file.
 
 	Parameters:
 	----------
 	pipeline: PMMLPipeline
 		The input PMML pipeline object.
 
@@ -225,14 +236,17 @@
 		Java options.
 		Functionally analogous to the JAVA_OPTS environment variable.
 
 	user_classpath: list of strings, optional
 		The paths to JAR files that provide custom Transformer, Selector and/or Estimator converter classes.
 		The SkLearn2PMML classpath is constructed by appending user JAR files to package JAR files.
 
+	dump_flavour: string, optional
+		The flavour of pickle dump files.
+
 	debug: boolean, optional
 		If true, print information about the conversion process.
 
 	"""
 	if debug:
 		java_version = _java_version(java_home = java_home)
 		if java_version is None:
@@ -251,20 +265,28 @@
 		pipeline.repr_ = repr(pipeline)
 	dumps = []
 	try:
 		java_args = ["-cp", os.pathsep.join(_classpath(user_classpath)), "com.sklearn2pmml.Main"]
 		estimator = pipeline._final_estimator
 		# if isinstance(estimator, H2OEstimator):
 		if hasattr(estimator, "download_mojo"):
+			if dump_flavour != "dill":
+				warnings.warn("Changing dump flavour to dill")
+				dump_flavour = "dill"
 			# Avoid MOJO (re-)download if the indicator attribute is set
 			if not hasattr(estimator, "_mojo_path"):
 				estimator_mojo = estimator.download_mojo()
 				dumps.append(estimator_mojo)
 				estimator._mojo_path = estimator_mojo
-		pipeline_pkl = _dump(pipeline, "pipeline")
+		if dump_flavour == "dill":
+			pipeline_pkl = _dill_dump(pipeline, "pipeline")
+		elif dump_flavour == "joblib":
+			pipeline_pkl = _joblib_dump(pipeline, "pipeline")
+		else:
+			raise ValueError("Dump flavour {0} not in {1}".format(dump_flavour, ["dill", "joblib"]))
 		java_args.extend(["--pkl-pipeline-input", pipeline_pkl])
 		dumps.append(pipeline_pkl)
 		java_args.extend(["--pmml-output", pmml])
 		cmd = _make_java_command(java_home = java_home, java_opts = java_opts, java_args = java_args)
 		if debug:
 			print("Executing command:\n{0}".format(" ".join(cmd)))
 		try:
@@ -282,15 +304,15 @@
 				print("Standard error:\n{0}".format(error))
 			else:
 				print("Standard error is empty")
 		if retcode:
 			raise RuntimeError("The SkLearn2PMML application has failed. The Java executable should have printed more information about the failure into its standard output and/or standard error streams")
 	finally:
 		if debug:
-			print("Preserved joblib dump file(s): {0}".format(" ".join(dumps)))
+			print("Preserved dump file(s): {0}".format(" ".join(dumps)))
 		else:
 			for dump in dumps:
 				os.remove(dump)
 
 def _parse_properties(lines):
 	splitter = re.compile("\s*=\s*")
 	properties = dict()
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.95.0/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.95.0/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.95.0/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-python-1.1.15.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-python-1.1.16.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,174 +1,176 @@
-Zip file size: 202327 bytes, number of entries: 172
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Jun-11 13:10 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 patsy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 functools/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 treelib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 pandas/core/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 numpy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 numpy/random/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 numpy/core/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 collections/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 org/jpmml/python/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 joblib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/stats/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/interpolate/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 scipy/sparse/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 builtins/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-11 13:10 META-INF/maven/org.jpmml/pmml-python/
--rw-rw-r--  2.0 unx     2108 b- defN 23-Jun-11 13:10 patsy/PatsyOperation.class
--rw-rw-r--  2.0 unx     2272 b- defN 23-Jun-11 13:10 patsy/PatsyOperator.class
--rw-rw-r--  2.0 unx     3106 b- defN 23-Jun-11 13:10 patsy/PatsyToken.class
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-11 13:10 patsy/PatsyFactor.class
--rw-rw-r--  2.0 unx      747 b- defN 23-Jun-11 13:10 patsy/PatsyTerm.class
--rw-rw-r--  2.0 unx     8491 b- defN 23-Jun-11 13:10 patsy/FormulaParser.class
--rw-rw-r--  2.0 unx     3114 b- defN 23-Jun-11 13:10 META-INF/python2pmml.properties
--rw-rw-r--  2.0 unx     3265 b- defN 23-Jun-11 13:10 functools/Partial.class
--rw-rw-r--  2.0 unx     2675 b- defN 23-Jun-11 13:10 treelib/Node.class
--rw-rw-r--  2.0 unx     2537 b- defN 23-Jun-11 13:10 treelib/Tree.class
--rw-rw-r--  2.0 unx     1800 b- defN 23-Jun-11 13:10 pandas/NDArrayBackedConstructor.class
--rw-rw-r--  2.0 unx     2394 b- defN 23-Jun-11 13:10 pandas/NDArrayBacked.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-11 13:10 pandas/core/Index$NDArrayData.class
--rw-rw-r--  2.0 unx     3052 b- defN 23-Jun-11 13:10 pandas/core/Index.class
--rw-rw-r--  2.0 unx     4416 b- defN 23-Jun-11 13:10 pandas/core/BlockManager.class
--rw-rw-r--  2.0 unx     1602 b- defN 23-Jun-11 13:10 pandas/core/SingleBlockManager.class
--rw-rw-r--  2.0 unx      724 b- defN 23-Jun-11 13:10 pandas/core/DataFrame.class
--rw-rw-r--  2.0 unx     2419 b- defN 23-Jun-11 13:10 pandas/core/MaskedArray.class
--rw-rw-r--  2.0 unx      565 b- defN 23-Jun-11 13:10 pandas/core/StringDtype.class
--rw-rw-r--  2.0 unx     3212 b- defN 23-Jun-11 13:10 pandas/core/SeriesUtil.class
--rw-rw-r--  2.0 unx     2092 b- defN 23-Jun-11 13:10 pandas/core/Series.class
--rw-rw-r--  2.0 unx     1382 b- defN 23-Jun-11 13:10 pandas/core/Index$RangeData.class
--rw-rw-r--  2.0 unx     1397 b- defN 23-Jun-11 13:10 pandas/core/CategoricalDtype.class
--rw-rw-r--  2.0 unx      385 b- defN 23-Jun-11 13:10 pandas/core/StringArray.class
--rw-rw-r--  2.0 unx      569 b- defN 23-Jun-11 13:10 pandas/core/IntegerDtype.class
--rw-rw-r--  2.0 unx      703 b- defN 23-Jun-11 13:10 pandas/core/Index$Data.class
--rw-rw-r--  2.0 unx      569 b- defN 23-Jun-11 13:10 pandas/core/BooleanDtype.class
--rw-rw-r--  2.0 unx      713 b- defN 23-Jun-11 13:10 pandas/core/Categorical.class
--rw-rw-r--  2.0 unx      994 b- defN 23-Jun-11 13:10 pandas/core/SeriesUtil$1.class
--rw-rw-r--  2.0 unx     1122 b- defN 23-Jun-11 13:10 pandas/core/MaskedArray$1.class
--rw-rw-r--  2.0 unx      453 b- defN 23-Jun-11 13:10 pandas/core/ExtensionDtype.class
--rw-rw-r--  2.0 unx     1354 b- defN 23-Jun-11 13:10 pandas/core/Block.class
--rw-rw-r--  2.0 unx     1172 b- defN 23-Jun-11 13:10 numpy/DTypeUtil.class
--rw-rw-r--  2.0 unx     1404 b- defN 23-Jun-11 13:10 numpy/random/BitGeneratorUtil.class
--rw-rw-r--  2.0 unx     1064 b- defN 23-Jun-11 13:10 numpy/random/Generator.class
--rw-rw-r--  2.0 unx      853 b- defN 23-Jun-11 13:10 numpy/random/BitGenerator.class
--rw-rw-r--  2.0 unx      917 b- defN 23-Jun-11 13:10 numpy/random/RandomState.class
--rw-rw-r--  2.0 unx     1077 b- defN 23-Jun-11 13:10 numpy/random/LegacyRandomState.class
--rw-rw-r--  2.0 unx     4557 b- defN 23-Jun-11 13:10 numpy/DType.class
--rw-rw-r--  2.0 unx     2147 b- defN 23-Jun-11 13:10 numpy/core/TypeDescriptor$Kind.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Jun-11 13:10 numpy/core/MaskedArray.class
--rw-rw-r--  2.0 unx     1100 b- defN 23-Jun-11 13:10 numpy/core/UFunc.class
--rw-rw-r--  2.0 unx    12387 b- defN 23-Jun-11 13:10 numpy/core/NDArrayUtil.class
--rw-rw-r--  2.0 unx      641 b- defN 23-Jun-11 13:10 numpy/core/Function.class
--rw-rw-r--  2.0 unx     2386 b- defN 23-Jun-11 13:10 numpy/core/FromBufferConstructor.class
--rw-rw-r--  2.0 unx     1065 b- defN 23-Jun-11 13:10 numpy/core/TypeDescriptor$1.class
--rw-rw-r--  2.0 unx     4213 b- defN 23-Jun-11 13:10 numpy/core/NDArray.class
--rw-rw-r--  2.0 unx     5262 b- defN 23-Jun-11 13:10 numpy/core/TypeDescriptor.class
--rw-rw-r--  2.0 unx     3638 b- defN 23-Jun-11 13:10 numpy/core/Scalar.class
--rw-rw-r--  2.0 unx      586 b- defN 23-Jun-11 13:10 numpy/core/ScalarUtil.class
--rw-rw-r--  2.0 unx      109 b- defN 23-Jun-11 13:10 collections/Callable.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-11 13:10 collections/DefaultDict.class
--rw-rw-r--  2.0 unx     1467 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$5.class
--rw-rw-r--  2.0 unx     1256 b- defN 23-Jun-11 13:10 org/jpmml/python/Token.class
--rw-rw-r--  2.0 unx     2927 b- defN 23-Jun-11 13:10 org/jpmml/python/TokenMgrException.class
--rw-rw-r--  2.0 unx     2230 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil.class
--rw-rw-r--  2.0 unx     2734 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParserConstants.class
--rw-rw-r--  2.0 unx      472 b- defN 23-Jun-11 13:10 org/jpmml/python/Storage.class
--rw-rw-r--  2.0 unx     1689 b- defN 23-Jun-11 13:10 org/jpmml/python/CustomUnpickler.class
--rw-rw-r--  2.0 unx      497 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser$JJCalls.class
--rw-rw-r--  2.0 unx      914 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$Type$2.class
--rw-rw-r--  2.0 unx     1381 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$1.class
--rw-rw-r--  2.0 unx      242 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$1.class
--rw-rw-r--  2.0 unx     4157 b- defN 23-Jun-11 13:10 org/jpmml/python/ParseException.class
--rw-rw-r--  2.0 unx      282 b- defN 23-Jun-11 13:10 org/jpmml/python/HasArray.class
--rw-rw-r--  2.0 unx     3481 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParserUtil.class
--rw-rw-r--  2.0 unx     2631 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefScope.class
--rw-rw-r--  2.0 unx      784 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     2861 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage.class
--rw-rw-r--  2.0 unx      777 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     1016 b- defN 23-Jun-11 13:10 org/jpmml/python/CastUtil.class
--rw-rw-r--  2.0 unx      164 b- defN 23-Jun-11 13:10 org/jpmml/python/TypeInfo.class
--rw-rw-r--  2.0 unx     5554 b- defN 23-Jun-11 13:10 org/jpmml/python/ClassDictUtil.class
--rw-rw-r--  2.0 unx    39573 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator.class
--rw-rw-r--  2.0 unx     1294 b- defN 23-Jun-11 13:10 org/jpmml/python/StreamProvider.class
--rw-rw-r--  2.0 unx     1340 b- defN 23-Jun-11 13:10 org/jpmml/python/PickleUtil$1.class
--rw-rw-r--  2.0 unx     6658 b- defN 23-Jun-11 13:10 org/jpmml/python/SimpleCharStream.class
--rw-rw-r--  2.0 unx     9499 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser.class
--rw-rw-r--  2.0 unx     1139 b- defN 23-Jun-11 13:10 org/jpmml/python/InputStreamStorage.class
--rw-rw-r--  2.0 unx      986 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$Block.class
--rw-rw-r--  2.0 unx      914 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$Type$1.class
--rw-rw-r--  2.0 unx     4624 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParser.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Jun-11 13:10 org/jpmml/python/NamedTuple.class
--rw-rw-r--  2.0 unx     1303 b- defN 23-Jun-11 13:10 org/jpmml/python/ClassDictUtil$1.class
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-11 13:10 org/jpmml/python/NullConstructor.class
--rw-rw-r--  2.0 unx     1120 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonTypeUtil.class
--rw-rw-r--  2.0 unx     1145 b- defN 23-Jun-11 13:10 org/jpmml/python/FileStorage.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-11 13:10 org/jpmml/python/StringProvider.class
--rw-rw-r--  2.0 unx     1299 b- defN 23-Jun-11 13:10 org/jpmml/python/PushbackPythonParserTokenManager.class
--rw-rw-r--  2.0 unx     9731 b- defN 23-Jun-11 13:10 org/jpmml/python/AbstractTranslator.class
--rw-rw-r--  2.0 unx     8808 b- defN 23-Jun-11 13:10 org/jpmml/python/PickleUtil.class
--rw-rw-r--  2.0 unx     2017 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonEnumConstructor.class
--rw-rw-r--  2.0 unx     4475 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObjectConstructor.class
--rw-rw-r--  2.0 unx      800 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDef$Parameter.class
--rw-rw-r--  2.0 unx      183 b- defN 23-Jun-11 13:10 org/jpmml/python/Identifiable.class
--rw-rw-r--  2.0 unx     2647 b- defN 23-Jun-11 13:10 org/jpmml/python/ClassDictConstructorUtil.class
--rw-rw-r--  2.0 unx    10443 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject.class
--rw-rw-r--  2.0 unx     1442 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$1.class
--rw-rw-r--  2.0 unx    11022 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionUtil.class
--rw-rw-r--  2.0 unx     1456 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$3.class
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator$1.class
--rw-rw-r--  2.0 unx      434 b- defN 23-Jun-11 13:10 org/jpmml/python/IConstantConstructor.class
--rw-rw-r--  2.0 unx     1338 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDef.class
--rw-rw-r--  2.0 unx      270 b- defN 23-Jun-11 13:10 org/jpmml/python/HasContent.class
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser$LookaheadSuccess.class
--rw-rw-r--  2.0 unx     1545 b- defN 23-Jun-11 13:10 org/jpmml/python/CustomPythonObjectConstructor.class
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-11 13:10 org/jpmml/python/CompressedInputStreamStorage$Type.class
--rw-rw-r--  2.0 unx      233 b- defN 23-Jun-11 13:10 org/jpmml/python/FunctionDefParser$1.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Jun-11 13:10 org/jpmml/python/NullProvider.class
--rw-rw-r--  2.0 unx      219 b- defN 23-Jun-11 13:10 org/jpmml/python/Provider.class
--rw-rw-r--  2.0 unx      566 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonEnum.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator$JJCalls.class
--rw-rw-r--  2.0 unx     1201 b- defN 23-Jun-11 13:10 org/jpmml/python/CalendarUtil.class
--rw-rw-r--  2.0 unx     1793 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$2.class
--rw-rw-r--  2.0 unx     2786 b- defN 23-Jun-11 13:10 org/jpmml/python/SliceUtil.class
--rw-rw-r--  2.0 unx      234 b- defN 23-Jun-11 13:10 org/jpmml/python/Castable.class
--rw-rw-r--  2.0 unx     1107 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil$1.class
--rw-rw-r--  2.0 unx     1512 b- defN 23-Jun-11 13:10 org/jpmml/python/AbstractTranslator$1.class
--rw-rw-r--  2.0 unx     1795 b- defN 23-Jun-11 13:10 org/jpmml/python/CastFunction.class
--rw-rw-r--  2.0 unx     1106 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil$3.class
--rw-rw-r--  2.0 unx     1873 b- defN 23-Jun-11 13:10 org/jpmml/python/NamedTupleConstructor.class
--rw-rw-r--  2.0 unx      509 b- defN 23-Jun-11 13:10 org/jpmml/python/ExpressionTranslator$JJCalls.class
--rw-rw-r--  2.0 unx      875 b- defN 23-Jun-11 13:10 org/jpmml/python/SliceUtil$1.class
--rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-11 13:10 org/jpmml/python/BlockScope.class
--rw-rw-r--  2.0 unx     5585 b- defN 23-Jun-11 13:10 org/jpmml/python/DataFrameScope.class
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonEncoder.class
--rw-rw-r--  2.0 unx     1454 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonObject$4.class
--rw-rw-r--  2.0 unx     1729 b- defN 23-Jun-11 13:10 org/jpmml/python/Scope.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jun-11 13:10 org/jpmml/python/TupleUtil$2.class
--rw-rw-r--  2.0 unx    15414 b- defN 23-Jun-11 13:10 org/jpmml/python/PythonParserTokenManager.class
--rw-rw-r--  2.0 unx     3168 b- defN 23-Jun-11 13:10 org/jpmml/python/CustomPythonObject.class
--rw-rw-r--  2.0 unx    23578 b- defN 23-Jun-11 13:10 org/jpmml/python/PredicateTranslator.class
--rw-rw-r--  2.0 unx     1629 b- defN 23-Jun-11 13:10 org/jpmml/python/StorageUtil.class
--rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-11 13:10 joblib/NDArrayWrapperConstructor$1.class
--rw-rw-r--  2.0 unx     1371 b- defN 23-Jun-11 13:10 joblib/NDArrayWrapperConstructor.class
--rw-rw-r--  2.0 unx     2667 b- defN 23-Jun-11 13:10 joblib/NumpyArrayWrapper.class
--rw-rw-r--  2.0 unx     2493 b- defN 23-Jun-11 13:10 joblib/NDArrayWrapper.class
--rw-rw-r--  2.0 unx      388 b- defN 23-Jun-11 13:10 scipy/stats/RVGeneric.class
--rw-rw-r--  2.0 unx      559 b- defN 23-Jun-11 13:10 scipy/stats/RVContinuous.class
--rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-11 13:10 scipy/interpolate/BSpline.class
--rw-rw-r--  2.0 unx     1541 b- defN 23-Jun-11 13:10 scipy/sparse/CSRMatrix.class
--rw-rw-r--  2.0 unx     2618 b- defN 23-Jun-11 13:10 scipy/sparse/CSRMatrixUtil.class
--rw-rw-r--  2.0 unx     2086 b- defN 23-Jun-11 13:10 builtins/Type.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-11 13:10 builtins/GetAttr.class
--rw-rw-r--  2.0 unx      536 b- defN 23-Jun-11 13:10 builtins/TypeConstructor.class
--rw-rw-r--  2.0 unx      637 b- defN 23-Jun-11 13:10 builtins/Function.class
--rw-rw-r--  2.0 unx      855 b- defN 23-Jun-11 13:10 builtins/Slice.class
--rw-rw-r--  2.0 unx     5158 b- defN 23-Jun-11 13:10 META-INF/maven/org.jpmml/pmml-python/pom.xml
--rw-rw-r--  2.0 unx       56 b- defN 23-Jun-11 13:10 META-INF/maven/org.jpmml/pmml-python/pom.properties
-172 files, 378890 bytes uncompressed, 178291 bytes compressed:  52.9%
+Zip file size: 203268 bytes, number of entries: 174
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-13 20:26 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 patsy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 functools/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 treelib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 pandas/core/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 dill/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 numpy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 numpy/random/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 numpy/core/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 collections/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 org/jpmml/python/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 joblib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 scipy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 scipy/stats/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 scipy/interpolate/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 scipy/sparse/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 builtins/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-13 20:26 META-INF/maven/org.jpmml/pmml-python/
+-rw-rw-r--  2.0 unx     2108 b- defN 23-Jul-13 20:26 patsy/PatsyOperation.class
+-rw-rw-r--  2.0 unx     2272 b- defN 23-Jul-13 20:26 patsy/PatsyOperator.class
+-rw-rw-r--  2.0 unx     3106 b- defN 23-Jul-13 20:26 patsy/PatsyToken.class
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jul-13 20:26 patsy/PatsyFactor.class
+-rw-rw-r--  2.0 unx      747 b- defN 23-Jul-13 20:26 patsy/PatsyTerm.class
+-rw-rw-r--  2.0 unx     8491 b- defN 23-Jul-13 20:26 patsy/FormulaParser.class
+-rw-rw-r--  2.0 unx     3169 b- defN 23-Jul-13 20:26 META-INF/python2pmml.properties
+-rw-rw-r--  2.0 unx     3265 b- defN 23-Jul-13 20:26 functools/Partial.class
+-rw-rw-r--  2.0 unx     2675 b- defN 23-Jul-13 20:26 treelib/Node.class
+-rw-rw-r--  2.0 unx     2537 b- defN 23-Jul-13 20:26 treelib/Tree.class
+-rw-rw-r--  2.0 unx     1800 b- defN 23-Jul-13 20:26 pandas/NDArrayBackedConstructor.class
+-rw-rw-r--  2.0 unx     2394 b- defN 23-Jul-13 20:26 pandas/NDArrayBacked.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-13 20:26 pandas/core/Index$NDArrayData.class
+-rw-rw-r--  2.0 unx     3052 b- defN 23-Jul-13 20:26 pandas/core/Index.class
+-rw-rw-r--  2.0 unx     4416 b- defN 23-Jul-13 20:26 pandas/core/BlockManager.class
+-rw-rw-r--  2.0 unx     1602 b- defN 23-Jul-13 20:26 pandas/core/SingleBlockManager.class
+-rw-rw-r--  2.0 unx      724 b- defN 23-Jul-13 20:26 pandas/core/DataFrame.class
+-rw-rw-r--  2.0 unx     2419 b- defN 23-Jul-13 20:26 pandas/core/MaskedArray.class
+-rw-rw-r--  2.0 unx      565 b- defN 23-Jul-13 20:26 pandas/core/StringDtype.class
+-rw-rw-r--  2.0 unx     3212 b- defN 23-Jul-13 20:26 pandas/core/SeriesUtil.class
+-rw-rw-r--  2.0 unx     2092 b- defN 23-Jul-13 20:26 pandas/core/Series.class
+-rw-rw-r--  2.0 unx     1382 b- defN 23-Jul-13 20:26 pandas/core/Index$RangeData.class
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Jul-13 20:26 pandas/core/CategoricalDtype.class
+-rw-rw-r--  2.0 unx      385 b- defN 23-Jul-13 20:26 pandas/core/StringArray.class
+-rw-rw-r--  2.0 unx      569 b- defN 23-Jul-13 20:26 pandas/core/IntegerDtype.class
+-rw-rw-r--  2.0 unx      703 b- defN 23-Jul-13 20:26 pandas/core/Index$Data.class
+-rw-rw-r--  2.0 unx      569 b- defN 23-Jul-13 20:26 pandas/core/BooleanDtype.class
+-rw-rw-r--  2.0 unx      713 b- defN 23-Jul-13 20:26 pandas/core/Categorical.class
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jul-13 20:26 pandas/core/SeriesUtil$1.class
+-rw-rw-r--  2.0 unx     1122 b- defN 23-Jul-13 20:26 pandas/core/MaskedArray$1.class
+-rw-rw-r--  2.0 unx      453 b- defN 23-Jul-13 20:26 pandas/core/ExtensionDtype.class
+-rw-rw-r--  2.0 unx     1354 b- defN 23-Jul-13 20:26 pandas/core/Block.class
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-13 20:26 dill/CreateArrayConstructor.class
+-rw-rw-r--  2.0 unx     1172 b- defN 23-Jul-13 20:26 numpy/DTypeUtil.class
+-rw-rw-r--  2.0 unx     1404 b- defN 23-Jul-13 20:26 numpy/random/BitGeneratorUtil.class
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Jul-13 20:26 numpy/random/Generator.class
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jul-13 20:26 numpy/random/BitGenerator.class
+-rw-rw-r--  2.0 unx      917 b- defN 23-Jul-13 20:26 numpy/random/RandomState.class
+-rw-rw-r--  2.0 unx     1077 b- defN 23-Jul-13 20:26 numpy/random/LegacyRandomState.class
+-rw-rw-r--  2.0 unx     4557 b- defN 23-Jul-13 20:26 numpy/DType.class
+-rw-rw-r--  2.0 unx     2147 b- defN 23-Jul-13 20:26 numpy/core/TypeDescriptor$Kind.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jul-13 20:26 numpy/core/MaskedArray.class
+-rw-rw-r--  2.0 unx     1100 b- defN 23-Jul-13 20:26 numpy/core/UFunc.class
+-rw-rw-r--  2.0 unx    12387 b- defN 23-Jul-13 20:26 numpy/core/NDArrayUtil.class
+-rw-rw-r--  2.0 unx      641 b- defN 23-Jul-13 20:26 numpy/core/Function.class
+-rw-rw-r--  2.0 unx     2386 b- defN 23-Jul-13 20:26 numpy/core/FromBufferConstructor.class
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Jul-13 20:26 numpy/core/TypeDescriptor$1.class
+-rw-rw-r--  2.0 unx     4213 b- defN 23-Jul-13 20:26 numpy/core/NDArray.class
+-rw-rw-r--  2.0 unx     5262 b- defN 23-Jul-13 20:26 numpy/core/TypeDescriptor.class
+-rw-rw-r--  2.0 unx     3638 b- defN 23-Jul-13 20:26 numpy/core/Scalar.class
+-rw-rw-r--  2.0 unx      586 b- defN 23-Jul-13 20:26 numpy/core/ScalarUtil.class
+-rw-rw-r--  2.0 unx      109 b- defN 23-Jul-13 20:26 collections/Callable.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jul-13 20:26 collections/DefaultDict.class
+-rw-rw-r--  2.0 unx     1467 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObject$5.class
+-rw-rw-r--  2.0 unx     1256 b- defN 23-Jul-13 20:26 org/jpmml/python/Token.class
+-rw-rw-r--  2.0 unx     2927 b- defN 23-Jul-13 20:26 org/jpmml/python/TokenMgrException.class
+-rw-rw-r--  2.0 unx     2230 b- defN 23-Jul-13 20:26 org/jpmml/python/TupleUtil.class
+-rw-rw-r--  2.0 unx     2734 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonParserConstants.class
+-rw-rw-r--  2.0 unx      472 b- defN 23-Jul-13 20:26 org/jpmml/python/Storage.class
+-rw-rw-r--  2.0 unx     1689 b- defN 23-Jul-13 20:26 org/jpmml/python/CustomUnpickler.class
+-rw-rw-r--  2.0 unx      497 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDefParser$JJCalls.class
+-rw-rw-r--  2.0 unx      914 b- defN 23-Jul-13 20:26 org/jpmml/python/CompressedInputStreamStorage$Type$2.class
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Jul-13 20:26 org/jpmml/python/CompressedInputStreamStorage$1.class
+-rw-rw-r--  2.0 unx      242 b- defN 23-Jul-13 20:26 org/jpmml/python/ExpressionTranslator$1.class
+-rw-rw-r--  2.0 unx     4157 b- defN 23-Jul-13 20:26 org/jpmml/python/ParseException.class
+-rw-rw-r--  2.0 unx      282 b- defN 23-Jul-13 20:26 org/jpmml/python/HasArray.class
+-rw-rw-r--  2.0 unx     3481 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonParserUtil.class
+-rw-rw-r--  2.0 unx     2631 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDefScope.class
+-rw-rw-r--  2.0 unx      784 b- defN 23-Jul-13 20:26 org/jpmml/python/ExpressionTranslator$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     2861 b- defN 23-Jul-13 20:26 org/jpmml/python/CompressedInputStreamStorage.class
+-rw-rw-r--  2.0 unx      777 b- defN 23-Jul-13 20:26 org/jpmml/python/PredicateTranslator$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     1016 b- defN 23-Jul-13 20:26 org/jpmml/python/CastUtil.class
+-rw-rw-r--  2.0 unx      164 b- defN 23-Jul-13 20:26 org/jpmml/python/TypeInfo.class
+-rw-rw-r--  2.0 unx     5554 b- defN 23-Jul-13 20:26 org/jpmml/python/ClassDictUtil.class
+-rw-rw-r--  2.0 unx    39573 b- defN 23-Jul-13 20:26 org/jpmml/python/ExpressionTranslator.class
+-rw-rw-r--  2.0 unx     1294 b- defN 23-Jul-13 20:26 org/jpmml/python/StreamProvider.class
+-rw-rw-r--  2.0 unx     1340 b- defN 23-Jul-13 20:26 org/jpmml/python/PickleUtil$1.class
+-rw-rw-r--  2.0 unx     6658 b- defN 23-Jul-13 20:26 org/jpmml/python/SimpleCharStream.class
+-rw-rw-r--  2.0 unx     9499 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDefParser.class
+-rw-rw-r--  2.0 unx     1139 b- defN 23-Jul-13 20:26 org/jpmml/python/InputStreamStorage.class
+-rw-rw-r--  2.0 unx      986 b- defN 23-Jul-13 20:26 org/jpmml/python/ExpressionTranslator$Block.class
+-rw-rw-r--  2.0 unx      914 b- defN 23-Jul-13 20:26 org/jpmml/python/CompressedInputStreamStorage$Type$1.class
+-rw-rw-r--  2.0 unx     4624 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonParser.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jul-13 20:26 org/jpmml/python/NamedTuple.class
+-rw-rw-r--  2.0 unx     1303 b- defN 23-Jul-13 20:26 org/jpmml/python/ClassDictUtil$1.class
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jul-13 20:26 org/jpmml/python/NullConstructor.class
+-rw-rw-r--  2.0 unx     1120 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonTypeUtil.class
+-rw-rw-r--  2.0 unx     1145 b- defN 23-Jul-13 20:26 org/jpmml/python/FileStorage.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-13 20:26 org/jpmml/python/StringProvider.class
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Jul-13 20:26 org/jpmml/python/PushbackPythonParserTokenManager.class
+-rw-rw-r--  2.0 unx     9731 b- defN 23-Jul-13 20:26 org/jpmml/python/AbstractTranslator.class
+-rw-rw-r--  2.0 unx     8911 b- defN 23-Jul-13 20:26 org/jpmml/python/PickleUtil.class
+-rw-rw-r--  2.0 unx     2017 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonEnumConstructor.class
+-rw-rw-r--  2.0 unx     4475 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObjectConstructor.class
+-rw-rw-r--  2.0 unx      800 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDef$Parameter.class
+-rw-rw-r--  2.0 unx      183 b- defN 23-Jul-13 20:26 org/jpmml/python/Identifiable.class
+-rw-rw-r--  2.0 unx     2647 b- defN 23-Jul-13 20:26 org/jpmml/python/ClassDictConstructorUtil.class
+-rw-rw-r--  2.0 unx    10443 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObject.class
+-rw-rw-r--  2.0 unx     1442 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObject$1.class
+-rw-rw-r--  2.0 unx    11022 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionUtil.class
+-rw-rw-r--  2.0 unx     1456 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObject$3.class
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jul-13 20:26 org/jpmml/python/PredicateTranslator$1.class
+-rw-rw-r--  2.0 unx      434 b- defN 23-Jul-13 20:26 org/jpmml/python/IConstantConstructor.class
+-rw-rw-r--  2.0 unx     1338 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDef.class
+-rw-rw-r--  2.0 unx      270 b- defN 23-Jul-13 20:26 org/jpmml/python/HasContent.class
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDefParser$LookaheadSuccess.class
+-rw-rw-r--  2.0 unx     1545 b- defN 23-Jul-13 20:26 org/jpmml/python/CustomPythonObjectConstructor.class
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-13 20:26 org/jpmml/python/CompressedInputStreamStorage$Type.class
+-rw-rw-r--  2.0 unx      233 b- defN 23-Jul-13 20:26 org/jpmml/python/FunctionDefParser$1.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Jul-13 20:26 org/jpmml/python/NullProvider.class
+-rw-rw-r--  2.0 unx      219 b- defN 23-Jul-13 20:26 org/jpmml/python/Provider.class
+-rw-rw-r--  2.0 unx      566 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonEnum.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jul-13 20:26 org/jpmml/python/PredicateTranslator$JJCalls.class
+-rw-rw-r--  2.0 unx     1201 b- defN 23-Jul-13 20:26 org/jpmml/python/CalendarUtil.class
+-rw-rw-r--  2.0 unx     1793 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObject$2.class
+-rw-rw-r--  2.0 unx     2786 b- defN 23-Jul-13 20:26 org/jpmml/python/SliceUtil.class
+-rw-rw-r--  2.0 unx      234 b- defN 23-Jul-13 20:26 org/jpmml/python/Castable.class
+-rw-rw-r--  2.0 unx     1107 b- defN 23-Jul-13 20:26 org/jpmml/python/TupleUtil$1.class
+-rw-rw-r--  2.0 unx     1512 b- defN 23-Jul-13 20:26 org/jpmml/python/AbstractTranslator$1.class
+-rw-rw-r--  2.0 unx     1795 b- defN 23-Jul-13 20:26 org/jpmml/python/CastFunction.class
+-rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-13 20:26 org/jpmml/python/TupleUtil$3.class
+-rw-rw-r--  2.0 unx     1873 b- defN 23-Jul-13 20:26 org/jpmml/python/NamedTupleConstructor.class
+-rw-rw-r--  2.0 unx      509 b- defN 23-Jul-13 20:26 org/jpmml/python/ExpressionTranslator$JJCalls.class
+-rw-rw-r--  2.0 unx      875 b- defN 23-Jul-13 20:26 org/jpmml/python/SliceUtil$1.class
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jul-13 20:26 org/jpmml/python/BlockScope.class
+-rw-rw-r--  2.0 unx     5585 b- defN 23-Jul-13 20:26 org/jpmml/python/DataFrameScope.class
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonEncoder.class
+-rw-rw-r--  2.0 unx     1454 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonObject$4.class
+-rw-rw-r--  2.0 unx     1729 b- defN 23-Jul-13 20:26 org/jpmml/python/Scope.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jul-13 20:26 org/jpmml/python/TupleUtil$2.class
+-rw-rw-r--  2.0 unx    15414 b- defN 23-Jul-13 20:26 org/jpmml/python/PythonParserTokenManager.class
+-rw-rw-r--  2.0 unx     3168 b- defN 23-Jul-13 20:26 org/jpmml/python/CustomPythonObject.class
+-rw-rw-r--  2.0 unx    23578 b- defN 23-Jul-13 20:26 org/jpmml/python/PredicateTranslator.class
+-rw-rw-r--  2.0 unx     1629 b- defN 23-Jul-13 20:26 org/jpmml/python/StorageUtil.class
+-rw-rw-r--  2.0 unx     1128 b- defN 23-Jul-13 20:26 joblib/NDArrayWrapperConstructor$1.class
+-rw-rw-r--  2.0 unx     1371 b- defN 23-Jul-13 20:26 joblib/NDArrayWrapperConstructor.class
+-rw-rw-r--  2.0 unx     2667 b- defN 23-Jul-13 20:26 joblib/NumpyArrayWrapper.class
+-rw-rw-r--  2.0 unx     2493 b- defN 23-Jul-13 20:26 joblib/NDArrayWrapper.class
+-rw-rw-r--  2.0 unx      388 b- defN 23-Jul-13 20:26 scipy/stats/RVGeneric.class
+-rw-rw-r--  2.0 unx      559 b- defN 23-Jul-13 20:26 scipy/stats/RVContinuous.class
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jul-13 20:26 scipy/interpolate/BSpline.class
+-rw-rw-r--  2.0 unx     1541 b- defN 23-Jul-13 20:26 scipy/sparse/CSRMatrix.class
+-rw-rw-r--  2.0 unx     2618 b- defN 23-Jul-13 20:26 scipy/sparse/CSRMatrixUtil.class
+-rw-rw-r--  2.0 unx     2086 b- defN 23-Jul-13 20:26 builtins/Type.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Jul-13 20:26 builtins/GetAttr.class
+-rw-rw-r--  2.0 unx      536 b- defN 23-Jul-13 20:26 builtins/TypeConstructor.class
+-rw-rw-r--  2.0 unx      637 b- defN 23-Jul-13 20:26 builtins/Function.class
+-rw-rw-r--  2.0 unx      855 b- defN 23-Jul-13 20:26 builtins/Slice.class
+-rw-rw-r--  2.0 unx     5158 b- defN 23-Jul-13 20:25 META-INF/maven/org.jpmml/pmml-python/pom.xml
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jul-13 20:26 META-INF/maven/org.jpmml/pmml-python/pom.properties
+174 files, 380578 bytes uncompressed, 179004 bytes compressed:  53.0%
```

#### zipnote «TEMP»/diffoscope_fr7ro12l_/tmp2499ha2r_.zip

```diff
@@ -15,14 +15,17 @@
 
 Filename: pandas/
 Comment: 
 
 Filename: pandas/core/
 Comment: 
 
+Filename: dill/
+Comment: 
+
 Filename: numpy/
 Comment: 
 
 Filename: numpy/random/
 Comment: 
 
 Filename: numpy/core/
@@ -159,14 +162,17 @@
 
 Filename: pandas/core/ExtensionDtype.class
 Comment: 
 
 Filename: pandas/core/Block.class
 Comment: 
 
+Filename: dill/CreateArrayConstructor.class
+Comment: 
+
 Filename: numpy/DTypeUtil.class
 Comment: 
 
 Filename: numpy/random/BitGeneratorUtil.class
 Comment: 
 
 Filename: numpy/random/Generator.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-Python library
-Implementation-Version: 1.1.15
+Implementation-Version: 1.1.16
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/python2pmml.properties

```diff
@@ -1,11 +1,12 @@
 builtins.getattr = builtins.GetAttr
 builtins.slice = builtins.Slice
 builtins.(bool|float|int|str) = builtins.TypeConstructor
 collections.defaultdict = collections.DefaultDict
+dill._dill._create_array = dill.CreateArrayConstructor
 functools.partial = functools.Partial
 joblib.numpy_pickle.NumpyArrayWrapper = joblib.NumpyArrayWrapper
 math.(acos|asin|atan|atan2|ceil|copysign|cos|cosh|degrees|exp|expm1|fabs|floor|hypot|isnan|log|log1p|log10|pow|radians|sin|sinh|sqrt|tan|tanh|trunc) = builtins.Function
 numpy.(|core.fromnumeric.)clip = numpy.core.Function
 numpy.(|core._multiarray_umath.)(absolute|arccos|arcsin|arctan|arctan2|ceil|clip|cos|cosh|degrees|rad2deg|exp|expm1|floor|fmax|fmin|hypot|log|log1p|log10|negative|power|radians|deg2rad|reciprocal|rint|sign|sin|sinh|sqrt|square|tan|tanh) = numpy.core.Function
 numpy.(bool_|float_|float32|float64|int_|int8|int16|int32|int64|str_|uint8|uint16|uint32|uint64) = builtins.TypeConstructor
 numpy.core.(_multiarray_umath|multiarray)._reconstruct = numpy.core.NDArray
```

#### org/jpmml/python/PickleUtil$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 2f787e11570d78a2e4df5b226b618fc7f33cae7838a4c233f75a7e6aa21f0e9c
+  SHA-256 checksum 34e7a07a065718bd1736aea95327821746b5e069c038eb1661fbfd6bd0bbc4c6
   Compiled from "PickleUtil.java"
 final class org.jpmml.python.PickleUtil$1 extends org.jpmml.python.CustomUnpickler
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #11                         // org/jpmml/python/PickleUtil$1
   super_class: #12                        // org/jpmml/python/CustomUnpickler
@@ -92,15 +92,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field val$is:Ljava/io/InputStream;
          5: aload_0
          6: invokespecial #2                  // Method org/jpmml/python/CustomUnpickler."<init>":()V
          9: return
       LineNumberTable:
-        line 60: 0
+        line 61: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lorg/jpmml/python/PickleUtil$1;
 
   protected java.lang.Object dispatch(short) throws java.io.IOException;
     descriptor: (S)Ljava/lang/Object;
     flags: (0x0004) ACC_PROTECTED
@@ -135,23 +135,23 @@
         52: aload_0
         53: getfield      #5                  // Field org/jpmml/python/CustomUnpickler.stack:Lnet/razorvine/pickle/UnpickleStack;
         56: aload         5
         58: invokevirtual #10                 // Method net/razorvine/pickle/UnpickleStack.add:(Ljava/lang/Object;)V
         61: aload_2
         62: areturn
       LineNumberTable:
-        line 64: 0
-        line 66: 6
-        line 67: 12
-        line 70: 20
-        line 71: 27
-        line 73: 33
-        line 75: 41
-        line 77: 52
-        line 81: 61
+        line 65: 0
+        line 67: 6
+        line 68: 12
+        line 71: 20
+        line 72: 27
+        line 74: 33
+        line 76: 41
+        line 78: 52
+        line 82: 61
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            33      28     4 arrayWrapper   Ljoblib/NumpyArrayWrapper;
            52       9     5 array   Lnumpy/core/NDArray;
            20      41     3  head   Ljava/lang/Object;
             0      63     0  this   Lorg/jpmml/python/PickleUtil$1;
             0      63     1   key   S
```

#### org/jpmml/python/PickleUtil.class

##### procyon -ec {}

```diff
@@ -4,14 +4,15 @@
 import org.slf4j.LoggerFactory;
 import java.util.List;
 import java.util.ArrayList;
 import java.util.Collections;
 import java.lang.reflect.Constructor;
 import pandas.NDArrayBackedConstructor;
 import pandas.NDArrayBacked;
+import net.razorvine.pickle.objects.ClassDictConstructor;
 import java.util.Collection;
 import java.util.Iterator;
 import java.util.Set;
 import java.util.Enumeration;
 import java.util.Properties;
 import java.net.URL;
 import java.io.IOException;
@@ -114,50 +115,50 @@
         try {
             clazz = classLoader.loadClass(value);
         }
         catch (final ClassNotFoundException cnfe) {
             PickleUtil.logger.warn("Failed to load Java class {}", (Object)value);
             return;
         }
-        PythonObjectConstructor dictConstructor = null;
+        ClassDictConstructor dictConstructor = null;
         Label_0341: {
             if (!PythonObject.class.isAssignableFrom(clazz)) {
-                if (PythonObjectConstructor.class.isAssignableFrom(clazz)) {
+                if (ClassDictConstructor.class.isAssignableFrom(clazz)) {
                     try {
                         final Constructor<?> constructor = clazz.getDeclaredConstructor(String.class, String.class);
-                        dictConstructor = (PythonObjectConstructor)constructor.newInstance(module, name);
+                        dictConstructor = (ClassDictConstructor)constructor.newInstance(module, name);
                         break Label_0341;
                     }
                     catch (final ReflectiveOperationException roe) {
                         PickleUtil.logger.warn("Failed to instantiate Java constructor", (Throwable)roe);
                         return;
                     }
                 }
                 PickleUtil.logger.warn("Failed to identify the type of Java class {}", (Object)value);
                 return;
             }
             if (CustomPythonObject.class.isAssignableFrom(clazz)) {
                 if (NDArrayBacked.class.isAssignableFrom(clazz)) {
-                    dictConstructor = (PythonObjectConstructor)new NDArrayBackedConstructor(module, name, (Class)clazz.asSubclass(NDArrayBacked.class));
+                    dictConstructor = (ClassDictConstructor)new NDArrayBackedConstructor(module, name, (Class)clazz.asSubclass(NDArrayBacked.class));
                 }
                 else {
-                    dictConstructor = (PythonObjectConstructor)new CustomPythonObjectConstructor(module, name, (Class)clazz.asSubclass(CustomPythonObject.class));
+                    dictConstructor = (ClassDictConstructor)new CustomPythonObjectConstructor(module, name, (Class)clazz.asSubclass(CustomPythonObject.class));
                 }
             }
             else if (NamedTuple.class.isAssignableFrom(clazz)) {
-                dictConstructor = (PythonObjectConstructor)new NamedTupleConstructor(module, name, (Class)clazz.asSubclass(NamedTuple.class));
+                dictConstructor = (ClassDictConstructor)new NamedTupleConstructor(module, name, (Class)clazz.asSubclass(NamedTuple.class));
             }
             else if (PythonEnum.class.isAssignableFrom(clazz)) {
-                dictConstructor = (PythonObjectConstructor)new PythonEnumConstructor(module, name, (Class)clazz.asSubclass(PythonEnum.class));
+                dictConstructor = (ClassDictConstructor)new PythonEnumConstructor(module, name, (Class)clazz.asSubclass(PythonEnum.class));
             }
             else {
-                dictConstructor = new PythonObjectConstructor(module, name, (Class)clazz.asSubclass(PythonObject.class));
+                dictConstructor = (ClassDictConstructor)new PythonObjectConstructor(module, name, (Class)clazz.asSubclass(PythonObject.class));
             }
         }
-        Unpickler.registerConstructor(dictConstructor.getModule(), dictConstructor.getName(), (IObjectConstructor)dictConstructor);
+        Unpickler.registerConstructor(module, name, (IObjectConstructor)dictConstructor);
     }
     
     private static Collection<String> expandComplexKey(final String key) {
         final int begin = key.indexOf(40);
         final int end = key.indexOf(41, begin + 1);
         if (begin < 0 || end < 0) {
             return Collections.singletonList(key);
```

#### META-INF/maven/org.jpmml/pmml-python/pom.xml

##### META-INF/maven/org.jpmml/pmml-python/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-python</artifactId>
-    <version>1.1.15</version>
+    <version>1.1.16</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-python</artifactId>
   <packaging>jar</packaging>
   <name>JPMML Python converter</name>
   <description>JPMML Python to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-python/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-python
 groupId=org.jpmml
-version=1.1.15
+version=1.1.16
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.31.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.32.jar`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 7976 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Jul-08 09:03 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-Jul-08 09:03 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Jul-08 09:03 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-Jul-08 09:03 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-Jul-08 09:03 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-14 18:18 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Jul-14 18:18 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jul-14 18:18 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2270 b- defN 23-Jul-14 18:18 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Jul-14 18:18 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2246 b- defN 23-Jul-14 18:18 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Jul-14 18:18 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-14 18:17 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
 15 files, 13161 bytes uncompressed, 5920 bytes compressed:  55.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.31</version>
+    <version>1.7.32</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Jul 08 09:03:24 EEST 2023
-version=1.7.31
+#Fri Jul 14 18:18:07 EEST 2023
+version=1.7.32
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.31.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.32.jar`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 6242 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/statsmodels/
--rw-rw-r--  2.0 unx      152 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsClassifier.class
--rw-rw-r--  2.0 unx     1920 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsUtil.class
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-08 09:03 sklearn2pmml/statsmodels/StatsModelsRegressor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
--rw-rw-r--  2.0 unx     1331 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
--rw-rw-r--  2.0 unx      120 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
-14 files, 8762 bytes uncompressed, 4120 bytes compressed:  53.0%
+Zip file size: 6244 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-14 18:18 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/statsmodels/
+-rw-rw-r--  2.0 unx      152 b- defN 23-Jul-14 18:18 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-14 18:18 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-14 18:18 sklearn2pmml/statsmodels/StatsModelsClassifier.class
+-rw-rw-r--  2.0 unx     1920 b- defN 23-Jul-14 18:18 sklearn2pmml/statsmodels/StatsModelsUtil.class
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-14 18:18 sklearn2pmml/statsmodels/StatsModelsRegressor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
+-rw-rw-r--  2.0 unx     1331 b- defN 23-Jul-14 18:17 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx      120 b- defN 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
+14 files, 8762 bytes uncompressed, 4122 bytes compressed:  53.0%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.31</version>
+    <version>1.7.32</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn StatsModels converter</name>
   <description>JPMML Scikit-Learn StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Jul 08 09:03:24 EEST 2023
-version=1.7.31
+#Fri Jul 14 18:18:07 EEST 2023
+version=1.7.32
 groupId=org.jpmml
 artifactId=pmml-sklearn-statsmodels
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-1.7.31.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-1.7.32.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,407 +1,407 @@
 Zip file size: 472037 bytes, number of entries: 405
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Jul-08 09:03 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Jul-08 09:03 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Jul-08 09:03 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Jul-08 09:03 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Jul-08 09:03 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Jul-08 09:03 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-08 09:03 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Jul-08 09:03 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Jul-08 09:03 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Jul-08 09:03 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jul-08 09:03 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Jul-08 09:03 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-Jul-08 09:03 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Jul-08 09:03 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    12048 b- defN 23-Jul-08 09:03 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2953 b- defN 23-Jul-08 09:03 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Jul-08 09:03 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     3672 b- defN 23-Jul-08 09:03 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1671 b- defN 23-Jul-08 09:03 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-08 09:03 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5062 b- defN 23-Jul-08 09:03 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2003 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-08 09:03 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2298 b- defN 23-Jul-08 09:03 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     4913 b- defN 23-Jul-08 09:03 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2055 b- defN 23-Jul-08 09:03 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      454 b- defN 23-Jul-08 09:03 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Jul-08 09:03 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Jul-08 09:03 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     3421 b- defN 23-Jul-08 09:03 sklearn/OutlierDetectorUtil.class
--rw-rw-r--  2.0 unx     1236 b- defN 23-Jul-08 09:03 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Jul-08 09:03 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Jul-08 09:03 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Jul-08 09:03 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Jul-08 09:03 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-08 09:03 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-Jul-08 09:03 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     4114 b- defN 23-Jul-08 09:03 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Jul-08 09:03 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      342 b- defN 23-Jul-08 09:03 sklearn/HasOutlierField.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Jul-08 09:03 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-Jul-08 09:03 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-Jul-08 09:03 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2555 b- defN 23-Jul-08 09:03 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Jul-08 09:03 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx    10661 b- defN 23-Jul-08 09:03 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx      853 b- defN 23-Jul-08 09:03 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Jul-08 09:03 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-Jul-08 09:03 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Jul-08 09:03 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-Jul-08 09:03 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     6948 b- defN 23-Jul-08 09:03 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx     4434 b- defN 23-Jul-08 09:03 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     5040 b- defN 23-Jul-08 09:03 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7648 b- defN 23-Jul-08 09:03 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Jul-08 09:03 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jul-08 09:03 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-08 09:03 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      932 b- defN 23-Jul-08 09:03 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-08 09:03 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-Jul-08 09:03 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-Jul-08 09:03 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-08 09:03 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx      894 b- defN 23-Jul-08 09:03 sklearn/IdentityTransformer.class
--rw-rw-r--  2.0 unx     4089 b- defN 23-Jul-08 09:03 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Jul-08 09:03 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-Jul-08 09:03 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Jul-08 09:03 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Jul-08 09:03 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Jul-08 09:03 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Jul-08 09:03 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Jul-08 09:03 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-Jul-08 09:03 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-Jul-08 09:03 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2025 b- defN 23-Jul-08 09:03 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jul-08 09:03 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10733 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-08 09:03 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-Jul-08 09:03 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Jul-08 09:03 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Jul-08 09:03 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2654 b- defN 23-Jul-08 09:03 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3510 b- defN 23-Jul-08 09:03 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-08 09:03 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-Jul-08 09:03 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-Jul-08 09:03 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-Jul-08 09:03 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4450 b- defN 23-Jul-08 09:03 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Jul-08 09:03 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jul-08 09:03 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     1929 b- defN 23-Jul-08 09:03 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Jul-08 09:03 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      451 b- defN 23-Jul-08 09:03 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Jul-08 09:03 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4031 b- defN 23-Jul-08 09:03 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-Jul-08 09:03 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1375 b- defN 23-Jul-08 09:03 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Jul-08 09:03 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Jul-08 09:03 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3031 b- defN 23-Jul-08 09:03 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3862 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Jul-08 09:03 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7948 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Jul-08 09:03 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Jul-08 09:03 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2528 b- defN 23-Jul-08 09:03 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     2987 b- defN 23-Jul-08 09:03 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8225 b- defN 23-Jul-08 09:03 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-08 09:03 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-Jul-08 09:03 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6377 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Jul-08 09:03 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-08 09:03 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Jul-08 09:03 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     6043 b- defN 23-Jul-08 09:03 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Jul-08 09:03 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-Jul-08 09:03 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-08 09:03 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-Jul-08 09:03 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-Jul-08 09:03 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-08 09:03 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Jul-08 09:03 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Jul-08 09:03 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Jul-08 09:03 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Jul-08 09:03 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Jul-08 09:03 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Jul-08 09:03 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Jul-08 09:03 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Jul-08 09:03 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     5114 b- defN 23-Jul-08 09:03 sklearn/ScalarLabelUtil.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-08 09:03 sklearn/OutlierDetectorUtil$1.class
--rw-rw-r--  2.0 unx      195 b- defN 23-Jul-08 09:03 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4685 b- defN 23-Jul-08 09:03 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-Jul-08 09:03 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-Jul-08 09:03 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-08 09:03 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-Jul-08 09:03 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-Jul-08 09:03 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-Jul-08 09:03 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-Jul-08 09:03 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Jul-08 09:03 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-Jul-08 09:03 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-Jul-08 09:03 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Jul-08 09:03 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     6971 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-Jul-08 09:03 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-Jul-08 09:03 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-Jul-08 09:03 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-Jul-08 09:03 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-08 09:03 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Jul-08 09:03 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Jul-08 09:03 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Jul-08 09:03 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Jul-08 09:03 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Jul-08 09:03 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx     7408 b- defN 23-Jul-08 09:03 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2153 b- defN 23-Jul-08 09:03 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Jul-08 09:03 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx      879 b- defN 23-Jul-08 09:03 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx      978 b- defN 23-Jul-08 09:03 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-Jul-08 09:03 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    19425 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-08 09:03 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2257 b- defN 23-Jul-08 09:03 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Jul-08 09:03 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Jul-08 09:03 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Jul-08 09:03 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-Jul-08 09:03 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Jul-08 09:03 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Jul-08 09:03 sklearn/OutlierDetector.class
--rw-rw-r--  2.0 unx     2808 b- defN 23-Jul-08 09:03 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Jul-08 09:03 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     7080 b- defN 23-Jul-08 09:03 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Jul-08 09:03 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Jul-08 09:03 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-Jul-08 09:03 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx    14030 b- defN 23-Jul-08 09:03 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-Jul-08 09:03 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4598 b- defN 23-Jul-08 09:03 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Jul-08 09:03 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$4.class
--rw-rw-r--  2.0 unx    27116 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1346 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Jul-08 09:03 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     3544 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Jul-08 09:03 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7862 b- defN 23-Jul-08 09:03 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      391 b- defN 23-Jul-08 09:03 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Jul-08 09:03 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-Jul-08 09:03 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Jul-08 09:03 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Jul-08 09:03 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7398 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6582 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     4252 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-Jul-08 09:03 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jul-08 09:03 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Jul-08 09:03 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Jul-08 09:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Jul-08 09:03 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3424 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Jul-08 09:03 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1639 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    10719 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Jul-08 09:03 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     3864 b- defN 23-Jul-08 09:03 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1458 b- defN 23-Jul-08 09:03 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8687 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Jul-08 09:03 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    14546 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx     1437 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder$3.class
--rw-rw-r--  2.0 unx     1344 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder$2.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     4094 b- defN 23-Jul-08 09:03 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-14 18:18 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:17 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:17 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:17 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:17 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-Jul-14 18:17 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Jul-14 18:18 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-14 18:18 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Jul-14 18:17 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Jul-14 18:17 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Jul-14 18:17 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Jul-14 18:18 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-14 18:18 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Jul-14 18:18 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Jul-14 18:18 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Jul-14 18:18 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jul-14 18:18 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Jul-14 18:17 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-Jul-14 18:18 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Jul-14 18:18 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    12048 b- defN 23-Jul-14 18:18 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2953 b- defN 23-Jul-14 18:18 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Jul-14 18:18 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     3672 b- defN 23-Jul-14 18:18 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-14 18:18 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1671 b- defN 23-Jul-14 18:18 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-14 18:18 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     5062 b- defN 23-Jul-14 18:18 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2003 b- defN 23-Jul-14 18:18 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-14 18:18 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Jul-14 18:17 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2298 b- defN 23-Jul-14 18:18 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     4913 b- defN 23-Jul-14 18:18 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2055 b- defN 23-Jul-14 18:18 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      454 b- defN 23-Jul-14 18:18 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Jul-14 18:18 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Jul-14 18:18 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3421 b- defN 23-Jul-14 18:18 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1236 b- defN 23-Jul-14 18:18 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Jul-14 18:18 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Jul-14 18:18 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Jul-14 18:18 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Jul-14 18:18 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-14 18:18 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-Jul-14 18:18 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     4114 b- defN 23-Jul-14 18:18 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Jul-14 18:17 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      342 b- defN 23-Jul-14 18:17 sklearn/HasOutlierField.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Jul-14 18:17 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jul-14 18:17 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-Jul-14 18:18 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Jul-14 18:18 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Jul-14 18:18 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx    10661 b- defN 23-Jul-14 18:18 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx      853 b- defN 23-Jul-14 18:17 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Jul-14 18:17 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-Jul-14 18:18 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Jul-14 18:18 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-Jul-14 18:18 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6948 b- defN 23-Jul-14 18:18 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx     4434 b- defN 23-Jul-14 18:18 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     5040 b- defN 23-Jul-14 18:18 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7648 b- defN 23-Jul-14 18:18 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Jul-14 18:18 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jul-14 18:18 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-14 18:18 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      932 b- defN 23-Jul-14 18:18 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-14 18:18 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-Jul-14 18:18 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-Jul-14 18:18 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-14 18:18 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jul-14 18:17 sklearn/IdentityTransformer.class
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Jul-14 18:17 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Jul-14 18:18 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-Jul-14 18:18 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Jul-14 18:18 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Jul-14 18:17 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Jul-14 18:18 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Jul-14 18:17 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Jul-14 18:18 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-Jul-14 18:18 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-14 18:18 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Jul-14 18:18 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2025 b- defN 23-Jul-14 18:18 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Jul-14 18:18 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jul-14 18:18 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10733 b- defN 23-Jul-14 18:18 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-14 18:18 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1032 b- defN 23-Jul-14 18:18 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Jul-14 18:18 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Jul-14 18:18 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2654 b- defN 23-Jul-14 18:18 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3510 b- defN 23-Jul-14 18:18 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Jul-14 18:17 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Jul-14 18:18 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-Jul-14 18:18 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Jul-14 18:18 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4450 b- defN 23-Jul-14 18:18 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Jul-14 18:18 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jul-14 18:17 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     1929 b- defN 23-Jul-14 18:17 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Jul-14 18:18 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      451 b- defN 23-Jul-14 18:17 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Jul-14 18:18 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4031 b- defN 23-Jul-14 18:18 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-Jul-14 18:18 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1375 b- defN 23-Jul-14 18:18 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Jul-14 18:18 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Jul-14 18:17 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Jul-14 18:18 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3031 b- defN 23-Jul-14 18:18 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Jul-14 18:17 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-Jul-14 18:18 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jul-14 18:18 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-Jul-14 18:18 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Jul-14 18:18 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Jul-14 18:18 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Jul-14 18:18 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7948 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Jul-14 18:17 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jul-14 18:17 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Jul-14 18:18 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Jul-14 18:18 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Jul-14 18:18 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2528 b- defN 23-Jul-14 18:18 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2987 b- defN 23-Jul-14 18:18 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Jul-14 18:18 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Jul-14 18:18 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Jul-14 18:18 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8225 b- defN 23-Jul-14 18:18 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-14 18:17 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-Jul-14 18:18 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6377 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jul-14 18:18 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-14 18:18 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Jul-14 18:18 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     6043 b- defN 23-Jul-14 18:17 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jul-14 18:17 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-Jul-14 18:18 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-14 18:18 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-Jul-14 18:18 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-Jul-14 18:18 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-14 18:18 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jul-14 18:17 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Jul-14 18:18 sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Jul-14 18:18 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Jul-14 18:18 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Jul-14 18:18 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Jul-14 18:17 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Jul-14 18:17 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Jul-14 18:18 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     5114 b- defN 23-Jul-14 18:18 sklearn/ScalarLabelUtil.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Jul-14 18:18 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-Jul-14 18:17 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jul-14 18:18 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-Jul-14 18:18 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3311 b- defN 23-Jul-14 18:18 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-14 18:18 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Jul-14 18:18 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-Jul-14 18:17 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-Jul-14 18:18 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Jul-14 18:18 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Jul-14 18:18 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Jul-14 18:18 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Jul-14 18:17 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-Jul-14 18:18 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Jul-14 18:18 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Jul-14 18:18 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     6971 b- defN 23-Jul-14 18:18 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-Jul-14 18:18 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-Jul-14 18:18 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-Jul-14 18:18 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-Jul-14 18:18 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-14 18:18 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Jul-14 18:18 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Jul-14 18:18 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Jul-14 18:18 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Jul-14 18:18 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Jul-14 18:18 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx     7408 b- defN 23-Jul-14 18:18 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Jul-14 18:18 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Jul-14 18:18 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jul-14 18:18 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Jul-14 18:18 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Jul-14 18:18 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Jul-14 18:18 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jul-14 18:18 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx      879 b- defN 23-Jul-14 18:18 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx      978 b- defN 23-Jul-14 18:18 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-Jul-14 18:18 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    19425 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-14 18:18 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2257 b- defN 23-Jul-14 18:18 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Jul-14 18:18 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Jul-14 18:18 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Jul-14 18:18 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-Jul-14 18:17 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Jul-14 18:17 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Jul-14 18:18 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     2808 b- defN 23-Jul-14 18:18 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Jul-14 18:18 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     7080 b- defN 23-Jul-14 18:18 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Jul-14 18:17 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Jul-14 18:18 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-Jul-14 18:18 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    14030 b- defN 23-Jul-14 18:17 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Jul-14 18:17 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4598 b- defN 23-Jul-14 18:17 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Jul-14 18:18 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Jul-14 18:18 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Jul-14 18:18 sklearn2pmml/pipeline/PMMLPipeline$4.class
+-rw-rw-r--  2.0 unx    27116 b- defN 23-Jul-14 18:18 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-Jul-14 18:18 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1346 b- defN 23-Jul-14 18:18 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Jul-14 18:17 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     3544 b- defN 23-Jul-14 18:18 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jul-14 18:17 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7862 b- defN 23-Jul-14 18:18 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Jul-14 18:18 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-14 18:18 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Jul-14 18:18 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Jul-14 18:18 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-14 18:18 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Jul-14 18:18 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Jul-14 18:18 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Jul-14 18:18 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Jul-14 18:18 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7398 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6582 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     4252 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-Jul-14 18:18 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Jul-14 18:18 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Jul-14 18:18 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Jul-14 18:18 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jul-14 18:18 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Jul-14 18:17 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3424 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Jul-14 18:17 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Jul-14 18:17 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Jul-14 18:18 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Jul-14 18:18 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Jul-14 18:18 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-14 18:18 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Jul-14 18:18 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     3864 b- defN 23-Jul-14 18:18 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1458 b- defN 23-Jul-14 18:18 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Jul-14 18:18 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Jul-14 18:18 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jul-14 18:18 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8687 b- defN 23-Jul-14 18:18 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jul-14 18:18 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Jul-14 18:18 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2764 b- defN 23-Jul-14 18:18 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Jul-14 18:18 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    14546 b- defN 23-Jul-14 18:17 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx     1437 b- defN 23-Jul-14 18:17 org/jpmml/sklearn/SkLearnEncoder$3.class
+-rw-rw-r--  2.0 unx     1344 b- defN 23-Jul-14 18:17 org/jpmml/sklearn/SkLearnEncoder$2.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Jul-14 18:18 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Jul-14 18:17 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx     4094 b- defN 23-Jul-14 18:17 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Jul-14 18:17 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
 405 files, 930740 bytes uncompressed, 409879 bytes compressed:  56.0%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.31
+Implementation-Version: 1.7.32
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.31</version>
+    <version>1.7.32</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.31
+version=1.7.32
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/classpath.txt`

 * *Files 23% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 jakarta.activation-2.0.1.jar
 jakarta.xml.bind-api-3.0.1.jar
 jaxb-core-3.0.2.jar
 jaxb-runtime-3.0.2.jar
 jcommander-1.72.jar
 pickle-1.4.jar
 pmml-converter-1.5.4.jar
-pmml-h2o-1.2.7.jar
+pmml-h2o-1.2.8.jar
 pmml-lightgbm-1.4.5.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
-pmml-python-1.1.15.jar
-pmml-sklearn-1.7.31.jar
-pmml-sklearn-extension-1.7.31.jar
-pmml-sklearn-h2o-1.7.31.jar
-pmml-sklearn-lightgbm-1.7.31.jar
-pmml-sklearn-statsmodels-1.7.31.jar
-pmml-sklearn-xgboost-1.7.31.jar
+pmml-python-1.1.16.jar
+pmml-sklearn-1.7.32.jar
+pmml-sklearn-extension-1.7.32.jar
+pmml-sklearn-h2o-1.7.32.jar
+pmml-sklearn-lightgbm-1.7.32.jar
+pmml-sklearn-statsmodels-1.7.32.jar
+pmml-sklearn-xgboost-1.7.32.jar
 pmml-statsmodels-1.0.4.jar
 pmml-xgboost-1.7.3.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-h2o-1.2.7.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-h2o-1.2.8.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,39 +1,41 @@
-Zip file size: 46831 bytes, number of entries: 37
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/
--rw-r--r--  2.0 unx      154 b- defN 23-Jun-15 21:20 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/services/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/jpmml/h2o/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 org/jpmml/h2o/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-15 21:20 META-INF/maven/org.jpmml/pmml-h2o/
--rw-rw-r--  2.0 unx       32 b- defN 23-Jun-15 21:20 META-INF/services/hex.genmodel.ModelMojoReader
--rw-rw-r--  2.0 unx     7803 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GbmMojoModelConverter.class
--rw-rw-r--  2.0 unx     1798 b- defN 23-Jun-15 21:20 org/jpmml/h2o/IsolationForestMojoModelConverter$1.class
--rw-rw-r--  2.0 unx     4088 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoModelConverter.class
--rw-rw-r--  2.0 unx     2013 b- defN 23-Jun-15 21:20 org/jpmml/h2o/testing/H2OEncoderBatchTest.class
--rw-rw-r--  2.0 unx     2897 b- defN 23-Jun-15 21:20 org/jpmml/h2o/testing/H2OEncoderBatch.class
--rw-rw-r--  2.0 unx     1591 b- defN 23-Jun-15 21:20 org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     8548 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMojoModelBaseConverter.class
--rw-rw-r--  2.0 unx     4555 b- defN 23-Jun-15 21:20 org/jpmml/h2o/IsolationForestMojoModelConverter.class
--rw-rw-r--  2.0 unx     3400 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoModelConverter$1.class
--rw-rw-r--  2.0 unx     4469 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMojoModelConverter.class
--rw-rw-r--  2.0 unx      664 b- defN 23-Jun-15 21:20 org/jpmml/h2o/H2OEncoder$1.class
--rw-rw-r--  2.0 unx     1344 b- defN 23-Jun-15 21:20 org/jpmml/h2o/MojoModelUtil$1.class
--rw-rw-r--  2.0 unx     3560 b- defN 23-Jun-15 21:20 org/jpmml/h2o/H2OEncoder.class
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoModel.class
--rw-rw-r--  2.0 unx    13590 b- defN 23-Jun-15 21:20 org/jpmml/h2o/SharedTreeMojoModelConverter.class
--rw-rw-r--  2.0 unx     4030 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMultinomialMojoModelConverter.class
--rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-15 21:20 org/jpmml/h2o/XGBoostMojoReader.class
--rw-rw-r--  2.0 unx     1412 b- defN 23-Jun-15 21:20 org/jpmml/h2o/ImputerUtil.class
--rw-rw-r--  2.0 unx     7050 b- defN 23-Jun-15 21:20 org/jpmml/h2o/DrfMojoModelConverter.class
--rw-rw-r--  2.0 unx     4968 b- defN 23-Jun-15 21:20 org/jpmml/h2o/Converter.class
--rw-rw-r--  2.0 unx     1840 b- defN 23-Jun-15 21:20 org/jpmml/h2o/MojoModelUtil.class
--rw-rw-r--  2.0 unx     3179 b- defN 23-Jun-15 21:20 org/jpmml/h2o/GlmMojoModelBaseConverter$1.class
--rw-rw-r--  2.0 unx     7520 b- defN 23-Jun-15 21:20 org/jpmml/h2o/StackedEnsembleMojoModelConverter.class
--rw-rw-r--  2.0 unx     2304 b- defN 23-Jun-15 21:20 org/jpmml/h2o/ConverterFactory.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Jun-15 21:20 META-INF/maven/org.jpmml/pmml-h2o/pom.xml
--rw-rw-r--  2.0 unx       52 b- defN 23-Jun-15 21:20 META-INF/maven/org.jpmml/pmml-h2o/pom.properties
-37 files, 97516 bytes uncompressed, 41373 bytes compressed:  57.6%
+Zip file size: 48655 bytes, number of entries: 39
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 META-INF/
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-09 20:14 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 META-INF/services/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 org/jpmml/h2o/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 org/jpmml/h2o/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-09 20:14 META-INF/maven/org.jpmml/pmml-h2o/
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-09 20:14 META-INF/services/hex.genmodel.ModelMojoReader
+-rw-rw-r--  2.0 unx     7803 b- defN 23-Jul-09 20:14 org/jpmml/h2o/GbmMojoModelConverter.class
+-rw-rw-r--  2.0 unx     1798 b- defN 23-Jul-09 20:14 org/jpmml/h2o/IsolationForestMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx     4088 b- defN 23-Jul-09 20:14 org/jpmml/h2o/XGBoostMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2013 b- defN 23-Jul-09 20:14 org/jpmml/h2o/testing/H2OEncoderBatchTest.class
+-rw-rw-r--  2.0 unx     2897 b- defN 23-Jul-09 20:14 org/jpmml/h2o/testing/H2OEncoderBatch.class
+-rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-09 20:14 org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     8548 b- defN 23-Jul-09 20:14 org/jpmml/h2o/GlmMojoModelBaseConverter.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jul-09 20:14 org/jpmml/h2o/SharedTree.class
+-rw-rw-r--  2.0 unx     4555 b- defN 23-Jul-09 20:14 org/jpmml/h2o/IsolationForestMojoModelConverter.class
+-rw-rw-r--  2.0 unx     3400 b- defN 23-Jul-09 20:14 org/jpmml/h2o/XGBoostMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx     4469 b- defN 23-Jul-09 20:14 org/jpmml/h2o/GlmMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2199 b- defN 23-Jul-09 20:14 org/jpmml/h2o/SharedTreeMojoModelConverter$1.class
+-rw-rw-r--  2.0 unx      664 b- defN 23-Jul-09 20:14 org/jpmml/h2o/H2OEncoder$1.class
+-rw-rw-r--  2.0 unx     1344 b- defN 23-Jul-09 20:14 org/jpmml/h2o/MojoModelUtil$1.class
+-rw-rw-r--  2.0 unx     3560 b- defN 23-Jul-09 20:14 org/jpmml/h2o/H2OEncoder.class
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-09 20:14 org/jpmml/h2o/XGBoostMojoModel.class
+-rw-rw-r--  2.0 unx    14293 b- defN 23-Jul-09 20:14 org/jpmml/h2o/SharedTreeMojoModelConverter.class
+-rw-rw-r--  2.0 unx     4030 b- defN 23-Jul-09 20:14 org/jpmml/h2o/GlmMultinomialMojoModelConverter.class
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Jul-09 20:14 org/jpmml/h2o/XGBoostMojoReader.class
+-rw-rw-r--  2.0 unx     1412 b- defN 23-Jul-09 20:14 org/jpmml/h2o/ImputerUtil.class
+-rw-rw-r--  2.0 unx     7050 b- defN 23-Jul-09 20:14 org/jpmml/h2o/DrfMojoModelConverter.class
+-rw-rw-r--  2.0 unx     4968 b- defN 23-Jul-09 20:14 org/jpmml/h2o/Converter.class
+-rw-rw-r--  2.0 unx     1840 b- defN 23-Jul-09 20:14 org/jpmml/h2o/MojoModelUtil.class
+-rw-rw-r--  2.0 unx     3179 b- defN 23-Jul-09 20:14 org/jpmml/h2o/GlmMojoModelBaseConverter$1.class
+-rw-rw-r--  2.0 unx     7520 b- defN 23-Jul-09 20:14 org/jpmml/h2o/StackedEnsembleMojoModelConverter.class
+-rw-rw-r--  2.0 unx     2304 b- defN 23-Jul-09 20:14 org/jpmml/h2o/ConverterFactory.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Jul-09 20:14 META-INF/maven/org.jpmml/pmml-h2o/pom.xml
+-rw-rw-r--  2.0 unx       52 b- defN 23-Jul-09 20:14 META-INF/maven/org.jpmml/pmml-h2o/pom.properties
+39 files, 100923 bytes uncompressed, 42885 bytes compressed:  57.5%
```

#### zipnote «TEMP»/diffoscope_fr7ro12l_/tmps5drwdhs_.zip

```diff
@@ -48,23 +48,29 @@
 
 Filename: org/jpmml/h2o/testing/H2OEncoderBatchTest$1.class
 Comment: 
 
 Filename: org/jpmml/h2o/GlmMojoModelBaseConverter.class
 Comment: 
 
+Filename: org/jpmml/h2o/SharedTree.class
+Comment: 
+
 Filename: org/jpmml/h2o/IsolationForestMojoModelConverter.class
 Comment: 
 
 Filename: org/jpmml/h2o/XGBoostMojoModelConverter$1.class
 Comment: 
 
 Filename: org/jpmml/h2o/GlmMojoModelConverter.class
 Comment: 
 
+Filename: org/jpmml/h2o/SharedTreeMojoModelConverter$1.class
+Comment: 
+
 Filename: org/jpmml/h2o/H2OEncoder$1.class
 Comment: 
 
 Filename: org/jpmml/h2o/MojoModelUtil$1.class
 Comment: 
 
 Filename: org/jpmml/h2o/H2OEncoder.class
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-H2O library
-Implementation-Version: 1.2.7
+Implementation-Version: 1.2.8
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### org/jpmml/h2o/SharedTreeMojoModelConverter.class

##### procyon -ec {}

```diff
@@ -1,36 +1,36 @@
 
 package org.jpmml.h2o;
 
 import com.google.common.collect.Iterables;
 import org.dmg.pmml.Model;
 import org.dmg.pmml.mining.MiningModel;
 import java.util.function.Function;
-import org.jpmml.converter.ValueUtil;
-import java.util.Objects;
 import org.jpmml.converter.ContinuousFeature;
 import org.dmg.pmml.tree.CountingBranchNode;
 import org.jpmml.converter.Feature;
 import java.util.Collection;
 import hex.genmodel.utils.GenmodelBitSet;
 import org.jpmml.converter.CategoricalFeature;
 import org.dmg.pmml.SimplePredicate;
 import hex.genmodel.algos.tree.NaSplitDir;
 import org.dmg.pmml.tree.CountingLeafNode;
-import org.dmg.pmml.tree.Node;
-import java.util.Map;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.ModelUtil;
 import org.dmg.pmml.MiningFunction;
 import org.dmg.pmml.Predicate;
+import hex.genmodel.utils.ByteBufferWrapper;
 import org.jpmml.converter.CategoryManager;
 import org.dmg.pmml.True;
-import hex.genmodel.utils.ByteBufferWrapper;
 import org.jpmml.converter.ContinuousLabel;
 import org.dmg.pmml.DataType;
+import org.jpmml.converter.ValueUtil;
+import java.util.Objects;
+import org.dmg.pmml.tree.Node;
+import java.util.Map;
 import java.util.ArrayList;
 import org.jpmml.converter.PredicateManager;
 import org.dmg.pmml.tree.TreeModel;
 import java.util.List;
 import org.jpmml.converter.Schema;
 import hex.genmodel.MojoModel;
 import java.lang.reflect.Field;
@@ -55,42 +55,61 @@
         final byte[][] compressedTrees = getCompressedTrees(model);
         final byte[][] compressedTreesAux = getCompressedTreesAux(model);
         final PredicateManager predicateManager = new PredicateManager();
         final List<TreeModel> result = new ArrayList<TreeModel>();
         for (int i = 0, max = Math.max(compressedTrees.length, compressedTreesAux.length); i < max; ++i) {
             final byte[] compressedTree = compressedTrees[i];
             final byte[] compressedTreeAux = compressedTreesAux[i];
-            final TreeModel treeModel = this.encodeTreeModel(compressedTree, compressedTreeAux, predicateManager, schema);
+            final Map<Integer, SharedTreeMojoModel.AuxInfo> auxInfos = SharedTreeMojoModel.readAuxInfos(compressedTreeAux);
+            final SharedTree sharedTree = (SharedTree)new SharedTreeMojoModelConverter.SharedTreeMojoModelConverter$1(this, compressedTree, compressedTreeAux, (Map)auxInfos);
+            final TreeModel treeModel = encodeTreeModel(sharedTree, predicateManager, schema);
             result.add(treeModel);
         }
         return result;
     }
     
-    public TreeModel encodeTreeModel(final byte[] compressedTree, final byte[] compressedTreeAux, final PredicateManager predicateManager, final Schema schema) {
+    protected void ensureScore(final Node node, final double score) {
+        if (node.hasScore()) {
+            if (!Objects.equals(node.getScore(), Double.valueOf(score))) {
+                throw new IllegalArgumentException();
+            }
+        }
+        else {
+            node.setScore((Object)Double.valueOf(score));
+        }
+    }
+    
+    protected void ensureRecordCount(final Node node, final double recordCount) {
+        if (node.getRecordCount() != null) {
+            throw new IllegalArgumentException();
+        }
+        node.setRecordCount(ValueUtil.narrow(recordCount));
+    }
+    
+    public static TreeModel encodeTreeModel(final SharedTree sharedTree, final PredicateManager predicateManager, final Schema schema) {
         final Label label = (Label)new ContinuousLabel(DataType.DOUBLE);
-        final ByteBufferWrapper byteBuffer = new ByteBufferWrapper(compressedTree);
-        final Map<Integer, SharedTreeMojoModel.AuxInfo> auxInfos = SharedTreeMojoModel.readAuxInfos(compressedTreeAux);
-        final Node root = this.encodeNode(byteBuffer, Integer.valueOf(0), (Predicate)True.INSTANCE, compressedTree, auxInfos, new CategoryManager(), predicateManager, schema);
+        final Node root = encodeNode(sharedTree, null, sharedTree.nextId(), (Predicate)True.INSTANCE, new CategoryManager(), predicateManager, schema);
         final TreeModel treeModel = new TreeModel(MiningFunction.REGRESSION, ModelUtil.createMiningSchema(label), root).setMissingValueStrategy(TreeModel.MissingValueStrategy.DEFAULT_CHILD);
         return treeModel;
     }
     
-    public Node encodeNode(final ByteBufferWrapper byteBuffer, final Integer id, final Predicate predicate, final byte[] compressedTree, final Map<Integer, SharedTreeMojoModel.AuxInfo> auxInfos, final CategoryManager categoryManager, final PredicateManager predicateManager, final Schema schema) {
-        final SharedTreeMojoModel.AuxInfo auxInfo = (SharedTreeMojoModel.AuxInfo)auxInfos.get(id);
-        if (auxInfo == null) {
-            throw new IllegalArgumentException();
+    public static Node encodeNode(final SharedTree sharedTree, ByteBufferWrapper byteBuffer, final Integer id, final Predicate predicate, final CategoryManager categoryManager, final PredicateManager predicateManager, final Schema schema) {
+        final byte[] compressedTree = sharedTree.getCompressedTree();
+        if (byteBuffer == null) {
+            byteBuffer = new ByteBufferWrapper(compressedTree);
         }
+        final SharedTreeMojoModel.AuxInfo auxInfo = sharedTree.getAuxInfo((int)id);
         final int nodeType = byteBuffer.get1U();
         final int lmask = nodeType & 0x33;
         final int lmask2 = (nodeType & 0xC0) >> 2;
         final int equal = nodeType & 0xC;
         final int colId = byteBuffer.get2();
         if (colId == 65535) {
             final double score = (double)byteBuffer.get4f();
-            final Node result = (Node)new CountingLeafNode((Object)Double.valueOf(score), predicate).setId((Object)id);
+            final Node result = (Node)new CountingLeafNode((Object)Double.valueOf(score), predicate).setId((Object)toNodeId(auxInfo != null, id));
             return result;
         }
         final int naSplitDir = byteBuffer.get1U();
         final boolean naVsRest = naSplitDir == NaSplitDir.NAvsREST.value();
         final boolean leftward = naSplitDir == NaSplitDir.NALeft.value() || naSplitDir == NaSplitDir.Left.value();
         final Feature feature = schema.getFeature(colId);
         CategoryManager leftCategoryManager = categoryManager;
@@ -136,29 +155,29 @@
         }
         else {
             final ContinuousFeature continuousFeature = feature.toContinuousFeature();
             final Double splitVal = Double.valueOf(byteBuffer.get4f());
             leftPredicate = predicateManager.createSimplePredicate((Feature)continuousFeature, SimplePredicate.Operator.LESS_THAN, (Object)splitVal);
             rightPredicate = predicateManager.createSimplePredicate((Feature)continuousFeature, SimplePredicate.Operator.GREATER_OR_EQUAL, (Object)splitVal);
         }
-        final Integer leftId = Integer.valueOf(auxInfo.nidL);
+        final Integer leftId = Integer.valueOf((auxInfo != null) ? auxInfo.nidL : ((int)sharedTree.nextId()));
         final ByteBufferWrapper leftByteBuffer = new ByteBufferWrapper(compressedTree);
         leftByteBuffer.skip(byteBuffer.position());
         if (lmask <= 3) {
             leftByteBuffer.skip(lmask + 1);
         }
         Node leftChild;
         if ((lmask & 0x10) != 0x0) {
             final double score2 = (double)leftByteBuffer.get4f();
-            leftChild = (Node)new CountingLeafNode((Object)Double.valueOf(score2), leftPredicate).setId((Object)leftId);
+            leftChild = (Node)new CountingLeafNode((Object)Double.valueOf(score2), leftPredicate).setId((Object)toNodeId(auxInfo != null, leftId));
         }
         else {
-            leftChild = this.encodeNode(leftByteBuffer, leftId, leftPredicate, compressedTree, auxInfos, leftCategoryManager, predicateManager, schema);
+            leftChild = encodeNode(sharedTree, leftByteBuffer, leftId, leftPredicate, leftCategoryManager, predicateManager, schema);
         }
-        final Integer rightId = Integer.valueOf(auxInfo.nidR);
+        final Integer rightId = Integer.valueOf((auxInfo != null) ? auxInfo.nidR : ((int)sharedTree.nextId()));
         final ByteBufferWrapper rightByteBuffer = new ByteBufferWrapper(compressedTree);
         rightByteBuffer.skip(byteBuffer.position());
         switch (lmask) {
             case 0: {
                 rightByteBuffer.skip(rightByteBuffer.get1U());
                 break;
             }
@@ -181,50 +200,31 @@
             default: {
                 throw new IllegalArgumentException("Node type " + lmask + " is not supported");
             }
         }
         Node rightChild;
         if ((lmask2 & 0x10) != 0x0) {
             final double score3 = (double)rightByteBuffer.get4f();
-            rightChild = (Node)new CountingLeafNode((Object)Double.valueOf(score3), rightPredicate).setId((Object)rightId);
+            rightChild = (Node)new CountingLeafNode((Object)Double.valueOf(score3), rightPredicate).setId((Object)toNodeId(auxInfo != null, rightId));
         }
         else {
-            rightChild = this.encodeNode(rightByteBuffer, rightId, rightPredicate, compressedTree, auxInfos, rightCategoryManager, predicateManager, schema);
+            rightChild = encodeNode(sharedTree, rightByteBuffer, rightId, rightPredicate, rightCategoryManager, predicateManager, schema);
         }
-        this.ensureScore(leftChild, auxInfo.predL);
-        this.ensureScore(rightChild, auxInfo.predR);
-        this.ensureRecordCount(leftChild, auxInfo.weightL);
-        this.ensureRecordCount(rightChild, auxInfo.weightR);
-        final Node result2 = new CountingBranchNode((Object)null, predicate).setId((Object)id).setDefaultChild(leftward ? leftChild.getId() : rightChild.getId()).addNodes(leftChild, rightChild);
-        if (id == 0) {
+        if (auxInfo != null) {
+            sharedTree.encodeAuxInfo(leftChild, (double)auxInfo.predL, (double)auxInfo.weightL);
+            sharedTree.encodeAuxInfo(rightChild, (double)auxInfo.predR, (double)auxInfo.weightR);
+        }
+        final Node result2 = new CountingBranchNode((Object)null, predicate).setId((Object)toNodeId(auxInfo != null, id)).setDefaultChild(leftward ? leftChild.getId() : rightChild.getId()).addNodes(leftChild, rightChild);
+        if (auxInfo != null && id == 0) {
             final float weight = auxInfo.weightL + auxInfo.weightR;
-            this.ensureScore(result2, (auxInfo.predL * auxInfo.weightL + auxInfo.predR * auxInfo.weightR) / weight);
-            this.ensureRecordCount(result2, weight);
+            sharedTree.encodeAuxInfo(result2, (double)((auxInfo.predL * auxInfo.weightL + auxInfo.predR * auxInfo.weightR) / weight), (double)weight);
         }
         return result2;
     }
     
-    protected void ensureScore(final Node node, final double score) {
-        if (node.hasScore()) {
-            if (!Objects.equals(node.getScore(), Double.valueOf(score))) {
-                throw new IllegalArgumentException();
-            }
-        }
-        else {
-            node.setScore((Object)Double.valueOf(score));
-        }
-    }
-    
-    protected void ensureRecordCount(final Node node, final double recordCount) {
-        if (node.getRecordCount() != null) {
-            throw new IllegalArgumentException();
-        }
-        node.setRecordCount(ValueUtil.narrow(recordCount));
-    }
-    
     public static Model encodeTreeEnsemble(final List<TreeModel> treeModels, final Function<List<TreeModel>, MiningModel> ensembleFunction) {
         if (treeModels.size() == 1) {
             return (Model)Iterables.getOnlyElement((Iterable)treeModels);
         }
         return (Model)ensembleFunction.apply(treeModels);
     }
     
@@ -240,14 +240,18 @@
         return (int)getFieldValue(SharedTreeMojoModelConverter.FIELD_NTREEGROUPS, (MojoModel)model);
     }
     
     public static int getNTreesPerGroup(final SharedTreeMojoModel model) {
         return (int)getFieldValue(SharedTreeMojoModelConverter.FIELD_NTREESPERGROUP, (MojoModel)model);
     }
     
+    private static Integer toNodeId(final boolean hasAux, final Integer id) {
+        return Integer.valueOf(hasAux ? ((int)id) : (id + 1));
+    }
+    
     static {
         try {
             FIELD_COMPRESSEDTREES = SharedTreeMojoModel.class.getDeclaredField("_compressed_trees");
             FIELD_COMPRESSEDTREESAUX = SharedTreeMojoModel.class.getDeclaredField("_compressed_trees_aux");
             FIELD_NTREEGROUPS = SharedTreeMojoModel.class.getDeclaredField("_ntree_groups");
             FIELD_NTREESPERGROUP = SharedTreeMojoModel.class.getDeclaredField("_ntrees_per_group");
         }
```

#### META-INF/maven/org.jpmml/pmml-h2o/pom.xml

##### META-INF/maven/org.jpmml/pmml-h2o/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-h2o</artifactId>
-    <version>1.2.7</version>
+    <version>1.2.8</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-h2o</artifactId>
   <packaging>jar</packaging>
   <name>JPMML H2O.ai converter</name>
   <description>JPMML H2O.ai to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-h2o/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-h2o
 groupId=org.jpmml
-version=1.2.7
+version=1.2.8
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 23% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5711 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Jul-08 09:24 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:24 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-Jul-08 09:24 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-08 09:24 com/sklearn2pmml/Main$1.class
--rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-08 09:23 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-Jul-08 09:24 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-11 files, 13013 bytes uncompressed, 4235 bytes compressed:  67.5%
+Zip file size: 5709 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-14 19:11 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-Jul-14 19:11 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-14 19:11 com/sklearn2pmml/Main$1.class
+-rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+11 files, 13013 bytes uncompressed, 4233 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.94.1
+Implementation-Version: 0.95.0
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

##### META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml

```diff
@@ -24,15 +24,15 @@
     <tag>HEAD</tag>
   </scm>
   <issueManagement>
     <system>GitHub</system>
     <url>https://github.com/jpmml/sklearn2pmml/issues</url>
   </issueManagement>
   <properties>
-    <jpmml-sklearn.version>1.7.31</jpmml-sklearn.version>
+    <jpmml-sklearn.version>1.7.32</jpmml-sklearn.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>org.jpmml</groupId>
       <artifactId>pmml-sklearn</artifactId>
       <version>${jpmml-sklearn.version}</version>
       <exclusions>
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.31.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.32.jar`

 * *Files 13% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 7311 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Jul-08 09:03 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     1953 b- defN 23-Jul-08 09:03 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Jul-08 09:03 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-Jul-08 09:03 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-Jul-08 09:03 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-14 18:18 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Jul-14 18:18 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Jul-14 18:18 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     1953 b- defN 23-Jul-14 18:18 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2102 b- defN 23-Jul-14 18:18 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2126 b- defN 23-Jul-14 18:18 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3298 b- defN 23-Jul-14 18:18 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Jul-14 18:17 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
 15 files, 11392 bytes uncompressed, 5231 bytes compressed:  54.1%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.31</version>
+    <version>1.7.32</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Jul 08 09:03:24 EEST 2023
-version=1.7.31
+#Fri Jul 14 18:18:07 EEST 2023
+version=1.7.32
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.31.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.32.jar`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,65 +1,65 @@
-Zip file size: 83825 bytes, number of entries: 63
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-08 09:03 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-08 09:03 sklego/meta/
--rw-rw-r--  2.0 unx     4312 b- defN 23-Jul-08 09:03 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      412 b- defN 23-Jul-08 09:03 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Jul-08 09:03 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      421 b- defN 23-Jul-08 09:03 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     1332 b- defN 23-Jul-08 09:03 pycaret/preprocess/RemoveOutliers$1.class
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jul-08 09:03 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     3125 b- defN 23-Jul-08 09:03 pycaret/preprocess/RemoveOutliers.class
--rw-rw-r--  2.0 unx     7822 b- defN 23-Jul-08 09:03 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-08 09:03 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Jul-08 09:03 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-Jul-08 09:03 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Jul-08 09:03 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8333 b- defN 23-Jul-08 09:03 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Jul-08 09:03 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Jul-08 09:03 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Jul-08 09:03 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Jul-08 09:03 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1240 b- defN 23-Jul-08 09:03 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Jul-08 09:03 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      374 b- defN 23-Jul-08 09:03 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Jul-08 09:03 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Jul-08 09:03 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Jul-08 09:03 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-08 09:03 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Jul-08 09:03 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     8474 b- defN 23-Jul-08 09:03 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Jul-08 09:03 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Jul-08 09:03 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-08 09:03 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Jul-08 09:03 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Jul-08 09:03 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Jul-08 09:03 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     8108 b- defN 23-Jul-08 09:03 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Jul-08 09:03 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Jul-08 09:03 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Jul-08 09:03 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Jul-08 09:03 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-08 09:03 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-08 09:03 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Jul-08 09:03 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Jul-08 09:03 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-08 09:03 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Jul-08 09:03 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-08 09:03 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-Jul-08 09:03 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-08 09:03 sklego/meta/EstimatorTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Jul-08 09:03 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
-63 files, 171292 bytes uncompressed, 74759 bytes compressed:  56.4%
+Zip file size: 83824 bytes, number of entries: 63
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-14 18:18 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 18:18 sklego/meta/
+-rw-rw-r--  2.0 unx     4312 b- defN 23-Jul-14 18:18 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      412 b- defN 23-Jul-14 18:18 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Jul-14 18:18 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      421 b- defN 23-Jul-14 18:18 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Jul-14 18:18 pycaret/preprocess/RemoveOutliers$1.class
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jul-14 18:18 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     3125 b- defN 23-Jul-14 18:18 pycaret/preprocess/RemoveOutliers.class
+-rw-rw-r--  2.0 unx     7822 b- defN 23-Jul-14 18:18 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-14 18:18 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Jul-14 18:18 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-Jul-14 18:18 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Jul-14 18:18 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8333 b- defN 23-Jul-14 18:18 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Jul-14 18:18 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Jul-14 18:18 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Jul-14 18:18 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Jul-14 18:18 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Jul-14 18:18 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Jul-14 18:18 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      374 b- defN 23-Jul-14 18:18 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Jul-14 18:18 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Jul-14 18:18 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Jul-14 18:18 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Jul-14 18:18 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Jul-14 18:18 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     8474 b- defN 23-Jul-14 18:18 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Jul-14 18:18 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-Jul-14 18:18 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-14 18:18 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Jul-14 18:18 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Jul-14 18:18 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Jul-14 18:18 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     8108 b- defN 23-Jul-14 18:18 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Jul-14 18:18 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Jul-14 18:18 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Jul-14 18:18 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Jul-14 18:18 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-14 18:18 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-14 18:18 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Jul-14 18:18 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Jul-14 18:18 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jul-14 18:18 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Jul-14 18:18 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Jul-14 18:18 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-Jul-14 18:18 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-14 18:18 sklego/meta/EstimatorTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Jul-14 18:17 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-Jul-14 18:18 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+63 files, 171292 bytes uncompressed, 74758 bytes compressed:  56.4%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.31</version>
+    <version>1.7.32</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Jul 08 09:03:24 EEST 2023
-version=1.7.31
+#Fri Jul 14 18:18:06 EEST 2023
+version=1.7.32
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/pickle-1.4.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/pickle-1.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.95.0/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.95.0/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.94.1/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.95.0/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

