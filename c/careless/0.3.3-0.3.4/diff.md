# Comparing `tmp/careless-0.3.3.tar.gz` & `tmp/careless-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.3.3.tar", last modified: Thu Jul 13 21:22:53 2023, max compression
+gzip compressed data, was "careless-0.3.4.tar", last modified: Fri Jul 14 01:42:47 2023, max compression
```

## Comparing `careless-0.3.3.tar` & `careless-0.3.4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-13 21:22:42.000000 careless-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 21:22:42.000000 careless-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 21:22:53.940818 careless-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-13 21:22:42.000000 careless-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.932819 careless-0.3.3/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 21:22:42.000000 careless-0.3.3/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-13 21:22:42.000000 careless-0.3.3/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-13 21:22:42.000000 careless-0.3.3/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-13 21:22:42.000000 careless-0.3.3/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-07-13 21:22:42.000000 careless-0.3.3/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-13 21:22:42.000000 careless-0.3.3/careless/io/xds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.936818 careless-0.3.3/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-13 21:22:42.000000 careless-0.3.3/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-13 21:22:42.000000 careless-0.3.3/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/prior_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-13 21:22:42.000000 careless-0.3.3/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 21:22:42.000000 careless-0.3.3/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.932819 careless-0.3.3/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 21:22:53.000000 careless-0.3.3/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-13 21:22:42.000000 careless-0.3.3/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-13 21:22:42.000000 careless-0.3.3/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 21:22:53.940818 careless-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-13 21:22:42.000000 careless-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:53.940818 careless-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:22:42.000000 careless-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-13 21:22:42.000000 careless-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-13 21:22:42.000000 careless-0.3.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.234871 careless-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-14 01:42:35.000000 careless-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 01:42:35.000000 careless-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 01:42:47.234871 careless-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-07-14 01:42:35.000000 careless-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.226871 careless-0.3.4/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 01:42:35.000000 careless-0.3.4/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-14 01:42:35.000000 careless-0.3.4/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-14 01:42:35.000000 careless-0.3.4/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-14 01:42:35.000000 careless-0.3.4/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-07-14 01:42:35.000000 careless-0.3.4/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-14 01:42:35.000000 careless-0.3.4/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-14 01:42:35.000000 careless-0.3.4/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-07-14 01:42:35.000000 careless-0.3.4/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/prior_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-14 01:42:35.000000 careless-0.3.4/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-14 01:42:35.000000 careless-0.3.4/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.226871 careless-0.3.4/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 01:42:47.000000 careless-0.3.4/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.230871 careless-0.3.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-14 01:42:35.000000 careless-0.3.4/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-14 01:42:35.000000 careless-0.3.4/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 01:42:47.234871 careless-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-14 01:42:35.000000 careless-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:47.234871 careless-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:42:35.000000 careless-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-14 01:42:35.000000 careless-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-14 01:42:35.000000 careless-0.3.4/tests/test_cli.py
```

### Comparing `careless-0.3.3/LICENSE` & `careless-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/PKG-INFO` & `careless-0.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.3
+Version: 0.3.4
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.3/README.md` & `careless-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/common.py` & `careless-0.3.4/careless/args/common.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/crossvalidation.py` & `careless-0.3.4/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/filtration.py` & `careless-0.3.4/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/interpretation.py` & `careless-0.3.4/careless/args/interpretation.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/optimizer.py` & `careless-0.3.4/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/poly.py` & `careless-0.3.4/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/positional_encoding.py` & `careless-0.3.4/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/prior.py` & `careless-0.3.4/careless/args/prior.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 name = "Prior"
 description = """
 Options related to the prior distribution applied to the structure factors during merging.
 """
 
 args_and_kwargs = (
+    (("--kl-weight",), {
+        "help": "Set the weight of the kl divergence term relative to the likliehood. "
+                "By default, by default this is based purely on the number of reflections.",
+        "type": float, 
+        "default": None,
+    }),
+
     (("--wilson-prior-b",), {
         "help": "This flag enables learning reflections on a particular Wilson scale. "
                 "By default, the Wilson prior is flat across resolution bins. ",
         "type": float, 
         "default": None,
     }),
```

### Comparing `careless-0.3.3/careless/args/required.py` & `careless-0.3.4/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/scaling.py` & `careless-0.3.4/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/args/tf_options.py` & `careless-0.3.4/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/callbacks/progress_bar.py` & `careless-0.3.4/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/careless.py` & `careless-0.3.4/careless/careless.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/io/asu.py` & `careless-0.3.4/careless/io/asu.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/io/formatter.py` & `careless-0.3.4/careless/io/formatter.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/io/manager.py` & `careless-0.3.4/careless/io/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,15 +445,15 @@
                     n_images = np.max(BaseModel.get_image_id(self.inputs)) + 1
                     image_scaler = ImageScaler(n_images)
                     scaling_model = HybridImageScaler(mlp_scaler, image_scaler)
                 else:
                     scaling_model = mlp_scaler
 
         from tensorflow_probability import distributions as tfd
-        model = VariationalMergingModel(surrogate_posterior, prior, likelihood, scaling_model, parser.mc_samples)
+        model = VariationalMergingModel(surrogate_posterior, prior, likelihood, scaling_model, parser.mc_samples, kl_weight=parser.kl_weight)
 
         opt = tf.keras.optimizers.Adam(
             parser.learning_rate,
             parser.beta_1,
             parser.beta_2,
         )
```

### Comparing `careless-0.3.3/careless/io/xds.py` & `careless-0.3.4/careless/io/xds.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/base.py` & `careless-0.3.4/careless/models/base.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/likelihoods/laue.py` & `careless-0.3.4/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/likelihoods/mono.py` & `careless-0.3.4/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.4/careless/models/merging/surrogate_posteriors.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/merging/variational.py` & `careless-0.3.4/careless/models/merging/variational.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/priors/empirical.py` & `careless-0.3.4/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/priors/wilson.py` & `careless-0.3.4/careless/models/priors/wilson.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/scaling/image.py` & `careless-0.3.4/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/models/scaling/nn.py` & `careless-0.3.4/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/parser.py` & `careless-0.3.4/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/ccanom.py` & `careless-0.3.4/careless/stats/ccanom.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/cchalf.py` & `careless-0.3.4/careless/stats/cchalf.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/ccpred.py` & `careless-0.3.4/careless/stats/ccpred.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/completeness.py` & `careless-0.3.4/careless/stats/completeness.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/parser.py` & `careless-0.3.4/careless/stats/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/prior_b.py` & `careless-0.3.4/careless/stats/prior_b.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/rescale.py` & `careless-0.3.4/careless/stats/rescale.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/stats/rsplit.py` & `careless-0.3.4/careless/stats/rsplit.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/utils/distributions.py` & `careless-0.3.4/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/utils/laue.py` & `careless-0.3.4/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless/utils/positional_encoding.py` & `careless-0.3.4/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/careless.egg-info/PKG-INFO` & `careless-0.3.4/careless.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.3.3
+Version: 0.3.4
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
```

### Comparing `careless-0.3.3/careless.egg-info/SOURCES.txt` & `careless-0.3.4/careless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/scripts/make_difference_map` & `careless-0.3.4/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/scripts/stream2mtz` & `careless-0.3.4/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/setup.py` & `careless-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/tests/conftest.py` & `careless-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careless-0.3.3/tests/test_cli.py` & `careless-0.3.4/tests/test_cli.py`

 * *Files identical despite different names*

