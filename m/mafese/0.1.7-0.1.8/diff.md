# Comparing `tmp/mafese-0.1.7.tar.gz` & `tmp/mafese-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.7.tar", last modified: Thu Jul 13 10:58:39 2023, max compression
+gzip compressed data, was "mafese-0.1.8.tar", last modified: Fri Jul 14 03:49:53 2023, max compression
```

## Comparing `mafese-0.1.7.tar` & `mafese-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-13 10:57:18.000000 mafese-0.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-13 10:57:18.000000 mafese-0.1.7/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 10:57:18.000000 mafese-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 10:57:18.000000 mafese-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-13 10:58:39.781923 mafese-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-07-13 10:57:18.000000 mafese-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.777923 mafese-0.1.7/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.777923 mafese-0.1.7/mafese/embedded/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/embedded/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/embedded/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32353 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.777923 mafese-0.1.7/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:58:39.781923 mafese-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-13 10:57:18.000000 mafese-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 03:48:45.000000 mafese-0.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-14 03:48:45.000000 mafese-0.1.8/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 03:48:45.000000 mafese-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 03:48:45.000000 mafese-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-14 03:49:53.029676 mafese-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-07-14 03:48:45.000000 mafese-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.009676 mafese-0.1.8/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.005676 mafese-0.1.8/mafese/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.021676 mafese-0.1.8/mafese/data/cls/
+-rw-r--r--   0 runner    (1001) docker     (123)   369879 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Arrhythmia.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Blood.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22145 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/BreastCancer.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119681 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/BreastEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/CongressEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498322 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Digits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Glass.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/HeartEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   438254 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Hill-valley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    37338 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Horse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    75329 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Ionosphere.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Lymphography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  5205194 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Madelon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Monk1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Monk2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Monk3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    85876 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Sonar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Soybean-small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/SpectEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Tic-tac-toe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    65346 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Vowel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1053755 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/WaveformEW.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Wine.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/Zoo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/aggregation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40191 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/aniso.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/appendicitis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/balance.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45030 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/banknote.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39793 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/blobs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/circles.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/diagnosis_II.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/ecoli.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/flame.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/heart.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/jain.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/liver.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39579 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/moons.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/mouse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/pathbased.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/seeds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/smiley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40499 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/varied.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/vary-density.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/vertebral2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   119889 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/cls/wdbc.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.025676 mafese-0.1.8/mafese/data/reg/
+-rw-r--r--   0 runner    (1001) docker     (123)    35644 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/boston-housing.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/computer-hardware.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25774 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/diabetes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1981727 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/gauss-100-20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   400064 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/gauss-50-12.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   894463 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/gauss-75-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/data/reg/linnerud.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.025676 mafese-0.1.8/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32353 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-14 03:48:45.000000 mafese-0.1.8/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.009676 mafese-0.1.8/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 03:49:52.000000 mafese-0.1.8/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:49:53.029676 mafese-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-14 03:48:45.000000 mafese-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:49:53.029676 mafese-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-14 03:48:45.000000 mafese-0.1.8/tests/test_wrapper.py
```

### Comparing `mafese-0.1.7/CODE_OF_CONDUCT.md` & `mafese-0.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/ChangeLog.md` & `mafese-0.1.8/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Version 0.1.8
+
++ Fix bug load data from library.
+
+---------------------------------------------------------------------
+
 # Version 0.1.7
 
 + Remove some unknown datasets
 + Fix bug name in Kendall and Spearman functions of FilterSelector 
 + Add Relief-based family to FilterSelector 
   + Relief Original 
   + Relief-F
```

### Comparing `mafese-0.1.7/LICENSE` & `mafese-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/PKG-INFO` & `mafese-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.7
+Version: 0.1.8
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.7-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.8-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -82,15 +82,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.7
+$ pip install mafese==0.1.8
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
```

### Comparing `mafese-0.1.7/README.md` & `mafese-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.7-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.8-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -39,15 +39,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.7
+$ pip install mafese==0.1.8
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
```

### Comparing `mafese-0.1.7/mafese/__init__.py` & `mafese-0.1.8/mafese/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
 from mafese.wrapper.mha import MhaSelector, MultiMhaSelector
 from mafese.embedded.lasso import LassoSelector
```

### Comparing `mafese-0.1.7/mafese/embedded/lasso.py` & `mafese-0.1.8/mafese/embedded/lasso.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/embedded/tree.py` & `mafese-0.1.8/mafese/embedded/tree.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/filter.py` & `mafese-0.1.8/mafese/filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/selector.py` & `mafese-0.1.8/mafese/selector.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/unsupervised.py` & `mafese-0.1.8/mafese/unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/correlation.py` & `mafese-0.1.8/mafese/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/data_loader.py` & `mafese-0.1.8/mafese/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/encoder.py` & `mafese-0.1.8/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/estimator.py` & `mafese-0.1.8/mafese/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/evaluator.py` & `mafese-0.1.8/mafese/utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/mealpy_util.py` & `mafese-0.1.8/mafese/utils/mealpy_util.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/transfer.py` & `mafese-0.1.8/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/utils/validator.py` & `mafese-0.1.8/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/wrapper/mha.py` & `mafese-0.1.8/mafese/wrapper/mha.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/wrapper/recursive.py` & `mafese-0.1.8/mafese/wrapper/recursive.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese/wrapper/sequential.py` & `mafese-0.1.8/mafese/wrapper/sequential.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/mafese.egg-info/PKG-INFO` & `mafese-0.1.8/mafese.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.7
+Version: 0.1.8
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.7-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.8-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -82,15 +82,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.7
+$ pip install mafese==0.1.8
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
```

### Comparing `mafese-0.1.7/setup.py` & `mafese-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.7",
+    version="0.1.8",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
```

### Comparing `mafese-0.1.7/tests/test_embedded.py` & `mafese-0.1.8/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/tests/test_filter.py` & `mafese-0.1.8/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/tests/test_unsupervised.py` & `mafese-0.1.8/tests/test_unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.7/tests/test_wrapper.py` & `mafese-0.1.8/tests/test_wrapper.py`

 * *Files identical despite different names*

