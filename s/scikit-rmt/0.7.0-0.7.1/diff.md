# Comparing `tmp/scikit-rmt-0.7.0.tar.gz` & `tmp/scikit-rmt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-rmt-0.7.0.tar", last modified: Sat Jul  8 22:53:00 2023, max compression
+gzip compressed data, was "dist/scikit-rmt-0.7.1.tar", last modified: Fri Jul 14 20:29:18 2023, max compression
```

## Comparing `scikit-rmt-0.7.0.tar` & `scikit-rmt-0.7.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.380699 scikit-rmt-0.7.0/
--rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.7.0/.coveragerc
--rw-r--r--   0 santorum   (501) staff       (20)      278 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/.travis.yml
--rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.7.0/CITATION.cff
--rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.7.0/LICENSE
--rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.7.0/MANIFEST.in
--rw-r--r--   0 santorum   (501) staff       (20)     2569 2023-07-08 22:52:37.000000 scikit-rmt-0.7.0/Makefile
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 22:53:00.381033 scikit-rmt-0.7.0/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/README.md
--rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.7.0/conf.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.339736 scikit-rmt-0.7.0/docs/
--rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.7.0/docs/modules.rst
--rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.7.0/docs/readthedocs-requirements.txt
--rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.7.0/docs/skrmt.covariance.rst
--rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/docs/skrmt.ensemble.rst
--rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.7.0/docs/skrmt.rst
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.347457 scikit-rmt-0.7.0/examples/
--rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.7.0/examples/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2155 2023-07-08 20:47:44.000000 scikit-rmt-0.7.0/examples/plot_boosting_density_representation.py
--rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.7.0/examples/plot_circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.7.0/examples/plot_complex_histograms.py
--rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.7.0/examples/plot_gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.7.0/examples/plot_manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.7.0/examples/plot_wishart_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.7.0/index.rst
--rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.7.0/readthedocs.yml
--rw-r--r--   0 santorum   (501) staff       (20)       65 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/requirements.txt
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.350678 scikit-rmt-0.7.0/scikit_rmt.egg-info/
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/SOURCES.txt
--rw-r--r--   0 santorum   (501) staff       (20)        1 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/dependency_links.txt
--rw-r--r--   0 santorum   (501) staff       (20)       66 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/requires.txt
--rw-r--r--   0 santorum   (501) staff       (20)        6 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/top_level.txt
--rw-r--r--   0 santorum   (501) staff       (20)       38 2023-07-08 22:53:00.381638 scikit-rmt-0.7.0/setup.cfg
--rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.7.0/setup.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.352389 scikit-rmt-0.7.0/skrmt/
--rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.7.0/skrmt/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)       49 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/_version.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.357121 scikit-rmt-0.7.0/skrmt/covariance/
--rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.7.0/skrmt/covariance/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.7.0/skrmt/covariance/estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.7.0/skrmt/covariance/metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.359991 scikit-rmt-0.7.0/skrmt/covariance/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.7.0/skrmt/covariance/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.7.0/skrmt/covariance/tests/test_estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.7.0/skrmt/covariance/tests/test_metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.366985 scikit-rmt-0.7.0/skrmt/ensemble/
--rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/skrmt/ensemble/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10728 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/_base_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13872 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    15308 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    14125 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    56446 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/spectral_law.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.376211 scikit-rmt-0.7.0/skrmt/ensemble/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     1936 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_base_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_circular_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    12191 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_gaussian_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_manova_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    42454 2023-07-06 19:27:12.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_spectral_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
--rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tridiagonalization.py
--rw-r--r--   0 santorum   (501) staff       (20)    14730 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_wishart_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.7.0/skrmt/ensemble/tracy_widom_approximator.py
--rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.7.0/skrmt/ensemble/tridiagonal_utils.py
--rw-r--r--   0 santorum   (501) staff       (20)    17113 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/wishart_ensemble.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.380142 scikit-rmt-0.7.0/tutorial/
--rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.7.0/tutorial/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2689 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/tutorial/plot_0_introduction.py
--rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/tutorial/plot_1_spectral_laws.py
--rw-r--r--   0 santorum   (501) staff       (20)     9183 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/tutorial/plot_2_plot_spectral_laws.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.418631 scikit-rmt-0.7.1/
+-rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.7.1/.coveragerc
+-rw-r--r--   0 santorum   (501) staff       (20)      278 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/.travis.yml
+-rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.7.1/CITATION.cff
+-rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.7.1/LICENSE
+-rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.7.1/MANIFEST.in
+-rw-r--r--   0 santorum   (501) staff       (20)     2569 2023-07-08 22:52:37.000000 scikit-rmt-0.7.1/Makefile
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-14 20:29:18.419343 scikit-rmt-0.7.1/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/README.md
+-rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.7.1/conf.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.246593 scikit-rmt-0.7.1/docs/
+-rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.7.1/docs/modules.rst
+-rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.7.1/docs/readthedocs-requirements.txt
+-rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.7.1/docs/skrmt.covariance.rst
+-rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/docs/skrmt.ensemble.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.7.1/docs/skrmt.rst
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.255340 scikit-rmt-0.7.1/examples/
+-rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.7.1/examples/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2155 2023-07-08 20:47:44.000000 scikit-rmt-0.7.1/examples/plot_boosting_density_representation.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.7.1/examples/plot_circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.7.1/examples/plot_complex_histograms.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.7.1/examples/plot_gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.7.1/examples/plot_manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.7.1/examples/plot_wishart_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.7.1/index.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.7.1/readthedocs.yml
+-rw-r--r--   0 santorum   (501) staff       (20)       65 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/requirements.txt
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.274690 scikit-rmt-0.7.1/scikit_rmt.egg-info/
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/SOURCES.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        1 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/dependency_links.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       66 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/requires.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        6 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/top_level.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       38 2023-07-14 20:29:18.420190 scikit-rmt-0.7.1/setup.cfg
+-rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.7.1/setup.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.281512 scikit-rmt-0.7.1/skrmt/
+-rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.7.1/skrmt/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)       49 2023-07-14 20:17:58.000000 scikit-rmt-0.7.1/skrmt/_version.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.284218 scikit-rmt-0.7.1/skrmt/covariance/
+-rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.7.1/skrmt/covariance/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.7.1/skrmt/covariance/estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.7.1/skrmt/covariance/metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.287503 scikit-rmt-0.7.1/skrmt/covariance/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.7.1/skrmt/covariance/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.7.1/skrmt/covariance/tests/test_estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.7.1/skrmt/covariance/tests/test_metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.374422 scikit-rmt-0.7.1/skrmt/ensemble/
+-rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/skrmt/ensemble/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10728 2023-07-13 20:47:52.000000 scikit-rmt-0.7.1/skrmt/ensemble/_base_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13872 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    15829 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14125 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    56473 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/spectral_law.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.413581 scikit-rmt-0.7.1/skrmt/ensemble/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1936 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_base_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_circular_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    11990 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_gaussian_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_manova_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    42454 2023-07-06 19:27:12.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_spectral_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tracy_widom_approx.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tridiagonalization.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14730 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_wishart_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.7.1/skrmt/ensemble/tracy_widom_approximator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.7.1/skrmt/ensemble/tridiagonal_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    17231 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/wishart_ensemble.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.417897 scikit-rmt-0.7.1/tutorial/
+-rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.7.1/tutorial/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2689 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/tutorial/plot_0_introduction.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/tutorial/plot_1_spectral_laws.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9183 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.7.0/LICENSE` & `scikit-rmt-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/Makefile` & `scikit-rmt-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/PKG-INFO` & `scikit-rmt-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.7.0
+Version: 0.7.1
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.0.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.1.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
```

### Comparing `scikit-rmt-0.7.0/README.md` & `scikit-rmt-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/conf.py` & `scikit-rmt-0.7.1/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/docs/skrmt.covariance.rst` & `scikit-rmt-0.7.1/docs/skrmt.covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/docs/skrmt.ensemble.rst` & `scikit-rmt-0.7.1/docs/skrmt.ensemble.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/examples/plot_boosting_density_representation.py` & `scikit-rmt-0.7.1/examples/plot_boosting_density_representation.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/examples/plot_circular_ensemble.py` & `scikit-rmt-0.7.1/examples/plot_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/examples/plot_complex_histograms.py` & `scikit-rmt-0.7.1/examples/plot_complex_histograms.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/examples/plot_gaussian_ensemble.py` & `scikit-rmt-0.7.1/examples/plot_gaussian_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/examples/plot_manova_ensemble.py` & `scikit-rmt-0.7.1/examples/plot_manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/examples/plot_wishart_ensemble.py` & `scikit-rmt-0.7.1/examples/plot_wishart_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/index.rst` & `scikit-rmt-0.7.1/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/scikit_rmt.egg-info/PKG-INFO` & `scikit-rmt-0.7.1/scikit_rmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.7.0
+Version: 0.7.1
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.0.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.1.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
```

### Comparing `scikit-rmt-0.7.0/scikit_rmt.egg-info/SOURCES.txt` & `scikit-rmt-0.7.1/scikit_rmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/setup.py` & `scikit-rmt-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/covariance/__init__.py` & `scikit-rmt-0.7.1/skrmt/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/covariance/estimator.py` & `scikit-rmt-0.7.1/skrmt/covariance/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/covariance/metrics.py` & `scikit-rmt-0.7.1/skrmt/covariance/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/covariance/tests/test_estimator.py` & `scikit-rmt-0.7.1/skrmt/covariance/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/covariance/tests/test_metrics.py` & `scikit-rmt-0.7.1/skrmt/covariance/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/__init__.py` & `scikit-rmt-0.7.1/skrmt/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/_base_ensemble.py` & `scikit-rmt-0.7.1/skrmt/ensemble/_base_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/circular_ensemble.py` & `scikit-rmt-0.7.1/skrmt/ensemble/circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/gaussian_ensemble.py` & `scikit-rmt-0.7.1/skrmt/ensemble/gaussian_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,22 +83,27 @@
 
         super().__init__()
         # pylint: disable=invalid-name
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
         self.sigma = sigma
+        self.radius = 2 * np.sqrt(self.beta) * self.sigma
         self._eigvals = None
         self.matrix = self.sample()
 
         # default eigenvalue normalization constant
-        if self.use_tridiagonal:
-            self.eigval_norm_const = 1/np.sqrt(self.n) if self.beta==4 else 1/np.sqrt(self.n/2)
-        else:
-            self.eigval_norm_const = 1/np.sqrt(self.n)
+        self.eigval_norm_const = 1/np.sqrt(2*self.n) if self.beta==4 else 1/np.sqrt(self.n)
+
+        # non-normalized semicircle interval (keys are betas)
+        self._non_normalized_interval = {
+            1: (-2*np.sqrt(self.n), 2*np.sqrt(self.n)),
+            2: (-2*np.sqrt(2*self.n), 2*np.sqrt(2*self.n)),
+            4: (-4*np.sqrt(2*self.n), 4*np.sqrt(2*self.n)),
+        }
 
 
     def set_size(self, n, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
@@ -169,15 +174,16 @@
         y_mtx = np.random.randn(size,size)*self.sigma + 1j*np.random.randn(size,size)*self.sigma
         # [X Y; -conj(Y) conj(X)]
         mtx = np.block([
                        [x_mtx               , y_mtx],
                        [-np.conjugate(y_mtx), np.conjugate(x_mtx)]
                         ])
         # hermitian matrix
-        self.matrix = (mtx + mtx.transpose().conj())/np.sqrt(2)
+        # Before: self.matrix = (mtx + mtx.transpose().conj())/np.sqrt(2)
+        self.matrix = (mtx + mtx.transpose().conj())
         # setting array of eigenvalues to None to force re-computing them
         self._eigvals = None
         return self.matrix
 
     def sample_tridiagonal(self):
         '''Samples a Gaussian Ensemble random matrix in its tridiagonal form.
 
@@ -199,19 +205,21 @@
         if self.sigma != 1.0:
             raise ValueError("Error: cannot sample tridiagonal random matrix using non-unitary scale"
                              f" (sigma = {self.sigma}).\n"
                              "\t Set `sigma=1.0` (default) or deactivate tridiagonal sampling.")
 
         size = 2*self.n if self.beta==4 else self.n
         # sampling diagonal normals
-        normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=size)
+        # normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=size)
+        normals = np.random.normal(loc=0, scale=1, size=size)
         # sampling chi-squares
         dfs = np.flip(np.arange(1, size))
-        chisqs = (1/np.sqrt(2)) * \
-                 np.array([np.sqrt(np.random.chisquare(df*self.beta)) for df in dfs])
+        # chisqs = (1/np.sqrt(2)) * \
+        #          np.array([np.sqrt(np.random.chisquare(df*self.beta)) for df in dfs])
+        chisqs = np.array([np.sqrt(np.random.chisquare(df*self.beta)) for df in dfs])
         # inserting diagonals
         diagonals = [chisqs, normals, chisqs]
         mtx = sparse.diags(diagonals, [-1, 0, 1])
         # converting to numpy array
         self.matrix = mtx.toarray()
         # setting array of eigenvalues to None to force re-computing them
         self._eigvals = None
@@ -283,16 +291,18 @@
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         if interval is None:
-            wsl_radius = 2*np.sqrt(self.beta)*self.sigma
-            interval = (-wsl_radius, wsl_radius)
+            if normalize:
+                interval = (-self.radius, self.radius)
+            else:
+                interval = self._non_normalized_interval[self.beta]
 
         if self.use_tridiagonal:
             # pylint: disable=too-many-arguments
             observed, bins = self.eigval_hist(
                 bins=bins, interval=interval, density=density, normalize=normalize
             )
```

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/manova_ensemble.py` & `scikit-rmt-0.7.1/skrmt/ensemble/manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/spectral_law.py` & `scikit-rmt-0.7.1/skrmt/ensemble/spectral_law.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
         """
         # pylint: disable=too-many-arguments
         if n_size<1:
             raise ValueError("matrix size must be positive")
         
         if interval is None:
-            interval = (-self.radius, self.radius)
+            interval = (self.center - self.radius, self.center + self.radius)
 
         random_samples = self.rvs(size=n_size)
         observed, bins = np.histogram(random_samples, bins=bins, range=interval, density=density)
 
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
```

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_base_ens.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_base_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_circular_ens.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_circular_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_gaussian_ens.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_gaussian_ens.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     n_size = 5
     beta = 1
 
     np.random.seed(1)
     goe = GaussianEnsemble(beta=1, n=n_size, use_tridiagonal=True)
 
     np.random.seed(1)
-    normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=n_size)
+    normals = np.random.normal(loc=0, scale=1, size=n_size)
     dfs = np.flip(np.arange(1, n_size))
-    chisqs = (1/np.sqrt(2)) * np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
+    chisqs = np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
 
     for i in range(n_size):
         assert normals[i] == goe.matrix[i][i]
     for i in range(n_size-1):
         assert chisqs[i] == goe.matrix[i][i+1]
         assert chisqs[i] == goe.matrix[i+1][i]
 
@@ -213,17 +213,17 @@
     n_size = 5
     beta = 2
 
     np.random.seed(1)
     gue = GaussianEnsemble(beta=2, n=n_size, use_tridiagonal=True)
 
     np.random.seed(1)
-    normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=n_size)
+    normals = np.random.normal(loc=0, scale=1, size=n_size)
     dfs = np.flip(np.arange(1, n_size))
-    chisqs = (1/np.sqrt(2)) * np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
+    chisqs = np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
 
     for i in range(n_size):
         assert normals[i] == gue.matrix[i][i]
     for i in range(n_size-1):
         assert chisqs[i] == gue.matrix[i][i+1]
         assert chisqs[i] == gue.matrix[i+1][i]
 
@@ -268,24 +268,22 @@
     '''
     n_size = 2
     np.random.seed(1)
     gse = GaussianEnsemble(beta=4, n=n_size)
 
     assert gse.matrix.shape == (2*n_size,2*n_size)
 
-    mtx_sol = [[2.29717124+0.j, -0.80605094-2.86120185j,\
-                0.+0.j, -1.21019792-1.0732635j],
-               [-0.80605094+2.86120185j, -1.51740678+0.j,\
-                1.21019792+1.0732635j, 0.+0.j],
-               [0.+0.j, 1.21019792-1.0732635j,\
-                2.29717124+0.j, -0.80605094+2.86120185j],
-               [-1.21019792+1.0732635j, 0.+0.j,\
-                -0.80605094-2.86120185j, -1.51740678+0.j]]
+    mtx_sol = [
+        [3.24869073+0.j, -1.13992817-4.04635046j, 0.+0.j, -1.71147831-1.5178238j],
+        [-1.13992817+4.04635046j, -2.14593724+0.j, 1.71147831+1.5178238j, 0.+0.j],
+        [0.+0.j, 1.71147831-1.5178238j, 3.24869073+0.j, -1.13992817+4.04635046j],
+        [-1.71147831+1.5178238j, 0.+0.j, -1.13992817-4.04635046j, -2.14593724+0.j],
+    ]
 
-    assert_almost_equal(gse.matrix, np.array(mtx_sol),
+    assert_almost_equal(gse.matrix, np.asarray(mtx_sol),
                         decimal=4)
 
 
 def test_gse_hermitian():
     '''Testing that GSE matrix is hermitian
     '''
     n_size = 5
@@ -321,17 +319,17 @@
     beta = 4
 
     np.random.seed(1)
     gse = GaussianEnsemble(beta=4, n=n_size, use_tridiagonal=True)
 
     np.random.seed(1)
     n_size *= 2  # WQE matrices are 2p times 2p
-    normals = (1/np.sqrt(2)) * np.random.normal(loc=0, scale=np.sqrt(2), size=n_size)
+    normals = np.random.normal(loc=0, scale=1, size=n_size)
     dfs = np.flip(np.arange(1, n_size))
-    chisqs = (1/np.sqrt(2)) * np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
+    chisqs = np.array([np.sqrt(np.random.chisquare(df*beta)) for df in dfs])
 
     for i in range(n_size):
         assert normals[i] == gse.matrix[i][i]
     for i in range(n_size-1):
         assert chisqs[i] == gse.matrix[i][i+1]
         assert chisqs[i] == gse.matrix[i+1][i]
```

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_manova_ens.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_manova_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_spectral_law.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_spectral_law.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tracy_widom_approx.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tracy_widom_approx.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tridiagonalization.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tridiagonalization.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_wishart_ens.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_wishart_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tracy_widom_approximator.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tracy_widom_approximator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/tridiagonal_utils.py` & `scikit-rmt-0.7.1/skrmt/ensemble/tridiagonal_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/skrmt/ensemble/wishart_ensemble.py` & `scikit-rmt-0.7.1/skrmt/ensemble/wishart_ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,21 @@
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
         self.sigma = sigma
         self._eigvals = None
         self.matrix = self.sample()
         # default eigenvalue normalization constant
         self.eigval_norm_const = 1/self.n
+        self._compute_parameters()
+
+    def _compute_parameters(self):
+        # calculating constants depending on matrix sizes
+        self.ratio = self.p/self.n
+        self.lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(self.ratio))**2
+        self.lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(self.ratio))**2
 
     def set_size(self, p, n, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
@@ -114,14 +121,15 @@
                 the matrix of the corresponding ensemble.
             resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
 
         """
         self.p = p
         self.n = n
+        self._compute_parameters()
         if resample_mtx:
             self.matrix = self.sample()
 
     # pylint: disable=inconsistent-return-statements
     def sample(self):
         """Samples new Wishart Ensemble random matrix.
 
@@ -302,24 +310,20 @@
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
-        if not normalize:
-            print("Warning: setting normalize=False may cause normal instability and/or rounding errors.")
-
         # pylint: disable=too-many-arguments
         if interval is None:
-            # calculating constants depending on matrix sizes
-            ratio = self.p/self.n
-            lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(ratio))**2
-            lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(ratio))**2
-            interval = (lambda_minus, lambda_plus)
+            if normalize:
+                interval = (self.lambda_minus, self.lambda_plus)
+            else:
+                interval = (self.n*self.lambda_minus, self.n*self.lambda_plus)
 
         if self.use_tridiagonal:
             observed, bins = self.eigval_hist(
                 bins=bins, interval=interval, density=density, normalize=normalize
             )
 
             width = bins[1]-bins[0]
```

### Comparing `scikit-rmt-0.7.0/tutorial/plot_0_introduction.py` & `scikit-rmt-0.7.1/tutorial/plot_0_introduction.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/tutorial/plot_1_spectral_laws.py` & `scikit-rmt-0.7.1/tutorial/plot_1_spectral_laws.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.0/tutorial/plot_2_plot_spectral_laws.py` & `scikit-rmt-0.7.1/tutorial/plot_2_plot_spectral_laws.py`

 * *Files identical despite different names*

